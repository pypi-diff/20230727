# Comparing `tmp/mypy-boto3-fms-1.28.0.tar.gz` & `tmp/mypy-boto3-fms-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-fms-1.28.0.tar", last modified: Thu Jul  6 20:59:37 2023, max compression
+gzip compressed data, was "mypy-boto3-fms-1.28.12.tar", last modified: Thu Jul 27 05:34:42 2023, max compression
```

## Comparing `mypy-boto3-fms-1.28.0.tar` & `mypy-boto3-fms-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:37.006307 mypy-boto3-fms-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:41:09.000000 mypy-boto3-fms-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20839 2023-07-06 20:59:37.006307 mypy-boto3-fms-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19370 2023-07-06 20:41:09.000000 mypy-boto3-fms-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:36.986307 mypy-boto3-fms-1.28.0/mypy_boto3_fms/
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-06 20:41:09.000000 mypy-boto3-fms-1.28.0/mypy_boto3_fms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-06 20:41:09.000000 mypy-boto3-fms-1.28.0/mypy_boto3_fms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:41:09.000000 mypy-boto3-fms-1.28.0/mypy_boto3_fms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30820 2023-07-06 20:41:09.000000 mypy-boto3-fms-1.28.0/mypy_boto3_fms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30763 2023-07-06 20:41:09.000000 mypy-boto3-fms-1.28.0/mypy_boto3_fms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12996 2023-07-06 20:41:10.000000 mypy-boto3-fms-1.28.0/mypy_boto3_fms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12994 2023-07-06 20:41:09.000000 mypy-boto3-fms-1.28.0/mypy_boto3_fms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-07-06 20:41:09.000000 mypy-boto3-fms-1.28.0/mypy_boto3_fms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-07-06 20:41:09.000000 mypy-boto3-fms-1.28.0/mypy_boto3_fms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:41:09.000000 mypy-boto3-fms-1.28.0/mypy_boto3_fms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59433 2023-07-06 20:41:13.000000 mypy-boto3-fms-1.28.0/mypy_boto3_fms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59366 2023-07-06 20:41:12.000000 mypy-boto3-fms-1.28.0/mypy_boto3_fms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:41:09.000000 mypy-boto3-fms-1.28.0/mypy_boto3_fms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:37.006307 mypy-boto3-fms-1.28.0/mypy_boto3_fms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20839 2023-07-06 20:59:36.000000 mypy-boto3-fms-1.28.0/mypy_boto3_fms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 20:59:36.000000 mypy-boto3-fms-1.28.0/mypy_boto3_fms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:36.000000 mypy-boto3-fms-1.28.0/mypy_boto3_fms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:36.000000 mypy-boto3-fms-1.28.0/mypy_boto3_fms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:36.000000 mypy-boto3-fms-1.28.0/mypy_boto3_fms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:36.000000 mypy-boto3-fms-1.28.0/mypy_boto3_fms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:37.006307 mypy-boto3-fms-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:41:09.000000 mypy-boto3-fms-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.476507 mypy-boto3-fms-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-07-27 05:34:42.476507 mypy-boto3-fms-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19881 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.476507 mypy-boto3-fms-1.28.12/mypy_boto3_fms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30820 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30763 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-07-27 05:22:22.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-07-27 05:22:22.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    65998 2023-07-27 05:22:23.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65919 2023-07-27 05:22:22.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.476507 mypy-boto3-fms-1.28.12/mypy_boto3_fms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-07-27 05:34:42.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 05:34:42.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:42.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:42.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:42.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:42.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:42.476507 mypy-boto3-fms-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/setup.py
```

### Comparing `mypy-boto3-fms-1.28.0/LICENSE` & `mypy-boto3-fms-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.0/PKG-INFO` & `mypy-boto3-fms-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fms
-Version: 1.28.0
-Summary: Type annotations for boto3.FMS 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.FMS 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-fms"></a>
 
 # mypy-boto3-fms
 
 [![PyPI - mypy-boto3-fms](https://img.shields.io/pypi/v/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fms?color=blue)](https://pypistats.org/packages/mypy-boto3-fms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-fms)](https://pepy.tech/project/mypy-boto3-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FMS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[boto3.FMS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
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
 [mypy-boto3-fms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,20 +371,25 @@
 ### Typed dictionaries
 
 `mypy_boto3_fms.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_fms.type_defs import (
+    AccountScopeOutputTypeDef,
     AccountScopeTypeDef,
     ActionTargetTypeDef,
     AdminAccountSummaryTypeDef,
+    OrganizationalUnitScopeOutputTypeDef,
+    PolicyTypeScopeOutputTypeDef,
+    RegionScopeOutputTypeDef,
     OrganizationalUnitScopeTypeDef,
     PolicyTypeScopeTypeDef,
     RegionScopeTypeDef,
+    AppOutputTypeDef,
     AppTypeDef,
     AssociateAdminAccountRequestRequestTypeDef,
     AssociateThirdPartyFirewallRequestRequestTypeDef,
     AssociateThirdPartyFirewallResponseTypeDef,
     AwsEc2NetworkInterfaceViolationTypeDef,
     PartialMatchTypeDef,
     BatchAssociateResourceRequestRequestTypeDef,
@@ -412,17 +417,17 @@
     GetAppsListRequestRequestTypeDef,
     GetComplianceDetailRequestRequestTypeDef,
     GetNotificationChannelResponseTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetProtectionStatusRequestRequestTypeDef,
     GetProtectionStatusResponseTypeDef,
     GetProtocolsListRequestRequestTypeDef,
-    ProtocolsListDataTypeDef,
+    ProtocolsListDataOutputTypeDef,
     GetResourceSetRequestRequestTypeDef,
-    ResourceSetTypeDef,
+    ResourceSetOutputTypeDef,
     GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef,
     GetThirdPartyFirewallAssociationStatusResponseTypeDef,
     GetViolationDetailsRequestRequestTypeDef,
     ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef,
     ListAdminAccountsForOrganizationRequestRequestTypeDef,
     ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef,
     ListAdminsManagingAccountRequestRequestTypeDef,
@@ -442,45 +447,53 @@
     ListProtocolsListsRequestRequestTypeDef,
     ProtocolsListDataSummaryTypeDef,
     ListResourceSetResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListResourceSetsRequestRequestTypeDef,
     ResourceSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
     ThirdPartyFirewallFirewallPolicyTypeDef,
     RouteTypeDef,
     NetworkFirewallMissingExpectedRTViolationTypeDef,
     NetworkFirewallMissingFirewallViolationTypeDef,
     NetworkFirewallMissingSubnetViolationTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupTypeDef,
+    NetworkFirewallPolicyOutputTypeDef,
     NetworkFirewallPolicyTypeDef,
     NetworkFirewallStatefulRuleGroupOverrideTypeDef,
     PaginatorConfigTypeDef,
+    ThirdPartyFirewallPolicyOutputTypeDef,
     ThirdPartyFirewallPolicyTypeDef,
+    ResourceTagOutputTypeDef,
     ResourceTagTypeDef,
+    ProtocolsListDataTypeDef,
+    TagTypeDef,
     PutNotificationChannelRequestRequestTypeDef,
+    ResourceSetTypeDef,
     ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef,
     ThirdPartyFirewallMissingFirewallViolationTypeDef,
     ThirdPartyFirewallMissingSubnetViolationTypeDef,
     ResponseMetadataTypeDef,
     SecurityGroupRuleDescriptionTypeDef,
     UntagResourceRequestRequestTypeDef,
     EC2AssociateRouteTableActionTypeDef,
     EC2CopyRouteTableActionTypeDef,
     EC2CreateRouteActionTypeDef,
     EC2CreateRouteTableActionTypeDef,
     EC2DeleteRouteActionTypeDef,
     EC2ReplaceRouteActionTypeDef,
     EC2ReplaceRouteTableAssociationActionTypeDef,
     ListAdminAccountsForOrganizationResponseTypeDef,
+    AdminScopeOutputTypeDef,
     AdminScopeTypeDef,
+    AppsListDataOutputTypeDef,
     AppsListDataSummaryTypeDef,
     AppsListDataTypeDef,
     AwsEc2InstanceViolationTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     PolicyComplianceDetailTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
@@ -491,54 +504,57 @@
     GetResourceSetResponseTypeDef,
     PutResourceSetResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PutProtocolsListRequestRequestTypeDef,
-    PutResourceSetRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
     NetworkFirewallBlackHoleRouteDetectedViolationTypeDef,
     NetworkFirewallInternetTrafficNotInspectedViolationTypeDef,
     NetworkFirewallInvalidRouteConfigurationViolationTypeDef,
     NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef,
     NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef,
     RouteHasOutOfScopeEndpointViolationTypeDef,
     StatefulRuleGroupTypeDef,
+    PolicyOptionOutputTypeDef,
     PolicyOptionTypeDef,
+    PutProtocolsListRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    PutResourceSetRequestRequestTypeDef,
     SecurityGroupRemediationActionTypeDef,
     RemediationActionTypeDef,
     GetAdminScopeResponseTypeDef,
     PutAdminAccountRequestRequestTypeDef,
-    ListAppsListsResponseTypeDef,
     GetAppsListResponseTypeDef,
-    PutAppsListRequestRequestTypeDef,
     PutAppsListResponseTypeDef,
+    ListAppsListsResponseTypeDef,
+    PutAppsListRequestRequestTypeDef,
     GetComplianceDetailResponseTypeDef,
     ListComplianceStatusResponseTypeDef,
     NetworkFirewallPolicyDescriptionTypeDef,
+    SecurityServicePolicyDataOutputTypeDef,
     SecurityServicePolicyDataTypeDef,
     AwsVPCSecurityGroupViolationTypeDef,
     RemediationActionWithOrderTypeDef,
     NetworkFirewallPolicyModifiedViolationTypeDef,
+    PolicyOutputTypeDef,
     PolicyTypeDef,
     PossibleRemediationActionTypeDef,
     GetPolicyResponseTypeDef,
-    PutPolicyRequestRequestTypeDef,
     PutPolicyResponseTypeDef,
+    PutPolicyRequestRequestTypeDef,
     PossibleRemediationActionsTypeDef,
     ResourceViolationTypeDef,
     ViolationDetailTypeDef,
     GetViolationDetailsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountScopeTypeDef:
+def get_structure() -> AccountScopeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-fms-1.28.0/README.md` & `mypy-boto3-fms-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-fms"></a>
 
 # mypy-boto3-fms
 
 [![PyPI - mypy-boto3-fms](https://img.shields.io/pypi/v/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fms?color=blue)](https://pypistats.org/packages/mypy-boto3-fms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-fms)](https://pepy.tech/project/mypy-boto3-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FMS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[boto3.FMS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
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
 [mypy-boto3-fms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,20 +339,25 @@
 ### Typed dictionaries
 
 `mypy_boto3_fms.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_fms.type_defs import (
+    AccountScopeOutputTypeDef,
     AccountScopeTypeDef,
     ActionTargetTypeDef,
     AdminAccountSummaryTypeDef,
+    OrganizationalUnitScopeOutputTypeDef,
+    PolicyTypeScopeOutputTypeDef,
+    RegionScopeOutputTypeDef,
     OrganizationalUnitScopeTypeDef,
     PolicyTypeScopeTypeDef,
     RegionScopeTypeDef,
+    AppOutputTypeDef,
     AppTypeDef,
     AssociateAdminAccountRequestRequestTypeDef,
     AssociateThirdPartyFirewallRequestRequestTypeDef,
     AssociateThirdPartyFirewallResponseTypeDef,
     AwsEc2NetworkInterfaceViolationTypeDef,
     PartialMatchTypeDef,
     BatchAssociateResourceRequestRequestTypeDef,
@@ -380,17 +385,17 @@
     GetAppsListRequestRequestTypeDef,
     GetComplianceDetailRequestRequestTypeDef,
     GetNotificationChannelResponseTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetProtectionStatusRequestRequestTypeDef,
     GetProtectionStatusResponseTypeDef,
     GetProtocolsListRequestRequestTypeDef,
-    ProtocolsListDataTypeDef,
+    ProtocolsListDataOutputTypeDef,
     GetResourceSetRequestRequestTypeDef,
-    ResourceSetTypeDef,
+    ResourceSetOutputTypeDef,
     GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef,
     GetThirdPartyFirewallAssociationStatusResponseTypeDef,
     GetViolationDetailsRequestRequestTypeDef,
     ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef,
     ListAdminAccountsForOrganizationRequestRequestTypeDef,
     ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef,
     ListAdminsManagingAccountRequestRequestTypeDef,
@@ -410,45 +415,53 @@
     ListProtocolsListsRequestRequestTypeDef,
     ProtocolsListDataSummaryTypeDef,
     ListResourceSetResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListResourceSetsRequestRequestTypeDef,
     ResourceSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
     ThirdPartyFirewallFirewallPolicyTypeDef,
     RouteTypeDef,
     NetworkFirewallMissingExpectedRTViolationTypeDef,
     NetworkFirewallMissingFirewallViolationTypeDef,
     NetworkFirewallMissingSubnetViolationTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupTypeDef,
+    NetworkFirewallPolicyOutputTypeDef,
     NetworkFirewallPolicyTypeDef,
     NetworkFirewallStatefulRuleGroupOverrideTypeDef,
     PaginatorConfigTypeDef,
+    ThirdPartyFirewallPolicyOutputTypeDef,
     ThirdPartyFirewallPolicyTypeDef,
+    ResourceTagOutputTypeDef,
     ResourceTagTypeDef,
+    ProtocolsListDataTypeDef,
+    TagTypeDef,
     PutNotificationChannelRequestRequestTypeDef,
+    ResourceSetTypeDef,
     ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef,
     ThirdPartyFirewallMissingFirewallViolationTypeDef,
     ThirdPartyFirewallMissingSubnetViolationTypeDef,
     ResponseMetadataTypeDef,
     SecurityGroupRuleDescriptionTypeDef,
     UntagResourceRequestRequestTypeDef,
     EC2AssociateRouteTableActionTypeDef,
     EC2CopyRouteTableActionTypeDef,
     EC2CreateRouteActionTypeDef,
     EC2CreateRouteTableActionTypeDef,
     EC2DeleteRouteActionTypeDef,
     EC2ReplaceRouteActionTypeDef,
     EC2ReplaceRouteTableAssociationActionTypeDef,
     ListAdminAccountsForOrganizationResponseTypeDef,
+    AdminScopeOutputTypeDef,
     AdminScopeTypeDef,
+    AppsListDataOutputTypeDef,
     AppsListDataSummaryTypeDef,
     AppsListDataTypeDef,
     AwsEc2InstanceViolationTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     PolicyComplianceDetailTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
@@ -459,54 +472,57 @@
     GetResourceSetResponseTypeDef,
     PutResourceSetResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PutProtocolsListRequestRequestTypeDef,
-    PutResourceSetRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
     NetworkFirewallBlackHoleRouteDetectedViolationTypeDef,
     NetworkFirewallInternetTrafficNotInspectedViolationTypeDef,
     NetworkFirewallInvalidRouteConfigurationViolationTypeDef,
     NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef,
     NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef,
     RouteHasOutOfScopeEndpointViolationTypeDef,
     StatefulRuleGroupTypeDef,
+    PolicyOptionOutputTypeDef,
     PolicyOptionTypeDef,
+    PutProtocolsListRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    PutResourceSetRequestRequestTypeDef,
     SecurityGroupRemediationActionTypeDef,
     RemediationActionTypeDef,
     GetAdminScopeResponseTypeDef,
     PutAdminAccountRequestRequestTypeDef,
-    ListAppsListsResponseTypeDef,
     GetAppsListResponseTypeDef,
-    PutAppsListRequestRequestTypeDef,
     PutAppsListResponseTypeDef,
+    ListAppsListsResponseTypeDef,
+    PutAppsListRequestRequestTypeDef,
     GetComplianceDetailResponseTypeDef,
     ListComplianceStatusResponseTypeDef,
     NetworkFirewallPolicyDescriptionTypeDef,
+    SecurityServicePolicyDataOutputTypeDef,
     SecurityServicePolicyDataTypeDef,
     AwsVPCSecurityGroupViolationTypeDef,
     RemediationActionWithOrderTypeDef,
     NetworkFirewallPolicyModifiedViolationTypeDef,
+    PolicyOutputTypeDef,
     PolicyTypeDef,
     PossibleRemediationActionTypeDef,
     GetPolicyResponseTypeDef,
-    PutPolicyRequestRequestTypeDef,
     PutPolicyResponseTypeDef,
+    PutPolicyRequestRequestTypeDef,
     PossibleRemediationActionsTypeDef,
     ResourceViolationTypeDef,
     ViolationDetailTypeDef,
     GetViolationDetailsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountScopeTypeDef:
+def get_structure() -> AccountScopeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-fms-1.28.0/mypy_boto3_fms/__init__.py` & `mypy-boto3-fms-1.28.12/mypy_boto3_fms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.0/mypy_boto3_fms/__init__.pyi` & `mypy-boto3-fms-1.28.12/mypy_boto3_fms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.0/mypy_boto3_fms/__main__.py` & `mypy-boto3-fms-1.28.12/mypy_boto3_fms/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FMS 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.FMS 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS\nOther"
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

### Comparing `mypy-boto3-fms-1.28.0/mypy_boto3_fms/client.py` & `mypy-boto3-fms-1.28.12/mypy_boto3_fms/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.0/mypy_boto3_fms/client.pyi` & `mypy-boto3-fms-1.28.12/mypy_boto3_fms/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.0/mypy_boto3_fms/literals.py` & `mypy-boto3-fms-1.28.12/mypy_boto3_fms/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,14 +262,15 @@
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
@@ -348,26 +349,28 @@
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

### Comparing `mypy-boto3-fms-1.28.0/mypy_boto3_fms/literals.pyi` & `mypy-boto3-fms-1.28.12/mypy_boto3_fms/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -260,14 +260,15 @@
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
@@ -346,26 +347,28 @@
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

### Comparing `mypy-boto3-fms-1.28.0/mypy_boto3_fms/paginator.py` & `mypy-boto3-fms-1.28.12/mypy_boto3_fms/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.0/mypy_boto3_fms/paginator.pyi` & `mypy-boto3-fms-1.28.12/mypy_boto3_fms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.0/mypy_boto3_fms/type_defs.py` & `mypy-boto3-fms-1.28.12/mypy_boto3_fms/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for fms service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_fms.type_defs import AccountScopeTypeDef
+    from mypy_boto3_fms.type_defs import AccountScopeOutputTypeDef
 
-    data: AccountScopeTypeDef = {...}
+    data: AccountScopeOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccountRoleStatusType,
     CustomerPolicyScopeIdTypeType,
     CustomerPolicyStatusType,
     DependentServiceNameType,
     DestinationTypeType,
@@ -41,22 +41,26 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "AccountScopeOutputTypeDef",
     "AccountScopeTypeDef",
     "ActionTargetTypeDef",
     "AdminAccountSummaryTypeDef",
+    "OrganizationalUnitScopeOutputTypeDef",
+    "PolicyTypeScopeOutputTypeDef",
+    "RegionScopeOutputTypeDef",
     "OrganizationalUnitScopeTypeDef",
     "PolicyTypeScopeTypeDef",
     "RegionScopeTypeDef",
+    "AppOutputTypeDef",
     "AppTypeDef",
     "AssociateAdminAccountRequestRequestTypeDef",
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
     "AssociateThirdPartyFirewallResponseTypeDef",
     "AwsEc2NetworkInterfaceViolationTypeDef",
     "PartialMatchTypeDef",
     "BatchAssociateResourceRequestRequestTypeDef",
@@ -84,17 +88,17 @@
     "GetAppsListRequestRequestTypeDef",
     "GetComplianceDetailRequestRequestTypeDef",
     "GetNotificationChannelResponseTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "GetProtectionStatusRequestRequestTypeDef",
     "GetProtectionStatusResponseTypeDef",
     "GetProtocolsListRequestRequestTypeDef",
-    "ProtocolsListDataTypeDef",
+    "ProtocolsListDataOutputTypeDef",
     "GetResourceSetRequestRequestTypeDef",
-    "ResourceSetTypeDef",
+    "ResourceSetOutputTypeDef",
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
     "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
     "GetViolationDetailsRequestRequestTypeDef",
     "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
     "ListAdminAccountsForOrganizationRequestRequestTypeDef",
     "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
     "ListAdminsManagingAccountRequestRequestTypeDef",
@@ -114,45 +118,53 @@
     "ListProtocolsListsRequestRequestTypeDef",
     "ProtocolsListDataSummaryTypeDef",
     "ListResourceSetResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
     "ListResourceSetsRequestRequestTypeDef",
     "ResourceSetSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     "ThirdPartyFirewallFirewallPolicyTypeDef",
     "RouteTypeDef",
     "NetworkFirewallMissingExpectedRTViolationTypeDef",
     "NetworkFirewallMissingFirewallViolationTypeDef",
     "NetworkFirewallMissingSubnetViolationTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupTypeDef",
+    "NetworkFirewallPolicyOutputTypeDef",
     "NetworkFirewallPolicyTypeDef",
     "NetworkFirewallStatefulRuleGroupOverrideTypeDef",
     "PaginatorConfigTypeDef",
+    "ThirdPartyFirewallPolicyOutputTypeDef",
     "ThirdPartyFirewallPolicyTypeDef",
+    "ResourceTagOutputTypeDef",
     "ResourceTagTypeDef",
+    "ProtocolsListDataTypeDef",
+    "TagTypeDef",
     "PutNotificationChannelRequestRequestTypeDef",
+    "ResourceSetTypeDef",
     "ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef",
     "ThirdPartyFirewallMissingFirewallViolationTypeDef",
     "ThirdPartyFirewallMissingSubnetViolationTypeDef",
     "ResponseMetadataTypeDef",
     "SecurityGroupRuleDescriptionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "EC2AssociateRouteTableActionTypeDef",
     "EC2CopyRouteTableActionTypeDef",
     "EC2CreateRouteActionTypeDef",
     "EC2CreateRouteTableActionTypeDef",
     "EC2DeleteRouteActionTypeDef",
     "EC2ReplaceRouteActionTypeDef",
     "EC2ReplaceRouteTableAssociationActionTypeDef",
     "ListAdminAccountsForOrganizationResponseTypeDef",
+    "AdminScopeOutputTypeDef",
     "AdminScopeTypeDef",
+    "AppsListDataOutputTypeDef",
     "AppsListDataSummaryTypeDef",
     "AppsListDataTypeDef",
     "AwsEc2InstanceViolationTypeDef",
     "BatchAssociateResourceResponseTypeDef",
     "BatchDisassociateResourceResponseTypeDef",
     "PolicyComplianceDetailTypeDef",
     "ListDiscoveredResourcesResponseTypeDef",
@@ -163,56 +175,69 @@
     "GetResourceSetResponseTypeDef",
     "PutResourceSetResponseTypeDef",
     "ListPoliciesResponseTypeDef",
     "ListProtocolsListsResponseTypeDef",
     "ListResourceSetResourcesResponseTypeDef",
     "ListResourceSetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "PutProtocolsListRequestRequestTypeDef",
-    "PutResourceSetRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesResponseTypeDef",
     "NetworkFirewallBlackHoleRouteDetectedViolationTypeDef",
     "NetworkFirewallInternetTrafficNotInspectedViolationTypeDef",
     "NetworkFirewallInvalidRouteConfigurationViolationTypeDef",
     "NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef",
     "NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef",
     "RouteHasOutOfScopeEndpointViolationTypeDef",
     "StatefulRuleGroupTypeDef",
+    "PolicyOptionOutputTypeDef",
     "PolicyOptionTypeDef",
+    "PutProtocolsListRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "PutResourceSetRequestRequestTypeDef",
     "SecurityGroupRemediationActionTypeDef",
     "RemediationActionTypeDef",
     "GetAdminScopeResponseTypeDef",
     "PutAdminAccountRequestRequestTypeDef",
-    "ListAppsListsResponseTypeDef",
     "GetAppsListResponseTypeDef",
-    "PutAppsListRequestRequestTypeDef",
     "PutAppsListResponseTypeDef",
+    "ListAppsListsResponseTypeDef",
+    "PutAppsListRequestRequestTypeDef",
     "GetComplianceDetailResponseTypeDef",
     "ListComplianceStatusResponseTypeDef",
     "NetworkFirewallPolicyDescriptionTypeDef",
+    "SecurityServicePolicyDataOutputTypeDef",
     "SecurityServicePolicyDataTypeDef",
     "AwsVPCSecurityGroupViolationTypeDef",
     "RemediationActionWithOrderTypeDef",
     "NetworkFirewallPolicyModifiedViolationTypeDef",
+    "PolicyOutputTypeDef",
     "PolicyTypeDef",
     "PossibleRemediationActionTypeDef",
     "GetPolicyResponseTypeDef",
-    "PutPolicyRequestRequestTypeDef",
     "PutPolicyResponseTypeDef",
+    "PutPolicyRequestRequestTypeDef",
     "PossibleRemediationActionsTypeDef",
     "ResourceViolationTypeDef",
     "ViolationDetailTypeDef",
     "GetViolationDetailsResponseTypeDef",
 )
 
+AccountScopeOutputTypeDef = TypedDict(
+    "AccountScopeOutputTypeDef",
+    {
+        "Accounts": List[str],
+        "AllAccountsEnabled": bool,
+        "ExcludeSpecifiedAccounts": bool,
+    },
+    total=False,
+)
+
 AccountScopeTypeDef = TypedDict(
     "AccountScopeTypeDef",
     {
-        "Accounts": List[str],
+        "Accounts": Sequence[str],
         "AllAccountsEnabled": bool,
         "ExcludeSpecifiedAccounts": bool,
     },
     total=False,
 )
 
 ActionTargetTypeDef = TypedDict(
@@ -230,42 +255,79 @@
         "AdminAccount": str,
         "DefaultAdmin": bool,
         "Status": OrganizationStatusType,
     },
     total=False,
 )
 
+OrganizationalUnitScopeOutputTypeDef = TypedDict(
+    "OrganizationalUnitScopeOutputTypeDef",
+    {
+        "OrganizationalUnits": List[str],
+        "AllOrganizationalUnitsEnabled": bool,
+        "ExcludeSpecifiedOrganizationalUnits": bool,
+    },
+    total=False,
+)
+
+PolicyTypeScopeOutputTypeDef = TypedDict(
+    "PolicyTypeScopeOutputTypeDef",
+    {
+        "PolicyTypes": List[SecurityServiceTypeType],
+        "AllPolicyTypesEnabled": bool,
+    },
+    total=False,
+)
+
+RegionScopeOutputTypeDef = TypedDict(
+    "RegionScopeOutputTypeDef",
+    {
+        "Regions": List[str],
+        "AllRegionsEnabled": bool,
+    },
+    total=False,
+)
+
 OrganizationalUnitScopeTypeDef = TypedDict(
     "OrganizationalUnitScopeTypeDef",
     {
-        "OrganizationalUnits": List[str],
+        "OrganizationalUnits": Sequence[str],
         "AllOrganizationalUnitsEnabled": bool,
         "ExcludeSpecifiedOrganizationalUnits": bool,
     },
     total=False,
 )
 
 PolicyTypeScopeTypeDef = TypedDict(
     "PolicyTypeScopeTypeDef",
     {
-        "PolicyTypes": List[SecurityServiceTypeType],
+        "PolicyTypes": Sequence[SecurityServiceTypeType],
         "AllPolicyTypesEnabled": bool,
     },
     total=False,
 )
 
 RegionScopeTypeDef = TypedDict(
     "RegionScopeTypeDef",
     {
-        "Regions": List[str],
+        "Regions": Sequence[str],
         "AllRegionsEnabled": bool,
     },
     total=False,
 )
 
+AppOutputTypeDef = TypedDict(
+    "AppOutputTypeDef",
+    {
+        "AppName": str,
+        "Protocol": str,
+        "Port": int,
+    },
+)
+
 AppTypeDef = TypedDict(
     "AppTypeDef",
     {
         "AppName": str,
         "Protocol": str,
         "Port": int,
     },
@@ -364,21 +426,19 @@
     "_OptionalDeletePolicyRequestRequestTypeDef",
     {
         "DeleteAllPolicyResources": bool,
     },
     total=False,
 )
 
-
 class DeletePolicyRequestRequestTypeDef(
     _RequiredDeletePolicyRequestRequestTypeDef, _OptionalDeletePolicyRequestRequestTypeDef
 ):
     pass
 
-
 DeleteProtocolsListRequestRequestTypeDef = TypedDict(
     "DeleteProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
 
@@ -534,21 +594,19 @@
     "_OptionalGetAppsListRequestRequestTypeDef",
     {
         "DefaultList": bool,
     },
     total=False,
 )
 
-
 class GetAppsListRequestRequestTypeDef(
     _RequiredGetAppsListRequestRequestTypeDef, _OptionalGetAppsListRequestRequestTypeDef
 ):
     pass
 
-
 GetComplianceDetailRequestRequestTypeDef = TypedDict(
     "GetComplianceDetailRequestRequestTypeDef",
     {
         "PolicyId": str,
         "MemberAccount": str,
     },
 )
@@ -583,22 +641,20 @@
         "EndTime": Union[datetime, str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetProtectionStatusRequestRequestTypeDef(
     _RequiredGetProtectionStatusRequestRequestTypeDef,
     _OptionalGetProtectionStatusRequestRequestTypeDef,
 ):
     pass
 
-
 GetProtectionStatusResponseTypeDef = TypedDict(
     "GetProtectionStatusResponseTypeDef",
     {
         "AdminAccountId": str,
         "ServiceType": SecurityServiceTypeType,
         "Data": str,
         "NextToken": str,
@@ -616,78 +672,74 @@
     "_OptionalGetProtocolsListRequestRequestTypeDef",
     {
         "DefaultList": bool,
     },
     total=False,
 )
 
-
 class GetProtocolsListRequestRequestTypeDef(
     _RequiredGetProtocolsListRequestRequestTypeDef, _OptionalGetProtocolsListRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredProtocolsListDataTypeDef = TypedDict(
-    "_RequiredProtocolsListDataTypeDef",
+_RequiredProtocolsListDataOutputTypeDef = TypedDict(
+    "_RequiredProtocolsListDataOutputTypeDef",
     {
         "ListName": str,
         "ProtocolsList": List[str],
     },
 )
-_OptionalProtocolsListDataTypeDef = TypedDict(
-    "_OptionalProtocolsListDataTypeDef",
+_OptionalProtocolsListDataOutputTypeDef = TypedDict(
+    "_OptionalProtocolsListDataOutputTypeDef",
     {
         "ListId": str,
         "ListUpdateToken": str,
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "PreviousProtocolsList": Dict[str, List[str]],
     },
     total=False,
 )
 
-
-class ProtocolsListDataTypeDef(
-    _RequiredProtocolsListDataTypeDef, _OptionalProtocolsListDataTypeDef
+class ProtocolsListDataOutputTypeDef(
+    _RequiredProtocolsListDataOutputTypeDef, _OptionalProtocolsListDataOutputTypeDef
 ):
     pass
 
-
 GetResourceSetRequestRequestTypeDef = TypedDict(
     "GetResourceSetRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
-_RequiredResourceSetTypeDef = TypedDict(
-    "_RequiredResourceSetTypeDef",
+_RequiredResourceSetOutputTypeDef = TypedDict(
+    "_RequiredResourceSetOutputTypeDef",
     {
         "Name": str,
         "ResourceTypeList": List[str],
     },
 )
-_OptionalResourceSetTypeDef = TypedDict(
-    "_OptionalResourceSetTypeDef",
+_OptionalResourceSetOutputTypeDef = TypedDict(
+    "_OptionalResourceSetOutputTypeDef",
     {
         "Id": str,
         "Description": str,
         "UpdateToken": str,
         "LastUpdateTime": datetime,
         "ResourceSetStatus": ResourceSetStatusType,
     },
     total=False,
 )
 
-
-class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
+class ResourceSetOutputTypeDef(
+    _RequiredResourceSetOutputTypeDef, _OptionalResourceSetOutputTypeDef
+):
     pass
 
-
 GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef = TypedDict(
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
     },
 )
 
@@ -773,43 +825,39 @@
     {
         "DefaultLists": bool,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAppsListsRequestRequestTypeDef(
     _RequiredListAppsListsRequestRequestTypeDef, _OptionalListAppsListsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
     "_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
     {
         "PolicyId": str,
     },
 )
 _OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
     "_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListComplianceStatusRequestListComplianceStatusPaginateTypeDef(
     _RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
     _OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListComplianceStatusRequestRequestTypeDef = TypedDict(
     "_RequiredListComplianceStatusRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 _OptionalListComplianceStatusRequestRequestTypeDef = TypedDict(
@@ -817,22 +865,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListComplianceStatusRequestRequestTypeDef(
     _RequiredListComplianceStatusRequestRequestTypeDef,
     _OptionalListComplianceStatusRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDiscoveredResourcesRequestRequestTypeDef",
     {
         "MemberAccountIds": Sequence[str],
         "ResourceType": str,
     },
 )
@@ -841,22 +887,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
-
 ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
     "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -931,22 +975,20 @@
     {
         "DefaultLists": bool,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListProtocolsListsRequestRequestTypeDef(
     _RequiredListProtocolsListsRequestRequestTypeDef,
     _OptionalListProtocolsListsRequestRequestTypeDef,
 ):
     pass
 
-
 ProtocolsListDataSummaryTypeDef = TypedDict(
     "ProtocolsListDataSummaryTypeDef",
     {
         "ListArn": str,
         "ListId": str,
         "ListName": str,
         "ProtocolsList": List[str],
@@ -965,41 +1007,37 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListResourceSetResourcesRequestRequestTypeDef(
     _RequiredListResourceSetResourcesRequestRequestTypeDef,
     _OptionalListResourceSetResourcesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
         "URI": str,
     },
 )
 _OptionalResourceTypeDef = TypedDict(
     "_OptionalResourceTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
-
 class ResourceTypeDef(_RequiredResourceTypeDef, _OptionalResourceTypeDef):
     pass
 
-
 ListResourceSetsRequestRequestTypeDef = TypedDict(
     "ListResourceSetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1020,16 +1058,16 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 
 _RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
@@ -1042,22 +1080,20 @@
     "_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef(
     _RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     _OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
         "MaxResults": int,
     },
 )
@@ -1065,22 +1101,20 @@
     "_OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef(
     _RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
     _OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
 ):
     pass
 
-
 ThirdPartyFirewallFirewallPolicyTypeDef = TypedDict(
     "ThirdPartyFirewallFirewallPolicyTypeDef",
     {
         "FirewallPolicyId": str,
         "FirewallPolicyName": str,
     },
     total=False,
@@ -1145,14 +1179,22 @@
         "RuleGroupName": str,
         "ResourceId": str,
         "Priority": int,
     },
     total=False,
 )
 
+NetworkFirewallPolicyOutputTypeDef = TypedDict(
+    "NetworkFirewallPolicyOutputTypeDef",
+    {
+        "FirewallDeploymentModel": FirewallDeploymentModelType,
+    },
+    total=False,
+)
+
 NetworkFirewallPolicyTypeDef = TypedDict(
     "NetworkFirewallPolicyTypeDef",
     {
         "FirewallDeploymentModel": FirewallDeploymentModelType,
     },
     total=False,
 )
@@ -1171,49 +1213,128 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+ThirdPartyFirewallPolicyOutputTypeDef = TypedDict(
+    "ThirdPartyFirewallPolicyOutputTypeDef",
+    {
+        "FirewallDeploymentModel": FirewallDeploymentModelType,
+    },
+    total=False,
+)
+
 ThirdPartyFirewallPolicyTypeDef = TypedDict(
     "ThirdPartyFirewallPolicyTypeDef",
     {
         "FirewallDeploymentModel": FirewallDeploymentModelType,
     },
     total=False,
 )
 
+_RequiredResourceTagOutputTypeDef = TypedDict(
+    "_RequiredResourceTagOutputTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalResourceTagOutputTypeDef = TypedDict(
+    "_OptionalResourceTagOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+class ResourceTagOutputTypeDef(
+    _RequiredResourceTagOutputTypeDef, _OptionalResourceTagOutputTypeDef
+):
+    pass
+
 _RequiredResourceTagTypeDef = TypedDict(
     "_RequiredResourceTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalResourceTagTypeDef = TypedDict(
     "_OptionalResourceTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
     pass
 
+_RequiredProtocolsListDataTypeDef = TypedDict(
+    "_RequiredProtocolsListDataTypeDef",
+    {
+        "ListName": str,
+        "ProtocolsList": Sequence[str],
+    },
+)
+_OptionalProtocolsListDataTypeDef = TypedDict(
+    "_OptionalProtocolsListDataTypeDef",
+    {
+        "ListId": str,
+        "ListUpdateToken": str,
+        "CreateTime": Union[datetime, str],
+        "LastUpdateTime": Union[datetime, str],
+        "PreviousProtocolsList": Mapping[str, Sequence[str]],
+    },
+    total=False,
+)
+
+class ProtocolsListDataTypeDef(
+    _RequiredProtocolsListDataTypeDef, _OptionalProtocolsListDataTypeDef
+):
+    pass
+
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
 
 PutNotificationChannelRequestRequestTypeDef = TypedDict(
     "PutNotificationChannelRequestRequestTypeDef",
     {
         "SnsTopicArn": str,
         "SnsRoleName": str,
     },
 )
 
+_RequiredResourceSetTypeDef = TypedDict(
+    "_RequiredResourceSetTypeDef",
+    {
+        "Name": str,
+        "ResourceTypeList": Sequence[str],
+    },
+)
+_OptionalResourceSetTypeDef = TypedDict(
+    "_OptionalResourceSetTypeDef",
+    {
+        "Id": str,
+        "Description": str,
+        "UpdateToken": str,
+        "LastUpdateTime": Union[datetime, str],
+        "ResourceSetStatus": ResourceSetStatusType,
+    },
+    total=False,
+)
+
+class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
+    pass
+
 ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef = TypedDict(
     "ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef",
     {
         "ViolationTarget": str,
         "VPC": str,
         "AvailabilityZone": str,
         "CurrentRouteTable": str,
@@ -1288,21 +1409,19 @@
         "Description": str,
         "SubnetId": ActionTargetTypeDef,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
-
 class EC2AssociateRouteTableActionTypeDef(
     _RequiredEC2AssociateRouteTableActionTypeDef, _OptionalEC2AssociateRouteTableActionTypeDef
 ):
     pass
 
-
 _RequiredEC2CopyRouteTableActionTypeDef = TypedDict(
     "_RequiredEC2CopyRouteTableActionTypeDef",
     {
         "VpcId": ActionTargetTypeDef,
         "RouteTableId": ActionTargetTypeDef,
     },
 )
@@ -1310,21 +1429,19 @@
     "_OptionalEC2CopyRouteTableActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class EC2CopyRouteTableActionTypeDef(
     _RequiredEC2CopyRouteTableActionTypeDef, _OptionalEC2CopyRouteTableActionTypeDef
 ):
     pass
 
-
 _RequiredEC2CreateRouteActionTypeDef = TypedDict(
     "_RequiredEC2CreateRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2CreateRouteActionTypeDef = TypedDict(
@@ -1336,42 +1453,38 @@
         "DestinationIpv6CidrBlock": str,
         "VpcEndpointId": ActionTargetTypeDef,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
-
 class EC2CreateRouteActionTypeDef(
     _RequiredEC2CreateRouteActionTypeDef, _OptionalEC2CreateRouteActionTypeDef
 ):
     pass
 
-
 _RequiredEC2CreateRouteTableActionTypeDef = TypedDict(
     "_RequiredEC2CreateRouteTableActionTypeDef",
     {
         "VpcId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2CreateRouteTableActionTypeDef = TypedDict(
     "_OptionalEC2CreateRouteTableActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class EC2CreateRouteTableActionTypeDef(
     _RequiredEC2CreateRouteTableActionTypeDef, _OptionalEC2CreateRouteTableActionTypeDef
 ):
     pass
 
-
 _RequiredEC2DeleteRouteActionTypeDef = TypedDict(
     "_RequiredEC2DeleteRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2DeleteRouteActionTypeDef = TypedDict(
@@ -1381,21 +1494,19 @@
         "DestinationCidrBlock": str,
         "DestinationPrefixListId": str,
         "DestinationIpv6CidrBlock": str,
     },
     total=False,
 )
 
-
 class EC2DeleteRouteActionTypeDef(
     _RequiredEC2DeleteRouteActionTypeDef, _OptionalEC2DeleteRouteActionTypeDef
 ):
     pass
 
-
 _RequiredEC2ReplaceRouteActionTypeDef = TypedDict(
     "_RequiredEC2ReplaceRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2ReplaceRouteActionTypeDef = TypedDict(
@@ -1406,21 +1517,19 @@
         "DestinationPrefixListId": str,
         "DestinationIpv6CidrBlock": str,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
-
 class EC2ReplaceRouteActionTypeDef(
     _RequiredEC2ReplaceRouteActionTypeDef, _OptionalEC2ReplaceRouteActionTypeDef
 ):
     pass
 
-
 _RequiredEC2ReplaceRouteTableAssociationActionTypeDef = TypedDict(
     "_RequiredEC2ReplaceRouteTableAssociationActionTypeDef",
     {
         "AssociationId": ActionTargetTypeDef,
         "RouteTableId": ActionTargetTypeDef,
     },
 )
@@ -1428,77 +1537,108 @@
     "_OptionalEC2ReplaceRouteTableAssociationActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class EC2ReplaceRouteTableAssociationActionTypeDef(
     _RequiredEC2ReplaceRouteTableAssociationActionTypeDef,
     _OptionalEC2ReplaceRouteTableAssociationActionTypeDef,
 ):
     pass
 
-
 ListAdminAccountsForOrganizationResponseTypeDef = TypedDict(
     "ListAdminAccountsForOrganizationResponseTypeDef",
     {
         "AdminAccounts": List[AdminAccountSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AdminScopeOutputTypeDef = TypedDict(
+    "AdminScopeOutputTypeDef",
+    {
+        "AccountScope": AccountScopeOutputTypeDef,
+        "OrganizationalUnitScope": OrganizationalUnitScopeOutputTypeDef,
+        "RegionScope": RegionScopeOutputTypeDef,
+        "PolicyTypeScope": PolicyTypeScopeOutputTypeDef,
+    },
+    total=False,
+)
+
 AdminScopeTypeDef = TypedDict(
     "AdminScopeTypeDef",
     {
         "AccountScope": AccountScopeTypeDef,
         "OrganizationalUnitScope": OrganizationalUnitScopeTypeDef,
         "RegionScope": RegionScopeTypeDef,
         "PolicyTypeScope": PolicyTypeScopeTypeDef,
     },
     total=False,
 )
 
+_RequiredAppsListDataOutputTypeDef = TypedDict(
+    "_RequiredAppsListDataOutputTypeDef",
+    {
+        "ListName": str,
+        "AppsList": List[AppOutputTypeDef],
+    },
+)
+_OptionalAppsListDataOutputTypeDef = TypedDict(
+    "_OptionalAppsListDataOutputTypeDef",
+    {
+        "ListId": str,
+        "ListUpdateToken": str,
+        "CreateTime": datetime,
+        "LastUpdateTime": datetime,
+        "PreviousAppsList": Dict[str, List[AppOutputTypeDef]],
+    },
+    total=False,
+)
+
+class AppsListDataOutputTypeDef(
+    _RequiredAppsListDataOutputTypeDef, _OptionalAppsListDataOutputTypeDef
+):
+    pass
+
 AppsListDataSummaryTypeDef = TypedDict(
     "AppsListDataSummaryTypeDef",
     {
         "ListArn": str,
         "ListId": str,
         "ListName": str,
-        "AppsList": List[AppTypeDef],
+        "AppsList": List[AppOutputTypeDef],
     },
     total=False,
 )
 
 _RequiredAppsListDataTypeDef = TypedDict(
     "_RequiredAppsListDataTypeDef",
     {
         "ListName": str,
-        "AppsList": List[AppTypeDef],
+        "AppsList": Sequence[AppTypeDef],
     },
 )
 _OptionalAppsListDataTypeDef = TypedDict(
     "_OptionalAppsListDataTypeDef",
     {
         "ListId": str,
         "ListUpdateToken": str,
-        "CreateTime": datetime,
-        "LastUpdateTime": datetime,
-        "PreviousAppsList": Dict[str, List[AppTypeDef]],
+        "CreateTime": Union[datetime, str],
+        "LastUpdateTime": Union[datetime, str],
+        "PreviousAppsList": Mapping[str, Sequence[AppTypeDef]],
     },
     total=False,
 )
 
-
 class AppsListDataTypeDef(_RequiredAppsListDataTypeDef, _OptionalAppsListDataTypeDef):
     pass
 
-
 AwsEc2InstanceViolationTypeDef = TypedDict(
     "AwsEc2InstanceViolationTypeDef",
     {
         "ViolationTarget": str,
         "AwsEc2NetworkInterfaceViolations": List[AwsEc2NetworkInterfaceViolationTypeDef],
     },
     total=False,
@@ -1568,42 +1708,42 @@
     },
     total=False,
 )
 
 GetProtocolsListResponseTypeDef = TypedDict(
     "GetProtocolsListResponseTypeDef",
     {
-        "ProtocolsList": ProtocolsListDataTypeDef,
+        "ProtocolsList": ProtocolsListDataOutputTypeDef,
         "ProtocolsListArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutProtocolsListResponseTypeDef = TypedDict(
     "PutProtocolsListResponseTypeDef",
     {
-        "ProtocolsList": ProtocolsListDataTypeDef,
+        "ProtocolsList": ProtocolsListDataOutputTypeDef,
         "ProtocolsListArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourceSetResponseTypeDef = TypedDict(
     "GetResourceSetResponseTypeDef",
     {
-        "ResourceSet": ResourceSetTypeDef,
+        "ResourceSet": ResourceSetOutputTypeDef,
         "ResourceSetArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutResourceSetResponseTypeDef = TypedDict(
     "PutResourceSetResponseTypeDef",
     {
-        "ResourceSet": ResourceSetTypeDef,
+        "ResourceSet": ResourceSetOutputTypeDef,
         "ResourceSetArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPoliciesResponseTypeDef = TypedDict(
     "ListPoliciesResponseTypeDef",
@@ -1640,69 +1780,19 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "TagList": List[TagTypeDef],
+        "TagList": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPutProtocolsListRequestRequestTypeDef = TypedDict(
-    "_RequiredPutProtocolsListRequestRequestTypeDef",
-    {
-        "ProtocolsList": ProtocolsListDataTypeDef,
-    },
-)
-_OptionalPutProtocolsListRequestRequestTypeDef = TypedDict(
-    "_OptionalPutProtocolsListRequestRequestTypeDef",
-    {
-        "TagList": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class PutProtocolsListRequestRequestTypeDef(
-    _RequiredPutProtocolsListRequestRequestTypeDef, _OptionalPutProtocolsListRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredPutResourceSetRequestRequestTypeDef = TypedDict(
-    "_RequiredPutResourceSetRequestRequestTypeDef",
-    {
-        "ResourceSet": ResourceSetTypeDef,
-    },
-)
-_OptionalPutResourceSetRequestRequestTypeDef = TypedDict(
-    "_OptionalPutResourceSetRequestRequestTypeDef",
-    {
-        "TagList": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class PutResourceSetRequestRequestTypeDef(
-    _RequiredPutResourceSetRequestRequestTypeDef, _OptionalPutResourceSetRequestRequestTypeDef
-):
-    pass
-
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "TagList": Sequence[TagTypeDef],
-    },
-)
-
 ListThirdPartyFirewallFirewallPoliciesResponseTypeDef = TypedDict(
     "ListThirdPartyFirewallFirewallPoliciesResponseTypeDef",
     {
         "ThirdPartyFirewallFirewallPolicies": List[ThirdPartyFirewallFirewallPolicyTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1813,23 +1903,78 @@
         "ResourceId": str,
         "Priority": int,
         "Override": NetworkFirewallStatefulRuleGroupOverrideTypeDef,
     },
     total=False,
 )
 
+PolicyOptionOutputTypeDef = TypedDict(
+    "PolicyOptionOutputTypeDef",
+    {
+        "NetworkFirewallPolicy": NetworkFirewallPolicyOutputTypeDef,
+        "ThirdPartyFirewallPolicy": ThirdPartyFirewallPolicyOutputTypeDef,
+    },
+    total=False,
+)
+
 PolicyOptionTypeDef = TypedDict(
     "PolicyOptionTypeDef",
     {
         "NetworkFirewallPolicy": NetworkFirewallPolicyTypeDef,
         "ThirdPartyFirewallPolicy": ThirdPartyFirewallPolicyTypeDef,
     },
     total=False,
 )
 
+_RequiredPutProtocolsListRequestRequestTypeDef = TypedDict(
+    "_RequiredPutProtocolsListRequestRequestTypeDef",
+    {
+        "ProtocolsList": ProtocolsListDataTypeDef,
+    },
+)
+_OptionalPutProtocolsListRequestRequestTypeDef = TypedDict(
+    "_OptionalPutProtocolsListRequestRequestTypeDef",
+    {
+        "TagList": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class PutProtocolsListRequestRequestTypeDef(
+    _RequiredPutProtocolsListRequestRequestTypeDef, _OptionalPutProtocolsListRequestRequestTypeDef
+):
+    pass
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagList": Sequence[TagTypeDef],
+    },
+)
+
+_RequiredPutResourceSetRequestRequestTypeDef = TypedDict(
+    "_RequiredPutResourceSetRequestRequestTypeDef",
+    {
+        "ResourceSet": ResourceSetTypeDef,
+    },
+)
+_OptionalPutResourceSetRequestRequestTypeDef = TypedDict(
+    "_OptionalPutResourceSetRequestRequestTypeDef",
+    {
+        "TagList": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class PutResourceSetRequestRequestTypeDef(
+    _RequiredPutResourceSetRequestRequestTypeDef, _OptionalPutResourceSetRequestRequestTypeDef
+):
+    pass
+
 SecurityGroupRemediationActionTypeDef = TypedDict(
     "SecurityGroupRemediationActionTypeDef",
     {
         "RemediationActionType": RemediationActionTypeType,
         "Description": str,
         "RemediationResult": SecurityGroupRuleDescriptionTypeDef,
         "IsDefaultAction": bool,
@@ -1854,15 +1999,15 @@
     },
     total=False,
 )
 
 GetAdminScopeResponseTypeDef = TypedDict(
     "GetAdminScopeResponseTypeDef",
     {
-        "AdminScope": AdminScopeTypeDef,
+        "AdminScope": AdminScopeOutputTypeDef,
         "Status": OrganizationStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutAdminAccountRequestRequestTypeDef = TypedDict(
     "_RequiredPutAdminAccountRequestRequestTypeDef",
@@ -1874,69 +2019,65 @@
     "_OptionalPutAdminAccountRequestRequestTypeDef",
     {
         "AdminScope": AdminScopeTypeDef,
     },
     total=False,
 )
 
-
 class PutAdminAccountRequestRequestTypeDef(
     _RequiredPutAdminAccountRequestRequestTypeDef, _OptionalPutAdminAccountRequestRequestTypeDef
 ):
     pass
 
-
-ListAppsListsResponseTypeDef = TypedDict(
-    "ListAppsListsResponseTypeDef",
+GetAppsListResponseTypeDef = TypedDict(
+    "GetAppsListResponseTypeDef",
     {
-        "AppsLists": List[AppsListDataSummaryTypeDef],
-        "NextToken": str,
+        "AppsList": AppsListDataOutputTypeDef,
+        "AppsListArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetAppsListResponseTypeDef = TypedDict(
-    "GetAppsListResponseTypeDef",
+PutAppsListResponseTypeDef = TypedDict(
+    "PutAppsListResponseTypeDef",
     {
-        "AppsList": AppsListDataTypeDef,
+        "AppsList": AppsListDataOutputTypeDef,
         "AppsListArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListAppsListsResponseTypeDef = TypedDict(
+    "ListAppsListsResponseTypeDef",
+    {
+        "AppsLists": List[AppsListDataSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutAppsListRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppsListRequestRequestTypeDef",
     {
         "AppsList": AppsListDataTypeDef,
     },
 )
 _OptionalPutAppsListRequestRequestTypeDef = TypedDict(
     "_OptionalPutAppsListRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutAppsListRequestRequestTypeDef(
     _RequiredPutAppsListRequestRequestTypeDef, _OptionalPutAppsListRequestRequestTypeDef
 ):
     pass
 
-
-PutAppsListResponseTypeDef = TypedDict(
-    "PutAppsListResponseTypeDef",
-    {
-        "AppsList": AppsListDataTypeDef,
-        "AppsListArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetComplianceDetailResponseTypeDef = TypedDict(
     "GetComplianceDetailResponseTypeDef",
     {
         "PolicyComplianceDetail": PolicyComplianceDetailTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1960,14 +2101,34 @@
         "StatefulRuleGroups": List[StatefulRuleGroupTypeDef],
         "StatefulDefaultActions": List[str],
         "StatefulEngineOptions": StatefulEngineOptionsTypeDef,
     },
     total=False,
 )
 
+_RequiredSecurityServicePolicyDataOutputTypeDef = TypedDict(
+    "_RequiredSecurityServicePolicyDataOutputTypeDef",
+    {
+        "Type": SecurityServiceTypeType,
+    },
+)
+_OptionalSecurityServicePolicyDataOutputTypeDef = TypedDict(
+    "_OptionalSecurityServicePolicyDataOutputTypeDef",
+    {
+        "ManagedServiceData": str,
+        "PolicyOption": PolicyOptionOutputTypeDef,
+    },
+    total=False,
+)
+
+class SecurityServicePolicyDataOutputTypeDef(
+    _RequiredSecurityServicePolicyDataOutputTypeDef, _OptionalSecurityServicePolicyDataOutputTypeDef
+):
+    pass
+
 _RequiredSecurityServicePolicyDataTypeDef = TypedDict(
     "_RequiredSecurityServicePolicyDataTypeDef",
     {
         "Type": SecurityServiceTypeType,
     },
 )
 _OptionalSecurityServicePolicyDataTypeDef = TypedDict(
@@ -1975,21 +2136,19 @@
     {
         "ManagedServiceData": str,
         "PolicyOption": PolicyOptionTypeDef,
     },
     total=False,
 )
 
-
 class SecurityServicePolicyDataTypeDef(
     _RequiredSecurityServicePolicyDataTypeDef, _OptionalSecurityServicePolicyDataTypeDef
 ):
     pass
 
-
 AwsVPCSecurityGroupViolationTypeDef = TypedDict(
     "AwsVPCSecurityGroupViolationTypeDef",
     {
         "ViolationTarget": str,
         "ViolationTargetDescription": str,
         "PartialMatches": List[PartialMatchTypeDef],
         "PossibleSecurityGroupRemediationActions": List[SecurityGroupRemediationActionTypeDef],
@@ -2012,46 +2171,74 @@
         "ViolationTarget": str,
         "CurrentPolicyDescription": NetworkFirewallPolicyDescriptionTypeDef,
         "ExpectedPolicyDescription": NetworkFirewallPolicyDescriptionTypeDef,
     },
     total=False,
 )
 
-_RequiredPolicyTypeDef = TypedDict(
-    "_RequiredPolicyTypeDef",
+_RequiredPolicyOutputTypeDef = TypedDict(
+    "_RequiredPolicyOutputTypeDef",
     {
         "PolicyName": str,
-        "SecurityServicePolicyData": SecurityServicePolicyDataTypeDef,
+        "SecurityServicePolicyData": SecurityServicePolicyDataOutputTypeDef,
         "ResourceType": str,
         "ExcludeResourceTags": bool,
         "RemediationEnabled": bool,
     },
 )
-_OptionalPolicyTypeDef = TypedDict(
-    "_OptionalPolicyTypeDef",
+_OptionalPolicyOutputTypeDef = TypedDict(
+    "_OptionalPolicyOutputTypeDef",
     {
         "PolicyId": str,
         "PolicyUpdateToken": str,
         "ResourceTypeList": List[str],
-        "ResourceTags": List[ResourceTagTypeDef],
+        "ResourceTags": List[ResourceTagOutputTypeDef],
         "DeleteUnusedFMManagedResources": bool,
         "IncludeMap": Dict[CustomerPolicyScopeIdTypeType, List[str]],
         "ExcludeMap": Dict[CustomerPolicyScopeIdTypeType, List[str]],
         "ResourceSetIds": List[str],
         "PolicyDescription": str,
         "PolicyStatus": CustomerPolicyStatusType,
     },
     total=False,
 )
 
+class PolicyOutputTypeDef(_RequiredPolicyOutputTypeDef, _OptionalPolicyOutputTypeDef):
+    pass
+
+_RequiredPolicyTypeDef = TypedDict(
+    "_RequiredPolicyTypeDef",
+    {
+        "PolicyName": str,
+        "SecurityServicePolicyData": SecurityServicePolicyDataTypeDef,
+        "ResourceType": str,
+        "ExcludeResourceTags": bool,
+        "RemediationEnabled": bool,
+    },
+)
+_OptionalPolicyTypeDef = TypedDict(
+    "_OptionalPolicyTypeDef",
+    {
+        "PolicyId": str,
+        "PolicyUpdateToken": str,
+        "ResourceTypeList": Sequence[str],
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+        "DeleteUnusedFMManagedResources": bool,
+        "IncludeMap": Mapping[CustomerPolicyScopeIdTypeType, Sequence[str]],
+        "ExcludeMap": Mapping[CustomerPolicyScopeIdTypeType, Sequence[str]],
+        "ResourceSetIds": Sequence[str],
+        "PolicyDescription": str,
+        "PolicyStatus": CustomerPolicyStatusType,
+    },
+    total=False,
+)
 
 class PolicyTypeDef(_RequiredPolicyTypeDef, _OptionalPolicyTypeDef):
     pass
 
-
 _RequiredPossibleRemediationActionTypeDef = TypedDict(
     "_RequiredPossibleRemediationActionTypeDef",
     {
         "OrderedRemediationActions": List[RemediationActionWithOrderTypeDef],
     },
 )
 _OptionalPossibleRemediationActionTypeDef = TypedDict(
@@ -2059,25 +2246,32 @@
     {
         "Description": str,
         "IsDefaultAction": bool,
     },
     total=False,
 )
 
-
 class PossibleRemediationActionTypeDef(
     _RequiredPossibleRemediationActionTypeDef, _OptionalPossibleRemediationActionTypeDef
 ):
     pass
 
-
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
-        "Policy": PolicyTypeDef,
+        "Policy": PolicyOutputTypeDef,
+        "PolicyArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutPolicyResponseTypeDef = TypedDict(
+    "PutPolicyResponseTypeDef",
+    {
+        "Policy": PolicyOutputTypeDef,
         "PolicyArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutPolicyRequestRequestTypeDef",
@@ -2089,30 +2283,19 @@
     "_OptionalPutPolicyRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutPolicyRequestRequestTypeDef(
     _RequiredPutPolicyRequestRequestTypeDef, _OptionalPutPolicyRequestRequestTypeDef
 ):
     pass
 
-
-PutPolicyResponseTypeDef = TypedDict(
-    "PutPolicyResponseTypeDef",
-    {
-        "Policy": PolicyTypeDef,
-        "PolicyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PossibleRemediationActionsTypeDef = TypedDict(
     "PossibleRemediationActionsTypeDef",
     {
         "Description": str,
         "Actions": List[PossibleRemediationActionTypeDef],
     },
     total=False,
@@ -2177,25 +2360,23 @@
         "ResourceType": str,
         "ResourceViolations": List[ResourceViolationTypeDef],
     },
 )
 _OptionalViolationDetailTypeDef = TypedDict(
     "_OptionalViolationDetailTypeDef",
     {
-        "ResourceTags": List[TagTypeDef],
+        "ResourceTags": List[TagOutputTypeDef],
         "ResourceDescription": str,
     },
     total=False,
 )
 
-
 class ViolationDetailTypeDef(_RequiredViolationDetailTypeDef, _OptionalViolationDetailTypeDef):
     pass
 
-
 GetViolationDetailsResponseTypeDef = TypedDict(
     "GetViolationDetailsResponseTypeDef",
     {
         "ViolationDetail": ViolationDetailTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-fms-1.28.0/mypy_boto3_fms/type_defs.pyi` & `mypy-boto3-fms-1.28.12/mypy_boto3_fms/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for fms service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_fms.type_defs import AccountScopeTypeDef
+    from mypy_boto3_fms.type_defs import AccountScopeOutputTypeDef
 
-    data: AccountScopeTypeDef = {...}
+    data: AccountScopeOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccountRoleStatusType,
     CustomerPolicyScopeIdTypeType,
     CustomerPolicyStatusType,
     DependentServiceNameType,
     DestinationTypeType,
@@ -41,21 +41,27 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "AccountScopeOutputTypeDef",
     "AccountScopeTypeDef",
     "ActionTargetTypeDef",
     "AdminAccountSummaryTypeDef",
+    "OrganizationalUnitScopeOutputTypeDef",
+    "PolicyTypeScopeOutputTypeDef",
+    "RegionScopeOutputTypeDef",
     "OrganizationalUnitScopeTypeDef",
     "PolicyTypeScopeTypeDef",
     "RegionScopeTypeDef",
+    "AppOutputTypeDef",
     "AppTypeDef",
     "AssociateAdminAccountRequestRequestTypeDef",
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
     "AssociateThirdPartyFirewallResponseTypeDef",
     "AwsEc2NetworkInterfaceViolationTypeDef",
     "PartialMatchTypeDef",
     "BatchAssociateResourceRequestRequestTypeDef",
@@ -83,17 +89,17 @@
     "GetAppsListRequestRequestTypeDef",
     "GetComplianceDetailRequestRequestTypeDef",
     "GetNotificationChannelResponseTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "GetProtectionStatusRequestRequestTypeDef",
     "GetProtectionStatusResponseTypeDef",
     "GetProtocolsListRequestRequestTypeDef",
-    "ProtocolsListDataTypeDef",
+    "ProtocolsListDataOutputTypeDef",
     "GetResourceSetRequestRequestTypeDef",
-    "ResourceSetTypeDef",
+    "ResourceSetOutputTypeDef",
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
     "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
     "GetViolationDetailsRequestRequestTypeDef",
     "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
     "ListAdminAccountsForOrganizationRequestRequestTypeDef",
     "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
     "ListAdminsManagingAccountRequestRequestTypeDef",
@@ -113,45 +119,53 @@
     "ListProtocolsListsRequestRequestTypeDef",
     "ProtocolsListDataSummaryTypeDef",
     "ListResourceSetResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
     "ListResourceSetsRequestRequestTypeDef",
     "ResourceSetSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     "ThirdPartyFirewallFirewallPolicyTypeDef",
     "RouteTypeDef",
     "NetworkFirewallMissingExpectedRTViolationTypeDef",
     "NetworkFirewallMissingFirewallViolationTypeDef",
     "NetworkFirewallMissingSubnetViolationTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupTypeDef",
+    "NetworkFirewallPolicyOutputTypeDef",
     "NetworkFirewallPolicyTypeDef",
     "NetworkFirewallStatefulRuleGroupOverrideTypeDef",
     "PaginatorConfigTypeDef",
+    "ThirdPartyFirewallPolicyOutputTypeDef",
     "ThirdPartyFirewallPolicyTypeDef",
+    "ResourceTagOutputTypeDef",
     "ResourceTagTypeDef",
+    "ProtocolsListDataTypeDef",
+    "TagTypeDef",
     "PutNotificationChannelRequestRequestTypeDef",
+    "ResourceSetTypeDef",
     "ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef",
     "ThirdPartyFirewallMissingFirewallViolationTypeDef",
     "ThirdPartyFirewallMissingSubnetViolationTypeDef",
     "ResponseMetadataTypeDef",
     "SecurityGroupRuleDescriptionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "EC2AssociateRouteTableActionTypeDef",
     "EC2CopyRouteTableActionTypeDef",
     "EC2CreateRouteActionTypeDef",
     "EC2CreateRouteTableActionTypeDef",
     "EC2DeleteRouteActionTypeDef",
     "EC2ReplaceRouteActionTypeDef",
     "EC2ReplaceRouteTableAssociationActionTypeDef",
     "ListAdminAccountsForOrganizationResponseTypeDef",
+    "AdminScopeOutputTypeDef",
     "AdminScopeTypeDef",
+    "AppsListDataOutputTypeDef",
     "AppsListDataSummaryTypeDef",
     "AppsListDataTypeDef",
     "AwsEc2InstanceViolationTypeDef",
     "BatchAssociateResourceResponseTypeDef",
     "BatchDisassociateResourceResponseTypeDef",
     "PolicyComplianceDetailTypeDef",
     "ListDiscoveredResourcesResponseTypeDef",
@@ -162,56 +176,69 @@
     "GetResourceSetResponseTypeDef",
     "PutResourceSetResponseTypeDef",
     "ListPoliciesResponseTypeDef",
     "ListProtocolsListsResponseTypeDef",
     "ListResourceSetResourcesResponseTypeDef",
     "ListResourceSetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "PutProtocolsListRequestRequestTypeDef",
-    "PutResourceSetRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesResponseTypeDef",
     "NetworkFirewallBlackHoleRouteDetectedViolationTypeDef",
     "NetworkFirewallInternetTrafficNotInspectedViolationTypeDef",
     "NetworkFirewallInvalidRouteConfigurationViolationTypeDef",
     "NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef",
     "NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef",
     "RouteHasOutOfScopeEndpointViolationTypeDef",
     "StatefulRuleGroupTypeDef",
+    "PolicyOptionOutputTypeDef",
     "PolicyOptionTypeDef",
+    "PutProtocolsListRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "PutResourceSetRequestRequestTypeDef",
     "SecurityGroupRemediationActionTypeDef",
     "RemediationActionTypeDef",
     "GetAdminScopeResponseTypeDef",
     "PutAdminAccountRequestRequestTypeDef",
-    "ListAppsListsResponseTypeDef",
     "GetAppsListResponseTypeDef",
-    "PutAppsListRequestRequestTypeDef",
     "PutAppsListResponseTypeDef",
+    "ListAppsListsResponseTypeDef",
+    "PutAppsListRequestRequestTypeDef",
     "GetComplianceDetailResponseTypeDef",
     "ListComplianceStatusResponseTypeDef",
     "NetworkFirewallPolicyDescriptionTypeDef",
+    "SecurityServicePolicyDataOutputTypeDef",
     "SecurityServicePolicyDataTypeDef",
     "AwsVPCSecurityGroupViolationTypeDef",
     "RemediationActionWithOrderTypeDef",
     "NetworkFirewallPolicyModifiedViolationTypeDef",
+    "PolicyOutputTypeDef",
     "PolicyTypeDef",
     "PossibleRemediationActionTypeDef",
     "GetPolicyResponseTypeDef",
-    "PutPolicyRequestRequestTypeDef",
     "PutPolicyResponseTypeDef",
+    "PutPolicyRequestRequestTypeDef",
     "PossibleRemediationActionsTypeDef",
     "ResourceViolationTypeDef",
     "ViolationDetailTypeDef",
     "GetViolationDetailsResponseTypeDef",
 )
 
+AccountScopeOutputTypeDef = TypedDict(
+    "AccountScopeOutputTypeDef",
+    {
+        "Accounts": List[str],
+        "AllAccountsEnabled": bool,
+        "ExcludeSpecifiedAccounts": bool,
+    },
+    total=False,
+)
+
 AccountScopeTypeDef = TypedDict(
     "AccountScopeTypeDef",
     {
-        "Accounts": List[str],
+        "Accounts": Sequence[str],
         "AllAccountsEnabled": bool,
         "ExcludeSpecifiedAccounts": bool,
     },
     total=False,
 )
 
 ActionTargetTypeDef = TypedDict(
@@ -229,42 +256,79 @@
         "AdminAccount": str,
         "DefaultAdmin": bool,
         "Status": OrganizationStatusType,
     },
     total=False,
 )
 
+OrganizationalUnitScopeOutputTypeDef = TypedDict(
+    "OrganizationalUnitScopeOutputTypeDef",
+    {
+        "OrganizationalUnits": List[str],
+        "AllOrganizationalUnitsEnabled": bool,
+        "ExcludeSpecifiedOrganizationalUnits": bool,
+    },
+    total=False,
+)
+
+PolicyTypeScopeOutputTypeDef = TypedDict(
+    "PolicyTypeScopeOutputTypeDef",
+    {
+        "PolicyTypes": List[SecurityServiceTypeType],
+        "AllPolicyTypesEnabled": bool,
+    },
+    total=False,
+)
+
+RegionScopeOutputTypeDef = TypedDict(
+    "RegionScopeOutputTypeDef",
+    {
+        "Regions": List[str],
+        "AllRegionsEnabled": bool,
+    },
+    total=False,
+)
+
 OrganizationalUnitScopeTypeDef = TypedDict(
     "OrganizationalUnitScopeTypeDef",
     {
-        "OrganizationalUnits": List[str],
+        "OrganizationalUnits": Sequence[str],
         "AllOrganizationalUnitsEnabled": bool,
         "ExcludeSpecifiedOrganizationalUnits": bool,
     },
     total=False,
 )
 
 PolicyTypeScopeTypeDef = TypedDict(
     "PolicyTypeScopeTypeDef",
     {
-        "PolicyTypes": List[SecurityServiceTypeType],
+        "PolicyTypes": Sequence[SecurityServiceTypeType],
         "AllPolicyTypesEnabled": bool,
     },
     total=False,
 )
 
 RegionScopeTypeDef = TypedDict(
     "RegionScopeTypeDef",
     {
-        "Regions": List[str],
+        "Regions": Sequence[str],
         "AllRegionsEnabled": bool,
     },
     total=False,
 )
 
+AppOutputTypeDef = TypedDict(
+    "AppOutputTypeDef",
+    {
+        "AppName": str,
+        "Protocol": str,
+        "Port": int,
+    },
+)
+
 AppTypeDef = TypedDict(
     "AppTypeDef",
     {
         "AppName": str,
         "Protocol": str,
         "Port": int,
     },
@@ -363,19 +427,21 @@
     "_OptionalDeletePolicyRequestRequestTypeDef",
     {
         "DeleteAllPolicyResources": bool,
     },
     total=False,
 )
 
+
 class DeletePolicyRequestRequestTypeDef(
     _RequiredDeletePolicyRequestRequestTypeDef, _OptionalDeletePolicyRequestRequestTypeDef
 ):
     pass
 
+
 DeleteProtocolsListRequestRequestTypeDef = TypedDict(
     "DeleteProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
 
@@ -531,19 +597,21 @@
     "_OptionalGetAppsListRequestRequestTypeDef",
     {
         "DefaultList": bool,
     },
     total=False,
 )
 
+
 class GetAppsListRequestRequestTypeDef(
     _RequiredGetAppsListRequestRequestTypeDef, _OptionalGetAppsListRequestRequestTypeDef
 ):
     pass
 
+
 GetComplianceDetailRequestRequestTypeDef = TypedDict(
     "GetComplianceDetailRequestRequestTypeDef",
     {
         "PolicyId": str,
         "MemberAccount": str,
     },
 )
@@ -578,20 +646,22 @@
         "EndTime": Union[datetime, str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetProtectionStatusRequestRequestTypeDef(
     _RequiredGetProtectionStatusRequestRequestTypeDef,
     _OptionalGetProtectionStatusRequestRequestTypeDef,
 ):
     pass
 
+
 GetProtectionStatusResponseTypeDef = TypedDict(
     "GetProtectionStatusResponseTypeDef",
     {
         "AdminAccountId": str,
         "ServiceType": SecurityServiceTypeType,
         "Data": str,
         "NextToken": str,
@@ -609,72 +679,80 @@
     "_OptionalGetProtocolsListRequestRequestTypeDef",
     {
         "DefaultList": bool,
     },
     total=False,
 )
 
+
 class GetProtocolsListRequestRequestTypeDef(
     _RequiredGetProtocolsListRequestRequestTypeDef, _OptionalGetProtocolsListRequestRequestTypeDef
 ):
     pass
 
-_RequiredProtocolsListDataTypeDef = TypedDict(
-    "_RequiredProtocolsListDataTypeDef",
+
+_RequiredProtocolsListDataOutputTypeDef = TypedDict(
+    "_RequiredProtocolsListDataOutputTypeDef",
     {
         "ListName": str,
         "ProtocolsList": List[str],
     },
 )
-_OptionalProtocolsListDataTypeDef = TypedDict(
-    "_OptionalProtocolsListDataTypeDef",
+_OptionalProtocolsListDataOutputTypeDef = TypedDict(
+    "_OptionalProtocolsListDataOutputTypeDef",
     {
         "ListId": str,
         "ListUpdateToken": str,
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "PreviousProtocolsList": Dict[str, List[str]],
     },
     total=False,
 )
 
-class ProtocolsListDataTypeDef(
-    _RequiredProtocolsListDataTypeDef, _OptionalProtocolsListDataTypeDef
+
+class ProtocolsListDataOutputTypeDef(
+    _RequiredProtocolsListDataOutputTypeDef, _OptionalProtocolsListDataOutputTypeDef
 ):
     pass
 
+
 GetResourceSetRequestRequestTypeDef = TypedDict(
     "GetResourceSetRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
-_RequiredResourceSetTypeDef = TypedDict(
-    "_RequiredResourceSetTypeDef",
+_RequiredResourceSetOutputTypeDef = TypedDict(
+    "_RequiredResourceSetOutputTypeDef",
     {
         "Name": str,
         "ResourceTypeList": List[str],
     },
 )
-_OptionalResourceSetTypeDef = TypedDict(
-    "_OptionalResourceSetTypeDef",
+_OptionalResourceSetOutputTypeDef = TypedDict(
+    "_OptionalResourceSetOutputTypeDef",
     {
         "Id": str,
         "Description": str,
         "UpdateToken": str,
         "LastUpdateTime": datetime,
         "ResourceSetStatus": ResourceSetStatusType,
     },
     total=False,
 )
 
-class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
+
+class ResourceSetOutputTypeDef(
+    _RequiredResourceSetOutputTypeDef, _OptionalResourceSetOutputTypeDef
+):
     pass
 
+
 GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef = TypedDict(
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
     },
 )
 
@@ -760,39 +838,43 @@
     {
         "DefaultLists": bool,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAppsListsRequestRequestTypeDef(
     _RequiredListAppsListsRequestRequestTypeDef, _OptionalListAppsListsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
     "_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
     {
         "PolicyId": str,
     },
 )
 _OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
     "_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListComplianceStatusRequestListComplianceStatusPaginateTypeDef(
     _RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
     _OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListComplianceStatusRequestRequestTypeDef = TypedDict(
     "_RequiredListComplianceStatusRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 _OptionalListComplianceStatusRequestRequestTypeDef = TypedDict(
@@ -800,20 +882,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListComplianceStatusRequestRequestTypeDef(
     _RequiredListComplianceStatusRequestRequestTypeDef,
     _OptionalListComplianceStatusRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDiscoveredResourcesRequestRequestTypeDef",
     {
         "MemberAccountIds": Sequence[str],
         "ResourceType": str,
     },
 )
@@ -822,20 +906,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
+
 ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
     "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -910,20 +996,22 @@
     {
         "DefaultLists": bool,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListProtocolsListsRequestRequestTypeDef(
     _RequiredListProtocolsListsRequestRequestTypeDef,
     _OptionalListProtocolsListsRequestRequestTypeDef,
 ):
     pass
 
+
 ProtocolsListDataSummaryTypeDef = TypedDict(
     "ProtocolsListDataSummaryTypeDef",
     {
         "ListArn": str,
         "ListId": str,
         "ListName": str,
         "ProtocolsList": List[str],
@@ -942,37 +1030,41 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListResourceSetResourcesRequestRequestTypeDef(
     _RequiredListResourceSetResourcesRequestRequestTypeDef,
     _OptionalListResourceSetResourcesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
         "URI": str,
     },
 )
 _OptionalResourceTypeDef = TypedDict(
     "_OptionalResourceTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
+
 class ResourceTypeDef(_RequiredResourceTypeDef, _OptionalResourceTypeDef):
     pass
 
+
 ListResourceSetsRequestRequestTypeDef = TypedDict(
     "ListResourceSetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -993,16 +1085,16 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 
 _RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
@@ -1015,20 +1107,22 @@
     "_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef(
     _RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     _OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
         "MaxResults": int,
     },
 )
@@ -1036,20 +1130,22 @@
     "_OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef(
     _RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
     _OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
 ):
     pass
 
+
 ThirdPartyFirewallFirewallPolicyTypeDef = TypedDict(
     "ThirdPartyFirewallFirewallPolicyTypeDef",
     {
         "FirewallPolicyId": str,
         "FirewallPolicyName": str,
     },
     total=False,
@@ -1114,14 +1210,22 @@
         "RuleGroupName": str,
         "ResourceId": str,
         "Priority": int,
     },
     total=False,
 )
 
+NetworkFirewallPolicyOutputTypeDef = TypedDict(
+    "NetworkFirewallPolicyOutputTypeDef",
+    {
+        "FirewallDeploymentModel": FirewallDeploymentModelType,
+    },
+    total=False,
+)
+
 NetworkFirewallPolicyTypeDef = TypedDict(
     "NetworkFirewallPolicyTypeDef",
     {
         "FirewallDeploymentModel": FirewallDeploymentModelType,
     },
     total=False,
 )
@@ -1140,47 +1244,136 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+ThirdPartyFirewallPolicyOutputTypeDef = TypedDict(
+    "ThirdPartyFirewallPolicyOutputTypeDef",
+    {
+        "FirewallDeploymentModel": FirewallDeploymentModelType,
+    },
+    total=False,
+)
+
 ThirdPartyFirewallPolicyTypeDef = TypedDict(
     "ThirdPartyFirewallPolicyTypeDef",
     {
         "FirewallDeploymentModel": FirewallDeploymentModelType,
     },
     total=False,
 )
 
+_RequiredResourceTagOutputTypeDef = TypedDict(
+    "_RequiredResourceTagOutputTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalResourceTagOutputTypeDef = TypedDict(
+    "_OptionalResourceTagOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+
+class ResourceTagOutputTypeDef(
+    _RequiredResourceTagOutputTypeDef, _OptionalResourceTagOutputTypeDef
+):
+    pass
+
+
 _RequiredResourceTagTypeDef = TypedDict(
     "_RequiredResourceTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalResourceTagTypeDef = TypedDict(
     "_OptionalResourceTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
     pass
 
+
+_RequiredProtocolsListDataTypeDef = TypedDict(
+    "_RequiredProtocolsListDataTypeDef",
+    {
+        "ListName": str,
+        "ProtocolsList": Sequence[str],
+    },
+)
+_OptionalProtocolsListDataTypeDef = TypedDict(
+    "_OptionalProtocolsListDataTypeDef",
+    {
+        "ListId": str,
+        "ListUpdateToken": str,
+        "CreateTime": Union[datetime, str],
+        "LastUpdateTime": Union[datetime, str],
+        "PreviousProtocolsList": Mapping[str, Sequence[str]],
+    },
+    total=False,
+)
+
+
+class ProtocolsListDataTypeDef(
+    _RequiredProtocolsListDataTypeDef, _OptionalProtocolsListDataTypeDef
+):
+    pass
+
+
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 PutNotificationChannelRequestRequestTypeDef = TypedDict(
     "PutNotificationChannelRequestRequestTypeDef",
     {
         "SnsTopicArn": str,
         "SnsRoleName": str,
     },
 )
 
+_RequiredResourceSetTypeDef = TypedDict(
+    "_RequiredResourceSetTypeDef",
+    {
+        "Name": str,
+        "ResourceTypeList": Sequence[str],
+    },
+)
+_OptionalResourceSetTypeDef = TypedDict(
+    "_OptionalResourceSetTypeDef",
+    {
+        "Id": str,
+        "Description": str,
+        "UpdateToken": str,
+        "LastUpdateTime": Union[datetime, str],
+        "ResourceSetStatus": ResourceSetStatusType,
+    },
+    total=False,
+)
+
+
+class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
+    pass
+
+
 ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef = TypedDict(
     "ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef",
     {
         "ViolationTarget": str,
         "VPC": str,
         "AvailabilityZone": str,
         "CurrentRouteTable": str,
@@ -1255,19 +1448,21 @@
         "Description": str,
         "SubnetId": ActionTargetTypeDef,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
+
 class EC2AssociateRouteTableActionTypeDef(
     _RequiredEC2AssociateRouteTableActionTypeDef, _OptionalEC2AssociateRouteTableActionTypeDef
 ):
     pass
 
+
 _RequiredEC2CopyRouteTableActionTypeDef = TypedDict(
     "_RequiredEC2CopyRouteTableActionTypeDef",
     {
         "VpcId": ActionTargetTypeDef,
         "RouteTableId": ActionTargetTypeDef,
     },
 )
@@ -1275,19 +1470,21 @@
     "_OptionalEC2CopyRouteTableActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class EC2CopyRouteTableActionTypeDef(
     _RequiredEC2CopyRouteTableActionTypeDef, _OptionalEC2CopyRouteTableActionTypeDef
 ):
     pass
 
+
 _RequiredEC2CreateRouteActionTypeDef = TypedDict(
     "_RequiredEC2CreateRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2CreateRouteActionTypeDef = TypedDict(
@@ -1299,38 +1496,42 @@
         "DestinationIpv6CidrBlock": str,
         "VpcEndpointId": ActionTargetTypeDef,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
+
 class EC2CreateRouteActionTypeDef(
     _RequiredEC2CreateRouteActionTypeDef, _OptionalEC2CreateRouteActionTypeDef
 ):
     pass
 
+
 _RequiredEC2CreateRouteTableActionTypeDef = TypedDict(
     "_RequiredEC2CreateRouteTableActionTypeDef",
     {
         "VpcId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2CreateRouteTableActionTypeDef = TypedDict(
     "_OptionalEC2CreateRouteTableActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class EC2CreateRouteTableActionTypeDef(
     _RequiredEC2CreateRouteTableActionTypeDef, _OptionalEC2CreateRouteTableActionTypeDef
 ):
     pass
 
+
 _RequiredEC2DeleteRouteActionTypeDef = TypedDict(
     "_RequiredEC2DeleteRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2DeleteRouteActionTypeDef = TypedDict(
@@ -1340,19 +1541,21 @@
         "DestinationCidrBlock": str,
         "DestinationPrefixListId": str,
         "DestinationIpv6CidrBlock": str,
     },
     total=False,
 )
 
+
 class EC2DeleteRouteActionTypeDef(
     _RequiredEC2DeleteRouteActionTypeDef, _OptionalEC2DeleteRouteActionTypeDef
 ):
     pass
 
+
 _RequiredEC2ReplaceRouteActionTypeDef = TypedDict(
     "_RequiredEC2ReplaceRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2ReplaceRouteActionTypeDef = TypedDict(
@@ -1363,19 +1566,21 @@
         "DestinationPrefixListId": str,
         "DestinationIpv6CidrBlock": str,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
+
 class EC2ReplaceRouteActionTypeDef(
     _RequiredEC2ReplaceRouteActionTypeDef, _OptionalEC2ReplaceRouteActionTypeDef
 ):
     pass
 
+
 _RequiredEC2ReplaceRouteTableAssociationActionTypeDef = TypedDict(
     "_RequiredEC2ReplaceRouteTableAssociationActionTypeDef",
     {
         "AssociationId": ActionTargetTypeDef,
         "RouteTableId": ActionTargetTypeDef,
     },
 )
@@ -1383,73 +1588,114 @@
     "_OptionalEC2ReplaceRouteTableAssociationActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class EC2ReplaceRouteTableAssociationActionTypeDef(
     _RequiredEC2ReplaceRouteTableAssociationActionTypeDef,
     _OptionalEC2ReplaceRouteTableAssociationActionTypeDef,
 ):
     pass
 
+
 ListAdminAccountsForOrganizationResponseTypeDef = TypedDict(
     "ListAdminAccountsForOrganizationResponseTypeDef",
     {
         "AdminAccounts": List[AdminAccountSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AdminScopeOutputTypeDef = TypedDict(
+    "AdminScopeOutputTypeDef",
+    {
+        "AccountScope": AccountScopeOutputTypeDef,
+        "OrganizationalUnitScope": OrganizationalUnitScopeOutputTypeDef,
+        "RegionScope": RegionScopeOutputTypeDef,
+        "PolicyTypeScope": PolicyTypeScopeOutputTypeDef,
+    },
+    total=False,
+)
+
 AdminScopeTypeDef = TypedDict(
     "AdminScopeTypeDef",
     {
         "AccountScope": AccountScopeTypeDef,
         "OrganizationalUnitScope": OrganizationalUnitScopeTypeDef,
         "RegionScope": RegionScopeTypeDef,
         "PolicyTypeScope": PolicyTypeScopeTypeDef,
     },
     total=False,
 )
 
+_RequiredAppsListDataOutputTypeDef = TypedDict(
+    "_RequiredAppsListDataOutputTypeDef",
+    {
+        "ListName": str,
+        "AppsList": List[AppOutputTypeDef],
+    },
+)
+_OptionalAppsListDataOutputTypeDef = TypedDict(
+    "_OptionalAppsListDataOutputTypeDef",
+    {
+        "ListId": str,
+        "ListUpdateToken": str,
+        "CreateTime": datetime,
+        "LastUpdateTime": datetime,
+        "PreviousAppsList": Dict[str, List[AppOutputTypeDef]],
+    },
+    total=False,
+)
+
+
+class AppsListDataOutputTypeDef(
+    _RequiredAppsListDataOutputTypeDef, _OptionalAppsListDataOutputTypeDef
+):
+    pass
+
+
 AppsListDataSummaryTypeDef = TypedDict(
     "AppsListDataSummaryTypeDef",
     {
         "ListArn": str,
         "ListId": str,
         "ListName": str,
-        "AppsList": List[AppTypeDef],
+        "AppsList": List[AppOutputTypeDef],
     },
     total=False,
 )
 
 _RequiredAppsListDataTypeDef = TypedDict(
     "_RequiredAppsListDataTypeDef",
     {
         "ListName": str,
-        "AppsList": List[AppTypeDef],
+        "AppsList": Sequence[AppTypeDef],
     },
 )
 _OptionalAppsListDataTypeDef = TypedDict(
     "_OptionalAppsListDataTypeDef",
     {
         "ListId": str,
         "ListUpdateToken": str,
-        "CreateTime": datetime,
-        "LastUpdateTime": datetime,
-        "PreviousAppsList": Dict[str, List[AppTypeDef]],
+        "CreateTime": Union[datetime, str],
+        "LastUpdateTime": Union[datetime, str],
+        "PreviousAppsList": Mapping[str, Sequence[AppTypeDef]],
     },
     total=False,
 )
 
+
 class AppsListDataTypeDef(_RequiredAppsListDataTypeDef, _OptionalAppsListDataTypeDef):
     pass
 
+
 AwsEc2InstanceViolationTypeDef = TypedDict(
     "AwsEc2InstanceViolationTypeDef",
     {
         "ViolationTarget": str,
         "AwsEc2NetworkInterfaceViolations": List[AwsEc2NetworkInterfaceViolationTypeDef],
     },
     total=False,
@@ -1519,42 +1765,42 @@
     },
     total=False,
 )
 
 GetProtocolsListResponseTypeDef = TypedDict(
     "GetProtocolsListResponseTypeDef",
     {
-        "ProtocolsList": ProtocolsListDataTypeDef,
+        "ProtocolsList": ProtocolsListDataOutputTypeDef,
         "ProtocolsListArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutProtocolsListResponseTypeDef = TypedDict(
     "PutProtocolsListResponseTypeDef",
     {
-        "ProtocolsList": ProtocolsListDataTypeDef,
+        "ProtocolsList": ProtocolsListDataOutputTypeDef,
         "ProtocolsListArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourceSetResponseTypeDef = TypedDict(
     "GetResourceSetResponseTypeDef",
     {
-        "ResourceSet": ResourceSetTypeDef,
+        "ResourceSet": ResourceSetOutputTypeDef,
         "ResourceSetArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutResourceSetResponseTypeDef = TypedDict(
     "PutResourceSetResponseTypeDef",
     {
-        "ResourceSet": ResourceSetTypeDef,
+        "ResourceSet": ResourceSetOutputTypeDef,
         "ResourceSetArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPoliciesResponseTypeDef = TypedDict(
     "ListPoliciesResponseTypeDef",
@@ -1591,65 +1837,19 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "TagList": List[TagTypeDef],
+        "TagList": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPutProtocolsListRequestRequestTypeDef = TypedDict(
-    "_RequiredPutProtocolsListRequestRequestTypeDef",
-    {
-        "ProtocolsList": ProtocolsListDataTypeDef,
-    },
-)
-_OptionalPutProtocolsListRequestRequestTypeDef = TypedDict(
-    "_OptionalPutProtocolsListRequestRequestTypeDef",
-    {
-        "TagList": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class PutProtocolsListRequestRequestTypeDef(
-    _RequiredPutProtocolsListRequestRequestTypeDef, _OptionalPutProtocolsListRequestRequestTypeDef
-):
-    pass
-
-_RequiredPutResourceSetRequestRequestTypeDef = TypedDict(
-    "_RequiredPutResourceSetRequestRequestTypeDef",
-    {
-        "ResourceSet": ResourceSetTypeDef,
-    },
-)
-_OptionalPutResourceSetRequestRequestTypeDef = TypedDict(
-    "_OptionalPutResourceSetRequestRequestTypeDef",
-    {
-        "TagList": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class PutResourceSetRequestRequestTypeDef(
-    _RequiredPutResourceSetRequestRequestTypeDef, _OptionalPutResourceSetRequestRequestTypeDef
-):
-    pass
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "TagList": Sequence[TagTypeDef],
-    },
-)
-
 ListThirdPartyFirewallFirewallPoliciesResponseTypeDef = TypedDict(
     "ListThirdPartyFirewallFirewallPoliciesResponseTypeDef",
     {
         "ThirdPartyFirewallFirewallPolicies": List[ThirdPartyFirewallFirewallPolicyTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1760,23 +1960,82 @@
         "ResourceId": str,
         "Priority": int,
         "Override": NetworkFirewallStatefulRuleGroupOverrideTypeDef,
     },
     total=False,
 )
 
+PolicyOptionOutputTypeDef = TypedDict(
+    "PolicyOptionOutputTypeDef",
+    {
+        "NetworkFirewallPolicy": NetworkFirewallPolicyOutputTypeDef,
+        "ThirdPartyFirewallPolicy": ThirdPartyFirewallPolicyOutputTypeDef,
+    },
+    total=False,
+)
+
 PolicyOptionTypeDef = TypedDict(
     "PolicyOptionTypeDef",
     {
         "NetworkFirewallPolicy": NetworkFirewallPolicyTypeDef,
         "ThirdPartyFirewallPolicy": ThirdPartyFirewallPolicyTypeDef,
     },
     total=False,
 )
 
+_RequiredPutProtocolsListRequestRequestTypeDef = TypedDict(
+    "_RequiredPutProtocolsListRequestRequestTypeDef",
+    {
+        "ProtocolsList": ProtocolsListDataTypeDef,
+    },
+)
+_OptionalPutProtocolsListRequestRequestTypeDef = TypedDict(
+    "_OptionalPutProtocolsListRequestRequestTypeDef",
+    {
+        "TagList": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class PutProtocolsListRequestRequestTypeDef(
+    _RequiredPutProtocolsListRequestRequestTypeDef, _OptionalPutProtocolsListRequestRequestTypeDef
+):
+    pass
+
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagList": Sequence[TagTypeDef],
+    },
+)
+
+_RequiredPutResourceSetRequestRequestTypeDef = TypedDict(
+    "_RequiredPutResourceSetRequestRequestTypeDef",
+    {
+        "ResourceSet": ResourceSetTypeDef,
+    },
+)
+_OptionalPutResourceSetRequestRequestTypeDef = TypedDict(
+    "_OptionalPutResourceSetRequestRequestTypeDef",
+    {
+        "TagList": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class PutResourceSetRequestRequestTypeDef(
+    _RequiredPutResourceSetRequestRequestTypeDef, _OptionalPutResourceSetRequestRequestTypeDef
+):
+    pass
+
+
 SecurityGroupRemediationActionTypeDef = TypedDict(
     "SecurityGroupRemediationActionTypeDef",
     {
         "RemediationActionType": RemediationActionTypeType,
         "Description": str,
         "RemediationResult": SecurityGroupRuleDescriptionTypeDef,
         "IsDefaultAction": bool,
@@ -1801,15 +2060,15 @@
     },
     total=False,
 )
 
 GetAdminScopeResponseTypeDef = TypedDict(
     "GetAdminScopeResponseTypeDef",
     {
-        "AdminScope": AdminScopeTypeDef,
+        "AdminScope": AdminScopeOutputTypeDef,
         "Status": OrganizationStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutAdminAccountRequestRequestTypeDef = TypedDict(
     "_RequiredPutAdminAccountRequestRequestTypeDef",
@@ -1821,64 +2080,68 @@
     "_OptionalPutAdminAccountRequestRequestTypeDef",
     {
         "AdminScope": AdminScopeTypeDef,
     },
     total=False,
 )
 
+
 class PutAdminAccountRequestRequestTypeDef(
     _RequiredPutAdminAccountRequestRequestTypeDef, _OptionalPutAdminAccountRequestRequestTypeDef
 ):
     pass
 
-ListAppsListsResponseTypeDef = TypedDict(
-    "ListAppsListsResponseTypeDef",
+
+GetAppsListResponseTypeDef = TypedDict(
+    "GetAppsListResponseTypeDef",
     {
-        "AppsLists": List[AppsListDataSummaryTypeDef],
-        "NextToken": str,
+        "AppsList": AppsListDataOutputTypeDef,
+        "AppsListArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetAppsListResponseTypeDef = TypedDict(
-    "GetAppsListResponseTypeDef",
+PutAppsListResponseTypeDef = TypedDict(
+    "PutAppsListResponseTypeDef",
     {
-        "AppsList": AppsListDataTypeDef,
+        "AppsList": AppsListDataOutputTypeDef,
         "AppsListArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListAppsListsResponseTypeDef = TypedDict(
+    "ListAppsListsResponseTypeDef",
+    {
+        "AppsLists": List[AppsListDataSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutAppsListRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppsListRequestRequestTypeDef",
     {
         "AppsList": AppsListDataTypeDef,
     },
 )
 _OptionalPutAppsListRequestRequestTypeDef = TypedDict(
     "_OptionalPutAppsListRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutAppsListRequestRequestTypeDef(
     _RequiredPutAppsListRequestRequestTypeDef, _OptionalPutAppsListRequestRequestTypeDef
 ):
     pass
 
-PutAppsListResponseTypeDef = TypedDict(
-    "PutAppsListResponseTypeDef",
-    {
-        "AppsList": AppsListDataTypeDef,
-        "AppsListArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetComplianceDetailResponseTypeDef = TypedDict(
     "GetComplianceDetailResponseTypeDef",
     {
         "PolicyComplianceDetail": PolicyComplianceDetailTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1903,14 +2166,36 @@
         "StatefulRuleGroups": List[StatefulRuleGroupTypeDef],
         "StatefulDefaultActions": List[str],
         "StatefulEngineOptions": StatefulEngineOptionsTypeDef,
     },
     total=False,
 )
 
+_RequiredSecurityServicePolicyDataOutputTypeDef = TypedDict(
+    "_RequiredSecurityServicePolicyDataOutputTypeDef",
+    {
+        "Type": SecurityServiceTypeType,
+    },
+)
+_OptionalSecurityServicePolicyDataOutputTypeDef = TypedDict(
+    "_OptionalSecurityServicePolicyDataOutputTypeDef",
+    {
+        "ManagedServiceData": str,
+        "PolicyOption": PolicyOptionOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class SecurityServicePolicyDataOutputTypeDef(
+    _RequiredSecurityServicePolicyDataOutputTypeDef, _OptionalSecurityServicePolicyDataOutputTypeDef
+):
+    pass
+
+
 _RequiredSecurityServicePolicyDataTypeDef = TypedDict(
     "_RequiredSecurityServicePolicyDataTypeDef",
     {
         "Type": SecurityServiceTypeType,
     },
 )
 _OptionalSecurityServicePolicyDataTypeDef = TypedDict(
@@ -1918,19 +2203,21 @@
     {
         "ManagedServiceData": str,
         "PolicyOption": PolicyOptionTypeDef,
     },
     total=False,
 )
 
+
 class SecurityServicePolicyDataTypeDef(
     _RequiredSecurityServicePolicyDataTypeDef, _OptionalSecurityServicePolicyDataTypeDef
 ):
     pass
 
+
 AwsVPCSecurityGroupViolationTypeDef = TypedDict(
     "AwsVPCSecurityGroupViolationTypeDef",
     {
         "ViolationTarget": str,
         "ViolationTargetDescription": str,
         "PartialMatches": List[PartialMatchTypeDef],
         "PossibleSecurityGroupRemediationActions": List[SecurityGroupRemediationActionTypeDef],
@@ -1953,14 +2240,46 @@
         "ViolationTarget": str,
         "CurrentPolicyDescription": NetworkFirewallPolicyDescriptionTypeDef,
         "ExpectedPolicyDescription": NetworkFirewallPolicyDescriptionTypeDef,
     },
     total=False,
 )
 
+_RequiredPolicyOutputTypeDef = TypedDict(
+    "_RequiredPolicyOutputTypeDef",
+    {
+        "PolicyName": str,
+        "SecurityServicePolicyData": SecurityServicePolicyDataOutputTypeDef,
+        "ResourceType": str,
+        "ExcludeResourceTags": bool,
+        "RemediationEnabled": bool,
+    },
+)
+_OptionalPolicyOutputTypeDef = TypedDict(
+    "_OptionalPolicyOutputTypeDef",
+    {
+        "PolicyId": str,
+        "PolicyUpdateToken": str,
+        "ResourceTypeList": List[str],
+        "ResourceTags": List[ResourceTagOutputTypeDef],
+        "DeleteUnusedFMManagedResources": bool,
+        "IncludeMap": Dict[CustomerPolicyScopeIdTypeType, List[str]],
+        "ExcludeMap": Dict[CustomerPolicyScopeIdTypeType, List[str]],
+        "ResourceSetIds": List[str],
+        "PolicyDescription": str,
+        "PolicyStatus": CustomerPolicyStatusType,
+    },
+    total=False,
+)
+
+
+class PolicyOutputTypeDef(_RequiredPolicyOutputTypeDef, _OptionalPolicyOutputTypeDef):
+    pass
+
+
 _RequiredPolicyTypeDef = TypedDict(
     "_RequiredPolicyTypeDef",
     {
         "PolicyName": str,
         "SecurityServicePolicyData": SecurityServicePolicyDataTypeDef,
         "ResourceType": str,
         "ExcludeResourceTags": bool,
@@ -1968,29 +2287,31 @@
     },
 )
 _OptionalPolicyTypeDef = TypedDict(
     "_OptionalPolicyTypeDef",
     {
         "PolicyId": str,
         "PolicyUpdateToken": str,
-        "ResourceTypeList": List[str],
-        "ResourceTags": List[ResourceTagTypeDef],
+        "ResourceTypeList": Sequence[str],
+        "ResourceTags": Sequence[ResourceTagTypeDef],
         "DeleteUnusedFMManagedResources": bool,
-        "IncludeMap": Dict[CustomerPolicyScopeIdTypeType, List[str]],
-        "ExcludeMap": Dict[CustomerPolicyScopeIdTypeType, List[str]],
-        "ResourceSetIds": List[str],
+        "IncludeMap": Mapping[CustomerPolicyScopeIdTypeType, Sequence[str]],
+        "ExcludeMap": Mapping[CustomerPolicyScopeIdTypeType, Sequence[str]],
+        "ResourceSetIds": Sequence[str],
         "PolicyDescription": str,
         "PolicyStatus": CustomerPolicyStatusType,
     },
     total=False,
 )
 
+
 class PolicyTypeDef(_RequiredPolicyTypeDef, _OptionalPolicyTypeDef):
     pass
 
+
 _RequiredPossibleRemediationActionTypeDef = TypedDict(
     "_RequiredPossibleRemediationActionTypeDef",
     {
         "OrderedRemediationActions": List[RemediationActionWithOrderTypeDef],
     },
 )
 _OptionalPossibleRemediationActionTypeDef = TypedDict(
@@ -1998,23 +2319,34 @@
     {
         "Description": str,
         "IsDefaultAction": bool,
     },
     total=False,
 )
 
+
 class PossibleRemediationActionTypeDef(
     _RequiredPossibleRemediationActionTypeDef, _OptionalPossibleRemediationActionTypeDef
 ):
     pass
 
+
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
-        "Policy": PolicyTypeDef,
+        "Policy": PolicyOutputTypeDef,
+        "PolicyArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutPolicyResponseTypeDef = TypedDict(
+    "PutPolicyResponseTypeDef",
+    {
+        "Policy": PolicyOutputTypeDef,
         "PolicyArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutPolicyRequestRequestTypeDef",
@@ -2026,27 +2358,20 @@
     "_OptionalPutPolicyRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutPolicyRequestRequestTypeDef(
     _RequiredPutPolicyRequestRequestTypeDef, _OptionalPutPolicyRequestRequestTypeDef
 ):
     pass
 
-PutPolicyResponseTypeDef = TypedDict(
-    "PutPolicyResponseTypeDef",
-    {
-        "Policy": PolicyTypeDef,
-        "PolicyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 PossibleRemediationActionsTypeDef = TypedDict(
     "PossibleRemediationActionsTypeDef",
     {
         "Description": str,
         "Actions": List[PossibleRemediationActionTypeDef],
     },
@@ -2112,23 +2437,25 @@
         "ResourceType": str,
         "ResourceViolations": List[ResourceViolationTypeDef],
     },
 )
 _OptionalViolationDetailTypeDef = TypedDict(
     "_OptionalViolationDetailTypeDef",
     {
-        "ResourceTags": List[TagTypeDef],
+        "ResourceTags": List[TagOutputTypeDef],
         "ResourceDescription": str,
     },
     total=False,
 )
 
+
 class ViolationDetailTypeDef(_RequiredViolationDetailTypeDef, _OptionalViolationDetailTypeDef):
     pass
 
+
 GetViolationDetailsResponseTypeDef = TypedDict(
     "GetViolationDetailsResponseTypeDef",
     {
         "ViolationDetail": ViolationDetailTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-fms-1.28.0/mypy_boto3_fms.egg-info/PKG-INFO` & `mypy-boto3-fms-1.28.12/mypy_boto3_fms.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fms
-Version: 1.28.0
-Summary: Type annotations for boto3.FMS 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.FMS 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-fms"></a>
 
 # mypy-boto3-fms
 
 [![PyPI - mypy-boto3-fms](https://img.shields.io/pypi/v/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fms?color=blue)](https://pypistats.org/packages/mypy-boto3-fms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-fms)](https://pepy.tech/project/mypy-boto3-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FMS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[boto3.FMS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
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
 [mypy-boto3-fms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,20 +371,25 @@
 ### Typed dictionaries
 
 `mypy_boto3_fms.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_fms.type_defs import (
+    AccountScopeOutputTypeDef,
     AccountScopeTypeDef,
     ActionTargetTypeDef,
     AdminAccountSummaryTypeDef,
+    OrganizationalUnitScopeOutputTypeDef,
+    PolicyTypeScopeOutputTypeDef,
+    RegionScopeOutputTypeDef,
     OrganizationalUnitScopeTypeDef,
     PolicyTypeScopeTypeDef,
     RegionScopeTypeDef,
+    AppOutputTypeDef,
     AppTypeDef,
     AssociateAdminAccountRequestRequestTypeDef,
     AssociateThirdPartyFirewallRequestRequestTypeDef,
     AssociateThirdPartyFirewallResponseTypeDef,
     AwsEc2NetworkInterfaceViolationTypeDef,
     PartialMatchTypeDef,
     BatchAssociateResourceRequestRequestTypeDef,
@@ -412,17 +417,17 @@
     GetAppsListRequestRequestTypeDef,
     GetComplianceDetailRequestRequestTypeDef,
     GetNotificationChannelResponseTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetProtectionStatusRequestRequestTypeDef,
     GetProtectionStatusResponseTypeDef,
     GetProtocolsListRequestRequestTypeDef,
-    ProtocolsListDataTypeDef,
+    ProtocolsListDataOutputTypeDef,
     GetResourceSetRequestRequestTypeDef,
-    ResourceSetTypeDef,
+    ResourceSetOutputTypeDef,
     GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef,
     GetThirdPartyFirewallAssociationStatusResponseTypeDef,
     GetViolationDetailsRequestRequestTypeDef,
     ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef,
     ListAdminAccountsForOrganizationRequestRequestTypeDef,
     ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef,
     ListAdminsManagingAccountRequestRequestTypeDef,
@@ -442,45 +447,53 @@
     ListProtocolsListsRequestRequestTypeDef,
     ProtocolsListDataSummaryTypeDef,
     ListResourceSetResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListResourceSetsRequestRequestTypeDef,
     ResourceSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
     ThirdPartyFirewallFirewallPolicyTypeDef,
     RouteTypeDef,
     NetworkFirewallMissingExpectedRTViolationTypeDef,
     NetworkFirewallMissingFirewallViolationTypeDef,
     NetworkFirewallMissingSubnetViolationTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupTypeDef,
+    NetworkFirewallPolicyOutputTypeDef,
     NetworkFirewallPolicyTypeDef,
     NetworkFirewallStatefulRuleGroupOverrideTypeDef,
     PaginatorConfigTypeDef,
+    ThirdPartyFirewallPolicyOutputTypeDef,
     ThirdPartyFirewallPolicyTypeDef,
+    ResourceTagOutputTypeDef,
     ResourceTagTypeDef,
+    ProtocolsListDataTypeDef,
+    TagTypeDef,
     PutNotificationChannelRequestRequestTypeDef,
+    ResourceSetTypeDef,
     ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef,
     ThirdPartyFirewallMissingFirewallViolationTypeDef,
     ThirdPartyFirewallMissingSubnetViolationTypeDef,
     ResponseMetadataTypeDef,
     SecurityGroupRuleDescriptionTypeDef,
     UntagResourceRequestRequestTypeDef,
     EC2AssociateRouteTableActionTypeDef,
     EC2CopyRouteTableActionTypeDef,
     EC2CreateRouteActionTypeDef,
     EC2CreateRouteTableActionTypeDef,
     EC2DeleteRouteActionTypeDef,
     EC2ReplaceRouteActionTypeDef,
     EC2ReplaceRouteTableAssociationActionTypeDef,
     ListAdminAccountsForOrganizationResponseTypeDef,
+    AdminScopeOutputTypeDef,
     AdminScopeTypeDef,
+    AppsListDataOutputTypeDef,
     AppsListDataSummaryTypeDef,
     AppsListDataTypeDef,
     AwsEc2InstanceViolationTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     PolicyComplianceDetailTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
@@ -491,54 +504,57 @@
     GetResourceSetResponseTypeDef,
     PutResourceSetResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PutProtocolsListRequestRequestTypeDef,
-    PutResourceSetRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
     NetworkFirewallBlackHoleRouteDetectedViolationTypeDef,
     NetworkFirewallInternetTrafficNotInspectedViolationTypeDef,
     NetworkFirewallInvalidRouteConfigurationViolationTypeDef,
     NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef,
     NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef,
     RouteHasOutOfScopeEndpointViolationTypeDef,
     StatefulRuleGroupTypeDef,
+    PolicyOptionOutputTypeDef,
     PolicyOptionTypeDef,
+    PutProtocolsListRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    PutResourceSetRequestRequestTypeDef,
     SecurityGroupRemediationActionTypeDef,
     RemediationActionTypeDef,
     GetAdminScopeResponseTypeDef,
     PutAdminAccountRequestRequestTypeDef,
-    ListAppsListsResponseTypeDef,
     GetAppsListResponseTypeDef,
-    PutAppsListRequestRequestTypeDef,
     PutAppsListResponseTypeDef,
+    ListAppsListsResponseTypeDef,
+    PutAppsListRequestRequestTypeDef,
     GetComplianceDetailResponseTypeDef,
     ListComplianceStatusResponseTypeDef,
     NetworkFirewallPolicyDescriptionTypeDef,
+    SecurityServicePolicyDataOutputTypeDef,
     SecurityServicePolicyDataTypeDef,
     AwsVPCSecurityGroupViolationTypeDef,
     RemediationActionWithOrderTypeDef,
     NetworkFirewallPolicyModifiedViolationTypeDef,
+    PolicyOutputTypeDef,
     PolicyTypeDef,
     PossibleRemediationActionTypeDef,
     GetPolicyResponseTypeDef,
-    PutPolicyRequestRequestTypeDef,
     PutPolicyResponseTypeDef,
+    PutPolicyRequestRequestTypeDef,
     PossibleRemediationActionsTypeDef,
     ResourceViolationTypeDef,
     ViolationDetailTypeDef,
     GetViolationDetailsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountScopeTypeDef:
+def get_structure() -> AccountScopeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-fms-1.28.0/mypy_boto3_fms.egg-info/SOURCES.txt` & `mypy-boto3-fms-1.28.12/mypy_boto3_fms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.0/setup.py` & `mypy-boto3-fms-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-fms",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_fms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FMS 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.FMS 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

