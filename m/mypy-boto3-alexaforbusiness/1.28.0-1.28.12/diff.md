# Comparing `tmp/mypy-boto3-alexaforbusiness-1.28.0.tar.gz` & `tmp/mypy-boto3-alexaforbusiness-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-alexaforbusiness-1.28.0.tar", last modified: Thu Jul  6 20:58:51 2023, max compression
+gzip compressed data, was "mypy-boto3-alexaforbusiness-1.28.12.tar", last modified: Thu Jul 27 05:34:13 2023, max compression
```

## Comparing `mypy-boto3-alexaforbusiness-1.28.0.tar` & `mypy-boto3-alexaforbusiness-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:51.678206 mypy-boto3-alexaforbusiness-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:32:35.000000 mypy-boto3-alexaforbusiness-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24249 2023-07-06 20:58:51.674206 mypy-boto3-alexaforbusiness-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22728 2023-07-06 20:32:35.000000 mypy-boto3-alexaforbusiness-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:51.666206 mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-06 20:32:35.000000 mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-06 20:32:35.000000 mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-06 20:32:35.000000 mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67440 2023-07-06 20:32:35.000000 mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    67327 2023-07-06 20:32:35.000000 mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-07-06 20:32:36.000000 mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-07-06 20:32:36.000000 mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16333 2023-07-06 20:32:36.000000 mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-07-06 20:32:36.000000 mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:32:35.000000 mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    71403 2023-07-06 20:32:39.000000 mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    71328 2023-07-06 20:32:38.000000 mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:32:35.000000 mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:51.674206 mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24249 2023-07-06 20:58:51.000000 mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-06 20:58:51.000000 mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:51.000000 mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:51.000000 mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:58:51.000000 mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 20:58:51.000000 mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:58:51.678206 mypy-boto3-alexaforbusiness-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-06 20:32:35.000000 mypy-boto3-alexaforbusiness-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.852594 mypy-boto3-alexaforbusiness-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:16:55.000000 mypy-boto3-alexaforbusiness-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24570 2023-07-27 05:34:13.848594 mypy-boto3-alexaforbusiness-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23047 2023-07-27 05:16:55.000000 mypy-boto3-alexaforbusiness-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.844594 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-27 05:16:55.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-27 05:16:55.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-27 05:16:55.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67440 2023-07-27 05:16:56.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67327 2023-07-27 05:16:56.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-07-27 05:16:57.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-07-27 05:16:56.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16333 2023-07-27 05:16:56.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-07-27 05:16:56.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:16:55.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    73359 2023-07-27 05:16:58.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73284 2023-07-27 05:16:57.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:16:55.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.848594 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24570 2023-07-27 05:34:13.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-27 05:34:13.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:13.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:34:13.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:13.852594 mypy-boto3-alexaforbusiness-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 05:16:55.000000 mypy-boto3-alexaforbusiness-1.28.12/setup.py
```

### Comparing `mypy-boto3-alexaforbusiness-1.28.0/LICENSE` & `mypy-boto3-alexaforbusiness-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.28.0/PKG-INFO` & `mypy-boto3-alexaforbusiness-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-alexaforbusiness
-Version: 1.28.0
-Summary: Type annotations for boto3.AlexaForBusiness 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AlexaForBusiness 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-alexaforbusiness"></a>
 
 # mypy-boto3-alexaforbusiness
 
 [![PyPI - mypy-boto3-alexaforbusiness](https://img.shields.io/pypi/v/mypy-boto3-alexaforbusiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-alexaforbusiness)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-alexaforbusiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-alexaforbusiness)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-alexaforbusiness?color=blue)](https://pypistats.org/packages/mypy-boto3-alexaforbusiness)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-alexaforbusiness)](https://pepy.tech/project/mypy-boto3-alexaforbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AlexaForBusiness 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
+[boto3.AlexaForBusiness 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
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
 [mypy-boto3-alexaforbusiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/).
 
 See how it helps to find and fix potential bugs:
 
@@ -408,28 +408,36 @@
     AssociateContactWithAddressBookRequestRequestTypeDef,
     AssociateDeviceWithNetworkProfileRequestRequestTypeDef,
     AssociateDeviceWithRoomRequestRequestTypeDef,
     AssociateSkillGroupWithRoomRequestRequestTypeDef,
     AssociateSkillWithSkillGroupRequestRequestTypeDef,
     AssociateSkillWithUsersRequestRequestTypeDef,
     AudioTypeDef,
+    BusinessReportContentRangeOutputTypeDef,
     BusinessReportContentRangeTypeDef,
+    BusinessReportRecurrenceOutputTypeDef,
     BusinessReportRecurrenceTypeDef,
     BusinessReportS3LocationTypeDef,
     CategoryTypeDef,
+    ConferencePreferenceOutputTypeDef,
     ConferencePreferenceTypeDef,
+    IPDialInOutputTypeDef,
+    MeetingSettingOutputTypeDef,
+    PSTNDialInOutputTypeDef,
+    PhoneNumberOutputTypeDef,
+    SipAddressOutputTypeDef,
+    SsmlTypeDef,
+    TextTypeDef,
+    TagTypeDef,
+    ResponseMetadataTypeDef,
     IPDialInTypeDef,
     MeetingSettingTypeDef,
     PSTNDialInTypeDef,
     PhoneNumberTypeDef,
     SipAddressTypeDef,
-    SsmlTypeDef,
-    TextTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
     CreateEndOfMeetingReminderTypeDef,
     CreateInstantBookingTypeDef,
     CreateProactiveJoinTypeDef,
     CreateRequireCheckInTypeDef,
     DeleteAddressBookRequestRequestTypeDef,
     DeleteBusinessReportScheduleRequestRequestTypeDef,
     DeleteConferenceProviderRequestRequestTypeDef,
@@ -468,15 +476,15 @@
     GetGatewayRequestRequestTypeDef,
     GetNetworkProfileRequestRequestTypeDef,
     NetworkProfileTypeDef,
     GetProfileRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     RoomTypeDef,
     GetRoomSkillParameterRequestRequestTypeDef,
-    RoomSkillParameterTypeDef,
+    RoomSkillParameterOutputTypeDef,
     GetSkillGroupRequestRequestTypeDef,
     SkillGroupTypeDef,
     InstantBookingTypeDef,
     PaginatorConfigTypeDef,
     ListBusinessReportSchedulesRequestRequestTypeDef,
     ListConferenceProvidersRequestRequestTypeDef,
     ListDeviceEventsRequestRequestTypeDef,
@@ -485,19 +493,21 @@
     ListSkillsRequestRequestTypeDef,
     SkillSummaryTypeDef,
     ListSkillsStoreCategoriesRequestRequestTypeDef,
     ListSkillsStoreSkillsByCategoryRequestRequestTypeDef,
     ListSmartHomeAppliancesRequestRequestTypeDef,
     SmartHomeApplianceTypeDef,
     ListTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     ProactiveJoinTypeDef,
     RequireCheckInTypeDef,
     NetworkProfileDataTypeDef,
     ProfileDataTypeDef,
     PutInvitationConfigurationRequestRequestTypeDef,
+    RoomSkillParameterTypeDef,
     PutSkillAuthorizationRequestRequestTypeDef,
     RejectSkillRequestRequestTypeDef,
     ResolveRoomRequestRequestTypeDef,
     RevokeInvitationRequestRequestTypeDef,
     RoomDataTypeDef,
     SortTypeDef,
     SkillGroupDataTypeDef,
@@ -517,23 +527,19 @@
     UpdateNetworkProfileRequestRequestTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateSkillGroupRequestRequestTypeDef,
     UpdateBusinessReportScheduleRequestRequestTypeDef,
     BusinessReportTypeDef,
     PutConferencePreferenceRequestRequestTypeDef,
     ConferenceProviderTypeDef,
-    UpdateConferenceProviderRequestRequestTypeDef,
     ContactDataTypeDef,
     ContactTypeDef,
-    UpdateContactRequestRequestTypeDef,
     ContentTypeDef,
     CreateAddressBookRequestRequestTypeDef,
     CreateBusinessReportScheduleRequestRequestTypeDef,
-    CreateConferenceProviderRequestRequestTypeDef,
-    CreateContactRequestRequestTypeDef,
     CreateGatewayGroupRequestRequestTypeDef,
     CreateNetworkProfileRequestRequestTypeDef,
     CreateRoomRequestRequestTypeDef,
     CreateSkillGroupRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     RegisterAVSDeviceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -547,45 +553,49 @@
     CreateRoomResponseTypeDef,
     CreateSkillGroupResponseTypeDef,
     CreateUserResponseTypeDef,
     GetAddressBookResponseTypeDef,
     GetConferencePreferenceResponseTypeDef,
     GetInvitationConfigurationResponseTypeDef,
     ListSkillsStoreCategoriesResponseTypeDef,
-    ListTagsResponseTypeDef,
     RegisterAVSDeviceResponseTypeDef,
     SearchAddressBooksResponseTypeDef,
     SendAnnouncementResponseTypeDef,
+    CreateConferenceProviderRequestRequestTypeDef,
+    UpdateConferenceProviderRequestRequestTypeDef,
+    CreateContactRequestRequestTypeDef,
+    UpdateContactRequestRequestTypeDef,
     CreateMeetingRoomConfigurationTypeDef,
     SkillDetailsTypeDef,
     ListDeviceEventsResponseTypeDef,
     DeviceStatusInfoTypeDef,
     ListGatewayGroupsResponseTypeDef,
     GetGatewayGroupResponseTypeDef,
     ListGatewaysResponseTypeDef,
     GetGatewayResponseTypeDef,
     GetNetworkProfileResponseTypeDef,
     GetRoomResponseTypeDef,
     GetRoomSkillParameterResponseTypeDef,
-    PutRoomSkillParameterRequestRequestTypeDef,
     ResolveRoomResponseTypeDef,
     GetSkillGroupResponseTypeDef,
     ListBusinessReportSchedulesRequestListBusinessReportSchedulesPaginateTypeDef,
     ListConferenceProvidersRequestListConferenceProvidersPaginateTypeDef,
     ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
     ListSkillsRequestListSkillsPaginateTypeDef,
     ListSkillsStoreCategoriesRequestListSkillsStoreCategoriesPaginateTypeDef,
     ListSkillsStoreSkillsByCategoryRequestListSkillsStoreSkillsByCategoryPaginateTypeDef,
     ListSmartHomeAppliancesRequestListSmartHomeAppliancesPaginateTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
     ListSkillsResponseTypeDef,
     ListSmartHomeAppliancesResponseTypeDef,
+    ListTagsResponseTypeDef,
     MeetingRoomConfigurationTypeDef,
     SearchNetworkProfilesResponseTypeDef,
     SearchProfilesResponseTypeDef,
+    PutRoomSkillParameterRequestRequestTypeDef,
     SearchRoomsResponseTypeDef,
     SearchAddressBooksRequestRequestTypeDef,
     SearchContactsRequestRequestTypeDef,
     SearchDevicesRequestRequestTypeDef,
     SearchDevicesRequestSearchDevicesPaginateTypeDef,
     SearchNetworkProfilesRequestRequestTypeDef,
     SearchProfilesRequestRequestTypeDef,
```

### Comparing `mypy-boto3-alexaforbusiness-1.28.0/README.md` & `mypy-boto3-alexaforbusiness-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-alexaforbusiness"></a>
 
 # mypy-boto3-alexaforbusiness
 
 [![PyPI - mypy-boto3-alexaforbusiness](https://img.shields.io/pypi/v/mypy-boto3-alexaforbusiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-alexaforbusiness)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-alexaforbusiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-alexaforbusiness)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-alexaforbusiness?color=blue)](https://pypistats.org/packages/mypy-boto3-alexaforbusiness)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-alexaforbusiness)](https://pepy.tech/project/mypy-boto3-alexaforbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AlexaForBusiness 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
+[boto3.AlexaForBusiness 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
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
 [mypy-boto3-alexaforbusiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/).
 
 See how it helps to find and fix potential bugs:
 
@@ -376,28 +376,36 @@
     AssociateContactWithAddressBookRequestRequestTypeDef,
     AssociateDeviceWithNetworkProfileRequestRequestTypeDef,
     AssociateDeviceWithRoomRequestRequestTypeDef,
     AssociateSkillGroupWithRoomRequestRequestTypeDef,
     AssociateSkillWithSkillGroupRequestRequestTypeDef,
     AssociateSkillWithUsersRequestRequestTypeDef,
     AudioTypeDef,
+    BusinessReportContentRangeOutputTypeDef,
     BusinessReportContentRangeTypeDef,
+    BusinessReportRecurrenceOutputTypeDef,
     BusinessReportRecurrenceTypeDef,
     BusinessReportS3LocationTypeDef,
     CategoryTypeDef,
+    ConferencePreferenceOutputTypeDef,
     ConferencePreferenceTypeDef,
+    IPDialInOutputTypeDef,
+    MeetingSettingOutputTypeDef,
+    PSTNDialInOutputTypeDef,
+    PhoneNumberOutputTypeDef,
+    SipAddressOutputTypeDef,
+    SsmlTypeDef,
+    TextTypeDef,
+    TagTypeDef,
+    ResponseMetadataTypeDef,
     IPDialInTypeDef,
     MeetingSettingTypeDef,
     PSTNDialInTypeDef,
     PhoneNumberTypeDef,
     SipAddressTypeDef,
-    SsmlTypeDef,
-    TextTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
     CreateEndOfMeetingReminderTypeDef,
     CreateInstantBookingTypeDef,
     CreateProactiveJoinTypeDef,
     CreateRequireCheckInTypeDef,
     DeleteAddressBookRequestRequestTypeDef,
     DeleteBusinessReportScheduleRequestRequestTypeDef,
     DeleteConferenceProviderRequestRequestTypeDef,
@@ -436,15 +444,15 @@
     GetGatewayRequestRequestTypeDef,
     GetNetworkProfileRequestRequestTypeDef,
     NetworkProfileTypeDef,
     GetProfileRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     RoomTypeDef,
     GetRoomSkillParameterRequestRequestTypeDef,
-    RoomSkillParameterTypeDef,
+    RoomSkillParameterOutputTypeDef,
     GetSkillGroupRequestRequestTypeDef,
     SkillGroupTypeDef,
     InstantBookingTypeDef,
     PaginatorConfigTypeDef,
     ListBusinessReportSchedulesRequestRequestTypeDef,
     ListConferenceProvidersRequestRequestTypeDef,
     ListDeviceEventsRequestRequestTypeDef,
@@ -453,19 +461,21 @@
     ListSkillsRequestRequestTypeDef,
     SkillSummaryTypeDef,
     ListSkillsStoreCategoriesRequestRequestTypeDef,
     ListSkillsStoreSkillsByCategoryRequestRequestTypeDef,
     ListSmartHomeAppliancesRequestRequestTypeDef,
     SmartHomeApplianceTypeDef,
     ListTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     ProactiveJoinTypeDef,
     RequireCheckInTypeDef,
     NetworkProfileDataTypeDef,
     ProfileDataTypeDef,
     PutInvitationConfigurationRequestRequestTypeDef,
+    RoomSkillParameterTypeDef,
     PutSkillAuthorizationRequestRequestTypeDef,
     RejectSkillRequestRequestTypeDef,
     ResolveRoomRequestRequestTypeDef,
     RevokeInvitationRequestRequestTypeDef,
     RoomDataTypeDef,
     SortTypeDef,
     SkillGroupDataTypeDef,
@@ -485,23 +495,19 @@
     UpdateNetworkProfileRequestRequestTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateSkillGroupRequestRequestTypeDef,
     UpdateBusinessReportScheduleRequestRequestTypeDef,
     BusinessReportTypeDef,
     PutConferencePreferenceRequestRequestTypeDef,
     ConferenceProviderTypeDef,
-    UpdateConferenceProviderRequestRequestTypeDef,
     ContactDataTypeDef,
     ContactTypeDef,
-    UpdateContactRequestRequestTypeDef,
     ContentTypeDef,
     CreateAddressBookRequestRequestTypeDef,
     CreateBusinessReportScheduleRequestRequestTypeDef,
-    CreateConferenceProviderRequestRequestTypeDef,
-    CreateContactRequestRequestTypeDef,
     CreateGatewayGroupRequestRequestTypeDef,
     CreateNetworkProfileRequestRequestTypeDef,
     CreateRoomRequestRequestTypeDef,
     CreateSkillGroupRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     RegisterAVSDeviceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -515,45 +521,49 @@
     CreateRoomResponseTypeDef,
     CreateSkillGroupResponseTypeDef,
     CreateUserResponseTypeDef,
     GetAddressBookResponseTypeDef,
     GetConferencePreferenceResponseTypeDef,
     GetInvitationConfigurationResponseTypeDef,
     ListSkillsStoreCategoriesResponseTypeDef,
-    ListTagsResponseTypeDef,
     RegisterAVSDeviceResponseTypeDef,
     SearchAddressBooksResponseTypeDef,
     SendAnnouncementResponseTypeDef,
+    CreateConferenceProviderRequestRequestTypeDef,
+    UpdateConferenceProviderRequestRequestTypeDef,
+    CreateContactRequestRequestTypeDef,
+    UpdateContactRequestRequestTypeDef,
     CreateMeetingRoomConfigurationTypeDef,
     SkillDetailsTypeDef,
     ListDeviceEventsResponseTypeDef,
     DeviceStatusInfoTypeDef,
     ListGatewayGroupsResponseTypeDef,
     GetGatewayGroupResponseTypeDef,
     ListGatewaysResponseTypeDef,
     GetGatewayResponseTypeDef,
     GetNetworkProfileResponseTypeDef,
     GetRoomResponseTypeDef,
     GetRoomSkillParameterResponseTypeDef,
-    PutRoomSkillParameterRequestRequestTypeDef,
     ResolveRoomResponseTypeDef,
     GetSkillGroupResponseTypeDef,
     ListBusinessReportSchedulesRequestListBusinessReportSchedulesPaginateTypeDef,
     ListConferenceProvidersRequestListConferenceProvidersPaginateTypeDef,
     ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
     ListSkillsRequestListSkillsPaginateTypeDef,
     ListSkillsStoreCategoriesRequestListSkillsStoreCategoriesPaginateTypeDef,
     ListSkillsStoreSkillsByCategoryRequestListSkillsStoreSkillsByCategoryPaginateTypeDef,
     ListSmartHomeAppliancesRequestListSmartHomeAppliancesPaginateTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
     ListSkillsResponseTypeDef,
     ListSmartHomeAppliancesResponseTypeDef,
+    ListTagsResponseTypeDef,
     MeetingRoomConfigurationTypeDef,
     SearchNetworkProfilesResponseTypeDef,
     SearchProfilesResponseTypeDef,
+    PutRoomSkillParameterRequestRequestTypeDef,
     SearchRoomsResponseTypeDef,
     SearchAddressBooksRequestRequestTypeDef,
     SearchContactsRequestRequestTypeDef,
     SearchDevicesRequestRequestTypeDef,
     SearchDevicesRequestSearchDevicesPaginateTypeDef,
     SearchNetworkProfilesRequestRequestTypeDef,
     SearchProfilesRequestRequestTypeDef,
```

### Comparing `mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/__init__.py` & `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/__init__.pyi` & `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/__main__.py` & `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AlexaForBusiness 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.AlexaForBusiness 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness\nOther"
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

### Comparing `mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/client.py` & `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/client.pyi` & `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/literals.py` & `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,14 +261,15 @@
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
@@ -347,26 +348,28 @@
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

### Comparing `mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/literals.pyi` & `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -259,14 +259,15 @@
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
@@ -345,26 +346,28 @@
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

### Comparing `mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/paginator.py` & `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/paginator.pyi` & `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/type_defs.py` & `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,28 +59,36 @@
     "AssociateContactWithAddressBookRequestRequestTypeDef",
     "AssociateDeviceWithNetworkProfileRequestRequestTypeDef",
     "AssociateDeviceWithRoomRequestRequestTypeDef",
     "AssociateSkillGroupWithRoomRequestRequestTypeDef",
     "AssociateSkillWithSkillGroupRequestRequestTypeDef",
     "AssociateSkillWithUsersRequestRequestTypeDef",
     "AudioTypeDef",
+    "BusinessReportContentRangeOutputTypeDef",
     "BusinessReportContentRangeTypeDef",
+    "BusinessReportRecurrenceOutputTypeDef",
     "BusinessReportRecurrenceTypeDef",
     "BusinessReportS3LocationTypeDef",
     "CategoryTypeDef",
+    "ConferencePreferenceOutputTypeDef",
     "ConferencePreferenceTypeDef",
+    "IPDialInOutputTypeDef",
+    "MeetingSettingOutputTypeDef",
+    "PSTNDialInOutputTypeDef",
+    "PhoneNumberOutputTypeDef",
+    "SipAddressOutputTypeDef",
+    "SsmlTypeDef",
+    "TextTypeDef",
+    "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "IPDialInTypeDef",
     "MeetingSettingTypeDef",
     "PSTNDialInTypeDef",
     "PhoneNumberTypeDef",
     "SipAddressTypeDef",
-    "SsmlTypeDef",
-    "TextTypeDef",
-    "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateEndOfMeetingReminderTypeDef",
     "CreateInstantBookingTypeDef",
     "CreateProactiveJoinTypeDef",
     "CreateRequireCheckInTypeDef",
     "DeleteAddressBookRequestRequestTypeDef",
     "DeleteBusinessReportScheduleRequestRequestTypeDef",
     "DeleteConferenceProviderRequestRequestTypeDef",
@@ -119,15 +127,15 @@
     "GetGatewayRequestRequestTypeDef",
     "GetNetworkProfileRequestRequestTypeDef",
     "NetworkProfileTypeDef",
     "GetProfileRequestRequestTypeDef",
     "GetRoomRequestRequestTypeDef",
     "RoomTypeDef",
     "GetRoomSkillParameterRequestRequestTypeDef",
-    "RoomSkillParameterTypeDef",
+    "RoomSkillParameterOutputTypeDef",
     "GetSkillGroupRequestRequestTypeDef",
     "SkillGroupTypeDef",
     "InstantBookingTypeDef",
     "PaginatorConfigTypeDef",
     "ListBusinessReportSchedulesRequestRequestTypeDef",
     "ListConferenceProvidersRequestRequestTypeDef",
     "ListDeviceEventsRequestRequestTypeDef",
@@ -136,19 +144,21 @@
     "ListSkillsRequestRequestTypeDef",
     "SkillSummaryTypeDef",
     "ListSkillsStoreCategoriesRequestRequestTypeDef",
     "ListSkillsStoreSkillsByCategoryRequestRequestTypeDef",
     "ListSmartHomeAppliancesRequestRequestTypeDef",
     "SmartHomeApplianceTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ProactiveJoinTypeDef",
     "RequireCheckInTypeDef",
     "NetworkProfileDataTypeDef",
     "ProfileDataTypeDef",
     "PutInvitationConfigurationRequestRequestTypeDef",
+    "RoomSkillParameterTypeDef",
     "PutSkillAuthorizationRequestRequestTypeDef",
     "RejectSkillRequestRequestTypeDef",
     "ResolveRoomRequestRequestTypeDef",
     "RevokeInvitationRequestRequestTypeDef",
     "RoomDataTypeDef",
     "SortTypeDef",
     "SkillGroupDataTypeDef",
@@ -168,23 +178,19 @@
     "UpdateNetworkProfileRequestRequestTypeDef",
     "UpdateRoomRequestRequestTypeDef",
     "UpdateSkillGroupRequestRequestTypeDef",
     "UpdateBusinessReportScheduleRequestRequestTypeDef",
     "BusinessReportTypeDef",
     "PutConferencePreferenceRequestRequestTypeDef",
     "ConferenceProviderTypeDef",
-    "UpdateConferenceProviderRequestRequestTypeDef",
     "ContactDataTypeDef",
     "ContactTypeDef",
-    "UpdateContactRequestRequestTypeDef",
     "ContentTypeDef",
     "CreateAddressBookRequestRequestTypeDef",
     "CreateBusinessReportScheduleRequestRequestTypeDef",
-    "CreateConferenceProviderRequestRequestTypeDef",
-    "CreateContactRequestRequestTypeDef",
     "CreateGatewayGroupRequestRequestTypeDef",
     "CreateNetworkProfileRequestRequestTypeDef",
     "CreateRoomRequestRequestTypeDef",
     "CreateSkillGroupRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "RegisterAVSDeviceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -198,45 +204,49 @@
     "CreateRoomResponseTypeDef",
     "CreateSkillGroupResponseTypeDef",
     "CreateUserResponseTypeDef",
     "GetAddressBookResponseTypeDef",
     "GetConferencePreferenceResponseTypeDef",
     "GetInvitationConfigurationResponseTypeDef",
     "ListSkillsStoreCategoriesResponseTypeDef",
-    "ListTagsResponseTypeDef",
     "RegisterAVSDeviceResponseTypeDef",
     "SearchAddressBooksResponseTypeDef",
     "SendAnnouncementResponseTypeDef",
+    "CreateConferenceProviderRequestRequestTypeDef",
+    "UpdateConferenceProviderRequestRequestTypeDef",
+    "CreateContactRequestRequestTypeDef",
+    "UpdateContactRequestRequestTypeDef",
     "CreateMeetingRoomConfigurationTypeDef",
     "SkillDetailsTypeDef",
     "ListDeviceEventsResponseTypeDef",
     "DeviceStatusInfoTypeDef",
     "ListGatewayGroupsResponseTypeDef",
     "GetGatewayGroupResponseTypeDef",
     "ListGatewaysResponseTypeDef",
     "GetGatewayResponseTypeDef",
     "GetNetworkProfileResponseTypeDef",
     "GetRoomResponseTypeDef",
     "GetRoomSkillParameterResponseTypeDef",
-    "PutRoomSkillParameterRequestRequestTypeDef",
     "ResolveRoomResponseTypeDef",
     "GetSkillGroupResponseTypeDef",
     "ListBusinessReportSchedulesRequestListBusinessReportSchedulesPaginateTypeDef",
     "ListConferenceProvidersRequestListConferenceProvidersPaginateTypeDef",
     "ListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
     "ListSkillsRequestListSkillsPaginateTypeDef",
     "ListSkillsStoreCategoriesRequestListSkillsStoreCategoriesPaginateTypeDef",
     "ListSkillsStoreSkillsByCategoryRequestListSkillsStoreSkillsByCategoryPaginateTypeDef",
     "ListSmartHomeAppliancesRequestListSmartHomeAppliancesPaginateTypeDef",
     "ListTagsRequestListTagsPaginateTypeDef",
     "ListSkillsResponseTypeDef",
     "ListSmartHomeAppliancesResponseTypeDef",
+    "ListTagsResponseTypeDef",
     "MeetingRoomConfigurationTypeDef",
     "SearchNetworkProfilesResponseTypeDef",
     "SearchProfilesResponseTypeDef",
+    "PutRoomSkillParameterRequestRequestTypeDef",
     "SearchRoomsResponseTypeDef",
     "SearchAddressBooksRequestRequestTypeDef",
     "SearchContactsRequestRequestTypeDef",
     "SearchDevicesRequestRequestTypeDef",
     "SearchDevicesRequestSearchDevicesPaginateTypeDef",
     "SearchNetworkProfilesRequestRequestTypeDef",
     "SearchProfilesRequestRequestTypeDef",
@@ -363,21 +373,36 @@
     "AudioTypeDef",
     {
         "Locale": Literal["en-US"],
         "Location": str,
     },
 )
 
+BusinessReportContentRangeOutputTypeDef = TypedDict(
+    "BusinessReportContentRangeOutputTypeDef",
+    {
+        "Interval": BusinessReportIntervalType,
+    },
+)
+
 BusinessReportContentRangeTypeDef = TypedDict(
     "BusinessReportContentRangeTypeDef",
     {
         "Interval": BusinessReportIntervalType,
     },
 )
 
+BusinessReportRecurrenceOutputTypeDef = TypedDict(
+    "BusinessReportRecurrenceOutputTypeDef",
+    {
+        "StartDate": str,
+    },
+    total=False,
+)
+
 BusinessReportRecurrenceTypeDef = TypedDict(
     "BusinessReportRecurrenceTypeDef",
     {
         "StartDate": str,
     },
     total=False,
 )
@@ -396,57 +421,65 @@
     {
         "CategoryId": int,
         "CategoryName": str,
     },
     total=False,
 )
 
+ConferencePreferenceOutputTypeDef = TypedDict(
+    "ConferencePreferenceOutputTypeDef",
+    {
+        "DefaultConferenceProviderArn": str,
+    },
+    total=False,
+)
+
 ConferencePreferenceTypeDef = TypedDict(
     "ConferencePreferenceTypeDef",
     {
         "DefaultConferenceProviderArn": str,
     },
     total=False,
 )
 
-IPDialInTypeDef = TypedDict(
-    "IPDialInTypeDef",
+IPDialInOutputTypeDef = TypedDict(
+    "IPDialInOutputTypeDef",
     {
         "Endpoint": str,
         "CommsProtocol": CommsProtocolType,
     },
 )
 
-MeetingSettingTypeDef = TypedDict(
-    "MeetingSettingTypeDef",
+MeetingSettingOutputTypeDef = TypedDict(
+    "MeetingSettingOutputTypeDef",
     {
         "RequirePin": RequirePinType,
     },
 )
 
-PSTNDialInTypeDef = TypedDict(
-    "PSTNDialInTypeDef",
+PSTNDialInOutputTypeDef = TypedDict(
+    "PSTNDialInOutputTypeDef",
     {
         "CountryCode": str,
         "PhoneNumber": str,
         "OneClickIdDelay": str,
         "OneClickPinDelay": str,
     },
 )
 
-PhoneNumberTypeDef = TypedDict(
-    "PhoneNumberTypeDef",
+PhoneNumberOutputTypeDef = TypedDict(
+    "PhoneNumberOutputTypeDef",
     {
         "Number": str,
         "Type": PhoneNumberTypeType,
     },
 )
 
-SipAddressTypeDef = TypedDict(
-    "SipAddressTypeDef",
+SipAddressOutputTypeDef = TypedDict(
+    "SipAddressOutputTypeDef",
     {
         "Uri": str,
         "Type": Literal["WORK"],
     },
 )
 
 SsmlTypeDef = TypedDict(
@@ -480,14 +513,55 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+IPDialInTypeDef = TypedDict(
+    "IPDialInTypeDef",
+    {
+        "Endpoint": str,
+        "CommsProtocol": CommsProtocolType,
+    },
+)
+
+MeetingSettingTypeDef = TypedDict(
+    "MeetingSettingTypeDef",
+    {
+        "RequirePin": RequirePinType,
+    },
+)
+
+PSTNDialInTypeDef = TypedDict(
+    "PSTNDialInTypeDef",
+    {
+        "CountryCode": str,
+        "PhoneNumber": str,
+        "OneClickIdDelay": str,
+        "OneClickPinDelay": str,
+    },
+)
+
+PhoneNumberTypeDef = TypedDict(
+    "PhoneNumberTypeDef",
+    {
+        "Number": str,
+        "Type": PhoneNumberTypeType,
+    },
+)
+
+SipAddressTypeDef = TypedDict(
+    "SipAddressTypeDef",
+    {
+        "Uri": str,
+        "Type": Literal["WORK"],
+    },
+)
+
 CreateEndOfMeetingReminderTypeDef = TypedDict(
     "CreateEndOfMeetingReminderTypeDef",
     {
         "ReminderAtMinutes": Sequence[int],
         "ReminderType": EndOfMeetingReminderTypeType,
         "Enabled": bool,
     },
@@ -940,16 +1014,16 @@
 class GetRoomSkillParameterRequestRequestTypeDef(
     _RequiredGetRoomSkillParameterRequestRequestTypeDef,
     _OptionalGetRoomSkillParameterRequestRequestTypeDef,
 ):
     pass
 
 
-RoomSkillParameterTypeDef = TypedDict(
-    "RoomSkillParameterTypeDef",
+RoomSkillParameterOutputTypeDef = TypedDict(
+    "RoomSkillParameterOutputTypeDef",
     {
         "ParameterKey": str,
         "ParameterValue": str,
     },
 )
 
 GetSkillGroupRequestRequestTypeDef = TypedDict(
@@ -1156,14 +1230,22 @@
 
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 ProactiveJoinTypeDef = TypedDict(
     "ProactiveJoinTypeDef",
     {
         "EnabledByMotion": bool,
     },
     total=False,
 )
@@ -1226,14 +1308,22 @@
 class PutInvitationConfigurationRequestRequestTypeDef(
     _RequiredPutInvitationConfigurationRequestRequestTypeDef,
     _OptionalPutInvitationConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+RoomSkillParameterTypeDef = TypedDict(
+    "RoomSkillParameterTypeDef",
+    {
+        "ParameterKey": str,
+        "ParameterValue": str,
+    },
+)
+
 _RequiredPutSkillAuthorizationRequestRequestTypeDef = TypedDict(
     "_RequiredPutSkillAuthorizationRequestRequestTypeDef",
     {
         "AuthorizationResult": Mapping[str, str],
         "SkillId": str,
     },
 )
@@ -1574,100 +1664,49 @@
 
 ConferenceProviderTypeDef = TypedDict(
     "ConferenceProviderTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Type": ConferenceProviderTypeType,
-        "IPDialIn": IPDialInTypeDef,
-        "PSTNDialIn": PSTNDialInTypeDef,
-        "MeetingSetting": MeetingSettingTypeDef,
-    },
-    total=False,
-)
-
-_RequiredUpdateConferenceProviderRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateConferenceProviderRequestRequestTypeDef",
-    {
-        "ConferenceProviderArn": str,
-        "ConferenceProviderType": ConferenceProviderTypeType,
-        "MeetingSetting": MeetingSettingTypeDef,
-    },
-)
-_OptionalUpdateConferenceProviderRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateConferenceProviderRequestRequestTypeDef",
-    {
-        "IPDialIn": IPDialInTypeDef,
-        "PSTNDialIn": PSTNDialInTypeDef,
+        "IPDialIn": IPDialInOutputTypeDef,
+        "PSTNDialIn": PSTNDialInOutputTypeDef,
+        "MeetingSetting": MeetingSettingOutputTypeDef,
     },
     total=False,
 )
 
-
-class UpdateConferenceProviderRequestRequestTypeDef(
-    _RequiredUpdateConferenceProviderRequestRequestTypeDef,
-    _OptionalUpdateConferenceProviderRequestRequestTypeDef,
-):
-    pass
-
-
 ContactDataTypeDef = TypedDict(
     "ContactDataTypeDef",
     {
         "ContactArn": str,
         "DisplayName": str,
         "FirstName": str,
         "LastName": str,
         "PhoneNumber": str,
-        "PhoneNumbers": List[PhoneNumberTypeDef],
-        "SipAddresses": List[SipAddressTypeDef],
+        "PhoneNumbers": List[PhoneNumberOutputTypeDef],
+        "SipAddresses": List[SipAddressOutputTypeDef],
     },
     total=False,
 )
 
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "ContactArn": str,
         "DisplayName": str,
         "FirstName": str,
         "LastName": str,
         "PhoneNumber": str,
-        "PhoneNumbers": List[PhoneNumberTypeDef],
-        "SipAddresses": List[SipAddressTypeDef],
-    },
-    total=False,
-)
-
-_RequiredUpdateContactRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateContactRequestRequestTypeDef",
-    {
-        "ContactArn": str,
-    },
-)
-_OptionalUpdateContactRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateContactRequestRequestTypeDef",
-    {
-        "DisplayName": str,
-        "FirstName": str,
-        "LastName": str,
-        "PhoneNumber": str,
-        "PhoneNumbers": Sequence[PhoneNumberTypeDef],
-        "SipAddresses": Sequence[SipAddressTypeDef],
+        "PhoneNumbers": List[PhoneNumberOutputTypeDef],
+        "SipAddresses": List[SipAddressOutputTypeDef],
     },
     total=False,
 )
 
-
-class UpdateContactRequestRequestTypeDef(
-    _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
-):
-    pass
-
-
 ContentTypeDef = TypedDict(
     "ContentTypeDef",
     {
         "TextList": Sequence[TextTypeDef],
         "SsmlList": Sequence[SsmlTypeDef],
         "AudioList": Sequence[AudioTypeDef],
     },
@@ -1721,68 +1760,14 @@
 class CreateBusinessReportScheduleRequestRequestTypeDef(
     _RequiredCreateBusinessReportScheduleRequestRequestTypeDef,
     _OptionalCreateBusinessReportScheduleRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredCreateConferenceProviderRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateConferenceProviderRequestRequestTypeDef",
-    {
-        "ConferenceProviderName": str,
-        "ConferenceProviderType": ConferenceProviderTypeType,
-        "MeetingSetting": MeetingSettingTypeDef,
-    },
-)
-_OptionalCreateConferenceProviderRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateConferenceProviderRequestRequestTypeDef",
-    {
-        "IPDialIn": IPDialInTypeDef,
-        "PSTNDialIn": PSTNDialInTypeDef,
-        "ClientRequestToken": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateConferenceProviderRequestRequestTypeDef(
-    _RequiredCreateConferenceProviderRequestRequestTypeDef,
-    _OptionalCreateConferenceProviderRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateContactRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateContactRequestRequestTypeDef",
-    {
-        "FirstName": str,
-    },
-)
-_OptionalCreateContactRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateContactRequestRequestTypeDef",
-    {
-        "DisplayName": str,
-        "LastName": str,
-        "PhoneNumber": str,
-        "PhoneNumbers": Sequence[PhoneNumberTypeDef],
-        "SipAddresses": Sequence[SipAddressTypeDef],
-        "ClientRequestToken": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateContactRequestRequestTypeDef(
-    _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredCreateGatewayGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGatewayGroupRequestRequestTypeDef",
     {
         "Name": str,
         "ClientRequestToken": str,
     },
 )
@@ -2028,15 +2013,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConferencePreferenceResponseTypeDef = TypedDict(
     "GetConferencePreferenceResponseTypeDef",
     {
-        "Preference": ConferencePreferenceTypeDef,
+        "Preference": ConferencePreferenceOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInvitationConfigurationResponseTypeDef = TypedDict(
     "GetInvitationConfigurationResponseTypeDef",
     {
@@ -2052,23 +2037,14 @@
     {
         "CategoryList": List[CategoryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 RegisterAVSDeviceResponseTypeDef = TypedDict(
     "RegisterAVSDeviceResponseTypeDef",
     {
         "DeviceArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2087,14 +2063,119 @@
     "SendAnnouncementResponseTypeDef",
     {
         "AnnouncementArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateConferenceProviderRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateConferenceProviderRequestRequestTypeDef",
+    {
+        "ConferenceProviderName": str,
+        "ConferenceProviderType": ConferenceProviderTypeType,
+        "MeetingSetting": MeetingSettingTypeDef,
+    },
+)
+_OptionalCreateConferenceProviderRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateConferenceProviderRequestRequestTypeDef",
+    {
+        "IPDialIn": IPDialInTypeDef,
+        "PSTNDialIn": PSTNDialInTypeDef,
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateConferenceProviderRequestRequestTypeDef(
+    _RequiredCreateConferenceProviderRequestRequestTypeDef,
+    _OptionalCreateConferenceProviderRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateConferenceProviderRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateConferenceProviderRequestRequestTypeDef",
+    {
+        "ConferenceProviderArn": str,
+        "ConferenceProviderType": ConferenceProviderTypeType,
+        "MeetingSetting": MeetingSettingTypeDef,
+    },
+)
+_OptionalUpdateConferenceProviderRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateConferenceProviderRequestRequestTypeDef",
+    {
+        "IPDialIn": IPDialInTypeDef,
+        "PSTNDialIn": PSTNDialInTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateConferenceProviderRequestRequestTypeDef(
+    _RequiredUpdateConferenceProviderRequestRequestTypeDef,
+    _OptionalUpdateConferenceProviderRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateContactRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateContactRequestRequestTypeDef",
+    {
+        "FirstName": str,
+    },
+)
+_OptionalCreateContactRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateContactRequestRequestTypeDef",
+    {
+        "DisplayName": str,
+        "LastName": str,
+        "PhoneNumber": str,
+        "PhoneNumbers": Sequence[PhoneNumberTypeDef],
+        "SipAddresses": Sequence[SipAddressTypeDef],
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateContactRequestRequestTypeDef(
+    _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateContactRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateContactRequestRequestTypeDef",
+    {
+        "ContactArn": str,
+    },
+)
+_OptionalUpdateContactRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateContactRequestRequestTypeDef",
+    {
+        "DisplayName": str,
+        "FirstName": str,
+        "LastName": str,
+        "PhoneNumber": str,
+        "PhoneNumbers": Sequence[PhoneNumberTypeDef],
+        "SipAddresses": Sequence[SipAddressTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateContactRequestRequestTypeDef(
+    _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
+):
+    pass
+
+
 CreateMeetingRoomConfigurationTypeDef = TypedDict(
     "CreateMeetingRoomConfigurationTypeDef",
     {
         "RoomUtilizationMetricsEnabled": bool,
         "EndOfMeetingReminder": CreateEndOfMeetingReminderTypeDef,
         "InstantBooking": CreateInstantBookingTypeDef,
         "RequireCheckIn": CreateRequireCheckInTypeDef,
@@ -2188,48 +2269,25 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoomSkillParameterResponseTypeDef = TypedDict(
     "GetRoomSkillParameterResponseTypeDef",
     {
-        "RoomSkillParameter": RoomSkillParameterTypeDef,
+        "RoomSkillParameter": RoomSkillParameterOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutRoomSkillParameterRequestRequestTypeDef = TypedDict(
-    "_RequiredPutRoomSkillParameterRequestRequestTypeDef",
-    {
-        "SkillId": str,
-        "RoomSkillParameter": RoomSkillParameterTypeDef,
-    },
-)
-_OptionalPutRoomSkillParameterRequestRequestTypeDef = TypedDict(
-    "_OptionalPutRoomSkillParameterRequestRequestTypeDef",
-    {
-        "RoomArn": str,
-    },
-    total=False,
-)
-
-
-class PutRoomSkillParameterRequestRequestTypeDef(
-    _RequiredPutRoomSkillParameterRequestRequestTypeDef,
-    _OptionalPutRoomSkillParameterRequestRequestTypeDef,
-):
-    pass
-
-
 ResolveRoomResponseTypeDef = TypedDict(
     "ResolveRoomResponseTypeDef",
     {
         "RoomArn": str,
         "RoomName": str,
-        "RoomSkillParameters": List[RoomSkillParameterTypeDef],
+        "RoomSkillParameters": List[RoomSkillParameterOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSkillGroupResponseTypeDef = TypedDict(
     "GetSkillGroupResponseTypeDef",
     {
@@ -2375,14 +2433,23 @@
     {
         "SmartHomeAppliances": List[SmartHomeApplianceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 MeetingRoomConfigurationTypeDef = TypedDict(
     "MeetingRoomConfigurationTypeDef",
     {
         "RoomUtilizationMetricsEnabled": bool,
         "EndOfMeetingReminder": EndOfMeetingReminderTypeDef,
         "InstantBooking": InstantBookingTypeDef,
         "RequireCheckIn": RequireCheckInTypeDef,
@@ -2407,14 +2474,37 @@
         "Profiles": List[ProfileDataTypeDef],
         "NextToken": str,
         "TotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPutRoomSkillParameterRequestRequestTypeDef = TypedDict(
+    "_RequiredPutRoomSkillParameterRequestRequestTypeDef",
+    {
+        "SkillId": str,
+        "RoomSkillParameter": RoomSkillParameterTypeDef,
+    },
+)
+_OptionalPutRoomSkillParameterRequestRequestTypeDef = TypedDict(
+    "_OptionalPutRoomSkillParameterRequestRequestTypeDef",
+    {
+        "RoomArn": str,
+    },
+    total=False,
+)
+
+
+class PutRoomSkillParameterRequestRequestTypeDef(
+    _RequiredPutRoomSkillParameterRequestRequestTypeDef,
+    _OptionalPutRoomSkillParameterRequestRequestTypeDef,
+):
+    pass
+
+
 SearchRoomsResponseTypeDef = TypedDict(
     "SearchRoomsResponseTypeDef",
     {
         "Rooms": List[RoomDataTypeDef],
         "NextToken": str,
         "TotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2595,16 +2685,16 @@
     "BusinessReportScheduleTypeDef",
     {
         "ScheduleArn": str,
         "ScheduleName": str,
         "S3BucketName": str,
         "S3KeyPrefix": str,
         "Format": BusinessReportFormatType,
-        "ContentRange": BusinessReportContentRangeTypeDef,
-        "Recurrence": BusinessReportRecurrenceTypeDef,
+        "ContentRange": BusinessReportContentRangeOutputTypeDef,
+        "Recurrence": BusinessReportRecurrenceOutputTypeDef,
         "LastBusinessReport": BusinessReportTypeDef,
     },
     total=False,
 )
 
 GetConferenceProviderResponseTypeDef = TypedDict(
     "GetConferenceProviderResponseTypeDef",
```

### Comparing `mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness/type_defs.pyi` & `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -58,28 +58,36 @@
     "AssociateContactWithAddressBookRequestRequestTypeDef",
     "AssociateDeviceWithNetworkProfileRequestRequestTypeDef",
     "AssociateDeviceWithRoomRequestRequestTypeDef",
     "AssociateSkillGroupWithRoomRequestRequestTypeDef",
     "AssociateSkillWithSkillGroupRequestRequestTypeDef",
     "AssociateSkillWithUsersRequestRequestTypeDef",
     "AudioTypeDef",
+    "BusinessReportContentRangeOutputTypeDef",
     "BusinessReportContentRangeTypeDef",
+    "BusinessReportRecurrenceOutputTypeDef",
     "BusinessReportRecurrenceTypeDef",
     "BusinessReportS3LocationTypeDef",
     "CategoryTypeDef",
+    "ConferencePreferenceOutputTypeDef",
     "ConferencePreferenceTypeDef",
+    "IPDialInOutputTypeDef",
+    "MeetingSettingOutputTypeDef",
+    "PSTNDialInOutputTypeDef",
+    "PhoneNumberOutputTypeDef",
+    "SipAddressOutputTypeDef",
+    "SsmlTypeDef",
+    "TextTypeDef",
+    "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "IPDialInTypeDef",
     "MeetingSettingTypeDef",
     "PSTNDialInTypeDef",
     "PhoneNumberTypeDef",
     "SipAddressTypeDef",
-    "SsmlTypeDef",
-    "TextTypeDef",
-    "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateEndOfMeetingReminderTypeDef",
     "CreateInstantBookingTypeDef",
     "CreateProactiveJoinTypeDef",
     "CreateRequireCheckInTypeDef",
     "DeleteAddressBookRequestRequestTypeDef",
     "DeleteBusinessReportScheduleRequestRequestTypeDef",
     "DeleteConferenceProviderRequestRequestTypeDef",
@@ -118,15 +126,15 @@
     "GetGatewayRequestRequestTypeDef",
     "GetNetworkProfileRequestRequestTypeDef",
     "NetworkProfileTypeDef",
     "GetProfileRequestRequestTypeDef",
     "GetRoomRequestRequestTypeDef",
     "RoomTypeDef",
     "GetRoomSkillParameterRequestRequestTypeDef",
-    "RoomSkillParameterTypeDef",
+    "RoomSkillParameterOutputTypeDef",
     "GetSkillGroupRequestRequestTypeDef",
     "SkillGroupTypeDef",
     "InstantBookingTypeDef",
     "PaginatorConfigTypeDef",
     "ListBusinessReportSchedulesRequestRequestTypeDef",
     "ListConferenceProvidersRequestRequestTypeDef",
     "ListDeviceEventsRequestRequestTypeDef",
@@ -135,19 +143,21 @@
     "ListSkillsRequestRequestTypeDef",
     "SkillSummaryTypeDef",
     "ListSkillsStoreCategoriesRequestRequestTypeDef",
     "ListSkillsStoreSkillsByCategoryRequestRequestTypeDef",
     "ListSmartHomeAppliancesRequestRequestTypeDef",
     "SmartHomeApplianceTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ProactiveJoinTypeDef",
     "RequireCheckInTypeDef",
     "NetworkProfileDataTypeDef",
     "ProfileDataTypeDef",
     "PutInvitationConfigurationRequestRequestTypeDef",
+    "RoomSkillParameterTypeDef",
     "PutSkillAuthorizationRequestRequestTypeDef",
     "RejectSkillRequestRequestTypeDef",
     "ResolveRoomRequestRequestTypeDef",
     "RevokeInvitationRequestRequestTypeDef",
     "RoomDataTypeDef",
     "SortTypeDef",
     "SkillGroupDataTypeDef",
@@ -167,23 +177,19 @@
     "UpdateNetworkProfileRequestRequestTypeDef",
     "UpdateRoomRequestRequestTypeDef",
     "UpdateSkillGroupRequestRequestTypeDef",
     "UpdateBusinessReportScheduleRequestRequestTypeDef",
     "BusinessReportTypeDef",
     "PutConferencePreferenceRequestRequestTypeDef",
     "ConferenceProviderTypeDef",
-    "UpdateConferenceProviderRequestRequestTypeDef",
     "ContactDataTypeDef",
     "ContactTypeDef",
-    "UpdateContactRequestRequestTypeDef",
     "ContentTypeDef",
     "CreateAddressBookRequestRequestTypeDef",
     "CreateBusinessReportScheduleRequestRequestTypeDef",
-    "CreateConferenceProviderRequestRequestTypeDef",
-    "CreateContactRequestRequestTypeDef",
     "CreateGatewayGroupRequestRequestTypeDef",
     "CreateNetworkProfileRequestRequestTypeDef",
     "CreateRoomRequestRequestTypeDef",
     "CreateSkillGroupRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "RegisterAVSDeviceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -197,45 +203,49 @@
     "CreateRoomResponseTypeDef",
     "CreateSkillGroupResponseTypeDef",
     "CreateUserResponseTypeDef",
     "GetAddressBookResponseTypeDef",
     "GetConferencePreferenceResponseTypeDef",
     "GetInvitationConfigurationResponseTypeDef",
     "ListSkillsStoreCategoriesResponseTypeDef",
-    "ListTagsResponseTypeDef",
     "RegisterAVSDeviceResponseTypeDef",
     "SearchAddressBooksResponseTypeDef",
     "SendAnnouncementResponseTypeDef",
+    "CreateConferenceProviderRequestRequestTypeDef",
+    "UpdateConferenceProviderRequestRequestTypeDef",
+    "CreateContactRequestRequestTypeDef",
+    "UpdateContactRequestRequestTypeDef",
     "CreateMeetingRoomConfigurationTypeDef",
     "SkillDetailsTypeDef",
     "ListDeviceEventsResponseTypeDef",
     "DeviceStatusInfoTypeDef",
     "ListGatewayGroupsResponseTypeDef",
     "GetGatewayGroupResponseTypeDef",
     "ListGatewaysResponseTypeDef",
     "GetGatewayResponseTypeDef",
     "GetNetworkProfileResponseTypeDef",
     "GetRoomResponseTypeDef",
     "GetRoomSkillParameterResponseTypeDef",
-    "PutRoomSkillParameterRequestRequestTypeDef",
     "ResolveRoomResponseTypeDef",
     "GetSkillGroupResponseTypeDef",
     "ListBusinessReportSchedulesRequestListBusinessReportSchedulesPaginateTypeDef",
     "ListConferenceProvidersRequestListConferenceProvidersPaginateTypeDef",
     "ListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
     "ListSkillsRequestListSkillsPaginateTypeDef",
     "ListSkillsStoreCategoriesRequestListSkillsStoreCategoriesPaginateTypeDef",
     "ListSkillsStoreSkillsByCategoryRequestListSkillsStoreSkillsByCategoryPaginateTypeDef",
     "ListSmartHomeAppliancesRequestListSmartHomeAppliancesPaginateTypeDef",
     "ListTagsRequestListTagsPaginateTypeDef",
     "ListSkillsResponseTypeDef",
     "ListSmartHomeAppliancesResponseTypeDef",
+    "ListTagsResponseTypeDef",
     "MeetingRoomConfigurationTypeDef",
     "SearchNetworkProfilesResponseTypeDef",
     "SearchProfilesResponseTypeDef",
+    "PutRoomSkillParameterRequestRequestTypeDef",
     "SearchRoomsResponseTypeDef",
     "SearchAddressBooksRequestRequestTypeDef",
     "SearchContactsRequestRequestTypeDef",
     "SearchDevicesRequestRequestTypeDef",
     "SearchDevicesRequestSearchDevicesPaginateTypeDef",
     "SearchNetworkProfilesRequestRequestTypeDef",
     "SearchProfilesRequestRequestTypeDef",
@@ -360,21 +370,36 @@
     "AudioTypeDef",
     {
         "Locale": Literal["en-US"],
         "Location": str,
     },
 )
 
+BusinessReportContentRangeOutputTypeDef = TypedDict(
+    "BusinessReportContentRangeOutputTypeDef",
+    {
+        "Interval": BusinessReportIntervalType,
+    },
+)
+
 BusinessReportContentRangeTypeDef = TypedDict(
     "BusinessReportContentRangeTypeDef",
     {
         "Interval": BusinessReportIntervalType,
     },
 )
 
+BusinessReportRecurrenceOutputTypeDef = TypedDict(
+    "BusinessReportRecurrenceOutputTypeDef",
+    {
+        "StartDate": str,
+    },
+    total=False,
+)
+
 BusinessReportRecurrenceTypeDef = TypedDict(
     "BusinessReportRecurrenceTypeDef",
     {
         "StartDate": str,
     },
     total=False,
 )
@@ -393,57 +418,65 @@
     {
         "CategoryId": int,
         "CategoryName": str,
     },
     total=False,
 )
 
+ConferencePreferenceOutputTypeDef = TypedDict(
+    "ConferencePreferenceOutputTypeDef",
+    {
+        "DefaultConferenceProviderArn": str,
+    },
+    total=False,
+)
+
 ConferencePreferenceTypeDef = TypedDict(
     "ConferencePreferenceTypeDef",
     {
         "DefaultConferenceProviderArn": str,
     },
     total=False,
 )
 
-IPDialInTypeDef = TypedDict(
-    "IPDialInTypeDef",
+IPDialInOutputTypeDef = TypedDict(
+    "IPDialInOutputTypeDef",
     {
         "Endpoint": str,
         "CommsProtocol": CommsProtocolType,
     },
 )
 
-MeetingSettingTypeDef = TypedDict(
-    "MeetingSettingTypeDef",
+MeetingSettingOutputTypeDef = TypedDict(
+    "MeetingSettingOutputTypeDef",
     {
         "RequirePin": RequirePinType,
     },
 )
 
-PSTNDialInTypeDef = TypedDict(
-    "PSTNDialInTypeDef",
+PSTNDialInOutputTypeDef = TypedDict(
+    "PSTNDialInOutputTypeDef",
     {
         "CountryCode": str,
         "PhoneNumber": str,
         "OneClickIdDelay": str,
         "OneClickPinDelay": str,
     },
 )
 
-PhoneNumberTypeDef = TypedDict(
-    "PhoneNumberTypeDef",
+PhoneNumberOutputTypeDef = TypedDict(
+    "PhoneNumberOutputTypeDef",
     {
         "Number": str,
         "Type": PhoneNumberTypeType,
     },
 )
 
-SipAddressTypeDef = TypedDict(
-    "SipAddressTypeDef",
+SipAddressOutputTypeDef = TypedDict(
+    "SipAddressOutputTypeDef",
     {
         "Uri": str,
         "Type": Literal["WORK"],
     },
 )
 
 SsmlTypeDef = TypedDict(
@@ -477,14 +510,55 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+IPDialInTypeDef = TypedDict(
+    "IPDialInTypeDef",
+    {
+        "Endpoint": str,
+        "CommsProtocol": CommsProtocolType,
+    },
+)
+
+MeetingSettingTypeDef = TypedDict(
+    "MeetingSettingTypeDef",
+    {
+        "RequirePin": RequirePinType,
+    },
+)
+
+PSTNDialInTypeDef = TypedDict(
+    "PSTNDialInTypeDef",
+    {
+        "CountryCode": str,
+        "PhoneNumber": str,
+        "OneClickIdDelay": str,
+        "OneClickPinDelay": str,
+    },
+)
+
+PhoneNumberTypeDef = TypedDict(
+    "PhoneNumberTypeDef",
+    {
+        "Number": str,
+        "Type": PhoneNumberTypeType,
+    },
+)
+
+SipAddressTypeDef = TypedDict(
+    "SipAddressTypeDef",
+    {
+        "Uri": str,
+        "Type": Literal["WORK"],
+    },
+)
+
 CreateEndOfMeetingReminderTypeDef = TypedDict(
     "CreateEndOfMeetingReminderTypeDef",
     {
         "ReminderAtMinutes": Sequence[int],
         "ReminderType": EndOfMeetingReminderTypeType,
         "Enabled": bool,
     },
@@ -927,16 +1001,16 @@
 
 class GetRoomSkillParameterRequestRequestTypeDef(
     _RequiredGetRoomSkillParameterRequestRequestTypeDef,
     _OptionalGetRoomSkillParameterRequestRequestTypeDef,
 ):
     pass
 
-RoomSkillParameterTypeDef = TypedDict(
-    "RoomSkillParameterTypeDef",
+RoomSkillParameterOutputTypeDef = TypedDict(
+    "RoomSkillParameterOutputTypeDef",
     {
         "ParameterKey": str,
         "ParameterValue": str,
     },
 )
 
 GetSkillGroupRequestRequestTypeDef = TypedDict(
@@ -1135,14 +1209,22 @@
 )
 
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 ProactiveJoinTypeDef = TypedDict(
     "ProactiveJoinTypeDef",
     {
         "EnabledByMotion": bool,
     },
     total=False,
 )
@@ -1203,14 +1285,22 @@
 
 class PutInvitationConfigurationRequestRequestTypeDef(
     _RequiredPutInvitationConfigurationRequestRequestTypeDef,
     _OptionalPutInvitationConfigurationRequestRequestTypeDef,
 ):
     pass
 
+RoomSkillParameterTypeDef = TypedDict(
+    "RoomSkillParameterTypeDef",
+    {
+        "ParameterKey": str,
+        "ParameterValue": str,
+    },
+)
+
 _RequiredPutSkillAuthorizationRequestRequestTypeDef = TypedDict(
     "_RequiredPutSkillAuthorizationRequestRequestTypeDef",
     {
         "AuthorizationResult": Mapping[str, str],
         "SkillId": str,
     },
 )
@@ -1537,96 +1627,49 @@
 
 ConferenceProviderTypeDef = TypedDict(
     "ConferenceProviderTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Type": ConferenceProviderTypeType,
-        "IPDialIn": IPDialInTypeDef,
-        "PSTNDialIn": PSTNDialInTypeDef,
-        "MeetingSetting": MeetingSettingTypeDef,
-    },
-    total=False,
-)
-
-_RequiredUpdateConferenceProviderRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateConferenceProviderRequestRequestTypeDef",
-    {
-        "ConferenceProviderArn": str,
-        "ConferenceProviderType": ConferenceProviderTypeType,
-        "MeetingSetting": MeetingSettingTypeDef,
-    },
-)
-_OptionalUpdateConferenceProviderRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateConferenceProviderRequestRequestTypeDef",
-    {
-        "IPDialIn": IPDialInTypeDef,
-        "PSTNDialIn": PSTNDialInTypeDef,
+        "IPDialIn": IPDialInOutputTypeDef,
+        "PSTNDialIn": PSTNDialInOutputTypeDef,
+        "MeetingSetting": MeetingSettingOutputTypeDef,
     },
     total=False,
 )
 
-class UpdateConferenceProviderRequestRequestTypeDef(
-    _RequiredUpdateConferenceProviderRequestRequestTypeDef,
-    _OptionalUpdateConferenceProviderRequestRequestTypeDef,
-):
-    pass
-
 ContactDataTypeDef = TypedDict(
     "ContactDataTypeDef",
     {
         "ContactArn": str,
         "DisplayName": str,
         "FirstName": str,
         "LastName": str,
         "PhoneNumber": str,
-        "PhoneNumbers": List[PhoneNumberTypeDef],
-        "SipAddresses": List[SipAddressTypeDef],
+        "PhoneNumbers": List[PhoneNumberOutputTypeDef],
+        "SipAddresses": List[SipAddressOutputTypeDef],
     },
     total=False,
 )
 
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "ContactArn": str,
         "DisplayName": str,
         "FirstName": str,
         "LastName": str,
         "PhoneNumber": str,
-        "PhoneNumbers": List[PhoneNumberTypeDef],
-        "SipAddresses": List[SipAddressTypeDef],
+        "PhoneNumbers": List[PhoneNumberOutputTypeDef],
+        "SipAddresses": List[SipAddressOutputTypeDef],
     },
     total=False,
 )
 
-_RequiredUpdateContactRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateContactRequestRequestTypeDef",
-    {
-        "ContactArn": str,
-    },
-)
-_OptionalUpdateContactRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateContactRequestRequestTypeDef",
-    {
-        "DisplayName": str,
-        "FirstName": str,
-        "LastName": str,
-        "PhoneNumber": str,
-        "PhoneNumbers": Sequence[PhoneNumberTypeDef],
-        "SipAddresses": Sequence[SipAddressTypeDef],
-    },
-    total=False,
-)
-
-class UpdateContactRequestRequestTypeDef(
-    _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
-):
-    pass
-
 ContentTypeDef = TypedDict(
     "ContentTypeDef",
     {
         "TextList": Sequence[TextTypeDef],
         "SsmlList": Sequence[SsmlTypeDef],
         "AudioList": Sequence[AudioTypeDef],
     },
@@ -1676,64 +1719,14 @@
 
 class CreateBusinessReportScheduleRequestRequestTypeDef(
     _RequiredCreateBusinessReportScheduleRequestRequestTypeDef,
     _OptionalCreateBusinessReportScheduleRequestRequestTypeDef,
 ):
     pass
 
-_RequiredCreateConferenceProviderRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateConferenceProviderRequestRequestTypeDef",
-    {
-        "ConferenceProviderName": str,
-        "ConferenceProviderType": ConferenceProviderTypeType,
-        "MeetingSetting": MeetingSettingTypeDef,
-    },
-)
-_OptionalCreateConferenceProviderRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateConferenceProviderRequestRequestTypeDef",
-    {
-        "IPDialIn": IPDialInTypeDef,
-        "PSTNDialIn": PSTNDialInTypeDef,
-        "ClientRequestToken": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateConferenceProviderRequestRequestTypeDef(
-    _RequiredCreateConferenceProviderRequestRequestTypeDef,
-    _OptionalCreateConferenceProviderRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateContactRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateContactRequestRequestTypeDef",
-    {
-        "FirstName": str,
-    },
-)
-_OptionalCreateContactRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateContactRequestRequestTypeDef",
-    {
-        "DisplayName": str,
-        "LastName": str,
-        "PhoneNumber": str,
-        "PhoneNumbers": Sequence[PhoneNumberTypeDef],
-        "SipAddresses": Sequence[SipAddressTypeDef],
-        "ClientRequestToken": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateContactRequestRequestTypeDef(
-    _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
-):
-    pass
-
 _RequiredCreateGatewayGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGatewayGroupRequestRequestTypeDef",
     {
         "Name": str,
         "ClientRequestToken": str,
     },
 )
@@ -1967,15 +1960,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConferencePreferenceResponseTypeDef = TypedDict(
     "GetConferencePreferenceResponseTypeDef",
     {
-        "Preference": ConferencePreferenceTypeDef,
+        "Preference": ConferencePreferenceOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInvitationConfigurationResponseTypeDef = TypedDict(
     "GetInvitationConfigurationResponseTypeDef",
     {
@@ -1991,23 +1984,14 @@
     {
         "CategoryList": List[CategoryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 RegisterAVSDeviceResponseTypeDef = TypedDict(
     "RegisterAVSDeviceResponseTypeDef",
     {
         "DeviceArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2026,14 +2010,111 @@
     "SendAnnouncementResponseTypeDef",
     {
         "AnnouncementArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateConferenceProviderRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateConferenceProviderRequestRequestTypeDef",
+    {
+        "ConferenceProviderName": str,
+        "ConferenceProviderType": ConferenceProviderTypeType,
+        "MeetingSetting": MeetingSettingTypeDef,
+    },
+)
+_OptionalCreateConferenceProviderRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateConferenceProviderRequestRequestTypeDef",
+    {
+        "IPDialIn": IPDialInTypeDef,
+        "PSTNDialIn": PSTNDialInTypeDef,
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateConferenceProviderRequestRequestTypeDef(
+    _RequiredCreateConferenceProviderRequestRequestTypeDef,
+    _OptionalCreateConferenceProviderRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateConferenceProviderRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateConferenceProviderRequestRequestTypeDef",
+    {
+        "ConferenceProviderArn": str,
+        "ConferenceProviderType": ConferenceProviderTypeType,
+        "MeetingSetting": MeetingSettingTypeDef,
+    },
+)
+_OptionalUpdateConferenceProviderRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateConferenceProviderRequestRequestTypeDef",
+    {
+        "IPDialIn": IPDialInTypeDef,
+        "PSTNDialIn": PSTNDialInTypeDef,
+    },
+    total=False,
+)
+
+class UpdateConferenceProviderRequestRequestTypeDef(
+    _RequiredUpdateConferenceProviderRequestRequestTypeDef,
+    _OptionalUpdateConferenceProviderRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateContactRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateContactRequestRequestTypeDef",
+    {
+        "FirstName": str,
+    },
+)
+_OptionalCreateContactRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateContactRequestRequestTypeDef",
+    {
+        "DisplayName": str,
+        "LastName": str,
+        "PhoneNumber": str,
+        "PhoneNumbers": Sequence[PhoneNumberTypeDef],
+        "SipAddresses": Sequence[SipAddressTypeDef],
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateContactRequestRequestTypeDef(
+    _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateContactRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateContactRequestRequestTypeDef",
+    {
+        "ContactArn": str,
+    },
+)
+_OptionalUpdateContactRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateContactRequestRequestTypeDef",
+    {
+        "DisplayName": str,
+        "FirstName": str,
+        "LastName": str,
+        "PhoneNumber": str,
+        "PhoneNumbers": Sequence[PhoneNumberTypeDef],
+        "SipAddresses": Sequence[SipAddressTypeDef],
+    },
+    total=False,
+)
+
+class UpdateContactRequestRequestTypeDef(
+    _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
+):
+    pass
+
 CreateMeetingRoomConfigurationTypeDef = TypedDict(
     "CreateMeetingRoomConfigurationTypeDef",
     {
         "RoomUtilizationMetricsEnabled": bool,
         "EndOfMeetingReminder": CreateEndOfMeetingReminderTypeDef,
         "InstantBooking": CreateInstantBookingTypeDef,
         "RequireCheckIn": CreateRequireCheckInTypeDef,
@@ -2127,46 +2208,25 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoomSkillParameterResponseTypeDef = TypedDict(
     "GetRoomSkillParameterResponseTypeDef",
     {
-        "RoomSkillParameter": RoomSkillParameterTypeDef,
+        "RoomSkillParameter": RoomSkillParameterOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutRoomSkillParameterRequestRequestTypeDef = TypedDict(
-    "_RequiredPutRoomSkillParameterRequestRequestTypeDef",
-    {
-        "SkillId": str,
-        "RoomSkillParameter": RoomSkillParameterTypeDef,
-    },
-)
-_OptionalPutRoomSkillParameterRequestRequestTypeDef = TypedDict(
-    "_OptionalPutRoomSkillParameterRequestRequestTypeDef",
-    {
-        "RoomArn": str,
-    },
-    total=False,
-)
-
-class PutRoomSkillParameterRequestRequestTypeDef(
-    _RequiredPutRoomSkillParameterRequestRequestTypeDef,
-    _OptionalPutRoomSkillParameterRequestRequestTypeDef,
-):
-    pass
-
 ResolveRoomResponseTypeDef = TypedDict(
     "ResolveRoomResponseTypeDef",
     {
         "RoomArn": str,
         "RoomName": str,
-        "RoomSkillParameters": List[RoomSkillParameterTypeDef],
+        "RoomSkillParameters": List[RoomSkillParameterOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSkillGroupResponseTypeDef = TypedDict(
     "GetSkillGroupResponseTypeDef",
     {
@@ -2304,14 +2364,23 @@
     {
         "SmartHomeAppliances": List[SmartHomeApplianceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 MeetingRoomConfigurationTypeDef = TypedDict(
     "MeetingRoomConfigurationTypeDef",
     {
         "RoomUtilizationMetricsEnabled": bool,
         "EndOfMeetingReminder": EndOfMeetingReminderTypeDef,
         "InstantBooking": InstantBookingTypeDef,
         "RequireCheckIn": RequireCheckInTypeDef,
@@ -2336,14 +2405,35 @@
         "Profiles": List[ProfileDataTypeDef],
         "NextToken": str,
         "TotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPutRoomSkillParameterRequestRequestTypeDef = TypedDict(
+    "_RequiredPutRoomSkillParameterRequestRequestTypeDef",
+    {
+        "SkillId": str,
+        "RoomSkillParameter": RoomSkillParameterTypeDef,
+    },
+)
+_OptionalPutRoomSkillParameterRequestRequestTypeDef = TypedDict(
+    "_OptionalPutRoomSkillParameterRequestRequestTypeDef",
+    {
+        "RoomArn": str,
+    },
+    total=False,
+)
+
+class PutRoomSkillParameterRequestRequestTypeDef(
+    _RequiredPutRoomSkillParameterRequestRequestTypeDef,
+    _OptionalPutRoomSkillParameterRequestRequestTypeDef,
+):
+    pass
+
 SearchRoomsResponseTypeDef = TypedDict(
     "SearchRoomsResponseTypeDef",
     {
         "Rooms": List[RoomDataTypeDef],
         "NextToken": str,
         "TotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2524,16 +2614,16 @@
     "BusinessReportScheduleTypeDef",
     {
         "ScheduleArn": str,
         "ScheduleName": str,
         "S3BucketName": str,
         "S3KeyPrefix": str,
         "Format": BusinessReportFormatType,
-        "ContentRange": BusinessReportContentRangeTypeDef,
-        "Recurrence": BusinessReportRecurrenceTypeDef,
+        "ContentRange": BusinessReportContentRangeOutputTypeDef,
+        "Recurrence": BusinessReportRecurrenceOutputTypeDef,
         "LastBusinessReport": BusinessReportTypeDef,
     },
     total=False,
 )
 
 GetConferenceProviderResponseTypeDef = TypedDict(
     "GetConferenceProviderResponseTypeDef",
```

### Comparing `mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness.egg-info/PKG-INFO` & `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-alexaforbusiness
-Version: 1.28.0
-Summary: Type annotations for boto3.AlexaForBusiness 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AlexaForBusiness 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-alexaforbusiness"></a>
 
 # mypy-boto3-alexaforbusiness
 
 [![PyPI - mypy-boto3-alexaforbusiness](https://img.shields.io/pypi/v/mypy-boto3-alexaforbusiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-alexaforbusiness)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-alexaforbusiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-alexaforbusiness)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-alexaforbusiness?color=blue)](https://pypistats.org/packages/mypy-boto3-alexaforbusiness)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-alexaforbusiness)](https://pepy.tech/project/mypy-boto3-alexaforbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AlexaForBusiness 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
+[boto3.AlexaForBusiness 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
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
 [mypy-boto3-alexaforbusiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/).
 
 See how it helps to find and fix potential bugs:
 
@@ -408,28 +408,36 @@
     AssociateContactWithAddressBookRequestRequestTypeDef,
     AssociateDeviceWithNetworkProfileRequestRequestTypeDef,
     AssociateDeviceWithRoomRequestRequestTypeDef,
     AssociateSkillGroupWithRoomRequestRequestTypeDef,
     AssociateSkillWithSkillGroupRequestRequestTypeDef,
     AssociateSkillWithUsersRequestRequestTypeDef,
     AudioTypeDef,
+    BusinessReportContentRangeOutputTypeDef,
     BusinessReportContentRangeTypeDef,
+    BusinessReportRecurrenceOutputTypeDef,
     BusinessReportRecurrenceTypeDef,
     BusinessReportS3LocationTypeDef,
     CategoryTypeDef,
+    ConferencePreferenceOutputTypeDef,
     ConferencePreferenceTypeDef,
+    IPDialInOutputTypeDef,
+    MeetingSettingOutputTypeDef,
+    PSTNDialInOutputTypeDef,
+    PhoneNumberOutputTypeDef,
+    SipAddressOutputTypeDef,
+    SsmlTypeDef,
+    TextTypeDef,
+    TagTypeDef,
+    ResponseMetadataTypeDef,
     IPDialInTypeDef,
     MeetingSettingTypeDef,
     PSTNDialInTypeDef,
     PhoneNumberTypeDef,
     SipAddressTypeDef,
-    SsmlTypeDef,
-    TextTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
     CreateEndOfMeetingReminderTypeDef,
     CreateInstantBookingTypeDef,
     CreateProactiveJoinTypeDef,
     CreateRequireCheckInTypeDef,
     DeleteAddressBookRequestRequestTypeDef,
     DeleteBusinessReportScheduleRequestRequestTypeDef,
     DeleteConferenceProviderRequestRequestTypeDef,
@@ -468,15 +476,15 @@
     GetGatewayRequestRequestTypeDef,
     GetNetworkProfileRequestRequestTypeDef,
     NetworkProfileTypeDef,
     GetProfileRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     RoomTypeDef,
     GetRoomSkillParameterRequestRequestTypeDef,
-    RoomSkillParameterTypeDef,
+    RoomSkillParameterOutputTypeDef,
     GetSkillGroupRequestRequestTypeDef,
     SkillGroupTypeDef,
     InstantBookingTypeDef,
     PaginatorConfigTypeDef,
     ListBusinessReportSchedulesRequestRequestTypeDef,
     ListConferenceProvidersRequestRequestTypeDef,
     ListDeviceEventsRequestRequestTypeDef,
@@ -485,19 +493,21 @@
     ListSkillsRequestRequestTypeDef,
     SkillSummaryTypeDef,
     ListSkillsStoreCategoriesRequestRequestTypeDef,
     ListSkillsStoreSkillsByCategoryRequestRequestTypeDef,
     ListSmartHomeAppliancesRequestRequestTypeDef,
     SmartHomeApplianceTypeDef,
     ListTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     ProactiveJoinTypeDef,
     RequireCheckInTypeDef,
     NetworkProfileDataTypeDef,
     ProfileDataTypeDef,
     PutInvitationConfigurationRequestRequestTypeDef,
+    RoomSkillParameterTypeDef,
     PutSkillAuthorizationRequestRequestTypeDef,
     RejectSkillRequestRequestTypeDef,
     ResolveRoomRequestRequestTypeDef,
     RevokeInvitationRequestRequestTypeDef,
     RoomDataTypeDef,
     SortTypeDef,
     SkillGroupDataTypeDef,
@@ -517,23 +527,19 @@
     UpdateNetworkProfileRequestRequestTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateSkillGroupRequestRequestTypeDef,
     UpdateBusinessReportScheduleRequestRequestTypeDef,
     BusinessReportTypeDef,
     PutConferencePreferenceRequestRequestTypeDef,
     ConferenceProviderTypeDef,
-    UpdateConferenceProviderRequestRequestTypeDef,
     ContactDataTypeDef,
     ContactTypeDef,
-    UpdateContactRequestRequestTypeDef,
     ContentTypeDef,
     CreateAddressBookRequestRequestTypeDef,
     CreateBusinessReportScheduleRequestRequestTypeDef,
-    CreateConferenceProviderRequestRequestTypeDef,
-    CreateContactRequestRequestTypeDef,
     CreateGatewayGroupRequestRequestTypeDef,
     CreateNetworkProfileRequestRequestTypeDef,
     CreateRoomRequestRequestTypeDef,
     CreateSkillGroupRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     RegisterAVSDeviceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -547,45 +553,49 @@
     CreateRoomResponseTypeDef,
     CreateSkillGroupResponseTypeDef,
     CreateUserResponseTypeDef,
     GetAddressBookResponseTypeDef,
     GetConferencePreferenceResponseTypeDef,
     GetInvitationConfigurationResponseTypeDef,
     ListSkillsStoreCategoriesResponseTypeDef,
-    ListTagsResponseTypeDef,
     RegisterAVSDeviceResponseTypeDef,
     SearchAddressBooksResponseTypeDef,
     SendAnnouncementResponseTypeDef,
+    CreateConferenceProviderRequestRequestTypeDef,
+    UpdateConferenceProviderRequestRequestTypeDef,
+    CreateContactRequestRequestTypeDef,
+    UpdateContactRequestRequestTypeDef,
     CreateMeetingRoomConfigurationTypeDef,
     SkillDetailsTypeDef,
     ListDeviceEventsResponseTypeDef,
     DeviceStatusInfoTypeDef,
     ListGatewayGroupsResponseTypeDef,
     GetGatewayGroupResponseTypeDef,
     ListGatewaysResponseTypeDef,
     GetGatewayResponseTypeDef,
     GetNetworkProfileResponseTypeDef,
     GetRoomResponseTypeDef,
     GetRoomSkillParameterResponseTypeDef,
-    PutRoomSkillParameterRequestRequestTypeDef,
     ResolveRoomResponseTypeDef,
     GetSkillGroupResponseTypeDef,
     ListBusinessReportSchedulesRequestListBusinessReportSchedulesPaginateTypeDef,
     ListConferenceProvidersRequestListConferenceProvidersPaginateTypeDef,
     ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
     ListSkillsRequestListSkillsPaginateTypeDef,
     ListSkillsStoreCategoriesRequestListSkillsStoreCategoriesPaginateTypeDef,
     ListSkillsStoreSkillsByCategoryRequestListSkillsStoreSkillsByCategoryPaginateTypeDef,
     ListSmartHomeAppliancesRequestListSmartHomeAppliancesPaginateTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
     ListSkillsResponseTypeDef,
     ListSmartHomeAppliancesResponseTypeDef,
+    ListTagsResponseTypeDef,
     MeetingRoomConfigurationTypeDef,
     SearchNetworkProfilesResponseTypeDef,
     SearchProfilesResponseTypeDef,
+    PutRoomSkillParameterRequestRequestTypeDef,
     SearchRoomsResponseTypeDef,
     SearchAddressBooksRequestRequestTypeDef,
     SearchContactsRequestRequestTypeDef,
     SearchDevicesRequestRequestTypeDef,
     SearchDevicesRequestSearchDevicesPaginateTypeDef,
     SearchNetworkProfilesRequestRequestTypeDef,
     SearchProfilesRequestRequestTypeDef,
```

### Comparing `mypy-boto3-alexaforbusiness-1.28.0/mypy_boto3_alexaforbusiness.egg-info/SOURCES.txt` & `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.28.0/setup.py` & `mypy-boto3-alexaforbusiness-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-alexaforbusiness",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_alexaforbusiness"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AlexaForBusiness 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.AlexaForBusiness 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

