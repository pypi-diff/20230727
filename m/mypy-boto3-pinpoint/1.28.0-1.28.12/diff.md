# Comparing `tmp/mypy-boto3-pinpoint-1.28.0.tar.gz` & `tmp/mypy-boto3-pinpoint-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pinpoint-1.28.0.tar", last modified: Thu Jul  6 21:00:19 2023, max compression
+gzip compressed data, was "mypy-boto3-pinpoint-1.28.12.tar", last modified: Thu Jul 27 11:49:24 2023, max compression
```

## Comparing `mypy-boto3-pinpoint-1.28.0.tar` & `mypy-boto3-pinpoint-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:19.230394 mypy-boto3-pinpoint-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:49:23.000000 mypy-boto3-pinpoint-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29046 2023-07-06 21:00:19.230394 mypy-boto3-pinpoint-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27557 2023-07-06 20:49:23.000000 mypy-boto3-pinpoint-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:19.230394 mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-06 20:49:23.000000 mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-06 20:49:23.000000 mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:49:23.000000 mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79752 2023-07-06 20:49:24.000000 mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    79624 2023-07-06 20:49:23.000000 mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-07-06 20:49:24.000000 mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10818 2023-07-06 20:49:24.000000 mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:49:23.000000 mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   159276 2023-07-06 20:49:31.000000 mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   159059 2023-07-06 20:49:26.000000 mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:49:23.000000 mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:19.230394 mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29046 2023-07-06 21:00:19.000000 mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-06 21:00:19.000000 mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:19.000000 mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:19.000000 mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:19.000000 mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:00:19.000000 mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:19.230394 mypy-boto3-pinpoint-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:49:23.000000 mypy-boto3-pinpoint-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.893162 mypy-boto3-pinpoint-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:26.000000 mypy-boto3-pinpoint-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    31664 2023-07-27 11:49:24.893162 mypy-boto3-pinpoint-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30173 2023-07-27 11:41:26.000000 mypy-boto3-pinpoint-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.885162 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-27 11:41:26.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-27 11:41:26.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:41:26.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79752 2023-07-27 11:41:27.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79624 2023-07-27 11:41:27.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-07-27 11:41:27.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-07-27 11:41:27.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:26.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   182450 2023-07-27 11:41:33.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182215 2023-07-27 11:41:30.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:26.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.893162 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    31664 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:24.893162 mypy-boto3-pinpoint-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:41:26.000000 mypy-boto3-pinpoint-1.28.12/setup.py
```

### Comparing `mypy-boto3-pinpoint-1.28.0/LICENSE` & `mypy-boto3-pinpoint-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.28.0/PKG-INFO` & `mypy-boto3-pinpoint-1.28.12/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-pinpoint
-Version: 1.28.0
-Summary: Type annotations for boto3.Pinpoint 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 pinpoint type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-pinpoint"></a>
 
 # mypy-boto3-pinpoint
 
 [![PyPI - mypy-boto3-pinpoint](https://img.shields.io/pypi/v/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint)](https://pepy.tech/project/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
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
 [mypy-boto3-pinpoint docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,57 +297,74 @@
 from mypy_boto3_pinpoint.type_defs import (
     ADMChannelRequestTypeDef,
     ADMChannelResponseTypeDef,
     ADMMessageTypeDef,
     APNSChannelRequestTypeDef,
     APNSChannelResponseTypeDef,
     APNSMessageTypeDef,
+    APNSPushNotificationTemplateOutputTypeDef,
     APNSPushNotificationTemplateTypeDef,
     APNSSandboxChannelRequestTypeDef,
     APNSSandboxChannelResponseTypeDef,
     APNSVoipChannelRequestTypeDef,
     APNSVoipChannelResponseTypeDef,
     APNSVoipSandboxChannelRequestTypeDef,
     APNSVoipSandboxChannelResponseTypeDef,
     ActivityResponseTypeDef,
+    ContactCenterActivityOutputTypeDef,
+    HoldoutActivityOutputTypeDef,
     ContactCenterActivityTypeDef,
     HoldoutActivityTypeDef,
     AddressConfigurationTypeDef,
+    AndroidPushNotificationTemplateOutputTypeDef,
     AndroidPushNotificationTemplateTypeDef,
     ApplicationResponseTypeDef,
-    CampaignHookTypeDef,
-    CampaignLimitsTypeDef,
-    QuietTimeTypeDef,
+    CampaignHookOutputTypeDef,
+    CampaignLimitsOutputTypeDef,
+    QuietTimeOutputTypeDef,
+    AttributeDimensionOutputTypeDef,
     AttributeDimensionTypeDef,
     AttributesResourceTypeDef,
     BaiduChannelRequestTypeDef,
     BaiduChannelResponseTypeDef,
     BaiduMessageTypeDef,
+    CampaignCustomMessageOutputTypeDef,
     CampaignCustomMessageTypeDef,
+    CampaignEmailMessageOutputTypeDef,
     CampaignEmailMessageTypeDef,
+    CampaignHookTypeDef,
+    CampaignLimitsTypeDef,
     CampaignStateTypeDef,
-    CustomDeliveryConfigurationTypeDef,
+    CustomDeliveryConfigurationOutputTypeDef,
+    CampaignSmsMessageOutputTypeDef,
     CampaignSmsMessageTypeDef,
     ChannelResponseTypeDef,
+    ClosedDaysRuleOutputTypeDef,
     ClosedDaysRuleTypeDef,
+    WaitTimeOutputTypeDef,
     WaitTimeTypeDef,
     CreateApplicationRequestTypeDef,
+    ResponseMetadataTypeDef,
     EmailTemplateRequestTypeDef,
     CreateTemplateMessageBodyTypeDef,
     ExportJobRequestTypeDef,
     ImportJobRequestTypeDef,
     TemplateCreateMessageBodyTypeDef,
     CreateRecommenderConfigurationTypeDef,
     RecommenderConfigurationResponseTypeDef,
     SMSTemplateRequestTypeDef,
     VoiceTemplateRequestTypeDef,
+    CustomDeliveryConfigurationTypeDef,
+    JourneyCustomMessageOutputTypeDef,
     JourneyCustomMessageTypeDef,
+    DefaultButtonConfigurationOutputTypeDef,
     DefaultButtonConfigurationTypeDef,
     DefaultMessageTypeDef,
     DefaultPushNotificationMessageTypeDef,
+    DefaultPushNotificationTemplateOutputTypeDef,
     DefaultPushNotificationTemplateTypeDef,
     DeleteAdmChannelRequestRequestTypeDef,
     DeleteApnsChannelRequestRequestTypeDef,
     DeleteApnsSandboxChannelRequestRequestTypeDef,
     DeleteApnsVoipChannelRequestRequestTypeDef,
     DeleteApnsVoipSandboxChannelRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
@@ -406,30 +391,36 @@
     DeleteVoiceChannelRequestRequestTypeDef,
     VoiceChannelResponseTypeDef,
     DeleteVoiceTemplateRequestRequestTypeDef,
     GCMMessageTypeDef,
     SMSMessageTypeDef,
     VoiceMessageTypeDef,
     EmailChannelRequestTypeDef,
+    JourneyEmailMessageOutputTypeDef,
     JourneyEmailMessageTypeDef,
     RawEmailTypeDef,
     EmailTemplateResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     EndpointDemographicTypeDef,
     EndpointLocationTypeDef,
     EndpointUserTypeDef,
+    EndpointDemographicOutputTypeDef,
     EndpointItemResponseTypeDef,
+    EndpointLocationOutputTypeDef,
     EndpointMessageResultTypeDef,
+    EndpointUserOutputTypeDef,
     EndpointSendConfigurationTypeDef,
+    MetricDimensionOutputTypeDef,
+    SetDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     SetDimensionTypeDef,
     EventItemResponseTypeDef,
     SessionTypeDef,
     ExportJobResourceTypeDef,
     GCMChannelRequestTypeDef,
+    GPSCoordinatesOutputTypeDef,
     GPSCoordinatesTypeDef,
     GetAdmChannelRequestRequestTypeDef,
     GetApnsChannelRequestRequestTypeDef,
     GetApnsSandboxChannelRequestRequestTypeDef,
     GetApnsVoipChannelRequestRequestTypeDef,
     GetApnsVoipSandboxChannelRequestRequestTypeDef,
     GetAppRequestRequestTypeDef,
@@ -479,91 +470,109 @@
     GetSmsTemplateRequestRequestTypeDef,
     SMSTemplateResponseTypeDef,
     GetUserEndpointsRequestRequestTypeDef,
     GetVoiceChannelRequestRequestTypeDef,
     GetVoiceTemplateRequestRequestTypeDef,
     VoiceTemplateResponseTypeDef,
     ImportJobResourceTypeDef,
+    InAppMessageBodyConfigOutputTypeDef,
     InAppMessageBodyConfigTypeDef,
+    OverrideButtonConfigurationOutputTypeDef,
     OverrideButtonConfigurationTypeDef,
+    InAppMessageHeaderConfigOutputTypeDef,
     InAppMessageHeaderConfigTypeDef,
+    JourneyChannelSettingsOutputTypeDef,
     JourneyChannelSettingsTypeDef,
+    JourneyLimitsOutputTypeDef,
     JourneyLimitsTypeDef,
+    JourneyPushMessageOutputTypeDef,
     JourneyPushMessageTypeDef,
-    JourneyScheduleTypeDef,
+    JourneyScheduleOutputTypeDef,
     JourneyRunResponseTypeDef,
+    JourneySMSMessageOutputTypeDef,
     JourneySMSMessageTypeDef,
+    JourneyScheduleTypeDef,
     JourneyStateRequestTypeDef,
     ListJourneysRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagsModelTypeDef,
+    TagsModelOutputTypeDef,
     ListTemplateVersionsRequestRequestTypeDef,
     ListTemplatesRequestRequestTypeDef,
+    MessageOutputTypeDef,
     MessageTypeDef,
     MessageResultTypeDef,
     NumberValidateRequestTypeDef,
     NumberValidateResponseTypeDef,
+    OpenHoursRuleOutputTypeDef,
     OpenHoursRuleTypeDef,
     WriteEventStreamTypeDef,
+    QuietTimeTypeDef,
+    RandomSplitEntryOutputTypeDef,
     RandomSplitEntryTypeDef,
+    RecencyDimensionOutputTypeDef,
     RecencyDimensionTypeDef,
     UpdateAttributesRequestTypeDef,
-    ResponseMetadataTypeDef,
     ResultRowValueTypeDef,
     SMSChannelRequestTypeDef,
+    SegmentConditionOutputTypeDef,
     SegmentConditionTypeDef,
+    SegmentReferenceOutputTypeDef,
     SegmentReferenceTypeDef,
     SegmentImportResourceTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SimpleEmailPartTypeDef,
+    TagsModelTypeDef,
     TemplateActiveVersionRequestTypeDef,
+    TemplateOutputTypeDef,
     TemplateTypeDef,
     TemplateResponseTypeDef,
     TemplateVersionResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRecommenderConfigurationTypeDef,
     VoiceChannelRequestTypeDef,
     VerificationResponseTypeDef,
     VerifyOTPMessageRequestParametersTypeDef,
     UpdateAdmChannelRequestRequestTypeDef,
-    DeleteAdmChannelResponseTypeDef,
-    GetAdmChannelResponseTypeDef,
-    UpdateAdmChannelResponseTypeDef,
     UpdateApnsChannelRequestRequestTypeDef,
-    DeleteApnsChannelResponseTypeDef,
-    GetApnsChannelResponseTypeDef,
-    UpdateApnsChannelResponseTypeDef,
     UpdateApnsSandboxChannelRequestRequestTypeDef,
-    DeleteApnsSandboxChannelResponseTypeDef,
-    GetApnsSandboxChannelResponseTypeDef,
-    UpdateApnsSandboxChannelResponseTypeDef,
     UpdateApnsVoipChannelRequestRequestTypeDef,
-    DeleteApnsVoipChannelResponseTypeDef,
-    GetApnsVoipChannelResponseTypeDef,
-    UpdateApnsVoipChannelResponseTypeDef,
     UpdateApnsVoipSandboxChannelRequestRequestTypeDef,
-    DeleteApnsVoipSandboxChannelResponseTypeDef,
-    GetApnsVoipSandboxChannelResponseTypeDef,
-    UpdateApnsVoipSandboxChannelResponseTypeDef,
     ActivitiesResponseTypeDef,
     ApplicationsResponseTypeDef,
-    CreateAppResponseTypeDef,
-    DeleteAppResponseTypeDef,
-    GetAppResponseTypeDef,
     ApplicationSettingsResourceTypeDef,
-    WriteApplicationSettingsRequestTypeDef,
-    RemoveAttributesResponseTypeDef,
     UpdateBaiduChannelRequestRequestTypeDef,
-    DeleteBaiduChannelResponseTypeDef,
-    GetBaiduChannelResponseTypeDef,
-    UpdateBaiduChannelResponseTypeDef,
     ChannelsResponseTypeDef,
+    ClosedDaysOutputTypeDef,
     ClosedDaysTypeDef,
+    WaitActivityOutputTypeDef,
     WaitActivityTypeDef,
     CreateAppRequestRequestTypeDef,
+    CreateAppResponseTypeDef,
+    DeleteAdmChannelResponseTypeDef,
+    DeleteApnsChannelResponseTypeDef,
+    DeleteApnsSandboxChannelResponseTypeDef,
+    DeleteApnsVoipChannelResponseTypeDef,
+    DeleteApnsVoipSandboxChannelResponseTypeDef,
+    DeleteAppResponseTypeDef,
+    DeleteBaiduChannelResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAdmChannelResponseTypeDef,
+    GetApnsChannelResponseTypeDef,
+    GetApnsSandboxChannelResponseTypeDef,
+    GetApnsVoipChannelResponseTypeDef,
+    GetApnsVoipSandboxChannelResponseTypeDef,
+    GetAppResponseTypeDef,
+    GetBaiduChannelResponseTypeDef,
+    RemoveAttributesResponseTypeDef,
+    UpdateAdmChannelResponseTypeDef,
+    UpdateApnsChannelResponseTypeDef,
+    UpdateApnsSandboxChannelResponseTypeDef,
+    UpdateApnsVoipChannelResponseTypeDef,
+    UpdateApnsVoipSandboxChannelResponseTypeDef,
+    UpdateBaiduChannelResponseTypeDef,
     CreateEmailTemplateRequestRequestTypeDef,
     UpdateEmailTemplateRequestRequestTypeDef,
     CreateEmailTemplateResponseTypeDef,
     CreatePushTemplateResponseTypeDef,
     CreateSmsTemplateResponseTypeDef,
     CreateVoiceTemplateResponseTypeDef,
     CreateExportJobRequestRequestTypeDef,
@@ -575,17 +584,18 @@
     GetRecommenderConfigurationResponseTypeDef,
     ListRecommenderConfigurationsResponseTypeDef,
     UpdateRecommenderConfigurationResponseTypeDef,
     CreateSmsTemplateRequestRequestTypeDef,
     UpdateSmsTemplateRequestRequestTypeDef,
     CreateVoiceTemplateRequestRequestTypeDef,
     UpdateVoiceTemplateRequestRequestTypeDef,
+    CustomMessageActivityOutputTypeDef,
     CustomMessageActivityTypeDef,
-    PushNotificationTemplateRequestTypeDef,
     PushNotificationTemplateResponseTypeDef,
+    PushNotificationTemplateRequestTypeDef,
     DeleteEmailChannelResponseTypeDef,
     GetEmailChannelResponseTypeDef,
     UpdateEmailChannelResponseTypeDef,
     DeleteEmailTemplateResponseTypeDef,
     DeleteInAppTemplateResponseTypeDef,
     DeletePushTemplateResponseTypeDef,
     DeleteSmsTemplateResponseTypeDef,
@@ -607,154 +617,185 @@
     DeleteSmsChannelResponseTypeDef,
     GetSmsChannelResponseTypeDef,
     UpdateSmsChannelResponseTypeDef,
     DeleteVoiceChannelResponseTypeDef,
     GetVoiceChannelResponseTypeDef,
     UpdateVoiceChannelResponseTypeDef,
     UpdateEmailChannelRequestRequestTypeDef,
+    EmailMessageActivityOutputTypeDef,
     EmailMessageActivityTypeDef,
     GetEmailTemplateResponseTypeDef,
     EndpointBatchItemTypeDef,
     EndpointRequestTypeDef,
-    EndpointResponseTypeDef,
     PublicEndpointTypeDef,
     SendUsersMessageResponseTypeDef,
+    EndpointResponseTypeDef,
+    EventDimensionsOutputTypeDef,
+    SegmentDemographicsOutputTypeDef,
     EventDimensionsTypeDef,
     SegmentDemographicsTypeDef,
     ItemResponseTypeDef,
     EventTypeDef,
     ExportJobResponseTypeDef,
     UpdateGcmChannelRequestRequestTypeDef,
+    GPSPointDimensionOutputTypeDef,
     GPSPointDimensionTypeDef,
     GetJourneyExecutionActivityMetricsResponseTypeDef,
     GetJourneyExecutionMetricsResponseTypeDef,
     GetJourneyRunExecutionActivityMetricsResponseTypeDef,
     GetJourneyRunExecutionMetricsResponseTypeDef,
     GetSmsTemplateResponseTypeDef,
     GetVoiceTemplateResponseTypeDef,
     ImportJobResponseTypeDef,
+    InAppMessageButtonOutputTypeDef,
     InAppMessageButtonTypeDef,
+    PushMessageActivityOutputTypeDef,
     PushMessageActivityTypeDef,
     JourneyRunsResponseTypeDef,
+    SMSMessageActivityOutputTypeDef,
     SMSMessageActivityTypeDef,
     UpdateJourneyStateRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     MessageResponseTypeDef,
     PhoneNumberValidateRequestRequestTypeDef,
     PhoneNumberValidateResponseTypeDef,
+    OpenHoursOutputTypeDef,
     OpenHoursTypeDef,
     PutEventStreamRequestRequestTypeDef,
+    WriteApplicationSettingsRequestTypeDef,
+    RandomSplitActivityOutputTypeDef,
     RandomSplitActivityTypeDef,
+    SegmentBehaviorsOutputTypeDef,
     SegmentBehaviorsTypeDef,
     RemoveAttributesRequestRequestTypeDef,
     ResultRowTypeDef,
     UpdateSmsChannelRequestRequestTypeDef,
     SendOTPMessageRequestRequestTypeDef,
     SimpleEmailTypeDef,
+    TagResourceRequestRequestTypeDef,
     UpdateTemplateActiveVersionRequestRequestTypeDef,
+    TemplateConfigurationOutputTypeDef,
     TemplateConfigurationTypeDef,
     TemplatesResponseTypeDef,
     TemplateVersionsResponseTypeDef,
     UpdateRecommenderConfigurationRequestRequestTypeDef,
     UpdateVoiceChannelRequestRequestTypeDef,
     VerifyOTPMessageResponseTypeDef,
     VerifyOTPMessageRequestRequestTypeDef,
     GetCampaignActivitiesResponseTypeDef,
     GetAppsResponseTypeDef,
     GetApplicationSettingsResponseTypeDef,
     UpdateApplicationSettingsResponseTypeDef,
-    UpdateApplicationSettingsRequestRequestTypeDef,
     GetChannelsResponseTypeDef,
     GetRecommenderConfigurationsResponseTypeDef,
+    GetPushTemplateResponseTypeDef,
     CreatePushTemplateRequestRequestTypeDef,
     UpdatePushTemplateRequestRequestTypeDef,
-    GetPushTemplateResponseTypeDef,
     EndpointBatchRequestTypeDef,
     UpdateEndpointRequestRequestTypeDef,
+    SendUsersMessagesResponseTypeDef,
     DeleteEndpointResponseTypeDef,
     EndpointsResponseTypeDef,
     GetEndpointResponseTypeDef,
-    SendUsersMessagesResponseTypeDef,
+    CampaignEventFilterOutputTypeDef,
+    EventConditionOutputTypeDef,
+    EventFilterOutputTypeDef,
     CampaignEventFilterTypeDef,
     EventConditionTypeDef,
     EventFilterTypeDef,
     EventsResponseTypeDef,
     EventsBatchTypeDef,
     CreateExportJobResponseTypeDef,
     ExportJobsResponseTypeDef,
     GetExportJobResponseTypeDef,
+    SegmentLocationOutputTypeDef,
     SegmentLocationTypeDef,
     CreateImportJobResponseTypeDef,
     GetImportJobResponseTypeDef,
     ImportJobsResponseTypeDef,
+    InAppMessageContentOutputTypeDef,
     InAppMessageContentTypeDef,
     GetJourneyRunsResponseTypeDef,
     SendMessagesResponseTypeDef,
     SendOTPMessageResponseTypeDef,
+    UpdateApplicationSettingsRequestRequestTypeDef,
     BaseKpiResultTypeDef,
     EmailMessageTypeDef,
     ListTemplatesResponseTypeDef,
     ListTemplateVersionsResponseTypeDef,
     UpdateEndpointsBatchRequestRequestTypeDef,
     DeleteUserEndpointsResponseTypeDef,
     GetUserEndpointsResponseTypeDef,
     InAppCampaignScheduleTypeDef,
+    ScheduleOutputTypeDef,
+    EventStartConditionOutputTypeDef,
     ScheduleTypeDef,
     EventStartConditionTypeDef,
     PutEventsResponseTypeDef,
     EventsRequestTypeDef,
     GetExportJobsResponseTypeDef,
     GetSegmentExportJobsResponseTypeDef,
+    SegmentDimensionsOutputTypeDef,
     SegmentDimensionsTypeDef,
     GetImportJobsResponseTypeDef,
     GetSegmentImportJobsResponseTypeDef,
-    CampaignInAppMessageTypeDef,
+    CampaignInAppMessageOutputTypeDef,
     InAppMessageTypeDef,
-    InAppTemplateRequestTypeDef,
     InAppTemplateResponseTypeDef,
+    CampaignInAppMessageTypeDef,
+    InAppTemplateRequestTypeDef,
     ApplicationDateRangeKpiResponseTypeDef,
     CampaignDateRangeKpiResponseTypeDef,
     JourneyDateRangeKpiResponseTypeDef,
     DirectMessageConfigurationTypeDef,
+    StartConditionOutputTypeDef,
     StartConditionTypeDef,
     PutEventsRequestRequestTypeDef,
+    SegmentGroupOutputTypeDef,
+    SimpleConditionOutputTypeDef,
     SegmentGroupTypeDef,
     SimpleConditionTypeDef,
-    MessageConfigurationTypeDef,
+    MessageConfigurationOutputTypeDef,
     InAppMessageCampaignTypeDef,
+    GetInAppTemplateResponseTypeDef,
+    MessageConfigurationTypeDef,
     CreateInAppTemplateRequestRequestTypeDef,
     UpdateInAppTemplateRequestRequestTypeDef,
-    GetInAppTemplateResponseTypeDef,
     GetApplicationDateRangeKpiResponseTypeDef,
     GetCampaignDateRangeKpiResponseTypeDef,
     GetJourneyDateRangeKpiResponseTypeDef,
     MessageRequestTypeDef,
     SendUsersMessageRequestTypeDef,
+    SegmentGroupListOutputTypeDef,
+    ConditionOutputTypeDef,
+    MultiConditionalBranchOutputTypeDef,
     SegmentGroupListTypeDef,
     ConditionTypeDef,
     MultiConditionalBranchTypeDef,
     TreatmentResourceTypeDef,
-    WriteTreatmentResourceTypeDef,
     InAppMessagesResponseTypeDef,
+    WriteTreatmentResourceTypeDef,
     SendMessagesRequestRequestTypeDef,
     SendUsersMessagesRequestRequestTypeDef,
     SegmentResponseTypeDef,
+    ConditionalSplitActivityOutputTypeDef,
+    MultiConditionalSplitActivityOutputTypeDef,
     WriteSegmentRequestTypeDef,
     ConditionalSplitActivityTypeDef,
     MultiConditionalSplitActivityTypeDef,
     CampaignResponseTypeDef,
-    WriteCampaignRequestTypeDef,
     GetInAppMessagesResponseTypeDef,
+    WriteCampaignRequestTypeDef,
     CreateSegmentResponseTypeDef,
     DeleteSegmentResponseTypeDef,
     GetSegmentResponseTypeDef,
     GetSegmentVersionResponseTypeDef,
     SegmentsResponseTypeDef,
     UpdateSegmentResponseTypeDef,
+    ActivityOutputTypeDef,
     CreateSegmentRequestRequestTypeDef,
     UpdateSegmentRequestRequestTypeDef,
     ActivityTypeDef,
     CampaignsResponseTypeDef,
     CreateCampaignResponseTypeDef,
     DeleteCampaignResponseTypeDef,
     GetCampaignResponseTypeDef,
```

### Comparing `mypy-boto3-pinpoint-1.28.0/README.md` & `mypy-boto3-pinpoint-1.28.12/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-pinpoint
+Version: 1.28.12
+Summary: Type annotations for boto3.Pinpoint 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 pinpoint type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-pinpoint"></a>
 
 # mypy-boto3-pinpoint
 
 [![PyPI - mypy-boto3-pinpoint](https://img.shields.io/pypi/v/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint)](https://pepy.tech/project/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
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
 [mypy-boto3-pinpoint docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,57 +329,74 @@
 from mypy_boto3_pinpoint.type_defs import (
     ADMChannelRequestTypeDef,
     ADMChannelResponseTypeDef,
     ADMMessageTypeDef,
     APNSChannelRequestTypeDef,
     APNSChannelResponseTypeDef,
     APNSMessageTypeDef,
+    APNSPushNotificationTemplateOutputTypeDef,
     APNSPushNotificationTemplateTypeDef,
     APNSSandboxChannelRequestTypeDef,
     APNSSandboxChannelResponseTypeDef,
     APNSVoipChannelRequestTypeDef,
     APNSVoipChannelResponseTypeDef,
     APNSVoipSandboxChannelRequestTypeDef,
     APNSVoipSandboxChannelResponseTypeDef,
     ActivityResponseTypeDef,
+    ContactCenterActivityOutputTypeDef,
+    HoldoutActivityOutputTypeDef,
     ContactCenterActivityTypeDef,
     HoldoutActivityTypeDef,
     AddressConfigurationTypeDef,
+    AndroidPushNotificationTemplateOutputTypeDef,
     AndroidPushNotificationTemplateTypeDef,
     ApplicationResponseTypeDef,
-    CampaignHookTypeDef,
-    CampaignLimitsTypeDef,
-    QuietTimeTypeDef,
+    CampaignHookOutputTypeDef,
+    CampaignLimitsOutputTypeDef,
+    QuietTimeOutputTypeDef,
+    AttributeDimensionOutputTypeDef,
     AttributeDimensionTypeDef,
     AttributesResourceTypeDef,
     BaiduChannelRequestTypeDef,
     BaiduChannelResponseTypeDef,
     BaiduMessageTypeDef,
+    CampaignCustomMessageOutputTypeDef,
     CampaignCustomMessageTypeDef,
+    CampaignEmailMessageOutputTypeDef,
     CampaignEmailMessageTypeDef,
+    CampaignHookTypeDef,
+    CampaignLimitsTypeDef,
     CampaignStateTypeDef,
-    CustomDeliveryConfigurationTypeDef,
+    CustomDeliveryConfigurationOutputTypeDef,
+    CampaignSmsMessageOutputTypeDef,
     CampaignSmsMessageTypeDef,
     ChannelResponseTypeDef,
+    ClosedDaysRuleOutputTypeDef,
     ClosedDaysRuleTypeDef,
+    WaitTimeOutputTypeDef,
     WaitTimeTypeDef,
     CreateApplicationRequestTypeDef,
+    ResponseMetadataTypeDef,
     EmailTemplateRequestTypeDef,
     CreateTemplateMessageBodyTypeDef,
     ExportJobRequestTypeDef,
     ImportJobRequestTypeDef,
     TemplateCreateMessageBodyTypeDef,
     CreateRecommenderConfigurationTypeDef,
     RecommenderConfigurationResponseTypeDef,
     SMSTemplateRequestTypeDef,
     VoiceTemplateRequestTypeDef,
+    CustomDeliveryConfigurationTypeDef,
+    JourneyCustomMessageOutputTypeDef,
     JourneyCustomMessageTypeDef,
+    DefaultButtonConfigurationOutputTypeDef,
     DefaultButtonConfigurationTypeDef,
     DefaultMessageTypeDef,
     DefaultPushNotificationMessageTypeDef,
+    DefaultPushNotificationTemplateOutputTypeDef,
     DefaultPushNotificationTemplateTypeDef,
     DeleteAdmChannelRequestRequestTypeDef,
     DeleteApnsChannelRequestRequestTypeDef,
     DeleteApnsSandboxChannelRequestRequestTypeDef,
     DeleteApnsVoipChannelRequestRequestTypeDef,
     DeleteApnsVoipSandboxChannelRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
@@ -374,30 +423,36 @@
     DeleteVoiceChannelRequestRequestTypeDef,
     VoiceChannelResponseTypeDef,
     DeleteVoiceTemplateRequestRequestTypeDef,
     GCMMessageTypeDef,
     SMSMessageTypeDef,
     VoiceMessageTypeDef,
     EmailChannelRequestTypeDef,
+    JourneyEmailMessageOutputTypeDef,
     JourneyEmailMessageTypeDef,
     RawEmailTypeDef,
     EmailTemplateResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     EndpointDemographicTypeDef,
     EndpointLocationTypeDef,
     EndpointUserTypeDef,
+    EndpointDemographicOutputTypeDef,
     EndpointItemResponseTypeDef,
+    EndpointLocationOutputTypeDef,
     EndpointMessageResultTypeDef,
+    EndpointUserOutputTypeDef,
     EndpointSendConfigurationTypeDef,
+    MetricDimensionOutputTypeDef,
+    SetDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     SetDimensionTypeDef,
     EventItemResponseTypeDef,
     SessionTypeDef,
     ExportJobResourceTypeDef,
     GCMChannelRequestTypeDef,
+    GPSCoordinatesOutputTypeDef,
     GPSCoordinatesTypeDef,
     GetAdmChannelRequestRequestTypeDef,
     GetApnsChannelRequestRequestTypeDef,
     GetApnsSandboxChannelRequestRequestTypeDef,
     GetApnsVoipChannelRequestRequestTypeDef,
     GetApnsVoipSandboxChannelRequestRequestTypeDef,
     GetAppRequestRequestTypeDef,
@@ -447,91 +502,109 @@
     GetSmsTemplateRequestRequestTypeDef,
     SMSTemplateResponseTypeDef,
     GetUserEndpointsRequestRequestTypeDef,
     GetVoiceChannelRequestRequestTypeDef,
     GetVoiceTemplateRequestRequestTypeDef,
     VoiceTemplateResponseTypeDef,
     ImportJobResourceTypeDef,
+    InAppMessageBodyConfigOutputTypeDef,
     InAppMessageBodyConfigTypeDef,
+    OverrideButtonConfigurationOutputTypeDef,
     OverrideButtonConfigurationTypeDef,
+    InAppMessageHeaderConfigOutputTypeDef,
     InAppMessageHeaderConfigTypeDef,
+    JourneyChannelSettingsOutputTypeDef,
     JourneyChannelSettingsTypeDef,
+    JourneyLimitsOutputTypeDef,
     JourneyLimitsTypeDef,
+    JourneyPushMessageOutputTypeDef,
     JourneyPushMessageTypeDef,
-    JourneyScheduleTypeDef,
+    JourneyScheduleOutputTypeDef,
     JourneyRunResponseTypeDef,
+    JourneySMSMessageOutputTypeDef,
     JourneySMSMessageTypeDef,
+    JourneyScheduleTypeDef,
     JourneyStateRequestTypeDef,
     ListJourneysRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagsModelTypeDef,
+    TagsModelOutputTypeDef,
     ListTemplateVersionsRequestRequestTypeDef,
     ListTemplatesRequestRequestTypeDef,
+    MessageOutputTypeDef,
     MessageTypeDef,
     MessageResultTypeDef,
     NumberValidateRequestTypeDef,
     NumberValidateResponseTypeDef,
+    OpenHoursRuleOutputTypeDef,
     OpenHoursRuleTypeDef,
     WriteEventStreamTypeDef,
+    QuietTimeTypeDef,
+    RandomSplitEntryOutputTypeDef,
     RandomSplitEntryTypeDef,
+    RecencyDimensionOutputTypeDef,
     RecencyDimensionTypeDef,
     UpdateAttributesRequestTypeDef,
-    ResponseMetadataTypeDef,
     ResultRowValueTypeDef,
     SMSChannelRequestTypeDef,
+    SegmentConditionOutputTypeDef,
     SegmentConditionTypeDef,
+    SegmentReferenceOutputTypeDef,
     SegmentReferenceTypeDef,
     SegmentImportResourceTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SimpleEmailPartTypeDef,
+    TagsModelTypeDef,
     TemplateActiveVersionRequestTypeDef,
+    TemplateOutputTypeDef,
     TemplateTypeDef,
     TemplateResponseTypeDef,
     TemplateVersionResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRecommenderConfigurationTypeDef,
     VoiceChannelRequestTypeDef,
     VerificationResponseTypeDef,
     VerifyOTPMessageRequestParametersTypeDef,
     UpdateAdmChannelRequestRequestTypeDef,
-    DeleteAdmChannelResponseTypeDef,
-    GetAdmChannelResponseTypeDef,
-    UpdateAdmChannelResponseTypeDef,
     UpdateApnsChannelRequestRequestTypeDef,
-    DeleteApnsChannelResponseTypeDef,
-    GetApnsChannelResponseTypeDef,
-    UpdateApnsChannelResponseTypeDef,
     UpdateApnsSandboxChannelRequestRequestTypeDef,
-    DeleteApnsSandboxChannelResponseTypeDef,
-    GetApnsSandboxChannelResponseTypeDef,
-    UpdateApnsSandboxChannelResponseTypeDef,
     UpdateApnsVoipChannelRequestRequestTypeDef,
-    DeleteApnsVoipChannelResponseTypeDef,
-    GetApnsVoipChannelResponseTypeDef,
-    UpdateApnsVoipChannelResponseTypeDef,
     UpdateApnsVoipSandboxChannelRequestRequestTypeDef,
-    DeleteApnsVoipSandboxChannelResponseTypeDef,
-    GetApnsVoipSandboxChannelResponseTypeDef,
-    UpdateApnsVoipSandboxChannelResponseTypeDef,
     ActivitiesResponseTypeDef,
     ApplicationsResponseTypeDef,
-    CreateAppResponseTypeDef,
-    DeleteAppResponseTypeDef,
-    GetAppResponseTypeDef,
     ApplicationSettingsResourceTypeDef,
-    WriteApplicationSettingsRequestTypeDef,
-    RemoveAttributesResponseTypeDef,
     UpdateBaiduChannelRequestRequestTypeDef,
-    DeleteBaiduChannelResponseTypeDef,
-    GetBaiduChannelResponseTypeDef,
-    UpdateBaiduChannelResponseTypeDef,
     ChannelsResponseTypeDef,
+    ClosedDaysOutputTypeDef,
     ClosedDaysTypeDef,
+    WaitActivityOutputTypeDef,
     WaitActivityTypeDef,
     CreateAppRequestRequestTypeDef,
+    CreateAppResponseTypeDef,
+    DeleteAdmChannelResponseTypeDef,
+    DeleteApnsChannelResponseTypeDef,
+    DeleteApnsSandboxChannelResponseTypeDef,
+    DeleteApnsVoipChannelResponseTypeDef,
+    DeleteApnsVoipSandboxChannelResponseTypeDef,
+    DeleteAppResponseTypeDef,
+    DeleteBaiduChannelResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAdmChannelResponseTypeDef,
+    GetApnsChannelResponseTypeDef,
+    GetApnsSandboxChannelResponseTypeDef,
+    GetApnsVoipChannelResponseTypeDef,
+    GetApnsVoipSandboxChannelResponseTypeDef,
+    GetAppResponseTypeDef,
+    GetBaiduChannelResponseTypeDef,
+    RemoveAttributesResponseTypeDef,
+    UpdateAdmChannelResponseTypeDef,
+    UpdateApnsChannelResponseTypeDef,
+    UpdateApnsSandboxChannelResponseTypeDef,
+    UpdateApnsVoipChannelResponseTypeDef,
+    UpdateApnsVoipSandboxChannelResponseTypeDef,
+    UpdateBaiduChannelResponseTypeDef,
     CreateEmailTemplateRequestRequestTypeDef,
     UpdateEmailTemplateRequestRequestTypeDef,
     CreateEmailTemplateResponseTypeDef,
     CreatePushTemplateResponseTypeDef,
     CreateSmsTemplateResponseTypeDef,
     CreateVoiceTemplateResponseTypeDef,
     CreateExportJobRequestRequestTypeDef,
@@ -543,17 +616,18 @@
     GetRecommenderConfigurationResponseTypeDef,
     ListRecommenderConfigurationsResponseTypeDef,
     UpdateRecommenderConfigurationResponseTypeDef,
     CreateSmsTemplateRequestRequestTypeDef,
     UpdateSmsTemplateRequestRequestTypeDef,
     CreateVoiceTemplateRequestRequestTypeDef,
     UpdateVoiceTemplateRequestRequestTypeDef,
+    CustomMessageActivityOutputTypeDef,
     CustomMessageActivityTypeDef,
-    PushNotificationTemplateRequestTypeDef,
     PushNotificationTemplateResponseTypeDef,
+    PushNotificationTemplateRequestTypeDef,
     DeleteEmailChannelResponseTypeDef,
     GetEmailChannelResponseTypeDef,
     UpdateEmailChannelResponseTypeDef,
     DeleteEmailTemplateResponseTypeDef,
     DeleteInAppTemplateResponseTypeDef,
     DeletePushTemplateResponseTypeDef,
     DeleteSmsTemplateResponseTypeDef,
@@ -575,154 +649,185 @@
     DeleteSmsChannelResponseTypeDef,
     GetSmsChannelResponseTypeDef,
     UpdateSmsChannelResponseTypeDef,
     DeleteVoiceChannelResponseTypeDef,
     GetVoiceChannelResponseTypeDef,
     UpdateVoiceChannelResponseTypeDef,
     UpdateEmailChannelRequestRequestTypeDef,
+    EmailMessageActivityOutputTypeDef,
     EmailMessageActivityTypeDef,
     GetEmailTemplateResponseTypeDef,
     EndpointBatchItemTypeDef,
     EndpointRequestTypeDef,
-    EndpointResponseTypeDef,
     PublicEndpointTypeDef,
     SendUsersMessageResponseTypeDef,
+    EndpointResponseTypeDef,
+    EventDimensionsOutputTypeDef,
+    SegmentDemographicsOutputTypeDef,
     EventDimensionsTypeDef,
     SegmentDemographicsTypeDef,
     ItemResponseTypeDef,
     EventTypeDef,
     ExportJobResponseTypeDef,
     UpdateGcmChannelRequestRequestTypeDef,
+    GPSPointDimensionOutputTypeDef,
     GPSPointDimensionTypeDef,
     GetJourneyExecutionActivityMetricsResponseTypeDef,
     GetJourneyExecutionMetricsResponseTypeDef,
     GetJourneyRunExecutionActivityMetricsResponseTypeDef,
     GetJourneyRunExecutionMetricsResponseTypeDef,
     GetSmsTemplateResponseTypeDef,
     GetVoiceTemplateResponseTypeDef,
     ImportJobResponseTypeDef,
+    InAppMessageButtonOutputTypeDef,
     InAppMessageButtonTypeDef,
+    PushMessageActivityOutputTypeDef,
     PushMessageActivityTypeDef,
     JourneyRunsResponseTypeDef,
+    SMSMessageActivityOutputTypeDef,
     SMSMessageActivityTypeDef,
     UpdateJourneyStateRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     MessageResponseTypeDef,
     PhoneNumberValidateRequestRequestTypeDef,
     PhoneNumberValidateResponseTypeDef,
+    OpenHoursOutputTypeDef,
     OpenHoursTypeDef,
     PutEventStreamRequestRequestTypeDef,
+    WriteApplicationSettingsRequestTypeDef,
+    RandomSplitActivityOutputTypeDef,
     RandomSplitActivityTypeDef,
+    SegmentBehaviorsOutputTypeDef,
     SegmentBehaviorsTypeDef,
     RemoveAttributesRequestRequestTypeDef,
     ResultRowTypeDef,
     UpdateSmsChannelRequestRequestTypeDef,
     SendOTPMessageRequestRequestTypeDef,
     SimpleEmailTypeDef,
+    TagResourceRequestRequestTypeDef,
     UpdateTemplateActiveVersionRequestRequestTypeDef,
+    TemplateConfigurationOutputTypeDef,
     TemplateConfigurationTypeDef,
     TemplatesResponseTypeDef,
     TemplateVersionsResponseTypeDef,
     UpdateRecommenderConfigurationRequestRequestTypeDef,
     UpdateVoiceChannelRequestRequestTypeDef,
     VerifyOTPMessageResponseTypeDef,
     VerifyOTPMessageRequestRequestTypeDef,
     GetCampaignActivitiesResponseTypeDef,
     GetAppsResponseTypeDef,
     GetApplicationSettingsResponseTypeDef,
     UpdateApplicationSettingsResponseTypeDef,
-    UpdateApplicationSettingsRequestRequestTypeDef,
     GetChannelsResponseTypeDef,
     GetRecommenderConfigurationsResponseTypeDef,
+    GetPushTemplateResponseTypeDef,
     CreatePushTemplateRequestRequestTypeDef,
     UpdatePushTemplateRequestRequestTypeDef,
-    GetPushTemplateResponseTypeDef,
     EndpointBatchRequestTypeDef,
     UpdateEndpointRequestRequestTypeDef,
+    SendUsersMessagesResponseTypeDef,
     DeleteEndpointResponseTypeDef,
     EndpointsResponseTypeDef,
     GetEndpointResponseTypeDef,
-    SendUsersMessagesResponseTypeDef,
+    CampaignEventFilterOutputTypeDef,
+    EventConditionOutputTypeDef,
+    EventFilterOutputTypeDef,
     CampaignEventFilterTypeDef,
     EventConditionTypeDef,
     EventFilterTypeDef,
     EventsResponseTypeDef,
     EventsBatchTypeDef,
     CreateExportJobResponseTypeDef,
     ExportJobsResponseTypeDef,
     GetExportJobResponseTypeDef,
+    SegmentLocationOutputTypeDef,
     SegmentLocationTypeDef,
     CreateImportJobResponseTypeDef,
     GetImportJobResponseTypeDef,
     ImportJobsResponseTypeDef,
+    InAppMessageContentOutputTypeDef,
     InAppMessageContentTypeDef,
     GetJourneyRunsResponseTypeDef,
     SendMessagesResponseTypeDef,
     SendOTPMessageResponseTypeDef,
+    UpdateApplicationSettingsRequestRequestTypeDef,
     BaseKpiResultTypeDef,
     EmailMessageTypeDef,
     ListTemplatesResponseTypeDef,
     ListTemplateVersionsResponseTypeDef,
     UpdateEndpointsBatchRequestRequestTypeDef,
     DeleteUserEndpointsResponseTypeDef,
     GetUserEndpointsResponseTypeDef,
     InAppCampaignScheduleTypeDef,
+    ScheduleOutputTypeDef,
+    EventStartConditionOutputTypeDef,
     ScheduleTypeDef,
     EventStartConditionTypeDef,
     PutEventsResponseTypeDef,
     EventsRequestTypeDef,
     GetExportJobsResponseTypeDef,
     GetSegmentExportJobsResponseTypeDef,
+    SegmentDimensionsOutputTypeDef,
     SegmentDimensionsTypeDef,
     GetImportJobsResponseTypeDef,
     GetSegmentImportJobsResponseTypeDef,
-    CampaignInAppMessageTypeDef,
+    CampaignInAppMessageOutputTypeDef,
     InAppMessageTypeDef,
-    InAppTemplateRequestTypeDef,
     InAppTemplateResponseTypeDef,
+    CampaignInAppMessageTypeDef,
+    InAppTemplateRequestTypeDef,
     ApplicationDateRangeKpiResponseTypeDef,
     CampaignDateRangeKpiResponseTypeDef,
     JourneyDateRangeKpiResponseTypeDef,
     DirectMessageConfigurationTypeDef,
+    StartConditionOutputTypeDef,
     StartConditionTypeDef,
     PutEventsRequestRequestTypeDef,
+    SegmentGroupOutputTypeDef,
+    SimpleConditionOutputTypeDef,
     SegmentGroupTypeDef,
     SimpleConditionTypeDef,
-    MessageConfigurationTypeDef,
+    MessageConfigurationOutputTypeDef,
     InAppMessageCampaignTypeDef,
+    GetInAppTemplateResponseTypeDef,
+    MessageConfigurationTypeDef,
     CreateInAppTemplateRequestRequestTypeDef,
     UpdateInAppTemplateRequestRequestTypeDef,
-    GetInAppTemplateResponseTypeDef,
     GetApplicationDateRangeKpiResponseTypeDef,
     GetCampaignDateRangeKpiResponseTypeDef,
     GetJourneyDateRangeKpiResponseTypeDef,
     MessageRequestTypeDef,
     SendUsersMessageRequestTypeDef,
+    SegmentGroupListOutputTypeDef,
+    ConditionOutputTypeDef,
+    MultiConditionalBranchOutputTypeDef,
     SegmentGroupListTypeDef,
     ConditionTypeDef,
     MultiConditionalBranchTypeDef,
     TreatmentResourceTypeDef,
-    WriteTreatmentResourceTypeDef,
     InAppMessagesResponseTypeDef,
+    WriteTreatmentResourceTypeDef,
     SendMessagesRequestRequestTypeDef,
     SendUsersMessagesRequestRequestTypeDef,
     SegmentResponseTypeDef,
+    ConditionalSplitActivityOutputTypeDef,
+    MultiConditionalSplitActivityOutputTypeDef,
     WriteSegmentRequestTypeDef,
     ConditionalSplitActivityTypeDef,
     MultiConditionalSplitActivityTypeDef,
     CampaignResponseTypeDef,
-    WriteCampaignRequestTypeDef,
     GetInAppMessagesResponseTypeDef,
+    WriteCampaignRequestTypeDef,
     CreateSegmentResponseTypeDef,
     DeleteSegmentResponseTypeDef,
     GetSegmentResponseTypeDef,
     GetSegmentVersionResponseTypeDef,
     SegmentsResponseTypeDef,
     UpdateSegmentResponseTypeDef,
+    ActivityOutputTypeDef,
     CreateSegmentRequestRequestTypeDef,
     UpdateSegmentRequestRequestTypeDef,
     ActivityTypeDef,
     CampaignsResponseTypeDef,
     CreateCampaignResponseTypeDef,
     DeleteCampaignResponseTypeDef,
     GetCampaignResponseTypeDef,
```

### Comparing `mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint/__main__.py` & `mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Pinpoint 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Pinpoint 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint\nOther"
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

### Comparing `mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint/client.py` & `mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint/client.pyi` & `mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint/literals.py` & `mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,14 +253,15 @@
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
@@ -339,26 +340,28 @@
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

### Comparing `mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint/literals.pyi` & `mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -251,14 +251,15 @@
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
@@ -337,26 +338,28 @@
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

### Comparing `mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint/type_defs.py` & `mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -49,65 +49,81 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ADMChannelRequestTypeDef",
     "ADMChannelResponseTypeDef",
     "ADMMessageTypeDef",
     "APNSChannelRequestTypeDef",
     "APNSChannelResponseTypeDef",
     "APNSMessageTypeDef",
+    "APNSPushNotificationTemplateOutputTypeDef",
     "APNSPushNotificationTemplateTypeDef",
     "APNSSandboxChannelRequestTypeDef",
     "APNSSandboxChannelResponseTypeDef",
     "APNSVoipChannelRequestTypeDef",
     "APNSVoipChannelResponseTypeDef",
     "APNSVoipSandboxChannelRequestTypeDef",
     "APNSVoipSandboxChannelResponseTypeDef",
     "ActivityResponseTypeDef",
+    "ContactCenterActivityOutputTypeDef",
+    "HoldoutActivityOutputTypeDef",
     "ContactCenterActivityTypeDef",
     "HoldoutActivityTypeDef",
     "AddressConfigurationTypeDef",
+    "AndroidPushNotificationTemplateOutputTypeDef",
     "AndroidPushNotificationTemplateTypeDef",
     "ApplicationResponseTypeDef",
-    "CampaignHookTypeDef",
-    "CampaignLimitsTypeDef",
-    "QuietTimeTypeDef",
+    "CampaignHookOutputTypeDef",
+    "CampaignLimitsOutputTypeDef",
+    "QuietTimeOutputTypeDef",
+    "AttributeDimensionOutputTypeDef",
     "AttributeDimensionTypeDef",
     "AttributesResourceTypeDef",
     "BaiduChannelRequestTypeDef",
     "BaiduChannelResponseTypeDef",
     "BaiduMessageTypeDef",
+    "CampaignCustomMessageOutputTypeDef",
     "CampaignCustomMessageTypeDef",
+    "CampaignEmailMessageOutputTypeDef",
     "CampaignEmailMessageTypeDef",
+    "CampaignHookTypeDef",
+    "CampaignLimitsTypeDef",
     "CampaignStateTypeDef",
-    "CustomDeliveryConfigurationTypeDef",
+    "CustomDeliveryConfigurationOutputTypeDef",
+    "CampaignSmsMessageOutputTypeDef",
     "CampaignSmsMessageTypeDef",
     "ChannelResponseTypeDef",
+    "ClosedDaysRuleOutputTypeDef",
     "ClosedDaysRuleTypeDef",
+    "WaitTimeOutputTypeDef",
     "WaitTimeTypeDef",
     "CreateApplicationRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "EmailTemplateRequestTypeDef",
     "CreateTemplateMessageBodyTypeDef",
     "ExportJobRequestTypeDef",
     "ImportJobRequestTypeDef",
     "TemplateCreateMessageBodyTypeDef",
     "CreateRecommenderConfigurationTypeDef",
     "RecommenderConfigurationResponseTypeDef",
     "SMSTemplateRequestTypeDef",
     "VoiceTemplateRequestTypeDef",
+    "CustomDeliveryConfigurationTypeDef",
+    "JourneyCustomMessageOutputTypeDef",
     "JourneyCustomMessageTypeDef",
+    "DefaultButtonConfigurationOutputTypeDef",
     "DefaultButtonConfigurationTypeDef",
     "DefaultMessageTypeDef",
     "DefaultPushNotificationMessageTypeDef",
+    "DefaultPushNotificationTemplateOutputTypeDef",
     "DefaultPushNotificationTemplateTypeDef",
     "DeleteAdmChannelRequestRequestTypeDef",
     "DeleteApnsChannelRequestRequestTypeDef",
     "DeleteApnsSandboxChannelRequestRequestTypeDef",
     "DeleteApnsVoipChannelRequestRequestTypeDef",
     "DeleteApnsVoipSandboxChannelRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
@@ -134,30 +150,36 @@
     "DeleteVoiceChannelRequestRequestTypeDef",
     "VoiceChannelResponseTypeDef",
     "DeleteVoiceTemplateRequestRequestTypeDef",
     "GCMMessageTypeDef",
     "SMSMessageTypeDef",
     "VoiceMessageTypeDef",
     "EmailChannelRequestTypeDef",
+    "JourneyEmailMessageOutputTypeDef",
     "JourneyEmailMessageTypeDef",
     "RawEmailTypeDef",
     "EmailTemplateResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EndpointDemographicTypeDef",
     "EndpointLocationTypeDef",
     "EndpointUserTypeDef",
+    "EndpointDemographicOutputTypeDef",
     "EndpointItemResponseTypeDef",
+    "EndpointLocationOutputTypeDef",
     "EndpointMessageResultTypeDef",
+    "EndpointUserOutputTypeDef",
     "EndpointSendConfigurationTypeDef",
+    "MetricDimensionOutputTypeDef",
+    "SetDimensionOutputTypeDef",
     "MetricDimensionTypeDef",
     "SetDimensionTypeDef",
     "EventItemResponseTypeDef",
     "SessionTypeDef",
     "ExportJobResourceTypeDef",
     "GCMChannelRequestTypeDef",
+    "GPSCoordinatesOutputTypeDef",
     "GPSCoordinatesTypeDef",
     "GetAdmChannelRequestRequestTypeDef",
     "GetApnsChannelRequestRequestTypeDef",
     "GetApnsSandboxChannelRequestRequestTypeDef",
     "GetApnsVoipChannelRequestRequestTypeDef",
     "GetApnsVoipSandboxChannelRequestRequestTypeDef",
     "GetAppRequestRequestTypeDef",
@@ -207,91 +229,109 @@
     "GetSmsTemplateRequestRequestTypeDef",
     "SMSTemplateResponseTypeDef",
     "GetUserEndpointsRequestRequestTypeDef",
     "GetVoiceChannelRequestRequestTypeDef",
     "GetVoiceTemplateRequestRequestTypeDef",
     "VoiceTemplateResponseTypeDef",
     "ImportJobResourceTypeDef",
+    "InAppMessageBodyConfigOutputTypeDef",
     "InAppMessageBodyConfigTypeDef",
+    "OverrideButtonConfigurationOutputTypeDef",
     "OverrideButtonConfigurationTypeDef",
+    "InAppMessageHeaderConfigOutputTypeDef",
     "InAppMessageHeaderConfigTypeDef",
+    "JourneyChannelSettingsOutputTypeDef",
     "JourneyChannelSettingsTypeDef",
+    "JourneyLimitsOutputTypeDef",
     "JourneyLimitsTypeDef",
+    "JourneyPushMessageOutputTypeDef",
     "JourneyPushMessageTypeDef",
-    "JourneyScheduleTypeDef",
+    "JourneyScheduleOutputTypeDef",
     "JourneyRunResponseTypeDef",
+    "JourneySMSMessageOutputTypeDef",
     "JourneySMSMessageTypeDef",
+    "JourneyScheduleTypeDef",
     "JourneyStateRequestTypeDef",
     "ListJourneysRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagsModelTypeDef",
+    "TagsModelOutputTypeDef",
     "ListTemplateVersionsRequestRequestTypeDef",
     "ListTemplatesRequestRequestTypeDef",
+    "MessageOutputTypeDef",
     "MessageTypeDef",
     "MessageResultTypeDef",
     "NumberValidateRequestTypeDef",
     "NumberValidateResponseTypeDef",
+    "OpenHoursRuleOutputTypeDef",
     "OpenHoursRuleTypeDef",
     "WriteEventStreamTypeDef",
+    "QuietTimeTypeDef",
+    "RandomSplitEntryOutputTypeDef",
     "RandomSplitEntryTypeDef",
+    "RecencyDimensionOutputTypeDef",
     "RecencyDimensionTypeDef",
     "UpdateAttributesRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ResultRowValueTypeDef",
     "SMSChannelRequestTypeDef",
+    "SegmentConditionOutputTypeDef",
     "SegmentConditionTypeDef",
+    "SegmentReferenceOutputTypeDef",
     "SegmentReferenceTypeDef",
     "SegmentImportResourceTypeDef",
     "SendOTPMessageRequestParametersTypeDef",
     "SimpleEmailPartTypeDef",
+    "TagsModelTypeDef",
     "TemplateActiveVersionRequestTypeDef",
+    "TemplateOutputTypeDef",
     "TemplateTypeDef",
     "TemplateResponseTypeDef",
     "TemplateVersionResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateRecommenderConfigurationTypeDef",
     "VoiceChannelRequestTypeDef",
     "VerificationResponseTypeDef",
     "VerifyOTPMessageRequestParametersTypeDef",
     "UpdateAdmChannelRequestRequestTypeDef",
-    "DeleteAdmChannelResponseTypeDef",
-    "GetAdmChannelResponseTypeDef",
-    "UpdateAdmChannelResponseTypeDef",
     "UpdateApnsChannelRequestRequestTypeDef",
-    "DeleteApnsChannelResponseTypeDef",
-    "GetApnsChannelResponseTypeDef",
-    "UpdateApnsChannelResponseTypeDef",
     "UpdateApnsSandboxChannelRequestRequestTypeDef",
-    "DeleteApnsSandboxChannelResponseTypeDef",
-    "GetApnsSandboxChannelResponseTypeDef",
-    "UpdateApnsSandboxChannelResponseTypeDef",
     "UpdateApnsVoipChannelRequestRequestTypeDef",
-    "DeleteApnsVoipChannelResponseTypeDef",
-    "GetApnsVoipChannelResponseTypeDef",
-    "UpdateApnsVoipChannelResponseTypeDef",
     "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
-    "DeleteApnsVoipSandboxChannelResponseTypeDef",
-    "GetApnsVoipSandboxChannelResponseTypeDef",
-    "UpdateApnsVoipSandboxChannelResponseTypeDef",
     "ActivitiesResponseTypeDef",
     "ApplicationsResponseTypeDef",
-    "CreateAppResponseTypeDef",
-    "DeleteAppResponseTypeDef",
-    "GetAppResponseTypeDef",
     "ApplicationSettingsResourceTypeDef",
-    "WriteApplicationSettingsRequestTypeDef",
-    "RemoveAttributesResponseTypeDef",
     "UpdateBaiduChannelRequestRequestTypeDef",
-    "DeleteBaiduChannelResponseTypeDef",
-    "GetBaiduChannelResponseTypeDef",
-    "UpdateBaiduChannelResponseTypeDef",
     "ChannelsResponseTypeDef",
+    "ClosedDaysOutputTypeDef",
     "ClosedDaysTypeDef",
+    "WaitActivityOutputTypeDef",
     "WaitActivityTypeDef",
     "CreateAppRequestRequestTypeDef",
+    "CreateAppResponseTypeDef",
+    "DeleteAdmChannelResponseTypeDef",
+    "DeleteApnsChannelResponseTypeDef",
+    "DeleteApnsSandboxChannelResponseTypeDef",
+    "DeleteApnsVoipChannelResponseTypeDef",
+    "DeleteApnsVoipSandboxChannelResponseTypeDef",
+    "DeleteAppResponseTypeDef",
+    "DeleteBaiduChannelResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAdmChannelResponseTypeDef",
+    "GetApnsChannelResponseTypeDef",
+    "GetApnsSandboxChannelResponseTypeDef",
+    "GetApnsVoipChannelResponseTypeDef",
+    "GetApnsVoipSandboxChannelResponseTypeDef",
+    "GetAppResponseTypeDef",
+    "GetBaiduChannelResponseTypeDef",
+    "RemoveAttributesResponseTypeDef",
+    "UpdateAdmChannelResponseTypeDef",
+    "UpdateApnsChannelResponseTypeDef",
+    "UpdateApnsSandboxChannelResponseTypeDef",
+    "UpdateApnsVoipChannelResponseTypeDef",
+    "UpdateApnsVoipSandboxChannelResponseTypeDef",
+    "UpdateBaiduChannelResponseTypeDef",
     "CreateEmailTemplateRequestRequestTypeDef",
     "UpdateEmailTemplateRequestRequestTypeDef",
     "CreateEmailTemplateResponseTypeDef",
     "CreatePushTemplateResponseTypeDef",
     "CreateSmsTemplateResponseTypeDef",
     "CreateVoiceTemplateResponseTypeDef",
     "CreateExportJobRequestRequestTypeDef",
@@ -303,17 +343,18 @@
     "GetRecommenderConfigurationResponseTypeDef",
     "ListRecommenderConfigurationsResponseTypeDef",
     "UpdateRecommenderConfigurationResponseTypeDef",
     "CreateSmsTemplateRequestRequestTypeDef",
     "UpdateSmsTemplateRequestRequestTypeDef",
     "CreateVoiceTemplateRequestRequestTypeDef",
     "UpdateVoiceTemplateRequestRequestTypeDef",
+    "CustomMessageActivityOutputTypeDef",
     "CustomMessageActivityTypeDef",
-    "PushNotificationTemplateRequestTypeDef",
     "PushNotificationTemplateResponseTypeDef",
+    "PushNotificationTemplateRequestTypeDef",
     "DeleteEmailChannelResponseTypeDef",
     "GetEmailChannelResponseTypeDef",
     "UpdateEmailChannelResponseTypeDef",
     "DeleteEmailTemplateResponseTypeDef",
     "DeleteInAppTemplateResponseTypeDef",
     "DeletePushTemplateResponseTypeDef",
     "DeleteSmsTemplateResponseTypeDef",
@@ -335,154 +376,185 @@
     "DeleteSmsChannelResponseTypeDef",
     "GetSmsChannelResponseTypeDef",
     "UpdateSmsChannelResponseTypeDef",
     "DeleteVoiceChannelResponseTypeDef",
     "GetVoiceChannelResponseTypeDef",
     "UpdateVoiceChannelResponseTypeDef",
     "UpdateEmailChannelRequestRequestTypeDef",
+    "EmailMessageActivityOutputTypeDef",
     "EmailMessageActivityTypeDef",
     "GetEmailTemplateResponseTypeDef",
     "EndpointBatchItemTypeDef",
     "EndpointRequestTypeDef",
-    "EndpointResponseTypeDef",
     "PublicEndpointTypeDef",
     "SendUsersMessageResponseTypeDef",
+    "EndpointResponseTypeDef",
+    "EventDimensionsOutputTypeDef",
+    "SegmentDemographicsOutputTypeDef",
     "EventDimensionsTypeDef",
     "SegmentDemographicsTypeDef",
     "ItemResponseTypeDef",
     "EventTypeDef",
     "ExportJobResponseTypeDef",
     "UpdateGcmChannelRequestRequestTypeDef",
+    "GPSPointDimensionOutputTypeDef",
     "GPSPointDimensionTypeDef",
     "GetJourneyExecutionActivityMetricsResponseTypeDef",
     "GetJourneyExecutionMetricsResponseTypeDef",
     "GetJourneyRunExecutionActivityMetricsResponseTypeDef",
     "GetJourneyRunExecutionMetricsResponseTypeDef",
     "GetSmsTemplateResponseTypeDef",
     "GetVoiceTemplateResponseTypeDef",
     "ImportJobResponseTypeDef",
+    "InAppMessageButtonOutputTypeDef",
     "InAppMessageButtonTypeDef",
+    "PushMessageActivityOutputTypeDef",
     "PushMessageActivityTypeDef",
     "JourneyRunsResponseTypeDef",
+    "SMSMessageActivityOutputTypeDef",
     "SMSMessageActivityTypeDef",
     "UpdateJourneyStateRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "MessageResponseTypeDef",
     "PhoneNumberValidateRequestRequestTypeDef",
     "PhoneNumberValidateResponseTypeDef",
+    "OpenHoursOutputTypeDef",
     "OpenHoursTypeDef",
     "PutEventStreamRequestRequestTypeDef",
+    "WriteApplicationSettingsRequestTypeDef",
+    "RandomSplitActivityOutputTypeDef",
     "RandomSplitActivityTypeDef",
+    "SegmentBehaviorsOutputTypeDef",
     "SegmentBehaviorsTypeDef",
     "RemoveAttributesRequestRequestTypeDef",
     "ResultRowTypeDef",
     "UpdateSmsChannelRequestRequestTypeDef",
     "SendOTPMessageRequestRequestTypeDef",
     "SimpleEmailTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "UpdateTemplateActiveVersionRequestRequestTypeDef",
+    "TemplateConfigurationOutputTypeDef",
     "TemplateConfigurationTypeDef",
     "TemplatesResponseTypeDef",
     "TemplateVersionsResponseTypeDef",
     "UpdateRecommenderConfigurationRequestRequestTypeDef",
     "UpdateVoiceChannelRequestRequestTypeDef",
     "VerifyOTPMessageResponseTypeDef",
     "VerifyOTPMessageRequestRequestTypeDef",
     "GetCampaignActivitiesResponseTypeDef",
     "GetAppsResponseTypeDef",
     "GetApplicationSettingsResponseTypeDef",
     "UpdateApplicationSettingsResponseTypeDef",
-    "UpdateApplicationSettingsRequestRequestTypeDef",
     "GetChannelsResponseTypeDef",
     "GetRecommenderConfigurationsResponseTypeDef",
+    "GetPushTemplateResponseTypeDef",
     "CreatePushTemplateRequestRequestTypeDef",
     "UpdatePushTemplateRequestRequestTypeDef",
-    "GetPushTemplateResponseTypeDef",
     "EndpointBatchRequestTypeDef",
     "UpdateEndpointRequestRequestTypeDef",
+    "SendUsersMessagesResponseTypeDef",
     "DeleteEndpointResponseTypeDef",
     "EndpointsResponseTypeDef",
     "GetEndpointResponseTypeDef",
-    "SendUsersMessagesResponseTypeDef",
+    "CampaignEventFilterOutputTypeDef",
+    "EventConditionOutputTypeDef",
+    "EventFilterOutputTypeDef",
     "CampaignEventFilterTypeDef",
     "EventConditionTypeDef",
     "EventFilterTypeDef",
     "EventsResponseTypeDef",
     "EventsBatchTypeDef",
     "CreateExportJobResponseTypeDef",
     "ExportJobsResponseTypeDef",
     "GetExportJobResponseTypeDef",
+    "SegmentLocationOutputTypeDef",
     "SegmentLocationTypeDef",
     "CreateImportJobResponseTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobsResponseTypeDef",
+    "InAppMessageContentOutputTypeDef",
     "InAppMessageContentTypeDef",
     "GetJourneyRunsResponseTypeDef",
     "SendMessagesResponseTypeDef",
     "SendOTPMessageResponseTypeDef",
+    "UpdateApplicationSettingsRequestRequestTypeDef",
     "BaseKpiResultTypeDef",
     "EmailMessageTypeDef",
     "ListTemplatesResponseTypeDef",
     "ListTemplateVersionsResponseTypeDef",
     "UpdateEndpointsBatchRequestRequestTypeDef",
     "DeleteUserEndpointsResponseTypeDef",
     "GetUserEndpointsResponseTypeDef",
     "InAppCampaignScheduleTypeDef",
+    "ScheduleOutputTypeDef",
+    "EventStartConditionOutputTypeDef",
     "ScheduleTypeDef",
     "EventStartConditionTypeDef",
     "PutEventsResponseTypeDef",
     "EventsRequestTypeDef",
     "GetExportJobsResponseTypeDef",
     "GetSegmentExportJobsResponseTypeDef",
+    "SegmentDimensionsOutputTypeDef",
     "SegmentDimensionsTypeDef",
     "GetImportJobsResponseTypeDef",
     "GetSegmentImportJobsResponseTypeDef",
-    "CampaignInAppMessageTypeDef",
+    "CampaignInAppMessageOutputTypeDef",
     "InAppMessageTypeDef",
-    "InAppTemplateRequestTypeDef",
     "InAppTemplateResponseTypeDef",
+    "CampaignInAppMessageTypeDef",
+    "InAppTemplateRequestTypeDef",
     "ApplicationDateRangeKpiResponseTypeDef",
     "CampaignDateRangeKpiResponseTypeDef",
     "JourneyDateRangeKpiResponseTypeDef",
     "DirectMessageConfigurationTypeDef",
+    "StartConditionOutputTypeDef",
     "StartConditionTypeDef",
     "PutEventsRequestRequestTypeDef",
+    "SegmentGroupOutputTypeDef",
+    "SimpleConditionOutputTypeDef",
     "SegmentGroupTypeDef",
     "SimpleConditionTypeDef",
-    "MessageConfigurationTypeDef",
+    "MessageConfigurationOutputTypeDef",
     "InAppMessageCampaignTypeDef",
+    "GetInAppTemplateResponseTypeDef",
+    "MessageConfigurationTypeDef",
     "CreateInAppTemplateRequestRequestTypeDef",
     "UpdateInAppTemplateRequestRequestTypeDef",
-    "GetInAppTemplateResponseTypeDef",
     "GetApplicationDateRangeKpiResponseTypeDef",
     "GetCampaignDateRangeKpiResponseTypeDef",
     "GetJourneyDateRangeKpiResponseTypeDef",
     "MessageRequestTypeDef",
     "SendUsersMessageRequestTypeDef",
+    "SegmentGroupListOutputTypeDef",
+    "ConditionOutputTypeDef",
+    "MultiConditionalBranchOutputTypeDef",
     "SegmentGroupListTypeDef",
     "ConditionTypeDef",
     "MultiConditionalBranchTypeDef",
     "TreatmentResourceTypeDef",
-    "WriteTreatmentResourceTypeDef",
     "InAppMessagesResponseTypeDef",
+    "WriteTreatmentResourceTypeDef",
     "SendMessagesRequestRequestTypeDef",
     "SendUsersMessagesRequestRequestTypeDef",
     "SegmentResponseTypeDef",
+    "ConditionalSplitActivityOutputTypeDef",
+    "MultiConditionalSplitActivityOutputTypeDef",
     "WriteSegmentRequestTypeDef",
     "ConditionalSplitActivityTypeDef",
     "MultiConditionalSplitActivityTypeDef",
     "CampaignResponseTypeDef",
-    "WriteCampaignRequestTypeDef",
     "GetInAppMessagesResponseTypeDef",
+    "WriteCampaignRequestTypeDef",
     "CreateSegmentResponseTypeDef",
     "DeleteSegmentResponseTypeDef",
     "GetSegmentResponseTypeDef",
     "GetSegmentVersionResponseTypeDef",
     "SegmentsResponseTypeDef",
     "UpdateSegmentResponseTypeDef",
+    "ActivityOutputTypeDef",
     "CreateSegmentRequestRequestTypeDef",
     "UpdateSegmentRequestRequestTypeDef",
     "ActivityTypeDef",
     "CampaignsResponseTypeDef",
     "CreateCampaignResponseTypeDef",
     "DeleteCampaignResponseTypeDef",
     "GetCampaignResponseTypeDef",
@@ -518,21 +590,19 @@
     "_OptionalADMChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-
 class ADMChannelRequestTypeDef(
     _RequiredADMChannelRequestTypeDef, _OptionalADMChannelRequestTypeDef
 ):
     pass
 
-
 _RequiredADMChannelResponseTypeDef = TypedDict(
     "_RequiredADMChannelResponseTypeDef",
     {
         "Platform": str,
     },
 )
 _OptionalADMChannelResponseTypeDef = TypedDict(
@@ -547,21 +617,19 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class ADMChannelResponseTypeDef(
     _RequiredADMChannelResponseTypeDef, _OptionalADMChannelResponseTypeDef
 ):
     pass
 
-
 ADMMessageTypeDef = TypedDict(
     "ADMMessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "ConsolidationKey": str,
         "Data": Mapping[str, str],
@@ -616,21 +684,19 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class APNSChannelResponseTypeDef(
     _RequiredAPNSChannelResponseTypeDef, _OptionalAPNSChannelResponseTypeDef
 ):
     pass
 
-
 APNSMessageTypeDef = TypedDict(
     "APNSMessageTypeDef",
     {
         "APNSPushType": str,
         "Action": ActionType,
         "Badge": int,
         "Body": str,
@@ -648,14 +714,28 @@
         "TimeToLive": int,
         "Title": str,
         "Url": str,
     },
     total=False,
 )
 
+APNSPushNotificationTemplateOutputTypeDef = TypedDict(
+    "APNSPushNotificationTemplateOutputTypeDef",
+    {
+        "Action": ActionType,
+        "Body": str,
+        "MediaUrl": str,
+        "RawContent": str,
+        "Sound": str,
+        "Title": str,
+        "Url": str,
+    },
+    total=False,
+)
+
 APNSPushNotificationTemplateTypeDef = TypedDict(
     "APNSPushNotificationTemplateTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "MediaUrl": str,
         "RawContent": str,
@@ -701,21 +781,19 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class APNSSandboxChannelResponseTypeDef(
     _RequiredAPNSSandboxChannelResponseTypeDef, _OptionalAPNSSandboxChannelResponseTypeDef
 ):
     pass
 
-
 APNSVoipChannelRequestTypeDef = TypedDict(
     "APNSVoipChannelRequestTypeDef",
     {
         "BundleId": str,
         "Certificate": str,
         "DefaultAuthenticationMethod": str,
         "Enabled": bool,
@@ -747,21 +825,19 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class APNSVoipChannelResponseTypeDef(
     _RequiredAPNSVoipChannelResponseTypeDef, _OptionalAPNSVoipChannelResponseTypeDef
 ):
     pass
 
-
 APNSVoipSandboxChannelRequestTypeDef = TypedDict(
     "APNSVoipSandboxChannelRequestTypeDef",
     {
         "BundleId": str,
         "Certificate": str,
         "DefaultAuthenticationMethod": str,
         "Enabled": bool,
@@ -793,21 +869,19 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class APNSVoipSandboxChannelResponseTypeDef(
     _RequiredAPNSVoipSandboxChannelResponseTypeDef, _OptionalAPNSVoipSandboxChannelResponseTypeDef
 ):
     pass
 
-
 _RequiredActivityResponseTypeDef = TypedDict(
     "_RequiredActivityResponseTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
         "Id": str,
     },
@@ -826,18 +900,43 @@
         "TotalEndpointCount": int,
         "TreatmentId": str,
         "ExecutionMetrics": Dict[str, str],
     },
     total=False,
 )
 
-
 class ActivityResponseTypeDef(_RequiredActivityResponseTypeDef, _OptionalActivityResponseTypeDef):
     pass
 
+ContactCenterActivityOutputTypeDef = TypedDict(
+    "ContactCenterActivityOutputTypeDef",
+    {
+        "NextActivity": str,
+    },
+    total=False,
+)
+
+_RequiredHoldoutActivityOutputTypeDef = TypedDict(
+    "_RequiredHoldoutActivityOutputTypeDef",
+    {
+        "Percentage": int,
+    },
+)
+_OptionalHoldoutActivityOutputTypeDef = TypedDict(
+    "_OptionalHoldoutActivityOutputTypeDef",
+    {
+        "NextActivity": str,
+    },
+    total=False,
+)
+
+class HoldoutActivityOutputTypeDef(
+    _RequiredHoldoutActivityOutputTypeDef, _OptionalHoldoutActivityOutputTypeDef
+):
+    pass
 
 ContactCenterActivityTypeDef = TypedDict(
     "ContactCenterActivityTypeDef",
     {
         "NextActivity": str,
     },
     total=False,
@@ -853,32 +952,46 @@
     "_OptionalHoldoutActivityTypeDef",
     {
         "NextActivity": str,
     },
     total=False,
 )
 
-
 class HoldoutActivityTypeDef(_RequiredHoldoutActivityTypeDef, _OptionalHoldoutActivityTypeDef):
     pass
 
-
 AddressConfigurationTypeDef = TypedDict(
     "AddressConfigurationTypeDef",
     {
         "BodyOverride": str,
         "ChannelType": ChannelTypeType,
         "Context": Mapping[str, str],
         "RawContent": str,
         "Substitutions": Mapping[str, Sequence[str]],
         "TitleOverride": str,
     },
     total=False,
 )
 
+AndroidPushNotificationTemplateOutputTypeDef = TypedDict(
+    "AndroidPushNotificationTemplateOutputTypeDef",
+    {
+        "Action": ActionType,
+        "Body": str,
+        "ImageIconUrl": str,
+        "ImageUrl": str,
+        "RawContent": str,
+        "SmallImageIconUrl": str,
+        "Sound": str,
+        "Title": str,
+        "Url": str,
+    },
+    total=False,
+)
+
 AndroidPushNotificationTemplateTypeDef = TypedDict(
     "AndroidPushNotificationTemplateTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "ImageIconUrl": str,
         "ImageUrl": str,
@@ -904,73 +1017,88 @@
     {
         "tags": Dict[str, str],
         "CreationDate": str,
     },
     total=False,
 )
 
-
 class ApplicationResponseTypeDef(
     _RequiredApplicationResponseTypeDef, _OptionalApplicationResponseTypeDef
 ):
     pass
 
-
-CampaignHookTypeDef = TypedDict(
-    "CampaignHookTypeDef",
+CampaignHookOutputTypeDef = TypedDict(
+    "CampaignHookOutputTypeDef",
     {
         "LambdaFunctionName": str,
         "Mode": ModeType,
         "WebUrl": str,
     },
     total=False,
 )
 
-CampaignLimitsTypeDef = TypedDict(
-    "CampaignLimitsTypeDef",
+CampaignLimitsOutputTypeDef = TypedDict(
+    "CampaignLimitsOutputTypeDef",
     {
         "Daily": int,
         "MaximumDuration": int,
         "MessagesPerSecond": int,
         "Total": int,
         "Session": int,
     },
     total=False,
 )
 
-QuietTimeTypeDef = TypedDict(
-    "QuietTimeTypeDef",
+QuietTimeOutputTypeDef = TypedDict(
+    "QuietTimeOutputTypeDef",
     {
         "End": str,
         "Start": str,
     },
     total=False,
 )
 
+_RequiredAttributeDimensionOutputTypeDef = TypedDict(
+    "_RequiredAttributeDimensionOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+)
+_OptionalAttributeDimensionOutputTypeDef = TypedDict(
+    "_OptionalAttributeDimensionOutputTypeDef",
+    {
+        "AttributeType": AttributeTypeType,
+    },
+    total=False,
+)
+
+class AttributeDimensionOutputTypeDef(
+    _RequiredAttributeDimensionOutputTypeDef, _OptionalAttributeDimensionOutputTypeDef
+):
+    pass
+
 _RequiredAttributeDimensionTypeDef = TypedDict(
     "_RequiredAttributeDimensionTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 _OptionalAttributeDimensionTypeDef = TypedDict(
     "_OptionalAttributeDimensionTypeDef",
     {
         "AttributeType": AttributeTypeType,
     },
     total=False,
 )
 
-
 class AttributeDimensionTypeDef(
     _RequiredAttributeDimensionTypeDef, _OptionalAttributeDimensionTypeDef
 ):
     pass
 
-
 _RequiredAttributesResourceTypeDef = TypedDict(
     "_RequiredAttributesResourceTypeDef",
     {
         "ApplicationId": str,
         "AttributeType": str,
     },
 )
@@ -978,21 +1106,19 @@
     "_OptionalAttributesResourceTypeDef",
     {
         "Attributes": List[str],
     },
     total=False,
 )
 
-
 class AttributesResourceTypeDef(
     _RequiredAttributesResourceTypeDef, _OptionalAttributesResourceTypeDef
 ):
     pass
 
-
 _RequiredBaiduChannelRequestTypeDef = TypedDict(
     "_RequiredBaiduChannelRequestTypeDef",
     {
         "ApiKey": str,
         "SecretKey": str,
     },
 )
@@ -1000,21 +1126,19 @@
     "_OptionalBaiduChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-
 class BaiduChannelRequestTypeDef(
     _RequiredBaiduChannelRequestTypeDef, _OptionalBaiduChannelRequestTypeDef
 ):
     pass
 
-
 _RequiredBaiduChannelResponseTypeDef = TypedDict(
     "_RequiredBaiduChannelResponseTypeDef",
     {
         "Credential": str,
         "Platform": str,
     },
 )
@@ -1030,21 +1154,19 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class BaiduChannelResponseTypeDef(
     _RequiredBaiduChannelResponseTypeDef, _OptionalBaiduChannelResponseTypeDef
 ):
     pass
 
-
 BaiduMessageTypeDef = TypedDict(
     "BaiduMessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "Data": Mapping[str, str],
         "IconReference": str,
@@ -1058,61 +1180,114 @@
         "TimeToLive": int,
         "Title": str,
         "Url": str,
     },
     total=False,
 )
 
+CampaignCustomMessageOutputTypeDef = TypedDict(
+    "CampaignCustomMessageOutputTypeDef",
+    {
+        "Data": str,
+    },
+    total=False,
+)
+
 CampaignCustomMessageTypeDef = TypedDict(
     "CampaignCustomMessageTypeDef",
     {
         "Data": str,
     },
     total=False,
 )
 
+CampaignEmailMessageOutputTypeDef = TypedDict(
+    "CampaignEmailMessageOutputTypeDef",
+    {
+        "Body": str,
+        "FromAddress": str,
+        "HtmlBody": str,
+        "Title": str,
+    },
+    total=False,
+)
+
 CampaignEmailMessageTypeDef = TypedDict(
     "CampaignEmailMessageTypeDef",
     {
         "Body": str,
         "FromAddress": str,
         "HtmlBody": str,
         "Title": str,
     },
     total=False,
 )
 
+CampaignHookTypeDef = TypedDict(
+    "CampaignHookTypeDef",
+    {
+        "LambdaFunctionName": str,
+        "Mode": ModeType,
+        "WebUrl": str,
+    },
+    total=False,
+)
+
+CampaignLimitsTypeDef = TypedDict(
+    "CampaignLimitsTypeDef",
+    {
+        "Daily": int,
+        "MaximumDuration": int,
+        "MessagesPerSecond": int,
+        "Total": int,
+        "Session": int,
+    },
+    total=False,
+)
+
 CampaignStateTypeDef = TypedDict(
     "CampaignStateTypeDef",
     {
         "CampaignStatus": CampaignStatusType,
     },
     total=False,
 )
 
-_RequiredCustomDeliveryConfigurationTypeDef = TypedDict(
-    "_RequiredCustomDeliveryConfigurationTypeDef",
+_RequiredCustomDeliveryConfigurationOutputTypeDef = TypedDict(
+    "_RequiredCustomDeliveryConfigurationOutputTypeDef",
     {
         "DeliveryUri": str,
     },
 )
-_OptionalCustomDeliveryConfigurationTypeDef = TypedDict(
-    "_OptionalCustomDeliveryConfigurationTypeDef",
+_OptionalCustomDeliveryConfigurationOutputTypeDef = TypedDict(
+    "_OptionalCustomDeliveryConfigurationOutputTypeDef",
     {
-        "EndpointTypes": Sequence[EndpointTypesElementType],
+        "EndpointTypes": List[EndpointTypesElementType],
     },
     total=False,
 )
 
-
-class CustomDeliveryConfigurationTypeDef(
-    _RequiredCustomDeliveryConfigurationTypeDef, _OptionalCustomDeliveryConfigurationTypeDef
+class CustomDeliveryConfigurationOutputTypeDef(
+    _RequiredCustomDeliveryConfigurationOutputTypeDef,
+    _OptionalCustomDeliveryConfigurationOutputTypeDef,
 ):
     pass
 
+CampaignSmsMessageOutputTypeDef = TypedDict(
+    "CampaignSmsMessageOutputTypeDef",
+    {
+        "Body": str,
+        "MessageType": MessageTypeType,
+        "OriginationNumber": str,
+        "SenderId": str,
+        "EntityId": str,
+        "TemplateId": str,
+    },
+    total=False,
+)
 
 CampaignSmsMessageTypeDef = TypedDict(
     "CampaignSmsMessageTypeDef",
     {
         "Body": str,
         "MessageType": MessageTypeType,
         "OriginationNumber": str,
@@ -1135,24 +1310,43 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+ClosedDaysRuleOutputTypeDef = TypedDict(
+    "ClosedDaysRuleOutputTypeDef",
+    {
+        "Name": str,
+        "StartDateTime": str,
+        "EndDateTime": str,
+    },
+    total=False,
+)
+
 ClosedDaysRuleTypeDef = TypedDict(
     "ClosedDaysRuleTypeDef",
     {
         "Name": str,
         "StartDateTime": str,
         "EndDateTime": str,
     },
     total=False,
 )
 
+WaitTimeOutputTypeDef = TypedDict(
+    "WaitTimeOutputTypeDef",
+    {
+        "WaitFor": str,
+        "WaitUntil": str,
+    },
+    total=False,
+)
+
 WaitTimeTypeDef = TypedDict(
     "WaitTimeTypeDef",
     {
         "WaitFor": str,
         "WaitUntil": str,
     },
     total=False,
@@ -1168,20 +1362,29 @@
     "_OptionalCreateApplicationRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateApplicationRequestTypeDef(
     _RequiredCreateApplicationRequestTypeDef, _OptionalCreateApplicationRequestTypeDef
 ):
     pass
 
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
 
 EmailTemplateRequestTypeDef = TypedDict(
     "EmailTemplateRequestTypeDef",
     {
         "DefaultSubstitutions": str,
         "HtmlPart": str,
         "RecommenderId": str,
@@ -1215,19 +1418,17 @@
     {
         "SegmentId": str,
         "SegmentVersion": int,
     },
     total=False,
 )
 
-
 class ExportJobRequestTypeDef(_RequiredExportJobRequestTypeDef, _OptionalExportJobRequestTypeDef):
     pass
 
-
 _RequiredImportJobRequestTypeDef = TypedDict(
     "_RequiredImportJobRequestTypeDef",
     {
         "Format": FormatType,
         "RoleArn": str,
         "S3Url": str,
     },
@@ -1240,19 +1441,17 @@
         "RegisterEndpoints": bool,
         "SegmentId": str,
         "SegmentName": str,
     },
     total=False,
 )
 
-
 class ImportJobRequestTypeDef(_RequiredImportJobRequestTypeDef, _OptionalImportJobRequestTypeDef):
     pass
 
-
 TemplateCreateMessageBodyTypeDef = TypedDict(
     "TemplateCreateMessageBodyTypeDef",
     {
         "Arn": str,
         "Message": str,
         "RequestID": str,
     },
@@ -1276,21 +1475,19 @@
         "RecommendationTransformerUri": str,
         "RecommendationsDisplayName": str,
         "RecommendationsPerMessage": int,
     },
     total=False,
 )
 
-
 class CreateRecommenderConfigurationTypeDef(
     _RequiredCreateRecommenderConfigurationTypeDef, _OptionalCreateRecommenderConfigurationTypeDef
 ):
     pass
 
-
 _RequiredRecommenderConfigurationResponseTypeDef = TypedDict(
     "_RequiredRecommenderConfigurationResponseTypeDef",
     {
         "CreationDate": str,
         "Id": str,
         "LastModifiedDate": str,
         "RecommendationProviderRoleArn": str,
@@ -1307,22 +1504,20 @@
         "RecommendationTransformerUri": str,
         "RecommendationsDisplayName": str,
         "RecommendationsPerMessage": int,
     },
     total=False,
 )
 
-
 class RecommenderConfigurationResponseTypeDef(
     _RequiredRecommenderConfigurationResponseTypeDef,
     _OptionalRecommenderConfigurationResponseTypeDef,
 ):
     pass
 
-
 SMSTemplateRequestTypeDef = TypedDict(
     "SMSTemplateRequestTypeDef",
     {
         "Body": str,
         "DefaultSubstitutions": str,
         "RecommenderId": str,
         "tags": Mapping[str, str],
@@ -1340,22 +1535,73 @@
         "tags": Mapping[str, str],
         "TemplateDescription": str,
         "VoiceId": str,
     },
     total=False,
 )
 
+_RequiredCustomDeliveryConfigurationTypeDef = TypedDict(
+    "_RequiredCustomDeliveryConfigurationTypeDef",
+    {
+        "DeliveryUri": str,
+    },
+)
+_OptionalCustomDeliveryConfigurationTypeDef = TypedDict(
+    "_OptionalCustomDeliveryConfigurationTypeDef",
+    {
+        "EndpointTypes": Sequence[EndpointTypesElementType],
+    },
+    total=False,
+)
+
+class CustomDeliveryConfigurationTypeDef(
+    _RequiredCustomDeliveryConfigurationTypeDef, _OptionalCustomDeliveryConfigurationTypeDef
+):
+    pass
+
+JourneyCustomMessageOutputTypeDef = TypedDict(
+    "JourneyCustomMessageOutputTypeDef",
+    {
+        "Data": str,
+    },
+    total=False,
+)
+
 JourneyCustomMessageTypeDef = TypedDict(
     "JourneyCustomMessageTypeDef",
     {
         "Data": str,
     },
     total=False,
 )
 
+_RequiredDefaultButtonConfigurationOutputTypeDef = TypedDict(
+    "_RequiredDefaultButtonConfigurationOutputTypeDef",
+    {
+        "ButtonAction": ButtonActionType,
+        "Text": str,
+    },
+)
+_OptionalDefaultButtonConfigurationOutputTypeDef = TypedDict(
+    "_OptionalDefaultButtonConfigurationOutputTypeDef",
+    {
+        "BackgroundColor": str,
+        "BorderRadius": int,
+        "Link": str,
+        "TextColor": str,
+    },
+    total=False,
+)
+
+class DefaultButtonConfigurationOutputTypeDef(
+    _RequiredDefaultButtonConfigurationOutputTypeDef,
+    _OptionalDefaultButtonConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredDefaultButtonConfigurationTypeDef = TypedDict(
     "_RequiredDefaultButtonConfigurationTypeDef",
     {
         "ButtonAction": ButtonActionType,
         "Text": str,
     },
 )
@@ -1366,21 +1612,19 @@
         "BorderRadius": int,
         "Link": str,
         "TextColor": str,
     },
     total=False,
 )
 
-
 class DefaultButtonConfigurationTypeDef(
     _RequiredDefaultButtonConfigurationTypeDef, _OptionalDefaultButtonConfigurationTypeDef
 ):
     pass
 
-
 DefaultMessageTypeDef = TypedDict(
     "DefaultMessageTypeDef",
     {
         "Body": str,
         "Substitutions": Mapping[str, Sequence[str]],
     },
     total=False,
@@ -1396,14 +1640,26 @@
         "Substitutions": Mapping[str, Sequence[str]],
         "Title": str,
         "Url": str,
     },
     total=False,
 )
 
+DefaultPushNotificationTemplateOutputTypeDef = TypedDict(
+    "DefaultPushNotificationTemplateOutputTypeDef",
+    {
+        "Action": ActionType,
+        "Body": str,
+        "Sound": str,
+        "Title": str,
+        "Url": str,
+    },
+    total=False,
+)
+
 DefaultPushNotificationTemplateTypeDef = TypedDict(
     "DefaultPushNotificationTemplateTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "Sound": str,
         "Title": str,
@@ -1499,43 +1755,39 @@
         "MessagesPerSecond": int,
         "RoleArn": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class EmailChannelResponseTypeDef(
     _RequiredEmailChannelResponseTypeDef, _OptionalEmailChannelResponseTypeDef
 ):
     pass
 
-
 _RequiredDeleteEmailTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteEmailTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteEmailTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class DeleteEmailTemplateRequestRequestTypeDef(
     _RequiredDeleteEmailTemplateRequestRequestTypeDef,
     _OptionalDeleteEmailTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 MessageBodyTypeDef = TypedDict(
     "MessageBodyTypeDef",
     {
         "Message": str,
         "RequestID": str,
     },
     total=False,
@@ -1570,19 +1822,17 @@
         "ExternalId": str,
         "LastModifiedDate": str,
         "LastUpdatedBy": str,
     },
     total=False,
 )
 
-
 class EventStreamTypeDef(_RequiredEventStreamTypeDef, _OptionalEventStreamTypeDef):
     pass
 
-
 DeleteGcmChannelRequestRequestTypeDef = TypedDict(
     "DeleteGcmChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -1605,43 +1855,39 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class GCMChannelResponseTypeDef(
     _RequiredGCMChannelResponseTypeDef, _OptionalGCMChannelResponseTypeDef
 ):
     pass
 
-
 _RequiredDeleteInAppTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteInAppTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteInAppTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteInAppTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class DeleteInAppTemplateRequestRequestTypeDef(
     _RequiredDeleteInAppTemplateRequestRequestTypeDef,
     _OptionalDeleteInAppTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteJourneyRequestRequestTypeDef = TypedDict(
     "DeleteJourneyRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
     },
 )
@@ -1656,22 +1902,20 @@
     "_OptionalDeletePushTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class DeletePushTemplateRequestRequestTypeDef(
     _RequiredDeletePushTemplateRequestRequestTypeDef,
     _OptionalDeletePushTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteRecommenderConfigurationRequestRequestTypeDef",
     {
         "RecommenderId": str,
     },
 )
 
@@ -1712,42 +1956,38 @@
         "ShortCode": str,
         "TransactionalMessagesPerSecond": int,
         "Version": int,
     },
     total=False,
 )
 
-
 class SMSChannelResponseTypeDef(
     _RequiredSMSChannelResponseTypeDef, _OptionalSMSChannelResponseTypeDef
 ):
     pass
 
-
 _RequiredDeleteSmsTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteSmsTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteSmsTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteSmsTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class DeleteSmsTemplateRequestRequestTypeDef(
     _RequiredDeleteSmsTemplateRequestRequestTypeDef, _OptionalDeleteSmsTemplateRequestRequestTypeDef
 ):
     pass
 
-
 DeleteUserEndpointsRequestRequestTypeDef = TypedDict(
     "DeleteUserEndpointsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "UserId": str,
     },
 )
@@ -1777,43 +2017,39 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-
 class VoiceChannelResponseTypeDef(
     _RequiredVoiceChannelResponseTypeDef, _OptionalVoiceChannelResponseTypeDef
 ):
     pass
 
-
 _RequiredDeleteVoiceTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteVoiceTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteVoiceTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteVoiceTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class DeleteVoiceTemplateRequestRequestTypeDef(
     _RequiredDeleteVoiceTemplateRequestRequestTypeDef,
     _OptionalDeleteVoiceTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 GCMMessageTypeDef = TypedDict(
     "GCMMessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "CollapseKey": str,
         "Data": Mapping[str, str],
@@ -1875,20 +2111,26 @@
         "ConfigurationSet": str,
         "Enabled": bool,
         "RoleArn": str,
     },
     total=False,
 )
 
-
 class EmailChannelRequestTypeDef(
     _RequiredEmailChannelRequestTypeDef, _OptionalEmailChannelRequestTypeDef
 ):
     pass
 
+JourneyEmailMessageOutputTypeDef = TypedDict(
+    "JourneyEmailMessageOutputTypeDef",
+    {
+        "FromAddress": str,
+    },
+    total=False,
+)
 
 JourneyEmailMessageTypeDef = TypedDict(
     "JourneyEmailMessageTypeDef",
     {
         "FromAddress": str,
     },
     total=False,
@@ -1923,28 +2165,19 @@
         "TemplateDescription": str,
         "TextPart": str,
         "Version": str,
     },
     total=False,
 )
 
-
 class EmailTemplateResponseTypeDef(
     _RequiredEmailTemplateResponseTypeDef, _OptionalEmailTemplateResponseTypeDef
 ):
     pass
 
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EndpointDemographicTypeDef = TypedDict(
     "EndpointDemographicTypeDef",
     {
         "AppVersion": str,
         "Locale": str,
         "Make": str,
         "Model": str,
@@ -1968,29 +2201,57 @@
     },
     total=False,
 )
 
 EndpointUserTypeDef = TypedDict(
     "EndpointUserTypeDef",
     {
-        "UserAttributes": Dict[str, List[str]],
+        "UserAttributes": Mapping[str, Sequence[str]],
         "UserId": str,
     },
     total=False,
 )
 
+EndpointDemographicOutputTypeDef = TypedDict(
+    "EndpointDemographicOutputTypeDef",
+    {
+        "AppVersion": str,
+        "Locale": str,
+        "Make": str,
+        "Model": str,
+        "ModelVersion": str,
+        "Platform": str,
+        "PlatformVersion": str,
+        "Timezone": str,
+    },
+    total=False,
+)
+
 EndpointItemResponseTypeDef = TypedDict(
     "EndpointItemResponseTypeDef",
     {
         "Message": str,
         "StatusCode": int,
     },
     total=False,
 )
 
+EndpointLocationOutputTypeDef = TypedDict(
+    "EndpointLocationOutputTypeDef",
+    {
+        "City": str,
+        "Country": str,
+        "Latitude": float,
+        "Longitude": float,
+        "PostalCode": str,
+        "Region": str,
+    },
+    total=False,
+)
+
 _RequiredEndpointMessageResultTypeDef = TypedDict(
     "_RequiredEndpointMessageResultTypeDef",
     {
         "DeliveryStatus": DeliveryStatusType,
         "StatusCode": int,
     },
 )
@@ -2001,33 +2262,67 @@
         "MessageId": str,
         "StatusMessage": str,
         "UpdatedToken": str,
     },
     total=False,
 )
 
-
 class EndpointMessageResultTypeDef(
     _RequiredEndpointMessageResultTypeDef, _OptionalEndpointMessageResultTypeDef
 ):
     pass
 
+EndpointUserOutputTypeDef = TypedDict(
+    "EndpointUserOutputTypeDef",
+    {
+        "UserAttributes": Dict[str, List[str]],
+        "UserId": str,
+    },
+    total=False,
+)
 
 EndpointSendConfigurationTypeDef = TypedDict(
     "EndpointSendConfigurationTypeDef",
     {
         "BodyOverride": str,
         "Context": Mapping[str, str],
         "RawContent": str,
         "Substitutions": Mapping[str, Sequence[str]],
         "TitleOverride": str,
     },
     total=False,
 )
 
+MetricDimensionOutputTypeDef = TypedDict(
+    "MetricDimensionOutputTypeDef",
+    {
+        "ComparisonOperator": str,
+        "Value": float,
+    },
+)
+
+_RequiredSetDimensionOutputTypeDef = TypedDict(
+    "_RequiredSetDimensionOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+)
+_OptionalSetDimensionOutputTypeDef = TypedDict(
+    "_OptionalSetDimensionOutputTypeDef",
+    {
+        "DimensionType": DimensionTypeType,
+    },
+    total=False,
+)
+
+class SetDimensionOutputTypeDef(
+    _RequiredSetDimensionOutputTypeDef, _OptionalSetDimensionOutputTypeDef
+):
+    pass
+
 MetricDimensionTypeDef = TypedDict(
     "MetricDimensionTypeDef",
     {
         "ComparisonOperator": str,
         "Value": float,
     },
 )
@@ -2042,19 +2337,17 @@
     "_OptionalSetDimensionTypeDef",
     {
         "DimensionType": DimensionTypeType,
     },
     total=False,
 )
 
-
 class SetDimensionTypeDef(_RequiredSetDimensionTypeDef, _OptionalSetDimensionTypeDef):
     pass
 
-
 EventItemResponseTypeDef = TypedDict(
     "EventItemResponseTypeDef",
     {
         "Message": str,
         "StatusCode": int,
     },
     total=False,
@@ -2072,19 +2365,17 @@
     {
         "Duration": int,
         "StopTimestamp": str,
     },
     total=False,
 )
 
-
 class SessionTypeDef(_RequiredSessionTypeDef, _OptionalSessionTypeDef):
     pass
 
-
 _RequiredExportJobResourceTypeDef = TypedDict(
     "_RequiredExportJobResourceTypeDef",
     {
         "RoleArn": str,
         "S3UrlPrefix": str,
     },
 )
@@ -2093,41 +2384,45 @@
     {
         "SegmentId": str,
         "SegmentVersion": int,
     },
     total=False,
 )
 
-
 class ExportJobResourceTypeDef(
     _RequiredExportJobResourceTypeDef, _OptionalExportJobResourceTypeDef
 ):
     pass
 
-
 _RequiredGCMChannelRequestTypeDef = TypedDict(
     "_RequiredGCMChannelRequestTypeDef",
     {
         "ApiKey": str,
     },
 )
 _OptionalGCMChannelRequestTypeDef = TypedDict(
     "_OptionalGCMChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-
 class GCMChannelRequestTypeDef(
     _RequiredGCMChannelRequestTypeDef, _OptionalGCMChannelRequestTypeDef
 ):
     pass
 
+GPSCoordinatesOutputTypeDef = TypedDict(
+    "GPSCoordinatesOutputTypeDef",
+    {
+        "Latitude": float,
+        "Longitude": float,
+    },
+)
 
 GPSCoordinatesTypeDef = TypedDict(
     "GPSCoordinatesTypeDef",
     {
         "Latitude": float,
         "Longitude": float,
     },
@@ -2189,22 +2484,20 @@
         "NextToken": str,
         "PageSize": str,
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class GetApplicationDateRangeKpiRequestRequestTypeDef(
     _RequiredGetApplicationDateRangeKpiRequestRequestTypeDef,
     _OptionalGetApplicationDateRangeKpiRequestRequestTypeDef,
 ):
     pass
 
-
 GetApplicationSettingsRequestRequestTypeDef = TypedDict(
     "GetApplicationSettingsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2236,22 +2529,20 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetCampaignActivitiesRequestRequestTypeDef(
     _RequiredGetCampaignActivitiesRequestRequestTypeDef,
     _OptionalGetCampaignActivitiesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetCampaignDateRangeKpiRequestRequestTypeDef = TypedDict(
     "_RequiredGetCampaignDateRangeKpiRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
         "KpiName": str,
     },
@@ -2263,22 +2554,20 @@
         "NextToken": str,
         "PageSize": str,
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class GetCampaignDateRangeKpiRequestRequestTypeDef(
     _RequiredGetCampaignDateRangeKpiRequestRequestTypeDef,
     _OptionalGetCampaignDateRangeKpiRequestRequestTypeDef,
 ):
     pass
 
-
 GetCampaignRequestRequestTypeDef = TypedDict(
     "GetCampaignRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
     },
 )
@@ -2304,22 +2593,20 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetCampaignVersionsRequestRequestTypeDef(
     _RequiredGetCampaignVersionsRequestRequestTypeDef,
     _OptionalGetCampaignVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetCampaignsRequestRequestTypeDef = TypedDict(
     "_RequiredGetCampaignsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalGetCampaignsRequestRequestTypeDef = TypedDict(
@@ -2327,21 +2614,19 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetCampaignsRequestRequestTypeDef(
     _RequiredGetCampaignsRequestRequestTypeDef, _OptionalGetCampaignsRequestRequestTypeDef
 ):
     pass
 
-
 GetChannelsRequestRequestTypeDef = TypedDict(
     "GetChannelsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2362,21 +2647,19 @@
     "_OptionalGetEmailTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class GetEmailTemplateRequestRequestTypeDef(
     _RequiredGetEmailTemplateRequestRequestTypeDef, _OptionalGetEmailTemplateRequestRequestTypeDef
 ):
     pass
 
-
 GetEndpointRequestRequestTypeDef = TypedDict(
     "GetEndpointRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EndpointId": str,
     },
 )
@@ -2407,21 +2690,19 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetExportJobsRequestRequestTypeDef(
     _RequiredGetExportJobsRequestRequestTypeDef, _OptionalGetExportJobsRequestRequestTypeDef
 ):
     pass
 
-
 GetGcmChannelRequestRequestTypeDef = TypedDict(
     "GetGcmChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2444,21 +2725,19 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetImportJobsRequestRequestTypeDef(
     _RequiredGetImportJobsRequestRequestTypeDef, _OptionalGetImportJobsRequestRequestTypeDef
 ):
     pass
 
-
 GetInAppMessagesRequestRequestTypeDef = TypedDict(
     "GetInAppMessagesRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EndpointId": str,
     },
 )
@@ -2473,21 +2752,19 @@
     "_OptionalGetInAppTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class GetInAppTemplateRequestRequestTypeDef(
     _RequiredGetInAppTemplateRequestRequestTypeDef, _OptionalGetInAppTemplateRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetJourneyDateRangeKpiRequestRequestTypeDef = TypedDict(
     "_RequiredGetJourneyDateRangeKpiRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
         "KpiName": str,
     },
@@ -2499,22 +2776,20 @@
         "NextToken": str,
         "PageSize": str,
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class GetJourneyDateRangeKpiRequestRequestTypeDef(
     _RequiredGetJourneyDateRangeKpiRequestRequestTypeDef,
     _OptionalGetJourneyDateRangeKpiRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyActivityId": str,
         "JourneyId": str,
     },
@@ -2524,22 +2799,20 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
-
 class GetJourneyExecutionActivityMetricsRequestRequestTypeDef(
     _RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef,
     _OptionalGetJourneyExecutionActivityMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 JourneyExecutionActivityMetricsResponseTypeDef = TypedDict(
     "JourneyExecutionActivityMetricsResponseTypeDef",
     {
         "ActivityType": str,
         "ApplicationId": str,
         "JourneyActivityId": str,
         "JourneyId": str,
@@ -2560,22 +2833,20 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
-
 class GetJourneyExecutionMetricsRequestRequestTypeDef(
     _RequiredGetJourneyExecutionMetricsRequestRequestTypeDef,
     _OptionalGetJourneyExecutionMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 JourneyExecutionMetricsResponseTypeDef = TypedDict(
     "JourneyExecutionMetricsResponseTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
         "LastEvaluatedTime": str,
         "Metrics": Dict[str, str],
@@ -2604,22 +2875,20 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
-
 class GetJourneyRunExecutionActivityMetricsRequestRequestTypeDef(
     _RequiredGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
     _OptionalGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 JourneyRunExecutionActivityMetricsResponseTypeDef = TypedDict(
     "JourneyRunExecutionActivityMetricsResponseTypeDef",
     {
         "ActivityType": str,
         "ApplicationId": str,
         "JourneyActivityId": str,
         "JourneyId": str,
@@ -2642,22 +2911,20 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
-
 class GetJourneyRunExecutionMetricsRequestRequestTypeDef(
     _RequiredGetJourneyRunExecutionMetricsRequestRequestTypeDef,
     _OptionalGetJourneyRunExecutionMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 JourneyRunExecutionMetricsResponseTypeDef = TypedDict(
     "JourneyRunExecutionMetricsResponseTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
         "LastEvaluatedTime": str,
         "Metrics": Dict[str, str],
@@ -2677,42 +2944,38 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetJourneyRunsRequestRequestTypeDef(
     _RequiredGetJourneyRunsRequestRequestTypeDef, _OptionalGetJourneyRunsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetPushTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredGetPushTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalGetPushTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalGetPushTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class GetPushTemplateRequestRequestTypeDef(
     _RequiredGetPushTemplateRequestRequestTypeDef, _OptionalGetPushTemplateRequestRequestTypeDef
 ):
     pass
 
-
 GetRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "GetRecommenderConfigurationRequestRequestTypeDef",
     {
         "RecommenderId": str,
     },
 )
 
@@ -2737,22 +3000,20 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetSegmentExportJobsRequestRequestTypeDef(
     _RequiredGetSegmentExportJobsRequestRequestTypeDef,
     _OptionalGetSegmentExportJobsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetSegmentImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSegmentImportJobsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "SegmentId": str,
     },
 )
@@ -2761,22 +3022,20 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetSegmentImportJobsRequestRequestTypeDef(
     _RequiredGetSegmentImportJobsRequestRequestTypeDef,
     _OptionalGetSegmentImportJobsRequestRequestTypeDef,
 ):
     pass
 
-
 GetSegmentRequestRequestTypeDef = TypedDict(
     "GetSegmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "SegmentId": str,
     },
 )
@@ -2802,22 +3061,20 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetSegmentVersionsRequestRequestTypeDef(
     _RequiredGetSegmentVersionsRequestRequestTypeDef,
     _OptionalGetSegmentVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetSegmentsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSegmentsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalGetSegmentsRequestRequestTypeDef = TypedDict(
@@ -2825,21 +3082,19 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class GetSegmentsRequestRequestTypeDef(
     _RequiredGetSegmentsRequestRequestTypeDef, _OptionalGetSegmentsRequestRequestTypeDef
 ):
     pass
 
-
 GetSmsChannelRequestRequestTypeDef = TypedDict(
     "GetSmsChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2853,21 +3108,19 @@
     "_OptionalGetSmsTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class GetSmsTemplateRequestRequestTypeDef(
     _RequiredGetSmsTemplateRequestRequestTypeDef, _OptionalGetSmsTemplateRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredSMSTemplateResponseTypeDef = TypedDict(
     "_RequiredSMSTemplateResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
@@ -2883,21 +3136,19 @@
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
-
 class SMSTemplateResponseTypeDef(
     _RequiredSMSTemplateResponseTypeDef, _OptionalSMSTemplateResponseTypeDef
 ):
     pass
 
-
 GetUserEndpointsRequestRequestTypeDef = TypedDict(
     "GetUserEndpointsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "UserId": str,
     },
 )
@@ -2919,21 +3170,19 @@
     "_OptionalGetVoiceTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class GetVoiceTemplateRequestRequestTypeDef(
     _RequiredGetVoiceTemplateRequestRequestTypeDef, _OptionalGetVoiceTemplateRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredVoiceTemplateResponseTypeDef = TypedDict(
     "_RequiredVoiceTemplateResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
@@ -2950,21 +3199,19 @@
         "TemplateDescription": str,
         "Version": str,
         "VoiceId": str,
     },
     total=False,
 )
 
-
 class VoiceTemplateResponseTypeDef(
     _RequiredVoiceTemplateResponseTypeDef, _OptionalVoiceTemplateResponseTypeDef
 ):
     pass
 
-
 _RequiredImportJobResourceTypeDef = TypedDict(
     "_RequiredImportJobResourceTypeDef",
     {
         "Format": FormatType,
         "RoleArn": str,
         "S3Url": str,
     },
@@ -2977,93 +3224,155 @@
         "RegisterEndpoints": bool,
         "SegmentId": str,
         "SegmentName": str,
     },
     total=False,
 )
 
-
 class ImportJobResourceTypeDef(
     _RequiredImportJobResourceTypeDef, _OptionalImportJobResourceTypeDef
 ):
     pass
 
+InAppMessageBodyConfigOutputTypeDef = TypedDict(
+    "InAppMessageBodyConfigOutputTypeDef",
+    {
+        "Alignment": AlignmentType,
+        "Body": str,
+        "TextColor": str,
+    },
+)
 
 InAppMessageBodyConfigTypeDef = TypedDict(
     "InAppMessageBodyConfigTypeDef",
     {
         "Alignment": AlignmentType,
         "Body": str,
         "TextColor": str,
     },
 )
 
+_RequiredOverrideButtonConfigurationOutputTypeDef = TypedDict(
+    "_RequiredOverrideButtonConfigurationOutputTypeDef",
+    {
+        "ButtonAction": ButtonActionType,
+    },
+)
+_OptionalOverrideButtonConfigurationOutputTypeDef = TypedDict(
+    "_OptionalOverrideButtonConfigurationOutputTypeDef",
+    {
+        "Link": str,
+    },
+    total=False,
+)
+
+class OverrideButtonConfigurationOutputTypeDef(
+    _RequiredOverrideButtonConfigurationOutputTypeDef,
+    _OptionalOverrideButtonConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredOverrideButtonConfigurationTypeDef = TypedDict(
     "_RequiredOverrideButtonConfigurationTypeDef",
     {
         "ButtonAction": ButtonActionType,
     },
 )
 _OptionalOverrideButtonConfigurationTypeDef = TypedDict(
     "_OptionalOverrideButtonConfigurationTypeDef",
     {
         "Link": str,
     },
     total=False,
 )
 
-
 class OverrideButtonConfigurationTypeDef(
     _RequiredOverrideButtonConfigurationTypeDef, _OptionalOverrideButtonConfigurationTypeDef
 ):
     pass
 
+InAppMessageHeaderConfigOutputTypeDef = TypedDict(
+    "InAppMessageHeaderConfigOutputTypeDef",
+    {
+        "Alignment": AlignmentType,
+        "Header": str,
+        "TextColor": str,
+    },
+)
 
 InAppMessageHeaderConfigTypeDef = TypedDict(
     "InAppMessageHeaderConfigTypeDef",
     {
         "Alignment": AlignmentType,
         "Header": str,
         "TextColor": str,
     },
 )
 
+JourneyChannelSettingsOutputTypeDef = TypedDict(
+    "JourneyChannelSettingsOutputTypeDef",
+    {
+        "ConnectCampaignArn": str,
+        "ConnectCampaignExecutionRoleArn": str,
+    },
+    total=False,
+)
+
 JourneyChannelSettingsTypeDef = TypedDict(
     "JourneyChannelSettingsTypeDef",
     {
         "ConnectCampaignArn": str,
         "ConnectCampaignExecutionRoleArn": str,
     },
     total=False,
 )
 
+JourneyLimitsOutputTypeDef = TypedDict(
+    "JourneyLimitsOutputTypeDef",
+    {
+        "DailyCap": int,
+        "EndpointReentryCap": int,
+        "MessagesPerSecond": int,
+        "EndpointReentryInterval": str,
+    },
+    total=False,
+)
+
 JourneyLimitsTypeDef = TypedDict(
     "JourneyLimitsTypeDef",
     {
         "DailyCap": int,
         "EndpointReentryCap": int,
         "MessagesPerSecond": int,
         "EndpointReentryInterval": str,
     },
     total=False,
 )
 
+JourneyPushMessageOutputTypeDef = TypedDict(
+    "JourneyPushMessageOutputTypeDef",
+    {
+        "TimeToLive": str,
+    },
+    total=False,
+)
+
 JourneyPushMessageTypeDef = TypedDict(
     "JourneyPushMessageTypeDef",
     {
         "TimeToLive": str,
     },
     total=False,
 )
 
-JourneyScheduleTypeDef = TypedDict(
-    "JourneyScheduleTypeDef",
+JourneyScheduleOutputTypeDef = TypedDict(
+    "JourneyScheduleOutputTypeDef",
     {
-        "EndTime": Union[datetime, str],
-        "StartTime": Union[datetime, str],
+        "EndTime": datetime,
+        "StartTime": datetime,
         "Timezone": str,
     },
     total=False,
 )
 
 JourneyRunResponseTypeDef = TypedDict(
     "JourneyRunResponseTypeDef",
@@ -3071,26 +3380,48 @@
         "CreationTime": str,
         "LastUpdateTime": str,
         "RunId": str,
         "Status": JourneyRunStatusType,
     },
 )
 
+JourneySMSMessageOutputTypeDef = TypedDict(
+    "JourneySMSMessageOutputTypeDef",
+    {
+        "MessageType": MessageTypeType,
+        "OriginationNumber": str,
+        "SenderId": str,
+        "EntityId": str,
+        "TemplateId": str,
+    },
+    total=False,
+)
+
 JourneySMSMessageTypeDef = TypedDict(
     "JourneySMSMessageTypeDef",
     {
         "MessageType": MessageTypeType,
         "OriginationNumber": str,
         "SenderId": str,
         "EntityId": str,
         "TemplateId": str,
     },
     total=False,
 )
 
+JourneyScheduleTypeDef = TypedDict(
+    "JourneyScheduleTypeDef",
+    {
+        "EndTime": Union[datetime, str],
+        "StartTime": Union[datetime, str],
+        "Timezone": str,
+    },
+    total=False,
+)
+
 JourneyStateRequestTypeDef = TypedDict(
     "JourneyStateRequestTypeDef",
     {
         "State": StateType,
     },
     total=False,
 )
@@ -3106,30 +3437,28 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
-
 class ListJourneysRequestRequestTypeDef(
     _RequiredListJourneysRequestRequestTypeDef, _OptionalListJourneysRequestRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TagsModelTypeDef = TypedDict(
-    "TagsModelTypeDef",
+TagsModelOutputTypeDef = TypedDict(
+    "TagsModelOutputTypeDef",
     {
         "tags": Dict[str, str],
     },
 )
 
 _RequiredListTemplateVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplateVersionsRequestRequestTypeDef",
@@ -3143,33 +3472,50 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
-
 class ListTemplateVersionsRequestRequestTypeDef(
     _RequiredListTemplateVersionsRequestRequestTypeDef,
     _OptionalListTemplateVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListTemplatesRequestRequestTypeDef = TypedDict(
     "ListTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": str,
         "Prefix": str,
         "TemplateType": str,
     },
     total=False,
 )
 
+MessageOutputTypeDef = TypedDict(
+    "MessageOutputTypeDef",
+    {
+        "Action": ActionType,
+        "Body": str,
+        "ImageIconUrl": str,
+        "ImageSmallIconUrl": str,
+        "ImageUrl": str,
+        "JsonBody": str,
+        "MediaUrl": str,
+        "RawContent": str,
+        "SilentPush": bool,
+        "TimeToLive": int,
+        "Title": str,
+        "Url": str,
+    },
+    total=False,
+)
+
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "ImageIconUrl": str,
         "ImageSmallIconUrl": str,
@@ -3198,19 +3544,17 @@
         "MessageId": str,
         "StatusMessage": str,
         "UpdatedToken": str,
     },
     total=False,
 )
 
-
 class MessageResultTypeDef(_RequiredMessageResultTypeDef, _OptionalMessageResultTypeDef):
     pass
 
-
 NumberValidateRequestTypeDef = TypedDict(
     "NumberValidateRequestTypeDef",
     {
         "IsoCountryCode": str,
         "PhoneNumber": str,
     },
     total=False,
@@ -3233,14 +3577,23 @@
         "PhoneTypeCode": int,
         "Timezone": str,
         "ZipCode": str,
     },
     total=False,
 )
 
+OpenHoursRuleOutputTypeDef = TypedDict(
+    "OpenHoursRuleOutputTypeDef",
+    {
+        "StartTime": str,
+        "EndTime": str,
+    },
+    total=False,
+)
+
 OpenHoursRuleTypeDef = TypedDict(
     "OpenHoursRuleTypeDef",
     {
         "StartTime": str,
         "EndTime": str,
     },
     total=False,
@@ -3250,23 +3603,49 @@
     "WriteEventStreamTypeDef",
     {
         "DestinationStreamArn": str,
         "RoleArn": str,
     },
 )
 
+QuietTimeTypeDef = TypedDict(
+    "QuietTimeTypeDef",
+    {
+        "End": str,
+        "Start": str,
+    },
+    total=False,
+)
+
+RandomSplitEntryOutputTypeDef = TypedDict(
+    "RandomSplitEntryOutputTypeDef",
+    {
+        "NextActivity": str,
+        "Percentage": int,
+    },
+    total=False,
+)
+
 RandomSplitEntryTypeDef = TypedDict(
     "RandomSplitEntryTypeDef",
     {
         "NextActivity": str,
         "Percentage": int,
     },
     total=False,
 )
 
+RecencyDimensionOutputTypeDef = TypedDict(
+    "RecencyDimensionOutputTypeDef",
+    {
+        "Duration": DurationType,
+        "RecencyType": RecencyTypeType,
+    },
+)
+
 RecencyDimensionTypeDef = TypedDict(
     "RecencyDimensionTypeDef",
     {
         "Duration": DurationType,
         "RecencyType": RecencyTypeType,
     },
 )
@@ -3275,25 +3654,14 @@
     "UpdateAttributesRequestTypeDef",
     {
         "Blacklist": Sequence[str],
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
 ResultRowValueTypeDef = TypedDict(
     "ResultRowValueTypeDef",
     {
         "Key": str,
         "Type": str,
         "Value": str,
     },
@@ -3305,40 +3673,64 @@
         "Enabled": bool,
         "SenderId": str,
         "ShortCode": str,
     },
     total=False,
 )
 
+SegmentConditionOutputTypeDef = TypedDict(
+    "SegmentConditionOutputTypeDef",
+    {
+        "SegmentId": str,
+    },
+)
+
 SegmentConditionTypeDef = TypedDict(
     "SegmentConditionTypeDef",
     {
         "SegmentId": str,
     },
 )
 
+_RequiredSegmentReferenceOutputTypeDef = TypedDict(
+    "_RequiredSegmentReferenceOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalSegmentReferenceOutputTypeDef = TypedDict(
+    "_OptionalSegmentReferenceOutputTypeDef",
+    {
+        "Version": int,
+    },
+    total=False,
+)
+
+class SegmentReferenceOutputTypeDef(
+    _RequiredSegmentReferenceOutputTypeDef, _OptionalSegmentReferenceOutputTypeDef
+):
+    pass
+
 _RequiredSegmentReferenceTypeDef = TypedDict(
     "_RequiredSegmentReferenceTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalSegmentReferenceTypeDef = TypedDict(
     "_OptionalSegmentReferenceTypeDef",
     {
         "Version": int,
     },
     total=False,
 )
 
-
 class SegmentReferenceTypeDef(_RequiredSegmentReferenceTypeDef, _OptionalSegmentReferenceTypeDef):
     pass
 
-
 _RequiredSegmentImportResourceTypeDef = TypedDict(
     "_RequiredSegmentImportResourceTypeDef",
     {
         "ExternalId": str,
         "Format": FormatType,
         "RoleArn": str,
         "S3Url": str,
@@ -3349,21 +3741,19 @@
     "_OptionalSegmentImportResourceTypeDef",
     {
         "ChannelCounts": Dict[str, int],
     },
     total=False,
 )
 
-
 class SegmentImportResourceTypeDef(
     _RequiredSegmentImportResourceTypeDef, _OptionalSegmentImportResourceTypeDef
 ):
     pass
 
-
 _RequiredSendOTPMessageRequestParametersTypeDef = TypedDict(
     "_RequiredSendOTPMessageRequestParametersTypeDef",
     {
         "BrandName": str,
         "Channel": str,
         "DestinationIdentity": str,
         "OriginationIdentity": str,
@@ -3379,38 +3769,52 @@
         "Language": str,
         "TemplateId": str,
         "ValidityPeriod": int,
     },
     total=False,
 )
 
-
 class SendOTPMessageRequestParametersTypeDef(
     _RequiredSendOTPMessageRequestParametersTypeDef, _OptionalSendOTPMessageRequestParametersTypeDef
 ):
     pass
 
-
 SimpleEmailPartTypeDef = TypedDict(
     "SimpleEmailPartTypeDef",
     {
         "Charset": str,
         "Data": str,
     },
     total=False,
 )
 
+TagsModelTypeDef = TypedDict(
+    "TagsModelTypeDef",
+    {
+        "tags": Mapping[str, str],
+    },
+)
+
 TemplateActiveVersionRequestTypeDef = TypedDict(
     "TemplateActiveVersionRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+TemplateOutputTypeDef = TypedDict(
+    "TemplateOutputTypeDef",
+    {
+        "Name": str,
+        "Version": str,
+    },
+    total=False,
+)
+
 TemplateTypeDef = TypedDict(
     "TemplateTypeDef",
     {
         "Name": str,
         "Version": str,
     },
     total=False,
@@ -3433,19 +3837,17 @@
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
-
 class TemplateResponseTypeDef(_RequiredTemplateResponseTypeDef, _OptionalTemplateResponseTypeDef):
     pass
 
-
 _RequiredTemplateVersionResponseTypeDef = TypedDict(
     "_RequiredTemplateVersionResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": str,
@@ -3457,21 +3859,19 @@
         "DefaultSubstitutions": str,
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
-
 class TemplateVersionResponseTypeDef(
     _RequiredTemplateVersionResponseTypeDef, _OptionalTemplateVersionResponseTypeDef
 ):
     pass
 
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -3493,21 +3893,19 @@
         "RecommendationTransformerUri": str,
         "RecommendationsDisplayName": str,
         "RecommendationsPerMessage": int,
     },
     total=False,
 )
 
-
 class UpdateRecommenderConfigurationTypeDef(
     _RequiredUpdateRecommenderConfigurationTypeDef, _OptionalUpdateRecommenderConfigurationTypeDef
 ):
     pass
 
-
 VoiceChannelRequestTypeDef = TypedDict(
     "VoiceChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -3533,328 +3931,340 @@
     "UpdateAdmChannelRequestRequestTypeDef",
     {
         "ADMChannelRequest": ADMChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
 
-DeleteAdmChannelResponseTypeDef = TypedDict(
-    "DeleteAdmChannelResponseTypeDef",
+UpdateApnsChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsChannelRequestRequestTypeDef",
     {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSChannelRequest": APNSChannelRequestTypeDef,
+        "ApplicationId": str,
     },
 )
 
-GetAdmChannelResponseTypeDef = TypedDict(
-    "GetAdmChannelResponseTypeDef",
+UpdateApnsSandboxChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsSandboxChannelRequestRequestTypeDef",
     {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSSandboxChannelRequest": APNSSandboxChannelRequestTypeDef,
+        "ApplicationId": str,
     },
 )
 
-UpdateAdmChannelResponseTypeDef = TypedDict(
-    "UpdateAdmChannelResponseTypeDef",
+UpdateApnsVoipChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsVoipChannelRequestRequestTypeDef",
     {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSVoipChannelRequest": APNSVoipChannelRequestTypeDef,
+        "ApplicationId": str,
     },
 )
 
-UpdateApnsChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsChannelRequestRequestTypeDef",
+UpdateApnsVoipSandboxChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
     {
-        "APNSChannelRequest": APNSChannelRequestTypeDef,
+        "APNSVoipSandboxChannelRequest": APNSVoipSandboxChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
 
-DeleteApnsChannelResponseTypeDef = TypedDict(
-    "DeleteApnsChannelResponseTypeDef",
+_RequiredActivitiesResponseTypeDef = TypedDict(
+    "_RequiredActivitiesResponseTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Item": List[ActivityResponseTypeDef],
     },
 )
-
-GetApnsChannelResponseTypeDef = TypedDict(
-    "GetApnsChannelResponseTypeDef",
+_OptionalActivitiesResponseTypeDef = TypedDict(
+    "_OptionalActivitiesResponseTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "NextToken": str,
     },
+    total=False,
 )
 
-UpdateApnsChannelResponseTypeDef = TypedDict(
-    "UpdateApnsChannelResponseTypeDef",
+class ActivitiesResponseTypeDef(
+    _RequiredActivitiesResponseTypeDef, _OptionalActivitiesResponseTypeDef
+):
+    pass
+
+ApplicationsResponseTypeDef = TypedDict(
+    "ApplicationsResponseTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Item": List[ApplicationResponseTypeDef],
+        "NextToken": str,
     },
+    total=False,
 )
 
-UpdateApnsSandboxChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsSandboxChannelRequestRequestTypeDef",
+_RequiredApplicationSettingsResourceTypeDef = TypedDict(
+    "_RequiredApplicationSettingsResourceTypeDef",
     {
-        "APNSSandboxChannelRequest": APNSSandboxChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
-
-DeleteApnsSandboxChannelResponseTypeDef = TypedDict(
-    "DeleteApnsSandboxChannelResponseTypeDef",
+_OptionalApplicationSettingsResourceTypeDef = TypedDict(
+    "_OptionalApplicationSettingsResourceTypeDef",
     {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CampaignHook": CampaignHookOutputTypeDef,
+        "LastModifiedDate": str,
+        "Limits": CampaignLimitsOutputTypeDef,
+        "QuietTime": QuietTimeOutputTypeDef,
     },
+    total=False,
 )
 
-GetApnsSandboxChannelResponseTypeDef = TypedDict(
-    "GetApnsSandboxChannelResponseTypeDef",
-    {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+class ApplicationSettingsResourceTypeDef(
+    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
+):
+    pass
 
-UpdateApnsSandboxChannelResponseTypeDef = TypedDict(
-    "UpdateApnsSandboxChannelResponseTypeDef",
+UpdateBaiduChannelRequestRequestTypeDef = TypedDict(
+    "UpdateBaiduChannelRequestRequestTypeDef",
     {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApplicationId": str,
+        "BaiduChannelRequest": BaiduChannelRequestTypeDef,
     },
 )
 
-UpdateApnsVoipChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsVoipChannelRequestRequestTypeDef",
+ChannelsResponseTypeDef = TypedDict(
+    "ChannelsResponseTypeDef",
     {
-        "APNSVoipChannelRequest": APNSVoipChannelRequestTypeDef,
-        "ApplicationId": str,
+        "Channels": Dict[str, ChannelResponseTypeDef],
     },
 )
 
-DeleteApnsVoipChannelResponseTypeDef = TypedDict(
-    "DeleteApnsVoipChannelResponseTypeDef",
+ClosedDaysOutputTypeDef = TypedDict(
+    "ClosedDaysOutputTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EMAIL": List[ClosedDaysRuleOutputTypeDef],
+        "SMS": List[ClosedDaysRuleOutputTypeDef],
+        "PUSH": List[ClosedDaysRuleOutputTypeDef],
+        "VOICE": List[ClosedDaysRuleOutputTypeDef],
+        "CUSTOM": List[ClosedDaysRuleOutputTypeDef],
     },
+    total=False,
 )
 
-GetApnsVoipChannelResponseTypeDef = TypedDict(
-    "GetApnsVoipChannelResponseTypeDef",
+ClosedDaysTypeDef = TypedDict(
+    "ClosedDaysTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EMAIL": Sequence[ClosedDaysRuleTypeDef],
+        "SMS": Sequence[ClosedDaysRuleTypeDef],
+        "PUSH": Sequence[ClosedDaysRuleTypeDef],
+        "VOICE": Sequence[ClosedDaysRuleTypeDef],
+        "CUSTOM": Sequence[ClosedDaysRuleTypeDef],
     },
+    total=False,
 )
 
-UpdateApnsVoipChannelResponseTypeDef = TypedDict(
-    "UpdateApnsVoipChannelResponseTypeDef",
+WaitActivityOutputTypeDef = TypedDict(
+    "WaitActivityOutputTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "NextActivity": str,
+        "WaitTime": WaitTimeOutputTypeDef,
     },
+    total=False,
 )
 
-UpdateApnsVoipSandboxChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
+WaitActivityTypeDef = TypedDict(
+    "WaitActivityTypeDef",
     {
-        "APNSVoipSandboxChannelRequest": APNSVoipSandboxChannelRequestTypeDef,
-        "ApplicationId": str,
+        "NextActivity": str,
+        "WaitTime": WaitTimeTypeDef,
     },
+    total=False,
 )
 
-DeleteApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "DeleteApnsVoipSandboxChannelResponseTypeDef",
+CreateAppRequestRequestTypeDef = TypedDict(
+    "CreateAppRequestRequestTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CreateApplicationRequest": CreateApplicationRequestTypeDef,
     },
 )
 
-GetApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "GetApnsVoipSandboxChannelResponseTypeDef",
+CreateAppResponseTypeDef = TypedDict(
+    "CreateAppResponseTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApplicationResponse": ApplicationResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "UpdateApnsVoipSandboxChannelResponseTypeDef",
+DeleteAdmChannelResponseTypeDef = TypedDict(
+    "DeleteAdmChannelResponseTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredActivitiesResponseTypeDef = TypedDict(
-    "_RequiredActivitiesResponseTypeDef",
+DeleteApnsChannelResponseTypeDef = TypedDict(
+    "DeleteApnsChannelResponseTypeDef",
     {
-        "Item": List[ActivityResponseTypeDef],
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalActivitiesResponseTypeDef = TypedDict(
-    "_OptionalActivitiesResponseTypeDef",
+
+DeleteApnsSandboxChannelResponseTypeDef = TypedDict(
+    "DeleteApnsSandboxChannelResponseTypeDef",
     {
-        "NextToken": str,
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class ActivitiesResponseTypeDef(
-    _RequiredActivitiesResponseTypeDef, _OptionalActivitiesResponseTypeDef
-):
-    pass
-
-
-ApplicationsResponseTypeDef = TypedDict(
-    "ApplicationsResponseTypeDef",
+DeleteApnsVoipChannelResponseTypeDef = TypedDict(
+    "DeleteApnsVoipChannelResponseTypeDef",
     {
-        "Item": List[ApplicationResponseTypeDef],
-        "NextToken": str,
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-CreateAppResponseTypeDef = TypedDict(
-    "CreateAppResponseTypeDef",
+DeleteApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "DeleteApnsVoipSandboxChannelResponseTypeDef",
     {
-        "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAppResponseTypeDef = TypedDict(
     "DeleteAppResponseTypeDef",
     {
         "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetAppResponseTypeDef = TypedDict(
-    "GetAppResponseTypeDef",
+DeleteBaiduChannelResponseTypeDef = TypedDict(
+    "DeleteBaiduChannelResponseTypeDef",
     {
-        "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredApplicationSettingsResourceTypeDef = TypedDict(
-    "_RequiredApplicationSettingsResourceTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "ApplicationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalApplicationSettingsResourceTypeDef = TypedDict(
-    "_OptionalApplicationSettingsResourceTypeDef",
+
+GetAdmChannelResponseTypeDef = TypedDict(
+    "GetAdmChannelResponseTypeDef",
     {
-        "CampaignHook": CampaignHookTypeDef,
-        "LastModifiedDate": str,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+GetApnsChannelResponseTypeDef = TypedDict(
+    "GetApnsChannelResponseTypeDef",
+    {
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ApplicationSettingsResourceTypeDef(
-    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
-):
-    pass
-
-
-WriteApplicationSettingsRequestTypeDef = TypedDict(
-    "WriteApplicationSettingsRequestTypeDef",
+GetApnsSandboxChannelResponseTypeDef = TypedDict(
+    "GetApnsSandboxChannelResponseTypeDef",
     {
-        "CampaignHook": CampaignHookTypeDef,
-        "CloudWatchMetricsEnabled": bool,
-        "EventTaggingEnabled": bool,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-RemoveAttributesResponseTypeDef = TypedDict(
-    "RemoveAttributesResponseTypeDef",
+GetApnsVoipChannelResponseTypeDef = TypedDict(
+    "GetApnsVoipChannelResponseTypeDef",
     {
-        "AttributesResource": AttributesResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateBaiduChannelRequestRequestTypeDef = TypedDict(
-    "UpdateBaiduChannelRequestRequestTypeDef",
+GetApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "GetApnsVoipSandboxChannelResponseTypeDef",
     {
-        "ApplicationId": str,
-        "BaiduChannelRequest": BaiduChannelRequestTypeDef,
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteBaiduChannelResponseTypeDef = TypedDict(
-    "DeleteBaiduChannelResponseTypeDef",
+GetAppResponseTypeDef = TypedDict(
+    "GetAppResponseTypeDef",
     {
-        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApplicationResponse": ApplicationResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBaiduChannelResponseTypeDef = TypedDict(
     "GetBaiduChannelResponseTypeDef",
     {
         "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateBaiduChannelResponseTypeDef = TypedDict(
-    "UpdateBaiduChannelResponseTypeDef",
+RemoveAttributesResponseTypeDef = TypedDict(
+    "RemoveAttributesResponseTypeDef",
     {
-        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AttributesResource": AttributesResourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ChannelsResponseTypeDef = TypedDict(
-    "ChannelsResponseTypeDef",
+UpdateAdmChannelResponseTypeDef = TypedDict(
+    "UpdateAdmChannelResponseTypeDef",
     {
-        "Channels": Dict[str, ChannelResponseTypeDef],
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ClosedDaysTypeDef = TypedDict(
-    "ClosedDaysTypeDef",
+UpdateApnsChannelResponseTypeDef = TypedDict(
+    "UpdateApnsChannelResponseTypeDef",
     {
-        "EMAIL": Sequence[ClosedDaysRuleTypeDef],
-        "SMS": Sequence[ClosedDaysRuleTypeDef],
-        "PUSH": Sequence[ClosedDaysRuleTypeDef],
-        "VOICE": Sequence[ClosedDaysRuleTypeDef],
-        "CUSTOM": Sequence[ClosedDaysRuleTypeDef],
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-WaitActivityTypeDef = TypedDict(
-    "WaitActivityTypeDef",
+UpdateApnsSandboxChannelResponseTypeDef = TypedDict(
+    "UpdateApnsSandboxChannelResponseTypeDef",
     {
-        "NextActivity": str,
-        "WaitTime": WaitTimeTypeDef,
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-CreateAppRequestRequestTypeDef = TypedDict(
-    "CreateAppRequestRequestTypeDef",
+UpdateApnsVoipChannelResponseTypeDef = TypedDict(
+    "UpdateApnsVoipChannelResponseTypeDef",
     {
-        "CreateApplicationRequest": CreateApplicationRequestTypeDef,
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "UpdateApnsVoipSandboxChannelResponseTypeDef",
+    {
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBaiduChannelResponseTypeDef = TypedDict(
+    "UpdateBaiduChannelResponseTypeDef",
+    {
+        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEmailTemplateRequestRequestTypeDef = TypedDict(
     "CreateEmailTemplateRequestRequestTypeDef",
     {
         "EmailTemplateRequest": EmailTemplateRequestTypeDef,
@@ -3874,51 +4284,49 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
-
 class UpdateEmailTemplateRequestRequestTypeDef(
     _RequiredUpdateEmailTemplateRequestRequestTypeDef,
     _OptionalUpdateEmailTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 CreateEmailTemplateResponseTypeDef = TypedDict(
     "CreateEmailTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePushTemplateResponseTypeDef = TypedDict(
     "CreatePushTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSmsTemplateResponseTypeDef = TypedDict(
     "CreateSmsTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVoiceTemplateResponseTypeDef = TypedDict(
     "CreateVoiceTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateExportJobRequestRequestTypeDef = TypedDict(
     "CreateExportJobRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -3934,46 +4342,46 @@
     },
 )
 
 CreateInAppTemplateResponseTypeDef = TypedDict(
     "CreateInAppTemplateResponseTypeDef",
     {
         "TemplateCreateMessageBody": TemplateCreateMessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "CreateRecommenderConfigurationRequestRequestTypeDef",
     {
         "CreateRecommenderConfiguration": CreateRecommenderConfigurationTypeDef,
     },
 )
 
 CreateRecommenderConfigurationResponseTypeDef = TypedDict(
     "CreateRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRecommenderConfigurationResponseTypeDef = TypedDict(
     "DeleteRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommenderConfigurationResponseTypeDef = TypedDict(
     "GetRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListRecommenderConfigurationsResponseTypeDef = TypedDict(
     "_RequiredListRecommenderConfigurationsResponseTypeDef",
     {
         "Item": List[RecommenderConfigurationResponseTypeDef],
@@ -3983,27 +4391,25 @@
     "_OptionalListRecommenderConfigurationsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListRecommenderConfigurationsResponseTypeDef(
     _RequiredListRecommenderConfigurationsResponseTypeDef,
     _OptionalListRecommenderConfigurationsResponseTypeDef,
 ):
     pass
 
-
 UpdateRecommenderConfigurationResponseTypeDef = TypedDict(
     "UpdateRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSmsTemplateRequestRequestTypeDef = TypedDict(
     "CreateSmsTemplateRequestRequestTypeDef",
     {
         "SMSTemplateRequest": SMSTemplateRequestTypeDef,
@@ -4023,21 +4429,19 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
-
 class UpdateSmsTemplateRequestRequestTypeDef(
     _RequiredUpdateSmsTemplateRequestRequestTypeDef, _OptionalUpdateSmsTemplateRequestRequestTypeDef
 ):
     pass
 
-
 CreateVoiceTemplateRequestRequestTypeDef = TypedDict(
     "CreateVoiceTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "VoiceTemplateRequest": VoiceTemplateRequestTypeDef,
     },
 )
@@ -4054,47 +4458,42 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
-
 class UpdateVoiceTemplateRequestRequestTypeDef(
     _RequiredUpdateVoiceTemplateRequestRequestTypeDef,
     _OptionalUpdateVoiceTemplateRequestRequestTypeDef,
 ):
     pass
 
-
-CustomMessageActivityTypeDef = TypedDict(
-    "CustomMessageActivityTypeDef",
+CustomMessageActivityOutputTypeDef = TypedDict(
+    "CustomMessageActivityOutputTypeDef",
     {
         "DeliveryUri": str,
-        "EndpointTypes": Sequence[EndpointTypesElementType],
-        "MessageConfig": JourneyCustomMessageTypeDef,
+        "EndpointTypes": List[EndpointTypesElementType],
+        "MessageConfig": JourneyCustomMessageOutputTypeDef,
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
     },
     total=False,
 )
 
-PushNotificationTemplateRequestTypeDef = TypedDict(
-    "PushNotificationTemplateRequestTypeDef",
+CustomMessageActivityTypeDef = TypedDict(
+    "CustomMessageActivityTypeDef",
     {
-        "ADM": AndroidPushNotificationTemplateTypeDef,
-        "APNS": APNSPushNotificationTemplateTypeDef,
-        "Baidu": AndroidPushNotificationTemplateTypeDef,
-        "Default": DefaultPushNotificationTemplateTypeDef,
-        "DefaultSubstitutions": str,
-        "GCM": AndroidPushNotificationTemplateTypeDef,
-        "RecommenderId": str,
-        "tags": Mapping[str, str],
-        "TemplateDescription": str,
+        "DeliveryUri": str,
+        "EndpointTypes": Sequence[EndpointTypesElementType],
+        "MessageConfig": JourneyCustomMessageTypeDef,
+        "NextActivity": str,
+        "TemplateName": str,
+        "TemplateVersion": str,
     },
     total=False,
 )
 
 _RequiredPushNotificationTemplateResponseTypeDef = TypedDict(
     "_RequiredPushNotificationTemplateResponseTypeDef",
     {
@@ -4103,269 +4502,294 @@
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
     },
 )
 _OptionalPushNotificationTemplateResponseTypeDef = TypedDict(
     "_OptionalPushNotificationTemplateResponseTypeDef",
     {
-        "ADM": AndroidPushNotificationTemplateTypeDef,
-        "APNS": APNSPushNotificationTemplateTypeDef,
+        "ADM": AndroidPushNotificationTemplateOutputTypeDef,
+        "APNS": APNSPushNotificationTemplateOutputTypeDef,
         "Arn": str,
-        "Baidu": AndroidPushNotificationTemplateTypeDef,
-        "Default": DefaultPushNotificationTemplateTypeDef,
+        "Baidu": AndroidPushNotificationTemplateOutputTypeDef,
+        "Default": DefaultPushNotificationTemplateOutputTypeDef,
         "DefaultSubstitutions": str,
-        "GCM": AndroidPushNotificationTemplateTypeDef,
+        "GCM": AndroidPushNotificationTemplateOutputTypeDef,
         "RecommenderId": str,
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
-
 class PushNotificationTemplateResponseTypeDef(
     _RequiredPushNotificationTemplateResponseTypeDef,
     _OptionalPushNotificationTemplateResponseTypeDef,
 ):
     pass
 
+PushNotificationTemplateRequestTypeDef = TypedDict(
+    "PushNotificationTemplateRequestTypeDef",
+    {
+        "ADM": AndroidPushNotificationTemplateTypeDef,
+        "APNS": APNSPushNotificationTemplateTypeDef,
+        "Baidu": AndroidPushNotificationTemplateTypeDef,
+        "Default": DefaultPushNotificationTemplateTypeDef,
+        "DefaultSubstitutions": str,
+        "GCM": AndroidPushNotificationTemplateTypeDef,
+        "RecommenderId": str,
+        "tags": Mapping[str, str],
+        "TemplateDescription": str,
+    },
+    total=False,
+)
 
 DeleteEmailChannelResponseTypeDef = TypedDict(
     "DeleteEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEmailChannelResponseTypeDef = TypedDict(
     "GetEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEmailChannelResponseTypeDef = TypedDict(
     "UpdateEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEmailTemplateResponseTypeDef = TypedDict(
     "DeleteEmailTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInAppTemplateResponseTypeDef = TypedDict(
     "DeleteInAppTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePushTemplateResponseTypeDef = TypedDict(
     "DeletePushTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSmsTemplateResponseTypeDef = TypedDict(
     "DeleteSmsTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVoiceTemplateResponseTypeDef = TypedDict(
     "DeleteVoiceTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEmailTemplateResponseTypeDef = TypedDict(
     "UpdateEmailTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEndpointResponseTypeDef = TypedDict(
     "UpdateEndpointResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEndpointsBatchResponseTypeDef = TypedDict(
     "UpdateEndpointsBatchResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateInAppTemplateResponseTypeDef = TypedDict(
     "UpdateInAppTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePushTemplateResponseTypeDef = TypedDict(
     "UpdatePushTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSmsTemplateResponseTypeDef = TypedDict(
     "UpdateSmsTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTemplateActiveVersionResponseTypeDef = TypedDict(
     "UpdateTemplateActiveVersionResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVoiceTemplateResponseTypeDef = TypedDict(
     "UpdateVoiceTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEventStreamResponseTypeDef = TypedDict(
     "DeleteEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEventStreamResponseTypeDef = TypedDict(
     "GetEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutEventStreamResponseTypeDef = TypedDict(
     "PutEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteGcmChannelResponseTypeDef = TypedDict(
     "DeleteGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGcmChannelResponseTypeDef = TypedDict(
     "GetGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGcmChannelResponseTypeDef = TypedDict(
     "UpdateGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSmsChannelResponseTypeDef = TypedDict(
     "DeleteSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSmsChannelResponseTypeDef = TypedDict(
     "GetSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSmsChannelResponseTypeDef = TypedDict(
     "UpdateSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVoiceChannelResponseTypeDef = TypedDict(
     "DeleteVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceChannelResponseTypeDef = TypedDict(
     "GetVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVoiceChannelResponseTypeDef = TypedDict(
     "UpdateVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEmailChannelRequestRequestTypeDef = TypedDict(
     "UpdateEmailChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EmailChannelRequest": EmailChannelRequestTypeDef,
     },
 )
 
+EmailMessageActivityOutputTypeDef = TypedDict(
+    "EmailMessageActivityOutputTypeDef",
+    {
+        "MessageConfig": JourneyEmailMessageOutputTypeDef,
+        "NextActivity": str,
+        "TemplateName": str,
+        "TemplateVersion": str,
+    },
+    total=False,
+)
+
 EmailMessageActivityTypeDef = TypedDict(
     "EmailMessageActivityTypeDef",
     {
         "MessageConfig": JourneyEmailMessageTypeDef,
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
@@ -4373,15 +4797,15 @@
     total=False,
 )
 
 GetEmailTemplateResponseTypeDef = TypedDict(
     "GetEmailTemplateResponseTypeDef",
     {
         "EmailTemplateResponse": EmailTemplateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointBatchItemTypeDef = TypedDict(
     "EndpointBatchItemTypeDef",
     {
         "Address": str,
@@ -4414,36 +4838,14 @@
         "OptOut": str,
         "RequestId": str,
         "User": EndpointUserTypeDef,
     },
     total=False,
 )
 
-EndpointResponseTypeDef = TypedDict(
-    "EndpointResponseTypeDef",
-    {
-        "Address": str,
-        "ApplicationId": str,
-        "Attributes": Dict[str, List[str]],
-        "ChannelType": ChannelTypeType,
-        "CohortId": str,
-        "CreationDate": str,
-        "Demographic": EndpointDemographicTypeDef,
-        "EffectiveDate": str,
-        "EndpointStatus": str,
-        "Id": str,
-        "Location": EndpointLocationTypeDef,
-        "Metrics": Dict[str, float],
-        "OptOut": str,
-        "RequestId": str,
-        "User": EndpointUserTypeDef,
-    },
-    total=False,
-)
-
 PublicEndpointTypeDef = TypedDict(
     "PublicEndpointTypeDef",
     {
         "Address": str,
         "Attributes": Mapping[str, Sequence[str]],
         "ChannelType": ChannelTypeType,
         "Demographic": EndpointDemographicTypeDef,
@@ -4469,20 +4871,63 @@
     {
         "RequestId": str,
         "Result": Dict[str, Dict[str, EndpointMessageResultTypeDef]],
     },
     total=False,
 )
 
-
 class SendUsersMessageResponseTypeDef(
     _RequiredSendUsersMessageResponseTypeDef, _OptionalSendUsersMessageResponseTypeDef
 ):
     pass
 
+EndpointResponseTypeDef = TypedDict(
+    "EndpointResponseTypeDef",
+    {
+        "Address": str,
+        "ApplicationId": str,
+        "Attributes": Dict[str, List[str]],
+        "ChannelType": ChannelTypeType,
+        "CohortId": str,
+        "CreationDate": str,
+        "Demographic": EndpointDemographicOutputTypeDef,
+        "EffectiveDate": str,
+        "EndpointStatus": str,
+        "Id": str,
+        "Location": EndpointLocationOutputTypeDef,
+        "Metrics": Dict[str, float],
+        "OptOut": str,
+        "RequestId": str,
+        "User": EndpointUserOutputTypeDef,
+    },
+    total=False,
+)
+
+EventDimensionsOutputTypeDef = TypedDict(
+    "EventDimensionsOutputTypeDef",
+    {
+        "Attributes": Dict[str, AttributeDimensionOutputTypeDef],
+        "EventType": SetDimensionOutputTypeDef,
+        "Metrics": Dict[str, MetricDimensionOutputTypeDef],
+    },
+    total=False,
+)
+
+SegmentDemographicsOutputTypeDef = TypedDict(
+    "SegmentDemographicsOutputTypeDef",
+    {
+        "AppVersion": SetDimensionOutputTypeDef,
+        "Channel": SetDimensionOutputTypeDef,
+        "DeviceType": SetDimensionOutputTypeDef,
+        "Make": SetDimensionOutputTypeDef,
+        "Model": SetDimensionOutputTypeDef,
+        "Platform": SetDimensionOutputTypeDef,
+    },
+    total=False,
+)
 
 EventDimensionsTypeDef = TypedDict(
     "EventDimensionsTypeDef",
     {
         "Attributes": Mapping[str, AttributeDimensionTypeDef],
         "EventType": SetDimensionTypeDef,
         "Metrics": Mapping[str, MetricDimensionTypeDef],
@@ -4530,19 +4975,17 @@
         "Metrics": Mapping[str, float],
         "SdkName": str,
         "Session": SessionTypeDef,
     },
     total=False,
 )
 
-
 class EventTypeDef(_RequiredEventTypeDef, _OptionalEventTypeDef):
     pass
 
-
 _RequiredExportJobResponseTypeDef = TypedDict(
     "_RequiredExportJobResponseTypeDef",
     {
         "ApplicationId": str,
         "CreationDate": str,
         "Definition": ExportJobResourceTypeDef,
         "Id": str,
@@ -4560,97 +5003,112 @@
         "TotalFailures": int,
         "TotalPieces": int,
         "TotalProcessed": int,
     },
     total=False,
 )
 
-
 class ExportJobResponseTypeDef(
     _RequiredExportJobResponseTypeDef, _OptionalExportJobResponseTypeDef
 ):
     pass
 
-
 UpdateGcmChannelRequestRequestTypeDef = TypedDict(
     "UpdateGcmChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "GCMChannelRequest": GCMChannelRequestTypeDef,
     },
 )
 
+_RequiredGPSPointDimensionOutputTypeDef = TypedDict(
+    "_RequiredGPSPointDimensionOutputTypeDef",
+    {
+        "Coordinates": GPSCoordinatesOutputTypeDef,
+    },
+)
+_OptionalGPSPointDimensionOutputTypeDef = TypedDict(
+    "_OptionalGPSPointDimensionOutputTypeDef",
+    {
+        "RangeInKilometers": float,
+    },
+    total=False,
+)
+
+class GPSPointDimensionOutputTypeDef(
+    _RequiredGPSPointDimensionOutputTypeDef, _OptionalGPSPointDimensionOutputTypeDef
+):
+    pass
+
 _RequiredGPSPointDimensionTypeDef = TypedDict(
     "_RequiredGPSPointDimensionTypeDef",
     {
         "Coordinates": GPSCoordinatesTypeDef,
     },
 )
 _OptionalGPSPointDimensionTypeDef = TypedDict(
     "_OptionalGPSPointDimensionTypeDef",
     {
         "RangeInKilometers": float,
     },
     total=False,
 )
 
-
 class GPSPointDimensionTypeDef(
     _RequiredGPSPointDimensionTypeDef, _OptionalGPSPointDimensionTypeDef
 ):
     pass
 
-
 GetJourneyExecutionActivityMetricsResponseTypeDef = TypedDict(
     "GetJourneyExecutionActivityMetricsResponseTypeDef",
     {
         "JourneyExecutionActivityMetricsResponse": JourneyExecutionActivityMetricsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJourneyExecutionMetricsResponseTypeDef = TypedDict(
     "GetJourneyExecutionMetricsResponseTypeDef",
     {
         "JourneyExecutionMetricsResponse": JourneyExecutionMetricsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJourneyRunExecutionActivityMetricsResponseTypeDef = TypedDict(
     "GetJourneyRunExecutionActivityMetricsResponseTypeDef",
     {
         "JourneyRunExecutionActivityMetricsResponse": (
             JourneyRunExecutionActivityMetricsResponseTypeDef
         ),
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJourneyRunExecutionMetricsResponseTypeDef = TypedDict(
     "GetJourneyRunExecutionMetricsResponseTypeDef",
     {
         "JourneyRunExecutionMetricsResponse": JourneyRunExecutionMetricsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSmsTemplateResponseTypeDef = TypedDict(
     "GetSmsTemplateResponseTypeDef",
     {
         "SMSTemplateResponse": SMSTemplateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceTemplateResponseTypeDef = TypedDict(
     "GetVoiceTemplateResponseTypeDef",
     {
         "VoiceTemplateResponse": VoiceTemplateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportJobResponseTypeDef = TypedDict(
     "_RequiredImportJobResponseTypeDef",
     {
         "ApplicationId": str,
@@ -4671,32 +5129,52 @@
         "TotalFailures": int,
         "TotalPieces": int,
         "TotalProcessed": int,
     },
     total=False,
 )
 
-
 class ImportJobResponseTypeDef(
     _RequiredImportJobResponseTypeDef, _OptionalImportJobResponseTypeDef
 ):
     pass
 
+InAppMessageButtonOutputTypeDef = TypedDict(
+    "InAppMessageButtonOutputTypeDef",
+    {
+        "Android": OverrideButtonConfigurationOutputTypeDef,
+        "DefaultConfig": DefaultButtonConfigurationOutputTypeDef,
+        "IOS": OverrideButtonConfigurationOutputTypeDef,
+        "Web": OverrideButtonConfigurationOutputTypeDef,
+    },
+    total=False,
+)
 
 InAppMessageButtonTypeDef = TypedDict(
     "InAppMessageButtonTypeDef",
     {
         "Android": OverrideButtonConfigurationTypeDef,
         "DefaultConfig": DefaultButtonConfigurationTypeDef,
         "IOS": OverrideButtonConfigurationTypeDef,
         "Web": OverrideButtonConfigurationTypeDef,
     },
     total=False,
 )
 
+PushMessageActivityOutputTypeDef = TypedDict(
+    "PushMessageActivityOutputTypeDef",
+    {
+        "MessageConfig": JourneyPushMessageOutputTypeDef,
+        "NextActivity": str,
+        "TemplateName": str,
+        "TemplateVersion": str,
+    },
+    total=False,
+)
+
 PushMessageActivityTypeDef = TypedDict(
     "PushMessageActivityTypeDef",
     {
         "MessageConfig": JourneyPushMessageTypeDef,
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
@@ -4714,20 +5192,29 @@
     "_OptionalJourneyRunsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class JourneyRunsResponseTypeDef(
     _RequiredJourneyRunsResponseTypeDef, _OptionalJourneyRunsResponseTypeDef
 ):
     pass
 
+SMSMessageActivityOutputTypeDef = TypedDict(
+    "SMSMessageActivityOutputTypeDef",
+    {
+        "MessageConfig": JourneySMSMessageOutputTypeDef,
+        "NextActivity": str,
+        "TemplateName": str,
+        "TemplateVersion": str,
+    },
+    total=False,
+)
 
 SMSMessageActivityTypeDef = TypedDict(
     "SMSMessageActivityTypeDef",
     {
         "MessageConfig": JourneySMSMessageTypeDef,
         "NextActivity": str,
         "TemplateName": str,
@@ -4744,24 +5231,16 @@
         "JourneyStateRequest": JourneyStateRequestTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "TagsModel": TagsModelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "TagsModel": TagsModelTypeDef,
+        "TagsModel": TagsModelOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMessageResponseTypeDef = TypedDict(
     "_RequiredMessageResponseTypeDef",
     {
         "ApplicationId": str,
@@ -4773,34 +5252,44 @@
         "EndpointResult": Dict[str, EndpointMessageResultTypeDef],
         "RequestId": str,
         "Result": Dict[str, MessageResultTypeDef],
     },
     total=False,
 )
 
-
 class MessageResponseTypeDef(_RequiredMessageResponseTypeDef, _OptionalMessageResponseTypeDef):
     pass
 
-
 PhoneNumberValidateRequestRequestTypeDef = TypedDict(
     "PhoneNumberValidateRequestRequestTypeDef",
     {
         "NumberValidateRequest": NumberValidateRequestTypeDef,
     },
 )
 
 PhoneNumberValidateResponseTypeDef = TypedDict(
     "PhoneNumberValidateResponseTypeDef",
     {
         "NumberValidateResponse": NumberValidateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+OpenHoursOutputTypeDef = TypedDict(
+    "OpenHoursOutputTypeDef",
+    {
+        "EMAIL": Dict[DayOfWeekType, List[OpenHoursRuleOutputTypeDef]],
+        "SMS": Dict[DayOfWeekType, List[OpenHoursRuleOutputTypeDef]],
+        "PUSH": Dict[DayOfWeekType, List[OpenHoursRuleOutputTypeDef]],
+        "VOICE": Dict[DayOfWeekType, List[OpenHoursRuleOutputTypeDef]],
+        "CUSTOM": Dict[DayOfWeekType, List[OpenHoursRuleOutputTypeDef]],
+    },
+    total=False,
+)
+
 OpenHoursTypeDef = TypedDict(
     "OpenHoursTypeDef",
     {
         "EMAIL": Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]],
         "SMS": Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]],
         "PUSH": Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]],
         "VOICE": Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]],
@@ -4813,22 +5302,50 @@
     "PutEventStreamRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "WriteEventStream": WriteEventStreamTypeDef,
     },
 )
 
+WriteApplicationSettingsRequestTypeDef = TypedDict(
+    "WriteApplicationSettingsRequestTypeDef",
+    {
+        "CampaignHook": CampaignHookTypeDef,
+        "CloudWatchMetricsEnabled": bool,
+        "EventTaggingEnabled": bool,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
+    },
+    total=False,
+)
+
+RandomSplitActivityOutputTypeDef = TypedDict(
+    "RandomSplitActivityOutputTypeDef",
+    {
+        "Branches": List[RandomSplitEntryOutputTypeDef],
+    },
+    total=False,
+)
+
 RandomSplitActivityTypeDef = TypedDict(
     "RandomSplitActivityTypeDef",
     {
         "Branches": Sequence[RandomSplitEntryTypeDef],
     },
     total=False,
 )
 
+SegmentBehaviorsOutputTypeDef = TypedDict(
+    "SegmentBehaviorsOutputTypeDef",
+    {
+        "Recency": RecencyDimensionOutputTypeDef,
+    },
+    total=False,
+)
+
 SegmentBehaviorsTypeDef = TypedDict(
     "SegmentBehaviorsTypeDef",
     {
         "Recency": RecencyDimensionTypeDef,
     },
     total=False,
 )
@@ -4872,23 +5389,42 @@
         "HtmlPart": SimpleEmailPartTypeDef,
         "Subject": SimpleEmailPartTypeDef,
         "TextPart": SimpleEmailPartTypeDef,
     },
     total=False,
 )
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagsModel": TagsModelTypeDef,
+    },
+)
+
 UpdateTemplateActiveVersionRequestRequestTypeDef = TypedDict(
     "UpdateTemplateActiveVersionRequestRequestTypeDef",
     {
         "TemplateActiveVersionRequest": TemplateActiveVersionRequestTypeDef,
         "TemplateName": str,
         "TemplateType": str,
     },
 )
 
+TemplateConfigurationOutputTypeDef = TypedDict(
+    "TemplateConfigurationOutputTypeDef",
+    {
+        "EmailTemplate": TemplateOutputTypeDef,
+        "PushTemplate": TemplateOutputTypeDef,
+        "SMSTemplate": TemplateOutputTypeDef,
+        "VoiceTemplate": TemplateOutputTypeDef,
+    },
+    total=False,
+)
+
 TemplateConfigurationTypeDef = TypedDict(
     "TemplateConfigurationTypeDef",
     {
         "EmailTemplate": TemplateTypeDef,
         "PushTemplate": TemplateTypeDef,
         "SMSTemplate": TemplateTypeDef,
         "VoiceTemplate": TemplateTypeDef,
@@ -4906,21 +5442,19 @@
     "_OptionalTemplatesResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class TemplatesResponseTypeDef(
     _RequiredTemplatesResponseTypeDef, _OptionalTemplatesResponseTypeDef
 ):
     pass
 
-
 _RequiredTemplateVersionsResponseTypeDef = TypedDict(
     "_RequiredTemplateVersionsResponseTypeDef",
     {
         "Item": List[TemplateVersionResponseTypeDef],
     },
 )
 _OptionalTemplateVersionsResponseTypeDef = TypedDict(
@@ -4929,21 +5463,19 @@
         "Message": str,
         "NextToken": str,
         "RequestID": str,
     },
     total=False,
 )
 
-
 class TemplateVersionsResponseTypeDef(
     _RequiredTemplateVersionsResponseTypeDef, _OptionalTemplateVersionsResponseTypeDef
 ):
     pass
 
-
 UpdateRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateRecommenderConfigurationRequestRequestTypeDef",
     {
         "RecommenderId": str,
         "UpdateRecommenderConfiguration": UpdateRecommenderConfigurationTypeDef,
     },
 )
@@ -4956,15 +5488,15 @@
     },
 )
 
 VerifyOTPMessageResponseTypeDef = TypedDict(
     "VerifyOTPMessageResponseTypeDef",
     {
         "VerificationResponse": VerificationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VerifyOTPMessageRequestRequestTypeDef = TypedDict(
     "VerifyOTPMessageRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -4972,63 +5504,63 @@
     },
 )
 
 GetCampaignActivitiesResponseTypeDef = TypedDict(
     "GetCampaignActivitiesResponseTypeDef",
     {
         "ActivitiesResponse": ActivitiesResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAppsResponseTypeDef = TypedDict(
     "GetAppsResponseTypeDef",
     {
         "ApplicationsResponse": ApplicationsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApplicationSettingsResponseTypeDef = TypedDict(
     "GetApplicationSettingsResponseTypeDef",
     {
         "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationSettingsResponseTypeDef = TypedDict(
     "UpdateApplicationSettingsResponseTypeDef",
     {
         "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateApplicationSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateApplicationSettingsRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "WriteApplicationSettingsRequest": WriteApplicationSettingsRequestTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChannelsResponseTypeDef = TypedDict(
     "GetChannelsResponseTypeDef",
     {
         "ChannelsResponse": ChannelsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommenderConfigurationsResponseTypeDef = TypedDict(
     "GetRecommenderConfigurationsResponseTypeDef",
     {
         "ListRecommenderConfigurationsResponse": ListRecommenderConfigurationsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPushTemplateResponseTypeDef = TypedDict(
+    "GetPushTemplateResponseTypeDef",
+    {
+        "PushNotificationTemplateResponse": PushNotificationTemplateResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePushTemplateRequestRequestTypeDef = TypedDict(
     "CreatePushTemplateRequestRequestTypeDef",
     {
         "PushNotificationTemplateRequest": PushNotificationTemplateRequestTypeDef,
@@ -5048,30 +5580,20 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
-
 class UpdatePushTemplateRequestRequestTypeDef(
     _RequiredUpdatePushTemplateRequestRequestTypeDef,
     _OptionalUpdatePushTemplateRequestRequestTypeDef,
 ):
     pass
 
-
-GetPushTemplateResponseTypeDef = TypedDict(
-    "GetPushTemplateResponseTypeDef",
-    {
-        "PushNotificationTemplateResponse": PushNotificationTemplateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EndpointBatchRequestTypeDef = TypedDict(
     "EndpointBatchRequestTypeDef",
     {
         "Item": Sequence[EndpointBatchItemTypeDef],
     },
 )
 
@@ -5080,42 +5602,67 @@
     {
         "ApplicationId": str,
         "EndpointId": str,
         "EndpointRequest": EndpointRequestTypeDef,
     },
 )
 
+SendUsersMessagesResponseTypeDef = TypedDict(
+    "SendUsersMessagesResponseTypeDef",
+    {
+        "SendUsersMessageResponse": SendUsersMessageResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeleteEndpointResponseTypeDef = TypedDict(
     "DeleteEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointsResponseTypeDef = TypedDict(
     "EndpointsResponseTypeDef",
     {
         "Item": List[EndpointResponseTypeDef],
     },
 )
 
 GetEndpointResponseTypeDef = TypedDict(
     "GetEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SendUsersMessagesResponseTypeDef = TypedDict(
-    "SendUsersMessagesResponseTypeDef",
+CampaignEventFilterOutputTypeDef = TypedDict(
+    "CampaignEventFilterOutputTypeDef",
     {
-        "SendUsersMessageResponse": SendUsersMessageResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Dimensions": EventDimensionsOutputTypeDef,
+        "FilterType": FilterTypeType,
+    },
+)
+
+EventConditionOutputTypeDef = TypedDict(
+    "EventConditionOutputTypeDef",
+    {
+        "Dimensions": EventDimensionsOutputTypeDef,
+        "MessageActivity": str,
+    },
+    total=False,
+)
+
+EventFilterOutputTypeDef = TypedDict(
+    "EventFilterOutputTypeDef",
+    {
+        "Dimensions": EventDimensionsOutputTypeDef,
+        "FilterType": FilterTypeType,
     },
 )
 
 CampaignEventFilterTypeDef = TypedDict(
     "CampaignEventFilterTypeDef",
     {
         "Dimensions": EventDimensionsTypeDef,
@@ -5156,15 +5703,15 @@
     },
 )
 
 CreateExportJobResponseTypeDef = TypedDict(
     "CreateExportJobResponseTypeDef",
     {
         "ExportJobResponse": ExportJobResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredExportJobsResponseTypeDef = TypedDict(
     "_RequiredExportJobsResponseTypeDef",
     {
         "Item": List[ExportJobResponseTypeDef],
@@ -5174,27 +5721,34 @@
     "_OptionalExportJobsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ExportJobsResponseTypeDef(
     _RequiredExportJobsResponseTypeDef, _OptionalExportJobsResponseTypeDef
 ):
     pass
 
-
 GetExportJobResponseTypeDef = TypedDict(
     "GetExportJobResponseTypeDef",
     {
         "ExportJobResponse": ExportJobResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SegmentLocationOutputTypeDef = TypedDict(
+    "SegmentLocationOutputTypeDef",
+    {
+        "Country": SetDimensionOutputTypeDef,
+        "GPSPoint": GPSPointDimensionOutputTypeDef,
     },
+    total=False,
 )
 
 SegmentLocationTypeDef = TypedDict(
     "SegmentLocationTypeDef",
     {
         "Country": SetDimensionTypeDef,
         "GPSPoint": GPSPointDimensionTypeDef,
@@ -5202,23 +5756,23 @@
     total=False,
 )
 
 CreateImportJobResponseTypeDef = TypedDict(
     "CreateImportJobResponseTypeDef",
     {
         "ImportJobResponse": ImportJobResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetImportJobResponseTypeDef = TypedDict(
     "GetImportJobResponseTypeDef",
     {
         "ImportJobResponse": ImportJobResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportJobsResponseTypeDef = TypedDict(
     "_RequiredImportJobsResponseTypeDef",
     {
         "Item": List[ImportJobResponseTypeDef],
@@ -5228,20 +5782,31 @@
     "_OptionalImportJobsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ImportJobsResponseTypeDef(
     _RequiredImportJobsResponseTypeDef, _OptionalImportJobsResponseTypeDef
 ):
     pass
 
+InAppMessageContentOutputTypeDef = TypedDict(
+    "InAppMessageContentOutputTypeDef",
+    {
+        "BackgroundColor": str,
+        "BodyConfig": InAppMessageBodyConfigOutputTypeDef,
+        "HeaderConfig": InAppMessageHeaderConfigOutputTypeDef,
+        "ImageUrl": str,
+        "PrimaryBtn": InAppMessageButtonOutputTypeDef,
+        "SecondaryBtn": InAppMessageButtonOutputTypeDef,
+    },
+    total=False,
+)
 
 InAppMessageContentTypeDef = TypedDict(
     "InAppMessageContentTypeDef",
     {
         "BackgroundColor": str,
         "BodyConfig": InAppMessageBodyConfigTypeDef,
         "HeaderConfig": InAppMessageHeaderConfigTypeDef,
@@ -5252,31 +5817,39 @@
     total=False,
 )
 
 GetJourneyRunsResponseTypeDef = TypedDict(
     "GetJourneyRunsResponseTypeDef",
     {
         "JourneyRunsResponse": JourneyRunsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendMessagesResponseTypeDef = TypedDict(
     "SendMessagesResponseTypeDef",
     {
         "MessageResponse": MessageResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendOTPMessageResponseTypeDef = TypedDict(
     "SendOTPMessageResponseTypeDef",
     {
         "MessageResponse": MessageResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApplicationSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateApplicationSettingsRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "WriteApplicationSettingsRequest": WriteApplicationSettingsRequestTypeDef,
     },
 )
 
 BaseKpiResultTypeDef = TypedDict(
     "BaseKpiResultTypeDef",
     {
         "Rows": List[ResultRowTypeDef],
@@ -5297,23 +5870,23 @@
     total=False,
 )
 
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "TemplatesResponse": TemplatesResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTemplateVersionsResponseTypeDef = TypedDict(
     "ListTemplateVersionsResponseTypeDef",
     {
         "TemplateVersionsResponse": TemplateVersionsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEndpointsBatchRequestRequestTypeDef = TypedDict(
     "UpdateEndpointsBatchRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -5321,32 +5894,63 @@
     },
 )
 
 DeleteUserEndpointsResponseTypeDef = TypedDict(
     "DeleteUserEndpointsResponseTypeDef",
     {
         "EndpointsResponse": EndpointsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserEndpointsResponseTypeDef = TypedDict(
     "GetUserEndpointsResponseTypeDef",
     {
         "EndpointsResponse": EndpointsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InAppCampaignScheduleTypeDef = TypedDict(
     "InAppCampaignScheduleTypeDef",
     {
         "EndDate": str,
-        "EventFilter": CampaignEventFilterTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "EventFilter": CampaignEventFilterOutputTypeDef,
+        "QuietTime": QuietTimeOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredScheduleOutputTypeDef = TypedDict(
+    "_RequiredScheduleOutputTypeDef",
+    {
+        "StartTime": str,
+    },
+)
+_OptionalScheduleOutputTypeDef = TypedDict(
+    "_OptionalScheduleOutputTypeDef",
+    {
+        "EndTime": str,
+        "EventFilter": CampaignEventFilterOutputTypeDef,
+        "Frequency": FrequencyType,
+        "IsLocalTime": bool,
+        "QuietTime": QuietTimeOutputTypeDef,
+        "Timezone": str,
+    },
+    total=False,
+)
+
+class ScheduleOutputTypeDef(_RequiredScheduleOutputTypeDef, _OptionalScheduleOutputTypeDef):
+    pass
+
+EventStartConditionOutputTypeDef = TypedDict(
+    "EventStartConditionOutputTypeDef",
+    {
+        "EventFilter": EventFilterOutputTypeDef,
+        "SegmentId": str,
     },
     total=False,
 )
 
 _RequiredScheduleTypeDef = TypedDict(
     "_RequiredScheduleTypeDef",
     {
@@ -5362,57 +5966,68 @@
         "IsLocalTime": bool,
         "QuietTime": QuietTimeTypeDef,
         "Timezone": str,
     },
     total=False,
 )
 
-
 class ScheduleTypeDef(_RequiredScheduleTypeDef, _OptionalScheduleTypeDef):
     pass
 
-
 EventStartConditionTypeDef = TypedDict(
     "EventStartConditionTypeDef",
     {
         "EventFilter": EventFilterTypeDef,
         "SegmentId": str,
     },
     total=False,
 )
 
 PutEventsResponseTypeDef = TypedDict(
     "PutEventsResponseTypeDef",
     {
         "EventsResponse": EventsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventsRequestTypeDef = TypedDict(
     "EventsRequestTypeDef",
     {
         "BatchItem": Mapping[str, EventsBatchTypeDef],
     },
 )
 
 GetExportJobsResponseTypeDef = TypedDict(
     "GetExportJobsResponseTypeDef",
     {
         "ExportJobsResponse": ExportJobsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentExportJobsResponseTypeDef = TypedDict(
     "GetSegmentExportJobsResponseTypeDef",
     {
         "ExportJobsResponse": ExportJobsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SegmentDimensionsOutputTypeDef = TypedDict(
+    "SegmentDimensionsOutputTypeDef",
+    {
+        "Attributes": Dict[str, AttributeDimensionOutputTypeDef],
+        "Behavior": SegmentBehaviorsOutputTypeDef,
+        "Demographic": SegmentDemographicsOutputTypeDef,
+        "Location": SegmentLocationOutputTypeDef,
+        "Metrics": Dict[str, MetricDimensionOutputTypeDef],
+        "UserAttributes": Dict[str, AttributeDimensionOutputTypeDef],
     },
+    total=False,
 )
 
 SegmentDimensionsTypeDef = TypedDict(
     "SegmentDimensionsTypeDef",
     {
         "Attributes": Mapping[str, AttributeDimensionTypeDef],
         "Behavior": SegmentBehaviorsTypeDef,
@@ -5424,88 +6039,97 @@
     total=False,
 )
 
 GetImportJobsResponseTypeDef = TypedDict(
     "GetImportJobsResponseTypeDef",
     {
         "ImportJobsResponse": ImportJobsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentImportJobsResponseTypeDef = TypedDict(
     "GetSegmentImportJobsResponseTypeDef",
     {
         "ImportJobsResponse": ImportJobsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CampaignInAppMessageTypeDef = TypedDict(
-    "CampaignInAppMessageTypeDef",
+CampaignInAppMessageOutputTypeDef = TypedDict(
+    "CampaignInAppMessageOutputTypeDef",
     {
         "Body": str,
-        "Content": Sequence[InAppMessageContentTypeDef],
-        "CustomConfig": Mapping[str, str],
+        "Content": List[InAppMessageContentOutputTypeDef],
+        "CustomConfig": Dict[str, str],
         "Layout": LayoutType,
     },
     total=False,
 )
 
 InAppMessageTypeDef = TypedDict(
     "InAppMessageTypeDef",
     {
-        "Content": List[InAppMessageContentTypeDef],
+        "Content": List[InAppMessageContentOutputTypeDef],
         "CustomConfig": Dict[str, str],
         "Layout": LayoutType,
     },
     total=False,
 )
 
-InAppTemplateRequestTypeDef = TypedDict(
-    "InAppTemplateRequestTypeDef",
-    {
-        "Content": Sequence[InAppMessageContentTypeDef],
-        "CustomConfig": Mapping[str, str],
-        "Layout": LayoutType,
-        "tags": Mapping[str, str],
-        "TemplateDescription": str,
-    },
-    total=False,
-)
-
 _RequiredInAppTemplateResponseTypeDef = TypedDict(
     "_RequiredInAppTemplateResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
     },
 )
 _OptionalInAppTemplateResponseTypeDef = TypedDict(
     "_OptionalInAppTemplateResponseTypeDef",
     {
         "Arn": str,
-        "Content": List[InAppMessageContentTypeDef],
+        "Content": List[InAppMessageContentOutputTypeDef],
         "CustomConfig": Dict[str, str],
         "Layout": LayoutType,
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
-
 class InAppTemplateResponseTypeDef(
     _RequiredInAppTemplateResponseTypeDef, _OptionalInAppTemplateResponseTypeDef
 ):
     pass
 
+CampaignInAppMessageTypeDef = TypedDict(
+    "CampaignInAppMessageTypeDef",
+    {
+        "Body": str,
+        "Content": Sequence[InAppMessageContentTypeDef],
+        "CustomConfig": Mapping[str, str],
+        "Layout": LayoutType,
+    },
+    total=False,
+)
+
+InAppTemplateRequestTypeDef = TypedDict(
+    "InAppTemplateRequestTypeDef",
+    {
+        "Content": Sequence[InAppMessageContentTypeDef],
+        "CustomConfig": Mapping[str, str],
+        "Layout": LayoutType,
+        "tags": Mapping[str, str],
+        "TemplateDescription": str,
+    },
+    total=False,
+)
 
 _RequiredApplicationDateRangeKpiResponseTypeDef = TypedDict(
     "_RequiredApplicationDateRangeKpiResponseTypeDef",
     {
         "ApplicationId": str,
         "EndTime": datetime,
         "KpiName": str,
@@ -5517,21 +6141,19 @@
     "_OptionalApplicationDateRangeKpiResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ApplicationDateRangeKpiResponseTypeDef(
     _RequiredApplicationDateRangeKpiResponseTypeDef, _OptionalApplicationDateRangeKpiResponseTypeDef
 ):
     pass
 
-
 _RequiredCampaignDateRangeKpiResponseTypeDef = TypedDict(
     "_RequiredCampaignDateRangeKpiResponseTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
         "EndTime": datetime,
         "KpiName": str,
@@ -5543,21 +6165,19 @@
     "_OptionalCampaignDateRangeKpiResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class CampaignDateRangeKpiResponseTypeDef(
     _RequiredCampaignDateRangeKpiResponseTypeDef, _OptionalCampaignDateRangeKpiResponseTypeDef
 ):
     pass
 
-
 _RequiredJourneyDateRangeKpiResponseTypeDef = TypedDict(
     "_RequiredJourneyDateRangeKpiResponseTypeDef",
     {
         "ApplicationId": str,
         "EndTime": datetime,
         "JourneyId": str,
         "KpiName": str,
@@ -5569,21 +6189,19 @@
     "_OptionalJourneyDateRangeKpiResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class JourneyDateRangeKpiResponseTypeDef(
     _RequiredJourneyDateRangeKpiResponseTypeDef, _OptionalJourneyDateRangeKpiResponseTypeDef
 ):
     pass
 
-
 DirectMessageConfigurationTypeDef = TypedDict(
     "DirectMessageConfigurationTypeDef",
     {
         "ADMMessage": ADMMessageTypeDef,
         "APNSMessage": APNSMessageTypeDef,
         "BaiduMessage": BaiduMessageTypeDef,
         "DefaultMessage": DefaultMessageTypeDef,
@@ -5592,14 +6210,24 @@
         "GCMMessage": GCMMessageTypeDef,
         "SMSMessage": SMSMessageTypeDef,
         "VoiceMessage": VoiceMessageTypeDef,
     },
     total=False,
 )
 
+StartConditionOutputTypeDef = TypedDict(
+    "StartConditionOutputTypeDef",
+    {
+        "Description": str,
+        "EventStartCondition": EventStartConditionOutputTypeDef,
+        "SegmentStartCondition": SegmentConditionOutputTypeDef,
+    },
+    total=False,
+)
+
 StartConditionTypeDef = TypedDict(
     "StartConditionTypeDef",
     {
         "Description": str,
         "EventStartCondition": EventStartConditionTypeDef,
         "SegmentStartCondition": SegmentConditionTypeDef,
     },
@@ -5610,14 +6238,35 @@
     "PutEventsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EventsRequest": EventsRequestTypeDef,
     },
 )
 
+SegmentGroupOutputTypeDef = TypedDict(
+    "SegmentGroupOutputTypeDef",
+    {
+        "Dimensions": List[SegmentDimensionsOutputTypeDef],
+        "SourceSegments": List[SegmentReferenceOutputTypeDef],
+        "SourceType": SourceTypeType,
+        "Type": TypeType,
+    },
+    total=False,
+)
+
+SimpleConditionOutputTypeDef = TypedDict(
+    "SimpleConditionOutputTypeDef",
+    {
+        "EventCondition": EventConditionOutputTypeDef,
+        "SegmentCondition": SegmentConditionOutputTypeDef,
+        "SegmentDimensions": SegmentDimensionsOutputTypeDef,
+    },
+    total=False,
+)
+
 SegmentGroupTypeDef = TypedDict(
     "SegmentGroupTypeDef",
     {
         "Dimensions": Sequence[SegmentDimensionsTypeDef],
         "SourceSegments": Sequence[SegmentReferenceTypeDef],
         "SourceType": SourceTypeType,
         "Type": TypeType,
@@ -5631,26 +6280,26 @@
         "EventCondition": EventConditionTypeDef,
         "SegmentCondition": SegmentConditionTypeDef,
         "SegmentDimensions": SegmentDimensionsTypeDef,
     },
     total=False,
 )
 
-MessageConfigurationTypeDef = TypedDict(
-    "MessageConfigurationTypeDef",
+MessageConfigurationOutputTypeDef = TypedDict(
+    "MessageConfigurationOutputTypeDef",
     {
-        "ADMMessage": MessageTypeDef,
-        "APNSMessage": MessageTypeDef,
-        "BaiduMessage": MessageTypeDef,
-        "CustomMessage": CampaignCustomMessageTypeDef,
-        "DefaultMessage": MessageTypeDef,
-        "EmailMessage": CampaignEmailMessageTypeDef,
-        "GCMMessage": MessageTypeDef,
-        "SMSMessage": CampaignSmsMessageTypeDef,
-        "InAppMessage": CampaignInAppMessageTypeDef,
+        "ADMMessage": MessageOutputTypeDef,
+        "APNSMessage": MessageOutputTypeDef,
+        "BaiduMessage": MessageOutputTypeDef,
+        "CustomMessage": CampaignCustomMessageOutputTypeDef,
+        "DefaultMessage": MessageOutputTypeDef,
+        "EmailMessage": CampaignEmailMessageOutputTypeDef,
+        "GCMMessage": MessageOutputTypeDef,
+        "SMSMessage": CampaignSmsMessageOutputTypeDef,
+        "InAppMessage": CampaignInAppMessageOutputTypeDef,
     },
     total=False,
 )
 
 InAppMessageCampaignTypeDef = TypedDict(
     "InAppMessageCampaignTypeDef",
     {
@@ -5662,14 +6311,38 @@
         "SessionCap": int,
         "TotalCap": int,
         "TreatmentId": str,
     },
     total=False,
 )
 
+GetInAppTemplateResponseTypeDef = TypedDict(
+    "GetInAppTemplateResponseTypeDef",
+    {
+        "InAppTemplateResponse": InAppTemplateResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MessageConfigurationTypeDef = TypedDict(
+    "MessageConfigurationTypeDef",
+    {
+        "ADMMessage": MessageTypeDef,
+        "APNSMessage": MessageTypeDef,
+        "BaiduMessage": MessageTypeDef,
+        "CustomMessage": CampaignCustomMessageTypeDef,
+        "DefaultMessage": MessageTypeDef,
+        "EmailMessage": CampaignEmailMessageTypeDef,
+        "GCMMessage": MessageTypeDef,
+        "SMSMessage": CampaignSmsMessageTypeDef,
+        "InAppMessage": CampaignInAppMessageTypeDef,
+    },
+    total=False,
+)
+
 CreateInAppTemplateRequestRequestTypeDef = TypedDict(
     "CreateInAppTemplateRequestRequestTypeDef",
     {
         "InAppTemplateRequest": InAppTemplateRequestTypeDef,
         "TemplateName": str,
     },
 )
@@ -5686,51 +6359,41 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
-
 class UpdateInAppTemplateRequestRequestTypeDef(
     _RequiredUpdateInAppTemplateRequestRequestTypeDef,
     _OptionalUpdateInAppTemplateRequestRequestTypeDef,
 ):
     pass
 
-
-GetInAppTemplateResponseTypeDef = TypedDict(
-    "GetInAppTemplateResponseTypeDef",
-    {
-        "InAppTemplateResponse": InAppTemplateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetApplicationDateRangeKpiResponseTypeDef = TypedDict(
     "GetApplicationDateRangeKpiResponseTypeDef",
     {
         "ApplicationDateRangeKpiResponse": ApplicationDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCampaignDateRangeKpiResponseTypeDef = TypedDict(
     "GetCampaignDateRangeKpiResponseTypeDef",
     {
         "CampaignDateRangeKpiResponse": CampaignDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJourneyDateRangeKpiResponseTypeDef = TypedDict(
     "GetJourneyDateRangeKpiResponseTypeDef",
     {
         "JourneyDateRangeKpiResponse": JourneyDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMessageRequestTypeDef = TypedDict(
     "_RequiredMessageRequestTypeDef",
     {
         "MessageConfiguration": DirectMessageConfigurationTypeDef,
@@ -5744,19 +6407,17 @@
         "Endpoints": Mapping[str, EndpointSendConfigurationTypeDef],
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TraceId": str,
     },
     total=False,
 )
 
-
 class MessageRequestTypeDef(_RequiredMessageRequestTypeDef, _OptionalMessageRequestTypeDef):
     pass
 
-
 _RequiredSendUsersMessageRequestTypeDef = TypedDict(
     "_RequiredSendUsersMessageRequestTypeDef",
     {
         "MessageConfiguration": DirectMessageConfigurationTypeDef,
         "Users": Mapping[str, EndpointSendConfigurationTypeDef],
     },
 )
@@ -5766,20 +6427,45 @@
         "Context": Mapping[str, str],
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TraceId": str,
     },
     total=False,
 )
 
-
 class SendUsersMessageRequestTypeDef(
     _RequiredSendUsersMessageRequestTypeDef, _OptionalSendUsersMessageRequestTypeDef
 ):
     pass
 
+SegmentGroupListOutputTypeDef = TypedDict(
+    "SegmentGroupListOutputTypeDef",
+    {
+        "Groups": List[SegmentGroupOutputTypeDef],
+        "Include": IncludeType,
+    },
+    total=False,
+)
+
+ConditionOutputTypeDef = TypedDict(
+    "ConditionOutputTypeDef",
+    {
+        "Conditions": List[SimpleConditionOutputTypeDef],
+        "Operator": OperatorType,
+    },
+    total=False,
+)
+
+MultiConditionalBranchOutputTypeDef = TypedDict(
+    "MultiConditionalBranchOutputTypeDef",
+    {
+        "Condition": SimpleConditionOutputTypeDef,
+        "NextActivity": str,
+    },
+    total=False,
+)
 
 SegmentGroupListTypeDef = TypedDict(
     "SegmentGroupListTypeDef",
     {
         "Groups": Sequence[SegmentGroupTypeDef],
         "Include": IncludeType,
     },
@@ -5810,31 +6496,37 @@
         "Id": str,
         "SizePercent": int,
     },
 )
 _OptionalTreatmentResourceTypeDef = TypedDict(
     "_OptionalTreatmentResourceTypeDef",
     {
-        "CustomDeliveryConfiguration": CustomDeliveryConfigurationTypeDef,
-        "MessageConfiguration": MessageConfigurationTypeDef,
-        "Schedule": ScheduleTypeDef,
+        "CustomDeliveryConfiguration": CustomDeliveryConfigurationOutputTypeDef,
+        "MessageConfiguration": MessageConfigurationOutputTypeDef,
+        "Schedule": ScheduleOutputTypeDef,
         "State": CampaignStateTypeDef,
-        "TemplateConfiguration": TemplateConfigurationTypeDef,
+        "TemplateConfiguration": TemplateConfigurationOutputTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
     },
     total=False,
 )
 
-
 class TreatmentResourceTypeDef(
     _RequiredTreatmentResourceTypeDef, _OptionalTreatmentResourceTypeDef
 ):
     pass
 
+InAppMessagesResponseTypeDef = TypedDict(
+    "InAppMessagesResponseTypeDef",
+    {
+        "InAppMessageCampaigns": List[InAppMessageCampaignTypeDef],
+    },
+    total=False,
+)
 
 _RequiredWriteTreatmentResourceTypeDef = TypedDict(
     "_RequiredWriteTreatmentResourceTypeDef",
     {
         "SizePercent": int,
     },
 )
@@ -5847,29 +6539,19 @@
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
     },
     total=False,
 )
 
-
 class WriteTreatmentResourceTypeDef(
     _RequiredWriteTreatmentResourceTypeDef, _OptionalWriteTreatmentResourceTypeDef
 ):
     pass
 
-
-InAppMessagesResponseTypeDef = TypedDict(
-    "InAppMessagesResponseTypeDef",
-    {
-        "InAppMessageCampaigns": List[InAppMessageCampaignTypeDef],
-    },
-    total=False,
-)
-
 SendMessagesRequestRequestTypeDef = TypedDict(
     "SendMessagesRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "MessageRequest": MessageRequestTypeDef,
     },
 )
@@ -5891,29 +6573,48 @@
         "Id": str,
         "SegmentType": SegmentTypeType,
     },
 )
 _OptionalSegmentResponseTypeDef = TypedDict(
     "_OptionalSegmentResponseTypeDef",
     {
-        "Dimensions": SegmentDimensionsTypeDef,
+        "Dimensions": SegmentDimensionsOutputTypeDef,
         "ImportDefinition": SegmentImportResourceTypeDef,
         "LastModifiedDate": str,
         "Name": str,
-        "SegmentGroups": SegmentGroupListTypeDef,
+        "SegmentGroups": SegmentGroupListOutputTypeDef,
         "tags": Dict[str, str],
         "Version": int,
     },
     total=False,
 )
 
-
 class SegmentResponseTypeDef(_RequiredSegmentResponseTypeDef, _OptionalSegmentResponseTypeDef):
     pass
 
+ConditionalSplitActivityOutputTypeDef = TypedDict(
+    "ConditionalSplitActivityOutputTypeDef",
+    {
+        "Condition": ConditionOutputTypeDef,
+        "EvaluationWaitTime": WaitTimeOutputTypeDef,
+        "FalseActivity": str,
+        "TrueActivity": str,
+    },
+    total=False,
+)
+
+MultiConditionalSplitActivityOutputTypeDef = TypedDict(
+    "MultiConditionalSplitActivityOutputTypeDef",
+    {
+        "Branches": List[MultiConditionalBranchOutputTypeDef],
+        "DefaultActivity": str,
+        "EvaluationWaitTime": WaitTimeOutputTypeDef,
+    },
+    total=False,
+)
 
 WriteSegmentRequestTypeDef = TypedDict(
     "WriteSegmentRequestTypeDef",
     {
         "Dimensions": SegmentDimensionsTypeDef,
         "Name": str,
         "SegmentGroups": SegmentGroupListTypeDef,
@@ -5955,39 +6656,45 @@
         "SegmentVersion": int,
     },
 )
 _OptionalCampaignResponseTypeDef = TypedDict(
     "_OptionalCampaignResponseTypeDef",
     {
         "AdditionalTreatments": List[TreatmentResourceTypeDef],
-        "CustomDeliveryConfiguration": CustomDeliveryConfigurationTypeDef,
+        "CustomDeliveryConfiguration": CustomDeliveryConfigurationOutputTypeDef,
         "DefaultState": CampaignStateTypeDef,
         "Description": str,
         "HoldoutPercent": int,
-        "Hook": CampaignHookTypeDef,
+        "Hook": CampaignHookOutputTypeDef,
         "IsPaused": bool,
-        "Limits": CampaignLimitsTypeDef,
-        "MessageConfiguration": MessageConfigurationTypeDef,
+        "Limits": CampaignLimitsOutputTypeDef,
+        "MessageConfiguration": MessageConfigurationOutputTypeDef,
         "Name": str,
-        "Schedule": ScheduleTypeDef,
+        "Schedule": ScheduleOutputTypeDef,
         "State": CampaignStateTypeDef,
         "tags": Dict[str, str],
-        "TemplateConfiguration": TemplateConfigurationTypeDef,
+        "TemplateConfiguration": TemplateConfigurationOutputTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
         "Version": int,
         "Priority": int,
     },
     total=False,
 )
 
-
 class CampaignResponseTypeDef(_RequiredCampaignResponseTypeDef, _OptionalCampaignResponseTypeDef):
     pass
 
+GetInAppMessagesResponseTypeDef = TypedDict(
+    "GetInAppMessagesResponseTypeDef",
+    {
+        "InAppMessagesResponse": InAppMessagesResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 WriteCampaignRequestTypeDef = TypedDict(
     "WriteCampaignRequestTypeDef",
     {
         "AdditionalTreatments": Sequence[WriteTreatmentResourceTypeDef],
         "CustomDeliveryConfiguration": CustomDeliveryConfigurationTypeDef,
         "Description": str,
@@ -6005,51 +6712,43 @@
         "TreatmentDescription": str,
         "TreatmentName": str,
         "Priority": int,
     },
     total=False,
 )
 
-GetInAppMessagesResponseTypeDef = TypedDict(
-    "GetInAppMessagesResponseTypeDef",
-    {
-        "InAppMessagesResponse": InAppMessagesResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateSegmentResponseTypeDef = TypedDict(
     "CreateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSegmentResponseTypeDef = TypedDict(
     "DeleteSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentResponseTypeDef = TypedDict(
     "GetSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentVersionResponseTypeDef = TypedDict(
     "GetSegmentVersionResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSegmentsResponseTypeDef = TypedDict(
     "_RequiredSegmentsResponseTypeDef",
     {
         "Item": List[SegmentResponseTypeDef],
@@ -6059,27 +6758,43 @@
     "_OptionalSegmentsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class SegmentsResponseTypeDef(_RequiredSegmentsResponseTypeDef, _OptionalSegmentsResponseTypeDef):
     pass
 
-
 UpdateSegmentResponseTypeDef = TypedDict(
     "UpdateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ActivityOutputTypeDef = TypedDict(
+    "ActivityOutputTypeDef",
+    {
+        "CUSTOM": CustomMessageActivityOutputTypeDef,
+        "ConditionalSplit": ConditionalSplitActivityOutputTypeDef,
+        "Description": str,
+        "EMAIL": EmailMessageActivityOutputTypeDef,
+        "Holdout": HoldoutActivityOutputTypeDef,
+        "MultiCondition": MultiConditionalSplitActivityOutputTypeDef,
+        "PUSH": PushMessageActivityOutputTypeDef,
+        "RandomSplit": RandomSplitActivityOutputTypeDef,
+        "SMS": SMSMessageActivityOutputTypeDef,
+        "Wait": WaitActivityOutputTypeDef,
+        "ContactCenter": ContactCenterActivityOutputTypeDef,
+    },
+    total=False,
+)
+
 CreateSegmentRequestRequestTypeDef = TypedDict(
     "CreateSegmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "WriteSegmentRequest": WriteSegmentRequestTypeDef,
     },
 )
@@ -6121,58 +6836,56 @@
     "_OptionalCampaignsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class CampaignsResponseTypeDef(
     _RequiredCampaignsResponseTypeDef, _OptionalCampaignsResponseTypeDef
 ):
     pass
 
-
 CreateCampaignResponseTypeDef = TypedDict(
     "CreateCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCampaignResponseTypeDef = TypedDict(
     "DeleteCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCampaignResponseTypeDef = TypedDict(
     "GetCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCampaignVersionResponseTypeDef = TypedDict(
     "GetCampaignVersionResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCampaignResponseTypeDef = TypedDict(
     "UpdateCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCampaignRequestRequestTypeDef = TypedDict(
     "CreateCampaignRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -6189,65 +6902,63 @@
     },
 )
 
 GetSegmentVersionsResponseTypeDef = TypedDict(
     "GetSegmentVersionsResponseTypeDef",
     {
         "SegmentsResponse": SegmentsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentsResponseTypeDef = TypedDict(
     "GetSegmentsResponseTypeDef",
     {
         "SegmentsResponse": SegmentsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJourneyResponseTypeDef = TypedDict(
     "_RequiredJourneyResponseTypeDef",
     {
         "ApplicationId": str,
         "Id": str,
         "Name": str,
     },
 )
 _OptionalJourneyResponseTypeDef = TypedDict(
     "_OptionalJourneyResponseTypeDef",
     {
-        "Activities": Dict[str, ActivityTypeDef],
+        "Activities": Dict[str, ActivityOutputTypeDef],
         "CreationDate": str,
         "LastModifiedDate": str,
-        "Limits": JourneyLimitsTypeDef,
+        "Limits": JourneyLimitsOutputTypeDef,
         "LocalTime": bool,
-        "QuietTime": QuietTimeTypeDef,
+        "QuietTime": QuietTimeOutputTypeDef,
         "RefreshFrequency": str,
-        "Schedule": JourneyScheduleTypeDef,
+        "Schedule": JourneyScheduleOutputTypeDef,
         "StartActivity": str,
-        "StartCondition": StartConditionTypeDef,
+        "StartCondition": StartConditionOutputTypeDef,
         "State": StateType,
         "tags": Dict[str, str],
         "WaitForQuietTime": bool,
         "RefreshOnSegmentUpdate": bool,
-        "JourneyChannelSettings": JourneyChannelSettingsTypeDef,
+        "JourneyChannelSettings": JourneyChannelSettingsOutputTypeDef,
         "SendingSchedule": bool,
-        "OpenHours": OpenHoursTypeDef,
-        "ClosedDays": ClosedDaysTypeDef,
+        "OpenHours": OpenHoursOutputTypeDef,
+        "ClosedDays": ClosedDaysOutputTypeDef,
         "TimezoneEstimationMethods": List[TimezoneEstimationMethodsElementType],
     },
     total=False,
 )
 
-
 class JourneyResponseTypeDef(_RequiredJourneyResponseTypeDef, _OptionalJourneyResponseTypeDef):
     pass
 
-
 _RequiredWriteJourneyRequestTypeDef = TypedDict(
     "_RequiredWriteJourneyRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalWriteJourneyRequestTypeDef = TypedDict(
@@ -6271,58 +6982,56 @@
         "OpenHours": OpenHoursTypeDef,
         "ClosedDays": ClosedDaysTypeDef,
         "TimezoneEstimationMethods": Sequence[TimezoneEstimationMethodsElementType],
     },
     total=False,
 )
 
-
 class WriteJourneyRequestTypeDef(
     _RequiredWriteJourneyRequestTypeDef, _OptionalWriteJourneyRequestTypeDef
 ):
     pass
 
-
 GetCampaignVersionsResponseTypeDef = TypedDict(
     "GetCampaignVersionsResponseTypeDef",
     {
         "CampaignsResponse": CampaignsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCampaignsResponseTypeDef = TypedDict(
     "GetCampaignsResponseTypeDef",
     {
         "CampaignsResponse": CampaignsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateJourneyResponseTypeDef = TypedDict(
     "CreateJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteJourneyResponseTypeDef = TypedDict(
     "DeleteJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJourneyResponseTypeDef = TypedDict(
     "GetJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJourneysResponseTypeDef = TypedDict(
     "_RequiredJourneysResponseTypeDef",
     {
         "Item": List[JourneyResponseTypeDef],
@@ -6332,32 +7041,30 @@
     "_OptionalJourneysResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class JourneysResponseTypeDef(_RequiredJourneysResponseTypeDef, _OptionalJourneysResponseTypeDef):
     pass
 
-
 UpdateJourneyResponseTypeDef = TypedDict(
     "UpdateJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateJourneyStateResponseTypeDef = TypedDict(
     "UpdateJourneyStateResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateJourneyRequestRequestTypeDef = TypedDict(
     "CreateJourneyRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -6374,10 +7081,10 @@
     },
 )
 
 ListJourneysResponseTypeDef = TypedDict(
     "ListJourneysResponseTypeDef",
     {
         "JourneysResponse": JourneysResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint/type_defs.pyi` & `mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,64 +49,82 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ADMChannelRequestTypeDef",
     "ADMChannelResponseTypeDef",
     "ADMMessageTypeDef",
     "APNSChannelRequestTypeDef",
     "APNSChannelResponseTypeDef",
     "APNSMessageTypeDef",
+    "APNSPushNotificationTemplateOutputTypeDef",
     "APNSPushNotificationTemplateTypeDef",
     "APNSSandboxChannelRequestTypeDef",
     "APNSSandboxChannelResponseTypeDef",
     "APNSVoipChannelRequestTypeDef",
     "APNSVoipChannelResponseTypeDef",
     "APNSVoipSandboxChannelRequestTypeDef",
     "APNSVoipSandboxChannelResponseTypeDef",
     "ActivityResponseTypeDef",
+    "ContactCenterActivityOutputTypeDef",
+    "HoldoutActivityOutputTypeDef",
     "ContactCenterActivityTypeDef",
     "HoldoutActivityTypeDef",
     "AddressConfigurationTypeDef",
+    "AndroidPushNotificationTemplateOutputTypeDef",
     "AndroidPushNotificationTemplateTypeDef",
     "ApplicationResponseTypeDef",
-    "CampaignHookTypeDef",
-    "CampaignLimitsTypeDef",
-    "QuietTimeTypeDef",
+    "CampaignHookOutputTypeDef",
+    "CampaignLimitsOutputTypeDef",
+    "QuietTimeOutputTypeDef",
+    "AttributeDimensionOutputTypeDef",
     "AttributeDimensionTypeDef",
     "AttributesResourceTypeDef",
     "BaiduChannelRequestTypeDef",
     "BaiduChannelResponseTypeDef",
     "BaiduMessageTypeDef",
+    "CampaignCustomMessageOutputTypeDef",
     "CampaignCustomMessageTypeDef",
+    "CampaignEmailMessageOutputTypeDef",
     "CampaignEmailMessageTypeDef",
+    "CampaignHookTypeDef",
+    "CampaignLimitsTypeDef",
     "CampaignStateTypeDef",
-    "CustomDeliveryConfigurationTypeDef",
+    "CustomDeliveryConfigurationOutputTypeDef",
+    "CampaignSmsMessageOutputTypeDef",
     "CampaignSmsMessageTypeDef",
     "ChannelResponseTypeDef",
+    "ClosedDaysRuleOutputTypeDef",
     "ClosedDaysRuleTypeDef",
+    "WaitTimeOutputTypeDef",
     "WaitTimeTypeDef",
     "CreateApplicationRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "EmailTemplateRequestTypeDef",
     "CreateTemplateMessageBodyTypeDef",
     "ExportJobRequestTypeDef",
     "ImportJobRequestTypeDef",
     "TemplateCreateMessageBodyTypeDef",
     "CreateRecommenderConfigurationTypeDef",
     "RecommenderConfigurationResponseTypeDef",
     "SMSTemplateRequestTypeDef",
     "VoiceTemplateRequestTypeDef",
+    "CustomDeliveryConfigurationTypeDef",
+    "JourneyCustomMessageOutputTypeDef",
     "JourneyCustomMessageTypeDef",
+    "DefaultButtonConfigurationOutputTypeDef",
     "DefaultButtonConfigurationTypeDef",
     "DefaultMessageTypeDef",
     "DefaultPushNotificationMessageTypeDef",
+    "DefaultPushNotificationTemplateOutputTypeDef",
     "DefaultPushNotificationTemplateTypeDef",
     "DeleteAdmChannelRequestRequestTypeDef",
     "DeleteApnsChannelRequestRequestTypeDef",
     "DeleteApnsSandboxChannelRequestRequestTypeDef",
     "DeleteApnsVoipChannelRequestRequestTypeDef",
     "DeleteApnsVoipSandboxChannelRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
@@ -133,30 +151,36 @@
     "DeleteVoiceChannelRequestRequestTypeDef",
     "VoiceChannelResponseTypeDef",
     "DeleteVoiceTemplateRequestRequestTypeDef",
     "GCMMessageTypeDef",
     "SMSMessageTypeDef",
     "VoiceMessageTypeDef",
     "EmailChannelRequestTypeDef",
+    "JourneyEmailMessageOutputTypeDef",
     "JourneyEmailMessageTypeDef",
     "RawEmailTypeDef",
     "EmailTemplateResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EndpointDemographicTypeDef",
     "EndpointLocationTypeDef",
     "EndpointUserTypeDef",
+    "EndpointDemographicOutputTypeDef",
     "EndpointItemResponseTypeDef",
+    "EndpointLocationOutputTypeDef",
     "EndpointMessageResultTypeDef",
+    "EndpointUserOutputTypeDef",
     "EndpointSendConfigurationTypeDef",
+    "MetricDimensionOutputTypeDef",
+    "SetDimensionOutputTypeDef",
     "MetricDimensionTypeDef",
     "SetDimensionTypeDef",
     "EventItemResponseTypeDef",
     "SessionTypeDef",
     "ExportJobResourceTypeDef",
     "GCMChannelRequestTypeDef",
+    "GPSCoordinatesOutputTypeDef",
     "GPSCoordinatesTypeDef",
     "GetAdmChannelRequestRequestTypeDef",
     "GetApnsChannelRequestRequestTypeDef",
     "GetApnsSandboxChannelRequestRequestTypeDef",
     "GetApnsVoipChannelRequestRequestTypeDef",
     "GetApnsVoipSandboxChannelRequestRequestTypeDef",
     "GetAppRequestRequestTypeDef",
@@ -206,91 +230,109 @@
     "GetSmsTemplateRequestRequestTypeDef",
     "SMSTemplateResponseTypeDef",
     "GetUserEndpointsRequestRequestTypeDef",
     "GetVoiceChannelRequestRequestTypeDef",
     "GetVoiceTemplateRequestRequestTypeDef",
     "VoiceTemplateResponseTypeDef",
     "ImportJobResourceTypeDef",
+    "InAppMessageBodyConfigOutputTypeDef",
     "InAppMessageBodyConfigTypeDef",
+    "OverrideButtonConfigurationOutputTypeDef",
     "OverrideButtonConfigurationTypeDef",
+    "InAppMessageHeaderConfigOutputTypeDef",
     "InAppMessageHeaderConfigTypeDef",
+    "JourneyChannelSettingsOutputTypeDef",
     "JourneyChannelSettingsTypeDef",
+    "JourneyLimitsOutputTypeDef",
     "JourneyLimitsTypeDef",
+    "JourneyPushMessageOutputTypeDef",
     "JourneyPushMessageTypeDef",
-    "JourneyScheduleTypeDef",
+    "JourneyScheduleOutputTypeDef",
     "JourneyRunResponseTypeDef",
+    "JourneySMSMessageOutputTypeDef",
     "JourneySMSMessageTypeDef",
+    "JourneyScheduleTypeDef",
     "JourneyStateRequestTypeDef",
     "ListJourneysRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagsModelTypeDef",
+    "TagsModelOutputTypeDef",
     "ListTemplateVersionsRequestRequestTypeDef",
     "ListTemplatesRequestRequestTypeDef",
+    "MessageOutputTypeDef",
     "MessageTypeDef",
     "MessageResultTypeDef",
     "NumberValidateRequestTypeDef",
     "NumberValidateResponseTypeDef",
+    "OpenHoursRuleOutputTypeDef",
     "OpenHoursRuleTypeDef",
     "WriteEventStreamTypeDef",
+    "QuietTimeTypeDef",
+    "RandomSplitEntryOutputTypeDef",
     "RandomSplitEntryTypeDef",
+    "RecencyDimensionOutputTypeDef",
     "RecencyDimensionTypeDef",
     "UpdateAttributesRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ResultRowValueTypeDef",
     "SMSChannelRequestTypeDef",
+    "SegmentConditionOutputTypeDef",
     "SegmentConditionTypeDef",
+    "SegmentReferenceOutputTypeDef",
     "SegmentReferenceTypeDef",
     "SegmentImportResourceTypeDef",
     "SendOTPMessageRequestParametersTypeDef",
     "SimpleEmailPartTypeDef",
+    "TagsModelTypeDef",
     "TemplateActiveVersionRequestTypeDef",
+    "TemplateOutputTypeDef",
     "TemplateTypeDef",
     "TemplateResponseTypeDef",
     "TemplateVersionResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateRecommenderConfigurationTypeDef",
     "VoiceChannelRequestTypeDef",
     "VerificationResponseTypeDef",
     "VerifyOTPMessageRequestParametersTypeDef",
     "UpdateAdmChannelRequestRequestTypeDef",
-    "DeleteAdmChannelResponseTypeDef",
-    "GetAdmChannelResponseTypeDef",
-    "UpdateAdmChannelResponseTypeDef",
     "UpdateApnsChannelRequestRequestTypeDef",
-    "DeleteApnsChannelResponseTypeDef",
-    "GetApnsChannelResponseTypeDef",
-    "UpdateApnsChannelResponseTypeDef",
     "UpdateApnsSandboxChannelRequestRequestTypeDef",
-    "DeleteApnsSandboxChannelResponseTypeDef",
-    "GetApnsSandboxChannelResponseTypeDef",
-    "UpdateApnsSandboxChannelResponseTypeDef",
     "UpdateApnsVoipChannelRequestRequestTypeDef",
-    "DeleteApnsVoipChannelResponseTypeDef",
-    "GetApnsVoipChannelResponseTypeDef",
-    "UpdateApnsVoipChannelResponseTypeDef",
     "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
-    "DeleteApnsVoipSandboxChannelResponseTypeDef",
-    "GetApnsVoipSandboxChannelResponseTypeDef",
-    "UpdateApnsVoipSandboxChannelResponseTypeDef",
     "ActivitiesResponseTypeDef",
     "ApplicationsResponseTypeDef",
-    "CreateAppResponseTypeDef",
-    "DeleteAppResponseTypeDef",
-    "GetAppResponseTypeDef",
     "ApplicationSettingsResourceTypeDef",
-    "WriteApplicationSettingsRequestTypeDef",
-    "RemoveAttributesResponseTypeDef",
     "UpdateBaiduChannelRequestRequestTypeDef",
-    "DeleteBaiduChannelResponseTypeDef",
-    "GetBaiduChannelResponseTypeDef",
-    "UpdateBaiduChannelResponseTypeDef",
     "ChannelsResponseTypeDef",
+    "ClosedDaysOutputTypeDef",
     "ClosedDaysTypeDef",
+    "WaitActivityOutputTypeDef",
     "WaitActivityTypeDef",
     "CreateAppRequestRequestTypeDef",
+    "CreateAppResponseTypeDef",
+    "DeleteAdmChannelResponseTypeDef",
+    "DeleteApnsChannelResponseTypeDef",
+    "DeleteApnsSandboxChannelResponseTypeDef",
+    "DeleteApnsVoipChannelResponseTypeDef",
+    "DeleteApnsVoipSandboxChannelResponseTypeDef",
+    "DeleteAppResponseTypeDef",
+    "DeleteBaiduChannelResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAdmChannelResponseTypeDef",
+    "GetApnsChannelResponseTypeDef",
+    "GetApnsSandboxChannelResponseTypeDef",
+    "GetApnsVoipChannelResponseTypeDef",
+    "GetApnsVoipSandboxChannelResponseTypeDef",
+    "GetAppResponseTypeDef",
+    "GetBaiduChannelResponseTypeDef",
+    "RemoveAttributesResponseTypeDef",
+    "UpdateAdmChannelResponseTypeDef",
+    "UpdateApnsChannelResponseTypeDef",
+    "UpdateApnsSandboxChannelResponseTypeDef",
+    "UpdateApnsVoipChannelResponseTypeDef",
+    "UpdateApnsVoipSandboxChannelResponseTypeDef",
+    "UpdateBaiduChannelResponseTypeDef",
     "CreateEmailTemplateRequestRequestTypeDef",
     "UpdateEmailTemplateRequestRequestTypeDef",
     "CreateEmailTemplateResponseTypeDef",
     "CreatePushTemplateResponseTypeDef",
     "CreateSmsTemplateResponseTypeDef",
     "CreateVoiceTemplateResponseTypeDef",
     "CreateExportJobRequestRequestTypeDef",
@@ -302,17 +344,18 @@
     "GetRecommenderConfigurationResponseTypeDef",
     "ListRecommenderConfigurationsResponseTypeDef",
     "UpdateRecommenderConfigurationResponseTypeDef",
     "CreateSmsTemplateRequestRequestTypeDef",
     "UpdateSmsTemplateRequestRequestTypeDef",
     "CreateVoiceTemplateRequestRequestTypeDef",
     "UpdateVoiceTemplateRequestRequestTypeDef",
+    "CustomMessageActivityOutputTypeDef",
     "CustomMessageActivityTypeDef",
-    "PushNotificationTemplateRequestTypeDef",
     "PushNotificationTemplateResponseTypeDef",
+    "PushNotificationTemplateRequestTypeDef",
     "DeleteEmailChannelResponseTypeDef",
     "GetEmailChannelResponseTypeDef",
     "UpdateEmailChannelResponseTypeDef",
     "DeleteEmailTemplateResponseTypeDef",
     "DeleteInAppTemplateResponseTypeDef",
     "DeletePushTemplateResponseTypeDef",
     "DeleteSmsTemplateResponseTypeDef",
@@ -334,154 +377,185 @@
     "DeleteSmsChannelResponseTypeDef",
     "GetSmsChannelResponseTypeDef",
     "UpdateSmsChannelResponseTypeDef",
     "DeleteVoiceChannelResponseTypeDef",
     "GetVoiceChannelResponseTypeDef",
     "UpdateVoiceChannelResponseTypeDef",
     "UpdateEmailChannelRequestRequestTypeDef",
+    "EmailMessageActivityOutputTypeDef",
     "EmailMessageActivityTypeDef",
     "GetEmailTemplateResponseTypeDef",
     "EndpointBatchItemTypeDef",
     "EndpointRequestTypeDef",
-    "EndpointResponseTypeDef",
     "PublicEndpointTypeDef",
     "SendUsersMessageResponseTypeDef",
+    "EndpointResponseTypeDef",
+    "EventDimensionsOutputTypeDef",
+    "SegmentDemographicsOutputTypeDef",
     "EventDimensionsTypeDef",
     "SegmentDemographicsTypeDef",
     "ItemResponseTypeDef",
     "EventTypeDef",
     "ExportJobResponseTypeDef",
     "UpdateGcmChannelRequestRequestTypeDef",
+    "GPSPointDimensionOutputTypeDef",
     "GPSPointDimensionTypeDef",
     "GetJourneyExecutionActivityMetricsResponseTypeDef",
     "GetJourneyExecutionMetricsResponseTypeDef",
     "GetJourneyRunExecutionActivityMetricsResponseTypeDef",
     "GetJourneyRunExecutionMetricsResponseTypeDef",
     "GetSmsTemplateResponseTypeDef",
     "GetVoiceTemplateResponseTypeDef",
     "ImportJobResponseTypeDef",
+    "InAppMessageButtonOutputTypeDef",
     "InAppMessageButtonTypeDef",
+    "PushMessageActivityOutputTypeDef",
     "PushMessageActivityTypeDef",
     "JourneyRunsResponseTypeDef",
+    "SMSMessageActivityOutputTypeDef",
     "SMSMessageActivityTypeDef",
     "UpdateJourneyStateRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "MessageResponseTypeDef",
     "PhoneNumberValidateRequestRequestTypeDef",
     "PhoneNumberValidateResponseTypeDef",
+    "OpenHoursOutputTypeDef",
     "OpenHoursTypeDef",
     "PutEventStreamRequestRequestTypeDef",
+    "WriteApplicationSettingsRequestTypeDef",
+    "RandomSplitActivityOutputTypeDef",
     "RandomSplitActivityTypeDef",
+    "SegmentBehaviorsOutputTypeDef",
     "SegmentBehaviorsTypeDef",
     "RemoveAttributesRequestRequestTypeDef",
     "ResultRowTypeDef",
     "UpdateSmsChannelRequestRequestTypeDef",
     "SendOTPMessageRequestRequestTypeDef",
     "SimpleEmailTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "UpdateTemplateActiveVersionRequestRequestTypeDef",
+    "TemplateConfigurationOutputTypeDef",
     "TemplateConfigurationTypeDef",
     "TemplatesResponseTypeDef",
     "TemplateVersionsResponseTypeDef",
     "UpdateRecommenderConfigurationRequestRequestTypeDef",
     "UpdateVoiceChannelRequestRequestTypeDef",
     "VerifyOTPMessageResponseTypeDef",
     "VerifyOTPMessageRequestRequestTypeDef",
     "GetCampaignActivitiesResponseTypeDef",
     "GetAppsResponseTypeDef",
     "GetApplicationSettingsResponseTypeDef",
     "UpdateApplicationSettingsResponseTypeDef",
-    "UpdateApplicationSettingsRequestRequestTypeDef",
     "GetChannelsResponseTypeDef",
     "GetRecommenderConfigurationsResponseTypeDef",
+    "GetPushTemplateResponseTypeDef",
     "CreatePushTemplateRequestRequestTypeDef",
     "UpdatePushTemplateRequestRequestTypeDef",
-    "GetPushTemplateResponseTypeDef",
     "EndpointBatchRequestTypeDef",
     "UpdateEndpointRequestRequestTypeDef",
+    "SendUsersMessagesResponseTypeDef",
     "DeleteEndpointResponseTypeDef",
     "EndpointsResponseTypeDef",
     "GetEndpointResponseTypeDef",
-    "SendUsersMessagesResponseTypeDef",
+    "CampaignEventFilterOutputTypeDef",
+    "EventConditionOutputTypeDef",
+    "EventFilterOutputTypeDef",
     "CampaignEventFilterTypeDef",
     "EventConditionTypeDef",
     "EventFilterTypeDef",
     "EventsResponseTypeDef",
     "EventsBatchTypeDef",
     "CreateExportJobResponseTypeDef",
     "ExportJobsResponseTypeDef",
     "GetExportJobResponseTypeDef",
+    "SegmentLocationOutputTypeDef",
     "SegmentLocationTypeDef",
     "CreateImportJobResponseTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobsResponseTypeDef",
+    "InAppMessageContentOutputTypeDef",
     "InAppMessageContentTypeDef",
     "GetJourneyRunsResponseTypeDef",
     "SendMessagesResponseTypeDef",
     "SendOTPMessageResponseTypeDef",
+    "UpdateApplicationSettingsRequestRequestTypeDef",
     "BaseKpiResultTypeDef",
     "EmailMessageTypeDef",
     "ListTemplatesResponseTypeDef",
     "ListTemplateVersionsResponseTypeDef",
     "UpdateEndpointsBatchRequestRequestTypeDef",
     "DeleteUserEndpointsResponseTypeDef",
     "GetUserEndpointsResponseTypeDef",
     "InAppCampaignScheduleTypeDef",
+    "ScheduleOutputTypeDef",
+    "EventStartConditionOutputTypeDef",
     "ScheduleTypeDef",
     "EventStartConditionTypeDef",
     "PutEventsResponseTypeDef",
     "EventsRequestTypeDef",
     "GetExportJobsResponseTypeDef",
     "GetSegmentExportJobsResponseTypeDef",
+    "SegmentDimensionsOutputTypeDef",
     "SegmentDimensionsTypeDef",
     "GetImportJobsResponseTypeDef",
     "GetSegmentImportJobsResponseTypeDef",
-    "CampaignInAppMessageTypeDef",
+    "CampaignInAppMessageOutputTypeDef",
     "InAppMessageTypeDef",
-    "InAppTemplateRequestTypeDef",
     "InAppTemplateResponseTypeDef",
+    "CampaignInAppMessageTypeDef",
+    "InAppTemplateRequestTypeDef",
     "ApplicationDateRangeKpiResponseTypeDef",
     "CampaignDateRangeKpiResponseTypeDef",
     "JourneyDateRangeKpiResponseTypeDef",
     "DirectMessageConfigurationTypeDef",
+    "StartConditionOutputTypeDef",
     "StartConditionTypeDef",
     "PutEventsRequestRequestTypeDef",
+    "SegmentGroupOutputTypeDef",
+    "SimpleConditionOutputTypeDef",
     "SegmentGroupTypeDef",
     "SimpleConditionTypeDef",
-    "MessageConfigurationTypeDef",
+    "MessageConfigurationOutputTypeDef",
     "InAppMessageCampaignTypeDef",
+    "GetInAppTemplateResponseTypeDef",
+    "MessageConfigurationTypeDef",
     "CreateInAppTemplateRequestRequestTypeDef",
     "UpdateInAppTemplateRequestRequestTypeDef",
-    "GetInAppTemplateResponseTypeDef",
     "GetApplicationDateRangeKpiResponseTypeDef",
     "GetCampaignDateRangeKpiResponseTypeDef",
     "GetJourneyDateRangeKpiResponseTypeDef",
     "MessageRequestTypeDef",
     "SendUsersMessageRequestTypeDef",
+    "SegmentGroupListOutputTypeDef",
+    "ConditionOutputTypeDef",
+    "MultiConditionalBranchOutputTypeDef",
     "SegmentGroupListTypeDef",
     "ConditionTypeDef",
     "MultiConditionalBranchTypeDef",
     "TreatmentResourceTypeDef",
-    "WriteTreatmentResourceTypeDef",
     "InAppMessagesResponseTypeDef",
+    "WriteTreatmentResourceTypeDef",
     "SendMessagesRequestRequestTypeDef",
     "SendUsersMessagesRequestRequestTypeDef",
     "SegmentResponseTypeDef",
+    "ConditionalSplitActivityOutputTypeDef",
+    "MultiConditionalSplitActivityOutputTypeDef",
     "WriteSegmentRequestTypeDef",
     "ConditionalSplitActivityTypeDef",
     "MultiConditionalSplitActivityTypeDef",
     "CampaignResponseTypeDef",
-    "WriteCampaignRequestTypeDef",
     "GetInAppMessagesResponseTypeDef",
+    "WriteCampaignRequestTypeDef",
     "CreateSegmentResponseTypeDef",
     "DeleteSegmentResponseTypeDef",
     "GetSegmentResponseTypeDef",
     "GetSegmentVersionResponseTypeDef",
     "SegmentsResponseTypeDef",
     "UpdateSegmentResponseTypeDef",
+    "ActivityOutputTypeDef",
     "CreateSegmentRequestRequestTypeDef",
     "UpdateSegmentRequestRequestTypeDef",
     "ActivityTypeDef",
     "CampaignsResponseTypeDef",
     "CreateCampaignResponseTypeDef",
     "DeleteCampaignResponseTypeDef",
     "GetCampaignResponseTypeDef",
@@ -517,19 +591,21 @@
     "_OptionalADMChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+
 class ADMChannelRequestTypeDef(
     _RequiredADMChannelRequestTypeDef, _OptionalADMChannelRequestTypeDef
 ):
     pass
 
+
 _RequiredADMChannelResponseTypeDef = TypedDict(
     "_RequiredADMChannelResponseTypeDef",
     {
         "Platform": str,
     },
 )
 _OptionalADMChannelResponseTypeDef = TypedDict(
@@ -544,19 +620,21 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class ADMChannelResponseTypeDef(
     _RequiredADMChannelResponseTypeDef, _OptionalADMChannelResponseTypeDef
 ):
     pass
 
+
 ADMMessageTypeDef = TypedDict(
     "ADMMessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "ConsolidationKey": str,
         "Data": Mapping[str, str],
@@ -611,19 +689,21 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class APNSChannelResponseTypeDef(
     _RequiredAPNSChannelResponseTypeDef, _OptionalAPNSChannelResponseTypeDef
 ):
     pass
 
+
 APNSMessageTypeDef = TypedDict(
     "APNSMessageTypeDef",
     {
         "APNSPushType": str,
         "Action": ActionType,
         "Badge": int,
         "Body": str,
@@ -641,14 +721,28 @@
         "TimeToLive": int,
         "Title": str,
         "Url": str,
     },
     total=False,
 )
 
+APNSPushNotificationTemplateOutputTypeDef = TypedDict(
+    "APNSPushNotificationTemplateOutputTypeDef",
+    {
+        "Action": ActionType,
+        "Body": str,
+        "MediaUrl": str,
+        "RawContent": str,
+        "Sound": str,
+        "Title": str,
+        "Url": str,
+    },
+    total=False,
+)
+
 APNSPushNotificationTemplateTypeDef = TypedDict(
     "APNSPushNotificationTemplateTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "MediaUrl": str,
         "RawContent": str,
@@ -694,19 +788,21 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class APNSSandboxChannelResponseTypeDef(
     _RequiredAPNSSandboxChannelResponseTypeDef, _OptionalAPNSSandboxChannelResponseTypeDef
 ):
     pass
 
+
 APNSVoipChannelRequestTypeDef = TypedDict(
     "APNSVoipChannelRequestTypeDef",
     {
         "BundleId": str,
         "Certificate": str,
         "DefaultAuthenticationMethod": str,
         "Enabled": bool,
@@ -738,19 +834,21 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class APNSVoipChannelResponseTypeDef(
     _RequiredAPNSVoipChannelResponseTypeDef, _OptionalAPNSVoipChannelResponseTypeDef
 ):
     pass
 
+
 APNSVoipSandboxChannelRequestTypeDef = TypedDict(
     "APNSVoipSandboxChannelRequestTypeDef",
     {
         "BundleId": str,
         "Certificate": str,
         "DefaultAuthenticationMethod": str,
         "Enabled": bool,
@@ -782,19 +880,21 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class APNSVoipSandboxChannelResponseTypeDef(
     _RequiredAPNSVoipSandboxChannelResponseTypeDef, _OptionalAPNSVoipSandboxChannelResponseTypeDef
 ):
     pass
 
+
 _RequiredActivityResponseTypeDef = TypedDict(
     "_RequiredActivityResponseTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
         "Id": str,
     },
@@ -813,17 +913,48 @@
         "TotalEndpointCount": int,
         "TreatmentId": str,
         "ExecutionMetrics": Dict[str, str],
     },
     total=False,
 )
 
+
 class ActivityResponseTypeDef(_RequiredActivityResponseTypeDef, _OptionalActivityResponseTypeDef):
     pass
 
+
+ContactCenterActivityOutputTypeDef = TypedDict(
+    "ContactCenterActivityOutputTypeDef",
+    {
+        "NextActivity": str,
+    },
+    total=False,
+)
+
+_RequiredHoldoutActivityOutputTypeDef = TypedDict(
+    "_RequiredHoldoutActivityOutputTypeDef",
+    {
+        "Percentage": int,
+    },
+)
+_OptionalHoldoutActivityOutputTypeDef = TypedDict(
+    "_OptionalHoldoutActivityOutputTypeDef",
+    {
+        "NextActivity": str,
+    },
+    total=False,
+)
+
+
+class HoldoutActivityOutputTypeDef(
+    _RequiredHoldoutActivityOutputTypeDef, _OptionalHoldoutActivityOutputTypeDef
+):
+    pass
+
+
 ContactCenterActivityTypeDef = TypedDict(
     "ContactCenterActivityTypeDef",
     {
         "NextActivity": str,
     },
     total=False,
 )
@@ -838,30 +969,48 @@
     "_OptionalHoldoutActivityTypeDef",
     {
         "NextActivity": str,
     },
     total=False,
 )
 
+
 class HoldoutActivityTypeDef(_RequiredHoldoutActivityTypeDef, _OptionalHoldoutActivityTypeDef):
     pass
 
+
 AddressConfigurationTypeDef = TypedDict(
     "AddressConfigurationTypeDef",
     {
         "BodyOverride": str,
         "ChannelType": ChannelTypeType,
         "Context": Mapping[str, str],
         "RawContent": str,
         "Substitutions": Mapping[str, Sequence[str]],
         "TitleOverride": str,
     },
     total=False,
 )
 
+AndroidPushNotificationTemplateOutputTypeDef = TypedDict(
+    "AndroidPushNotificationTemplateOutputTypeDef",
+    {
+        "Action": ActionType,
+        "Body": str,
+        "ImageIconUrl": str,
+        "ImageUrl": str,
+        "RawContent": str,
+        "SmallImageIconUrl": str,
+        "Sound": str,
+        "Title": str,
+        "Url": str,
+    },
+    total=False,
+)
+
 AndroidPushNotificationTemplateTypeDef = TypedDict(
     "AndroidPushNotificationTemplateTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "ImageIconUrl": str,
         "ImageUrl": str,
@@ -887,69 +1036,94 @@
     {
         "tags": Dict[str, str],
         "CreationDate": str,
     },
     total=False,
 )
 
+
 class ApplicationResponseTypeDef(
     _RequiredApplicationResponseTypeDef, _OptionalApplicationResponseTypeDef
 ):
     pass
 
-CampaignHookTypeDef = TypedDict(
-    "CampaignHookTypeDef",
+
+CampaignHookOutputTypeDef = TypedDict(
+    "CampaignHookOutputTypeDef",
     {
         "LambdaFunctionName": str,
         "Mode": ModeType,
         "WebUrl": str,
     },
     total=False,
 )
 
-CampaignLimitsTypeDef = TypedDict(
-    "CampaignLimitsTypeDef",
+CampaignLimitsOutputTypeDef = TypedDict(
+    "CampaignLimitsOutputTypeDef",
     {
         "Daily": int,
         "MaximumDuration": int,
         "MessagesPerSecond": int,
         "Total": int,
         "Session": int,
     },
     total=False,
 )
 
-QuietTimeTypeDef = TypedDict(
-    "QuietTimeTypeDef",
+QuietTimeOutputTypeDef = TypedDict(
+    "QuietTimeOutputTypeDef",
     {
         "End": str,
         "Start": str,
     },
     total=False,
 )
 
+_RequiredAttributeDimensionOutputTypeDef = TypedDict(
+    "_RequiredAttributeDimensionOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+)
+_OptionalAttributeDimensionOutputTypeDef = TypedDict(
+    "_OptionalAttributeDimensionOutputTypeDef",
+    {
+        "AttributeType": AttributeTypeType,
+    },
+    total=False,
+)
+
+
+class AttributeDimensionOutputTypeDef(
+    _RequiredAttributeDimensionOutputTypeDef, _OptionalAttributeDimensionOutputTypeDef
+):
+    pass
+
+
 _RequiredAttributeDimensionTypeDef = TypedDict(
     "_RequiredAttributeDimensionTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 _OptionalAttributeDimensionTypeDef = TypedDict(
     "_OptionalAttributeDimensionTypeDef",
     {
         "AttributeType": AttributeTypeType,
     },
     total=False,
 )
 
+
 class AttributeDimensionTypeDef(
     _RequiredAttributeDimensionTypeDef, _OptionalAttributeDimensionTypeDef
 ):
     pass
 
+
 _RequiredAttributesResourceTypeDef = TypedDict(
     "_RequiredAttributesResourceTypeDef",
     {
         "ApplicationId": str,
         "AttributeType": str,
     },
 )
@@ -957,19 +1131,21 @@
     "_OptionalAttributesResourceTypeDef",
     {
         "Attributes": List[str],
     },
     total=False,
 )
 
+
 class AttributesResourceTypeDef(
     _RequiredAttributesResourceTypeDef, _OptionalAttributesResourceTypeDef
 ):
     pass
 
+
 _RequiredBaiduChannelRequestTypeDef = TypedDict(
     "_RequiredBaiduChannelRequestTypeDef",
     {
         "ApiKey": str,
         "SecretKey": str,
     },
 )
@@ -977,19 +1153,21 @@
     "_OptionalBaiduChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+
 class BaiduChannelRequestTypeDef(
     _RequiredBaiduChannelRequestTypeDef, _OptionalBaiduChannelRequestTypeDef
 ):
     pass
 
+
 _RequiredBaiduChannelResponseTypeDef = TypedDict(
     "_RequiredBaiduChannelResponseTypeDef",
     {
         "Credential": str,
         "Platform": str,
     },
 )
@@ -1005,19 +1183,21 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class BaiduChannelResponseTypeDef(
     _RequiredBaiduChannelResponseTypeDef, _OptionalBaiduChannelResponseTypeDef
 ):
     pass
 
+
 BaiduMessageTypeDef = TypedDict(
     "BaiduMessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "Data": Mapping[str, str],
         "IconReference": str,
@@ -1031,60 +1211,117 @@
         "TimeToLive": int,
         "Title": str,
         "Url": str,
     },
     total=False,
 )
 
+CampaignCustomMessageOutputTypeDef = TypedDict(
+    "CampaignCustomMessageOutputTypeDef",
+    {
+        "Data": str,
+    },
+    total=False,
+)
+
 CampaignCustomMessageTypeDef = TypedDict(
     "CampaignCustomMessageTypeDef",
     {
         "Data": str,
     },
     total=False,
 )
 
+CampaignEmailMessageOutputTypeDef = TypedDict(
+    "CampaignEmailMessageOutputTypeDef",
+    {
+        "Body": str,
+        "FromAddress": str,
+        "HtmlBody": str,
+        "Title": str,
+    },
+    total=False,
+)
+
 CampaignEmailMessageTypeDef = TypedDict(
     "CampaignEmailMessageTypeDef",
     {
         "Body": str,
         "FromAddress": str,
         "HtmlBody": str,
         "Title": str,
     },
     total=False,
 )
 
+CampaignHookTypeDef = TypedDict(
+    "CampaignHookTypeDef",
+    {
+        "LambdaFunctionName": str,
+        "Mode": ModeType,
+        "WebUrl": str,
+    },
+    total=False,
+)
+
+CampaignLimitsTypeDef = TypedDict(
+    "CampaignLimitsTypeDef",
+    {
+        "Daily": int,
+        "MaximumDuration": int,
+        "MessagesPerSecond": int,
+        "Total": int,
+        "Session": int,
+    },
+    total=False,
+)
+
 CampaignStateTypeDef = TypedDict(
     "CampaignStateTypeDef",
     {
         "CampaignStatus": CampaignStatusType,
     },
     total=False,
 )
 
-_RequiredCustomDeliveryConfigurationTypeDef = TypedDict(
-    "_RequiredCustomDeliveryConfigurationTypeDef",
+_RequiredCustomDeliveryConfigurationOutputTypeDef = TypedDict(
+    "_RequiredCustomDeliveryConfigurationOutputTypeDef",
     {
         "DeliveryUri": str,
     },
 )
-_OptionalCustomDeliveryConfigurationTypeDef = TypedDict(
-    "_OptionalCustomDeliveryConfigurationTypeDef",
+_OptionalCustomDeliveryConfigurationOutputTypeDef = TypedDict(
+    "_OptionalCustomDeliveryConfigurationOutputTypeDef",
     {
-        "EndpointTypes": Sequence[EndpointTypesElementType],
+        "EndpointTypes": List[EndpointTypesElementType],
     },
     total=False,
 )
 
-class CustomDeliveryConfigurationTypeDef(
-    _RequiredCustomDeliveryConfigurationTypeDef, _OptionalCustomDeliveryConfigurationTypeDef
+
+class CustomDeliveryConfigurationOutputTypeDef(
+    _RequiredCustomDeliveryConfigurationOutputTypeDef,
+    _OptionalCustomDeliveryConfigurationOutputTypeDef,
 ):
     pass
 
+
+CampaignSmsMessageOutputTypeDef = TypedDict(
+    "CampaignSmsMessageOutputTypeDef",
+    {
+        "Body": str,
+        "MessageType": MessageTypeType,
+        "OriginationNumber": str,
+        "SenderId": str,
+        "EntityId": str,
+        "TemplateId": str,
+    },
+    total=False,
+)
+
 CampaignSmsMessageTypeDef = TypedDict(
     "CampaignSmsMessageTypeDef",
     {
         "Body": str,
         "MessageType": MessageTypeType,
         "OriginationNumber": str,
         "SenderId": str,
@@ -1106,24 +1343,43 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+ClosedDaysRuleOutputTypeDef = TypedDict(
+    "ClosedDaysRuleOutputTypeDef",
+    {
+        "Name": str,
+        "StartDateTime": str,
+        "EndDateTime": str,
+    },
+    total=False,
+)
+
 ClosedDaysRuleTypeDef = TypedDict(
     "ClosedDaysRuleTypeDef",
     {
         "Name": str,
         "StartDateTime": str,
         "EndDateTime": str,
     },
     total=False,
 )
 
+WaitTimeOutputTypeDef = TypedDict(
+    "WaitTimeOutputTypeDef",
+    {
+        "WaitFor": str,
+        "WaitUntil": str,
+    },
+    total=False,
+)
+
 WaitTimeTypeDef = TypedDict(
     "WaitTimeTypeDef",
     {
         "WaitFor": str,
         "WaitUntil": str,
     },
     total=False,
@@ -1139,19 +1395,32 @@
     "_OptionalCreateApplicationRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateApplicationRequestTypeDef(
     _RequiredCreateApplicationRequestTypeDef, _OptionalCreateApplicationRequestTypeDef
 ):
     pass
 
+
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
 EmailTemplateRequestTypeDef = TypedDict(
     "EmailTemplateRequestTypeDef",
     {
         "DefaultSubstitutions": str,
         "HtmlPart": str,
         "RecommenderId": str,
         "Subject": str,
@@ -1184,17 +1453,19 @@
     {
         "SegmentId": str,
         "SegmentVersion": int,
     },
     total=False,
 )
 
+
 class ExportJobRequestTypeDef(_RequiredExportJobRequestTypeDef, _OptionalExportJobRequestTypeDef):
     pass
 
+
 _RequiredImportJobRequestTypeDef = TypedDict(
     "_RequiredImportJobRequestTypeDef",
     {
         "Format": FormatType,
         "RoleArn": str,
         "S3Url": str,
     },
@@ -1207,17 +1478,19 @@
         "RegisterEndpoints": bool,
         "SegmentId": str,
         "SegmentName": str,
     },
     total=False,
 )
 
+
 class ImportJobRequestTypeDef(_RequiredImportJobRequestTypeDef, _OptionalImportJobRequestTypeDef):
     pass
 
+
 TemplateCreateMessageBodyTypeDef = TypedDict(
     "TemplateCreateMessageBodyTypeDef",
     {
         "Arn": str,
         "Message": str,
         "RequestID": str,
     },
@@ -1241,19 +1514,21 @@
         "RecommendationTransformerUri": str,
         "RecommendationsDisplayName": str,
         "RecommendationsPerMessage": int,
     },
     total=False,
 )
 
+
 class CreateRecommenderConfigurationTypeDef(
     _RequiredCreateRecommenderConfigurationTypeDef, _OptionalCreateRecommenderConfigurationTypeDef
 ):
     pass
 
+
 _RequiredRecommenderConfigurationResponseTypeDef = TypedDict(
     "_RequiredRecommenderConfigurationResponseTypeDef",
     {
         "CreationDate": str,
         "Id": str,
         "LastModifiedDate": str,
         "RecommendationProviderRoleArn": str,
@@ -1270,20 +1545,22 @@
         "RecommendationTransformerUri": str,
         "RecommendationsDisplayName": str,
         "RecommendationsPerMessage": int,
     },
     total=False,
 )
 
+
 class RecommenderConfigurationResponseTypeDef(
     _RequiredRecommenderConfigurationResponseTypeDef,
     _OptionalRecommenderConfigurationResponseTypeDef,
 ):
     pass
 
+
 SMSTemplateRequestTypeDef = TypedDict(
     "SMSTemplateRequestTypeDef",
     {
         "Body": str,
         "DefaultSubstitutions": str,
         "RecommenderId": str,
         "tags": Mapping[str, str],
@@ -1301,22 +1578,77 @@
         "tags": Mapping[str, str],
         "TemplateDescription": str,
         "VoiceId": str,
     },
     total=False,
 )
 
+_RequiredCustomDeliveryConfigurationTypeDef = TypedDict(
+    "_RequiredCustomDeliveryConfigurationTypeDef",
+    {
+        "DeliveryUri": str,
+    },
+)
+_OptionalCustomDeliveryConfigurationTypeDef = TypedDict(
+    "_OptionalCustomDeliveryConfigurationTypeDef",
+    {
+        "EndpointTypes": Sequence[EndpointTypesElementType],
+    },
+    total=False,
+)
+
+
+class CustomDeliveryConfigurationTypeDef(
+    _RequiredCustomDeliveryConfigurationTypeDef, _OptionalCustomDeliveryConfigurationTypeDef
+):
+    pass
+
+
+JourneyCustomMessageOutputTypeDef = TypedDict(
+    "JourneyCustomMessageOutputTypeDef",
+    {
+        "Data": str,
+    },
+    total=False,
+)
+
 JourneyCustomMessageTypeDef = TypedDict(
     "JourneyCustomMessageTypeDef",
     {
         "Data": str,
     },
     total=False,
 )
 
+_RequiredDefaultButtonConfigurationOutputTypeDef = TypedDict(
+    "_RequiredDefaultButtonConfigurationOutputTypeDef",
+    {
+        "ButtonAction": ButtonActionType,
+        "Text": str,
+    },
+)
+_OptionalDefaultButtonConfigurationOutputTypeDef = TypedDict(
+    "_OptionalDefaultButtonConfigurationOutputTypeDef",
+    {
+        "BackgroundColor": str,
+        "BorderRadius": int,
+        "Link": str,
+        "TextColor": str,
+    },
+    total=False,
+)
+
+
+class DefaultButtonConfigurationOutputTypeDef(
+    _RequiredDefaultButtonConfigurationOutputTypeDef,
+    _OptionalDefaultButtonConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredDefaultButtonConfigurationTypeDef = TypedDict(
     "_RequiredDefaultButtonConfigurationTypeDef",
     {
         "ButtonAction": ButtonActionType,
         "Text": str,
     },
 )
@@ -1327,19 +1659,21 @@
         "BorderRadius": int,
         "Link": str,
         "TextColor": str,
     },
     total=False,
 )
 
+
 class DefaultButtonConfigurationTypeDef(
     _RequiredDefaultButtonConfigurationTypeDef, _OptionalDefaultButtonConfigurationTypeDef
 ):
     pass
 
+
 DefaultMessageTypeDef = TypedDict(
     "DefaultMessageTypeDef",
     {
         "Body": str,
         "Substitutions": Mapping[str, Sequence[str]],
     },
     total=False,
@@ -1355,14 +1689,26 @@
         "Substitutions": Mapping[str, Sequence[str]],
         "Title": str,
         "Url": str,
     },
     total=False,
 )
 
+DefaultPushNotificationTemplateOutputTypeDef = TypedDict(
+    "DefaultPushNotificationTemplateOutputTypeDef",
+    {
+        "Action": ActionType,
+        "Body": str,
+        "Sound": str,
+        "Title": str,
+        "Url": str,
+    },
+    total=False,
+)
+
 DefaultPushNotificationTemplateTypeDef = TypedDict(
     "DefaultPushNotificationTemplateTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "Sound": str,
         "Title": str,
@@ -1458,39 +1804,43 @@
         "MessagesPerSecond": int,
         "RoleArn": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class EmailChannelResponseTypeDef(
     _RequiredEmailChannelResponseTypeDef, _OptionalEmailChannelResponseTypeDef
 ):
     pass
 
+
 _RequiredDeleteEmailTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteEmailTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteEmailTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class DeleteEmailTemplateRequestRequestTypeDef(
     _RequiredDeleteEmailTemplateRequestRequestTypeDef,
     _OptionalDeleteEmailTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 MessageBodyTypeDef = TypedDict(
     "MessageBodyTypeDef",
     {
         "Message": str,
         "RequestID": str,
     },
     total=False,
@@ -1525,17 +1875,19 @@
         "ExternalId": str,
         "LastModifiedDate": str,
         "LastUpdatedBy": str,
     },
     total=False,
 )
 
+
 class EventStreamTypeDef(_RequiredEventStreamTypeDef, _OptionalEventStreamTypeDef):
     pass
 
+
 DeleteGcmChannelRequestRequestTypeDef = TypedDict(
     "DeleteGcmChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -1558,39 +1910,43 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class GCMChannelResponseTypeDef(
     _RequiredGCMChannelResponseTypeDef, _OptionalGCMChannelResponseTypeDef
 ):
     pass
 
+
 _RequiredDeleteInAppTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteInAppTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteInAppTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteInAppTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class DeleteInAppTemplateRequestRequestTypeDef(
     _RequiredDeleteInAppTemplateRequestRequestTypeDef,
     _OptionalDeleteInAppTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteJourneyRequestRequestTypeDef = TypedDict(
     "DeleteJourneyRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
     },
 )
@@ -1605,20 +1961,22 @@
     "_OptionalDeletePushTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class DeletePushTemplateRequestRequestTypeDef(
     _RequiredDeletePushTemplateRequestRequestTypeDef,
     _OptionalDeletePushTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteRecommenderConfigurationRequestRequestTypeDef",
     {
         "RecommenderId": str,
     },
 )
 
@@ -1659,38 +2017,42 @@
         "ShortCode": str,
         "TransactionalMessagesPerSecond": int,
         "Version": int,
     },
     total=False,
 )
 
+
 class SMSChannelResponseTypeDef(
     _RequiredSMSChannelResponseTypeDef, _OptionalSMSChannelResponseTypeDef
 ):
     pass
 
+
 _RequiredDeleteSmsTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteSmsTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteSmsTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteSmsTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class DeleteSmsTemplateRequestRequestTypeDef(
     _RequiredDeleteSmsTemplateRequestRequestTypeDef, _OptionalDeleteSmsTemplateRequestRequestTypeDef
 ):
     pass
 
+
 DeleteUserEndpointsRequestRequestTypeDef = TypedDict(
     "DeleteUserEndpointsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "UserId": str,
     },
 )
@@ -1720,39 +2082,43 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
+
 class VoiceChannelResponseTypeDef(
     _RequiredVoiceChannelResponseTypeDef, _OptionalVoiceChannelResponseTypeDef
 ):
     pass
 
+
 _RequiredDeleteVoiceTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteVoiceTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalDeleteVoiceTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteVoiceTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class DeleteVoiceTemplateRequestRequestTypeDef(
     _RequiredDeleteVoiceTemplateRequestRequestTypeDef,
     _OptionalDeleteVoiceTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 GCMMessageTypeDef = TypedDict(
     "GCMMessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "CollapseKey": str,
         "Data": Mapping[str, str],
@@ -1814,19 +2180,29 @@
         "ConfigurationSet": str,
         "Enabled": bool,
         "RoleArn": str,
     },
     total=False,
 )
 
+
 class EmailChannelRequestTypeDef(
     _RequiredEmailChannelRequestTypeDef, _OptionalEmailChannelRequestTypeDef
 ):
     pass
 
+
+JourneyEmailMessageOutputTypeDef = TypedDict(
+    "JourneyEmailMessageOutputTypeDef",
+    {
+        "FromAddress": str,
+    },
+    total=False,
+)
+
 JourneyEmailMessageTypeDef = TypedDict(
     "JourneyEmailMessageTypeDef",
     {
         "FromAddress": str,
     },
     total=False,
 )
@@ -1860,25 +2236,20 @@
         "TemplateDescription": str,
         "TextPart": str,
         "Version": str,
     },
     total=False,
 )
 
+
 class EmailTemplateResponseTypeDef(
     _RequiredEmailTemplateResponseTypeDef, _OptionalEmailTemplateResponseTypeDef
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 EndpointDemographicTypeDef = TypedDict(
     "EndpointDemographicTypeDef",
     {
         "AppVersion": str,
         "Locale": str,
         "Make": str,
@@ -1903,29 +2274,57 @@
     },
     total=False,
 )
 
 EndpointUserTypeDef = TypedDict(
     "EndpointUserTypeDef",
     {
-        "UserAttributes": Dict[str, List[str]],
+        "UserAttributes": Mapping[str, Sequence[str]],
         "UserId": str,
     },
     total=False,
 )
 
+EndpointDemographicOutputTypeDef = TypedDict(
+    "EndpointDemographicOutputTypeDef",
+    {
+        "AppVersion": str,
+        "Locale": str,
+        "Make": str,
+        "Model": str,
+        "ModelVersion": str,
+        "Platform": str,
+        "PlatformVersion": str,
+        "Timezone": str,
+    },
+    total=False,
+)
+
 EndpointItemResponseTypeDef = TypedDict(
     "EndpointItemResponseTypeDef",
     {
         "Message": str,
         "StatusCode": int,
     },
     total=False,
 )
 
+EndpointLocationOutputTypeDef = TypedDict(
+    "EndpointLocationOutputTypeDef",
+    {
+        "City": str,
+        "Country": str,
+        "Latitude": float,
+        "Longitude": float,
+        "PostalCode": str,
+        "Region": str,
+    },
+    total=False,
+)
+
 _RequiredEndpointMessageResultTypeDef = TypedDict(
     "_RequiredEndpointMessageResultTypeDef",
     {
         "DeliveryStatus": DeliveryStatusType,
         "StatusCode": int,
     },
 )
@@ -1936,31 +2335,71 @@
         "MessageId": str,
         "StatusMessage": str,
         "UpdatedToken": str,
     },
     total=False,
 )
 
+
 class EndpointMessageResultTypeDef(
     _RequiredEndpointMessageResultTypeDef, _OptionalEndpointMessageResultTypeDef
 ):
     pass
 
+
+EndpointUserOutputTypeDef = TypedDict(
+    "EndpointUserOutputTypeDef",
+    {
+        "UserAttributes": Dict[str, List[str]],
+        "UserId": str,
+    },
+    total=False,
+)
+
 EndpointSendConfigurationTypeDef = TypedDict(
     "EndpointSendConfigurationTypeDef",
     {
         "BodyOverride": str,
         "Context": Mapping[str, str],
         "RawContent": str,
         "Substitutions": Mapping[str, Sequence[str]],
         "TitleOverride": str,
     },
     total=False,
 )
 
+MetricDimensionOutputTypeDef = TypedDict(
+    "MetricDimensionOutputTypeDef",
+    {
+        "ComparisonOperator": str,
+        "Value": float,
+    },
+)
+
+_RequiredSetDimensionOutputTypeDef = TypedDict(
+    "_RequiredSetDimensionOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+)
+_OptionalSetDimensionOutputTypeDef = TypedDict(
+    "_OptionalSetDimensionOutputTypeDef",
+    {
+        "DimensionType": DimensionTypeType,
+    },
+    total=False,
+)
+
+
+class SetDimensionOutputTypeDef(
+    _RequiredSetDimensionOutputTypeDef, _OptionalSetDimensionOutputTypeDef
+):
+    pass
+
+
 MetricDimensionTypeDef = TypedDict(
     "MetricDimensionTypeDef",
     {
         "ComparisonOperator": str,
         "Value": float,
     },
 )
@@ -1975,17 +2414,19 @@
     "_OptionalSetDimensionTypeDef",
     {
         "DimensionType": DimensionTypeType,
     },
     total=False,
 )
 
+
 class SetDimensionTypeDef(_RequiredSetDimensionTypeDef, _OptionalSetDimensionTypeDef):
     pass
 
+
 EventItemResponseTypeDef = TypedDict(
     "EventItemResponseTypeDef",
     {
         "Message": str,
         "StatusCode": int,
     },
     total=False,
@@ -2003,17 +2444,19 @@
     {
         "Duration": int,
         "StopTimestamp": str,
     },
     total=False,
 )
 
+
 class SessionTypeDef(_RequiredSessionTypeDef, _OptionalSessionTypeDef):
     pass
 
+
 _RequiredExportJobResourceTypeDef = TypedDict(
     "_RequiredExportJobResourceTypeDef",
     {
         "RoleArn": str,
         "S3UrlPrefix": str,
     },
 )
@@ -2022,38 +2465,50 @@
     {
         "SegmentId": str,
         "SegmentVersion": int,
     },
     total=False,
 )
 
+
 class ExportJobResourceTypeDef(
     _RequiredExportJobResourceTypeDef, _OptionalExportJobResourceTypeDef
 ):
     pass
 
+
 _RequiredGCMChannelRequestTypeDef = TypedDict(
     "_RequiredGCMChannelRequestTypeDef",
     {
         "ApiKey": str,
     },
 )
 _OptionalGCMChannelRequestTypeDef = TypedDict(
     "_OptionalGCMChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+
 class GCMChannelRequestTypeDef(
     _RequiredGCMChannelRequestTypeDef, _OptionalGCMChannelRequestTypeDef
 ):
     pass
 
+
+GPSCoordinatesOutputTypeDef = TypedDict(
+    "GPSCoordinatesOutputTypeDef",
+    {
+        "Latitude": float,
+        "Longitude": float,
+    },
+)
+
 GPSCoordinatesTypeDef = TypedDict(
     "GPSCoordinatesTypeDef",
     {
         "Latitude": float,
         "Longitude": float,
     },
 )
@@ -2114,20 +2569,22 @@
         "NextToken": str,
         "PageSize": str,
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class GetApplicationDateRangeKpiRequestRequestTypeDef(
     _RequiredGetApplicationDateRangeKpiRequestRequestTypeDef,
     _OptionalGetApplicationDateRangeKpiRequestRequestTypeDef,
 ):
     pass
 
+
 GetApplicationSettingsRequestRequestTypeDef = TypedDict(
     "GetApplicationSettingsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2159,20 +2616,22 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetCampaignActivitiesRequestRequestTypeDef(
     _RequiredGetCampaignActivitiesRequestRequestTypeDef,
     _OptionalGetCampaignActivitiesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetCampaignDateRangeKpiRequestRequestTypeDef = TypedDict(
     "_RequiredGetCampaignDateRangeKpiRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
         "KpiName": str,
     },
@@ -2184,20 +2643,22 @@
         "NextToken": str,
         "PageSize": str,
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class GetCampaignDateRangeKpiRequestRequestTypeDef(
     _RequiredGetCampaignDateRangeKpiRequestRequestTypeDef,
     _OptionalGetCampaignDateRangeKpiRequestRequestTypeDef,
 ):
     pass
 
+
 GetCampaignRequestRequestTypeDef = TypedDict(
     "GetCampaignRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
     },
 )
@@ -2223,20 +2684,22 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetCampaignVersionsRequestRequestTypeDef(
     _RequiredGetCampaignVersionsRequestRequestTypeDef,
     _OptionalGetCampaignVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetCampaignsRequestRequestTypeDef = TypedDict(
     "_RequiredGetCampaignsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalGetCampaignsRequestRequestTypeDef = TypedDict(
@@ -2244,19 +2707,21 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetCampaignsRequestRequestTypeDef(
     _RequiredGetCampaignsRequestRequestTypeDef, _OptionalGetCampaignsRequestRequestTypeDef
 ):
     pass
 
+
 GetChannelsRequestRequestTypeDef = TypedDict(
     "GetChannelsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2277,19 +2742,21 @@
     "_OptionalGetEmailTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class GetEmailTemplateRequestRequestTypeDef(
     _RequiredGetEmailTemplateRequestRequestTypeDef, _OptionalGetEmailTemplateRequestRequestTypeDef
 ):
     pass
 
+
 GetEndpointRequestRequestTypeDef = TypedDict(
     "GetEndpointRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EndpointId": str,
     },
 )
@@ -2320,19 +2787,21 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetExportJobsRequestRequestTypeDef(
     _RequiredGetExportJobsRequestRequestTypeDef, _OptionalGetExportJobsRequestRequestTypeDef
 ):
     pass
 
+
 GetGcmChannelRequestRequestTypeDef = TypedDict(
     "GetGcmChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2355,19 +2824,21 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetImportJobsRequestRequestTypeDef(
     _RequiredGetImportJobsRequestRequestTypeDef, _OptionalGetImportJobsRequestRequestTypeDef
 ):
     pass
 
+
 GetInAppMessagesRequestRequestTypeDef = TypedDict(
     "GetInAppMessagesRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EndpointId": str,
     },
 )
@@ -2382,19 +2853,21 @@
     "_OptionalGetInAppTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class GetInAppTemplateRequestRequestTypeDef(
     _RequiredGetInAppTemplateRequestRequestTypeDef, _OptionalGetInAppTemplateRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetJourneyDateRangeKpiRequestRequestTypeDef = TypedDict(
     "_RequiredGetJourneyDateRangeKpiRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
         "KpiName": str,
     },
@@ -2406,20 +2879,22 @@
         "NextToken": str,
         "PageSize": str,
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class GetJourneyDateRangeKpiRequestRequestTypeDef(
     _RequiredGetJourneyDateRangeKpiRequestRequestTypeDef,
     _OptionalGetJourneyDateRangeKpiRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyActivityId": str,
         "JourneyId": str,
     },
@@ -2429,20 +2904,22 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
+
 class GetJourneyExecutionActivityMetricsRequestRequestTypeDef(
     _RequiredGetJourneyExecutionActivityMetricsRequestRequestTypeDef,
     _OptionalGetJourneyExecutionActivityMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 JourneyExecutionActivityMetricsResponseTypeDef = TypedDict(
     "JourneyExecutionActivityMetricsResponseTypeDef",
     {
         "ActivityType": str,
         "ApplicationId": str,
         "JourneyActivityId": str,
         "JourneyId": str,
@@ -2463,20 +2940,22 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
+
 class GetJourneyExecutionMetricsRequestRequestTypeDef(
     _RequiredGetJourneyExecutionMetricsRequestRequestTypeDef,
     _OptionalGetJourneyExecutionMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 JourneyExecutionMetricsResponseTypeDef = TypedDict(
     "JourneyExecutionMetricsResponseTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
         "LastEvaluatedTime": str,
         "Metrics": Dict[str, str],
@@ -2505,20 +2984,22 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
+
 class GetJourneyRunExecutionActivityMetricsRequestRequestTypeDef(
     _RequiredGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
     _OptionalGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 JourneyRunExecutionActivityMetricsResponseTypeDef = TypedDict(
     "JourneyRunExecutionActivityMetricsResponseTypeDef",
     {
         "ActivityType": str,
         "ApplicationId": str,
         "JourneyActivityId": str,
         "JourneyId": str,
@@ -2541,20 +3022,22 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
+
 class GetJourneyRunExecutionMetricsRequestRequestTypeDef(
     _RequiredGetJourneyRunExecutionMetricsRequestRequestTypeDef,
     _OptionalGetJourneyRunExecutionMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 JourneyRunExecutionMetricsResponseTypeDef = TypedDict(
     "JourneyRunExecutionMetricsResponseTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
         "LastEvaluatedTime": str,
         "Metrics": Dict[str, str],
@@ -2574,38 +3057,42 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetJourneyRunsRequestRequestTypeDef(
     _RequiredGetJourneyRunsRequestRequestTypeDef, _OptionalGetJourneyRunsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetPushTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredGetPushTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalGetPushTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalGetPushTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class GetPushTemplateRequestRequestTypeDef(
     _RequiredGetPushTemplateRequestRequestTypeDef, _OptionalGetPushTemplateRequestRequestTypeDef
 ):
     pass
 
+
 GetRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "GetRecommenderConfigurationRequestRequestTypeDef",
     {
         "RecommenderId": str,
     },
 )
 
@@ -2630,20 +3117,22 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetSegmentExportJobsRequestRequestTypeDef(
     _RequiredGetSegmentExportJobsRequestRequestTypeDef,
     _OptionalGetSegmentExportJobsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetSegmentImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSegmentImportJobsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "SegmentId": str,
     },
 )
@@ -2652,20 +3141,22 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetSegmentImportJobsRequestRequestTypeDef(
     _RequiredGetSegmentImportJobsRequestRequestTypeDef,
     _OptionalGetSegmentImportJobsRequestRequestTypeDef,
 ):
     pass
 
+
 GetSegmentRequestRequestTypeDef = TypedDict(
     "GetSegmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "SegmentId": str,
     },
 )
@@ -2691,20 +3182,22 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetSegmentVersionsRequestRequestTypeDef(
     _RequiredGetSegmentVersionsRequestRequestTypeDef,
     _OptionalGetSegmentVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetSegmentsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSegmentsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalGetSegmentsRequestRequestTypeDef = TypedDict(
@@ -2712,19 +3205,21 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class GetSegmentsRequestRequestTypeDef(
     _RequiredGetSegmentsRequestRequestTypeDef, _OptionalGetSegmentsRequestRequestTypeDef
 ):
     pass
 
+
 GetSmsChannelRequestRequestTypeDef = TypedDict(
     "GetSmsChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -2738,19 +3233,21 @@
     "_OptionalGetSmsTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class GetSmsTemplateRequestRequestTypeDef(
     _RequiredGetSmsTemplateRequestRequestTypeDef, _OptionalGetSmsTemplateRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredSMSTemplateResponseTypeDef = TypedDict(
     "_RequiredSMSTemplateResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
@@ -2766,19 +3263,21 @@
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
+
 class SMSTemplateResponseTypeDef(
     _RequiredSMSTemplateResponseTypeDef, _OptionalSMSTemplateResponseTypeDef
 ):
     pass
 
+
 GetUserEndpointsRequestRequestTypeDef = TypedDict(
     "GetUserEndpointsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "UserId": str,
     },
 )
@@ -2800,19 +3299,21 @@
     "_OptionalGetVoiceTemplateRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class GetVoiceTemplateRequestRequestTypeDef(
     _RequiredGetVoiceTemplateRequestRequestTypeDef, _OptionalGetVoiceTemplateRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredVoiceTemplateResponseTypeDef = TypedDict(
     "_RequiredVoiceTemplateResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
@@ -2829,19 +3330,21 @@
         "TemplateDescription": str,
         "Version": str,
         "VoiceId": str,
     },
     total=False,
 )
 
+
 class VoiceTemplateResponseTypeDef(
     _RequiredVoiceTemplateResponseTypeDef, _OptionalVoiceTemplateResponseTypeDef
 ):
     pass
 
+
 _RequiredImportJobResourceTypeDef = TypedDict(
     "_RequiredImportJobResourceTypeDef",
     {
         "Format": FormatType,
         "RoleArn": str,
         "S3Url": str,
     },
@@ -2854,89 +3357,161 @@
         "RegisterEndpoints": bool,
         "SegmentId": str,
         "SegmentName": str,
     },
     total=False,
 )
 
+
 class ImportJobResourceTypeDef(
     _RequiredImportJobResourceTypeDef, _OptionalImportJobResourceTypeDef
 ):
     pass
 
+
+InAppMessageBodyConfigOutputTypeDef = TypedDict(
+    "InAppMessageBodyConfigOutputTypeDef",
+    {
+        "Alignment": AlignmentType,
+        "Body": str,
+        "TextColor": str,
+    },
+)
+
 InAppMessageBodyConfigTypeDef = TypedDict(
     "InAppMessageBodyConfigTypeDef",
     {
         "Alignment": AlignmentType,
         "Body": str,
         "TextColor": str,
     },
 )
 
+_RequiredOverrideButtonConfigurationOutputTypeDef = TypedDict(
+    "_RequiredOverrideButtonConfigurationOutputTypeDef",
+    {
+        "ButtonAction": ButtonActionType,
+    },
+)
+_OptionalOverrideButtonConfigurationOutputTypeDef = TypedDict(
+    "_OptionalOverrideButtonConfigurationOutputTypeDef",
+    {
+        "Link": str,
+    },
+    total=False,
+)
+
+
+class OverrideButtonConfigurationOutputTypeDef(
+    _RequiredOverrideButtonConfigurationOutputTypeDef,
+    _OptionalOverrideButtonConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredOverrideButtonConfigurationTypeDef = TypedDict(
     "_RequiredOverrideButtonConfigurationTypeDef",
     {
         "ButtonAction": ButtonActionType,
     },
 )
 _OptionalOverrideButtonConfigurationTypeDef = TypedDict(
     "_OptionalOverrideButtonConfigurationTypeDef",
     {
         "Link": str,
     },
     total=False,
 )
 
+
 class OverrideButtonConfigurationTypeDef(
     _RequiredOverrideButtonConfigurationTypeDef, _OptionalOverrideButtonConfigurationTypeDef
 ):
     pass
 
+
+InAppMessageHeaderConfigOutputTypeDef = TypedDict(
+    "InAppMessageHeaderConfigOutputTypeDef",
+    {
+        "Alignment": AlignmentType,
+        "Header": str,
+        "TextColor": str,
+    },
+)
+
 InAppMessageHeaderConfigTypeDef = TypedDict(
     "InAppMessageHeaderConfigTypeDef",
     {
         "Alignment": AlignmentType,
         "Header": str,
         "TextColor": str,
     },
 )
 
+JourneyChannelSettingsOutputTypeDef = TypedDict(
+    "JourneyChannelSettingsOutputTypeDef",
+    {
+        "ConnectCampaignArn": str,
+        "ConnectCampaignExecutionRoleArn": str,
+    },
+    total=False,
+)
+
 JourneyChannelSettingsTypeDef = TypedDict(
     "JourneyChannelSettingsTypeDef",
     {
         "ConnectCampaignArn": str,
         "ConnectCampaignExecutionRoleArn": str,
     },
     total=False,
 )
 
+JourneyLimitsOutputTypeDef = TypedDict(
+    "JourneyLimitsOutputTypeDef",
+    {
+        "DailyCap": int,
+        "EndpointReentryCap": int,
+        "MessagesPerSecond": int,
+        "EndpointReentryInterval": str,
+    },
+    total=False,
+)
+
 JourneyLimitsTypeDef = TypedDict(
     "JourneyLimitsTypeDef",
     {
         "DailyCap": int,
         "EndpointReentryCap": int,
         "MessagesPerSecond": int,
         "EndpointReentryInterval": str,
     },
     total=False,
 )
 
+JourneyPushMessageOutputTypeDef = TypedDict(
+    "JourneyPushMessageOutputTypeDef",
+    {
+        "TimeToLive": str,
+    },
+    total=False,
+)
+
 JourneyPushMessageTypeDef = TypedDict(
     "JourneyPushMessageTypeDef",
     {
         "TimeToLive": str,
     },
     total=False,
 )
 
-JourneyScheduleTypeDef = TypedDict(
-    "JourneyScheduleTypeDef",
+JourneyScheduleOutputTypeDef = TypedDict(
+    "JourneyScheduleOutputTypeDef",
     {
-        "EndTime": Union[datetime, str],
-        "StartTime": Union[datetime, str],
+        "EndTime": datetime,
+        "StartTime": datetime,
         "Timezone": str,
     },
     total=False,
 )
 
 JourneyRunResponseTypeDef = TypedDict(
     "JourneyRunResponseTypeDef",
@@ -2944,26 +3519,48 @@
         "CreationTime": str,
         "LastUpdateTime": str,
         "RunId": str,
         "Status": JourneyRunStatusType,
     },
 )
 
+JourneySMSMessageOutputTypeDef = TypedDict(
+    "JourneySMSMessageOutputTypeDef",
+    {
+        "MessageType": MessageTypeType,
+        "OriginationNumber": str,
+        "SenderId": str,
+        "EntityId": str,
+        "TemplateId": str,
+    },
+    total=False,
+)
+
 JourneySMSMessageTypeDef = TypedDict(
     "JourneySMSMessageTypeDef",
     {
         "MessageType": MessageTypeType,
         "OriginationNumber": str,
         "SenderId": str,
         "EntityId": str,
         "TemplateId": str,
     },
     total=False,
 )
 
+JourneyScheduleTypeDef = TypedDict(
+    "JourneyScheduleTypeDef",
+    {
+        "EndTime": Union[datetime, str],
+        "StartTime": Union[datetime, str],
+        "Timezone": str,
+    },
+    total=False,
+)
+
 JourneyStateRequestTypeDef = TypedDict(
     "JourneyStateRequestTypeDef",
     {
         "State": StateType,
     },
     total=False,
 )
@@ -2979,28 +3576,30 @@
     {
         "PageSize": str,
         "Token": str,
     },
     total=False,
 )
 
+
 class ListJourneysRequestRequestTypeDef(
     _RequiredListJourneysRequestRequestTypeDef, _OptionalListJourneysRequestRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TagsModelTypeDef = TypedDict(
-    "TagsModelTypeDef",
+TagsModelOutputTypeDef = TypedDict(
+    "TagsModelOutputTypeDef",
     {
         "tags": Dict[str, str],
     },
 )
 
 _RequiredListTemplateVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplateVersionsRequestRequestTypeDef",
@@ -3014,31 +3613,52 @@
     {
         "NextToken": str,
         "PageSize": str,
     },
     total=False,
 )
 
+
 class ListTemplateVersionsRequestRequestTypeDef(
     _RequiredListTemplateVersionsRequestRequestTypeDef,
     _OptionalListTemplateVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListTemplatesRequestRequestTypeDef = TypedDict(
     "ListTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": str,
         "Prefix": str,
         "TemplateType": str,
     },
     total=False,
 )
 
+MessageOutputTypeDef = TypedDict(
+    "MessageOutputTypeDef",
+    {
+        "Action": ActionType,
+        "Body": str,
+        "ImageIconUrl": str,
+        "ImageSmallIconUrl": str,
+        "ImageUrl": str,
+        "JsonBody": str,
+        "MediaUrl": str,
+        "RawContent": str,
+        "SilentPush": bool,
+        "TimeToLive": int,
+        "Title": str,
+        "Url": str,
+    },
+    total=False,
+)
+
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "ImageIconUrl": str,
         "ImageSmallIconUrl": str,
@@ -3067,17 +3687,19 @@
         "MessageId": str,
         "StatusMessage": str,
         "UpdatedToken": str,
     },
     total=False,
 )
 
+
 class MessageResultTypeDef(_RequiredMessageResultTypeDef, _OptionalMessageResultTypeDef):
     pass
 
+
 NumberValidateRequestTypeDef = TypedDict(
     "NumberValidateRequestTypeDef",
     {
         "IsoCountryCode": str,
         "PhoneNumber": str,
     },
     total=False,
@@ -3100,14 +3722,23 @@
         "PhoneTypeCode": int,
         "Timezone": str,
         "ZipCode": str,
     },
     total=False,
 )
 
+OpenHoursRuleOutputTypeDef = TypedDict(
+    "OpenHoursRuleOutputTypeDef",
+    {
+        "StartTime": str,
+        "EndTime": str,
+    },
+    total=False,
+)
+
 OpenHoursRuleTypeDef = TypedDict(
     "OpenHoursRuleTypeDef",
     {
         "StartTime": str,
         "EndTime": str,
     },
     total=False,
@@ -3117,23 +3748,49 @@
     "WriteEventStreamTypeDef",
     {
         "DestinationStreamArn": str,
         "RoleArn": str,
     },
 )
 
+QuietTimeTypeDef = TypedDict(
+    "QuietTimeTypeDef",
+    {
+        "End": str,
+        "Start": str,
+    },
+    total=False,
+)
+
+RandomSplitEntryOutputTypeDef = TypedDict(
+    "RandomSplitEntryOutputTypeDef",
+    {
+        "NextActivity": str,
+        "Percentage": int,
+    },
+    total=False,
+)
+
 RandomSplitEntryTypeDef = TypedDict(
     "RandomSplitEntryTypeDef",
     {
         "NextActivity": str,
         "Percentage": int,
     },
     total=False,
 )
 
+RecencyDimensionOutputTypeDef = TypedDict(
+    "RecencyDimensionOutputTypeDef",
+    {
+        "Duration": DurationType,
+        "RecencyType": RecencyTypeType,
+    },
+)
+
 RecencyDimensionTypeDef = TypedDict(
     "RecencyDimensionTypeDef",
     {
         "Duration": DurationType,
         "RecencyType": RecencyTypeType,
     },
 )
@@ -3142,25 +3799,14 @@
     "UpdateAttributesRequestTypeDef",
     {
         "Blacklist": Sequence[str],
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
 ResultRowValueTypeDef = TypedDict(
     "ResultRowValueTypeDef",
     {
         "Key": str,
         "Type": str,
         "Value": str,
     },
@@ -3172,38 +3818,68 @@
         "Enabled": bool,
         "SenderId": str,
         "ShortCode": str,
     },
     total=False,
 )
 
+SegmentConditionOutputTypeDef = TypedDict(
+    "SegmentConditionOutputTypeDef",
+    {
+        "SegmentId": str,
+    },
+)
+
 SegmentConditionTypeDef = TypedDict(
     "SegmentConditionTypeDef",
     {
         "SegmentId": str,
     },
 )
 
+_RequiredSegmentReferenceOutputTypeDef = TypedDict(
+    "_RequiredSegmentReferenceOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalSegmentReferenceOutputTypeDef = TypedDict(
+    "_OptionalSegmentReferenceOutputTypeDef",
+    {
+        "Version": int,
+    },
+    total=False,
+)
+
+
+class SegmentReferenceOutputTypeDef(
+    _RequiredSegmentReferenceOutputTypeDef, _OptionalSegmentReferenceOutputTypeDef
+):
+    pass
+
+
 _RequiredSegmentReferenceTypeDef = TypedDict(
     "_RequiredSegmentReferenceTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalSegmentReferenceTypeDef = TypedDict(
     "_OptionalSegmentReferenceTypeDef",
     {
         "Version": int,
     },
     total=False,
 )
 
+
 class SegmentReferenceTypeDef(_RequiredSegmentReferenceTypeDef, _OptionalSegmentReferenceTypeDef):
     pass
 
+
 _RequiredSegmentImportResourceTypeDef = TypedDict(
     "_RequiredSegmentImportResourceTypeDef",
     {
         "ExternalId": str,
         "Format": FormatType,
         "RoleArn": str,
         "S3Url": str,
@@ -3214,19 +3890,21 @@
     "_OptionalSegmentImportResourceTypeDef",
     {
         "ChannelCounts": Dict[str, int],
     },
     total=False,
 )
 
+
 class SegmentImportResourceTypeDef(
     _RequiredSegmentImportResourceTypeDef, _OptionalSegmentImportResourceTypeDef
 ):
     pass
 
+
 _RequiredSendOTPMessageRequestParametersTypeDef = TypedDict(
     "_RequiredSendOTPMessageRequestParametersTypeDef",
     {
         "BrandName": str,
         "Channel": str,
         "DestinationIdentity": str,
         "OriginationIdentity": str,
@@ -3242,36 +3920,54 @@
         "Language": str,
         "TemplateId": str,
         "ValidityPeriod": int,
     },
     total=False,
 )
 
+
 class SendOTPMessageRequestParametersTypeDef(
     _RequiredSendOTPMessageRequestParametersTypeDef, _OptionalSendOTPMessageRequestParametersTypeDef
 ):
     pass
 
+
 SimpleEmailPartTypeDef = TypedDict(
     "SimpleEmailPartTypeDef",
     {
         "Charset": str,
         "Data": str,
     },
     total=False,
 )
 
+TagsModelTypeDef = TypedDict(
+    "TagsModelTypeDef",
+    {
+        "tags": Mapping[str, str],
+    },
+)
+
 TemplateActiveVersionRequestTypeDef = TypedDict(
     "TemplateActiveVersionRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+TemplateOutputTypeDef = TypedDict(
+    "TemplateOutputTypeDef",
+    {
+        "Name": str,
+        "Version": str,
+    },
+    total=False,
+)
+
 TemplateTypeDef = TypedDict(
     "TemplateTypeDef",
     {
         "Name": str,
         "Version": str,
     },
     total=False,
@@ -3294,17 +3990,19 @@
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
+
 class TemplateResponseTypeDef(_RequiredTemplateResponseTypeDef, _OptionalTemplateResponseTypeDef):
     pass
 
+
 _RequiredTemplateVersionResponseTypeDef = TypedDict(
     "_RequiredTemplateVersionResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": str,
@@ -3316,19 +4014,21 @@
         "DefaultSubstitutions": str,
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
+
 class TemplateVersionResponseTypeDef(
     _RequiredTemplateVersionResponseTypeDef, _OptionalTemplateVersionResponseTypeDef
 ):
     pass
 
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -3350,19 +4050,21 @@
         "RecommendationTransformerUri": str,
         "RecommendationsDisplayName": str,
         "RecommendationsPerMessage": int,
     },
     total=False,
 )
 
+
 class UpdateRecommenderConfigurationTypeDef(
     _RequiredUpdateRecommenderConfigurationTypeDef, _OptionalUpdateRecommenderConfigurationTypeDef
 ):
     pass
 
+
 VoiceChannelRequestTypeDef = TypedDict(
     "VoiceChannelRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -3388,324 +4090,344 @@
     "UpdateAdmChannelRequestRequestTypeDef",
     {
         "ADMChannelRequest": ADMChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
 
-DeleteAdmChannelResponseTypeDef = TypedDict(
-    "DeleteAdmChannelResponseTypeDef",
+UpdateApnsChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsChannelRequestRequestTypeDef",
     {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSChannelRequest": APNSChannelRequestTypeDef,
+        "ApplicationId": str,
     },
 )
 
-GetAdmChannelResponseTypeDef = TypedDict(
-    "GetAdmChannelResponseTypeDef",
+UpdateApnsSandboxChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsSandboxChannelRequestRequestTypeDef",
     {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSSandboxChannelRequest": APNSSandboxChannelRequestTypeDef,
+        "ApplicationId": str,
     },
 )
 
-UpdateAdmChannelResponseTypeDef = TypedDict(
-    "UpdateAdmChannelResponseTypeDef",
+UpdateApnsVoipChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsVoipChannelRequestRequestTypeDef",
     {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSVoipChannelRequest": APNSVoipChannelRequestTypeDef,
+        "ApplicationId": str,
     },
 )
 
-UpdateApnsChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsChannelRequestRequestTypeDef",
+UpdateApnsVoipSandboxChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
     {
-        "APNSChannelRequest": APNSChannelRequestTypeDef,
+        "APNSVoipSandboxChannelRequest": APNSVoipSandboxChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
 
-DeleteApnsChannelResponseTypeDef = TypedDict(
-    "DeleteApnsChannelResponseTypeDef",
+_RequiredActivitiesResponseTypeDef = TypedDict(
+    "_RequiredActivitiesResponseTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Item": List[ActivityResponseTypeDef],
     },
 )
-
-GetApnsChannelResponseTypeDef = TypedDict(
-    "GetApnsChannelResponseTypeDef",
+_OptionalActivitiesResponseTypeDef = TypedDict(
+    "_OptionalActivitiesResponseTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "NextToken": str,
     },
+    total=False,
 )
 
-UpdateApnsChannelResponseTypeDef = TypedDict(
-    "UpdateApnsChannelResponseTypeDef",
+
+class ActivitiesResponseTypeDef(
+    _RequiredActivitiesResponseTypeDef, _OptionalActivitiesResponseTypeDef
+):
+    pass
+
+
+ApplicationsResponseTypeDef = TypedDict(
+    "ApplicationsResponseTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Item": List[ApplicationResponseTypeDef],
+        "NextToken": str,
     },
+    total=False,
 )
 
-UpdateApnsSandboxChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsSandboxChannelRequestRequestTypeDef",
+_RequiredApplicationSettingsResourceTypeDef = TypedDict(
+    "_RequiredApplicationSettingsResourceTypeDef",
     {
-        "APNSSandboxChannelRequest": APNSSandboxChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
-
-DeleteApnsSandboxChannelResponseTypeDef = TypedDict(
-    "DeleteApnsSandboxChannelResponseTypeDef",
+_OptionalApplicationSettingsResourceTypeDef = TypedDict(
+    "_OptionalApplicationSettingsResourceTypeDef",
     {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CampaignHook": CampaignHookOutputTypeDef,
+        "LastModifiedDate": str,
+        "Limits": CampaignLimitsOutputTypeDef,
+        "QuietTime": QuietTimeOutputTypeDef,
     },
+    total=False,
 )
 
-GetApnsSandboxChannelResponseTypeDef = TypedDict(
-    "GetApnsSandboxChannelResponseTypeDef",
-    {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-UpdateApnsSandboxChannelResponseTypeDef = TypedDict(
-    "UpdateApnsSandboxChannelResponseTypeDef",
+class ApplicationSettingsResourceTypeDef(
+    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
+):
+    pass
+
+
+UpdateBaiduChannelRequestRequestTypeDef = TypedDict(
+    "UpdateBaiduChannelRequestRequestTypeDef",
     {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApplicationId": str,
+        "BaiduChannelRequest": BaiduChannelRequestTypeDef,
     },
 )
 
-UpdateApnsVoipChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsVoipChannelRequestRequestTypeDef",
+ChannelsResponseTypeDef = TypedDict(
+    "ChannelsResponseTypeDef",
     {
-        "APNSVoipChannelRequest": APNSVoipChannelRequestTypeDef,
-        "ApplicationId": str,
+        "Channels": Dict[str, ChannelResponseTypeDef],
     },
 )
 
-DeleteApnsVoipChannelResponseTypeDef = TypedDict(
-    "DeleteApnsVoipChannelResponseTypeDef",
+ClosedDaysOutputTypeDef = TypedDict(
+    "ClosedDaysOutputTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EMAIL": List[ClosedDaysRuleOutputTypeDef],
+        "SMS": List[ClosedDaysRuleOutputTypeDef],
+        "PUSH": List[ClosedDaysRuleOutputTypeDef],
+        "VOICE": List[ClosedDaysRuleOutputTypeDef],
+        "CUSTOM": List[ClosedDaysRuleOutputTypeDef],
     },
+    total=False,
 )
 
-GetApnsVoipChannelResponseTypeDef = TypedDict(
-    "GetApnsVoipChannelResponseTypeDef",
+ClosedDaysTypeDef = TypedDict(
+    "ClosedDaysTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EMAIL": Sequence[ClosedDaysRuleTypeDef],
+        "SMS": Sequence[ClosedDaysRuleTypeDef],
+        "PUSH": Sequence[ClosedDaysRuleTypeDef],
+        "VOICE": Sequence[ClosedDaysRuleTypeDef],
+        "CUSTOM": Sequence[ClosedDaysRuleTypeDef],
     },
+    total=False,
 )
 
-UpdateApnsVoipChannelResponseTypeDef = TypedDict(
-    "UpdateApnsVoipChannelResponseTypeDef",
+WaitActivityOutputTypeDef = TypedDict(
+    "WaitActivityOutputTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "NextActivity": str,
+        "WaitTime": WaitTimeOutputTypeDef,
     },
+    total=False,
 )
 
-UpdateApnsVoipSandboxChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
+WaitActivityTypeDef = TypedDict(
+    "WaitActivityTypeDef",
     {
-        "APNSVoipSandboxChannelRequest": APNSVoipSandboxChannelRequestTypeDef,
-        "ApplicationId": str,
+        "NextActivity": str,
+        "WaitTime": WaitTimeTypeDef,
     },
+    total=False,
 )
 
-DeleteApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "DeleteApnsVoipSandboxChannelResponseTypeDef",
+CreateAppRequestRequestTypeDef = TypedDict(
+    "CreateAppRequestRequestTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CreateApplicationRequest": CreateApplicationRequestTypeDef,
     },
 )
 
-GetApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "GetApnsVoipSandboxChannelResponseTypeDef",
+CreateAppResponseTypeDef = TypedDict(
+    "CreateAppResponseTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApplicationResponse": ApplicationResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "UpdateApnsVoipSandboxChannelResponseTypeDef",
+DeleteAdmChannelResponseTypeDef = TypedDict(
+    "DeleteAdmChannelResponseTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredActivitiesResponseTypeDef = TypedDict(
-    "_RequiredActivitiesResponseTypeDef",
+DeleteApnsChannelResponseTypeDef = TypedDict(
+    "DeleteApnsChannelResponseTypeDef",
     {
-        "Item": List[ActivityResponseTypeDef],
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalActivitiesResponseTypeDef = TypedDict(
-    "_OptionalActivitiesResponseTypeDef",
+
+DeleteApnsSandboxChannelResponseTypeDef = TypedDict(
+    "DeleteApnsSandboxChannelResponseTypeDef",
     {
-        "NextToken": str,
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ActivitiesResponseTypeDef(
-    _RequiredActivitiesResponseTypeDef, _OptionalActivitiesResponseTypeDef
-):
-    pass
-
-ApplicationsResponseTypeDef = TypedDict(
-    "ApplicationsResponseTypeDef",
+DeleteApnsVoipChannelResponseTypeDef = TypedDict(
+    "DeleteApnsVoipChannelResponseTypeDef",
     {
-        "Item": List[ApplicationResponseTypeDef],
-        "NextToken": str,
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-CreateAppResponseTypeDef = TypedDict(
-    "CreateAppResponseTypeDef",
+DeleteApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "DeleteApnsVoipSandboxChannelResponseTypeDef",
     {
-        "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAppResponseTypeDef = TypedDict(
     "DeleteAppResponseTypeDef",
     {
         "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetAppResponseTypeDef = TypedDict(
-    "GetAppResponseTypeDef",
+DeleteBaiduChannelResponseTypeDef = TypedDict(
+    "DeleteBaiduChannelResponseTypeDef",
     {
-        "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredApplicationSettingsResourceTypeDef = TypedDict(
-    "_RequiredApplicationSettingsResourceTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "ApplicationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalApplicationSettingsResourceTypeDef = TypedDict(
-    "_OptionalApplicationSettingsResourceTypeDef",
+
+GetAdmChannelResponseTypeDef = TypedDict(
+    "GetAdmChannelResponseTypeDef",
     {
-        "CampaignHook": CampaignHookTypeDef,
-        "LastModifiedDate": str,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ApplicationSettingsResourceTypeDef(
-    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
-):
-    pass
+GetApnsChannelResponseTypeDef = TypedDict(
+    "GetApnsChannelResponseTypeDef",
+    {
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-WriteApplicationSettingsRequestTypeDef = TypedDict(
-    "WriteApplicationSettingsRequestTypeDef",
+GetApnsSandboxChannelResponseTypeDef = TypedDict(
+    "GetApnsSandboxChannelResponseTypeDef",
     {
-        "CampaignHook": CampaignHookTypeDef,
-        "CloudWatchMetricsEnabled": bool,
-        "EventTaggingEnabled": bool,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-RemoveAttributesResponseTypeDef = TypedDict(
-    "RemoveAttributesResponseTypeDef",
+GetApnsVoipChannelResponseTypeDef = TypedDict(
+    "GetApnsVoipChannelResponseTypeDef",
     {
-        "AttributesResource": AttributesResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateBaiduChannelRequestRequestTypeDef = TypedDict(
-    "UpdateBaiduChannelRequestRequestTypeDef",
+GetApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "GetApnsVoipSandboxChannelResponseTypeDef",
     {
-        "ApplicationId": str,
-        "BaiduChannelRequest": BaiduChannelRequestTypeDef,
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteBaiduChannelResponseTypeDef = TypedDict(
-    "DeleteBaiduChannelResponseTypeDef",
+GetAppResponseTypeDef = TypedDict(
+    "GetAppResponseTypeDef",
     {
-        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApplicationResponse": ApplicationResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBaiduChannelResponseTypeDef = TypedDict(
     "GetBaiduChannelResponseTypeDef",
     {
         "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateBaiduChannelResponseTypeDef = TypedDict(
-    "UpdateBaiduChannelResponseTypeDef",
+RemoveAttributesResponseTypeDef = TypedDict(
+    "RemoveAttributesResponseTypeDef",
     {
-        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AttributesResource": AttributesResourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ChannelsResponseTypeDef = TypedDict(
-    "ChannelsResponseTypeDef",
+UpdateAdmChannelResponseTypeDef = TypedDict(
+    "UpdateAdmChannelResponseTypeDef",
     {
-        "Channels": Dict[str, ChannelResponseTypeDef],
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ClosedDaysTypeDef = TypedDict(
-    "ClosedDaysTypeDef",
+UpdateApnsChannelResponseTypeDef = TypedDict(
+    "UpdateApnsChannelResponseTypeDef",
     {
-        "EMAIL": Sequence[ClosedDaysRuleTypeDef],
-        "SMS": Sequence[ClosedDaysRuleTypeDef],
-        "PUSH": Sequence[ClosedDaysRuleTypeDef],
-        "VOICE": Sequence[ClosedDaysRuleTypeDef],
-        "CUSTOM": Sequence[ClosedDaysRuleTypeDef],
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-WaitActivityTypeDef = TypedDict(
-    "WaitActivityTypeDef",
+UpdateApnsSandboxChannelResponseTypeDef = TypedDict(
+    "UpdateApnsSandboxChannelResponseTypeDef",
     {
-        "NextActivity": str,
-        "WaitTime": WaitTimeTypeDef,
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-CreateAppRequestRequestTypeDef = TypedDict(
-    "CreateAppRequestRequestTypeDef",
+UpdateApnsVoipChannelResponseTypeDef = TypedDict(
+    "UpdateApnsVoipChannelResponseTypeDef",
     {
-        "CreateApplicationRequest": CreateApplicationRequestTypeDef,
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "UpdateApnsVoipSandboxChannelResponseTypeDef",
+    {
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBaiduChannelResponseTypeDef = TypedDict(
+    "UpdateBaiduChannelResponseTypeDef",
+    {
+        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEmailTemplateRequestRequestTypeDef = TypedDict(
     "CreateEmailTemplateRequestRequestTypeDef",
     {
         "EmailTemplateRequest": EmailTemplateRequestTypeDef,
@@ -3725,49 +4447,51 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
+
 class UpdateEmailTemplateRequestRequestTypeDef(
     _RequiredUpdateEmailTemplateRequestRequestTypeDef,
     _OptionalUpdateEmailTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 CreateEmailTemplateResponseTypeDef = TypedDict(
     "CreateEmailTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePushTemplateResponseTypeDef = TypedDict(
     "CreatePushTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSmsTemplateResponseTypeDef = TypedDict(
     "CreateSmsTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVoiceTemplateResponseTypeDef = TypedDict(
     "CreateVoiceTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateExportJobRequestRequestTypeDef = TypedDict(
     "CreateExportJobRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -3783,46 +4507,46 @@
     },
 )
 
 CreateInAppTemplateResponseTypeDef = TypedDict(
     "CreateInAppTemplateResponseTypeDef",
     {
         "TemplateCreateMessageBody": TemplateCreateMessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "CreateRecommenderConfigurationRequestRequestTypeDef",
     {
         "CreateRecommenderConfiguration": CreateRecommenderConfigurationTypeDef,
     },
 )
 
 CreateRecommenderConfigurationResponseTypeDef = TypedDict(
     "CreateRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRecommenderConfigurationResponseTypeDef = TypedDict(
     "DeleteRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommenderConfigurationResponseTypeDef = TypedDict(
     "GetRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListRecommenderConfigurationsResponseTypeDef = TypedDict(
     "_RequiredListRecommenderConfigurationsResponseTypeDef",
     {
         "Item": List[RecommenderConfigurationResponseTypeDef],
@@ -3832,25 +4556,27 @@
     "_OptionalListRecommenderConfigurationsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListRecommenderConfigurationsResponseTypeDef(
     _RequiredListRecommenderConfigurationsResponseTypeDef,
     _OptionalListRecommenderConfigurationsResponseTypeDef,
 ):
     pass
 
+
 UpdateRecommenderConfigurationResponseTypeDef = TypedDict(
     "UpdateRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSmsTemplateRequestRequestTypeDef = TypedDict(
     "CreateSmsTemplateRequestRequestTypeDef",
     {
         "SMSTemplateRequest": SMSTemplateRequestTypeDef,
@@ -3870,19 +4596,21 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
+
 class UpdateSmsTemplateRequestRequestTypeDef(
     _RequiredUpdateSmsTemplateRequestRequestTypeDef, _OptionalUpdateSmsTemplateRequestRequestTypeDef
 ):
     pass
 
+
 CreateVoiceTemplateRequestRequestTypeDef = TypedDict(
     "CreateVoiceTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "VoiceTemplateRequest": VoiceTemplateRequestTypeDef,
     },
 )
@@ -3899,45 +4627,44 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
+
 class UpdateVoiceTemplateRequestRequestTypeDef(
     _RequiredUpdateVoiceTemplateRequestRequestTypeDef,
     _OptionalUpdateVoiceTemplateRequestRequestTypeDef,
 ):
     pass
 
-CustomMessageActivityTypeDef = TypedDict(
-    "CustomMessageActivityTypeDef",
+
+CustomMessageActivityOutputTypeDef = TypedDict(
+    "CustomMessageActivityOutputTypeDef",
     {
         "DeliveryUri": str,
-        "EndpointTypes": Sequence[EndpointTypesElementType],
-        "MessageConfig": JourneyCustomMessageTypeDef,
+        "EndpointTypes": List[EndpointTypesElementType],
+        "MessageConfig": JourneyCustomMessageOutputTypeDef,
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
     },
     total=False,
 )
 
-PushNotificationTemplateRequestTypeDef = TypedDict(
-    "PushNotificationTemplateRequestTypeDef",
+CustomMessageActivityTypeDef = TypedDict(
+    "CustomMessageActivityTypeDef",
     {
-        "ADM": AndroidPushNotificationTemplateTypeDef,
-        "APNS": APNSPushNotificationTemplateTypeDef,
-        "Baidu": AndroidPushNotificationTemplateTypeDef,
-        "Default": DefaultPushNotificationTemplateTypeDef,
-        "DefaultSubstitutions": str,
-        "GCM": AndroidPushNotificationTemplateTypeDef,
-        "RecommenderId": str,
-        "tags": Mapping[str, str],
-        "TemplateDescription": str,
+        "DeliveryUri": str,
+        "EndpointTypes": Sequence[EndpointTypesElementType],
+        "MessageConfig": JourneyCustomMessageTypeDef,
+        "NextActivity": str,
+        "TemplateName": str,
+        "TemplateVersion": str,
     },
     total=False,
 )
 
 _RequiredPushNotificationTemplateResponseTypeDef = TypedDict(
     "_RequiredPushNotificationTemplateResponseTypeDef",
     {
@@ -3946,267 +4673,296 @@
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
     },
 )
 _OptionalPushNotificationTemplateResponseTypeDef = TypedDict(
     "_OptionalPushNotificationTemplateResponseTypeDef",
     {
-        "ADM": AndroidPushNotificationTemplateTypeDef,
-        "APNS": APNSPushNotificationTemplateTypeDef,
+        "ADM": AndroidPushNotificationTemplateOutputTypeDef,
+        "APNS": APNSPushNotificationTemplateOutputTypeDef,
         "Arn": str,
-        "Baidu": AndroidPushNotificationTemplateTypeDef,
-        "Default": DefaultPushNotificationTemplateTypeDef,
+        "Baidu": AndroidPushNotificationTemplateOutputTypeDef,
+        "Default": DefaultPushNotificationTemplateOutputTypeDef,
         "DefaultSubstitutions": str,
-        "GCM": AndroidPushNotificationTemplateTypeDef,
+        "GCM": AndroidPushNotificationTemplateOutputTypeDef,
         "RecommenderId": str,
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
+
 class PushNotificationTemplateResponseTypeDef(
     _RequiredPushNotificationTemplateResponseTypeDef,
     _OptionalPushNotificationTemplateResponseTypeDef,
 ):
     pass
 
+
+PushNotificationTemplateRequestTypeDef = TypedDict(
+    "PushNotificationTemplateRequestTypeDef",
+    {
+        "ADM": AndroidPushNotificationTemplateTypeDef,
+        "APNS": APNSPushNotificationTemplateTypeDef,
+        "Baidu": AndroidPushNotificationTemplateTypeDef,
+        "Default": DefaultPushNotificationTemplateTypeDef,
+        "DefaultSubstitutions": str,
+        "GCM": AndroidPushNotificationTemplateTypeDef,
+        "RecommenderId": str,
+        "tags": Mapping[str, str],
+        "TemplateDescription": str,
+    },
+    total=False,
+)
+
 DeleteEmailChannelResponseTypeDef = TypedDict(
     "DeleteEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEmailChannelResponseTypeDef = TypedDict(
     "GetEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEmailChannelResponseTypeDef = TypedDict(
     "UpdateEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEmailTemplateResponseTypeDef = TypedDict(
     "DeleteEmailTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInAppTemplateResponseTypeDef = TypedDict(
     "DeleteInAppTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePushTemplateResponseTypeDef = TypedDict(
     "DeletePushTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSmsTemplateResponseTypeDef = TypedDict(
     "DeleteSmsTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVoiceTemplateResponseTypeDef = TypedDict(
     "DeleteVoiceTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEmailTemplateResponseTypeDef = TypedDict(
     "UpdateEmailTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEndpointResponseTypeDef = TypedDict(
     "UpdateEndpointResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEndpointsBatchResponseTypeDef = TypedDict(
     "UpdateEndpointsBatchResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateInAppTemplateResponseTypeDef = TypedDict(
     "UpdateInAppTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePushTemplateResponseTypeDef = TypedDict(
     "UpdatePushTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSmsTemplateResponseTypeDef = TypedDict(
     "UpdateSmsTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTemplateActiveVersionResponseTypeDef = TypedDict(
     "UpdateTemplateActiveVersionResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVoiceTemplateResponseTypeDef = TypedDict(
     "UpdateVoiceTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEventStreamResponseTypeDef = TypedDict(
     "DeleteEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEventStreamResponseTypeDef = TypedDict(
     "GetEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutEventStreamResponseTypeDef = TypedDict(
     "PutEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteGcmChannelResponseTypeDef = TypedDict(
     "DeleteGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGcmChannelResponseTypeDef = TypedDict(
     "GetGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGcmChannelResponseTypeDef = TypedDict(
     "UpdateGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSmsChannelResponseTypeDef = TypedDict(
     "DeleteSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSmsChannelResponseTypeDef = TypedDict(
     "GetSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSmsChannelResponseTypeDef = TypedDict(
     "UpdateSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVoiceChannelResponseTypeDef = TypedDict(
     "DeleteVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceChannelResponseTypeDef = TypedDict(
     "GetVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVoiceChannelResponseTypeDef = TypedDict(
     "UpdateVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEmailChannelRequestRequestTypeDef = TypedDict(
     "UpdateEmailChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EmailChannelRequest": EmailChannelRequestTypeDef,
     },
 )
 
+EmailMessageActivityOutputTypeDef = TypedDict(
+    "EmailMessageActivityOutputTypeDef",
+    {
+        "MessageConfig": JourneyEmailMessageOutputTypeDef,
+        "NextActivity": str,
+        "TemplateName": str,
+        "TemplateVersion": str,
+    },
+    total=False,
+)
+
 EmailMessageActivityTypeDef = TypedDict(
     "EmailMessageActivityTypeDef",
     {
         "MessageConfig": JourneyEmailMessageTypeDef,
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
@@ -4214,15 +4970,15 @@
     total=False,
 )
 
 GetEmailTemplateResponseTypeDef = TypedDict(
     "GetEmailTemplateResponseTypeDef",
     {
         "EmailTemplateResponse": EmailTemplateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointBatchItemTypeDef = TypedDict(
     "EndpointBatchItemTypeDef",
     {
         "Address": str,
@@ -4255,36 +5011,14 @@
         "OptOut": str,
         "RequestId": str,
         "User": EndpointUserTypeDef,
     },
     total=False,
 )
 
-EndpointResponseTypeDef = TypedDict(
-    "EndpointResponseTypeDef",
-    {
-        "Address": str,
-        "ApplicationId": str,
-        "Attributes": Dict[str, List[str]],
-        "ChannelType": ChannelTypeType,
-        "CohortId": str,
-        "CreationDate": str,
-        "Demographic": EndpointDemographicTypeDef,
-        "EffectiveDate": str,
-        "EndpointStatus": str,
-        "Id": str,
-        "Location": EndpointLocationTypeDef,
-        "Metrics": Dict[str, float],
-        "OptOut": str,
-        "RequestId": str,
-        "User": EndpointUserTypeDef,
-    },
-    total=False,
-)
-
 PublicEndpointTypeDef = TypedDict(
     "PublicEndpointTypeDef",
     {
         "Address": str,
         "Attributes": Mapping[str, Sequence[str]],
         "ChannelType": ChannelTypeType,
         "Demographic": EndpointDemographicTypeDef,
@@ -4310,19 +5044,66 @@
     {
         "RequestId": str,
         "Result": Dict[str, Dict[str, EndpointMessageResultTypeDef]],
     },
     total=False,
 )
 
+
 class SendUsersMessageResponseTypeDef(
     _RequiredSendUsersMessageResponseTypeDef, _OptionalSendUsersMessageResponseTypeDef
 ):
     pass
 
+
+EndpointResponseTypeDef = TypedDict(
+    "EndpointResponseTypeDef",
+    {
+        "Address": str,
+        "ApplicationId": str,
+        "Attributes": Dict[str, List[str]],
+        "ChannelType": ChannelTypeType,
+        "CohortId": str,
+        "CreationDate": str,
+        "Demographic": EndpointDemographicOutputTypeDef,
+        "EffectiveDate": str,
+        "EndpointStatus": str,
+        "Id": str,
+        "Location": EndpointLocationOutputTypeDef,
+        "Metrics": Dict[str, float],
+        "OptOut": str,
+        "RequestId": str,
+        "User": EndpointUserOutputTypeDef,
+    },
+    total=False,
+)
+
+EventDimensionsOutputTypeDef = TypedDict(
+    "EventDimensionsOutputTypeDef",
+    {
+        "Attributes": Dict[str, AttributeDimensionOutputTypeDef],
+        "EventType": SetDimensionOutputTypeDef,
+        "Metrics": Dict[str, MetricDimensionOutputTypeDef],
+    },
+    total=False,
+)
+
+SegmentDemographicsOutputTypeDef = TypedDict(
+    "SegmentDemographicsOutputTypeDef",
+    {
+        "AppVersion": SetDimensionOutputTypeDef,
+        "Channel": SetDimensionOutputTypeDef,
+        "DeviceType": SetDimensionOutputTypeDef,
+        "Make": SetDimensionOutputTypeDef,
+        "Model": SetDimensionOutputTypeDef,
+        "Platform": SetDimensionOutputTypeDef,
+    },
+    total=False,
+)
+
 EventDimensionsTypeDef = TypedDict(
     "EventDimensionsTypeDef",
     {
         "Attributes": Mapping[str, AttributeDimensionTypeDef],
         "EventType": SetDimensionTypeDef,
         "Metrics": Mapping[str, MetricDimensionTypeDef],
     },
@@ -4369,17 +5150,19 @@
         "Metrics": Mapping[str, float],
         "SdkName": str,
         "Session": SessionTypeDef,
     },
     total=False,
 )
 
+
 class EventTypeDef(_RequiredEventTypeDef, _OptionalEventTypeDef):
     pass
 
+
 _RequiredExportJobResponseTypeDef = TypedDict(
     "_RequiredExportJobResponseTypeDef",
     {
         "ApplicationId": str,
         "CreationDate": str,
         "Definition": ExportJobResourceTypeDef,
         "Id": str,
@@ -4397,93 +5180,118 @@
         "TotalFailures": int,
         "TotalPieces": int,
         "TotalProcessed": int,
     },
     total=False,
 )
 
+
 class ExportJobResponseTypeDef(
     _RequiredExportJobResponseTypeDef, _OptionalExportJobResponseTypeDef
 ):
     pass
 
+
 UpdateGcmChannelRequestRequestTypeDef = TypedDict(
     "UpdateGcmChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "GCMChannelRequest": GCMChannelRequestTypeDef,
     },
 )
 
+_RequiredGPSPointDimensionOutputTypeDef = TypedDict(
+    "_RequiredGPSPointDimensionOutputTypeDef",
+    {
+        "Coordinates": GPSCoordinatesOutputTypeDef,
+    },
+)
+_OptionalGPSPointDimensionOutputTypeDef = TypedDict(
+    "_OptionalGPSPointDimensionOutputTypeDef",
+    {
+        "RangeInKilometers": float,
+    },
+    total=False,
+)
+
+
+class GPSPointDimensionOutputTypeDef(
+    _RequiredGPSPointDimensionOutputTypeDef, _OptionalGPSPointDimensionOutputTypeDef
+):
+    pass
+
+
 _RequiredGPSPointDimensionTypeDef = TypedDict(
     "_RequiredGPSPointDimensionTypeDef",
     {
         "Coordinates": GPSCoordinatesTypeDef,
     },
 )
 _OptionalGPSPointDimensionTypeDef = TypedDict(
     "_OptionalGPSPointDimensionTypeDef",
     {
         "RangeInKilometers": float,
     },
     total=False,
 )
 
+
 class GPSPointDimensionTypeDef(
     _RequiredGPSPointDimensionTypeDef, _OptionalGPSPointDimensionTypeDef
 ):
     pass
 
+
 GetJourneyExecutionActivityMetricsResponseTypeDef = TypedDict(
     "GetJourneyExecutionActivityMetricsResponseTypeDef",
     {
         "JourneyExecutionActivityMetricsResponse": JourneyExecutionActivityMetricsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJourneyExecutionMetricsResponseTypeDef = TypedDict(
     "GetJourneyExecutionMetricsResponseTypeDef",
     {
         "JourneyExecutionMetricsResponse": JourneyExecutionMetricsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJourneyRunExecutionActivityMetricsResponseTypeDef = TypedDict(
     "GetJourneyRunExecutionActivityMetricsResponseTypeDef",
     {
         "JourneyRunExecutionActivityMetricsResponse": (
             JourneyRunExecutionActivityMetricsResponseTypeDef
         ),
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJourneyRunExecutionMetricsResponseTypeDef = TypedDict(
     "GetJourneyRunExecutionMetricsResponseTypeDef",
     {
         "JourneyRunExecutionMetricsResponse": JourneyRunExecutionMetricsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSmsTemplateResponseTypeDef = TypedDict(
     "GetSmsTemplateResponseTypeDef",
     {
         "SMSTemplateResponse": SMSTemplateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceTemplateResponseTypeDef = TypedDict(
     "GetVoiceTemplateResponseTypeDef",
     {
         "VoiceTemplateResponse": VoiceTemplateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportJobResponseTypeDef = TypedDict(
     "_RequiredImportJobResponseTypeDef",
     {
         "ApplicationId": str,
@@ -4504,30 +5312,54 @@
         "TotalFailures": int,
         "TotalPieces": int,
         "TotalProcessed": int,
     },
     total=False,
 )
 
+
 class ImportJobResponseTypeDef(
     _RequiredImportJobResponseTypeDef, _OptionalImportJobResponseTypeDef
 ):
     pass
 
+
+InAppMessageButtonOutputTypeDef = TypedDict(
+    "InAppMessageButtonOutputTypeDef",
+    {
+        "Android": OverrideButtonConfigurationOutputTypeDef,
+        "DefaultConfig": DefaultButtonConfigurationOutputTypeDef,
+        "IOS": OverrideButtonConfigurationOutputTypeDef,
+        "Web": OverrideButtonConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 InAppMessageButtonTypeDef = TypedDict(
     "InAppMessageButtonTypeDef",
     {
         "Android": OverrideButtonConfigurationTypeDef,
         "DefaultConfig": DefaultButtonConfigurationTypeDef,
         "IOS": OverrideButtonConfigurationTypeDef,
         "Web": OverrideButtonConfigurationTypeDef,
     },
     total=False,
 )
 
+PushMessageActivityOutputTypeDef = TypedDict(
+    "PushMessageActivityOutputTypeDef",
+    {
+        "MessageConfig": JourneyPushMessageOutputTypeDef,
+        "NextActivity": str,
+        "TemplateName": str,
+        "TemplateVersion": str,
+    },
+    total=False,
+)
+
 PushMessageActivityTypeDef = TypedDict(
     "PushMessageActivityTypeDef",
     {
         "MessageConfig": JourneyPushMessageTypeDef,
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
@@ -4545,19 +5377,32 @@
     "_OptionalJourneyRunsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class JourneyRunsResponseTypeDef(
     _RequiredJourneyRunsResponseTypeDef, _OptionalJourneyRunsResponseTypeDef
 ):
     pass
 
+
+SMSMessageActivityOutputTypeDef = TypedDict(
+    "SMSMessageActivityOutputTypeDef",
+    {
+        "MessageConfig": JourneySMSMessageOutputTypeDef,
+        "NextActivity": str,
+        "TemplateName": str,
+        "TemplateVersion": str,
+    },
+    total=False,
+)
+
 SMSMessageActivityTypeDef = TypedDict(
     "SMSMessageActivityTypeDef",
     {
         "MessageConfig": JourneySMSMessageTypeDef,
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
@@ -4573,24 +5418,16 @@
         "JourneyStateRequest": JourneyStateRequestTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "TagsModel": TagsModelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "TagsModel": TagsModelTypeDef,
+        "TagsModel": TagsModelOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMessageResponseTypeDef = TypedDict(
     "_RequiredMessageResponseTypeDef",
     {
         "ApplicationId": str,
@@ -4602,30 +5439,44 @@
         "EndpointResult": Dict[str, EndpointMessageResultTypeDef],
         "RequestId": str,
         "Result": Dict[str, MessageResultTypeDef],
     },
     total=False,
 )
 
+
 class MessageResponseTypeDef(_RequiredMessageResponseTypeDef, _OptionalMessageResponseTypeDef):
     pass
 
+
 PhoneNumberValidateRequestRequestTypeDef = TypedDict(
     "PhoneNumberValidateRequestRequestTypeDef",
     {
         "NumberValidateRequest": NumberValidateRequestTypeDef,
     },
 )
 
 PhoneNumberValidateResponseTypeDef = TypedDict(
     "PhoneNumberValidateResponseTypeDef",
     {
         "NumberValidateResponse": NumberValidateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+OpenHoursOutputTypeDef = TypedDict(
+    "OpenHoursOutputTypeDef",
+    {
+        "EMAIL": Dict[DayOfWeekType, List[OpenHoursRuleOutputTypeDef]],
+        "SMS": Dict[DayOfWeekType, List[OpenHoursRuleOutputTypeDef]],
+        "PUSH": Dict[DayOfWeekType, List[OpenHoursRuleOutputTypeDef]],
+        "VOICE": Dict[DayOfWeekType, List[OpenHoursRuleOutputTypeDef]],
+        "CUSTOM": Dict[DayOfWeekType, List[OpenHoursRuleOutputTypeDef]],
     },
+    total=False,
 )
 
 OpenHoursTypeDef = TypedDict(
     "OpenHoursTypeDef",
     {
         "EMAIL": Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]],
         "SMS": Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]],
@@ -4640,22 +5491,50 @@
     "PutEventStreamRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "WriteEventStream": WriteEventStreamTypeDef,
     },
 )
 
+WriteApplicationSettingsRequestTypeDef = TypedDict(
+    "WriteApplicationSettingsRequestTypeDef",
+    {
+        "CampaignHook": CampaignHookTypeDef,
+        "CloudWatchMetricsEnabled": bool,
+        "EventTaggingEnabled": bool,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
+    },
+    total=False,
+)
+
+RandomSplitActivityOutputTypeDef = TypedDict(
+    "RandomSplitActivityOutputTypeDef",
+    {
+        "Branches": List[RandomSplitEntryOutputTypeDef],
+    },
+    total=False,
+)
+
 RandomSplitActivityTypeDef = TypedDict(
     "RandomSplitActivityTypeDef",
     {
         "Branches": Sequence[RandomSplitEntryTypeDef],
     },
     total=False,
 )
 
+SegmentBehaviorsOutputTypeDef = TypedDict(
+    "SegmentBehaviorsOutputTypeDef",
+    {
+        "Recency": RecencyDimensionOutputTypeDef,
+    },
+    total=False,
+)
+
 SegmentBehaviorsTypeDef = TypedDict(
     "SegmentBehaviorsTypeDef",
     {
         "Recency": RecencyDimensionTypeDef,
     },
     total=False,
 )
@@ -4699,23 +5578,42 @@
         "HtmlPart": SimpleEmailPartTypeDef,
         "Subject": SimpleEmailPartTypeDef,
         "TextPart": SimpleEmailPartTypeDef,
     },
     total=False,
 )
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagsModel": TagsModelTypeDef,
+    },
+)
+
 UpdateTemplateActiveVersionRequestRequestTypeDef = TypedDict(
     "UpdateTemplateActiveVersionRequestRequestTypeDef",
     {
         "TemplateActiveVersionRequest": TemplateActiveVersionRequestTypeDef,
         "TemplateName": str,
         "TemplateType": str,
     },
 )
 
+TemplateConfigurationOutputTypeDef = TypedDict(
+    "TemplateConfigurationOutputTypeDef",
+    {
+        "EmailTemplate": TemplateOutputTypeDef,
+        "PushTemplate": TemplateOutputTypeDef,
+        "SMSTemplate": TemplateOutputTypeDef,
+        "VoiceTemplate": TemplateOutputTypeDef,
+    },
+    total=False,
+)
+
 TemplateConfigurationTypeDef = TypedDict(
     "TemplateConfigurationTypeDef",
     {
         "EmailTemplate": TemplateTypeDef,
         "PushTemplate": TemplateTypeDef,
         "SMSTemplate": TemplateTypeDef,
         "VoiceTemplate": TemplateTypeDef,
@@ -4733,19 +5631,21 @@
     "_OptionalTemplatesResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class TemplatesResponseTypeDef(
     _RequiredTemplatesResponseTypeDef, _OptionalTemplatesResponseTypeDef
 ):
     pass
 
+
 _RequiredTemplateVersionsResponseTypeDef = TypedDict(
     "_RequiredTemplateVersionsResponseTypeDef",
     {
         "Item": List[TemplateVersionResponseTypeDef],
     },
 )
 _OptionalTemplateVersionsResponseTypeDef = TypedDict(
@@ -4754,19 +5654,21 @@
         "Message": str,
         "NextToken": str,
         "RequestID": str,
     },
     total=False,
 )
 
+
 class TemplateVersionsResponseTypeDef(
     _RequiredTemplateVersionsResponseTypeDef, _OptionalTemplateVersionsResponseTypeDef
 ):
     pass
 
+
 UpdateRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateRecommenderConfigurationRequestRequestTypeDef",
     {
         "RecommenderId": str,
         "UpdateRecommenderConfiguration": UpdateRecommenderConfigurationTypeDef,
     },
 )
@@ -4779,15 +5681,15 @@
     },
 )
 
 VerifyOTPMessageResponseTypeDef = TypedDict(
     "VerifyOTPMessageResponseTypeDef",
     {
         "VerificationResponse": VerificationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VerifyOTPMessageRequestRequestTypeDef = TypedDict(
     "VerifyOTPMessageRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -4795,63 +5697,63 @@
     },
 )
 
 GetCampaignActivitiesResponseTypeDef = TypedDict(
     "GetCampaignActivitiesResponseTypeDef",
     {
         "ActivitiesResponse": ActivitiesResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAppsResponseTypeDef = TypedDict(
     "GetAppsResponseTypeDef",
     {
         "ApplicationsResponse": ApplicationsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApplicationSettingsResponseTypeDef = TypedDict(
     "GetApplicationSettingsResponseTypeDef",
     {
         "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationSettingsResponseTypeDef = TypedDict(
     "UpdateApplicationSettingsResponseTypeDef",
     {
         "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateApplicationSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateApplicationSettingsRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "WriteApplicationSettingsRequest": WriteApplicationSettingsRequestTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChannelsResponseTypeDef = TypedDict(
     "GetChannelsResponseTypeDef",
     {
         "ChannelsResponse": ChannelsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommenderConfigurationsResponseTypeDef = TypedDict(
     "GetRecommenderConfigurationsResponseTypeDef",
     {
         "ListRecommenderConfigurationsResponse": ListRecommenderConfigurationsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPushTemplateResponseTypeDef = TypedDict(
+    "GetPushTemplateResponseTypeDef",
+    {
+        "PushNotificationTemplateResponse": PushNotificationTemplateResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePushTemplateRequestRequestTypeDef = TypedDict(
     "CreatePushTemplateRequestRequestTypeDef",
     {
         "PushNotificationTemplateRequest": PushNotificationTemplateRequestTypeDef,
@@ -4871,27 +5773,21 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
+
 class UpdatePushTemplateRequestRequestTypeDef(
     _RequiredUpdatePushTemplateRequestRequestTypeDef,
     _OptionalUpdatePushTemplateRequestRequestTypeDef,
 ):
     pass
 
-GetPushTemplateResponseTypeDef = TypedDict(
-    "GetPushTemplateResponseTypeDef",
-    {
-        "PushNotificationTemplateResponse": PushNotificationTemplateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 EndpointBatchRequestTypeDef = TypedDict(
     "EndpointBatchRequestTypeDef",
     {
         "Item": Sequence[EndpointBatchItemTypeDef],
     },
 )
@@ -4901,42 +5797,67 @@
     {
         "ApplicationId": str,
         "EndpointId": str,
         "EndpointRequest": EndpointRequestTypeDef,
     },
 )
 
+SendUsersMessagesResponseTypeDef = TypedDict(
+    "SendUsersMessagesResponseTypeDef",
+    {
+        "SendUsersMessageResponse": SendUsersMessageResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeleteEndpointResponseTypeDef = TypedDict(
     "DeleteEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointsResponseTypeDef = TypedDict(
     "EndpointsResponseTypeDef",
     {
         "Item": List[EndpointResponseTypeDef],
     },
 )
 
 GetEndpointResponseTypeDef = TypedDict(
     "GetEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SendUsersMessagesResponseTypeDef = TypedDict(
-    "SendUsersMessagesResponseTypeDef",
+CampaignEventFilterOutputTypeDef = TypedDict(
+    "CampaignEventFilterOutputTypeDef",
     {
-        "SendUsersMessageResponse": SendUsersMessageResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Dimensions": EventDimensionsOutputTypeDef,
+        "FilterType": FilterTypeType,
+    },
+)
+
+EventConditionOutputTypeDef = TypedDict(
+    "EventConditionOutputTypeDef",
+    {
+        "Dimensions": EventDimensionsOutputTypeDef,
+        "MessageActivity": str,
+    },
+    total=False,
+)
+
+EventFilterOutputTypeDef = TypedDict(
+    "EventFilterOutputTypeDef",
+    {
+        "Dimensions": EventDimensionsOutputTypeDef,
+        "FilterType": FilterTypeType,
     },
 )
 
 CampaignEventFilterTypeDef = TypedDict(
     "CampaignEventFilterTypeDef",
     {
         "Dimensions": EventDimensionsTypeDef,
@@ -4977,15 +5898,15 @@
     },
 )
 
 CreateExportJobResponseTypeDef = TypedDict(
     "CreateExportJobResponseTypeDef",
     {
         "ExportJobResponse": ExportJobResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredExportJobsResponseTypeDef = TypedDict(
     "_RequiredExportJobsResponseTypeDef",
     {
         "Item": List[ExportJobResponseTypeDef],
@@ -4995,49 +5916,60 @@
     "_OptionalExportJobsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ExportJobsResponseTypeDef(
     _RequiredExportJobsResponseTypeDef, _OptionalExportJobsResponseTypeDef
 ):
     pass
 
+
 GetExportJobResponseTypeDef = TypedDict(
     "GetExportJobResponseTypeDef",
     {
         "ExportJobResponse": ExportJobResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SegmentLocationOutputTypeDef = TypedDict(
+    "SegmentLocationOutputTypeDef",
+    {
+        "Country": SetDimensionOutputTypeDef,
+        "GPSPoint": GPSPointDimensionOutputTypeDef,
+    },
+    total=False,
+)
+
 SegmentLocationTypeDef = TypedDict(
     "SegmentLocationTypeDef",
     {
         "Country": SetDimensionTypeDef,
         "GPSPoint": GPSPointDimensionTypeDef,
     },
     total=False,
 )
 
 CreateImportJobResponseTypeDef = TypedDict(
     "CreateImportJobResponseTypeDef",
     {
         "ImportJobResponse": ImportJobResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetImportJobResponseTypeDef = TypedDict(
     "GetImportJobResponseTypeDef",
     {
         "ImportJobResponse": ImportJobResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportJobsResponseTypeDef = TypedDict(
     "_RequiredImportJobsResponseTypeDef",
     {
         "Item": List[ImportJobResponseTypeDef],
@@ -5047,19 +5979,34 @@
     "_OptionalImportJobsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ImportJobsResponseTypeDef(
     _RequiredImportJobsResponseTypeDef, _OptionalImportJobsResponseTypeDef
 ):
     pass
 
+
+InAppMessageContentOutputTypeDef = TypedDict(
+    "InAppMessageContentOutputTypeDef",
+    {
+        "BackgroundColor": str,
+        "BodyConfig": InAppMessageBodyConfigOutputTypeDef,
+        "HeaderConfig": InAppMessageHeaderConfigOutputTypeDef,
+        "ImageUrl": str,
+        "PrimaryBtn": InAppMessageButtonOutputTypeDef,
+        "SecondaryBtn": InAppMessageButtonOutputTypeDef,
+    },
+    total=False,
+)
+
 InAppMessageContentTypeDef = TypedDict(
     "InAppMessageContentTypeDef",
     {
         "BackgroundColor": str,
         "BodyConfig": InAppMessageBodyConfigTypeDef,
         "HeaderConfig": InAppMessageHeaderConfigTypeDef,
         "ImageUrl": str,
@@ -5069,31 +6016,39 @@
     total=False,
 )
 
 GetJourneyRunsResponseTypeDef = TypedDict(
     "GetJourneyRunsResponseTypeDef",
     {
         "JourneyRunsResponse": JourneyRunsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendMessagesResponseTypeDef = TypedDict(
     "SendMessagesResponseTypeDef",
     {
         "MessageResponse": MessageResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendOTPMessageResponseTypeDef = TypedDict(
     "SendOTPMessageResponseTypeDef",
     {
         "MessageResponse": MessageResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApplicationSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateApplicationSettingsRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "WriteApplicationSettingsRequest": WriteApplicationSettingsRequestTypeDef,
     },
 )
 
 BaseKpiResultTypeDef = TypedDict(
     "BaseKpiResultTypeDef",
     {
         "Rows": List[ResultRowTypeDef],
@@ -5114,23 +6069,23 @@
     total=False,
 )
 
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "TemplatesResponse": TemplatesResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTemplateVersionsResponseTypeDef = TypedDict(
     "ListTemplateVersionsResponseTypeDef",
     {
         "TemplateVersionsResponse": TemplateVersionsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEndpointsBatchRequestRequestTypeDef = TypedDict(
     "UpdateEndpointsBatchRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -5138,32 +6093,65 @@
     },
 )
 
 DeleteUserEndpointsResponseTypeDef = TypedDict(
     "DeleteUserEndpointsResponseTypeDef",
     {
         "EndpointsResponse": EndpointsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserEndpointsResponseTypeDef = TypedDict(
     "GetUserEndpointsResponseTypeDef",
     {
         "EndpointsResponse": EndpointsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InAppCampaignScheduleTypeDef = TypedDict(
     "InAppCampaignScheduleTypeDef",
     {
         "EndDate": str,
-        "EventFilter": CampaignEventFilterTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "EventFilter": CampaignEventFilterOutputTypeDef,
+        "QuietTime": QuietTimeOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredScheduleOutputTypeDef = TypedDict(
+    "_RequiredScheduleOutputTypeDef",
+    {
+        "StartTime": str,
+    },
+)
+_OptionalScheduleOutputTypeDef = TypedDict(
+    "_OptionalScheduleOutputTypeDef",
+    {
+        "EndTime": str,
+        "EventFilter": CampaignEventFilterOutputTypeDef,
+        "Frequency": FrequencyType,
+        "IsLocalTime": bool,
+        "QuietTime": QuietTimeOutputTypeDef,
+        "Timezone": str,
+    },
+    total=False,
+)
+
+
+class ScheduleOutputTypeDef(_RequiredScheduleOutputTypeDef, _OptionalScheduleOutputTypeDef):
+    pass
+
+
+EventStartConditionOutputTypeDef = TypedDict(
+    "EventStartConditionOutputTypeDef",
+    {
+        "EventFilter": EventFilterOutputTypeDef,
+        "SegmentId": str,
     },
     total=False,
 )
 
 _RequiredScheduleTypeDef = TypedDict(
     "_RequiredScheduleTypeDef",
     {
@@ -5179,57 +6167,72 @@
         "IsLocalTime": bool,
         "QuietTime": QuietTimeTypeDef,
         "Timezone": str,
     },
     total=False,
 )
 
+
 class ScheduleTypeDef(_RequiredScheduleTypeDef, _OptionalScheduleTypeDef):
     pass
 
+
 EventStartConditionTypeDef = TypedDict(
     "EventStartConditionTypeDef",
     {
         "EventFilter": EventFilterTypeDef,
         "SegmentId": str,
     },
     total=False,
 )
 
 PutEventsResponseTypeDef = TypedDict(
     "PutEventsResponseTypeDef",
     {
         "EventsResponse": EventsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventsRequestTypeDef = TypedDict(
     "EventsRequestTypeDef",
     {
         "BatchItem": Mapping[str, EventsBatchTypeDef],
     },
 )
 
 GetExportJobsResponseTypeDef = TypedDict(
     "GetExportJobsResponseTypeDef",
     {
         "ExportJobsResponse": ExportJobsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentExportJobsResponseTypeDef = TypedDict(
     "GetSegmentExportJobsResponseTypeDef",
     {
         "ExportJobsResponse": ExportJobsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SegmentDimensionsOutputTypeDef = TypedDict(
+    "SegmentDimensionsOutputTypeDef",
+    {
+        "Attributes": Dict[str, AttributeDimensionOutputTypeDef],
+        "Behavior": SegmentBehaviorsOutputTypeDef,
+        "Demographic": SegmentDemographicsOutputTypeDef,
+        "Location": SegmentLocationOutputTypeDef,
+        "Metrics": Dict[str, MetricDimensionOutputTypeDef],
+        "UserAttributes": Dict[str, AttributeDimensionOutputTypeDef],
+    },
+    total=False,
+)
+
 SegmentDimensionsTypeDef = TypedDict(
     "SegmentDimensionsTypeDef",
     {
         "Attributes": Mapping[str, AttributeDimensionTypeDef],
         "Behavior": SegmentBehaviorsTypeDef,
         "Demographic": SegmentDemographicsTypeDef,
         "Location": SegmentLocationTypeDef,
@@ -5239,87 +6242,100 @@
     total=False,
 )
 
 GetImportJobsResponseTypeDef = TypedDict(
     "GetImportJobsResponseTypeDef",
     {
         "ImportJobsResponse": ImportJobsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentImportJobsResponseTypeDef = TypedDict(
     "GetSegmentImportJobsResponseTypeDef",
     {
         "ImportJobsResponse": ImportJobsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CampaignInAppMessageTypeDef = TypedDict(
-    "CampaignInAppMessageTypeDef",
+CampaignInAppMessageOutputTypeDef = TypedDict(
+    "CampaignInAppMessageOutputTypeDef",
     {
         "Body": str,
-        "Content": Sequence[InAppMessageContentTypeDef],
-        "CustomConfig": Mapping[str, str],
+        "Content": List[InAppMessageContentOutputTypeDef],
+        "CustomConfig": Dict[str, str],
         "Layout": LayoutType,
     },
     total=False,
 )
 
 InAppMessageTypeDef = TypedDict(
     "InAppMessageTypeDef",
     {
-        "Content": List[InAppMessageContentTypeDef],
+        "Content": List[InAppMessageContentOutputTypeDef],
         "CustomConfig": Dict[str, str],
         "Layout": LayoutType,
     },
     total=False,
 )
 
-InAppTemplateRequestTypeDef = TypedDict(
-    "InAppTemplateRequestTypeDef",
-    {
-        "Content": Sequence[InAppMessageContentTypeDef],
-        "CustomConfig": Mapping[str, str],
-        "Layout": LayoutType,
-        "tags": Mapping[str, str],
-        "TemplateDescription": str,
-    },
-    total=False,
-)
-
 _RequiredInAppTemplateResponseTypeDef = TypedDict(
     "_RequiredInAppTemplateResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
     },
 )
 _OptionalInAppTemplateResponseTypeDef = TypedDict(
     "_OptionalInAppTemplateResponseTypeDef",
     {
         "Arn": str,
-        "Content": List[InAppMessageContentTypeDef],
+        "Content": List[InAppMessageContentOutputTypeDef],
         "CustomConfig": Dict[str, str],
         "Layout": LayoutType,
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
+
 class InAppTemplateResponseTypeDef(
     _RequiredInAppTemplateResponseTypeDef, _OptionalInAppTemplateResponseTypeDef
 ):
     pass
 
+
+CampaignInAppMessageTypeDef = TypedDict(
+    "CampaignInAppMessageTypeDef",
+    {
+        "Body": str,
+        "Content": Sequence[InAppMessageContentTypeDef],
+        "CustomConfig": Mapping[str, str],
+        "Layout": LayoutType,
+    },
+    total=False,
+)
+
+InAppTemplateRequestTypeDef = TypedDict(
+    "InAppTemplateRequestTypeDef",
+    {
+        "Content": Sequence[InAppMessageContentTypeDef],
+        "CustomConfig": Mapping[str, str],
+        "Layout": LayoutType,
+        "tags": Mapping[str, str],
+        "TemplateDescription": str,
+    },
+    total=False,
+)
+
 _RequiredApplicationDateRangeKpiResponseTypeDef = TypedDict(
     "_RequiredApplicationDateRangeKpiResponseTypeDef",
     {
         "ApplicationId": str,
         "EndTime": datetime,
         "KpiName": str,
         "KpiResult": BaseKpiResultTypeDef,
@@ -5330,19 +6346,21 @@
     "_OptionalApplicationDateRangeKpiResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ApplicationDateRangeKpiResponseTypeDef(
     _RequiredApplicationDateRangeKpiResponseTypeDef, _OptionalApplicationDateRangeKpiResponseTypeDef
 ):
     pass
 
+
 _RequiredCampaignDateRangeKpiResponseTypeDef = TypedDict(
     "_RequiredCampaignDateRangeKpiResponseTypeDef",
     {
         "ApplicationId": str,
         "CampaignId": str,
         "EndTime": datetime,
         "KpiName": str,
@@ -5354,19 +6372,21 @@
     "_OptionalCampaignDateRangeKpiResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class CampaignDateRangeKpiResponseTypeDef(
     _RequiredCampaignDateRangeKpiResponseTypeDef, _OptionalCampaignDateRangeKpiResponseTypeDef
 ):
     pass
 
+
 _RequiredJourneyDateRangeKpiResponseTypeDef = TypedDict(
     "_RequiredJourneyDateRangeKpiResponseTypeDef",
     {
         "ApplicationId": str,
         "EndTime": datetime,
         "JourneyId": str,
         "KpiName": str,
@@ -5378,19 +6398,21 @@
     "_OptionalJourneyDateRangeKpiResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class JourneyDateRangeKpiResponseTypeDef(
     _RequiredJourneyDateRangeKpiResponseTypeDef, _OptionalJourneyDateRangeKpiResponseTypeDef
 ):
     pass
 
+
 DirectMessageConfigurationTypeDef = TypedDict(
     "DirectMessageConfigurationTypeDef",
     {
         "ADMMessage": ADMMessageTypeDef,
         "APNSMessage": APNSMessageTypeDef,
         "BaiduMessage": BaiduMessageTypeDef,
         "DefaultMessage": DefaultMessageTypeDef,
@@ -5399,14 +6421,24 @@
         "GCMMessage": GCMMessageTypeDef,
         "SMSMessage": SMSMessageTypeDef,
         "VoiceMessage": VoiceMessageTypeDef,
     },
     total=False,
 )
 
+StartConditionOutputTypeDef = TypedDict(
+    "StartConditionOutputTypeDef",
+    {
+        "Description": str,
+        "EventStartCondition": EventStartConditionOutputTypeDef,
+        "SegmentStartCondition": SegmentConditionOutputTypeDef,
+    },
+    total=False,
+)
+
 StartConditionTypeDef = TypedDict(
     "StartConditionTypeDef",
     {
         "Description": str,
         "EventStartCondition": EventStartConditionTypeDef,
         "SegmentStartCondition": SegmentConditionTypeDef,
     },
@@ -5417,14 +6449,35 @@
     "PutEventsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EventsRequest": EventsRequestTypeDef,
     },
 )
 
+SegmentGroupOutputTypeDef = TypedDict(
+    "SegmentGroupOutputTypeDef",
+    {
+        "Dimensions": List[SegmentDimensionsOutputTypeDef],
+        "SourceSegments": List[SegmentReferenceOutputTypeDef],
+        "SourceType": SourceTypeType,
+        "Type": TypeType,
+    },
+    total=False,
+)
+
+SimpleConditionOutputTypeDef = TypedDict(
+    "SimpleConditionOutputTypeDef",
+    {
+        "EventCondition": EventConditionOutputTypeDef,
+        "SegmentCondition": SegmentConditionOutputTypeDef,
+        "SegmentDimensions": SegmentDimensionsOutputTypeDef,
+    },
+    total=False,
+)
+
 SegmentGroupTypeDef = TypedDict(
     "SegmentGroupTypeDef",
     {
         "Dimensions": Sequence[SegmentDimensionsTypeDef],
         "SourceSegments": Sequence[SegmentReferenceTypeDef],
         "SourceType": SourceTypeType,
         "Type": TypeType,
@@ -5438,26 +6491,26 @@
         "EventCondition": EventConditionTypeDef,
         "SegmentCondition": SegmentConditionTypeDef,
         "SegmentDimensions": SegmentDimensionsTypeDef,
     },
     total=False,
 )
 
-MessageConfigurationTypeDef = TypedDict(
-    "MessageConfigurationTypeDef",
+MessageConfigurationOutputTypeDef = TypedDict(
+    "MessageConfigurationOutputTypeDef",
     {
-        "ADMMessage": MessageTypeDef,
-        "APNSMessage": MessageTypeDef,
-        "BaiduMessage": MessageTypeDef,
-        "CustomMessage": CampaignCustomMessageTypeDef,
-        "DefaultMessage": MessageTypeDef,
-        "EmailMessage": CampaignEmailMessageTypeDef,
-        "GCMMessage": MessageTypeDef,
-        "SMSMessage": CampaignSmsMessageTypeDef,
-        "InAppMessage": CampaignInAppMessageTypeDef,
+        "ADMMessage": MessageOutputTypeDef,
+        "APNSMessage": MessageOutputTypeDef,
+        "BaiduMessage": MessageOutputTypeDef,
+        "CustomMessage": CampaignCustomMessageOutputTypeDef,
+        "DefaultMessage": MessageOutputTypeDef,
+        "EmailMessage": CampaignEmailMessageOutputTypeDef,
+        "GCMMessage": MessageOutputTypeDef,
+        "SMSMessage": CampaignSmsMessageOutputTypeDef,
+        "InAppMessage": CampaignInAppMessageOutputTypeDef,
     },
     total=False,
 )
 
 InAppMessageCampaignTypeDef = TypedDict(
     "InAppMessageCampaignTypeDef",
     {
@@ -5469,14 +6522,38 @@
         "SessionCap": int,
         "TotalCap": int,
         "TreatmentId": str,
     },
     total=False,
 )
 
+GetInAppTemplateResponseTypeDef = TypedDict(
+    "GetInAppTemplateResponseTypeDef",
+    {
+        "InAppTemplateResponse": InAppTemplateResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MessageConfigurationTypeDef = TypedDict(
+    "MessageConfigurationTypeDef",
+    {
+        "ADMMessage": MessageTypeDef,
+        "APNSMessage": MessageTypeDef,
+        "BaiduMessage": MessageTypeDef,
+        "CustomMessage": CampaignCustomMessageTypeDef,
+        "DefaultMessage": MessageTypeDef,
+        "EmailMessage": CampaignEmailMessageTypeDef,
+        "GCMMessage": MessageTypeDef,
+        "SMSMessage": CampaignSmsMessageTypeDef,
+        "InAppMessage": CampaignInAppMessageTypeDef,
+    },
+    total=False,
+)
+
 CreateInAppTemplateRequestRequestTypeDef = TypedDict(
     "CreateInAppTemplateRequestRequestTypeDef",
     {
         "InAppTemplateRequest": InAppTemplateRequestTypeDef,
         "TemplateName": str,
     },
 )
@@ -5493,49 +6570,43 @@
     {
         "CreateNewVersion": bool,
         "Version": str,
     },
     total=False,
 )
 
+
 class UpdateInAppTemplateRequestRequestTypeDef(
     _RequiredUpdateInAppTemplateRequestRequestTypeDef,
     _OptionalUpdateInAppTemplateRequestRequestTypeDef,
 ):
     pass
 
-GetInAppTemplateResponseTypeDef = TypedDict(
-    "GetInAppTemplateResponseTypeDef",
-    {
-        "InAppTemplateResponse": InAppTemplateResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetApplicationDateRangeKpiResponseTypeDef = TypedDict(
     "GetApplicationDateRangeKpiResponseTypeDef",
     {
         "ApplicationDateRangeKpiResponse": ApplicationDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCampaignDateRangeKpiResponseTypeDef = TypedDict(
     "GetCampaignDateRangeKpiResponseTypeDef",
     {
         "CampaignDateRangeKpiResponse": CampaignDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJourneyDateRangeKpiResponseTypeDef = TypedDict(
     "GetJourneyDateRangeKpiResponseTypeDef",
     {
         "JourneyDateRangeKpiResponse": JourneyDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMessageRequestTypeDef = TypedDict(
     "_RequiredMessageRequestTypeDef",
     {
         "MessageConfiguration": DirectMessageConfigurationTypeDef,
@@ -5549,17 +6620,19 @@
         "Endpoints": Mapping[str, EndpointSendConfigurationTypeDef],
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TraceId": str,
     },
     total=False,
 )
 
+
 class MessageRequestTypeDef(_RequiredMessageRequestTypeDef, _OptionalMessageRequestTypeDef):
     pass
 
+
 _RequiredSendUsersMessageRequestTypeDef = TypedDict(
     "_RequiredSendUsersMessageRequestTypeDef",
     {
         "MessageConfiguration": DirectMessageConfigurationTypeDef,
         "Users": Mapping[str, EndpointSendConfigurationTypeDef],
     },
 )
@@ -5569,19 +6642,48 @@
         "Context": Mapping[str, str],
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TraceId": str,
     },
     total=False,
 )
 
+
 class SendUsersMessageRequestTypeDef(
     _RequiredSendUsersMessageRequestTypeDef, _OptionalSendUsersMessageRequestTypeDef
 ):
     pass
 
+
+SegmentGroupListOutputTypeDef = TypedDict(
+    "SegmentGroupListOutputTypeDef",
+    {
+        "Groups": List[SegmentGroupOutputTypeDef],
+        "Include": IncludeType,
+    },
+    total=False,
+)
+
+ConditionOutputTypeDef = TypedDict(
+    "ConditionOutputTypeDef",
+    {
+        "Conditions": List[SimpleConditionOutputTypeDef],
+        "Operator": OperatorType,
+    },
+    total=False,
+)
+
+MultiConditionalBranchOutputTypeDef = TypedDict(
+    "MultiConditionalBranchOutputTypeDef",
+    {
+        "Condition": SimpleConditionOutputTypeDef,
+        "NextActivity": str,
+    },
+    total=False,
+)
+
 SegmentGroupListTypeDef = TypedDict(
     "SegmentGroupListTypeDef",
     {
         "Groups": Sequence[SegmentGroupTypeDef],
         "Include": IncludeType,
     },
     total=False,
@@ -5611,30 +6713,40 @@
         "Id": str,
         "SizePercent": int,
     },
 )
 _OptionalTreatmentResourceTypeDef = TypedDict(
     "_OptionalTreatmentResourceTypeDef",
     {
-        "CustomDeliveryConfiguration": CustomDeliveryConfigurationTypeDef,
-        "MessageConfiguration": MessageConfigurationTypeDef,
-        "Schedule": ScheduleTypeDef,
+        "CustomDeliveryConfiguration": CustomDeliveryConfigurationOutputTypeDef,
+        "MessageConfiguration": MessageConfigurationOutputTypeDef,
+        "Schedule": ScheduleOutputTypeDef,
         "State": CampaignStateTypeDef,
-        "TemplateConfiguration": TemplateConfigurationTypeDef,
+        "TemplateConfiguration": TemplateConfigurationOutputTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
     },
     total=False,
 )
 
+
 class TreatmentResourceTypeDef(
     _RequiredTreatmentResourceTypeDef, _OptionalTreatmentResourceTypeDef
 ):
     pass
 
+
+InAppMessagesResponseTypeDef = TypedDict(
+    "InAppMessagesResponseTypeDef",
+    {
+        "InAppMessageCampaigns": List[InAppMessageCampaignTypeDef],
+    },
+    total=False,
+)
+
 _RequiredWriteTreatmentResourceTypeDef = TypedDict(
     "_RequiredWriteTreatmentResourceTypeDef",
     {
         "SizePercent": int,
     },
 )
 _OptionalWriteTreatmentResourceTypeDef = TypedDict(
@@ -5646,26 +6758,20 @@
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
     },
     total=False,
 )
 
+
 class WriteTreatmentResourceTypeDef(
     _RequiredWriteTreatmentResourceTypeDef, _OptionalWriteTreatmentResourceTypeDef
 ):
     pass
 
-InAppMessagesResponseTypeDef = TypedDict(
-    "InAppMessagesResponseTypeDef",
-    {
-        "InAppMessageCampaigns": List[InAppMessageCampaignTypeDef],
-    },
-    total=False,
-)
 
 SendMessagesRequestRequestTypeDef = TypedDict(
     "SendMessagesRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "MessageRequest": MessageRequestTypeDef,
     },
@@ -5688,28 +6794,51 @@
         "Id": str,
         "SegmentType": SegmentTypeType,
     },
 )
 _OptionalSegmentResponseTypeDef = TypedDict(
     "_OptionalSegmentResponseTypeDef",
     {
-        "Dimensions": SegmentDimensionsTypeDef,
+        "Dimensions": SegmentDimensionsOutputTypeDef,
         "ImportDefinition": SegmentImportResourceTypeDef,
         "LastModifiedDate": str,
         "Name": str,
-        "SegmentGroups": SegmentGroupListTypeDef,
+        "SegmentGroups": SegmentGroupListOutputTypeDef,
         "tags": Dict[str, str],
         "Version": int,
     },
     total=False,
 )
 
+
 class SegmentResponseTypeDef(_RequiredSegmentResponseTypeDef, _OptionalSegmentResponseTypeDef):
     pass
 
+
+ConditionalSplitActivityOutputTypeDef = TypedDict(
+    "ConditionalSplitActivityOutputTypeDef",
+    {
+        "Condition": ConditionOutputTypeDef,
+        "EvaluationWaitTime": WaitTimeOutputTypeDef,
+        "FalseActivity": str,
+        "TrueActivity": str,
+    },
+    total=False,
+)
+
+MultiConditionalSplitActivityOutputTypeDef = TypedDict(
+    "MultiConditionalSplitActivityOutputTypeDef",
+    {
+        "Branches": List[MultiConditionalBranchOutputTypeDef],
+        "DefaultActivity": str,
+        "EvaluationWaitTime": WaitTimeOutputTypeDef,
+    },
+    total=False,
+)
+
 WriteSegmentRequestTypeDef = TypedDict(
     "WriteSegmentRequestTypeDef",
     {
         "Dimensions": SegmentDimensionsTypeDef,
         "Name": str,
         "SegmentGroups": SegmentGroupListTypeDef,
         "tags": Mapping[str, str],
@@ -5750,38 +6879,48 @@
         "SegmentVersion": int,
     },
 )
 _OptionalCampaignResponseTypeDef = TypedDict(
     "_OptionalCampaignResponseTypeDef",
     {
         "AdditionalTreatments": List[TreatmentResourceTypeDef],
-        "CustomDeliveryConfiguration": CustomDeliveryConfigurationTypeDef,
+        "CustomDeliveryConfiguration": CustomDeliveryConfigurationOutputTypeDef,
         "DefaultState": CampaignStateTypeDef,
         "Description": str,
         "HoldoutPercent": int,
-        "Hook": CampaignHookTypeDef,
+        "Hook": CampaignHookOutputTypeDef,
         "IsPaused": bool,
-        "Limits": CampaignLimitsTypeDef,
-        "MessageConfiguration": MessageConfigurationTypeDef,
+        "Limits": CampaignLimitsOutputTypeDef,
+        "MessageConfiguration": MessageConfigurationOutputTypeDef,
         "Name": str,
-        "Schedule": ScheduleTypeDef,
+        "Schedule": ScheduleOutputTypeDef,
         "State": CampaignStateTypeDef,
         "tags": Dict[str, str],
-        "TemplateConfiguration": TemplateConfigurationTypeDef,
+        "TemplateConfiguration": TemplateConfigurationOutputTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
         "Version": int,
         "Priority": int,
     },
     total=False,
 )
 
+
 class CampaignResponseTypeDef(_RequiredCampaignResponseTypeDef, _OptionalCampaignResponseTypeDef):
     pass
 
+
+GetInAppMessagesResponseTypeDef = TypedDict(
+    "GetInAppMessagesResponseTypeDef",
+    {
+        "InAppMessagesResponse": InAppMessagesResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 WriteCampaignRequestTypeDef = TypedDict(
     "WriteCampaignRequestTypeDef",
     {
         "AdditionalTreatments": Sequence[WriteTreatmentResourceTypeDef],
         "CustomDeliveryConfiguration": CustomDeliveryConfigurationTypeDef,
         "Description": str,
         "HoldoutPercent": int,
@@ -5798,51 +6937,43 @@
         "TreatmentDescription": str,
         "TreatmentName": str,
         "Priority": int,
     },
     total=False,
 )
 
-GetInAppMessagesResponseTypeDef = TypedDict(
-    "GetInAppMessagesResponseTypeDef",
-    {
-        "InAppMessagesResponse": InAppMessagesResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateSegmentResponseTypeDef = TypedDict(
     "CreateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSegmentResponseTypeDef = TypedDict(
     "DeleteSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentResponseTypeDef = TypedDict(
     "GetSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentVersionResponseTypeDef = TypedDict(
     "GetSegmentVersionResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSegmentsResponseTypeDef = TypedDict(
     "_RequiredSegmentsResponseTypeDef",
     {
         "Item": List[SegmentResponseTypeDef],
@@ -5852,23 +6983,43 @@
     "_OptionalSegmentsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class SegmentsResponseTypeDef(_RequiredSegmentsResponseTypeDef, _OptionalSegmentsResponseTypeDef):
     pass
 
+
 UpdateSegmentResponseTypeDef = TypedDict(
     "UpdateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ActivityOutputTypeDef = TypedDict(
+    "ActivityOutputTypeDef",
+    {
+        "CUSTOM": CustomMessageActivityOutputTypeDef,
+        "ConditionalSplit": ConditionalSplitActivityOutputTypeDef,
+        "Description": str,
+        "EMAIL": EmailMessageActivityOutputTypeDef,
+        "Holdout": HoldoutActivityOutputTypeDef,
+        "MultiCondition": MultiConditionalSplitActivityOutputTypeDef,
+        "PUSH": PushMessageActivityOutputTypeDef,
+        "RandomSplit": RandomSplitActivityOutputTypeDef,
+        "SMS": SMSMessageActivityOutputTypeDef,
+        "Wait": WaitActivityOutputTypeDef,
+        "ContactCenter": ContactCenterActivityOutputTypeDef,
     },
+    total=False,
 )
 
 CreateSegmentRequestRequestTypeDef = TypedDict(
     "CreateSegmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "WriteSegmentRequest": WriteSegmentRequestTypeDef,
@@ -5912,56 +7063,58 @@
     "_OptionalCampaignsResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class CampaignsResponseTypeDef(
     _RequiredCampaignsResponseTypeDef, _OptionalCampaignsResponseTypeDef
 ):
     pass
 
+
 CreateCampaignResponseTypeDef = TypedDict(
     "CreateCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCampaignResponseTypeDef = TypedDict(
     "DeleteCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCampaignResponseTypeDef = TypedDict(
     "GetCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCampaignVersionResponseTypeDef = TypedDict(
     "GetCampaignVersionResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCampaignResponseTypeDef = TypedDict(
     "UpdateCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCampaignRequestRequestTypeDef = TypedDict(
     "CreateCampaignRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -5978,63 +7131,65 @@
     },
 )
 
 GetSegmentVersionsResponseTypeDef = TypedDict(
     "GetSegmentVersionsResponseTypeDef",
     {
         "SegmentsResponse": SegmentsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentsResponseTypeDef = TypedDict(
     "GetSegmentsResponseTypeDef",
     {
         "SegmentsResponse": SegmentsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJourneyResponseTypeDef = TypedDict(
     "_RequiredJourneyResponseTypeDef",
     {
         "ApplicationId": str,
         "Id": str,
         "Name": str,
     },
 )
 _OptionalJourneyResponseTypeDef = TypedDict(
     "_OptionalJourneyResponseTypeDef",
     {
-        "Activities": Dict[str, ActivityTypeDef],
+        "Activities": Dict[str, ActivityOutputTypeDef],
         "CreationDate": str,
         "LastModifiedDate": str,
-        "Limits": JourneyLimitsTypeDef,
+        "Limits": JourneyLimitsOutputTypeDef,
         "LocalTime": bool,
-        "QuietTime": QuietTimeTypeDef,
+        "QuietTime": QuietTimeOutputTypeDef,
         "RefreshFrequency": str,
-        "Schedule": JourneyScheduleTypeDef,
+        "Schedule": JourneyScheduleOutputTypeDef,
         "StartActivity": str,
-        "StartCondition": StartConditionTypeDef,
+        "StartCondition": StartConditionOutputTypeDef,
         "State": StateType,
         "tags": Dict[str, str],
         "WaitForQuietTime": bool,
         "RefreshOnSegmentUpdate": bool,
-        "JourneyChannelSettings": JourneyChannelSettingsTypeDef,
+        "JourneyChannelSettings": JourneyChannelSettingsOutputTypeDef,
         "SendingSchedule": bool,
-        "OpenHours": OpenHoursTypeDef,
-        "ClosedDays": ClosedDaysTypeDef,
+        "OpenHours": OpenHoursOutputTypeDef,
+        "ClosedDays": ClosedDaysOutputTypeDef,
         "TimezoneEstimationMethods": List[TimezoneEstimationMethodsElementType],
     },
     total=False,
 )
 
+
 class JourneyResponseTypeDef(_RequiredJourneyResponseTypeDef, _OptionalJourneyResponseTypeDef):
     pass
 
+
 _RequiredWriteJourneyRequestTypeDef = TypedDict(
     "_RequiredWriteJourneyRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalWriteJourneyRequestTypeDef = TypedDict(
@@ -6058,56 +7213,58 @@
         "OpenHours": OpenHoursTypeDef,
         "ClosedDays": ClosedDaysTypeDef,
         "TimezoneEstimationMethods": Sequence[TimezoneEstimationMethodsElementType],
     },
     total=False,
 )
 
+
 class WriteJourneyRequestTypeDef(
     _RequiredWriteJourneyRequestTypeDef, _OptionalWriteJourneyRequestTypeDef
 ):
     pass
 
+
 GetCampaignVersionsResponseTypeDef = TypedDict(
     "GetCampaignVersionsResponseTypeDef",
     {
         "CampaignsResponse": CampaignsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCampaignsResponseTypeDef = TypedDict(
     "GetCampaignsResponseTypeDef",
     {
         "CampaignsResponse": CampaignsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateJourneyResponseTypeDef = TypedDict(
     "CreateJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteJourneyResponseTypeDef = TypedDict(
     "DeleteJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJourneyResponseTypeDef = TypedDict(
     "GetJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJourneysResponseTypeDef = TypedDict(
     "_RequiredJourneysResponseTypeDef",
     {
         "Item": List[JourneyResponseTypeDef],
@@ -6117,30 +7274,32 @@
     "_OptionalJourneysResponseTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class JourneysResponseTypeDef(_RequiredJourneysResponseTypeDef, _OptionalJourneysResponseTypeDef):
     pass
 
+
 UpdateJourneyResponseTypeDef = TypedDict(
     "UpdateJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateJourneyStateResponseTypeDef = TypedDict(
     "UpdateJourneyStateResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateJourneyRequestRequestTypeDef = TypedDict(
     "CreateJourneyRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -6157,10 +7316,10 @@
     },
 )
 
 ListJourneysResponseTypeDef = TypedDict(
     "ListJourneysResponseTypeDef",
     {
         "JourneysResponse": JourneysResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint.egg-info/PKG-INFO` & `mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint
-Version: 1.28.0
-Summary: Type annotations for boto3.Pinpoint 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Pinpoint 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-pinpoint"></a>
 
 # mypy-boto3-pinpoint
 
 [![PyPI - mypy-boto3-pinpoint](https://img.shields.io/pypi/v/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint)](https://pepy.tech/project/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
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
 [mypy-boto3-pinpoint docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,57 +329,74 @@
 from mypy_boto3_pinpoint.type_defs import (
     ADMChannelRequestTypeDef,
     ADMChannelResponseTypeDef,
     ADMMessageTypeDef,
     APNSChannelRequestTypeDef,
     APNSChannelResponseTypeDef,
     APNSMessageTypeDef,
+    APNSPushNotificationTemplateOutputTypeDef,
     APNSPushNotificationTemplateTypeDef,
     APNSSandboxChannelRequestTypeDef,
     APNSSandboxChannelResponseTypeDef,
     APNSVoipChannelRequestTypeDef,
     APNSVoipChannelResponseTypeDef,
     APNSVoipSandboxChannelRequestTypeDef,
     APNSVoipSandboxChannelResponseTypeDef,
     ActivityResponseTypeDef,
+    ContactCenterActivityOutputTypeDef,
+    HoldoutActivityOutputTypeDef,
     ContactCenterActivityTypeDef,
     HoldoutActivityTypeDef,
     AddressConfigurationTypeDef,
+    AndroidPushNotificationTemplateOutputTypeDef,
     AndroidPushNotificationTemplateTypeDef,
     ApplicationResponseTypeDef,
-    CampaignHookTypeDef,
-    CampaignLimitsTypeDef,
-    QuietTimeTypeDef,
+    CampaignHookOutputTypeDef,
+    CampaignLimitsOutputTypeDef,
+    QuietTimeOutputTypeDef,
+    AttributeDimensionOutputTypeDef,
     AttributeDimensionTypeDef,
     AttributesResourceTypeDef,
     BaiduChannelRequestTypeDef,
     BaiduChannelResponseTypeDef,
     BaiduMessageTypeDef,
+    CampaignCustomMessageOutputTypeDef,
     CampaignCustomMessageTypeDef,
+    CampaignEmailMessageOutputTypeDef,
     CampaignEmailMessageTypeDef,
+    CampaignHookTypeDef,
+    CampaignLimitsTypeDef,
     CampaignStateTypeDef,
-    CustomDeliveryConfigurationTypeDef,
+    CustomDeliveryConfigurationOutputTypeDef,
+    CampaignSmsMessageOutputTypeDef,
     CampaignSmsMessageTypeDef,
     ChannelResponseTypeDef,
+    ClosedDaysRuleOutputTypeDef,
     ClosedDaysRuleTypeDef,
+    WaitTimeOutputTypeDef,
     WaitTimeTypeDef,
     CreateApplicationRequestTypeDef,
+    ResponseMetadataTypeDef,
     EmailTemplateRequestTypeDef,
     CreateTemplateMessageBodyTypeDef,
     ExportJobRequestTypeDef,
     ImportJobRequestTypeDef,
     TemplateCreateMessageBodyTypeDef,
     CreateRecommenderConfigurationTypeDef,
     RecommenderConfigurationResponseTypeDef,
     SMSTemplateRequestTypeDef,
     VoiceTemplateRequestTypeDef,
+    CustomDeliveryConfigurationTypeDef,
+    JourneyCustomMessageOutputTypeDef,
     JourneyCustomMessageTypeDef,
+    DefaultButtonConfigurationOutputTypeDef,
     DefaultButtonConfigurationTypeDef,
     DefaultMessageTypeDef,
     DefaultPushNotificationMessageTypeDef,
+    DefaultPushNotificationTemplateOutputTypeDef,
     DefaultPushNotificationTemplateTypeDef,
     DeleteAdmChannelRequestRequestTypeDef,
     DeleteApnsChannelRequestRequestTypeDef,
     DeleteApnsSandboxChannelRequestRequestTypeDef,
     DeleteApnsVoipChannelRequestRequestTypeDef,
     DeleteApnsVoipSandboxChannelRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
@@ -406,30 +423,36 @@
     DeleteVoiceChannelRequestRequestTypeDef,
     VoiceChannelResponseTypeDef,
     DeleteVoiceTemplateRequestRequestTypeDef,
     GCMMessageTypeDef,
     SMSMessageTypeDef,
     VoiceMessageTypeDef,
     EmailChannelRequestTypeDef,
+    JourneyEmailMessageOutputTypeDef,
     JourneyEmailMessageTypeDef,
     RawEmailTypeDef,
     EmailTemplateResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     EndpointDemographicTypeDef,
     EndpointLocationTypeDef,
     EndpointUserTypeDef,
+    EndpointDemographicOutputTypeDef,
     EndpointItemResponseTypeDef,
+    EndpointLocationOutputTypeDef,
     EndpointMessageResultTypeDef,
+    EndpointUserOutputTypeDef,
     EndpointSendConfigurationTypeDef,
+    MetricDimensionOutputTypeDef,
+    SetDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     SetDimensionTypeDef,
     EventItemResponseTypeDef,
     SessionTypeDef,
     ExportJobResourceTypeDef,
     GCMChannelRequestTypeDef,
+    GPSCoordinatesOutputTypeDef,
     GPSCoordinatesTypeDef,
     GetAdmChannelRequestRequestTypeDef,
     GetApnsChannelRequestRequestTypeDef,
     GetApnsSandboxChannelRequestRequestTypeDef,
     GetApnsVoipChannelRequestRequestTypeDef,
     GetApnsVoipSandboxChannelRequestRequestTypeDef,
     GetAppRequestRequestTypeDef,
@@ -479,91 +502,109 @@
     GetSmsTemplateRequestRequestTypeDef,
     SMSTemplateResponseTypeDef,
     GetUserEndpointsRequestRequestTypeDef,
     GetVoiceChannelRequestRequestTypeDef,
     GetVoiceTemplateRequestRequestTypeDef,
     VoiceTemplateResponseTypeDef,
     ImportJobResourceTypeDef,
+    InAppMessageBodyConfigOutputTypeDef,
     InAppMessageBodyConfigTypeDef,
+    OverrideButtonConfigurationOutputTypeDef,
     OverrideButtonConfigurationTypeDef,
+    InAppMessageHeaderConfigOutputTypeDef,
     InAppMessageHeaderConfigTypeDef,
+    JourneyChannelSettingsOutputTypeDef,
     JourneyChannelSettingsTypeDef,
+    JourneyLimitsOutputTypeDef,
     JourneyLimitsTypeDef,
+    JourneyPushMessageOutputTypeDef,
     JourneyPushMessageTypeDef,
-    JourneyScheduleTypeDef,
+    JourneyScheduleOutputTypeDef,
     JourneyRunResponseTypeDef,
+    JourneySMSMessageOutputTypeDef,
     JourneySMSMessageTypeDef,
+    JourneyScheduleTypeDef,
     JourneyStateRequestTypeDef,
     ListJourneysRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagsModelTypeDef,
+    TagsModelOutputTypeDef,
     ListTemplateVersionsRequestRequestTypeDef,
     ListTemplatesRequestRequestTypeDef,
+    MessageOutputTypeDef,
     MessageTypeDef,
     MessageResultTypeDef,
     NumberValidateRequestTypeDef,
     NumberValidateResponseTypeDef,
+    OpenHoursRuleOutputTypeDef,
     OpenHoursRuleTypeDef,
     WriteEventStreamTypeDef,
+    QuietTimeTypeDef,
+    RandomSplitEntryOutputTypeDef,
     RandomSplitEntryTypeDef,
+    RecencyDimensionOutputTypeDef,
     RecencyDimensionTypeDef,
     UpdateAttributesRequestTypeDef,
-    ResponseMetadataTypeDef,
     ResultRowValueTypeDef,
     SMSChannelRequestTypeDef,
+    SegmentConditionOutputTypeDef,
     SegmentConditionTypeDef,
+    SegmentReferenceOutputTypeDef,
     SegmentReferenceTypeDef,
     SegmentImportResourceTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SimpleEmailPartTypeDef,
+    TagsModelTypeDef,
     TemplateActiveVersionRequestTypeDef,
+    TemplateOutputTypeDef,
     TemplateTypeDef,
     TemplateResponseTypeDef,
     TemplateVersionResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRecommenderConfigurationTypeDef,
     VoiceChannelRequestTypeDef,
     VerificationResponseTypeDef,
     VerifyOTPMessageRequestParametersTypeDef,
     UpdateAdmChannelRequestRequestTypeDef,
-    DeleteAdmChannelResponseTypeDef,
-    GetAdmChannelResponseTypeDef,
-    UpdateAdmChannelResponseTypeDef,
     UpdateApnsChannelRequestRequestTypeDef,
-    DeleteApnsChannelResponseTypeDef,
-    GetApnsChannelResponseTypeDef,
-    UpdateApnsChannelResponseTypeDef,
     UpdateApnsSandboxChannelRequestRequestTypeDef,
-    DeleteApnsSandboxChannelResponseTypeDef,
-    GetApnsSandboxChannelResponseTypeDef,
-    UpdateApnsSandboxChannelResponseTypeDef,
     UpdateApnsVoipChannelRequestRequestTypeDef,
-    DeleteApnsVoipChannelResponseTypeDef,
-    GetApnsVoipChannelResponseTypeDef,
-    UpdateApnsVoipChannelResponseTypeDef,
     UpdateApnsVoipSandboxChannelRequestRequestTypeDef,
-    DeleteApnsVoipSandboxChannelResponseTypeDef,
-    GetApnsVoipSandboxChannelResponseTypeDef,
-    UpdateApnsVoipSandboxChannelResponseTypeDef,
     ActivitiesResponseTypeDef,
     ApplicationsResponseTypeDef,
-    CreateAppResponseTypeDef,
-    DeleteAppResponseTypeDef,
-    GetAppResponseTypeDef,
     ApplicationSettingsResourceTypeDef,
-    WriteApplicationSettingsRequestTypeDef,
-    RemoveAttributesResponseTypeDef,
     UpdateBaiduChannelRequestRequestTypeDef,
-    DeleteBaiduChannelResponseTypeDef,
-    GetBaiduChannelResponseTypeDef,
-    UpdateBaiduChannelResponseTypeDef,
     ChannelsResponseTypeDef,
+    ClosedDaysOutputTypeDef,
     ClosedDaysTypeDef,
+    WaitActivityOutputTypeDef,
     WaitActivityTypeDef,
     CreateAppRequestRequestTypeDef,
+    CreateAppResponseTypeDef,
+    DeleteAdmChannelResponseTypeDef,
+    DeleteApnsChannelResponseTypeDef,
+    DeleteApnsSandboxChannelResponseTypeDef,
+    DeleteApnsVoipChannelResponseTypeDef,
+    DeleteApnsVoipSandboxChannelResponseTypeDef,
+    DeleteAppResponseTypeDef,
+    DeleteBaiduChannelResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAdmChannelResponseTypeDef,
+    GetApnsChannelResponseTypeDef,
+    GetApnsSandboxChannelResponseTypeDef,
+    GetApnsVoipChannelResponseTypeDef,
+    GetApnsVoipSandboxChannelResponseTypeDef,
+    GetAppResponseTypeDef,
+    GetBaiduChannelResponseTypeDef,
+    RemoveAttributesResponseTypeDef,
+    UpdateAdmChannelResponseTypeDef,
+    UpdateApnsChannelResponseTypeDef,
+    UpdateApnsSandboxChannelResponseTypeDef,
+    UpdateApnsVoipChannelResponseTypeDef,
+    UpdateApnsVoipSandboxChannelResponseTypeDef,
+    UpdateBaiduChannelResponseTypeDef,
     CreateEmailTemplateRequestRequestTypeDef,
     UpdateEmailTemplateRequestRequestTypeDef,
     CreateEmailTemplateResponseTypeDef,
     CreatePushTemplateResponseTypeDef,
     CreateSmsTemplateResponseTypeDef,
     CreateVoiceTemplateResponseTypeDef,
     CreateExportJobRequestRequestTypeDef,
@@ -575,17 +616,18 @@
     GetRecommenderConfigurationResponseTypeDef,
     ListRecommenderConfigurationsResponseTypeDef,
     UpdateRecommenderConfigurationResponseTypeDef,
     CreateSmsTemplateRequestRequestTypeDef,
     UpdateSmsTemplateRequestRequestTypeDef,
     CreateVoiceTemplateRequestRequestTypeDef,
     UpdateVoiceTemplateRequestRequestTypeDef,
+    CustomMessageActivityOutputTypeDef,
     CustomMessageActivityTypeDef,
-    PushNotificationTemplateRequestTypeDef,
     PushNotificationTemplateResponseTypeDef,
+    PushNotificationTemplateRequestTypeDef,
     DeleteEmailChannelResponseTypeDef,
     GetEmailChannelResponseTypeDef,
     UpdateEmailChannelResponseTypeDef,
     DeleteEmailTemplateResponseTypeDef,
     DeleteInAppTemplateResponseTypeDef,
     DeletePushTemplateResponseTypeDef,
     DeleteSmsTemplateResponseTypeDef,
@@ -607,154 +649,185 @@
     DeleteSmsChannelResponseTypeDef,
     GetSmsChannelResponseTypeDef,
     UpdateSmsChannelResponseTypeDef,
     DeleteVoiceChannelResponseTypeDef,
     GetVoiceChannelResponseTypeDef,
     UpdateVoiceChannelResponseTypeDef,
     UpdateEmailChannelRequestRequestTypeDef,
+    EmailMessageActivityOutputTypeDef,
     EmailMessageActivityTypeDef,
     GetEmailTemplateResponseTypeDef,
     EndpointBatchItemTypeDef,
     EndpointRequestTypeDef,
-    EndpointResponseTypeDef,
     PublicEndpointTypeDef,
     SendUsersMessageResponseTypeDef,
+    EndpointResponseTypeDef,
+    EventDimensionsOutputTypeDef,
+    SegmentDemographicsOutputTypeDef,
     EventDimensionsTypeDef,
     SegmentDemographicsTypeDef,
     ItemResponseTypeDef,
     EventTypeDef,
     ExportJobResponseTypeDef,
     UpdateGcmChannelRequestRequestTypeDef,
+    GPSPointDimensionOutputTypeDef,
     GPSPointDimensionTypeDef,
     GetJourneyExecutionActivityMetricsResponseTypeDef,
     GetJourneyExecutionMetricsResponseTypeDef,
     GetJourneyRunExecutionActivityMetricsResponseTypeDef,
     GetJourneyRunExecutionMetricsResponseTypeDef,
     GetSmsTemplateResponseTypeDef,
     GetVoiceTemplateResponseTypeDef,
     ImportJobResponseTypeDef,
+    InAppMessageButtonOutputTypeDef,
     InAppMessageButtonTypeDef,
+    PushMessageActivityOutputTypeDef,
     PushMessageActivityTypeDef,
     JourneyRunsResponseTypeDef,
+    SMSMessageActivityOutputTypeDef,
     SMSMessageActivityTypeDef,
     UpdateJourneyStateRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     MessageResponseTypeDef,
     PhoneNumberValidateRequestRequestTypeDef,
     PhoneNumberValidateResponseTypeDef,
+    OpenHoursOutputTypeDef,
     OpenHoursTypeDef,
     PutEventStreamRequestRequestTypeDef,
+    WriteApplicationSettingsRequestTypeDef,
+    RandomSplitActivityOutputTypeDef,
     RandomSplitActivityTypeDef,
+    SegmentBehaviorsOutputTypeDef,
     SegmentBehaviorsTypeDef,
     RemoveAttributesRequestRequestTypeDef,
     ResultRowTypeDef,
     UpdateSmsChannelRequestRequestTypeDef,
     SendOTPMessageRequestRequestTypeDef,
     SimpleEmailTypeDef,
+    TagResourceRequestRequestTypeDef,
     UpdateTemplateActiveVersionRequestRequestTypeDef,
+    TemplateConfigurationOutputTypeDef,
     TemplateConfigurationTypeDef,
     TemplatesResponseTypeDef,
     TemplateVersionsResponseTypeDef,
     UpdateRecommenderConfigurationRequestRequestTypeDef,
     UpdateVoiceChannelRequestRequestTypeDef,
     VerifyOTPMessageResponseTypeDef,
     VerifyOTPMessageRequestRequestTypeDef,
     GetCampaignActivitiesResponseTypeDef,
     GetAppsResponseTypeDef,
     GetApplicationSettingsResponseTypeDef,
     UpdateApplicationSettingsResponseTypeDef,
-    UpdateApplicationSettingsRequestRequestTypeDef,
     GetChannelsResponseTypeDef,
     GetRecommenderConfigurationsResponseTypeDef,
+    GetPushTemplateResponseTypeDef,
     CreatePushTemplateRequestRequestTypeDef,
     UpdatePushTemplateRequestRequestTypeDef,
-    GetPushTemplateResponseTypeDef,
     EndpointBatchRequestTypeDef,
     UpdateEndpointRequestRequestTypeDef,
+    SendUsersMessagesResponseTypeDef,
     DeleteEndpointResponseTypeDef,
     EndpointsResponseTypeDef,
     GetEndpointResponseTypeDef,
-    SendUsersMessagesResponseTypeDef,
+    CampaignEventFilterOutputTypeDef,
+    EventConditionOutputTypeDef,
+    EventFilterOutputTypeDef,
     CampaignEventFilterTypeDef,
     EventConditionTypeDef,
     EventFilterTypeDef,
     EventsResponseTypeDef,
     EventsBatchTypeDef,
     CreateExportJobResponseTypeDef,
     ExportJobsResponseTypeDef,
     GetExportJobResponseTypeDef,
+    SegmentLocationOutputTypeDef,
     SegmentLocationTypeDef,
     CreateImportJobResponseTypeDef,
     GetImportJobResponseTypeDef,
     ImportJobsResponseTypeDef,
+    InAppMessageContentOutputTypeDef,
     InAppMessageContentTypeDef,
     GetJourneyRunsResponseTypeDef,
     SendMessagesResponseTypeDef,
     SendOTPMessageResponseTypeDef,
+    UpdateApplicationSettingsRequestRequestTypeDef,
     BaseKpiResultTypeDef,
     EmailMessageTypeDef,
     ListTemplatesResponseTypeDef,
     ListTemplateVersionsResponseTypeDef,
     UpdateEndpointsBatchRequestRequestTypeDef,
     DeleteUserEndpointsResponseTypeDef,
     GetUserEndpointsResponseTypeDef,
     InAppCampaignScheduleTypeDef,
+    ScheduleOutputTypeDef,
+    EventStartConditionOutputTypeDef,
     ScheduleTypeDef,
     EventStartConditionTypeDef,
     PutEventsResponseTypeDef,
     EventsRequestTypeDef,
     GetExportJobsResponseTypeDef,
     GetSegmentExportJobsResponseTypeDef,
+    SegmentDimensionsOutputTypeDef,
     SegmentDimensionsTypeDef,
     GetImportJobsResponseTypeDef,
     GetSegmentImportJobsResponseTypeDef,
-    CampaignInAppMessageTypeDef,
+    CampaignInAppMessageOutputTypeDef,
     InAppMessageTypeDef,
-    InAppTemplateRequestTypeDef,
     InAppTemplateResponseTypeDef,
+    CampaignInAppMessageTypeDef,
+    InAppTemplateRequestTypeDef,
     ApplicationDateRangeKpiResponseTypeDef,
     CampaignDateRangeKpiResponseTypeDef,
     JourneyDateRangeKpiResponseTypeDef,
     DirectMessageConfigurationTypeDef,
+    StartConditionOutputTypeDef,
     StartConditionTypeDef,
     PutEventsRequestRequestTypeDef,
+    SegmentGroupOutputTypeDef,
+    SimpleConditionOutputTypeDef,
     SegmentGroupTypeDef,
     SimpleConditionTypeDef,
-    MessageConfigurationTypeDef,
+    MessageConfigurationOutputTypeDef,
     InAppMessageCampaignTypeDef,
+    GetInAppTemplateResponseTypeDef,
+    MessageConfigurationTypeDef,
     CreateInAppTemplateRequestRequestTypeDef,
     UpdateInAppTemplateRequestRequestTypeDef,
-    GetInAppTemplateResponseTypeDef,
     GetApplicationDateRangeKpiResponseTypeDef,
     GetCampaignDateRangeKpiResponseTypeDef,
     GetJourneyDateRangeKpiResponseTypeDef,
     MessageRequestTypeDef,
     SendUsersMessageRequestTypeDef,
+    SegmentGroupListOutputTypeDef,
+    ConditionOutputTypeDef,
+    MultiConditionalBranchOutputTypeDef,
     SegmentGroupListTypeDef,
     ConditionTypeDef,
     MultiConditionalBranchTypeDef,
     TreatmentResourceTypeDef,
-    WriteTreatmentResourceTypeDef,
     InAppMessagesResponseTypeDef,
+    WriteTreatmentResourceTypeDef,
     SendMessagesRequestRequestTypeDef,
     SendUsersMessagesRequestRequestTypeDef,
     SegmentResponseTypeDef,
+    ConditionalSplitActivityOutputTypeDef,
+    MultiConditionalSplitActivityOutputTypeDef,
     WriteSegmentRequestTypeDef,
     ConditionalSplitActivityTypeDef,
     MultiConditionalSplitActivityTypeDef,
     CampaignResponseTypeDef,
-    WriteCampaignRequestTypeDef,
     GetInAppMessagesResponseTypeDef,
+    WriteCampaignRequestTypeDef,
     CreateSegmentResponseTypeDef,
     DeleteSegmentResponseTypeDef,
     GetSegmentResponseTypeDef,
     GetSegmentVersionResponseTypeDef,
     SegmentsResponseTypeDef,
     UpdateSegmentResponseTypeDef,
+    ActivityOutputTypeDef,
     CreateSegmentRequestRequestTypeDef,
     UpdateSegmentRequestRequestTypeDef,
     ActivityTypeDef,
     CampaignsResponseTypeDef,
     CreateCampaignResponseTypeDef,
     DeleteCampaignResponseTypeDef,
     GetCampaignResponseTypeDef,
```

### Comparing `mypy-boto3-pinpoint-1.28.0/mypy_boto3_pinpoint.egg-info/SOURCES.txt` & `mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.28.0/setup.py` & `mypy-boto3-pinpoint-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pinpoint",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_pinpoint"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Pinpoint 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Pinpoint 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

