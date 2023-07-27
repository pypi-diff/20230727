# Comparing `tmp/mypy-boto3-ssm-contacts-1.28.0.tar.gz` & `tmp/mypy-boto3-ssm-contacts-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ssm-contacts-1.28.0.tar", last modified: Thu Jul  6 21:00:42 2023, max compression
+gzip compressed data, was "mypy-boto3-ssm-contacts-1.28.12.tar", last modified: Thu Jul 27 11:49:41 2023, max compression
```

## Comparing `mypy-boto3-ssm-contacts-1.28.0.tar` & `mypy-boto3-ssm-contacts-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:42.270441 mypy-boto3-ssm-contacts-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:56:32.000000 mypy-boto3-ssm-contacts-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-07-06 21:00:42.266440 mypy-boto3-ssm-contacts-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-07-06 20:56:32.000000 mypy-boto3-ssm-contacts-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:42.262441 mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-06 20:56:32.000000 mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-06 20:56:32.000000 mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-06 20:56:32.000000 mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32233 2023-07-06 20:56:32.000000 mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-07-06 20:56:32.000000 mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-07-06 20:56:32.000000 mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-07-06 20:56:32.000000 mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-07-06 20:56:32.000000 mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-07-06 20:56:32.000000 mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:56:32.000000 mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39505 2023-07-06 20:56:33.000000 mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39430 2023-07-06 20:56:33.000000 mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:56:32.000000 mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:42.266440 mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-07-06 21:00:41.000000 mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 21:00:42.000000 mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:41.000000 mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:41.000000 mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:41.000000 mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 21:00:41.000000 mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:42.270441 mypy-boto3-ssm-contacts-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-06 20:56:31.000000 mypy-boto3-ssm-contacts-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.665320 mypy-boto3-ssm-contacts-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19024 2023-07-27 11:49:41.657320 mypy-boto3-ssm-contacts-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17518 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.657320 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32233 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-07-27 11:47:29.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-07-27 11:47:29.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13820 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42975 2023-07-27 11:47:30.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42894 2023-07-27 11:47:29.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.657320 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19024 2023-07-27 11:49:41.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 11:49:41.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:41.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:41.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:41.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 11:49:41.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:41.665320 mypy-boto3-ssm-contacts-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/setup.py
```

### Comparing `mypy-boto3-ssm-contacts-1.28.0/LICENSE` & `mypy-boto3-ssm-contacts-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.0/PKG-INFO` & `mypy-boto3-ssm-contacts-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-contacts
-Version: 1.28.0
-Summary: Type annotations for boto3.SSMContacts 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SSMContacts 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ssm-contacts"></a>
 
 # mypy-boto3-ssm-contacts
 
 [![PyPI - mypy-boto3-ssm-contacts](https://img.shields.io/pypi/v/mypy-boto3-ssm-contacts.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-contacts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-contacts.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-contacts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm-contacts?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm-contacts)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-contacts)](https://pepy.tech/project/mypy-boto3-ssm-contacts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMContacts 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
+[boto3.SSMContacts 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
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
 [mypy-boto3-ssm-contacts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -375,110 +375,122 @@
 `mypy_boto3_ssm_contacts.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ssm_contacts.type_defs import (
     AcceptPageRequestRequestTypeDef,
     ActivateContactChannelRequestRequestTypeDef,
+    ChannelTargetInfoOutputTypeDef,
     ChannelTargetInfoTypeDef,
+    ContactChannelAddressOutputTypeDef,
     ContactChannelAddressTypeDef,
+    ContactTargetInfoOutputTypeDef,
     ContactTargetInfoTypeDef,
     ContactTypeDef,
+    HandOffTimeOutputTypeDef,
     HandOffTimeTypeDef,
-    CreateContactChannelResultTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
-    CreateContactResultTypeDef,
     CreateRotationOverrideRequestRequestTypeDef,
-    CreateRotationOverrideResultTypeDef,
-    CreateRotationResultTypeDef,
     DeactivateContactChannelRequestRequestTypeDef,
     DeleteContactChannelRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
     DeleteRotationOverrideRequestRequestTypeDef,
     DeleteRotationRequestRequestTypeDef,
     DescribeEngagementRequestRequestTypeDef,
-    DescribeEngagementResultTypeDef,
     DescribePageRequestRequestTypeDef,
-    DescribePageResultTypeDef,
     EngagementTypeDef,
     GetContactChannelRequestRequestTypeDef,
     GetContactPolicyRequestRequestTypeDef,
-    GetContactPolicyResultTypeDef,
     GetContactRequestRequestTypeDef,
     GetRotationOverrideRequestRequestTypeDef,
-    GetRotationOverrideResultTypeDef,
     GetRotationRequestRequestTypeDef,
-    ListContactChannelsRequestListContactChannelsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListContactChannelsRequestRequestTypeDef,
-    ListContactsRequestListContactsPaginateTypeDef,
     ListContactsRequestRequestTypeDef,
     TimeRangeTypeDef,
-    ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
     ListPageReceiptsRequestRequestTypeDef,
     ReceiptTypeDef,
-    ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
     ListPageResolutionsRequestRequestTypeDef,
     ResolutionContactTypeDef,
-    ListPagesByContactRequestListPagesByContactPaginateTypeDef,
     ListPagesByContactRequestRequestTypeDef,
     PageTypeDef,
-    ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
     ListPagesByEngagementRequestRequestTypeDef,
     PreviewOverrideTypeDef,
-    ListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
     ListRotationOverridesRequestRequestTypeDef,
     RotationOverrideTypeDef,
-    ListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
     ListRotationShiftsRequestRequestTypeDef,
-    ListRotationsRequestListRotationsPaginateTypeDef,
     ListRotationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     PutContactPolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ShiftDetailsTypeDef,
     SendActivationCodeRequestRequestTypeDef,
     StartEngagementRequestRequestTypeDef,
-    StartEngagementResultTypeDef,
     StopEngagementRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ContactChannelTypeDef,
     CreateContactChannelRequestRequestTypeDef,
-    GetContactChannelResultTypeDef,
     UpdateContactChannelRequestRequestTypeDef,
+    TargetOutputTypeDef,
     TargetTypeDef,
-    ListContactsResultTypeDef,
+    CoverageTimeOutputTypeDef,
+    MonthlySettingOutputTypeDef,
+    WeeklySettingOutputTypeDef,
     CoverageTimeTypeDef,
     MonthlySettingTypeDef,
     WeeklySettingTypeDef,
-    ListTagsForResourceResultTypeDef,
+    CreateContactChannelResultTypeDef,
+    CreateContactResultTypeDef,
+    CreateRotationOverrideResultTypeDef,
+    CreateRotationResultTypeDef,
+    DescribeEngagementResultTypeDef,
+    DescribePageResultTypeDef,
+    GetContactChannelResultTypeDef,
+    GetContactPolicyResultTypeDef,
+    GetRotationOverrideResultTypeDef,
+    ListContactsResultTypeDef,
+    StartEngagementResultTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEngagementsResultTypeDef,
+    ListContactChannelsRequestListContactChannelsPaginateTypeDef,
+    ListContactsRequestListContactsPaginateTypeDef,
+    ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
+    ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
+    ListPagesByContactRequestListPagesByContactPaginateTypeDef,
+    ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
+    ListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
+    ListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
+    ListRotationsRequestListRotationsPaginateTypeDef,
     ListEngagementsRequestListEngagementsPaginateTypeDef,
     ListEngagementsRequestRequestTypeDef,
     ListPageReceiptsResultTypeDef,
     ListPageResolutionsResultTypeDef,
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListRotationOverridesResultTypeDef,
+    ListTagsForResourceResultTypeDef,
     RotationShiftTypeDef,
     ListContactChannelsResultTypeDef,
+    StageOutputTypeDef,
     StageTypeDef,
+    RecurrenceSettingsOutputTypeDef,
     RecurrenceSettingsTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationShiftsResultTypeDef,
+    PlanOutputTypeDef,
     PlanTypeDef,
-    CreateRotationRequestRequestTypeDef,
     GetRotationResultTypeDef,
+    RotationTypeDef,
+    CreateRotationRequestRequestTypeDef,
     ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef,
     ListPreviewRotationShiftsRequestRequestTypeDef,
-    RotationTypeDef,
     UpdateRotationRequestRequestTypeDef,
-    CreateContactRequestRequestTypeDef,
     GetContactResultTypeDef,
+    CreateContactRequestRequestTypeDef,
     UpdateContactRequestRequestTypeDef,
     ListRotationsResultTypeDef,
 )
 
 
 def get_structure() -> AcceptPageRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-ssm-contacts-1.28.0/README.md` & `mypy-boto3-ssm-contacts-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ssm-contacts"></a>
 
 # mypy-boto3-ssm-contacts
 
 [![PyPI - mypy-boto3-ssm-contacts](https://img.shields.io/pypi/v/mypy-boto3-ssm-contacts.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-contacts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-contacts.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-contacts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm-contacts?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm-contacts)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-contacts)](https://pepy.tech/project/mypy-boto3-ssm-contacts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMContacts 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
+[boto3.SSMContacts 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
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
 [mypy-boto3-ssm-contacts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,110 +343,122 @@
 `mypy_boto3_ssm_contacts.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ssm_contacts.type_defs import (
     AcceptPageRequestRequestTypeDef,
     ActivateContactChannelRequestRequestTypeDef,
+    ChannelTargetInfoOutputTypeDef,
     ChannelTargetInfoTypeDef,
+    ContactChannelAddressOutputTypeDef,
     ContactChannelAddressTypeDef,
+    ContactTargetInfoOutputTypeDef,
     ContactTargetInfoTypeDef,
     ContactTypeDef,
+    HandOffTimeOutputTypeDef,
     HandOffTimeTypeDef,
-    CreateContactChannelResultTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
-    CreateContactResultTypeDef,
     CreateRotationOverrideRequestRequestTypeDef,
-    CreateRotationOverrideResultTypeDef,
-    CreateRotationResultTypeDef,
     DeactivateContactChannelRequestRequestTypeDef,
     DeleteContactChannelRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
     DeleteRotationOverrideRequestRequestTypeDef,
     DeleteRotationRequestRequestTypeDef,
     DescribeEngagementRequestRequestTypeDef,
-    DescribeEngagementResultTypeDef,
     DescribePageRequestRequestTypeDef,
-    DescribePageResultTypeDef,
     EngagementTypeDef,
     GetContactChannelRequestRequestTypeDef,
     GetContactPolicyRequestRequestTypeDef,
-    GetContactPolicyResultTypeDef,
     GetContactRequestRequestTypeDef,
     GetRotationOverrideRequestRequestTypeDef,
-    GetRotationOverrideResultTypeDef,
     GetRotationRequestRequestTypeDef,
-    ListContactChannelsRequestListContactChannelsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListContactChannelsRequestRequestTypeDef,
-    ListContactsRequestListContactsPaginateTypeDef,
     ListContactsRequestRequestTypeDef,
     TimeRangeTypeDef,
-    ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
     ListPageReceiptsRequestRequestTypeDef,
     ReceiptTypeDef,
-    ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
     ListPageResolutionsRequestRequestTypeDef,
     ResolutionContactTypeDef,
-    ListPagesByContactRequestListPagesByContactPaginateTypeDef,
     ListPagesByContactRequestRequestTypeDef,
     PageTypeDef,
-    ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
     ListPagesByEngagementRequestRequestTypeDef,
     PreviewOverrideTypeDef,
-    ListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
     ListRotationOverridesRequestRequestTypeDef,
     RotationOverrideTypeDef,
-    ListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
     ListRotationShiftsRequestRequestTypeDef,
-    ListRotationsRequestListRotationsPaginateTypeDef,
     ListRotationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     PutContactPolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ShiftDetailsTypeDef,
     SendActivationCodeRequestRequestTypeDef,
     StartEngagementRequestRequestTypeDef,
-    StartEngagementResultTypeDef,
     StopEngagementRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ContactChannelTypeDef,
     CreateContactChannelRequestRequestTypeDef,
-    GetContactChannelResultTypeDef,
     UpdateContactChannelRequestRequestTypeDef,
+    TargetOutputTypeDef,
     TargetTypeDef,
-    ListContactsResultTypeDef,
+    CoverageTimeOutputTypeDef,
+    MonthlySettingOutputTypeDef,
+    WeeklySettingOutputTypeDef,
     CoverageTimeTypeDef,
     MonthlySettingTypeDef,
     WeeklySettingTypeDef,
-    ListTagsForResourceResultTypeDef,
+    CreateContactChannelResultTypeDef,
+    CreateContactResultTypeDef,
+    CreateRotationOverrideResultTypeDef,
+    CreateRotationResultTypeDef,
+    DescribeEngagementResultTypeDef,
+    DescribePageResultTypeDef,
+    GetContactChannelResultTypeDef,
+    GetContactPolicyResultTypeDef,
+    GetRotationOverrideResultTypeDef,
+    ListContactsResultTypeDef,
+    StartEngagementResultTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEngagementsResultTypeDef,
+    ListContactChannelsRequestListContactChannelsPaginateTypeDef,
+    ListContactsRequestListContactsPaginateTypeDef,
+    ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
+    ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
+    ListPagesByContactRequestListPagesByContactPaginateTypeDef,
+    ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
+    ListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
+    ListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
+    ListRotationsRequestListRotationsPaginateTypeDef,
     ListEngagementsRequestListEngagementsPaginateTypeDef,
     ListEngagementsRequestRequestTypeDef,
     ListPageReceiptsResultTypeDef,
     ListPageResolutionsResultTypeDef,
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListRotationOverridesResultTypeDef,
+    ListTagsForResourceResultTypeDef,
     RotationShiftTypeDef,
     ListContactChannelsResultTypeDef,
+    StageOutputTypeDef,
     StageTypeDef,
+    RecurrenceSettingsOutputTypeDef,
     RecurrenceSettingsTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationShiftsResultTypeDef,
+    PlanOutputTypeDef,
     PlanTypeDef,
-    CreateRotationRequestRequestTypeDef,
     GetRotationResultTypeDef,
+    RotationTypeDef,
+    CreateRotationRequestRequestTypeDef,
     ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef,
     ListPreviewRotationShiftsRequestRequestTypeDef,
-    RotationTypeDef,
     UpdateRotationRequestRequestTypeDef,
-    CreateContactRequestRequestTypeDef,
     GetContactResultTypeDef,
+    CreateContactRequestRequestTypeDef,
     UpdateContactRequestRequestTypeDef,
     ListRotationsResultTypeDef,
 )
 
 
 def get_structure() -> AcceptPageRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/__init__.py` & `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/__init__.pyi` & `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/__main__.py` & `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSMContacts 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.SSMContacts 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts\nOther"
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

### Comparing `mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/client.py` & `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/client.pyi` & `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/literals.py` & `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AcceptCodeValidationType",
     "AcceptTypeType",
     "ActivationStatusType",
     "ChannelTypeType",
     "ContactTypeType",
     "DayOfWeekType",
@@ -42,15 +41,14 @@
     "SSMContactsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AcceptCodeValidationType = Literal["ENFORCE", "IGNORE"]
 AcceptTypeType = Literal["DELIVERED", "READ"]
 ActivationStatusType = Literal["ACTIVATED", "NOT_ACTIVATED"]
 ChannelTypeType = Literal["EMAIL", "SMS", "VOICE"]
 ContactTypeType = Literal["ESCALATION", "ONCALL_SCHEDULE", "PERSONAL"]
 DayOfWeekType = Literal["FRI", "MON", "SAT", "SUN", "THU", "TUE", "WED"]
 ListContactChannelsPaginatorName = Literal["list_contact_channels"]
@@ -182,14 +180,15 @@
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
@@ -268,26 +267,28 @@
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

### Comparing `mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/literals.pyi` & `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AcceptCodeValidationType",
     "AcceptTypeType",
     "ActivationStatusType",
     "ChannelTypeType",
     "ContactTypeType",
     "DayOfWeekType",
@@ -41,14 +42,15 @@
     "SSMContactsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AcceptCodeValidationType = Literal["ENFORCE", "IGNORE"]
 AcceptTypeType = Literal["DELIVERED", "READ"]
 ActivationStatusType = Literal["ACTIVATED", "NOT_ACTIVATED"]
 ChannelTypeType = Literal["EMAIL", "SMS", "VOICE"]
 ContactTypeType = Literal["ESCALATION", "ONCALL_SCHEDULE", "PERSONAL"]
 DayOfWeekType = Literal["FRI", "MON", "SAT", "SUN", "THU", "TUE", "WED"]
 ListContactChannelsPaginatorName = Literal["list_contact_channels"]
@@ -180,14 +182,15 @@
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
@@ -266,26 +269,28 @@
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

### Comparing `mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/paginator.py` & `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -73,138 +73,128 @@
     "ListPagesByEngagementPaginator",
     "ListPreviewRotationShiftsPaginator",
     "ListRotationOverridesPaginator",
     "ListRotationShiftsPaginator",
     "ListRotationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListContactChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContactChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listcontactchannelspaginator)
     """
 
     def paginate(
-        self, *, ContactId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ContactId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListContactChannelsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContactChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listcontactchannelspaginator)
         """
 
-
 class ListContactsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContacts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listcontactspaginator)
     """
 
     def paginate(
         self,
         *,
         AliasPrefix: str = ...,
         Type: ContactTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListContactsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContacts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listcontactspaginator)
         """
 
-
 class ListEngagementsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListEngagements)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listengagementspaginator)
     """
 
     def paginate(
         self,
         *,
         IncidentId: str = ...,
         TimeRangeValue: TimeRangeTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEngagementsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListEngagements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listengagementspaginator)
         """
 
-
 class ListPageReceiptsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageReceipts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagereceiptspaginator)
     """
 
     def paginate(
-        self, *, PageId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PageId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPageReceiptsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageReceipts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagereceiptspaginator)
         """
 
-
 class ListPageResolutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageResolutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpageresolutionspaginator)
     """
 
     def paginate(
-        self, *, PageId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PageId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPageResolutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageResolutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpageresolutionspaginator)
         """
 
-
 class ListPagesByContactPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByContact)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagesbycontactpaginator)
     """
 
     def paginate(
-        self, *, ContactId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ContactId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPagesByContactResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByContact.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagesbycontactpaginator)
         """
 
-
 class ListPagesByEngagementPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByEngagement)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagesbyengagementpaginator)
     """
 
     def paginate(
-        self, *, EngagementId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, EngagementId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPagesByEngagementResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByEngagement.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagesbyengagementpaginator)
         """
 
-
 class ListPreviewRotationShiftsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpreviewrotationshiftspaginator)
     """
 
     def paginate(
@@ -213,68 +203,65 @@
         EndTime: Union[datetime, str],
         Members: Sequence[str],
         TimeZoneId: str,
         Recurrence: RecurrenceSettingsTypeDef,
         RotationStartTime: Union[datetime, str] = ...,
         StartTime: Union[datetime, str] = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPreviewRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpreviewrotationshiftspaginator)
         """
 
-
 class ListRotationOverridesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationOverrides)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationoverridespaginator)
     """
 
     def paginate(
         self,
         *,
         RotationId: str,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRotationOverridesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationOverrides.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationoverridespaginator)
         """
 
-
 class ListRotationShiftsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationShifts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationshiftspaginator)
     """
 
     def paginate(
         self,
         *,
         RotationId: str,
         EndTime: Union[datetime, str],
         StartTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationShifts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationshiftspaginator)
         """
 
-
 class ListRotationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationspaginator)
     """
 
     def paginate(
-        self, *, RotationNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RotationNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRotationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationspaginator)
         """
```

### Comparing `mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/paginator.pyi` & `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,128 +73,138 @@
     "ListPagesByEngagementPaginator",
     "ListPreviewRotationShiftsPaginator",
     "ListRotationOverridesPaginator",
     "ListRotationShiftsPaginator",
     "ListRotationsPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListContactChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContactChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listcontactchannelspaginator)
     """
 
     def paginate(
-        self, *, ContactId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ContactId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListContactChannelsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContactChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listcontactchannelspaginator)
         """
 
+
 class ListContactsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContacts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listcontactspaginator)
     """
 
     def paginate(
         self,
         *,
         AliasPrefix: str = ...,
         Type: ContactTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListContactsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContacts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listcontactspaginator)
         """
 
+
 class ListEngagementsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListEngagements)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listengagementspaginator)
     """
 
     def paginate(
         self,
         *,
         IncidentId: str = ...,
         TimeRangeValue: TimeRangeTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEngagementsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListEngagements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listengagementspaginator)
         """
 
+
 class ListPageReceiptsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageReceipts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagereceiptspaginator)
     """
 
     def paginate(
-        self, *, PageId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PageId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPageReceiptsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageReceipts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagereceiptspaginator)
         """
 
+
 class ListPageResolutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageResolutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpageresolutionspaginator)
     """
 
     def paginate(
-        self, *, PageId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PageId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPageResolutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageResolutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpageresolutionspaginator)
         """
 
+
 class ListPagesByContactPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByContact)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagesbycontactpaginator)
     """
 
     def paginate(
-        self, *, ContactId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ContactId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPagesByContactResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByContact.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagesbycontactpaginator)
         """
 
+
 class ListPagesByEngagementPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByEngagement)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagesbyengagementpaginator)
     """
 
     def paginate(
-        self, *, EngagementId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, EngagementId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPagesByEngagementResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByEngagement.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagesbyengagementpaginator)
         """
 
+
 class ListPreviewRotationShiftsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpreviewrotationshiftspaginator)
     """
 
     def paginate(
@@ -203,65 +213,68 @@
         EndTime: Union[datetime, str],
         Members: Sequence[str],
         TimeZoneId: str,
         Recurrence: RecurrenceSettingsTypeDef,
         RotationStartTime: Union[datetime, str] = ...,
         StartTime: Union[datetime, str] = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPreviewRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpreviewrotationshiftspaginator)
         """
 
+
 class ListRotationOverridesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationOverrides)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationoverridespaginator)
     """
 
     def paginate(
         self,
         *,
         RotationId: str,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRotationOverridesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationOverrides.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationoverridespaginator)
         """
 
+
 class ListRotationShiftsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationShifts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationshiftspaginator)
     """
 
     def paginate(
         self,
         *,
         RotationId: str,
         EndTime: Union[datetime, str],
         StartTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationShifts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationshiftspaginator)
         """
 
+
 class ListRotationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationspaginator)
     """
 
     def paginate(
-        self, *, RotationNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RotationNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRotationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationspaginator)
         """
```

### Comparing `mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/type_defs.py` & `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,110 +31,122 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AcceptPageRequestRequestTypeDef",
     "ActivateContactChannelRequestRequestTypeDef",
+    "ChannelTargetInfoOutputTypeDef",
     "ChannelTargetInfoTypeDef",
+    "ContactChannelAddressOutputTypeDef",
     "ContactChannelAddressTypeDef",
+    "ContactTargetInfoOutputTypeDef",
     "ContactTargetInfoTypeDef",
     "ContactTypeDef",
+    "HandOffTimeOutputTypeDef",
     "HandOffTimeTypeDef",
-    "CreateContactChannelResultTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
-    "CreateContactResultTypeDef",
     "CreateRotationOverrideRequestRequestTypeDef",
-    "CreateRotationOverrideResultTypeDef",
-    "CreateRotationResultTypeDef",
     "DeactivateContactChannelRequestRequestTypeDef",
     "DeleteContactChannelRequestRequestTypeDef",
     "DeleteContactRequestRequestTypeDef",
     "DeleteRotationOverrideRequestRequestTypeDef",
     "DeleteRotationRequestRequestTypeDef",
     "DescribeEngagementRequestRequestTypeDef",
-    "DescribeEngagementResultTypeDef",
     "DescribePageRequestRequestTypeDef",
-    "DescribePageResultTypeDef",
     "EngagementTypeDef",
     "GetContactChannelRequestRequestTypeDef",
     "GetContactPolicyRequestRequestTypeDef",
-    "GetContactPolicyResultTypeDef",
     "GetContactRequestRequestTypeDef",
     "GetRotationOverrideRequestRequestTypeDef",
-    "GetRotationOverrideResultTypeDef",
     "GetRotationRequestRequestTypeDef",
-    "ListContactChannelsRequestListContactChannelsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListContactChannelsRequestRequestTypeDef",
-    "ListContactsRequestListContactsPaginateTypeDef",
     "ListContactsRequestRequestTypeDef",
     "TimeRangeTypeDef",
-    "ListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
     "ListPageReceiptsRequestRequestTypeDef",
     "ReceiptTypeDef",
-    "ListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
     "ListPageResolutionsRequestRequestTypeDef",
     "ResolutionContactTypeDef",
-    "ListPagesByContactRequestListPagesByContactPaginateTypeDef",
     "ListPagesByContactRequestRequestTypeDef",
     "PageTypeDef",
-    "ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
     "ListPagesByEngagementRequestRequestTypeDef",
     "PreviewOverrideTypeDef",
-    "ListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
     "ListRotationOverridesRequestRequestTypeDef",
     "RotationOverrideTypeDef",
-    "ListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
     "ListRotationShiftsRequestRequestTypeDef",
-    "ListRotationsRequestListRotationsPaginateTypeDef",
     "ListRotationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
     "PutContactPolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ShiftDetailsTypeDef",
     "SendActivationCodeRequestRequestTypeDef",
     "StartEngagementRequestRequestTypeDef",
-    "StartEngagementResultTypeDef",
     "StopEngagementRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ContactChannelTypeDef",
     "CreateContactChannelRequestRequestTypeDef",
-    "GetContactChannelResultTypeDef",
     "UpdateContactChannelRequestRequestTypeDef",
+    "TargetOutputTypeDef",
     "TargetTypeDef",
-    "ListContactsResultTypeDef",
+    "CoverageTimeOutputTypeDef",
+    "MonthlySettingOutputTypeDef",
+    "WeeklySettingOutputTypeDef",
     "CoverageTimeTypeDef",
     "MonthlySettingTypeDef",
     "WeeklySettingTypeDef",
-    "ListTagsForResourceResultTypeDef",
+    "CreateContactChannelResultTypeDef",
+    "CreateContactResultTypeDef",
+    "CreateRotationOverrideResultTypeDef",
+    "CreateRotationResultTypeDef",
+    "DescribeEngagementResultTypeDef",
+    "DescribePageResultTypeDef",
+    "GetContactChannelResultTypeDef",
+    "GetContactPolicyResultTypeDef",
+    "GetRotationOverrideResultTypeDef",
+    "ListContactsResultTypeDef",
+    "StartEngagementResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEngagementsResultTypeDef",
+    "ListContactChannelsRequestListContactChannelsPaginateTypeDef",
+    "ListContactsRequestListContactsPaginateTypeDef",
+    "ListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
+    "ListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
+    "ListPagesByContactRequestListPagesByContactPaginateTypeDef",
+    "ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
+    "ListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
+    "ListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
+    "ListRotationsRequestListRotationsPaginateTypeDef",
     "ListEngagementsRequestListEngagementsPaginateTypeDef",
     "ListEngagementsRequestRequestTypeDef",
     "ListPageReceiptsResultTypeDef",
     "ListPageResolutionsResultTypeDef",
     "ListPagesByContactResultTypeDef",
     "ListPagesByEngagementResultTypeDef",
     "ListRotationOverridesResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "RotationShiftTypeDef",
     "ListContactChannelsResultTypeDef",
+    "StageOutputTypeDef",
     "StageTypeDef",
+    "RecurrenceSettingsOutputTypeDef",
     "RecurrenceSettingsTypeDef",
     "ListPreviewRotationShiftsResultTypeDef",
     "ListRotationShiftsResultTypeDef",
+    "PlanOutputTypeDef",
     "PlanTypeDef",
-    "CreateRotationRequestRequestTypeDef",
     "GetRotationResultTypeDef",
+    "RotationTypeDef",
+    "CreateRotationRequestRequestTypeDef",
     "ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     "ListPreviewRotationShiftsRequestRequestTypeDef",
-    "RotationTypeDef",
     "UpdateRotationRequestRequestTypeDef",
-    "CreateContactRequestRequestTypeDef",
     "GetContactResultTypeDef",
+    "CreateContactRequestRequestTypeDef",
     "UpdateContactRequestRequestTypeDef",
     "ListRotationsResultTypeDef",
 )
 
 _RequiredAcceptPageRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptPageRequestRequestTypeDef",
     {
@@ -164,14 +176,35 @@
     "ActivateContactChannelRequestRequestTypeDef",
     {
         "ContactChannelId": str,
         "ActivationCode": str,
     },
 )
 
+_RequiredChannelTargetInfoOutputTypeDef = TypedDict(
+    "_RequiredChannelTargetInfoOutputTypeDef",
+    {
+        "ContactChannelId": str,
+    },
+)
+_OptionalChannelTargetInfoOutputTypeDef = TypedDict(
+    "_OptionalChannelTargetInfoOutputTypeDef",
+    {
+        "RetryIntervalInMinutes": int,
+    },
+    total=False,
+)
+
+
+class ChannelTargetInfoOutputTypeDef(
+    _RequiredChannelTargetInfoOutputTypeDef, _OptionalChannelTargetInfoOutputTypeDef
+):
+    pass
+
+
 _RequiredChannelTargetInfoTypeDef = TypedDict(
     "_RequiredChannelTargetInfoTypeDef",
     {
         "ContactChannelId": str,
     },
 )
 _OptionalChannelTargetInfoTypeDef = TypedDict(
@@ -185,22 +218,51 @@
 
 class ChannelTargetInfoTypeDef(
     _RequiredChannelTargetInfoTypeDef, _OptionalChannelTargetInfoTypeDef
 ):
     pass
 
 
+ContactChannelAddressOutputTypeDef = TypedDict(
+    "ContactChannelAddressOutputTypeDef",
+    {
+        "SimpleAddress": str,
+    },
+    total=False,
+)
+
 ContactChannelAddressTypeDef = TypedDict(
     "ContactChannelAddressTypeDef",
     {
         "SimpleAddress": str,
     },
     total=False,
 )
 
+_RequiredContactTargetInfoOutputTypeDef = TypedDict(
+    "_RequiredContactTargetInfoOutputTypeDef",
+    {
+        "IsEssential": bool,
+    },
+)
+_OptionalContactTargetInfoOutputTypeDef = TypedDict(
+    "_OptionalContactTargetInfoOutputTypeDef",
+    {
+        "ContactId": str,
+    },
+    total=False,
+)
+
+
+class ContactTargetInfoOutputTypeDef(
+    _RequiredContactTargetInfoOutputTypeDef, _OptionalContactTargetInfoOutputTypeDef
+):
+    pass
+
+
 _RequiredContactTargetInfoTypeDef = TypedDict(
     "_RequiredContactTargetInfoTypeDef",
     {
         "IsEssential": bool,
     },
 )
 _OptionalContactTargetInfoTypeDef = TypedDict(
@@ -235,47 +297,50 @@
 )
 
 
 class ContactTypeDef(_RequiredContactTypeDef, _OptionalContactTypeDef):
     pass
 
 
+HandOffTimeOutputTypeDef = TypedDict(
+    "HandOffTimeOutputTypeDef",
+    {
+        "HourOfDay": int,
+        "MinuteOfHour": int,
+    },
+)
+
 HandOffTimeTypeDef = TypedDict(
     "HandOffTimeTypeDef",
     {
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
 )
 
-CreateContactChannelResultTypeDef = TypedDict(
-    "CreateContactChannelResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ContactChannelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-CreateContactResultTypeDef = TypedDict(
-    "CreateContactResultTypeDef",
-    {
-        "ContactArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateRotationOverrideRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRotationOverrideRequestRequestTypeDef",
     {
         "RotationId": str,
         "NewContactIds": Sequence[str],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -293,30 +358,14 @@
 class CreateRotationOverrideRequestRequestTypeDef(
     _RequiredCreateRotationOverrideRequestRequestTypeDef,
     _OptionalCreateRotationOverrideRequestRequestTypeDef,
 ):
     pass
 
 
-CreateRotationOverrideResultTypeDef = TypedDict(
-    "CreateRotationOverrideResultTypeDef",
-    {
-        "RotationOverrideId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateRotationResultTypeDef = TypedDict(
-    "CreateRotationResultTypeDef",
-    {
-        "RotationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeactivateContactChannelRequestRequestTypeDef = TypedDict(
     "DeactivateContactChannelRequestRequestTypeDef",
     {
         "ContactChannelId": str,
     },
 )
 
@@ -352,57 +401,21 @@
 DescribeEngagementRequestRequestTypeDef = TypedDict(
     "DescribeEngagementRequestRequestTypeDef",
     {
         "EngagementId": str,
     },
 )
 
-DescribeEngagementResultTypeDef = TypedDict(
-    "DescribeEngagementResultTypeDef",
-    {
-        "ContactArn": str,
-        "EngagementArn": str,
-        "Sender": str,
-        "Subject": str,
-        "Content": str,
-        "PublicSubject": str,
-        "PublicContent": str,
-        "IncidentId": str,
-        "StartTime": datetime,
-        "StopTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribePageRequestRequestTypeDef = TypedDict(
     "DescribePageRequestRequestTypeDef",
     {
         "PageId": str,
     },
 )
 
-DescribePageResultTypeDef = TypedDict(
-    "DescribePageResultTypeDef",
-    {
-        "PageArn": str,
-        "EngagementArn": str,
-        "ContactArn": str,
-        "Sender": str,
-        "Subject": str,
-        "Content": str,
-        "PublicSubject": str,
-        "PublicContent": str,
-        "IncidentId": str,
-        "SentTime": datetime,
-        "ReadTime": datetime,
-        "DeliveryTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEngagementTypeDef = TypedDict(
     "_RequiredEngagementTypeDef",
     {
         "EngagementArn": str,
         "ContactArn": str,
         "Sender": str,
     },
@@ -432,23 +445,14 @@
 GetContactPolicyRequestRequestTypeDef = TypedDict(
     "GetContactPolicyRequestRequestTypeDef",
     {
         "ContactArn": str,
     },
 )
 
-GetContactPolicyResultTypeDef = TypedDict(
-    "GetContactPolicyResultTypeDef",
-    {
-        "ContactArn": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetContactRequestRequestTypeDef = TypedDict(
     "GetContactRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 
@@ -456,56 +460,31 @@
     "GetRotationOverrideRequestRequestTypeDef",
     {
         "RotationId": str,
         "RotationOverrideId": str,
     },
 )
 
-GetRotationOverrideResultTypeDef = TypedDict(
-    "GetRotationOverrideResultTypeDef",
-    {
-        "RotationOverrideId": str,
-        "RotationArn": str,
-        "NewContactIds": List[str],
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "CreateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRotationRequestRequestTypeDef = TypedDict(
     "GetRotationRequestRequestTypeDef",
     {
         "RotationId": str,
     },
 )
 
-_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
-    "_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef",
-    {
-        "ContactId": str,
-    },
-)
-_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
-    "_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef",
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
 
-
-class ListContactChannelsRequestListContactChannelsPaginateTypeDef(
-    _RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef,
-    _OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListContactChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactChannelsRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 _OptionalListContactChannelsRequestRequestTypeDef = TypedDict(
@@ -521,24 +500,14 @@
 class ListContactChannelsRequestRequestTypeDef(
     _RequiredListContactChannelsRequestRequestTypeDef,
     _OptionalListContactChannelsRequestRequestTypeDef,
 ):
     pass
 
 
-ListContactsRequestListContactsPaginateTypeDef = TypedDict(
-    "ListContactsRequestListContactsPaginateTypeDef",
-    {
-        "AliasPrefix": str,
-        "Type": ContactTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListContactsRequestRequestTypeDef = TypedDict(
     "ListContactsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "AliasPrefix": str,
         "Type": ContactTypeType,
@@ -551,36 +520,14 @@
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
-    "_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
-    {
-        "PageId": str,
-    },
-)
-_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
-    "_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPageReceiptsRequestListPageReceiptsPaginateTypeDef(
-    _RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
-    _OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPageReceiptsRequestRequestTypeDef = TypedDict(
     "_RequiredListPageReceiptsRequestRequestTypeDef",
     {
         "PageId": str,
     },
 )
 _OptionalListPageReceiptsRequestRequestTypeDef = TypedDict(
@@ -616,36 +563,14 @@
 )
 
 
 class ReceiptTypeDef(_RequiredReceiptTypeDef, _OptionalReceiptTypeDef):
     pass
 
 
-_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
-    "_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
-    {
-        "PageId": str,
-    },
-)
-_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
-    "_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPageResolutionsRequestListPageResolutionsPaginateTypeDef(
-    _RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
-    _OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPageResolutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPageResolutionsRequestRequestTypeDef",
     {
         "PageId": str,
     },
 )
 _OptionalListPageResolutionsRequestRequestTypeDef = TypedDict(
@@ -682,36 +607,14 @@
 
 class ResolutionContactTypeDef(
     _RequiredResolutionContactTypeDef, _OptionalResolutionContactTypeDef
 ):
     pass
 
 
-_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
-    "_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef",
-    {
-        "ContactId": str,
-    },
-)
-_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
-    "_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPagesByContactRequestListPagesByContactPaginateTypeDef(
-    _RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef,
-    _OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPagesByContactRequestRequestTypeDef = TypedDict(
     "_RequiredListPagesByContactRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 _OptionalListPagesByContactRequestRequestTypeDef = TypedDict(
@@ -752,36 +655,14 @@
 )
 
 
 class PageTypeDef(_RequiredPageTypeDef, _OptionalPageTypeDef):
     pass
 
 
-_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
-    "_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
-    {
-        "EngagementId": str,
-    },
-)
-_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
-    "_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef(
-    _RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
-    _OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPagesByEngagementRequestRequestTypeDef = TypedDict(
     "_RequiredListPagesByEngagementRequestRequestTypeDef",
     {
         "EngagementId": str,
     },
 )
 _OptionalListPagesByEngagementRequestRequestTypeDef = TypedDict(
@@ -807,38 +688,14 @@
         "NewMembers": Sequence[str],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
-    "_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
-    {
-        "RotationId": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
-    "_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRotationOverridesRequestListRotationOverridesPaginateTypeDef(
-    _RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
-    _OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRotationOverridesRequestRequestTypeDef = TypedDict(
     "_RequiredListRotationOverridesRequestRequestTypeDef",
     {
         "RotationId": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
@@ -867,38 +724,14 @@
         "NewContactIds": List[str],
         "StartTime": datetime,
         "EndTime": datetime,
         "CreateTime": datetime,
     },
 )
 
-_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
-    "_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
-    {
-        "RotationId": str,
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
-    "_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRotationShiftsRequestListRotationShiftsPaginateTypeDef(
-    _RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
-    _OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRotationShiftsRequestRequestTypeDef = TypedDict(
     "_RequiredListRotationShiftsRequestRequestTypeDef",
     {
         "RotationId": str,
         "EndTime": Union[datetime, str],
     },
 )
@@ -916,23 +749,14 @@
 class ListRotationShiftsRequestRequestTypeDef(
     _RequiredListRotationShiftsRequestRequestTypeDef,
     _OptionalListRotationShiftsRequestRequestTypeDef,
 ):
     pass
 
 
-ListRotationsRequestListRotationsPaginateTypeDef = TypedDict(
-    "ListRotationsRequestListRotationsPaginateTypeDef",
-    {
-        "RotationNamePrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRotationsRequestRequestTypeDef = TypedDict(
     "ListRotationsRequestRequestTypeDef",
     {
         "RotationNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -942,43 +766,31 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Key": str,
+        "Value": str,
     },
     total=False,
 )
 
 PutContactPolicyRequestRequestTypeDef = TypedDict(
     "PutContactPolicyRequestRequestTypeDef",
     {
         "ContactArn": str,
         "Policy": str,
     },
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
 ShiftDetailsTypeDef = TypedDict(
     "ShiftDetailsTypeDef",
     {
         "OverriddenContactIds": List[str],
     },
 )
 
@@ -1012,22 +824,14 @@
 
 class StartEngagementRequestRequestTypeDef(
     _RequiredStartEngagementRequestRequestTypeDef, _OptionalStartEngagementRequestRequestTypeDef
 ):
     pass
 
 
-StartEngagementResultTypeDef = TypedDict(
-    "StartEngagementResultTypeDef",
-    {
-        "EngagementArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStopEngagementRequestRequestTypeDef = TypedDict(
     "_RequiredStopEngagementRequestRequestTypeDef",
     {
         "EngagementId": str,
     },
 )
 _OptionalStopEngagementRequestRequestTypeDef = TypedDict(
@@ -1055,15 +859,15 @@
 
 _RequiredContactChannelTypeDef = TypedDict(
     "_RequiredContactChannelTypeDef",
     {
         "ContactChannelArn": str,
         "ContactArn": str,
         "Name": str,
-        "DeliveryAddress": ContactChannelAddressTypeDef,
+        "DeliveryAddress": ContactChannelAddressOutputTypeDef,
         "ActivationStatus": ActivationStatusType,
     },
 )
 _OptionalContactChannelTypeDef = TypedDict(
     "_OptionalContactChannelTypeDef",
     {
         "Type": ChannelTypeType,
@@ -1098,27 +902,14 @@
 class CreateContactChannelRequestRequestTypeDef(
     _RequiredCreateContactChannelRequestRequestTypeDef,
     _OptionalCreateContactChannelRequestRequestTypeDef,
 ):
     pass
 
 
-GetContactChannelResultTypeDef = TypedDict(
-    "GetContactChannelResultTypeDef",
-    {
-        "ContactArn": str,
-        "ContactChannelArn": str,
-        "Name": str,
-        "Type": ChannelTypeType,
-        "DeliveryAddress": ContactChannelAddressTypeDef,
-        "ActivationStatus": ActivationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateContactChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactChannelRequestRequestTypeDef",
     {
         "ContactChannelId": str,
     },
 )
 _OptionalUpdateContactChannelRequestRequestTypeDef = TypedDict(
@@ -1134,29 +925,54 @@
 class UpdateContactChannelRequestRequestTypeDef(
     _RequiredUpdateContactChannelRequestRequestTypeDef,
     _OptionalUpdateContactChannelRequestRequestTypeDef,
 ):
     pass
 
 
+TargetOutputTypeDef = TypedDict(
+    "TargetOutputTypeDef",
+    {
+        "ChannelTargetInfo": ChannelTargetInfoOutputTypeDef,
+        "ContactTargetInfo": ContactTargetInfoOutputTypeDef,
+    },
+    total=False,
+)
+
 TargetTypeDef = TypedDict(
     "TargetTypeDef",
     {
         "ChannelTargetInfo": ChannelTargetInfoTypeDef,
         "ContactTargetInfo": ContactTargetInfoTypeDef,
     },
     total=False,
 )
 
-ListContactsResultTypeDef = TypedDict(
-    "ListContactsResultTypeDef",
+CoverageTimeOutputTypeDef = TypedDict(
+    "CoverageTimeOutputTypeDef",
     {
-        "NextToken": str,
-        "Contacts": List[ContactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Start": HandOffTimeOutputTypeDef,
+        "End": HandOffTimeOutputTypeDef,
+    },
+    total=False,
+)
+
+MonthlySettingOutputTypeDef = TypedDict(
+    "MonthlySettingOutputTypeDef",
+    {
+        "DayOfMonth": int,
+        "HandOffTime": HandOffTimeOutputTypeDef,
+    },
+)
+
+WeeklySettingOutputTypeDef = TypedDict(
+    "WeeklySettingOutputTypeDef",
+    {
+        "DayOfWeek": DayOfWeekType,
+        "HandOffTime": HandOffTimeOutputTypeDef,
     },
 )
 
 CoverageTimeTypeDef = TypedDict(
     "CoverageTimeTypeDef",
     {
         "Start": HandOffTimeTypeDef,
@@ -1177,19 +993,131 @@
     "WeeklySettingTypeDef",
     {
         "DayOfWeek": DayOfWeekType,
         "HandOffTime": HandOffTimeTypeDef,
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
+CreateContactChannelResultTypeDef = TypedDict(
+    "CreateContactChannelResultTypeDef",
+    {
+        "ContactChannelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateContactResultTypeDef = TypedDict(
+    "CreateContactResultTypeDef",
+    {
+        "ContactArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRotationOverrideResultTypeDef = TypedDict(
+    "CreateRotationOverrideResultTypeDef",
+    {
+        "RotationOverrideId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRotationResultTypeDef = TypedDict(
+    "CreateRotationResultTypeDef",
+    {
+        "RotationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEngagementResultTypeDef = TypedDict(
+    "DescribeEngagementResultTypeDef",
+    {
+        "ContactArn": str,
+        "EngagementArn": str,
+        "Sender": str,
+        "Subject": str,
+        "Content": str,
+        "PublicSubject": str,
+        "PublicContent": str,
+        "IncidentId": str,
+        "StartTime": datetime,
+        "StopTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePageResultTypeDef = TypedDict(
+    "DescribePageResultTypeDef",
+    {
+        "PageArn": str,
+        "EngagementArn": str,
+        "ContactArn": str,
+        "Sender": str,
+        "Subject": str,
+        "Content": str,
+        "PublicSubject": str,
+        "PublicContent": str,
+        "IncidentId": str,
+        "SentTime": datetime,
+        "ReadTime": datetime,
+        "DeliveryTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContactChannelResultTypeDef = TypedDict(
+    "GetContactChannelResultTypeDef",
+    {
+        "ContactArn": str,
+        "ContactChannelArn": str,
+        "Name": str,
+        "Type": ChannelTypeType,
+        "DeliveryAddress": ContactChannelAddressOutputTypeDef,
+        "ActivationStatus": ActivationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContactPolicyResultTypeDef = TypedDict(
+    "GetContactPolicyResultTypeDef",
+    {
+        "ContactArn": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRotationOverrideResultTypeDef = TypedDict(
+    "GetRotationOverrideResultTypeDef",
+    {
+        "RotationOverrideId": str,
+        "RotationArn": str,
+        "NewContactIds": List[str],
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "CreateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListContactsResultTypeDef = TypedDict(
+    "ListContactsResultTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "NextToken": str,
+        "Contacts": List[ContactTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartEngagementResultTypeDef = TypedDict(
+    "StartEngagementResultTypeDef",
+    {
+        "EngagementArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -1198,24 +1126,201 @@
 )
 
 ListEngagementsResultTypeDef = TypedDict(
     "ListEngagementsResultTypeDef",
     {
         "NextToken": str,
         "Engagements": List[EngagementTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
+    "_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef",
+    {
+        "ContactId": str,
+    },
+)
+_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
+    "_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListContactChannelsRequestListContactChannelsPaginateTypeDef(
+    _RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef,
+    _OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef,
+):
+    pass
+
+
+ListContactsRequestListContactsPaginateTypeDef = TypedDict(
+    "ListContactsRequestListContactsPaginateTypeDef",
+    {
+        "AliasPrefix": str,
+        "Type": ContactTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
+    "_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
+    {
+        "PageId": str,
+    },
+)
+_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
+    "_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPageReceiptsRequestListPageReceiptsPaginateTypeDef(
+    _RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
+    _OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
+    "_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
+    {
+        "PageId": str,
+    },
+)
+_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
+    "_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPageResolutionsRequestListPageResolutionsPaginateTypeDef(
+    _RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
+    _OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
+    "_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef",
+    {
+        "ContactId": str,
+    },
+)
+_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
+    "_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+
+class ListPagesByContactRequestListPagesByContactPaginateTypeDef(
+    _RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef,
+    _OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
+    "_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
+    {
+        "EngagementId": str,
+    },
+)
+_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
+    "_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef(
+    _RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
+    _OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
+    "_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
+    {
+        "RotationId": str,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+    },
+)
+_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
+    "_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRotationOverridesRequestListRotationOverridesPaginateTypeDef(
+    _RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
+    _OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
+    "_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
+    {
+        "RotationId": str,
+        "EndTime": Union[datetime, str],
+    },
+)
+_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
+    "_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRotationShiftsRequestListRotationShiftsPaginateTypeDef(
+    _RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
+    _OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
+):
+    pass
+
+
+ListRotationsRequestListRotationsPaginateTypeDef = TypedDict(
+    "ListRotationsRequestListRotationsPaginateTypeDef",
+    {
+        "RotationNamePrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListEngagementsRequestListEngagementsPaginateTypeDef = TypedDict(
     "ListEngagementsRequestListEngagementsPaginateTypeDef",
     {
         "IncidentId": str,
         "TimeRangeValue": TimeRangeTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListEngagementsRequestRequestTypeDef = TypedDict(
     "ListEngagementsRequestRequestTypeDef",
     {
@@ -1228,51 +1333,59 @@
 )
 
 ListPageReceiptsResultTypeDef = TypedDict(
     "ListPageReceiptsResultTypeDef",
     {
         "NextToken": str,
         "Receipts": List[ReceiptTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPageResolutionsResultTypeDef = TypedDict(
     "ListPageResolutionsResultTypeDef",
     {
         "NextToken": str,
         "PageResolutions": List[ResolutionContactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPagesByContactResultTypeDef = TypedDict(
     "ListPagesByContactResultTypeDef",
     {
         "NextToken": str,
         "Pages": List[PageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPagesByEngagementResultTypeDef = TypedDict(
     "ListPagesByEngagementResultTypeDef",
     {
         "NextToken": str,
         "Pages": List[PageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRotationOverridesResultTypeDef = TypedDict(
     "ListRotationOverridesResultTypeDef",
     {
         "RotationOverrides": List[RotationOverrideTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRotationShiftTypeDef = TypedDict(
     "_RequiredRotationShiftTypeDef",
     {
         "StartTime": datetime,
@@ -1295,26 +1408,59 @@
 
 
 ListContactChannelsResultTypeDef = TypedDict(
     "ListContactChannelsResultTypeDef",
     {
         "NextToken": str,
         "ContactChannels": List[ContactChannelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StageOutputTypeDef = TypedDict(
+    "StageOutputTypeDef",
+    {
+        "DurationInMinutes": int,
+        "Targets": List[TargetOutputTypeDef],
     },
 )
 
 StageTypeDef = TypedDict(
     "StageTypeDef",
     {
         "DurationInMinutes": int,
         "Targets": Sequence[TargetTypeDef],
     },
 )
 
+_RequiredRecurrenceSettingsOutputTypeDef = TypedDict(
+    "_RequiredRecurrenceSettingsOutputTypeDef",
+    {
+        "NumberOfOnCalls": int,
+        "RecurrenceMultiplier": int,
+    },
+)
+_OptionalRecurrenceSettingsOutputTypeDef = TypedDict(
+    "_OptionalRecurrenceSettingsOutputTypeDef",
+    {
+        "MonthlySettings": List[MonthlySettingOutputTypeDef],
+        "WeeklySettings": List[WeeklySettingOutputTypeDef],
+        "DailySettings": List[HandOffTimeOutputTypeDef],
+        "ShiftCoverages": Dict[DayOfWeekType, List[CoverageTimeOutputTypeDef]],
+    },
+    total=False,
+)
+
+
+class RecurrenceSettingsOutputTypeDef(
+    _RequiredRecurrenceSettingsOutputTypeDef, _OptionalRecurrenceSettingsOutputTypeDef
+):
+    pass
+
+
 _RequiredRecurrenceSettingsTypeDef = TypedDict(
     "_RequiredRecurrenceSettingsTypeDef",
     {
         "NumberOfOnCalls": int,
         "RecurrenceMultiplier": int,
     },
 )
@@ -1337,36 +1483,81 @@
 
 
 ListPreviewRotationShiftsResultTypeDef = TypedDict(
     "ListPreviewRotationShiftsResultTypeDef",
     {
         "RotationShifts": List[RotationShiftTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRotationShiftsResultTypeDef = TypedDict(
     "ListRotationShiftsResultTypeDef",
     {
         "RotationShifts": List[RotationShiftTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PlanOutputTypeDef = TypedDict(
+    "PlanOutputTypeDef",
+    {
+        "Stages": List[StageOutputTypeDef],
+        "RotationIds": List[str],
+    },
+    total=False,
+)
+
 PlanTypeDef = TypedDict(
     "PlanTypeDef",
     {
         "Stages": Sequence[StageTypeDef],
         "RotationIds": Sequence[str],
     },
     total=False,
 )
 
+GetRotationResultTypeDef = TypedDict(
+    "GetRotationResultTypeDef",
+    {
+        "RotationArn": str,
+        "Name": str,
+        "ContactIds": List[str],
+        "StartTime": datetime,
+        "TimeZoneId": str,
+        "Recurrence": RecurrenceSettingsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredRotationTypeDef = TypedDict(
+    "_RequiredRotationTypeDef",
+    {
+        "RotationArn": str,
+        "Name": str,
+    },
+)
+_OptionalRotationTypeDef = TypedDict(
+    "_OptionalRotationTypeDef",
+    {
+        "ContactIds": List[str],
+        "StartTime": datetime,
+        "TimeZoneId": str,
+        "Recurrence": RecurrenceSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class RotationTypeDef(_RequiredRotationTypeDef, _OptionalRotationTypeDef):
+    pass
+
+
 _RequiredCreateRotationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRotationRequestRequestTypeDef",
     {
         "Name": str,
         "ContactIds": Sequence[str],
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
@@ -1385,27 +1576,14 @@
 
 class CreateRotationRequestRequestTypeDef(
     _RequiredCreateRotationRequestRequestTypeDef, _OptionalCreateRotationRequestRequestTypeDef
 ):
     pass
 
 
-GetRotationResultTypeDef = TypedDict(
-    "GetRotationResultTypeDef",
-    {
-        "RotationArn": str,
-        "Name": str,
-        "ContactIds": List[str],
-        "StartTime": datetime,
-        "TimeZoneId": str,
-        "Recurrence": RecurrenceSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef = TypedDict(
     "_RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     {
         "EndTime": Union[datetime, str],
         "Members": Sequence[str],
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
@@ -1413,15 +1591,15 @@
 )
 _OptionalListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef = TypedDict(
     "_OptionalListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     {
         "RotationStartTime": Union[datetime, str],
         "StartTime": Union[datetime, str],
         "Overrides": Sequence[PreviewOverrideTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef(
     _RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef,
@@ -1455,37 +1633,14 @@
 class ListPreviewRotationShiftsRequestRequestTypeDef(
     _RequiredListPreviewRotationShiftsRequestRequestTypeDef,
     _OptionalListPreviewRotationShiftsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredRotationTypeDef = TypedDict(
-    "_RequiredRotationTypeDef",
-    {
-        "RotationArn": str,
-        "Name": str,
-    },
-)
-_OptionalRotationTypeDef = TypedDict(
-    "_OptionalRotationTypeDef",
-    {
-        "ContactIds": List[str],
-        "StartTime": datetime,
-        "TimeZoneId": str,
-        "Recurrence": RecurrenceSettingsTypeDef,
-    },
-    total=False,
-)
-
-
-class RotationTypeDef(_RequiredRotationTypeDef, _OptionalRotationTypeDef):
-    pass
-
-
 _RequiredUpdateRotationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRotationRequestRequestTypeDef",
     {
         "RotationId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
     },
 )
@@ -1502,14 +1657,26 @@
 
 class UpdateRotationRequestRequestTypeDef(
     _RequiredUpdateRotationRequestRequestTypeDef, _OptionalUpdateRotationRequestRequestTypeDef
 ):
     pass
 
 
+GetContactResultTypeDef = TypedDict(
+    "GetContactResultTypeDef",
+    {
+        "ContactArn": str,
+        "Alias": str,
+        "DisplayName": str,
+        "Type": ContactTypeType,
+        "Plan": PlanOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateContactRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContactRequestRequestTypeDef",
     {
         "Alias": str,
         "Type": ContactTypeType,
         "Plan": PlanTypeDef,
     },
@@ -1527,26 +1694,14 @@
 
 class CreateContactRequestRequestTypeDef(
     _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
 ):
     pass
 
 
-GetContactResultTypeDef = TypedDict(
-    "GetContactResultTypeDef",
-    {
-        "ContactArn": str,
-        "Alias": str,
-        "DisplayName": str,
-        "Type": ContactTypeType,
-        "Plan": PlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateContactRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 _OptionalUpdateContactRequestRequestTypeDef = TypedDict(
@@ -1566,10 +1721,10 @@
 
 
 ListRotationsResultTypeDef = TypedDict(
     "ListRotationsResultTypeDef",
     {
         "NextToken": str,
         "Rotations": List[RotationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts/type_defs.pyi` & `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -30,110 +30,122 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceptPageRequestRequestTypeDef",
     "ActivateContactChannelRequestRequestTypeDef",
+    "ChannelTargetInfoOutputTypeDef",
     "ChannelTargetInfoTypeDef",
+    "ContactChannelAddressOutputTypeDef",
     "ContactChannelAddressTypeDef",
+    "ContactTargetInfoOutputTypeDef",
     "ContactTargetInfoTypeDef",
     "ContactTypeDef",
+    "HandOffTimeOutputTypeDef",
     "HandOffTimeTypeDef",
-    "CreateContactChannelResultTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
-    "CreateContactResultTypeDef",
     "CreateRotationOverrideRequestRequestTypeDef",
-    "CreateRotationOverrideResultTypeDef",
-    "CreateRotationResultTypeDef",
     "DeactivateContactChannelRequestRequestTypeDef",
     "DeleteContactChannelRequestRequestTypeDef",
     "DeleteContactRequestRequestTypeDef",
     "DeleteRotationOverrideRequestRequestTypeDef",
     "DeleteRotationRequestRequestTypeDef",
     "DescribeEngagementRequestRequestTypeDef",
-    "DescribeEngagementResultTypeDef",
     "DescribePageRequestRequestTypeDef",
-    "DescribePageResultTypeDef",
     "EngagementTypeDef",
     "GetContactChannelRequestRequestTypeDef",
     "GetContactPolicyRequestRequestTypeDef",
-    "GetContactPolicyResultTypeDef",
     "GetContactRequestRequestTypeDef",
     "GetRotationOverrideRequestRequestTypeDef",
-    "GetRotationOverrideResultTypeDef",
     "GetRotationRequestRequestTypeDef",
-    "ListContactChannelsRequestListContactChannelsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListContactChannelsRequestRequestTypeDef",
-    "ListContactsRequestListContactsPaginateTypeDef",
     "ListContactsRequestRequestTypeDef",
     "TimeRangeTypeDef",
-    "ListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
     "ListPageReceiptsRequestRequestTypeDef",
     "ReceiptTypeDef",
-    "ListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
     "ListPageResolutionsRequestRequestTypeDef",
     "ResolutionContactTypeDef",
-    "ListPagesByContactRequestListPagesByContactPaginateTypeDef",
     "ListPagesByContactRequestRequestTypeDef",
     "PageTypeDef",
-    "ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
     "ListPagesByEngagementRequestRequestTypeDef",
     "PreviewOverrideTypeDef",
-    "ListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
     "ListRotationOverridesRequestRequestTypeDef",
     "RotationOverrideTypeDef",
-    "ListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
     "ListRotationShiftsRequestRequestTypeDef",
-    "ListRotationsRequestListRotationsPaginateTypeDef",
     "ListRotationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
     "PutContactPolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ShiftDetailsTypeDef",
     "SendActivationCodeRequestRequestTypeDef",
     "StartEngagementRequestRequestTypeDef",
-    "StartEngagementResultTypeDef",
     "StopEngagementRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ContactChannelTypeDef",
     "CreateContactChannelRequestRequestTypeDef",
-    "GetContactChannelResultTypeDef",
     "UpdateContactChannelRequestRequestTypeDef",
+    "TargetOutputTypeDef",
     "TargetTypeDef",
-    "ListContactsResultTypeDef",
+    "CoverageTimeOutputTypeDef",
+    "MonthlySettingOutputTypeDef",
+    "WeeklySettingOutputTypeDef",
     "CoverageTimeTypeDef",
     "MonthlySettingTypeDef",
     "WeeklySettingTypeDef",
-    "ListTagsForResourceResultTypeDef",
+    "CreateContactChannelResultTypeDef",
+    "CreateContactResultTypeDef",
+    "CreateRotationOverrideResultTypeDef",
+    "CreateRotationResultTypeDef",
+    "DescribeEngagementResultTypeDef",
+    "DescribePageResultTypeDef",
+    "GetContactChannelResultTypeDef",
+    "GetContactPolicyResultTypeDef",
+    "GetRotationOverrideResultTypeDef",
+    "ListContactsResultTypeDef",
+    "StartEngagementResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEngagementsResultTypeDef",
+    "ListContactChannelsRequestListContactChannelsPaginateTypeDef",
+    "ListContactsRequestListContactsPaginateTypeDef",
+    "ListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
+    "ListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
+    "ListPagesByContactRequestListPagesByContactPaginateTypeDef",
+    "ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
+    "ListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
+    "ListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
+    "ListRotationsRequestListRotationsPaginateTypeDef",
     "ListEngagementsRequestListEngagementsPaginateTypeDef",
     "ListEngagementsRequestRequestTypeDef",
     "ListPageReceiptsResultTypeDef",
     "ListPageResolutionsResultTypeDef",
     "ListPagesByContactResultTypeDef",
     "ListPagesByEngagementResultTypeDef",
     "ListRotationOverridesResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "RotationShiftTypeDef",
     "ListContactChannelsResultTypeDef",
+    "StageOutputTypeDef",
     "StageTypeDef",
+    "RecurrenceSettingsOutputTypeDef",
     "RecurrenceSettingsTypeDef",
     "ListPreviewRotationShiftsResultTypeDef",
     "ListRotationShiftsResultTypeDef",
+    "PlanOutputTypeDef",
     "PlanTypeDef",
-    "CreateRotationRequestRequestTypeDef",
     "GetRotationResultTypeDef",
+    "RotationTypeDef",
+    "CreateRotationRequestRequestTypeDef",
     "ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     "ListPreviewRotationShiftsRequestRequestTypeDef",
-    "RotationTypeDef",
     "UpdateRotationRequestRequestTypeDef",
-    "CreateContactRequestRequestTypeDef",
     "GetContactResultTypeDef",
+    "CreateContactRequestRequestTypeDef",
     "UpdateContactRequestRequestTypeDef",
     "ListRotationsResultTypeDef",
 )
 
 _RequiredAcceptPageRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptPageRequestRequestTypeDef",
     {
@@ -161,14 +173,33 @@
     "ActivateContactChannelRequestRequestTypeDef",
     {
         "ContactChannelId": str,
         "ActivationCode": str,
     },
 )
 
+_RequiredChannelTargetInfoOutputTypeDef = TypedDict(
+    "_RequiredChannelTargetInfoOutputTypeDef",
+    {
+        "ContactChannelId": str,
+    },
+)
+_OptionalChannelTargetInfoOutputTypeDef = TypedDict(
+    "_OptionalChannelTargetInfoOutputTypeDef",
+    {
+        "RetryIntervalInMinutes": int,
+    },
+    total=False,
+)
+
+class ChannelTargetInfoOutputTypeDef(
+    _RequiredChannelTargetInfoOutputTypeDef, _OptionalChannelTargetInfoOutputTypeDef
+):
+    pass
+
 _RequiredChannelTargetInfoTypeDef = TypedDict(
     "_RequiredChannelTargetInfoTypeDef",
     {
         "ContactChannelId": str,
     },
 )
 _OptionalChannelTargetInfoTypeDef = TypedDict(
@@ -180,22 +211,49 @@
 )
 
 class ChannelTargetInfoTypeDef(
     _RequiredChannelTargetInfoTypeDef, _OptionalChannelTargetInfoTypeDef
 ):
     pass
 
+ContactChannelAddressOutputTypeDef = TypedDict(
+    "ContactChannelAddressOutputTypeDef",
+    {
+        "SimpleAddress": str,
+    },
+    total=False,
+)
+
 ContactChannelAddressTypeDef = TypedDict(
     "ContactChannelAddressTypeDef",
     {
         "SimpleAddress": str,
     },
     total=False,
 )
 
+_RequiredContactTargetInfoOutputTypeDef = TypedDict(
+    "_RequiredContactTargetInfoOutputTypeDef",
+    {
+        "IsEssential": bool,
+    },
+)
+_OptionalContactTargetInfoOutputTypeDef = TypedDict(
+    "_OptionalContactTargetInfoOutputTypeDef",
+    {
+        "ContactId": str,
+    },
+    total=False,
+)
+
+class ContactTargetInfoOutputTypeDef(
+    _RequiredContactTargetInfoOutputTypeDef, _OptionalContactTargetInfoOutputTypeDef
+):
+    pass
+
 _RequiredContactTargetInfoTypeDef = TypedDict(
     "_RequiredContactTargetInfoTypeDef",
     {
         "IsEssential": bool,
     },
 )
 _OptionalContactTargetInfoTypeDef = TypedDict(
@@ -226,47 +284,50 @@
     },
     total=False,
 )
 
 class ContactTypeDef(_RequiredContactTypeDef, _OptionalContactTypeDef):
     pass
 
+HandOffTimeOutputTypeDef = TypedDict(
+    "HandOffTimeOutputTypeDef",
+    {
+        "HourOfDay": int,
+        "MinuteOfHour": int,
+    },
+)
+
 HandOffTimeTypeDef = TypedDict(
     "HandOffTimeTypeDef",
     {
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
 )
 
-CreateContactChannelResultTypeDef = TypedDict(
-    "CreateContactChannelResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ContactChannelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-CreateContactResultTypeDef = TypedDict(
-    "CreateContactResultTypeDef",
-    {
-        "ContactArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateRotationOverrideRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRotationOverrideRequestRequestTypeDef",
     {
         "RotationId": str,
         "NewContactIds": Sequence[str],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -282,30 +343,14 @@
 
 class CreateRotationOverrideRequestRequestTypeDef(
     _RequiredCreateRotationOverrideRequestRequestTypeDef,
     _OptionalCreateRotationOverrideRequestRequestTypeDef,
 ):
     pass
 
-CreateRotationOverrideResultTypeDef = TypedDict(
-    "CreateRotationOverrideResultTypeDef",
-    {
-        "RotationOverrideId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateRotationResultTypeDef = TypedDict(
-    "CreateRotationResultTypeDef",
-    {
-        "RotationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeactivateContactChannelRequestRequestTypeDef = TypedDict(
     "DeactivateContactChannelRequestRequestTypeDef",
     {
         "ContactChannelId": str,
     },
 )
 
@@ -341,57 +386,21 @@
 DescribeEngagementRequestRequestTypeDef = TypedDict(
     "DescribeEngagementRequestRequestTypeDef",
     {
         "EngagementId": str,
     },
 )
 
-DescribeEngagementResultTypeDef = TypedDict(
-    "DescribeEngagementResultTypeDef",
-    {
-        "ContactArn": str,
-        "EngagementArn": str,
-        "Sender": str,
-        "Subject": str,
-        "Content": str,
-        "PublicSubject": str,
-        "PublicContent": str,
-        "IncidentId": str,
-        "StartTime": datetime,
-        "StopTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribePageRequestRequestTypeDef = TypedDict(
     "DescribePageRequestRequestTypeDef",
     {
         "PageId": str,
     },
 )
 
-DescribePageResultTypeDef = TypedDict(
-    "DescribePageResultTypeDef",
-    {
-        "PageArn": str,
-        "EngagementArn": str,
-        "ContactArn": str,
-        "Sender": str,
-        "Subject": str,
-        "Content": str,
-        "PublicSubject": str,
-        "PublicContent": str,
-        "IncidentId": str,
-        "SentTime": datetime,
-        "ReadTime": datetime,
-        "DeliveryTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEngagementTypeDef = TypedDict(
     "_RequiredEngagementTypeDef",
     {
         "EngagementArn": str,
         "ContactArn": str,
         "Sender": str,
     },
@@ -419,23 +428,14 @@
 GetContactPolicyRequestRequestTypeDef = TypedDict(
     "GetContactPolicyRequestRequestTypeDef",
     {
         "ContactArn": str,
     },
 )
 
-GetContactPolicyResultTypeDef = TypedDict(
-    "GetContactPolicyResultTypeDef",
-    {
-        "ContactArn": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetContactRequestRequestTypeDef = TypedDict(
     "GetContactRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 
@@ -443,54 +443,31 @@
     "GetRotationOverrideRequestRequestTypeDef",
     {
         "RotationId": str,
         "RotationOverrideId": str,
     },
 )
 
-GetRotationOverrideResultTypeDef = TypedDict(
-    "GetRotationOverrideResultTypeDef",
-    {
-        "RotationOverrideId": str,
-        "RotationArn": str,
-        "NewContactIds": List[str],
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "CreateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRotationRequestRequestTypeDef = TypedDict(
     "GetRotationRequestRequestTypeDef",
     {
         "RotationId": str,
     },
 )
 
-_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
-    "_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef",
-    {
-        "ContactId": str,
-    },
-)
-_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
-    "_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef",
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
 
-class ListContactChannelsRequestListContactChannelsPaginateTypeDef(
-    _RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef,
-    _OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef,
-):
-    pass
-
 _RequiredListContactChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactChannelsRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 _OptionalListContactChannelsRequestRequestTypeDef = TypedDict(
@@ -504,24 +481,14 @@
 
 class ListContactChannelsRequestRequestTypeDef(
     _RequiredListContactChannelsRequestRequestTypeDef,
     _OptionalListContactChannelsRequestRequestTypeDef,
 ):
     pass
 
-ListContactsRequestListContactsPaginateTypeDef = TypedDict(
-    "ListContactsRequestListContactsPaginateTypeDef",
-    {
-        "AliasPrefix": str,
-        "Type": ContactTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListContactsRequestRequestTypeDef = TypedDict(
     "ListContactsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "AliasPrefix": str,
         "Type": ContactTypeType,
@@ -534,34 +501,14 @@
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
-    "_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
-    {
-        "PageId": str,
-    },
-)
-_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
-    "_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPageReceiptsRequestListPageReceiptsPaginateTypeDef(
-    _RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
-    _OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPageReceiptsRequestRequestTypeDef = TypedDict(
     "_RequiredListPageReceiptsRequestRequestTypeDef",
     {
         "PageId": str,
     },
 )
 _OptionalListPageReceiptsRequestRequestTypeDef = TypedDict(
@@ -593,34 +540,14 @@
     },
     total=False,
 )
 
 class ReceiptTypeDef(_RequiredReceiptTypeDef, _OptionalReceiptTypeDef):
     pass
 
-_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
-    "_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
-    {
-        "PageId": str,
-    },
-)
-_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
-    "_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPageResolutionsRequestListPageResolutionsPaginateTypeDef(
-    _RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
-    _OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPageResolutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPageResolutionsRequestRequestTypeDef",
     {
         "PageId": str,
     },
 )
 _OptionalListPageResolutionsRequestRequestTypeDef = TypedDict(
@@ -653,34 +580,14 @@
 )
 
 class ResolutionContactTypeDef(
     _RequiredResolutionContactTypeDef, _OptionalResolutionContactTypeDef
 ):
     pass
 
-_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
-    "_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef",
-    {
-        "ContactId": str,
-    },
-)
-_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
-    "_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPagesByContactRequestListPagesByContactPaginateTypeDef(
-    _RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef,
-    _OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef,
-):
-    pass
-
 _RequiredListPagesByContactRequestRequestTypeDef = TypedDict(
     "_RequiredListPagesByContactRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 _OptionalListPagesByContactRequestRequestTypeDef = TypedDict(
@@ -717,34 +624,14 @@
     },
     total=False,
 )
 
 class PageTypeDef(_RequiredPageTypeDef, _OptionalPageTypeDef):
     pass
 
-_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
-    "_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
-    {
-        "EngagementId": str,
-    },
-)
-_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
-    "_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef(
-    _RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
-    _OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
-):
-    pass
-
 _RequiredListPagesByEngagementRequestRequestTypeDef = TypedDict(
     "_RequiredListPagesByEngagementRequestRequestTypeDef",
     {
         "EngagementId": str,
     },
 )
 _OptionalListPagesByEngagementRequestRequestTypeDef = TypedDict(
@@ -768,36 +655,14 @@
         "NewMembers": Sequence[str],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
-    "_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
-    {
-        "RotationId": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
-    "_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRotationOverridesRequestListRotationOverridesPaginateTypeDef(
-    _RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
-    _OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
-):
-    pass
-
 _RequiredListRotationOverridesRequestRequestTypeDef = TypedDict(
     "_RequiredListRotationOverridesRequestRequestTypeDef",
     {
         "RotationId": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
@@ -824,36 +689,14 @@
         "NewContactIds": List[str],
         "StartTime": datetime,
         "EndTime": datetime,
         "CreateTime": datetime,
     },
 )
 
-_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
-    "_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
-    {
-        "RotationId": str,
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
-    "_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRotationShiftsRequestListRotationShiftsPaginateTypeDef(
-    _RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
-    _OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
-):
-    pass
-
 _RequiredListRotationShiftsRequestRequestTypeDef = TypedDict(
     "_RequiredListRotationShiftsRequestRequestTypeDef",
     {
         "RotationId": str,
         "EndTime": Union[datetime, str],
     },
 )
@@ -869,23 +712,14 @@
 
 class ListRotationShiftsRequestRequestTypeDef(
     _RequiredListRotationShiftsRequestRequestTypeDef,
     _OptionalListRotationShiftsRequestRequestTypeDef,
 ):
     pass
 
-ListRotationsRequestListRotationsPaginateTypeDef = TypedDict(
-    "ListRotationsRequestListRotationsPaginateTypeDef",
-    {
-        "RotationNamePrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRotationsRequestRequestTypeDef = TypedDict(
     "ListRotationsRequestRequestTypeDef",
     {
         "RotationNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -895,43 +729,31 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Key": str,
+        "Value": str,
     },
     total=False,
 )
 
 PutContactPolicyRequestRequestTypeDef = TypedDict(
     "PutContactPolicyRequestRequestTypeDef",
     {
         "ContactArn": str,
         "Policy": str,
     },
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
 ShiftDetailsTypeDef = TypedDict(
     "ShiftDetailsTypeDef",
     {
         "OverriddenContactIds": List[str],
     },
 )
 
@@ -963,22 +785,14 @@
 )
 
 class StartEngagementRequestRequestTypeDef(
     _RequiredStartEngagementRequestRequestTypeDef, _OptionalStartEngagementRequestRequestTypeDef
 ):
     pass
 
-StartEngagementResultTypeDef = TypedDict(
-    "StartEngagementResultTypeDef",
-    {
-        "EngagementArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStopEngagementRequestRequestTypeDef = TypedDict(
     "_RequiredStopEngagementRequestRequestTypeDef",
     {
         "EngagementId": str,
     },
 )
 _OptionalStopEngagementRequestRequestTypeDef = TypedDict(
@@ -1004,15 +818,15 @@
 
 _RequiredContactChannelTypeDef = TypedDict(
     "_RequiredContactChannelTypeDef",
     {
         "ContactChannelArn": str,
         "ContactArn": str,
         "Name": str,
-        "DeliveryAddress": ContactChannelAddressTypeDef,
+        "DeliveryAddress": ContactChannelAddressOutputTypeDef,
         "ActivationStatus": ActivationStatusType,
     },
 )
 _OptionalContactChannelTypeDef = TypedDict(
     "_OptionalContactChannelTypeDef",
     {
         "Type": ChannelTypeType,
@@ -1043,27 +857,14 @@
 
 class CreateContactChannelRequestRequestTypeDef(
     _RequiredCreateContactChannelRequestRequestTypeDef,
     _OptionalCreateContactChannelRequestRequestTypeDef,
 ):
     pass
 
-GetContactChannelResultTypeDef = TypedDict(
-    "GetContactChannelResultTypeDef",
-    {
-        "ContactArn": str,
-        "ContactChannelArn": str,
-        "Name": str,
-        "Type": ChannelTypeType,
-        "DeliveryAddress": ContactChannelAddressTypeDef,
-        "ActivationStatus": ActivationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateContactChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactChannelRequestRequestTypeDef",
     {
         "ContactChannelId": str,
     },
 )
 _OptionalUpdateContactChannelRequestRequestTypeDef = TypedDict(
@@ -1077,29 +878,54 @@
 
 class UpdateContactChannelRequestRequestTypeDef(
     _RequiredUpdateContactChannelRequestRequestTypeDef,
     _OptionalUpdateContactChannelRequestRequestTypeDef,
 ):
     pass
 
+TargetOutputTypeDef = TypedDict(
+    "TargetOutputTypeDef",
+    {
+        "ChannelTargetInfo": ChannelTargetInfoOutputTypeDef,
+        "ContactTargetInfo": ContactTargetInfoOutputTypeDef,
+    },
+    total=False,
+)
+
 TargetTypeDef = TypedDict(
     "TargetTypeDef",
     {
         "ChannelTargetInfo": ChannelTargetInfoTypeDef,
         "ContactTargetInfo": ContactTargetInfoTypeDef,
     },
     total=False,
 )
 
-ListContactsResultTypeDef = TypedDict(
-    "ListContactsResultTypeDef",
+CoverageTimeOutputTypeDef = TypedDict(
+    "CoverageTimeOutputTypeDef",
     {
-        "NextToken": str,
-        "Contacts": List[ContactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Start": HandOffTimeOutputTypeDef,
+        "End": HandOffTimeOutputTypeDef,
+    },
+    total=False,
+)
+
+MonthlySettingOutputTypeDef = TypedDict(
+    "MonthlySettingOutputTypeDef",
+    {
+        "DayOfMonth": int,
+        "HandOffTime": HandOffTimeOutputTypeDef,
+    },
+)
+
+WeeklySettingOutputTypeDef = TypedDict(
+    "WeeklySettingOutputTypeDef",
+    {
+        "DayOfWeek": DayOfWeekType,
+        "HandOffTime": HandOffTimeOutputTypeDef,
     },
 )
 
 CoverageTimeTypeDef = TypedDict(
     "CoverageTimeTypeDef",
     {
         "Start": HandOffTimeTypeDef,
@@ -1120,19 +946,131 @@
     "WeeklySettingTypeDef",
     {
         "DayOfWeek": DayOfWeekType,
         "HandOffTime": HandOffTimeTypeDef,
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
+CreateContactChannelResultTypeDef = TypedDict(
+    "CreateContactChannelResultTypeDef",
+    {
+        "ContactChannelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateContactResultTypeDef = TypedDict(
+    "CreateContactResultTypeDef",
+    {
+        "ContactArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRotationOverrideResultTypeDef = TypedDict(
+    "CreateRotationOverrideResultTypeDef",
+    {
+        "RotationOverrideId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRotationResultTypeDef = TypedDict(
+    "CreateRotationResultTypeDef",
+    {
+        "RotationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEngagementResultTypeDef = TypedDict(
+    "DescribeEngagementResultTypeDef",
+    {
+        "ContactArn": str,
+        "EngagementArn": str,
+        "Sender": str,
+        "Subject": str,
+        "Content": str,
+        "PublicSubject": str,
+        "PublicContent": str,
+        "IncidentId": str,
+        "StartTime": datetime,
+        "StopTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePageResultTypeDef = TypedDict(
+    "DescribePageResultTypeDef",
+    {
+        "PageArn": str,
+        "EngagementArn": str,
+        "ContactArn": str,
+        "Sender": str,
+        "Subject": str,
+        "Content": str,
+        "PublicSubject": str,
+        "PublicContent": str,
+        "IncidentId": str,
+        "SentTime": datetime,
+        "ReadTime": datetime,
+        "DeliveryTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContactChannelResultTypeDef = TypedDict(
+    "GetContactChannelResultTypeDef",
+    {
+        "ContactArn": str,
+        "ContactChannelArn": str,
+        "Name": str,
+        "Type": ChannelTypeType,
+        "DeliveryAddress": ContactChannelAddressOutputTypeDef,
+        "ActivationStatus": ActivationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContactPolicyResultTypeDef = TypedDict(
+    "GetContactPolicyResultTypeDef",
+    {
+        "ContactArn": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRotationOverrideResultTypeDef = TypedDict(
+    "GetRotationOverrideResultTypeDef",
+    {
+        "RotationOverrideId": str,
+        "RotationArn": str,
+        "NewContactIds": List[str],
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "CreateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListContactsResultTypeDef = TypedDict(
+    "ListContactsResultTypeDef",
+    {
+        "NextToken": str,
+        "Contacts": List[ContactTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartEngagementResultTypeDef = TypedDict(
+    "StartEngagementResultTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EngagementArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -1141,24 +1079,187 @@
 )
 
 ListEngagementsResultTypeDef = TypedDict(
     "ListEngagementsResultTypeDef",
     {
         "NextToken": str,
         "Engagements": List[EngagementTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
+    "_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef",
+    {
+        "ContactId": str,
+    },
+)
+_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
+    "_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListContactChannelsRequestListContactChannelsPaginateTypeDef(
+    _RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef,
+    _OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef,
+):
+    pass
+
+ListContactsRequestListContactsPaginateTypeDef = TypedDict(
+    "ListContactsRequestListContactsPaginateTypeDef",
+    {
+        "AliasPrefix": str,
+        "Type": ContactTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
+    "_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
+    {
+        "PageId": str,
+    },
+)
+_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
+    "_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPageReceiptsRequestListPageReceiptsPaginateTypeDef(
+    _RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
+    _OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
+):
+    pass
+
+_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
+    "_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
+    {
+        "PageId": str,
+    },
+)
+_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
+    "_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPageResolutionsRequestListPageResolutionsPaginateTypeDef(
+    _RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
+    _OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
+    "_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef",
+    {
+        "ContactId": str,
+    },
+)
+_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
+    "_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+class ListPagesByContactRequestListPagesByContactPaginateTypeDef(
+    _RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef,
+    _OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef,
+):
+    pass
+
+_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
+    "_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
+    {
+        "EngagementId": str,
+    },
+)
+_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
+    "_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef(
+    _RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
+    _OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
+):
+    pass
+
+_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
+    "_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
+    {
+        "RotationId": str,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+    },
+)
+_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
+    "_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRotationOverridesRequestListRotationOverridesPaginateTypeDef(
+    _RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
+    _OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
+):
+    pass
+
+_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
+    "_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
+    {
+        "RotationId": str,
+        "EndTime": Union[datetime, str],
+    },
+)
+_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
+    "_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRotationShiftsRequestListRotationShiftsPaginateTypeDef(
+    _RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
+    _OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
+):
+    pass
+
+ListRotationsRequestListRotationsPaginateTypeDef = TypedDict(
+    "ListRotationsRequestListRotationsPaginateTypeDef",
+    {
+        "RotationNamePrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListEngagementsRequestListEngagementsPaginateTypeDef = TypedDict(
     "ListEngagementsRequestListEngagementsPaginateTypeDef",
     {
         "IncidentId": str,
         "TimeRangeValue": TimeRangeTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListEngagementsRequestRequestTypeDef = TypedDict(
     "ListEngagementsRequestRequestTypeDef",
     {
@@ -1171,51 +1272,59 @@
 )
 
 ListPageReceiptsResultTypeDef = TypedDict(
     "ListPageReceiptsResultTypeDef",
     {
         "NextToken": str,
         "Receipts": List[ReceiptTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPageResolutionsResultTypeDef = TypedDict(
     "ListPageResolutionsResultTypeDef",
     {
         "NextToken": str,
         "PageResolutions": List[ResolutionContactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPagesByContactResultTypeDef = TypedDict(
     "ListPagesByContactResultTypeDef",
     {
         "NextToken": str,
         "Pages": List[PageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPagesByEngagementResultTypeDef = TypedDict(
     "ListPagesByEngagementResultTypeDef",
     {
         "NextToken": str,
         "Pages": List[PageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRotationOverridesResultTypeDef = TypedDict(
     "ListRotationOverridesResultTypeDef",
     {
         "RotationOverrides": List[RotationOverrideTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRotationShiftTypeDef = TypedDict(
     "_RequiredRotationShiftTypeDef",
     {
         "StartTime": datetime,
@@ -1236,26 +1345,57 @@
     pass
 
 ListContactChannelsResultTypeDef = TypedDict(
     "ListContactChannelsResultTypeDef",
     {
         "NextToken": str,
         "ContactChannels": List[ContactChannelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StageOutputTypeDef = TypedDict(
+    "StageOutputTypeDef",
+    {
+        "DurationInMinutes": int,
+        "Targets": List[TargetOutputTypeDef],
     },
 )
 
 StageTypeDef = TypedDict(
     "StageTypeDef",
     {
         "DurationInMinutes": int,
         "Targets": Sequence[TargetTypeDef],
     },
 )
 
+_RequiredRecurrenceSettingsOutputTypeDef = TypedDict(
+    "_RequiredRecurrenceSettingsOutputTypeDef",
+    {
+        "NumberOfOnCalls": int,
+        "RecurrenceMultiplier": int,
+    },
+)
+_OptionalRecurrenceSettingsOutputTypeDef = TypedDict(
+    "_OptionalRecurrenceSettingsOutputTypeDef",
+    {
+        "MonthlySettings": List[MonthlySettingOutputTypeDef],
+        "WeeklySettings": List[WeeklySettingOutputTypeDef],
+        "DailySettings": List[HandOffTimeOutputTypeDef],
+        "ShiftCoverages": Dict[DayOfWeekType, List[CoverageTimeOutputTypeDef]],
+    },
+    total=False,
+)
+
+class RecurrenceSettingsOutputTypeDef(
+    _RequiredRecurrenceSettingsOutputTypeDef, _OptionalRecurrenceSettingsOutputTypeDef
+):
+    pass
+
 _RequiredRecurrenceSettingsTypeDef = TypedDict(
     "_RequiredRecurrenceSettingsTypeDef",
     {
         "NumberOfOnCalls": int,
         "RecurrenceMultiplier": int,
     },
 )
@@ -1276,36 +1416,79 @@
     pass
 
 ListPreviewRotationShiftsResultTypeDef = TypedDict(
     "ListPreviewRotationShiftsResultTypeDef",
     {
         "RotationShifts": List[RotationShiftTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRotationShiftsResultTypeDef = TypedDict(
     "ListRotationShiftsResultTypeDef",
     {
         "RotationShifts": List[RotationShiftTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PlanOutputTypeDef = TypedDict(
+    "PlanOutputTypeDef",
+    {
+        "Stages": List[StageOutputTypeDef],
+        "RotationIds": List[str],
     },
+    total=False,
 )
 
 PlanTypeDef = TypedDict(
     "PlanTypeDef",
     {
         "Stages": Sequence[StageTypeDef],
         "RotationIds": Sequence[str],
     },
     total=False,
 )
 
+GetRotationResultTypeDef = TypedDict(
+    "GetRotationResultTypeDef",
+    {
+        "RotationArn": str,
+        "Name": str,
+        "ContactIds": List[str],
+        "StartTime": datetime,
+        "TimeZoneId": str,
+        "Recurrence": RecurrenceSettingsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredRotationTypeDef = TypedDict(
+    "_RequiredRotationTypeDef",
+    {
+        "RotationArn": str,
+        "Name": str,
+    },
+)
+_OptionalRotationTypeDef = TypedDict(
+    "_OptionalRotationTypeDef",
+    {
+        "ContactIds": List[str],
+        "StartTime": datetime,
+        "TimeZoneId": str,
+        "Recurrence": RecurrenceSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+class RotationTypeDef(_RequiredRotationTypeDef, _OptionalRotationTypeDef):
+    pass
+
 _RequiredCreateRotationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRotationRequestRequestTypeDef",
     {
         "Name": str,
         "ContactIds": Sequence[str],
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
@@ -1322,27 +1505,14 @@
 )
 
 class CreateRotationRequestRequestTypeDef(
     _RequiredCreateRotationRequestRequestTypeDef, _OptionalCreateRotationRequestRequestTypeDef
 ):
     pass
 
-GetRotationResultTypeDef = TypedDict(
-    "GetRotationResultTypeDef",
-    {
-        "RotationArn": str,
-        "Name": str,
-        "ContactIds": List[str],
-        "StartTime": datetime,
-        "TimeZoneId": str,
-        "Recurrence": RecurrenceSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef = TypedDict(
     "_RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     {
         "EndTime": Union[datetime, str],
         "Members": Sequence[str],
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
@@ -1350,15 +1520,15 @@
 )
 _OptionalListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef = TypedDict(
     "_OptionalListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     {
         "RotationStartTime": Union[datetime, str],
         "StartTime": Union[datetime, str],
         "Overrides": Sequence[PreviewOverrideTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef(
     _RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef,
     _OptionalListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef,
@@ -1388,35 +1558,14 @@
 
 class ListPreviewRotationShiftsRequestRequestTypeDef(
     _RequiredListPreviewRotationShiftsRequestRequestTypeDef,
     _OptionalListPreviewRotationShiftsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredRotationTypeDef = TypedDict(
-    "_RequiredRotationTypeDef",
-    {
-        "RotationArn": str,
-        "Name": str,
-    },
-)
-_OptionalRotationTypeDef = TypedDict(
-    "_OptionalRotationTypeDef",
-    {
-        "ContactIds": List[str],
-        "StartTime": datetime,
-        "TimeZoneId": str,
-        "Recurrence": RecurrenceSettingsTypeDef,
-    },
-    total=False,
-)
-
-class RotationTypeDef(_RequiredRotationTypeDef, _OptionalRotationTypeDef):
-    pass
-
 _RequiredUpdateRotationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRotationRequestRequestTypeDef",
     {
         "RotationId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
     },
 )
@@ -1431,14 +1580,26 @@
 )
 
 class UpdateRotationRequestRequestTypeDef(
     _RequiredUpdateRotationRequestRequestTypeDef, _OptionalUpdateRotationRequestRequestTypeDef
 ):
     pass
 
+GetContactResultTypeDef = TypedDict(
+    "GetContactResultTypeDef",
+    {
+        "ContactArn": str,
+        "Alias": str,
+        "DisplayName": str,
+        "Type": ContactTypeType,
+        "Plan": PlanOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateContactRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContactRequestRequestTypeDef",
     {
         "Alias": str,
         "Type": ContactTypeType,
         "Plan": PlanTypeDef,
     },
@@ -1454,26 +1615,14 @@
 )
 
 class CreateContactRequestRequestTypeDef(
     _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
 ):
     pass
 
-GetContactResultTypeDef = TypedDict(
-    "GetContactResultTypeDef",
-    {
-        "ContactArn": str,
-        "Alias": str,
-        "DisplayName": str,
-        "Type": ContactTypeType,
-        "Plan": PlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateContactRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 _OptionalUpdateContactRequestRequestTypeDef = TypedDict(
@@ -1491,10 +1640,10 @@
     pass
 
 ListRotationsResultTypeDef = TypedDict(
     "ListRotationsResultTypeDef",
     {
         "NextToken": str,
         "Rotations": List[RotationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts.egg-info/PKG-INFO` & `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-contacts
-Version: 1.28.0
-Summary: Type annotations for boto3.SSMContacts 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SSMContacts 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ssm-contacts"></a>
 
 # mypy-boto3-ssm-contacts
 
 [![PyPI - mypy-boto3-ssm-contacts](https://img.shields.io/pypi/v/mypy-boto3-ssm-contacts.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-contacts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-contacts.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-contacts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm-contacts?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm-contacts)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-contacts)](https://pepy.tech/project/mypy-boto3-ssm-contacts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMContacts 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
+[boto3.SSMContacts 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
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
 [mypy-boto3-ssm-contacts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -375,110 +375,122 @@
 `mypy_boto3_ssm_contacts.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ssm_contacts.type_defs import (
     AcceptPageRequestRequestTypeDef,
     ActivateContactChannelRequestRequestTypeDef,
+    ChannelTargetInfoOutputTypeDef,
     ChannelTargetInfoTypeDef,
+    ContactChannelAddressOutputTypeDef,
     ContactChannelAddressTypeDef,
+    ContactTargetInfoOutputTypeDef,
     ContactTargetInfoTypeDef,
     ContactTypeDef,
+    HandOffTimeOutputTypeDef,
     HandOffTimeTypeDef,
-    CreateContactChannelResultTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
-    CreateContactResultTypeDef,
     CreateRotationOverrideRequestRequestTypeDef,
-    CreateRotationOverrideResultTypeDef,
-    CreateRotationResultTypeDef,
     DeactivateContactChannelRequestRequestTypeDef,
     DeleteContactChannelRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
     DeleteRotationOverrideRequestRequestTypeDef,
     DeleteRotationRequestRequestTypeDef,
     DescribeEngagementRequestRequestTypeDef,
-    DescribeEngagementResultTypeDef,
     DescribePageRequestRequestTypeDef,
-    DescribePageResultTypeDef,
     EngagementTypeDef,
     GetContactChannelRequestRequestTypeDef,
     GetContactPolicyRequestRequestTypeDef,
-    GetContactPolicyResultTypeDef,
     GetContactRequestRequestTypeDef,
     GetRotationOverrideRequestRequestTypeDef,
-    GetRotationOverrideResultTypeDef,
     GetRotationRequestRequestTypeDef,
-    ListContactChannelsRequestListContactChannelsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListContactChannelsRequestRequestTypeDef,
-    ListContactsRequestListContactsPaginateTypeDef,
     ListContactsRequestRequestTypeDef,
     TimeRangeTypeDef,
-    ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
     ListPageReceiptsRequestRequestTypeDef,
     ReceiptTypeDef,
-    ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
     ListPageResolutionsRequestRequestTypeDef,
     ResolutionContactTypeDef,
-    ListPagesByContactRequestListPagesByContactPaginateTypeDef,
     ListPagesByContactRequestRequestTypeDef,
     PageTypeDef,
-    ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
     ListPagesByEngagementRequestRequestTypeDef,
     PreviewOverrideTypeDef,
-    ListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
     ListRotationOverridesRequestRequestTypeDef,
     RotationOverrideTypeDef,
-    ListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
     ListRotationShiftsRequestRequestTypeDef,
-    ListRotationsRequestListRotationsPaginateTypeDef,
     ListRotationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     PutContactPolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ShiftDetailsTypeDef,
     SendActivationCodeRequestRequestTypeDef,
     StartEngagementRequestRequestTypeDef,
-    StartEngagementResultTypeDef,
     StopEngagementRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ContactChannelTypeDef,
     CreateContactChannelRequestRequestTypeDef,
-    GetContactChannelResultTypeDef,
     UpdateContactChannelRequestRequestTypeDef,
+    TargetOutputTypeDef,
     TargetTypeDef,
-    ListContactsResultTypeDef,
+    CoverageTimeOutputTypeDef,
+    MonthlySettingOutputTypeDef,
+    WeeklySettingOutputTypeDef,
     CoverageTimeTypeDef,
     MonthlySettingTypeDef,
     WeeklySettingTypeDef,
-    ListTagsForResourceResultTypeDef,
+    CreateContactChannelResultTypeDef,
+    CreateContactResultTypeDef,
+    CreateRotationOverrideResultTypeDef,
+    CreateRotationResultTypeDef,
+    DescribeEngagementResultTypeDef,
+    DescribePageResultTypeDef,
+    GetContactChannelResultTypeDef,
+    GetContactPolicyResultTypeDef,
+    GetRotationOverrideResultTypeDef,
+    ListContactsResultTypeDef,
+    StartEngagementResultTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEngagementsResultTypeDef,
+    ListContactChannelsRequestListContactChannelsPaginateTypeDef,
+    ListContactsRequestListContactsPaginateTypeDef,
+    ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
+    ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
+    ListPagesByContactRequestListPagesByContactPaginateTypeDef,
+    ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
+    ListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
+    ListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
+    ListRotationsRequestListRotationsPaginateTypeDef,
     ListEngagementsRequestListEngagementsPaginateTypeDef,
     ListEngagementsRequestRequestTypeDef,
     ListPageReceiptsResultTypeDef,
     ListPageResolutionsResultTypeDef,
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListRotationOverridesResultTypeDef,
+    ListTagsForResourceResultTypeDef,
     RotationShiftTypeDef,
     ListContactChannelsResultTypeDef,
+    StageOutputTypeDef,
     StageTypeDef,
+    RecurrenceSettingsOutputTypeDef,
     RecurrenceSettingsTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationShiftsResultTypeDef,
+    PlanOutputTypeDef,
     PlanTypeDef,
-    CreateRotationRequestRequestTypeDef,
     GetRotationResultTypeDef,
+    RotationTypeDef,
+    CreateRotationRequestRequestTypeDef,
     ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef,
     ListPreviewRotationShiftsRequestRequestTypeDef,
-    RotationTypeDef,
     UpdateRotationRequestRequestTypeDef,
-    CreateContactRequestRequestTypeDef,
     GetContactResultTypeDef,
+    CreateContactRequestRequestTypeDef,
     UpdateContactRequestRequestTypeDef,
     ListRotationsResultTypeDef,
 )
 
 
 def get_structure() -> AcceptPageRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-ssm-contacts-1.28.0/mypy_boto3_ssm_contacts.egg-info/SOURCES.txt` & `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.0/setup.py` & `mypy-boto3-ssm-contacts-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ssm-contacts",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_ssm_contacts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSMContacts 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.SSMContacts 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

