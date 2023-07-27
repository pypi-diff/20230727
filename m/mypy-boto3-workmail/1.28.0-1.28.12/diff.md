# Comparing `tmp/mypy-boto3-workmail-1.28.0.tar.gz` & `tmp/mypy-boto3-workmail-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workmail-1.28.0.tar", last modified: Thu Jul  6 21:00:52 2023, max compression
+gzip compressed data, was "mypy-boto3-workmail-1.28.12.tar", last modified: Thu Jul 27 11:49:50 2023, max compression
```

## Comparing `mypy-boto3-workmail-1.28.0.tar` & `mypy-boto3-workmail-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:52.494461 mypy-boto3-workmail-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:58:14.000000 mypy-boto3-workmail-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21166 2023-07-06 21:00:52.494461 mypy-boto3-workmail-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19677 2023-07-06 20:58:14.000000 mypy-boto3-workmail-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:52.494461 mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-06 20:58:14.000000 mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-06 20:58:14.000000 mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:58:14.000000 mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57101 2023-07-06 20:58:14.000000 mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57005 2023-07-06 20:58:14.000000 mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-07-06 20:58:15.000000 mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-07-06 20:58:15.000000 mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-07-06 20:58:15.000000 mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-07-06 20:58:14.000000 mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:14.000000 mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59791 2023-07-06 20:58:16.000000 mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59712 2023-07-06 20:58:16.000000 mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:58:14.000000 mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:52.494461 mypy-boto3-workmail-1.28.0/mypy_boto3_workmail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21166 2023-07-06 21:00:52.000000 mypy-boto3-workmail-1.28.0/mypy_boto3_workmail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 21:00:52.000000 mypy-boto3-workmail-1.28.0/mypy_boto3_workmail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:52.000000 mypy-boto3-workmail-1.28.0/mypy_boto3_workmail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:52.000000 mypy-boto3-workmail-1.28.0/mypy_boto3_workmail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:52.000000 mypy-boto3-workmail-1.28.0/mypy_boto3_workmail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:00:52.000000 mypy-boto3-workmail-1.28.0/mypy_boto3_workmail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:52.494461 mypy-boto3-workmail-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:58:14.000000 mypy-boto3-workmail-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:50.277499 mypy-boto3-workmail-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:54.000000 mypy-boto3-workmail-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21327 2023-07-27 11:49:50.277499 mypy-boto3-workmail-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-07-27 11:48:54.000000 mypy-boto3-workmail-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:50.265499 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-27 11:48:55.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-27 11:48:54.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:48:55.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57101 2023-07-27 11:48:55.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57005 2023-07-27 11:48:55.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-07-27 11:48:55.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-07-27 11:48:55.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-07-27 11:48:55.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-07-27 11:48:55.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:55.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    61470 2023-07-27 11:48:57.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61387 2023-07-27 11:48:56.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:54.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:50.277499 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21327 2023-07-27 11:49:50.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 11:49:50.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:50.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:50.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:50.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:50.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:50.277499 mypy-boto3-workmail-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:48:54.000000 mypy-boto3-workmail-1.28.12/setup.py
```

### Comparing `mypy-boto3-workmail-1.28.0/LICENSE` & `mypy-boto3-workmail-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.0/PKG-INFO` & `mypy-boto3-workmail-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workmail
-Version: 1.28.0
-Summary: Type annotations for boto3.WorkMail 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.WorkMail 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-workmail"></a>
 
 # mypy-boto3-workmail
 
 [![PyPI - mypy-boto3-workmail](https://img.shields.io/pypi/v/mypy-boto3-workmail.svg?color=blue)](https://pypi.org/project/mypy-boto3-workmail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workmail.svg?color=blue)](https://pypi.org/project/mypy-boto3-workmail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workmail?color=blue)](https://pypistats.org/packages/mypy-boto3-workmail)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workmail)](https://pepy.tech/project/mypy-boto3-workmail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkMail 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
+[boto3.WorkMail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
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
 [mypy-boto3-workmail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -370,166 +370,171 @@
 
 ```python
 from mypy_boto3_workmail.type_defs import (
     AccessControlRuleTypeDef,
     AssociateDelegateToResourceRequestRequestTypeDef,
     AssociateMemberToGroupRequestRequestTypeDef,
     AssumeImpersonationRoleRequestRequestTypeDef,
-    AssumeImpersonationRoleResponseTypeDef,
-    LambdaAvailabilityProviderTypeDef,
+    ResponseMetadataTypeDef,
+    LambdaAvailabilityProviderOutputTypeDef,
     RedactedEwsAvailabilityProviderTypeDef,
+    BookingOptionsOutputTypeDef,
     BookingOptionsTypeDef,
     CancelMailboxExportJobRequestRequestTypeDef,
     CreateAliasRequestRequestTypeDef,
     EwsAvailabilityProviderTypeDef,
+    LambdaAvailabilityProviderTypeDef,
     CreateGroupRequestRequestTypeDef,
-    CreateGroupResponseTypeDef,
     ImpersonationRuleTypeDef,
-    CreateImpersonationRoleResponseTypeDef,
     CreateMobileDeviceAccessRuleRequestRequestTypeDef,
-    CreateMobileDeviceAccessRuleResponseTypeDef,
     DomainTypeDef,
-    CreateOrganizationResponseTypeDef,
     CreateResourceRequestRequestTypeDef,
-    CreateResourceResponseTypeDef,
     CreateUserRequestRequestTypeDef,
-    CreateUserResponseTypeDef,
     DelegateTypeDef,
     DeleteAccessControlRuleRequestRequestTypeDef,
     DeleteAliasRequestRequestTypeDef,
     DeleteAvailabilityConfigurationRequestRequestTypeDef,
     DeleteEmailMonitoringConfigurationRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteImpersonationRoleRequestRequestTypeDef,
     DeleteMailboxPermissionsRequestRequestTypeDef,
     DeleteMobileDeviceAccessOverrideRequestRequestTypeDef,
     DeleteMobileDeviceAccessRuleRequestRequestTypeDef,
     DeleteOrganizationRequestRequestTypeDef,
-    DeleteOrganizationResponseTypeDef,
     DeleteResourceRequestRequestTypeDef,
     DeleteRetentionPolicyRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeregisterFromWorkMailRequestRequestTypeDef,
     DeregisterMailDomainRequestRequestTypeDef,
     DescribeEmailMonitoringConfigurationRequestRequestTypeDef,
-    DescribeEmailMonitoringConfigurationResponseTypeDef,
     DescribeGroupRequestRequestTypeDef,
-    DescribeGroupResponseTypeDef,
     DescribeInboundDmarcSettingsRequestRequestTypeDef,
-    DescribeInboundDmarcSettingsResponseTypeDef,
     DescribeMailboxExportJobRequestRequestTypeDef,
-    DescribeMailboxExportJobResponseTypeDef,
     DescribeOrganizationRequestRequestTypeDef,
-    DescribeOrganizationResponseTypeDef,
     DescribeResourceRequestRequestTypeDef,
     DescribeUserRequestRequestTypeDef,
-    DescribeUserResponseTypeDef,
     DisassociateDelegateFromResourceRequestRequestTypeDef,
     DisassociateMemberFromGroupRequestRequestTypeDef,
     DnsRecordTypeDef,
+    FolderConfigurationOutputTypeDef,
     FolderConfigurationTypeDef,
     GetAccessControlEffectRequestRequestTypeDef,
-    GetAccessControlEffectResponseTypeDef,
     GetDefaultRetentionPolicyRequestRequestTypeDef,
     GetImpersonationRoleEffectRequestRequestTypeDef,
     ImpersonationMatchedRuleTypeDef,
     GetImpersonationRoleRequestRequestTypeDef,
+    ImpersonationRuleOutputTypeDef,
     GetMailDomainRequestRequestTypeDef,
     GetMailboxDetailsRequestRequestTypeDef,
-    GetMailboxDetailsResponseTypeDef,
     GetMobileDeviceAccessEffectRequestRequestTypeDef,
     MobileDeviceAccessMatchedRuleTypeDef,
     GetMobileDeviceAccessOverrideRequestRequestTypeDef,
-    GetMobileDeviceAccessOverrideResponseTypeDef,
     GroupTypeDef,
     ImpersonationRoleTypeDef,
     ListAccessControlRulesRequestRequestTypeDef,
-    ListAliasesRequestListAliasesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAliasesRequestRequestTypeDef,
-    ListAliasesResponseTypeDef,
-    ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
     ListAvailabilityConfigurationsRequestRequestTypeDef,
-    ListGroupMembersRequestListGroupMembersPaginateTypeDef,
     ListGroupMembersRequestRequestTypeDef,
     MemberTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListImpersonationRolesRequestRequestTypeDef,
     ListMailDomainsRequestRequestTypeDef,
     MailDomainSummaryTypeDef,
     ListMailboxExportJobsRequestRequestTypeDef,
     MailboxExportJobTypeDef,
-    ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
     ListMailboxPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
     ListMobileDeviceAccessOverridesRequestRequestTypeDef,
     MobileDeviceAccessOverrideTypeDef,
     ListMobileDeviceAccessRulesRequestRequestTypeDef,
     MobileDeviceAccessRuleTypeDef,
-    ListOrganizationsRequestListOrganizationsPaginateTypeDef,
     ListOrganizationsRequestRequestTypeDef,
     OrganizationSummaryTypeDef,
-    ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
     ListResourceDelegatesRequestRequestTypeDef,
-    ListResourcesRequestListResourcesPaginateTypeDef,
     ListResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
+    TagOutputTypeDef,
     ListUsersRequestRequestTypeDef,
     UserTypeDef,
-    PaginatorConfigTypeDef,
     PutAccessControlRuleRequestRequestTypeDef,
     PutEmailMonitoringConfigurationRequestRequestTypeDef,
     PutInboundDmarcSettingsRequestRequestTypeDef,
     PutMailboxPermissionsRequestRequestTypeDef,
     PutMobileDeviceAccessOverrideRequestRequestTypeDef,
     RegisterMailDomainRequestRequestTypeDef,
     RegisterToWorkMailRequestRequestTypeDef,
     ResetPasswordRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartMailboxExportJobRequestRequestTypeDef,
-    StartMailboxExportJobResponseTypeDef,
-    TestAvailabilityConfigurationResponseTypeDef,
+    TagTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDefaultMailDomainRequestRequestTypeDef,
     UpdateMailboxQuotaRequestRequestTypeDef,
     UpdateMobileDeviceAccessRuleRequestRequestTypeDef,
     UpdatePrimaryEmailAddressRequestRequestTypeDef,
+    AssumeImpersonationRoleResponseTypeDef,
+    CreateGroupResponseTypeDef,
+    CreateImpersonationRoleResponseTypeDef,
+    CreateMobileDeviceAccessRuleResponseTypeDef,
+    CreateOrganizationResponseTypeDef,
+    CreateResourceResponseTypeDef,
+    CreateUserResponseTypeDef,
+    DeleteOrganizationResponseTypeDef,
+    DescribeEmailMonitoringConfigurationResponseTypeDef,
+    DescribeGroupResponseTypeDef,
+    DescribeInboundDmarcSettingsResponseTypeDef,
+    DescribeMailboxExportJobResponseTypeDef,
+    DescribeOrganizationResponseTypeDef,
+    DescribeUserResponseTypeDef,
+    GetAccessControlEffectResponseTypeDef,
+    GetMailboxDetailsResponseTypeDef,
+    GetMobileDeviceAccessOverrideResponseTypeDef,
     ListAccessControlRulesResponseTypeDef,
+    ListAliasesResponseTypeDef,
+    StartMailboxExportJobResponseTypeDef,
+    TestAvailabilityConfigurationResponseTypeDef,
     AvailabilityConfigurationTypeDef,
     DescribeResourceResponseTypeDef,
     UpdateResourceRequestRequestTypeDef,
     CreateAvailabilityConfigurationRequestRequestTypeDef,
     TestAvailabilityConfigurationRequestRequestTypeDef,
     UpdateAvailabilityConfigurationRequestRequestTypeDef,
     CreateImpersonationRoleRequestRequestTypeDef,
-    GetImpersonationRoleResponseTypeDef,
     UpdateImpersonationRoleRequestRequestTypeDef,
     CreateOrganizationRequestRequestTypeDef,
     ListResourceDelegatesResponseTypeDef,
     GetMailDomainResponseTypeDef,
     GetDefaultRetentionPolicyResponseTypeDef,
     PutRetentionPolicyRequestRequestTypeDef,
     GetImpersonationRoleEffectResponseTypeDef,
+    GetImpersonationRoleResponseTypeDef,
     GetMobileDeviceAccessEffectResponseTypeDef,
     ListGroupsResponseTypeDef,
     ListImpersonationRolesResponseTypeDef,
+    ListAliasesRequestListAliasesPaginateTypeDef,
+    ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
+    ListGroupMembersRequestListGroupMembersPaginateTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
+    ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
+    ListOrganizationsRequestListOrganizationsPaginateTypeDef,
+    ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
+    ListResourcesRequestListResourcesPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     ListGroupMembersResponseTypeDef,
     ListMailDomainsResponseTypeDef,
     ListMailboxExportJobsResponseTypeDef,
     ListMailboxPermissionsResponseTypeDef,
     ListMobileDeviceAccessOverridesResponseTypeDef,
     ListMobileDeviceAccessRulesResponseTypeDef,
     ListOrganizationsResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     ListUsersResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ListAvailabilityConfigurationsResponseTypeDef,
 )
 
 
 def get_structure() -> AccessControlRuleTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-workmail-1.28.0/README.md` & `mypy-boto3-workmail-1.28.12/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-workmail"></a>
 
 # mypy-boto3-workmail
 
 [![PyPI - mypy-boto3-workmail](https://img.shields.io/pypi/v/mypy-boto3-workmail.svg?color=blue)](https://pypi.org/project/mypy-boto3-workmail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workmail.svg?color=blue)](https://pypi.org/project/mypy-boto3-workmail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workmail?color=blue)](https://pypistats.org/packages/mypy-boto3-workmail)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workmail)](https://pepy.tech/project/mypy-boto3-workmail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkMail 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
+[boto3.WorkMail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
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
 [mypy-boto3-workmail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,166 +338,171 @@
 
 ```python
 from mypy_boto3_workmail.type_defs import (
     AccessControlRuleTypeDef,
     AssociateDelegateToResourceRequestRequestTypeDef,
     AssociateMemberToGroupRequestRequestTypeDef,
     AssumeImpersonationRoleRequestRequestTypeDef,
-    AssumeImpersonationRoleResponseTypeDef,
-    LambdaAvailabilityProviderTypeDef,
+    ResponseMetadataTypeDef,
+    LambdaAvailabilityProviderOutputTypeDef,
     RedactedEwsAvailabilityProviderTypeDef,
+    BookingOptionsOutputTypeDef,
     BookingOptionsTypeDef,
     CancelMailboxExportJobRequestRequestTypeDef,
     CreateAliasRequestRequestTypeDef,
     EwsAvailabilityProviderTypeDef,
+    LambdaAvailabilityProviderTypeDef,
     CreateGroupRequestRequestTypeDef,
-    CreateGroupResponseTypeDef,
     ImpersonationRuleTypeDef,
-    CreateImpersonationRoleResponseTypeDef,
     CreateMobileDeviceAccessRuleRequestRequestTypeDef,
-    CreateMobileDeviceAccessRuleResponseTypeDef,
     DomainTypeDef,
-    CreateOrganizationResponseTypeDef,
     CreateResourceRequestRequestTypeDef,
-    CreateResourceResponseTypeDef,
     CreateUserRequestRequestTypeDef,
-    CreateUserResponseTypeDef,
     DelegateTypeDef,
     DeleteAccessControlRuleRequestRequestTypeDef,
     DeleteAliasRequestRequestTypeDef,
     DeleteAvailabilityConfigurationRequestRequestTypeDef,
     DeleteEmailMonitoringConfigurationRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteImpersonationRoleRequestRequestTypeDef,
     DeleteMailboxPermissionsRequestRequestTypeDef,
     DeleteMobileDeviceAccessOverrideRequestRequestTypeDef,
     DeleteMobileDeviceAccessRuleRequestRequestTypeDef,
     DeleteOrganizationRequestRequestTypeDef,
-    DeleteOrganizationResponseTypeDef,
     DeleteResourceRequestRequestTypeDef,
     DeleteRetentionPolicyRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeregisterFromWorkMailRequestRequestTypeDef,
     DeregisterMailDomainRequestRequestTypeDef,
     DescribeEmailMonitoringConfigurationRequestRequestTypeDef,
-    DescribeEmailMonitoringConfigurationResponseTypeDef,
     DescribeGroupRequestRequestTypeDef,
-    DescribeGroupResponseTypeDef,
     DescribeInboundDmarcSettingsRequestRequestTypeDef,
-    DescribeInboundDmarcSettingsResponseTypeDef,
     DescribeMailboxExportJobRequestRequestTypeDef,
-    DescribeMailboxExportJobResponseTypeDef,
     DescribeOrganizationRequestRequestTypeDef,
-    DescribeOrganizationResponseTypeDef,
     DescribeResourceRequestRequestTypeDef,
     DescribeUserRequestRequestTypeDef,
-    DescribeUserResponseTypeDef,
     DisassociateDelegateFromResourceRequestRequestTypeDef,
     DisassociateMemberFromGroupRequestRequestTypeDef,
     DnsRecordTypeDef,
+    FolderConfigurationOutputTypeDef,
     FolderConfigurationTypeDef,
     GetAccessControlEffectRequestRequestTypeDef,
-    GetAccessControlEffectResponseTypeDef,
     GetDefaultRetentionPolicyRequestRequestTypeDef,
     GetImpersonationRoleEffectRequestRequestTypeDef,
     ImpersonationMatchedRuleTypeDef,
     GetImpersonationRoleRequestRequestTypeDef,
+    ImpersonationRuleOutputTypeDef,
     GetMailDomainRequestRequestTypeDef,
     GetMailboxDetailsRequestRequestTypeDef,
-    GetMailboxDetailsResponseTypeDef,
     GetMobileDeviceAccessEffectRequestRequestTypeDef,
     MobileDeviceAccessMatchedRuleTypeDef,
     GetMobileDeviceAccessOverrideRequestRequestTypeDef,
-    GetMobileDeviceAccessOverrideResponseTypeDef,
     GroupTypeDef,
     ImpersonationRoleTypeDef,
     ListAccessControlRulesRequestRequestTypeDef,
-    ListAliasesRequestListAliasesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAliasesRequestRequestTypeDef,
-    ListAliasesResponseTypeDef,
-    ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
     ListAvailabilityConfigurationsRequestRequestTypeDef,
-    ListGroupMembersRequestListGroupMembersPaginateTypeDef,
     ListGroupMembersRequestRequestTypeDef,
     MemberTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListImpersonationRolesRequestRequestTypeDef,
     ListMailDomainsRequestRequestTypeDef,
     MailDomainSummaryTypeDef,
     ListMailboxExportJobsRequestRequestTypeDef,
     MailboxExportJobTypeDef,
-    ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
     ListMailboxPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
     ListMobileDeviceAccessOverridesRequestRequestTypeDef,
     MobileDeviceAccessOverrideTypeDef,
     ListMobileDeviceAccessRulesRequestRequestTypeDef,
     MobileDeviceAccessRuleTypeDef,
-    ListOrganizationsRequestListOrganizationsPaginateTypeDef,
     ListOrganizationsRequestRequestTypeDef,
     OrganizationSummaryTypeDef,
-    ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
     ListResourceDelegatesRequestRequestTypeDef,
-    ListResourcesRequestListResourcesPaginateTypeDef,
     ListResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
+    TagOutputTypeDef,
     ListUsersRequestRequestTypeDef,
     UserTypeDef,
-    PaginatorConfigTypeDef,
     PutAccessControlRuleRequestRequestTypeDef,
     PutEmailMonitoringConfigurationRequestRequestTypeDef,
     PutInboundDmarcSettingsRequestRequestTypeDef,
     PutMailboxPermissionsRequestRequestTypeDef,
     PutMobileDeviceAccessOverrideRequestRequestTypeDef,
     RegisterMailDomainRequestRequestTypeDef,
     RegisterToWorkMailRequestRequestTypeDef,
     ResetPasswordRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartMailboxExportJobRequestRequestTypeDef,
-    StartMailboxExportJobResponseTypeDef,
-    TestAvailabilityConfigurationResponseTypeDef,
+    TagTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDefaultMailDomainRequestRequestTypeDef,
     UpdateMailboxQuotaRequestRequestTypeDef,
     UpdateMobileDeviceAccessRuleRequestRequestTypeDef,
     UpdatePrimaryEmailAddressRequestRequestTypeDef,
+    AssumeImpersonationRoleResponseTypeDef,
+    CreateGroupResponseTypeDef,
+    CreateImpersonationRoleResponseTypeDef,
+    CreateMobileDeviceAccessRuleResponseTypeDef,
+    CreateOrganizationResponseTypeDef,
+    CreateResourceResponseTypeDef,
+    CreateUserResponseTypeDef,
+    DeleteOrganizationResponseTypeDef,
+    DescribeEmailMonitoringConfigurationResponseTypeDef,
+    DescribeGroupResponseTypeDef,
+    DescribeInboundDmarcSettingsResponseTypeDef,
+    DescribeMailboxExportJobResponseTypeDef,
+    DescribeOrganizationResponseTypeDef,
+    DescribeUserResponseTypeDef,
+    GetAccessControlEffectResponseTypeDef,
+    GetMailboxDetailsResponseTypeDef,
+    GetMobileDeviceAccessOverrideResponseTypeDef,
     ListAccessControlRulesResponseTypeDef,
+    ListAliasesResponseTypeDef,
+    StartMailboxExportJobResponseTypeDef,
+    TestAvailabilityConfigurationResponseTypeDef,
     AvailabilityConfigurationTypeDef,
     DescribeResourceResponseTypeDef,
     UpdateResourceRequestRequestTypeDef,
     CreateAvailabilityConfigurationRequestRequestTypeDef,
     TestAvailabilityConfigurationRequestRequestTypeDef,
     UpdateAvailabilityConfigurationRequestRequestTypeDef,
     CreateImpersonationRoleRequestRequestTypeDef,
-    GetImpersonationRoleResponseTypeDef,
     UpdateImpersonationRoleRequestRequestTypeDef,
     CreateOrganizationRequestRequestTypeDef,
     ListResourceDelegatesResponseTypeDef,
     GetMailDomainResponseTypeDef,
     GetDefaultRetentionPolicyResponseTypeDef,
     PutRetentionPolicyRequestRequestTypeDef,
     GetImpersonationRoleEffectResponseTypeDef,
+    GetImpersonationRoleResponseTypeDef,
     GetMobileDeviceAccessEffectResponseTypeDef,
     ListGroupsResponseTypeDef,
     ListImpersonationRolesResponseTypeDef,
+    ListAliasesRequestListAliasesPaginateTypeDef,
+    ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
+    ListGroupMembersRequestListGroupMembersPaginateTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
+    ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
+    ListOrganizationsRequestListOrganizationsPaginateTypeDef,
+    ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
+    ListResourcesRequestListResourcesPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     ListGroupMembersResponseTypeDef,
     ListMailDomainsResponseTypeDef,
     ListMailboxExportJobsResponseTypeDef,
     ListMailboxPermissionsResponseTypeDef,
     ListMobileDeviceAccessOverridesResponseTypeDef,
     ListMobileDeviceAccessRulesResponseTypeDef,
     ListOrganizationsResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     ListUsersResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ListAvailabilityConfigurationsResponseTypeDef,
 )
 
 
 def get_structure() -> AccessControlRuleTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/__init__.py` & `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/__init__.pyi` & `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/__main__.py` & `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkMail 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.WorkMail 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail\nOther"
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

### Comparing `mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/client.py` & `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/client.pyi` & `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/literals.py` & `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/literals.py`

 * *Files 1% similar despite different names*

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

### Comparing `mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/literals.pyi` & `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -188,14 +188,15 @@
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
@@ -274,26 +275,28 @@
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

### Comparing `mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/paginator.py` & `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,98 +78,90 @@
 class ListAliasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListAliases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listaliasespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        OrganizationId: str,
-        EntityId: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OrganizationId: str, EntityId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listaliasespaginator)
         """
 
 
 class ListAvailabilityConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListAvailabilityConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listavailabilityconfigurationspaginator)
     """
 
     def paginate(
-        self, *, OrganizationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OrganizationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAvailabilityConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListAvailabilityConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listavailabilityconfigurationspaginator)
         """
 
 
 class ListGroupMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListGroupMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listgroupmemberspaginator)
     """
 
     def paginate(
-        self, *, OrganizationId: str, GroupId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OrganizationId: str, GroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroupMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListGroupMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listgroupmemberspaginator)
         """
 
 
 class ListGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listgroupspaginator)
     """
 
     def paginate(
-        self, *, OrganizationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OrganizationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listgroupspaginator)
         """
 
 
 class ListMailboxPermissionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListMailboxPermissions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listmailboxpermissionspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        OrganizationId: str,
-        EntityId: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OrganizationId: str, EntityId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMailboxPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListMailboxPermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listmailboxpermissionspaginator)
         """
 
 
 class ListOrganizationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListOrganizations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listorganizationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOrganizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListOrganizations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listorganizationspaginator)
         """
 
 
@@ -180,43 +172,43 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationId: str,
         ResourceId: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceDelegatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListResourceDelegates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listresourcedelegatespaginator)
         """
 
 
 class ListResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listresourcespaginator)
     """
 
     def paginate(
-        self, *, OrganizationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OrganizationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listresourcespaginator)
         """
 
 
 class ListUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listuserspaginator)
     """
 
     def paginate(
-        self, *, OrganizationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OrganizationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listuserspaginator)
         """
```

### Comparing `mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/paginator.pyi` & `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -75,93 +75,85 @@
 class ListAliasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListAliases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listaliasespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        OrganizationId: str,
-        EntityId: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OrganizationId: str, EntityId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listaliasespaginator)
         """
 
 class ListAvailabilityConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListAvailabilityConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listavailabilityconfigurationspaginator)
     """
 
     def paginate(
-        self, *, OrganizationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OrganizationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAvailabilityConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListAvailabilityConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listavailabilityconfigurationspaginator)
         """
 
 class ListGroupMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListGroupMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listgroupmemberspaginator)
     """
 
     def paginate(
-        self, *, OrganizationId: str, GroupId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OrganizationId: str, GroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroupMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListGroupMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listgroupmemberspaginator)
         """
 
 class ListGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listgroupspaginator)
     """
 
     def paginate(
-        self, *, OrganizationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OrganizationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listgroupspaginator)
         """
 
 class ListMailboxPermissionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListMailboxPermissions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listmailboxpermissionspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        OrganizationId: str,
-        EntityId: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OrganizationId: str, EntityId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMailboxPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListMailboxPermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listmailboxpermissionspaginator)
         """
 
 class ListOrganizationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListOrganizations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listorganizationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOrganizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListOrganizations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listorganizationspaginator)
         """
 
 class ListResourceDelegatesPaginator(Paginator):
@@ -171,41 +163,41 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationId: str,
         ResourceId: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceDelegatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListResourceDelegates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listresourcedelegatespaginator)
         """
 
 class ListResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listresourcespaginator)
     """
 
     def paginate(
-        self, *, OrganizationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OrganizationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listresourcespaginator)
         """
 
 class ListUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listuserspaginator)
     """
 
     def paginate(
-        self, *, OrganizationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OrganizationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/paginators/#listuserspaginator)
         """
```

### Comparing `mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/type_defs.py` & `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,166 +39,171 @@
 
 
 __all__ = (
     "AccessControlRuleTypeDef",
     "AssociateDelegateToResourceRequestRequestTypeDef",
     "AssociateMemberToGroupRequestRequestTypeDef",
     "AssumeImpersonationRoleRequestRequestTypeDef",
-    "AssumeImpersonationRoleResponseTypeDef",
-    "LambdaAvailabilityProviderTypeDef",
+    "ResponseMetadataTypeDef",
+    "LambdaAvailabilityProviderOutputTypeDef",
     "RedactedEwsAvailabilityProviderTypeDef",
+    "BookingOptionsOutputTypeDef",
     "BookingOptionsTypeDef",
     "CancelMailboxExportJobRequestRequestTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "EwsAvailabilityProviderTypeDef",
+    "LambdaAvailabilityProviderTypeDef",
     "CreateGroupRequestRequestTypeDef",
-    "CreateGroupResponseTypeDef",
     "ImpersonationRuleTypeDef",
-    "CreateImpersonationRoleResponseTypeDef",
     "CreateMobileDeviceAccessRuleRequestRequestTypeDef",
-    "CreateMobileDeviceAccessRuleResponseTypeDef",
     "DomainTypeDef",
-    "CreateOrganizationResponseTypeDef",
     "CreateResourceRequestRequestTypeDef",
-    "CreateResourceResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
-    "CreateUserResponseTypeDef",
     "DelegateTypeDef",
     "DeleteAccessControlRuleRequestRequestTypeDef",
     "DeleteAliasRequestRequestTypeDef",
     "DeleteAvailabilityConfigurationRequestRequestTypeDef",
     "DeleteEmailMonitoringConfigurationRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteImpersonationRoleRequestRequestTypeDef",
     "DeleteMailboxPermissionsRequestRequestTypeDef",
     "DeleteMobileDeviceAccessOverrideRequestRequestTypeDef",
     "DeleteMobileDeviceAccessRuleRequestRequestTypeDef",
     "DeleteOrganizationRequestRequestTypeDef",
-    "DeleteOrganizationResponseTypeDef",
     "DeleteResourceRequestRequestTypeDef",
     "DeleteRetentionPolicyRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DeregisterFromWorkMailRequestRequestTypeDef",
     "DeregisterMailDomainRequestRequestTypeDef",
     "DescribeEmailMonitoringConfigurationRequestRequestTypeDef",
-    "DescribeEmailMonitoringConfigurationResponseTypeDef",
     "DescribeGroupRequestRequestTypeDef",
-    "DescribeGroupResponseTypeDef",
     "DescribeInboundDmarcSettingsRequestRequestTypeDef",
-    "DescribeInboundDmarcSettingsResponseTypeDef",
     "DescribeMailboxExportJobRequestRequestTypeDef",
-    "DescribeMailboxExportJobResponseTypeDef",
     "DescribeOrganizationRequestRequestTypeDef",
-    "DescribeOrganizationResponseTypeDef",
     "DescribeResourceRequestRequestTypeDef",
     "DescribeUserRequestRequestTypeDef",
-    "DescribeUserResponseTypeDef",
     "DisassociateDelegateFromResourceRequestRequestTypeDef",
     "DisassociateMemberFromGroupRequestRequestTypeDef",
     "DnsRecordTypeDef",
+    "FolderConfigurationOutputTypeDef",
     "FolderConfigurationTypeDef",
     "GetAccessControlEffectRequestRequestTypeDef",
-    "GetAccessControlEffectResponseTypeDef",
     "GetDefaultRetentionPolicyRequestRequestTypeDef",
     "GetImpersonationRoleEffectRequestRequestTypeDef",
     "ImpersonationMatchedRuleTypeDef",
     "GetImpersonationRoleRequestRequestTypeDef",
+    "ImpersonationRuleOutputTypeDef",
     "GetMailDomainRequestRequestTypeDef",
     "GetMailboxDetailsRequestRequestTypeDef",
-    "GetMailboxDetailsResponseTypeDef",
     "GetMobileDeviceAccessEffectRequestRequestTypeDef",
     "MobileDeviceAccessMatchedRuleTypeDef",
     "GetMobileDeviceAccessOverrideRequestRequestTypeDef",
-    "GetMobileDeviceAccessOverrideResponseTypeDef",
     "GroupTypeDef",
     "ImpersonationRoleTypeDef",
     "ListAccessControlRulesRequestRequestTypeDef",
-    "ListAliasesRequestListAliasesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAliasesRequestRequestTypeDef",
-    "ListAliasesResponseTypeDef",
-    "ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
     "ListAvailabilityConfigurationsRequestRequestTypeDef",
-    "ListGroupMembersRequestListGroupMembersPaginateTypeDef",
     "ListGroupMembersRequestRequestTypeDef",
     "MemberTypeDef",
-    "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
     "ListImpersonationRolesRequestRequestTypeDef",
     "ListMailDomainsRequestRequestTypeDef",
     "MailDomainSummaryTypeDef",
     "ListMailboxExportJobsRequestRequestTypeDef",
     "MailboxExportJobTypeDef",
-    "ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
     "ListMailboxPermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
     "ListMobileDeviceAccessOverridesRequestRequestTypeDef",
     "MobileDeviceAccessOverrideTypeDef",
     "ListMobileDeviceAccessRulesRequestRequestTypeDef",
     "MobileDeviceAccessRuleTypeDef",
-    "ListOrganizationsRequestListOrganizationsPaginateTypeDef",
     "ListOrganizationsRequestRequestTypeDef",
     "OrganizationSummaryTypeDef",
-    "ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef",
     "ListResourceDelegatesRequestRequestTypeDef",
-    "ListResourcesRequestListResourcesPaginateTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
+    "TagOutputTypeDef",
     "ListUsersRequestRequestTypeDef",
     "UserTypeDef",
-    "PaginatorConfigTypeDef",
     "PutAccessControlRuleRequestRequestTypeDef",
     "PutEmailMonitoringConfigurationRequestRequestTypeDef",
     "PutInboundDmarcSettingsRequestRequestTypeDef",
     "PutMailboxPermissionsRequestRequestTypeDef",
     "PutMobileDeviceAccessOverrideRequestRequestTypeDef",
     "RegisterMailDomainRequestRequestTypeDef",
     "RegisterToWorkMailRequestRequestTypeDef",
     "ResetPasswordRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StartMailboxExportJobRequestRequestTypeDef",
-    "StartMailboxExportJobResponseTypeDef",
-    "TestAvailabilityConfigurationResponseTypeDef",
+    "TagTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDefaultMailDomainRequestRequestTypeDef",
     "UpdateMailboxQuotaRequestRequestTypeDef",
     "UpdateMobileDeviceAccessRuleRequestRequestTypeDef",
     "UpdatePrimaryEmailAddressRequestRequestTypeDef",
+    "AssumeImpersonationRoleResponseTypeDef",
+    "CreateGroupResponseTypeDef",
+    "CreateImpersonationRoleResponseTypeDef",
+    "CreateMobileDeviceAccessRuleResponseTypeDef",
+    "CreateOrganizationResponseTypeDef",
+    "CreateResourceResponseTypeDef",
+    "CreateUserResponseTypeDef",
+    "DeleteOrganizationResponseTypeDef",
+    "DescribeEmailMonitoringConfigurationResponseTypeDef",
+    "DescribeGroupResponseTypeDef",
+    "DescribeInboundDmarcSettingsResponseTypeDef",
+    "DescribeMailboxExportJobResponseTypeDef",
+    "DescribeOrganizationResponseTypeDef",
+    "DescribeUserResponseTypeDef",
+    "GetAccessControlEffectResponseTypeDef",
+    "GetMailboxDetailsResponseTypeDef",
+    "GetMobileDeviceAccessOverrideResponseTypeDef",
     "ListAccessControlRulesResponseTypeDef",
+    "ListAliasesResponseTypeDef",
+    "StartMailboxExportJobResponseTypeDef",
+    "TestAvailabilityConfigurationResponseTypeDef",
     "AvailabilityConfigurationTypeDef",
     "DescribeResourceResponseTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "CreateAvailabilityConfigurationRequestRequestTypeDef",
     "TestAvailabilityConfigurationRequestRequestTypeDef",
     "UpdateAvailabilityConfigurationRequestRequestTypeDef",
     "CreateImpersonationRoleRequestRequestTypeDef",
-    "GetImpersonationRoleResponseTypeDef",
     "UpdateImpersonationRoleRequestRequestTypeDef",
     "CreateOrganizationRequestRequestTypeDef",
     "ListResourceDelegatesResponseTypeDef",
     "GetMailDomainResponseTypeDef",
     "GetDefaultRetentionPolicyResponseTypeDef",
     "PutRetentionPolicyRequestRequestTypeDef",
     "GetImpersonationRoleEffectResponseTypeDef",
+    "GetImpersonationRoleResponseTypeDef",
     "GetMobileDeviceAccessEffectResponseTypeDef",
     "ListGroupsResponseTypeDef",
     "ListImpersonationRolesResponseTypeDef",
+    "ListAliasesRequestListAliasesPaginateTypeDef",
+    "ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
+    "ListGroupMembersRequestListGroupMembersPaginateTypeDef",
+    "ListGroupsRequestListGroupsPaginateTypeDef",
+    "ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
+    "ListOrganizationsRequestListOrganizationsPaginateTypeDef",
+    "ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef",
+    "ListResourcesRequestListResourcesPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
     "ListGroupMembersResponseTypeDef",
     "ListMailDomainsResponseTypeDef",
     "ListMailboxExportJobsResponseTypeDef",
     "ListMailboxPermissionsResponseTypeDef",
     "ListMobileDeviceAccessOverridesResponseTypeDef",
     "ListMobileDeviceAccessRulesResponseTypeDef",
     "ListOrganizationsResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "ListUsersResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "ListAvailabilityConfigurationsResponseTypeDef",
 )
 
 AccessControlRuleTypeDef = TypedDict(
     "AccessControlRuleTypeDef",
     {
         "Name": str,
@@ -240,39 +245,51 @@
     "AssumeImpersonationRoleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ImpersonationRoleId": str,
     },
 )
 
-AssumeImpersonationRoleResponseTypeDef = TypedDict(
-    "AssumeImpersonationRoleResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Token": str,
-        "ExpiresIn": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-LambdaAvailabilityProviderTypeDef = TypedDict(
-    "LambdaAvailabilityProviderTypeDef",
+LambdaAvailabilityProviderOutputTypeDef = TypedDict(
+    "LambdaAvailabilityProviderOutputTypeDef",
     {
         "LambdaArn": str,
     },
 )
 
 RedactedEwsAvailabilityProviderTypeDef = TypedDict(
     "RedactedEwsAvailabilityProviderTypeDef",
     {
         "EwsEndpoint": str,
         "EwsUsername": str,
     },
     total=False,
 )
 
+BookingOptionsOutputTypeDef = TypedDict(
+    "BookingOptionsOutputTypeDef",
+    {
+        "AutoAcceptRequests": bool,
+        "AutoDeclineRecurringRequests": bool,
+        "AutoDeclineConflictingRequests": bool,
+    },
+    total=False,
+)
+
 BookingOptionsTypeDef = TypedDict(
     "BookingOptionsTypeDef",
     {
         "AutoAcceptRequests": bool,
         "AutoDeclineRecurringRequests": bool,
         "AutoDeclineConflictingRequests": bool,
     },
@@ -302,27 +319,26 @@
     {
         "EwsEndpoint": str,
         "EwsUsername": str,
         "EwsPassword": str,
     },
 )
 
-CreateGroupRequestRequestTypeDef = TypedDict(
-    "CreateGroupRequestRequestTypeDef",
+LambdaAvailabilityProviderTypeDef = TypedDict(
+    "LambdaAvailabilityProviderTypeDef",
     {
-        "OrganizationId": str,
-        "Name": str,
+        "LambdaArn": str,
     },
 )
 
-CreateGroupResponseTypeDef = TypedDict(
-    "CreateGroupResponseTypeDef",
+CreateGroupRequestRequestTypeDef = TypedDict(
+    "CreateGroupRequestRequestTypeDef",
     {
-        "GroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "OrganizationId": str,
+        "Name": str,
     },
 )
 
 _RequiredImpersonationRuleTypeDef = TypedDict(
     "_RequiredImpersonationRuleTypeDef",
     {
         "ImpersonationRuleId": str,
@@ -343,22 +359,14 @@
 
 class ImpersonationRuleTypeDef(
     _RequiredImpersonationRuleTypeDef, _OptionalImpersonationRuleTypeDef
 ):
     pass
 
 
-CreateImpersonationRoleResponseTypeDef = TypedDict(
-    "CreateImpersonationRoleResponseTypeDef",
-    {
-        "ImpersonationRoleId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
         "Effect": MobileDeviceAccessRuleEffectType,
     },
@@ -384,74 +392,42 @@
 class CreateMobileDeviceAccessRuleRequestRequestTypeDef(
     _RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef,
     _OptionalCreateMobileDeviceAccessRuleRequestRequestTypeDef,
 ):
     pass
 
 
-CreateMobileDeviceAccessRuleResponseTypeDef = TypedDict(
-    "CreateMobileDeviceAccessRuleResponseTypeDef",
-    {
-        "MobileDeviceAccessRuleId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DomainTypeDef = TypedDict(
     "DomainTypeDef",
     {
         "DomainName": str,
         "HostedZoneId": str,
     },
     total=False,
 )
 
-CreateOrganizationResponseTypeDef = TypedDict(
-    "CreateOrganizationResponseTypeDef",
-    {
-        "OrganizationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateResourceRequestRequestTypeDef = TypedDict(
     "CreateResourceRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
         "Type": ResourceTypeType,
     },
 )
 
-CreateResourceResponseTypeDef = TypedDict(
-    "CreateResourceResponseTypeDef",
-    {
-        "ResourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateUserRequestRequestTypeDef = TypedDict(
     "CreateUserRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
         "DisplayName": str,
         "Password": str,
     },
 )
 
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
-    {
-        "UserId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DelegateTypeDef = TypedDict(
     "DelegateTypeDef",
     {
         "Id": str,
         "Type": MemberTypeType,
     },
 )
@@ -549,23 +525,14 @@
 class DeleteOrganizationRequestRequestTypeDef(
     _RequiredDeleteOrganizationRequestRequestTypeDef,
     _OptionalDeleteOrganizationRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteOrganizationResponseTypeDef = TypedDict(
-    "DeleteOrganizationResponseTypeDef",
-    {
-        "OrganizationId": str,
-        "State": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteResourceRequestRequestTypeDef = TypedDict(
     "DeleteResourceRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ResourceId": str,
     },
 )
@@ -605,109 +572,44 @@
 DescribeEmailMonitoringConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeEmailMonitoringConfigurationRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 
-DescribeEmailMonitoringConfigurationResponseTypeDef = TypedDict(
-    "DescribeEmailMonitoringConfigurationResponseTypeDef",
-    {
-        "RoleArn": str,
-        "LogGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeGroupRequestRequestTypeDef = TypedDict(
     "DescribeGroupRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "GroupId": str,
     },
 )
 
-DescribeGroupResponseTypeDef = TypedDict(
-    "DescribeGroupResponseTypeDef",
-    {
-        "GroupId": str,
-        "Name": str,
-        "Email": str,
-        "State": EntityStateType,
-        "EnabledDate": datetime,
-        "DisabledDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeInboundDmarcSettingsRequestRequestTypeDef = TypedDict(
     "DescribeInboundDmarcSettingsRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 
-DescribeInboundDmarcSettingsResponseTypeDef = TypedDict(
-    "DescribeInboundDmarcSettingsResponseTypeDef",
-    {
-        "Enforced": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeMailboxExportJobRequestRequestTypeDef = TypedDict(
     "DescribeMailboxExportJobRequestRequestTypeDef",
     {
         "JobId": str,
         "OrganizationId": str,
     },
 )
 
-DescribeMailboxExportJobResponseTypeDef = TypedDict(
-    "DescribeMailboxExportJobResponseTypeDef",
-    {
-        "EntityId": str,
-        "Description": str,
-        "RoleArn": str,
-        "KmsKeyArn": str,
-        "S3BucketName": str,
-        "S3Prefix": str,
-        "S3Path": str,
-        "EstimatedProgress": int,
-        "State": MailboxExportJobStateType,
-        "ErrorInfo": str,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeOrganizationRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 
-DescribeOrganizationResponseTypeDef = TypedDict(
-    "DescribeOrganizationResponseTypeDef",
-    {
-        "OrganizationId": str,
-        "Alias": str,
-        "State": str,
-        "DirectoryId": str,
-        "DirectoryType": str,
-        "DefaultMailDomain": str,
-        "CompletedDate": datetime,
-        "ErrorMessage": str,
-        "ARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeResourceRequestRequestTypeDef = TypedDict(
     "DescribeResourceRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ResourceId": str,
     },
 )
@@ -716,29 +618,14 @@
     "DescribeUserRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "UserId": str,
     },
 )
 
-DescribeUserResponseTypeDef = TypedDict(
-    "DescribeUserResponseTypeDef",
-    {
-        "UserId": str,
-        "Name": str,
-        "Email": str,
-        "DisplayName": str,
-        "State": EntityStateType,
-        "UserRole": UserRoleType,
-        "EnabledDate": datetime,
-        "DisabledDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateDelegateFromResourceRequestRequestTypeDef = TypedDict(
     "DisassociateDelegateFromResourceRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ResourceId": str,
         "EntityId": str,
     },
@@ -759,14 +646,36 @@
         "Type": str,
         "Hostname": str,
         "Value": str,
     },
     total=False,
 )
 
+_RequiredFolderConfigurationOutputTypeDef = TypedDict(
+    "_RequiredFolderConfigurationOutputTypeDef",
+    {
+        "Name": FolderNameType,
+        "Action": RetentionActionType,
+    },
+)
+_OptionalFolderConfigurationOutputTypeDef = TypedDict(
+    "_OptionalFolderConfigurationOutputTypeDef",
+    {
+        "Period": int,
+    },
+    total=False,
+)
+
+
+class FolderConfigurationOutputTypeDef(
+    _RequiredFolderConfigurationOutputTypeDef, _OptionalFolderConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredFolderConfigurationTypeDef = TypedDict(
     "_RequiredFolderConfigurationTypeDef",
     {
         "Name": FolderNameType,
         "Action": RetentionActionType,
     },
 )
@@ -806,23 +715,14 @@
 class GetAccessControlEffectRequestRequestTypeDef(
     _RequiredGetAccessControlEffectRequestRequestTypeDef,
     _OptionalGetAccessControlEffectRequestRequestTypeDef,
 ):
     pass
 
 
-GetAccessControlEffectResponseTypeDef = TypedDict(
-    "GetAccessControlEffectResponseTypeDef",
-    {
-        "Effect": AccessControlRuleEffectType,
-        "MatchedRules": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDefaultRetentionPolicyRequestRequestTypeDef = TypedDict(
     "GetDefaultRetentionPolicyRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 
@@ -848,14 +748,39 @@
     "GetImpersonationRoleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ImpersonationRoleId": str,
     },
 )
 
+_RequiredImpersonationRuleOutputTypeDef = TypedDict(
+    "_RequiredImpersonationRuleOutputTypeDef",
+    {
+        "ImpersonationRuleId": str,
+        "Effect": AccessEffectType,
+    },
+)
+_OptionalImpersonationRuleOutputTypeDef = TypedDict(
+    "_OptionalImpersonationRuleOutputTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "TargetUsers": List[str],
+        "NotTargetUsers": List[str],
+    },
+    total=False,
+)
+
+
+class ImpersonationRuleOutputTypeDef(
+    _RequiredImpersonationRuleOutputTypeDef, _OptionalImpersonationRuleOutputTypeDef
+):
+    pass
+
+
 GetMailDomainRequestRequestTypeDef = TypedDict(
     "GetMailDomainRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -864,23 +789,14 @@
     "GetMailboxDetailsRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "UserId": str,
     },
 )
 
-GetMailboxDetailsResponseTypeDef = TypedDict(
-    "GetMailboxDetailsResponseTypeDef",
-    {
-        "MailboxQuota": int,
-        "MailboxSize": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMobileDeviceAccessEffectRequestRequestTypeDef = TypedDict(
     "_RequiredGetMobileDeviceAccessEffectRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalGetMobileDeviceAccessEffectRequestRequestTypeDef = TypedDict(
@@ -916,27 +832,14 @@
     {
         "OrganizationId": str,
         "UserId": str,
         "DeviceId": str,
     },
 )
 
-GetMobileDeviceAccessOverrideResponseTypeDef = TypedDict(
-    "GetMobileDeviceAccessOverrideResponseTypeDef",
-    {
-        "UserId": str,
-        "DeviceId": str,
-        "Effect": MobileDeviceAccessRuleEffectType,
-        "Description": str,
-        "DateCreated": datetime,
-        "DateModified": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GroupTypeDef = TypedDict(
     "GroupTypeDef",
     {
         "Id": str,
         "Email": str,
         "Name": str,
         "State": EntityStateType,
@@ -961,37 +864,24 @@
 ListAccessControlRulesRequestRequestTypeDef = TypedDict(
     "ListAccessControlRulesRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 
-_RequiredListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
-    "_RequiredListAliasesRequestListAliasesPaginateTypeDef",
-    {
-        "OrganizationId": str,
-        "EntityId": str,
-    },
-)
-_OptionalListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
-    "_OptionalListAliasesRequestListAliasesPaginateTypeDef",
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
-class ListAliasesRequestListAliasesPaginateTypeDef(
-    _RequiredListAliasesRequestListAliasesPaginateTypeDef,
-    _OptionalListAliasesRequestListAliasesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredListAliasesRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "EntityId": str,
     },
 )
@@ -1007,45 +897,14 @@
 
 class ListAliasesRequestRequestTypeDef(
     _RequiredListAliasesRequestRequestTypeDef, _OptionalListAliasesRequestRequestTypeDef
 ):
     pass
 
 
-ListAliasesResponseTypeDef = TypedDict(
-    "ListAliasesResponseTypeDef",
-    {
-        "Aliases": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef = TypedDict(
-    "_RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
-    {
-        "OrganizationId": str,
-    },
-)
-_OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef = TypedDict(
-    "_OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef(
-    _RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
-    _OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAvailabilityConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailabilityConfigurationsRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListAvailabilityConfigurationsRequestRequestTypeDef = TypedDict(
@@ -1061,37 +920,14 @@
 class ListAvailabilityConfigurationsRequestRequestTypeDef(
     _RequiredListAvailabilityConfigurationsRequestRequestTypeDef,
     _OptionalListAvailabilityConfigurationsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef = TypedDict(
-    "_RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef",
-    {
-        "OrganizationId": str,
-        "GroupId": str,
-    },
-)
-_OptionalListGroupMembersRequestListGroupMembersPaginateTypeDef = TypedDict(
-    "_OptionalListGroupMembersRequestListGroupMembersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListGroupMembersRequestListGroupMembersPaginateTypeDef(
-    _RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef,
-    _OptionalListGroupMembersRequestListGroupMembersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListGroupMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembersRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "GroupId": str,
     },
 )
@@ -1120,36 +956,14 @@
         "State": EntityStateType,
         "EnabledDate": datetime,
         "DisabledDate": datetime,
     },
     total=False,
 )
 
-_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "OrganizationId": str,
-    },
-)
-_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListGroupsRequestListGroupsPaginateTypeDef(
-    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
-    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupsRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListGroupsRequestRequestTypeDef = TypedDict(
@@ -1257,37 +1071,14 @@
         "State": MailboxExportJobStateType,
         "StartTime": datetime,
         "EndTime": datetime,
     },
     total=False,
 )
 
-_RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef = TypedDict(
-    "_RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
-    {
-        "OrganizationId": str,
-        "EntityId": str,
-    },
-)
-_OptionalListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef = TypedDict(
-    "_OptionalListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef(
-    _RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
-    _OptionalListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListMailboxPermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredListMailboxPermissionsRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "EntityId": str,
     },
 )
@@ -1379,22 +1170,14 @@
         "NotDeviceUserAgents": List[str],
         "DateCreated": datetime,
         "DateModified": datetime,
     },
     total=False,
 )
 
-ListOrganizationsRequestListOrganizationsPaginateTypeDef = TypedDict(
-    "ListOrganizationsRequestListOrganizationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOrganizationsRequestRequestTypeDef = TypedDict(
     "ListOrganizationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1408,37 +1191,14 @@
         "DefaultMailDomain": str,
         "ErrorMessage": str,
         "State": str,
     },
     total=False,
 )
 
-_RequiredListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef = TypedDict(
-    "_RequiredListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef",
-    {
-        "OrganizationId": str,
-        "ResourceId": str,
-    },
-)
-_OptionalListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef = TypedDict(
-    "_OptionalListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef(
-    _RequiredListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
-    _OptionalListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResourceDelegatesRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceDelegatesRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ResourceId": str,
     },
 )
@@ -1455,36 +1215,14 @@
 class ListResourceDelegatesRequestRequestTypeDef(
     _RequiredListResourceDelegatesRequestRequestTypeDef,
     _OptionalListResourceDelegatesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "OrganizationId": str,
-    },
-)
-_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListResourcesRequestListResourcesPaginateTypeDef(
-    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
-    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListResourcesRequestRequestTypeDef = TypedDict(
@@ -1520,44 +1258,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "OrganizationId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -1587,24 +1303,14 @@
         "UserRole": UserRoleType,
         "EnabledDate": datetime,
         "DisabledDate": datetime,
     },
     total=False,
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
 _RequiredPutAccessControlRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutAccessControlRuleRequestRequestTypeDef",
     {
         "Name": str,
         "Effect": AccessControlRuleEffectType,
         "Description": str,
         "OrganizationId": str,
@@ -1722,25 +1428,14 @@
     {
         "OrganizationId": str,
         "UserId": str,
         "Password": str,
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
 _RequiredStartMailboxExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartMailboxExportJobRequestRequestTypeDef",
     {
         "ClientToken": str,
         "OrganizationId": str,
         "EntityId": str,
         "RoleArn": str,
@@ -1761,28 +1456,19 @@
 class StartMailboxExportJobRequestRequestTypeDef(
     _RequiredStartMailboxExportJobRequestRequestTypeDef,
     _OptionalStartMailboxExportJobRequestRequestTypeDef,
 ):
     pass
 
 
-StartMailboxExportJobResponseTypeDef = TypedDict(
-    "StartMailboxExportJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TestAvailabilityConfigurationResponseTypeDef = TypedDict(
-    "TestAvailabilityConfigurationResponseTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "TestPassed": bool,
-        "FailureReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": str,
+        "Value": str,
     },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -1845,47 +1531,250 @@
     {
         "OrganizationId": str,
         "EntityId": str,
         "Email": str,
     },
 )
 
+AssumeImpersonationRoleResponseTypeDef = TypedDict(
+    "AssumeImpersonationRoleResponseTypeDef",
+    {
+        "Token": str,
+        "ExpiresIn": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGroupResponseTypeDef = TypedDict(
+    "CreateGroupResponseTypeDef",
+    {
+        "GroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateImpersonationRoleResponseTypeDef = TypedDict(
+    "CreateImpersonationRoleResponseTypeDef",
+    {
+        "ImpersonationRoleId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMobileDeviceAccessRuleResponseTypeDef = TypedDict(
+    "CreateMobileDeviceAccessRuleResponseTypeDef",
+    {
+        "MobileDeviceAccessRuleId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateOrganizationResponseTypeDef = TypedDict(
+    "CreateOrganizationResponseTypeDef",
+    {
+        "OrganizationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateResourceResponseTypeDef = TypedDict(
+    "CreateResourceResponseTypeDef",
+    {
+        "ResourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
+    {
+        "UserId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteOrganizationResponseTypeDef = TypedDict(
+    "DeleteOrganizationResponseTypeDef",
+    {
+        "OrganizationId": str,
+        "State": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEmailMonitoringConfigurationResponseTypeDef = TypedDict(
+    "DescribeEmailMonitoringConfigurationResponseTypeDef",
+    {
+        "RoleArn": str,
+        "LogGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGroupResponseTypeDef = TypedDict(
+    "DescribeGroupResponseTypeDef",
+    {
+        "GroupId": str,
+        "Name": str,
+        "Email": str,
+        "State": EntityStateType,
+        "EnabledDate": datetime,
+        "DisabledDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeInboundDmarcSettingsResponseTypeDef = TypedDict(
+    "DescribeInboundDmarcSettingsResponseTypeDef",
+    {
+        "Enforced": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeMailboxExportJobResponseTypeDef = TypedDict(
+    "DescribeMailboxExportJobResponseTypeDef",
+    {
+        "EntityId": str,
+        "Description": str,
+        "RoleArn": str,
+        "KmsKeyArn": str,
+        "S3BucketName": str,
+        "S3Prefix": str,
+        "S3Path": str,
+        "EstimatedProgress": int,
+        "State": MailboxExportJobStateType,
+        "ErrorInfo": str,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationResponseTypeDef = TypedDict(
+    "DescribeOrganizationResponseTypeDef",
+    {
+        "OrganizationId": str,
+        "Alias": str,
+        "State": str,
+        "DirectoryId": str,
+        "DirectoryType": str,
+        "DefaultMailDomain": str,
+        "CompletedDate": datetime,
+        "ErrorMessage": str,
+        "ARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeUserResponseTypeDef = TypedDict(
+    "DescribeUserResponseTypeDef",
+    {
+        "UserId": str,
+        "Name": str,
+        "Email": str,
+        "DisplayName": str,
+        "State": EntityStateType,
+        "UserRole": UserRoleType,
+        "EnabledDate": datetime,
+        "DisabledDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccessControlEffectResponseTypeDef = TypedDict(
+    "GetAccessControlEffectResponseTypeDef",
+    {
+        "Effect": AccessControlRuleEffectType,
+        "MatchedRules": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMailboxDetailsResponseTypeDef = TypedDict(
+    "GetMailboxDetailsResponseTypeDef",
+    {
+        "MailboxQuota": int,
+        "MailboxSize": float,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMobileDeviceAccessOverrideResponseTypeDef = TypedDict(
+    "GetMobileDeviceAccessOverrideResponseTypeDef",
+    {
+        "UserId": str,
+        "DeviceId": str,
+        "Effect": MobileDeviceAccessRuleEffectType,
+        "Description": str,
+        "DateCreated": datetime,
+        "DateModified": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAccessControlRulesResponseTypeDef = TypedDict(
     "ListAccessControlRulesResponseTypeDef",
     {
         "Rules": List[AccessControlRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAliasesResponseTypeDef = TypedDict(
+    "ListAliasesResponseTypeDef",
+    {
+        "Aliases": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartMailboxExportJobResponseTypeDef = TypedDict(
+    "StartMailboxExportJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestAvailabilityConfigurationResponseTypeDef = TypedDict(
+    "TestAvailabilityConfigurationResponseTypeDef",
+    {
+        "TestPassed": bool,
+        "FailureReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AvailabilityConfigurationTypeDef = TypedDict(
     "AvailabilityConfigurationTypeDef",
     {
         "DomainName": str,
         "ProviderType": AvailabilityProviderTypeType,
         "EwsProvider": RedactedEwsAvailabilityProviderTypeDef,
-        "LambdaProvider": LambdaAvailabilityProviderTypeDef,
+        "LambdaProvider": LambdaAvailabilityProviderOutputTypeDef,
         "DateCreated": datetime,
         "DateModified": datetime,
     },
     total=False,
 )
 
 DescribeResourceResponseTypeDef = TypedDict(
     "DescribeResourceResponseTypeDef",
     {
         "ResourceId": str,
         "Email": str,
         "Name": str,
         "Type": ResourceTypeType,
-        "BookingOptions": BookingOptionsTypeDef,
+        "BookingOptions": BookingOptionsOutputTypeDef,
         "State": EntityStateType,
         "EnabledDate": datetime,
         "DisabledDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateResourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceRequestRequestTypeDef",
     {
         "OrganizationId": str,
@@ -2003,28 +1892,14 @@
 class CreateImpersonationRoleRequestRequestTypeDef(
     _RequiredCreateImpersonationRoleRequestRequestTypeDef,
     _OptionalCreateImpersonationRoleRequestRequestTypeDef,
 ):
     pass
 
 
-GetImpersonationRoleResponseTypeDef = TypedDict(
-    "GetImpersonationRoleResponseTypeDef",
-    {
-        "ImpersonationRoleId": str,
-        "Name": str,
-        "Type": ImpersonationRoleTypeType,
-        "Description": str,
-        "Rules": List[ImpersonationRuleTypeDef],
-        "DateCreated": datetime,
-        "DateModified": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateImpersonationRoleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ImpersonationRoleId": str,
         "Name": str,
         "Type": ImpersonationRoleTypeType,
@@ -2074,38 +1949,38 @@
 
 
 ListResourceDelegatesResponseTypeDef = TypedDict(
     "ListResourceDelegatesResponseTypeDef",
     {
         "Delegates": List[DelegateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMailDomainResponseTypeDef = TypedDict(
     "GetMailDomainResponseTypeDef",
     {
         "Records": List[DnsRecordTypeDef],
         "IsTestDomain": bool,
         "IsDefault": bool,
         "OwnershipVerificationStatus": DnsRecordVerificationStatusType,
         "DkimVerificationStatus": DnsRecordVerificationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDefaultRetentionPolicyResponseTypeDef = TypedDict(
     "GetDefaultRetentionPolicyResponseTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
-        "FolderConfigurations": List[FolderConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FolderConfigurations": List[FolderConfigurationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutRetentionPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutRetentionPolicyRequestRequestTypeDef",
     {
         "OrganizationId": str,
@@ -2132,142 +2007,344 @@
 
 GetImpersonationRoleEffectResponseTypeDef = TypedDict(
     "GetImpersonationRoleEffectResponseTypeDef",
     {
         "Type": ImpersonationRoleTypeType,
         "Effect": AccessEffectType,
         "MatchedRules": List[ImpersonationMatchedRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetImpersonationRoleResponseTypeDef = TypedDict(
+    "GetImpersonationRoleResponseTypeDef",
+    {
+        "ImpersonationRoleId": str,
+        "Name": str,
+        "Type": ImpersonationRoleTypeType,
+        "Description": str,
+        "Rules": List[ImpersonationRuleOutputTypeDef],
+        "DateCreated": datetime,
+        "DateModified": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMobileDeviceAccessEffectResponseTypeDef = TypedDict(
     "GetMobileDeviceAccessEffectResponseTypeDef",
     {
         "Effect": MobileDeviceAccessRuleEffectType,
         "MatchedRules": List[MobileDeviceAccessMatchedRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImpersonationRolesResponseTypeDef = TypedDict(
     "ListImpersonationRolesResponseTypeDef",
     {
         "Roles": List[ImpersonationRoleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
+    "_RequiredListAliasesRequestListAliasesPaginateTypeDef",
+    {
+        "OrganizationId": str,
+        "EntityId": str,
+    },
+)
+_OptionalListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
+    "_OptionalListAliasesRequestListAliasesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAliasesRequestListAliasesPaginateTypeDef(
+    _RequiredListAliasesRequestListAliasesPaginateTypeDef,
+    _OptionalListAliasesRequestListAliasesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef = TypedDict(
+    "_RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
+    {
+        "OrganizationId": str,
+    },
+)
+_OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef = TypedDict(
+    "_OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef(
+    _RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
+    _OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef = TypedDict(
+    "_RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef",
+    {
+        "OrganizationId": str,
+        "GroupId": str,
+    },
+)
+_OptionalListGroupMembersRequestListGroupMembersPaginateTypeDef = TypedDict(
+    "_OptionalListGroupMembersRequestListGroupMembersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListGroupMembersRequestListGroupMembersPaginateTypeDef(
+    _RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef,
+    _OptionalListGroupMembersRequestListGroupMembersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "OrganizationId": str,
+    },
+)
+_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListGroupsRequestListGroupsPaginateTypeDef(
+    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
+    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef = TypedDict(
+    "_RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
+    {
+        "OrganizationId": str,
+        "EntityId": str,
+    },
+)
+_OptionalListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef = TypedDict(
+    "_OptionalListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef(
+    _RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
+    _OptionalListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
+):
+    pass
+
+
+ListOrganizationsRequestListOrganizationsPaginateTypeDef = TypedDict(
+    "ListOrganizationsRequestListOrganizationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef = TypedDict(
+    "_RequiredListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef",
+    {
+        "OrganizationId": str,
+        "ResourceId": str,
+    },
+)
+_OptionalListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef = TypedDict(
+    "_OptionalListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef(
+    _RequiredListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
+    _OptionalListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "OrganizationId": str,
     },
 )
+_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResourcesRequestListResourcesPaginateTypeDef(
+    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
+    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "OrganizationId": str,
+    },
+)
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
+):
+    pass
+
 
 ListGroupMembersResponseTypeDef = TypedDict(
     "ListGroupMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMailDomainsResponseTypeDef = TypedDict(
     "ListMailDomainsResponseTypeDef",
     {
         "MailDomains": List[MailDomainSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMailboxExportJobsResponseTypeDef = TypedDict(
     "ListMailboxExportJobsResponseTypeDef",
     {
         "Jobs": List[MailboxExportJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMailboxPermissionsResponseTypeDef = TypedDict(
     "ListMailboxPermissionsResponseTypeDef",
     {
         "Permissions": List[PermissionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMobileDeviceAccessOverridesResponseTypeDef = TypedDict(
     "ListMobileDeviceAccessOverridesResponseTypeDef",
     {
         "Overrides": List[MobileDeviceAccessOverrideTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMobileDeviceAccessRulesResponseTypeDef = TypedDict(
     "ListMobileDeviceAccessRulesResponseTypeDef",
     {
         "Rules": List[MobileDeviceAccessRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOrganizationsResponseTypeDef = TypedDict(
     "ListOrganizationsResponseTypeDef",
     {
         "OrganizationSummaries": List[OrganizationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesResponseTypeDef = TypedDict(
     "ListResourcesResponseTypeDef",
     {
         "Resources": List[ResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 ListAvailabilityConfigurationsResponseTypeDef = TypedDict(
     "ListAvailabilityConfigurationsResponseTypeDef",
     {
         "AvailabilityConfigurations": List[AvailabilityConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-workmail-1.28.0/mypy_boto3_workmail/type_defs.pyi` & `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -38,166 +38,171 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessControlRuleTypeDef",
     "AssociateDelegateToResourceRequestRequestTypeDef",
     "AssociateMemberToGroupRequestRequestTypeDef",
     "AssumeImpersonationRoleRequestRequestTypeDef",
-    "AssumeImpersonationRoleResponseTypeDef",
-    "LambdaAvailabilityProviderTypeDef",
+    "ResponseMetadataTypeDef",
+    "LambdaAvailabilityProviderOutputTypeDef",
     "RedactedEwsAvailabilityProviderTypeDef",
+    "BookingOptionsOutputTypeDef",
     "BookingOptionsTypeDef",
     "CancelMailboxExportJobRequestRequestTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "EwsAvailabilityProviderTypeDef",
+    "LambdaAvailabilityProviderTypeDef",
     "CreateGroupRequestRequestTypeDef",
-    "CreateGroupResponseTypeDef",
     "ImpersonationRuleTypeDef",
-    "CreateImpersonationRoleResponseTypeDef",
     "CreateMobileDeviceAccessRuleRequestRequestTypeDef",
-    "CreateMobileDeviceAccessRuleResponseTypeDef",
     "DomainTypeDef",
-    "CreateOrganizationResponseTypeDef",
     "CreateResourceRequestRequestTypeDef",
-    "CreateResourceResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
-    "CreateUserResponseTypeDef",
     "DelegateTypeDef",
     "DeleteAccessControlRuleRequestRequestTypeDef",
     "DeleteAliasRequestRequestTypeDef",
     "DeleteAvailabilityConfigurationRequestRequestTypeDef",
     "DeleteEmailMonitoringConfigurationRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteImpersonationRoleRequestRequestTypeDef",
     "DeleteMailboxPermissionsRequestRequestTypeDef",
     "DeleteMobileDeviceAccessOverrideRequestRequestTypeDef",
     "DeleteMobileDeviceAccessRuleRequestRequestTypeDef",
     "DeleteOrganizationRequestRequestTypeDef",
-    "DeleteOrganizationResponseTypeDef",
     "DeleteResourceRequestRequestTypeDef",
     "DeleteRetentionPolicyRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DeregisterFromWorkMailRequestRequestTypeDef",
     "DeregisterMailDomainRequestRequestTypeDef",
     "DescribeEmailMonitoringConfigurationRequestRequestTypeDef",
-    "DescribeEmailMonitoringConfigurationResponseTypeDef",
     "DescribeGroupRequestRequestTypeDef",
-    "DescribeGroupResponseTypeDef",
     "DescribeInboundDmarcSettingsRequestRequestTypeDef",
-    "DescribeInboundDmarcSettingsResponseTypeDef",
     "DescribeMailboxExportJobRequestRequestTypeDef",
-    "DescribeMailboxExportJobResponseTypeDef",
     "DescribeOrganizationRequestRequestTypeDef",
-    "DescribeOrganizationResponseTypeDef",
     "DescribeResourceRequestRequestTypeDef",
     "DescribeUserRequestRequestTypeDef",
-    "DescribeUserResponseTypeDef",
     "DisassociateDelegateFromResourceRequestRequestTypeDef",
     "DisassociateMemberFromGroupRequestRequestTypeDef",
     "DnsRecordTypeDef",
+    "FolderConfigurationOutputTypeDef",
     "FolderConfigurationTypeDef",
     "GetAccessControlEffectRequestRequestTypeDef",
-    "GetAccessControlEffectResponseTypeDef",
     "GetDefaultRetentionPolicyRequestRequestTypeDef",
     "GetImpersonationRoleEffectRequestRequestTypeDef",
     "ImpersonationMatchedRuleTypeDef",
     "GetImpersonationRoleRequestRequestTypeDef",
+    "ImpersonationRuleOutputTypeDef",
     "GetMailDomainRequestRequestTypeDef",
     "GetMailboxDetailsRequestRequestTypeDef",
-    "GetMailboxDetailsResponseTypeDef",
     "GetMobileDeviceAccessEffectRequestRequestTypeDef",
     "MobileDeviceAccessMatchedRuleTypeDef",
     "GetMobileDeviceAccessOverrideRequestRequestTypeDef",
-    "GetMobileDeviceAccessOverrideResponseTypeDef",
     "GroupTypeDef",
     "ImpersonationRoleTypeDef",
     "ListAccessControlRulesRequestRequestTypeDef",
-    "ListAliasesRequestListAliasesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAliasesRequestRequestTypeDef",
-    "ListAliasesResponseTypeDef",
-    "ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
     "ListAvailabilityConfigurationsRequestRequestTypeDef",
-    "ListGroupMembersRequestListGroupMembersPaginateTypeDef",
     "ListGroupMembersRequestRequestTypeDef",
     "MemberTypeDef",
-    "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
     "ListImpersonationRolesRequestRequestTypeDef",
     "ListMailDomainsRequestRequestTypeDef",
     "MailDomainSummaryTypeDef",
     "ListMailboxExportJobsRequestRequestTypeDef",
     "MailboxExportJobTypeDef",
-    "ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
     "ListMailboxPermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
     "ListMobileDeviceAccessOverridesRequestRequestTypeDef",
     "MobileDeviceAccessOverrideTypeDef",
     "ListMobileDeviceAccessRulesRequestRequestTypeDef",
     "MobileDeviceAccessRuleTypeDef",
-    "ListOrganizationsRequestListOrganizationsPaginateTypeDef",
     "ListOrganizationsRequestRequestTypeDef",
     "OrganizationSummaryTypeDef",
-    "ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef",
     "ListResourceDelegatesRequestRequestTypeDef",
-    "ListResourcesRequestListResourcesPaginateTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
+    "TagOutputTypeDef",
     "ListUsersRequestRequestTypeDef",
     "UserTypeDef",
-    "PaginatorConfigTypeDef",
     "PutAccessControlRuleRequestRequestTypeDef",
     "PutEmailMonitoringConfigurationRequestRequestTypeDef",
     "PutInboundDmarcSettingsRequestRequestTypeDef",
     "PutMailboxPermissionsRequestRequestTypeDef",
     "PutMobileDeviceAccessOverrideRequestRequestTypeDef",
     "RegisterMailDomainRequestRequestTypeDef",
     "RegisterToWorkMailRequestRequestTypeDef",
     "ResetPasswordRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StartMailboxExportJobRequestRequestTypeDef",
-    "StartMailboxExportJobResponseTypeDef",
-    "TestAvailabilityConfigurationResponseTypeDef",
+    "TagTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDefaultMailDomainRequestRequestTypeDef",
     "UpdateMailboxQuotaRequestRequestTypeDef",
     "UpdateMobileDeviceAccessRuleRequestRequestTypeDef",
     "UpdatePrimaryEmailAddressRequestRequestTypeDef",
+    "AssumeImpersonationRoleResponseTypeDef",
+    "CreateGroupResponseTypeDef",
+    "CreateImpersonationRoleResponseTypeDef",
+    "CreateMobileDeviceAccessRuleResponseTypeDef",
+    "CreateOrganizationResponseTypeDef",
+    "CreateResourceResponseTypeDef",
+    "CreateUserResponseTypeDef",
+    "DeleteOrganizationResponseTypeDef",
+    "DescribeEmailMonitoringConfigurationResponseTypeDef",
+    "DescribeGroupResponseTypeDef",
+    "DescribeInboundDmarcSettingsResponseTypeDef",
+    "DescribeMailboxExportJobResponseTypeDef",
+    "DescribeOrganizationResponseTypeDef",
+    "DescribeUserResponseTypeDef",
+    "GetAccessControlEffectResponseTypeDef",
+    "GetMailboxDetailsResponseTypeDef",
+    "GetMobileDeviceAccessOverrideResponseTypeDef",
     "ListAccessControlRulesResponseTypeDef",
+    "ListAliasesResponseTypeDef",
+    "StartMailboxExportJobResponseTypeDef",
+    "TestAvailabilityConfigurationResponseTypeDef",
     "AvailabilityConfigurationTypeDef",
     "DescribeResourceResponseTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "CreateAvailabilityConfigurationRequestRequestTypeDef",
     "TestAvailabilityConfigurationRequestRequestTypeDef",
     "UpdateAvailabilityConfigurationRequestRequestTypeDef",
     "CreateImpersonationRoleRequestRequestTypeDef",
-    "GetImpersonationRoleResponseTypeDef",
     "UpdateImpersonationRoleRequestRequestTypeDef",
     "CreateOrganizationRequestRequestTypeDef",
     "ListResourceDelegatesResponseTypeDef",
     "GetMailDomainResponseTypeDef",
     "GetDefaultRetentionPolicyResponseTypeDef",
     "PutRetentionPolicyRequestRequestTypeDef",
     "GetImpersonationRoleEffectResponseTypeDef",
+    "GetImpersonationRoleResponseTypeDef",
     "GetMobileDeviceAccessEffectResponseTypeDef",
     "ListGroupsResponseTypeDef",
     "ListImpersonationRolesResponseTypeDef",
+    "ListAliasesRequestListAliasesPaginateTypeDef",
+    "ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
+    "ListGroupMembersRequestListGroupMembersPaginateTypeDef",
+    "ListGroupsRequestListGroupsPaginateTypeDef",
+    "ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
+    "ListOrganizationsRequestListOrganizationsPaginateTypeDef",
+    "ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef",
+    "ListResourcesRequestListResourcesPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
     "ListGroupMembersResponseTypeDef",
     "ListMailDomainsResponseTypeDef",
     "ListMailboxExportJobsResponseTypeDef",
     "ListMailboxPermissionsResponseTypeDef",
     "ListMobileDeviceAccessOverridesResponseTypeDef",
     "ListMobileDeviceAccessRulesResponseTypeDef",
     "ListOrganizationsResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "ListUsersResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "ListAvailabilityConfigurationsResponseTypeDef",
 )
 
 AccessControlRuleTypeDef = TypedDict(
     "AccessControlRuleTypeDef",
     {
         "Name": str,
@@ -239,39 +244,51 @@
     "AssumeImpersonationRoleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ImpersonationRoleId": str,
     },
 )
 
-AssumeImpersonationRoleResponseTypeDef = TypedDict(
-    "AssumeImpersonationRoleResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Token": str,
-        "ExpiresIn": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-LambdaAvailabilityProviderTypeDef = TypedDict(
-    "LambdaAvailabilityProviderTypeDef",
+LambdaAvailabilityProviderOutputTypeDef = TypedDict(
+    "LambdaAvailabilityProviderOutputTypeDef",
     {
         "LambdaArn": str,
     },
 )
 
 RedactedEwsAvailabilityProviderTypeDef = TypedDict(
     "RedactedEwsAvailabilityProviderTypeDef",
     {
         "EwsEndpoint": str,
         "EwsUsername": str,
     },
     total=False,
 )
 
+BookingOptionsOutputTypeDef = TypedDict(
+    "BookingOptionsOutputTypeDef",
+    {
+        "AutoAcceptRequests": bool,
+        "AutoDeclineRecurringRequests": bool,
+        "AutoDeclineConflictingRequests": bool,
+    },
+    total=False,
+)
+
 BookingOptionsTypeDef = TypedDict(
     "BookingOptionsTypeDef",
     {
         "AutoAcceptRequests": bool,
         "AutoDeclineRecurringRequests": bool,
         "AutoDeclineConflictingRequests": bool,
     },
@@ -301,27 +318,26 @@
     {
         "EwsEndpoint": str,
         "EwsUsername": str,
         "EwsPassword": str,
     },
 )
 
-CreateGroupRequestRequestTypeDef = TypedDict(
-    "CreateGroupRequestRequestTypeDef",
+LambdaAvailabilityProviderTypeDef = TypedDict(
+    "LambdaAvailabilityProviderTypeDef",
     {
-        "OrganizationId": str,
-        "Name": str,
+        "LambdaArn": str,
     },
 )
 
-CreateGroupResponseTypeDef = TypedDict(
-    "CreateGroupResponseTypeDef",
+CreateGroupRequestRequestTypeDef = TypedDict(
+    "CreateGroupRequestRequestTypeDef",
     {
-        "GroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "OrganizationId": str,
+        "Name": str,
     },
 )
 
 _RequiredImpersonationRuleTypeDef = TypedDict(
     "_RequiredImpersonationRuleTypeDef",
     {
         "ImpersonationRuleId": str,
@@ -340,22 +356,14 @@
 )
 
 class ImpersonationRuleTypeDef(
     _RequiredImpersonationRuleTypeDef, _OptionalImpersonationRuleTypeDef
 ):
     pass
 
-CreateImpersonationRoleResponseTypeDef = TypedDict(
-    "CreateImpersonationRoleResponseTypeDef",
-    {
-        "ImpersonationRoleId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
         "Effect": MobileDeviceAccessRuleEffectType,
     },
@@ -379,74 +387,42 @@
 
 class CreateMobileDeviceAccessRuleRequestRequestTypeDef(
     _RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef,
     _OptionalCreateMobileDeviceAccessRuleRequestRequestTypeDef,
 ):
     pass
 
-CreateMobileDeviceAccessRuleResponseTypeDef = TypedDict(
-    "CreateMobileDeviceAccessRuleResponseTypeDef",
-    {
-        "MobileDeviceAccessRuleId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DomainTypeDef = TypedDict(
     "DomainTypeDef",
     {
         "DomainName": str,
         "HostedZoneId": str,
     },
     total=False,
 )
 
-CreateOrganizationResponseTypeDef = TypedDict(
-    "CreateOrganizationResponseTypeDef",
-    {
-        "OrganizationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateResourceRequestRequestTypeDef = TypedDict(
     "CreateResourceRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
         "Type": ResourceTypeType,
     },
 )
 
-CreateResourceResponseTypeDef = TypedDict(
-    "CreateResourceResponseTypeDef",
-    {
-        "ResourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateUserRequestRequestTypeDef = TypedDict(
     "CreateUserRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
         "DisplayName": str,
         "Password": str,
     },
 )
 
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
-    {
-        "UserId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DelegateTypeDef = TypedDict(
     "DelegateTypeDef",
     {
         "Id": str,
         "Type": MemberTypeType,
     },
 )
@@ -542,23 +518,14 @@
 
 class DeleteOrganizationRequestRequestTypeDef(
     _RequiredDeleteOrganizationRequestRequestTypeDef,
     _OptionalDeleteOrganizationRequestRequestTypeDef,
 ):
     pass
 
-DeleteOrganizationResponseTypeDef = TypedDict(
-    "DeleteOrganizationResponseTypeDef",
-    {
-        "OrganizationId": str,
-        "State": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteResourceRequestRequestTypeDef = TypedDict(
     "DeleteResourceRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ResourceId": str,
     },
 )
@@ -598,109 +565,44 @@
 DescribeEmailMonitoringConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeEmailMonitoringConfigurationRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 
-DescribeEmailMonitoringConfigurationResponseTypeDef = TypedDict(
-    "DescribeEmailMonitoringConfigurationResponseTypeDef",
-    {
-        "RoleArn": str,
-        "LogGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeGroupRequestRequestTypeDef = TypedDict(
     "DescribeGroupRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "GroupId": str,
     },
 )
 
-DescribeGroupResponseTypeDef = TypedDict(
-    "DescribeGroupResponseTypeDef",
-    {
-        "GroupId": str,
-        "Name": str,
-        "Email": str,
-        "State": EntityStateType,
-        "EnabledDate": datetime,
-        "DisabledDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeInboundDmarcSettingsRequestRequestTypeDef = TypedDict(
     "DescribeInboundDmarcSettingsRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 
-DescribeInboundDmarcSettingsResponseTypeDef = TypedDict(
-    "DescribeInboundDmarcSettingsResponseTypeDef",
-    {
-        "Enforced": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeMailboxExportJobRequestRequestTypeDef = TypedDict(
     "DescribeMailboxExportJobRequestRequestTypeDef",
     {
         "JobId": str,
         "OrganizationId": str,
     },
 )
 
-DescribeMailboxExportJobResponseTypeDef = TypedDict(
-    "DescribeMailboxExportJobResponseTypeDef",
-    {
-        "EntityId": str,
-        "Description": str,
-        "RoleArn": str,
-        "KmsKeyArn": str,
-        "S3BucketName": str,
-        "S3Prefix": str,
-        "S3Path": str,
-        "EstimatedProgress": int,
-        "State": MailboxExportJobStateType,
-        "ErrorInfo": str,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeOrganizationRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 
-DescribeOrganizationResponseTypeDef = TypedDict(
-    "DescribeOrganizationResponseTypeDef",
-    {
-        "OrganizationId": str,
-        "Alias": str,
-        "State": str,
-        "DirectoryId": str,
-        "DirectoryType": str,
-        "DefaultMailDomain": str,
-        "CompletedDate": datetime,
-        "ErrorMessage": str,
-        "ARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeResourceRequestRequestTypeDef = TypedDict(
     "DescribeResourceRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ResourceId": str,
     },
 )
@@ -709,29 +611,14 @@
     "DescribeUserRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "UserId": str,
     },
 )
 
-DescribeUserResponseTypeDef = TypedDict(
-    "DescribeUserResponseTypeDef",
-    {
-        "UserId": str,
-        "Name": str,
-        "Email": str,
-        "DisplayName": str,
-        "State": EntityStateType,
-        "UserRole": UserRoleType,
-        "EnabledDate": datetime,
-        "DisabledDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateDelegateFromResourceRequestRequestTypeDef = TypedDict(
     "DisassociateDelegateFromResourceRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ResourceId": str,
         "EntityId": str,
     },
@@ -752,14 +639,34 @@
         "Type": str,
         "Hostname": str,
         "Value": str,
     },
     total=False,
 )
 
+_RequiredFolderConfigurationOutputTypeDef = TypedDict(
+    "_RequiredFolderConfigurationOutputTypeDef",
+    {
+        "Name": FolderNameType,
+        "Action": RetentionActionType,
+    },
+)
+_OptionalFolderConfigurationOutputTypeDef = TypedDict(
+    "_OptionalFolderConfigurationOutputTypeDef",
+    {
+        "Period": int,
+    },
+    total=False,
+)
+
+class FolderConfigurationOutputTypeDef(
+    _RequiredFolderConfigurationOutputTypeDef, _OptionalFolderConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredFolderConfigurationTypeDef = TypedDict(
     "_RequiredFolderConfigurationTypeDef",
     {
         "Name": FolderNameType,
         "Action": RetentionActionType,
     },
 )
@@ -795,23 +702,14 @@
 
 class GetAccessControlEffectRequestRequestTypeDef(
     _RequiredGetAccessControlEffectRequestRequestTypeDef,
     _OptionalGetAccessControlEffectRequestRequestTypeDef,
 ):
     pass
 
-GetAccessControlEffectResponseTypeDef = TypedDict(
-    "GetAccessControlEffectResponseTypeDef",
-    {
-        "Effect": AccessControlRuleEffectType,
-        "MatchedRules": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDefaultRetentionPolicyRequestRequestTypeDef = TypedDict(
     "GetDefaultRetentionPolicyRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 
@@ -837,14 +735,37 @@
     "GetImpersonationRoleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ImpersonationRoleId": str,
     },
 )
 
+_RequiredImpersonationRuleOutputTypeDef = TypedDict(
+    "_RequiredImpersonationRuleOutputTypeDef",
+    {
+        "ImpersonationRuleId": str,
+        "Effect": AccessEffectType,
+    },
+)
+_OptionalImpersonationRuleOutputTypeDef = TypedDict(
+    "_OptionalImpersonationRuleOutputTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "TargetUsers": List[str],
+        "NotTargetUsers": List[str],
+    },
+    total=False,
+)
+
+class ImpersonationRuleOutputTypeDef(
+    _RequiredImpersonationRuleOutputTypeDef, _OptionalImpersonationRuleOutputTypeDef
+):
+    pass
+
 GetMailDomainRequestRequestTypeDef = TypedDict(
     "GetMailDomainRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -853,23 +774,14 @@
     "GetMailboxDetailsRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "UserId": str,
     },
 )
 
-GetMailboxDetailsResponseTypeDef = TypedDict(
-    "GetMailboxDetailsResponseTypeDef",
-    {
-        "MailboxQuota": int,
-        "MailboxSize": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMobileDeviceAccessEffectRequestRequestTypeDef = TypedDict(
     "_RequiredGetMobileDeviceAccessEffectRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalGetMobileDeviceAccessEffectRequestRequestTypeDef = TypedDict(
@@ -903,27 +815,14 @@
     {
         "OrganizationId": str,
         "UserId": str,
         "DeviceId": str,
     },
 )
 
-GetMobileDeviceAccessOverrideResponseTypeDef = TypedDict(
-    "GetMobileDeviceAccessOverrideResponseTypeDef",
-    {
-        "UserId": str,
-        "DeviceId": str,
-        "Effect": MobileDeviceAccessRuleEffectType,
-        "Description": str,
-        "DateCreated": datetime,
-        "DateModified": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GroupTypeDef = TypedDict(
     "GroupTypeDef",
     {
         "Id": str,
         "Email": str,
         "Name": str,
         "State": EntityStateType,
@@ -948,35 +847,24 @@
 ListAccessControlRulesRequestRequestTypeDef = TypedDict(
     "ListAccessControlRulesRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 
-_RequiredListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
-    "_RequiredListAliasesRequestListAliasesPaginateTypeDef",
-    {
-        "OrganizationId": str,
-        "EntityId": str,
-    },
-)
-_OptionalListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
-    "_OptionalListAliasesRequestListAliasesPaginateTypeDef",
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
 
-class ListAliasesRequestListAliasesPaginateTypeDef(
-    _RequiredListAliasesRequestListAliasesPaginateTypeDef,
-    _OptionalListAliasesRequestListAliasesPaginateTypeDef,
-):
-    pass
-
 _RequiredListAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredListAliasesRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "EntityId": str,
     },
 )
@@ -990,43 +878,14 @@
 )
 
 class ListAliasesRequestRequestTypeDef(
     _RequiredListAliasesRequestRequestTypeDef, _OptionalListAliasesRequestRequestTypeDef
 ):
     pass
 
-ListAliasesResponseTypeDef = TypedDict(
-    "ListAliasesResponseTypeDef",
-    {
-        "Aliases": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef = TypedDict(
-    "_RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
-    {
-        "OrganizationId": str,
-    },
-)
-_OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef = TypedDict(
-    "_OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef(
-    _RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
-    _OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAvailabilityConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailabilityConfigurationsRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListAvailabilityConfigurationsRequestRequestTypeDef = TypedDict(
@@ -1040,35 +899,14 @@
 
 class ListAvailabilityConfigurationsRequestRequestTypeDef(
     _RequiredListAvailabilityConfigurationsRequestRequestTypeDef,
     _OptionalListAvailabilityConfigurationsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef = TypedDict(
-    "_RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef",
-    {
-        "OrganizationId": str,
-        "GroupId": str,
-    },
-)
-_OptionalListGroupMembersRequestListGroupMembersPaginateTypeDef = TypedDict(
-    "_OptionalListGroupMembersRequestListGroupMembersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListGroupMembersRequestListGroupMembersPaginateTypeDef(
-    _RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef,
-    _OptionalListGroupMembersRequestListGroupMembersPaginateTypeDef,
-):
-    pass
-
 _RequiredListGroupMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembersRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "GroupId": str,
     },
 )
@@ -1095,34 +933,14 @@
         "State": EntityStateType,
         "EnabledDate": datetime,
         "DisabledDate": datetime,
     },
     total=False,
 )
 
-_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "OrganizationId": str,
-    },
-)
-_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListGroupsRequestListGroupsPaginateTypeDef(
-    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
-    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
-):
-    pass
-
 _RequiredListGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupsRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListGroupsRequestRequestTypeDef = TypedDict(
@@ -1222,35 +1040,14 @@
         "State": MailboxExportJobStateType,
         "StartTime": datetime,
         "EndTime": datetime,
     },
     total=False,
 )
 
-_RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef = TypedDict(
-    "_RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
-    {
-        "OrganizationId": str,
-        "EntityId": str,
-    },
-)
-_OptionalListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef = TypedDict(
-    "_OptionalListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef(
-    _RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
-    _OptionalListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListMailboxPermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredListMailboxPermissionsRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "EntityId": str,
     },
 )
@@ -1338,22 +1135,14 @@
         "NotDeviceUserAgents": List[str],
         "DateCreated": datetime,
         "DateModified": datetime,
     },
     total=False,
 )
 
-ListOrganizationsRequestListOrganizationsPaginateTypeDef = TypedDict(
-    "ListOrganizationsRequestListOrganizationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOrganizationsRequestRequestTypeDef = TypedDict(
     "ListOrganizationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1367,35 +1156,14 @@
         "DefaultMailDomain": str,
         "ErrorMessage": str,
         "State": str,
     },
     total=False,
 )
 
-_RequiredListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef = TypedDict(
-    "_RequiredListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef",
-    {
-        "OrganizationId": str,
-        "ResourceId": str,
-    },
-)
-_OptionalListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef = TypedDict(
-    "_OptionalListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef(
-    _RequiredListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
-    _OptionalListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
-):
-    pass
-
 _RequiredListResourceDelegatesRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceDelegatesRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ResourceId": str,
     },
 )
@@ -1410,34 +1178,14 @@
 
 class ListResourceDelegatesRequestRequestTypeDef(
     _RequiredListResourceDelegatesRequestRequestTypeDef,
     _OptionalListResourceDelegatesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "OrganizationId": str,
-    },
-)
-_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListResourcesRequestListResourcesPaginateTypeDef(
-    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
-    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredListResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListResourcesRequestRequestTypeDef = TypedDict(
@@ -1471,42 +1219,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "OrganizationId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
-):
-    pass
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -1534,24 +1262,14 @@
         "UserRole": UserRoleType,
         "EnabledDate": datetime,
         "DisabledDate": datetime,
     },
     total=False,
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
 _RequiredPutAccessControlRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutAccessControlRuleRequestRequestTypeDef",
     {
         "Name": str,
         "Effect": AccessControlRuleEffectType,
         "Description": str,
         "OrganizationId": str,
@@ -1663,25 +1381,14 @@
     {
         "OrganizationId": str,
         "UserId": str,
         "Password": str,
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
 _RequiredStartMailboxExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartMailboxExportJobRequestRequestTypeDef",
     {
         "ClientToken": str,
         "OrganizationId": str,
         "EntityId": str,
         "RoleArn": str,
@@ -1700,28 +1407,19 @@
 
 class StartMailboxExportJobRequestRequestTypeDef(
     _RequiredStartMailboxExportJobRequestRequestTypeDef,
     _OptionalStartMailboxExportJobRequestRequestTypeDef,
 ):
     pass
 
-StartMailboxExportJobResponseTypeDef = TypedDict(
-    "StartMailboxExportJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TestAvailabilityConfigurationResponseTypeDef = TypedDict(
-    "TestAvailabilityConfigurationResponseTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "TestPassed": bool,
-        "FailureReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": str,
+        "Value": str,
     },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -1782,47 +1480,250 @@
     {
         "OrganizationId": str,
         "EntityId": str,
         "Email": str,
     },
 )
 
+AssumeImpersonationRoleResponseTypeDef = TypedDict(
+    "AssumeImpersonationRoleResponseTypeDef",
+    {
+        "Token": str,
+        "ExpiresIn": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGroupResponseTypeDef = TypedDict(
+    "CreateGroupResponseTypeDef",
+    {
+        "GroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateImpersonationRoleResponseTypeDef = TypedDict(
+    "CreateImpersonationRoleResponseTypeDef",
+    {
+        "ImpersonationRoleId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMobileDeviceAccessRuleResponseTypeDef = TypedDict(
+    "CreateMobileDeviceAccessRuleResponseTypeDef",
+    {
+        "MobileDeviceAccessRuleId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateOrganizationResponseTypeDef = TypedDict(
+    "CreateOrganizationResponseTypeDef",
+    {
+        "OrganizationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateResourceResponseTypeDef = TypedDict(
+    "CreateResourceResponseTypeDef",
+    {
+        "ResourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
+    {
+        "UserId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteOrganizationResponseTypeDef = TypedDict(
+    "DeleteOrganizationResponseTypeDef",
+    {
+        "OrganizationId": str,
+        "State": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEmailMonitoringConfigurationResponseTypeDef = TypedDict(
+    "DescribeEmailMonitoringConfigurationResponseTypeDef",
+    {
+        "RoleArn": str,
+        "LogGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGroupResponseTypeDef = TypedDict(
+    "DescribeGroupResponseTypeDef",
+    {
+        "GroupId": str,
+        "Name": str,
+        "Email": str,
+        "State": EntityStateType,
+        "EnabledDate": datetime,
+        "DisabledDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeInboundDmarcSettingsResponseTypeDef = TypedDict(
+    "DescribeInboundDmarcSettingsResponseTypeDef",
+    {
+        "Enforced": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeMailboxExportJobResponseTypeDef = TypedDict(
+    "DescribeMailboxExportJobResponseTypeDef",
+    {
+        "EntityId": str,
+        "Description": str,
+        "RoleArn": str,
+        "KmsKeyArn": str,
+        "S3BucketName": str,
+        "S3Prefix": str,
+        "S3Path": str,
+        "EstimatedProgress": int,
+        "State": MailboxExportJobStateType,
+        "ErrorInfo": str,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationResponseTypeDef = TypedDict(
+    "DescribeOrganizationResponseTypeDef",
+    {
+        "OrganizationId": str,
+        "Alias": str,
+        "State": str,
+        "DirectoryId": str,
+        "DirectoryType": str,
+        "DefaultMailDomain": str,
+        "CompletedDate": datetime,
+        "ErrorMessage": str,
+        "ARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeUserResponseTypeDef = TypedDict(
+    "DescribeUserResponseTypeDef",
+    {
+        "UserId": str,
+        "Name": str,
+        "Email": str,
+        "DisplayName": str,
+        "State": EntityStateType,
+        "UserRole": UserRoleType,
+        "EnabledDate": datetime,
+        "DisabledDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccessControlEffectResponseTypeDef = TypedDict(
+    "GetAccessControlEffectResponseTypeDef",
+    {
+        "Effect": AccessControlRuleEffectType,
+        "MatchedRules": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMailboxDetailsResponseTypeDef = TypedDict(
+    "GetMailboxDetailsResponseTypeDef",
+    {
+        "MailboxQuota": int,
+        "MailboxSize": float,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMobileDeviceAccessOverrideResponseTypeDef = TypedDict(
+    "GetMobileDeviceAccessOverrideResponseTypeDef",
+    {
+        "UserId": str,
+        "DeviceId": str,
+        "Effect": MobileDeviceAccessRuleEffectType,
+        "Description": str,
+        "DateCreated": datetime,
+        "DateModified": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAccessControlRulesResponseTypeDef = TypedDict(
     "ListAccessControlRulesResponseTypeDef",
     {
         "Rules": List[AccessControlRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAliasesResponseTypeDef = TypedDict(
+    "ListAliasesResponseTypeDef",
+    {
+        "Aliases": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartMailboxExportJobResponseTypeDef = TypedDict(
+    "StartMailboxExportJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestAvailabilityConfigurationResponseTypeDef = TypedDict(
+    "TestAvailabilityConfigurationResponseTypeDef",
+    {
+        "TestPassed": bool,
+        "FailureReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AvailabilityConfigurationTypeDef = TypedDict(
     "AvailabilityConfigurationTypeDef",
     {
         "DomainName": str,
         "ProviderType": AvailabilityProviderTypeType,
         "EwsProvider": RedactedEwsAvailabilityProviderTypeDef,
-        "LambdaProvider": LambdaAvailabilityProviderTypeDef,
+        "LambdaProvider": LambdaAvailabilityProviderOutputTypeDef,
         "DateCreated": datetime,
         "DateModified": datetime,
     },
     total=False,
 )
 
 DescribeResourceResponseTypeDef = TypedDict(
     "DescribeResourceResponseTypeDef",
     {
         "ResourceId": str,
         "Email": str,
         "Name": str,
         "Type": ResourceTypeType,
-        "BookingOptions": BookingOptionsTypeDef,
+        "BookingOptions": BookingOptionsOutputTypeDef,
         "State": EntityStateType,
         "EnabledDate": datetime,
         "DisabledDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateResourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceRequestRequestTypeDef",
     {
         "OrganizationId": str,
@@ -1930,28 +1831,14 @@
 
 class CreateImpersonationRoleRequestRequestTypeDef(
     _RequiredCreateImpersonationRoleRequestRequestTypeDef,
     _OptionalCreateImpersonationRoleRequestRequestTypeDef,
 ):
     pass
 
-GetImpersonationRoleResponseTypeDef = TypedDict(
-    "GetImpersonationRoleResponseTypeDef",
-    {
-        "ImpersonationRoleId": str,
-        "Name": str,
-        "Type": ImpersonationRoleTypeType,
-        "Description": str,
-        "Rules": List[ImpersonationRuleTypeDef],
-        "DateCreated": datetime,
-        "DateModified": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateImpersonationRoleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ImpersonationRoleId": str,
         "Name": str,
         "Type": ImpersonationRoleTypeType,
@@ -1997,38 +1884,38 @@
     pass
 
 ListResourceDelegatesResponseTypeDef = TypedDict(
     "ListResourceDelegatesResponseTypeDef",
     {
         "Delegates": List[DelegateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMailDomainResponseTypeDef = TypedDict(
     "GetMailDomainResponseTypeDef",
     {
         "Records": List[DnsRecordTypeDef],
         "IsTestDomain": bool,
         "IsDefault": bool,
         "OwnershipVerificationStatus": DnsRecordVerificationStatusType,
         "DkimVerificationStatus": DnsRecordVerificationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDefaultRetentionPolicyResponseTypeDef = TypedDict(
     "GetDefaultRetentionPolicyResponseTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
-        "FolderConfigurations": List[FolderConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FolderConfigurations": List[FolderConfigurationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutRetentionPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutRetentionPolicyRequestRequestTypeDef",
     {
         "OrganizationId": str,
@@ -2053,142 +1940,328 @@
 
 GetImpersonationRoleEffectResponseTypeDef = TypedDict(
     "GetImpersonationRoleEffectResponseTypeDef",
     {
         "Type": ImpersonationRoleTypeType,
         "Effect": AccessEffectType,
         "MatchedRules": List[ImpersonationMatchedRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetImpersonationRoleResponseTypeDef = TypedDict(
+    "GetImpersonationRoleResponseTypeDef",
+    {
+        "ImpersonationRoleId": str,
+        "Name": str,
+        "Type": ImpersonationRoleTypeType,
+        "Description": str,
+        "Rules": List[ImpersonationRuleOutputTypeDef],
+        "DateCreated": datetime,
+        "DateModified": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMobileDeviceAccessEffectResponseTypeDef = TypedDict(
     "GetMobileDeviceAccessEffectResponseTypeDef",
     {
         "Effect": MobileDeviceAccessRuleEffectType,
         "MatchedRules": List[MobileDeviceAccessMatchedRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImpersonationRolesResponseTypeDef = TypedDict(
     "ListImpersonationRolesResponseTypeDef",
     {
         "Roles": List[ImpersonationRoleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
+    "_RequiredListAliasesRequestListAliasesPaginateTypeDef",
+    {
+        "OrganizationId": str,
+        "EntityId": str,
+    },
+)
+_OptionalListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
+    "_OptionalListAliasesRequestListAliasesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAliasesRequestListAliasesPaginateTypeDef(
+    _RequiredListAliasesRequestListAliasesPaginateTypeDef,
+    _OptionalListAliasesRequestListAliasesPaginateTypeDef,
+):
+    pass
+
+_RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef = TypedDict(
+    "_RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
+    {
+        "OrganizationId": str,
+    },
+)
+_OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef = TypedDict(
+    "_OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+class ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef(
+    _RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
+    _OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
+):
+    pass
+
+_RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef = TypedDict(
+    "_RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef",
+    {
+        "OrganizationId": str,
+        "GroupId": str,
+    },
+)
+_OptionalListGroupMembersRequestListGroupMembersPaginateTypeDef = TypedDict(
+    "_OptionalListGroupMembersRequestListGroupMembersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListGroupMembersRequestListGroupMembersPaginateTypeDef(
+    _RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef,
+    _OptionalListGroupMembersRequestListGroupMembersPaginateTypeDef,
+):
+    pass
+
+_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "OrganizationId": str,
+    },
+)
+_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListGroupsRequestListGroupsPaginateTypeDef(
+    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
+    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
+):
+    pass
+
+_RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef = TypedDict(
+    "_RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
+    {
+        "OrganizationId": str,
+        "EntityId": str,
+    },
+)
+_OptionalListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef = TypedDict(
+    "_OptionalListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef(
+    _RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
+    _OptionalListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
+):
+    pass
+
+ListOrganizationsRequestListOrganizationsPaginateTypeDef = TypedDict(
+    "ListOrganizationsRequestListOrganizationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef = TypedDict(
+    "_RequiredListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef",
+    {
+        "OrganizationId": str,
+        "ResourceId": str,
+    },
+)
+_OptionalListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef = TypedDict(
+    "_OptionalListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef(
+    _RequiredListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
+    _OptionalListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
+):
+    pass
+
+_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "OrganizationId": str,
+    },
+)
+_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListResourcesRequestListResourcesPaginateTypeDef(
+    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
+    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
+):
+    pass
+
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "OrganizationId": str,
+    },
+)
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
+):
+    pass
+
 ListGroupMembersResponseTypeDef = TypedDict(
     "ListGroupMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMailDomainsResponseTypeDef = TypedDict(
     "ListMailDomainsResponseTypeDef",
     {
         "MailDomains": List[MailDomainSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMailboxExportJobsResponseTypeDef = TypedDict(
     "ListMailboxExportJobsResponseTypeDef",
     {
         "Jobs": List[MailboxExportJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMailboxPermissionsResponseTypeDef = TypedDict(
     "ListMailboxPermissionsResponseTypeDef",
     {
         "Permissions": List[PermissionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMobileDeviceAccessOverridesResponseTypeDef = TypedDict(
     "ListMobileDeviceAccessOverridesResponseTypeDef",
     {
         "Overrides": List[MobileDeviceAccessOverrideTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMobileDeviceAccessRulesResponseTypeDef = TypedDict(
     "ListMobileDeviceAccessRulesResponseTypeDef",
     {
         "Rules": List[MobileDeviceAccessRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOrganizationsResponseTypeDef = TypedDict(
     "ListOrganizationsResponseTypeDef",
     {
         "OrganizationSummaries": List[OrganizationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesResponseTypeDef = TypedDict(
     "ListResourcesResponseTypeDef",
     {
         "Resources": List[ResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 ListAvailabilityConfigurationsResponseTypeDef = TypedDict(
     "ListAvailabilityConfigurationsResponseTypeDef",
     {
         "AvailabilityConfigurations": List[AvailabilityConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-workmail-1.28.0/mypy_boto3_workmail.egg-info/PKG-INFO` & `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workmail
-Version: 1.28.0
-Summary: Type annotations for boto3.WorkMail 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.WorkMail 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-workmail"></a>
 
 # mypy-boto3-workmail
 
 [![PyPI - mypy-boto3-workmail](https://img.shields.io/pypi/v/mypy-boto3-workmail.svg?color=blue)](https://pypi.org/project/mypy-boto3-workmail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workmail.svg?color=blue)](https://pypi.org/project/mypy-boto3-workmail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workmail?color=blue)](https://pypistats.org/packages/mypy-boto3-workmail)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workmail)](https://pepy.tech/project/mypy-boto3-workmail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkMail 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
+[boto3.WorkMail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
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
 [mypy-boto3-workmail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -370,166 +370,171 @@
 
 ```python
 from mypy_boto3_workmail.type_defs import (
     AccessControlRuleTypeDef,
     AssociateDelegateToResourceRequestRequestTypeDef,
     AssociateMemberToGroupRequestRequestTypeDef,
     AssumeImpersonationRoleRequestRequestTypeDef,
-    AssumeImpersonationRoleResponseTypeDef,
-    LambdaAvailabilityProviderTypeDef,
+    ResponseMetadataTypeDef,
+    LambdaAvailabilityProviderOutputTypeDef,
     RedactedEwsAvailabilityProviderTypeDef,
+    BookingOptionsOutputTypeDef,
     BookingOptionsTypeDef,
     CancelMailboxExportJobRequestRequestTypeDef,
     CreateAliasRequestRequestTypeDef,
     EwsAvailabilityProviderTypeDef,
+    LambdaAvailabilityProviderTypeDef,
     CreateGroupRequestRequestTypeDef,
-    CreateGroupResponseTypeDef,
     ImpersonationRuleTypeDef,
-    CreateImpersonationRoleResponseTypeDef,
     CreateMobileDeviceAccessRuleRequestRequestTypeDef,
-    CreateMobileDeviceAccessRuleResponseTypeDef,
     DomainTypeDef,
-    CreateOrganizationResponseTypeDef,
     CreateResourceRequestRequestTypeDef,
-    CreateResourceResponseTypeDef,
     CreateUserRequestRequestTypeDef,
-    CreateUserResponseTypeDef,
     DelegateTypeDef,
     DeleteAccessControlRuleRequestRequestTypeDef,
     DeleteAliasRequestRequestTypeDef,
     DeleteAvailabilityConfigurationRequestRequestTypeDef,
     DeleteEmailMonitoringConfigurationRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteImpersonationRoleRequestRequestTypeDef,
     DeleteMailboxPermissionsRequestRequestTypeDef,
     DeleteMobileDeviceAccessOverrideRequestRequestTypeDef,
     DeleteMobileDeviceAccessRuleRequestRequestTypeDef,
     DeleteOrganizationRequestRequestTypeDef,
-    DeleteOrganizationResponseTypeDef,
     DeleteResourceRequestRequestTypeDef,
     DeleteRetentionPolicyRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeregisterFromWorkMailRequestRequestTypeDef,
     DeregisterMailDomainRequestRequestTypeDef,
     DescribeEmailMonitoringConfigurationRequestRequestTypeDef,
-    DescribeEmailMonitoringConfigurationResponseTypeDef,
     DescribeGroupRequestRequestTypeDef,
-    DescribeGroupResponseTypeDef,
     DescribeInboundDmarcSettingsRequestRequestTypeDef,
-    DescribeInboundDmarcSettingsResponseTypeDef,
     DescribeMailboxExportJobRequestRequestTypeDef,
-    DescribeMailboxExportJobResponseTypeDef,
     DescribeOrganizationRequestRequestTypeDef,
-    DescribeOrganizationResponseTypeDef,
     DescribeResourceRequestRequestTypeDef,
     DescribeUserRequestRequestTypeDef,
-    DescribeUserResponseTypeDef,
     DisassociateDelegateFromResourceRequestRequestTypeDef,
     DisassociateMemberFromGroupRequestRequestTypeDef,
     DnsRecordTypeDef,
+    FolderConfigurationOutputTypeDef,
     FolderConfigurationTypeDef,
     GetAccessControlEffectRequestRequestTypeDef,
-    GetAccessControlEffectResponseTypeDef,
     GetDefaultRetentionPolicyRequestRequestTypeDef,
     GetImpersonationRoleEffectRequestRequestTypeDef,
     ImpersonationMatchedRuleTypeDef,
     GetImpersonationRoleRequestRequestTypeDef,
+    ImpersonationRuleOutputTypeDef,
     GetMailDomainRequestRequestTypeDef,
     GetMailboxDetailsRequestRequestTypeDef,
-    GetMailboxDetailsResponseTypeDef,
     GetMobileDeviceAccessEffectRequestRequestTypeDef,
     MobileDeviceAccessMatchedRuleTypeDef,
     GetMobileDeviceAccessOverrideRequestRequestTypeDef,
-    GetMobileDeviceAccessOverrideResponseTypeDef,
     GroupTypeDef,
     ImpersonationRoleTypeDef,
     ListAccessControlRulesRequestRequestTypeDef,
-    ListAliasesRequestListAliasesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAliasesRequestRequestTypeDef,
-    ListAliasesResponseTypeDef,
-    ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
     ListAvailabilityConfigurationsRequestRequestTypeDef,
-    ListGroupMembersRequestListGroupMembersPaginateTypeDef,
     ListGroupMembersRequestRequestTypeDef,
     MemberTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListImpersonationRolesRequestRequestTypeDef,
     ListMailDomainsRequestRequestTypeDef,
     MailDomainSummaryTypeDef,
     ListMailboxExportJobsRequestRequestTypeDef,
     MailboxExportJobTypeDef,
-    ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
     ListMailboxPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
     ListMobileDeviceAccessOverridesRequestRequestTypeDef,
     MobileDeviceAccessOverrideTypeDef,
     ListMobileDeviceAccessRulesRequestRequestTypeDef,
     MobileDeviceAccessRuleTypeDef,
-    ListOrganizationsRequestListOrganizationsPaginateTypeDef,
     ListOrganizationsRequestRequestTypeDef,
     OrganizationSummaryTypeDef,
-    ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
     ListResourceDelegatesRequestRequestTypeDef,
-    ListResourcesRequestListResourcesPaginateTypeDef,
     ListResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
+    TagOutputTypeDef,
     ListUsersRequestRequestTypeDef,
     UserTypeDef,
-    PaginatorConfigTypeDef,
     PutAccessControlRuleRequestRequestTypeDef,
     PutEmailMonitoringConfigurationRequestRequestTypeDef,
     PutInboundDmarcSettingsRequestRequestTypeDef,
     PutMailboxPermissionsRequestRequestTypeDef,
     PutMobileDeviceAccessOverrideRequestRequestTypeDef,
     RegisterMailDomainRequestRequestTypeDef,
     RegisterToWorkMailRequestRequestTypeDef,
     ResetPasswordRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartMailboxExportJobRequestRequestTypeDef,
-    StartMailboxExportJobResponseTypeDef,
-    TestAvailabilityConfigurationResponseTypeDef,
+    TagTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDefaultMailDomainRequestRequestTypeDef,
     UpdateMailboxQuotaRequestRequestTypeDef,
     UpdateMobileDeviceAccessRuleRequestRequestTypeDef,
     UpdatePrimaryEmailAddressRequestRequestTypeDef,
+    AssumeImpersonationRoleResponseTypeDef,
+    CreateGroupResponseTypeDef,
+    CreateImpersonationRoleResponseTypeDef,
+    CreateMobileDeviceAccessRuleResponseTypeDef,
+    CreateOrganizationResponseTypeDef,
+    CreateResourceResponseTypeDef,
+    CreateUserResponseTypeDef,
+    DeleteOrganizationResponseTypeDef,
+    DescribeEmailMonitoringConfigurationResponseTypeDef,
+    DescribeGroupResponseTypeDef,
+    DescribeInboundDmarcSettingsResponseTypeDef,
+    DescribeMailboxExportJobResponseTypeDef,
+    DescribeOrganizationResponseTypeDef,
+    DescribeUserResponseTypeDef,
+    GetAccessControlEffectResponseTypeDef,
+    GetMailboxDetailsResponseTypeDef,
+    GetMobileDeviceAccessOverrideResponseTypeDef,
     ListAccessControlRulesResponseTypeDef,
+    ListAliasesResponseTypeDef,
+    StartMailboxExportJobResponseTypeDef,
+    TestAvailabilityConfigurationResponseTypeDef,
     AvailabilityConfigurationTypeDef,
     DescribeResourceResponseTypeDef,
     UpdateResourceRequestRequestTypeDef,
     CreateAvailabilityConfigurationRequestRequestTypeDef,
     TestAvailabilityConfigurationRequestRequestTypeDef,
     UpdateAvailabilityConfigurationRequestRequestTypeDef,
     CreateImpersonationRoleRequestRequestTypeDef,
-    GetImpersonationRoleResponseTypeDef,
     UpdateImpersonationRoleRequestRequestTypeDef,
     CreateOrganizationRequestRequestTypeDef,
     ListResourceDelegatesResponseTypeDef,
     GetMailDomainResponseTypeDef,
     GetDefaultRetentionPolicyResponseTypeDef,
     PutRetentionPolicyRequestRequestTypeDef,
     GetImpersonationRoleEffectResponseTypeDef,
+    GetImpersonationRoleResponseTypeDef,
     GetMobileDeviceAccessEffectResponseTypeDef,
     ListGroupsResponseTypeDef,
     ListImpersonationRolesResponseTypeDef,
+    ListAliasesRequestListAliasesPaginateTypeDef,
+    ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
+    ListGroupMembersRequestListGroupMembersPaginateTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
+    ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
+    ListOrganizationsRequestListOrganizationsPaginateTypeDef,
+    ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
+    ListResourcesRequestListResourcesPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     ListGroupMembersResponseTypeDef,
     ListMailDomainsResponseTypeDef,
     ListMailboxExportJobsResponseTypeDef,
     ListMailboxPermissionsResponseTypeDef,
     ListMobileDeviceAccessOverridesResponseTypeDef,
     ListMobileDeviceAccessRulesResponseTypeDef,
     ListOrganizationsResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     ListUsersResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ListAvailabilityConfigurationsResponseTypeDef,
 )
 
 
 def get_structure() -> AccessControlRuleTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-workmail-1.28.0/mypy_boto3_workmail.egg-info/SOURCES.txt` & `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.0/setup.py` & `mypy-boto3-workmail-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-workmail",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_workmail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WorkMail 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.WorkMail 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

