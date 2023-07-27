# Comparing `tmp/mypy-boto3-wafv2-1.28.0.tar.gz` & `tmp/mypy-boto3-wafv2-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-wafv2-1.28.0.tar", last modified: Thu Jul  6 21:00:50 2023, max compression
+gzip compressed data, was "mypy-boto3-wafv2-1.28.12.tar", last modified: Thu Jul 27 11:49:49 2023, max compression
```

## Comparing `mypy-boto3-wafv2-1.28.0.tar` & `mypy-boto3-wafv2-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:50.482457 mypy-boto3-wafv2-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:57:55.000000 mypy-boto3-wafv2-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19830 2023-07-06 21:00:50.478457 mypy-boto3-wafv2-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-07-06 20:57:55.000000 mypy-boto3-wafv2-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:50.462457 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-06 20:57:55.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-06 20:57:55.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-06 20:57:55.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36893 2023-07-06 20:57:56.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36834 2023-07-06 20:57:56.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-07-06 20:57:56.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-07-06 20:57:56.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:57:55.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    68373 2023-07-06 20:57:58.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    68292 2023-07-06 20:57:57.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:57:55.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:50.478457 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19830 2023-07-06 21:00:50.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-06 21:00:50.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:50.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:50.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:50.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 21:00:50.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:50.482457 mypy-boto3-wafv2-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-06 20:57:55.000000 mypy-boto3-wafv2-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.453491 mypy-boto3-wafv2-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22824 2023-07-27 11:49:49.449491 mypy-boto3-wafv2-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.445491 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36893 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36834 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-07-27 11:48:39.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13529 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    94383 2023-07-27 11:48:41.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94278 2023-07-27 11:48:40.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.449491 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22824 2023-07-27 11:49:49.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-27 11:49:49.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:49.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:49.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:49.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 11:49:49.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:49.453491 mypy-boto3-wafv2-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/setup.py
```

### Comparing `mypy-boto3-wafv2-1.28.0/LICENSE` & `mypy-boto3-wafv2-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.28.0/PKG-INFO` & `mypy-boto3-wafv2-1.28.12/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wafv2
-Version: 1.28.0
-Summary: Type annotations for boto3.WAFV2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.WAFV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-wafv2"></a>
 
 # mypy-boto3-wafv2
 
 [![PyPI - mypy-boto3-wafv2](https://img.shields.io/pypi/v/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wafv2?color=blue)](https://pypistats.org/packages/mypy-boto3-wafv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wafv2)](https://pepy.tech/project/mypy-boto3-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[boto3.WAFV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
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
 [mypy-boto3-wafv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,217 +322,302 @@
 
 `mypy_boto3_wafv2.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_wafv2.type_defs import (
     APIKeySummaryTypeDef,
+    AWSManagedRulesBotControlRuleSetOutputTypeDef,
     AWSManagedRulesBotControlRuleSetTypeDef,
+    ActionConditionOutputTypeDef,
     ActionConditionTypeDef,
+    AddressFieldOutputTypeDef,
     AddressFieldTypeDef,
+    AndStatementOutputTypeDef,
     AndStatementTypeDef,
     AssociateWebACLRequestRequestTypeDef,
+    RequestBodyAssociatedResourceTypeConfigOutputTypeDef,
     RequestBodyAssociatedResourceTypeConfigTypeDef,
+    BodyOutputTypeDef,
     BodyTypeDef,
+    TextTransformationOutputTypeDef,
     TextTransformationTypeDef,
+    ImmunityTimePropertyOutputTypeDef,
     ImmunityTimePropertyTypeDef,
     CaptchaResponseTypeDef,
     ChallengeResponseTypeDef,
-    CheckCapacityResponseTypeDef,
+    ResponseMetadataTypeDef,
+    LabelNameConditionOutputTypeDef,
     LabelNameConditionTypeDef,
+    CookieMatchPatternOutputTypeDef,
     CookieMatchPatternTypeDef,
     CreateAPIKeyRequestRequestTypeDef,
-    CreateAPIKeyResponseTypeDef,
     TagTypeDef,
     IPSetSummaryTypeDef,
     RegexTypeDef,
     RegexPatternSetSummaryTypeDef,
     CustomResponseBodyTypeDef,
     VisibilityConfigTypeDef,
     RuleGroupSummaryTypeDef,
     WebACLSummaryTypeDef,
+    CustomHTTPHeaderOutputTypeDef,
     CustomHTTPHeaderTypeDef,
+    CustomResponseBodyOutputTypeDef,
     DeleteFirewallManagerRuleGroupsRequestRequestTypeDef,
-    DeleteFirewallManagerRuleGroupsResponseTypeDef,
     DeleteIPSetRequestRequestTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeletePermissionPolicyRequestRequestTypeDef,
     DeleteRegexPatternSetRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteWebACLRequestRequestTypeDef,
     DescribeAllManagedProductsRequestRequestTypeDef,
     ManagedProductDescriptorTypeDef,
     DescribeManagedProductsByVendorRequestRequestTypeDef,
     DescribeManagedRuleGroupRequestRequestTypeDef,
     LabelSummaryTypeDef,
     DisassociateWebACLRequestRequestTypeDef,
+    EmailFieldOutputTypeDef,
     EmailFieldTypeDef,
+    ExcludedRuleOutputTypeDef,
     ExcludedRuleTypeDef,
+    HeaderOrderOutputTypeDef,
+    SingleHeaderOutputTypeDef,
+    SingleQueryArgumentOutputTypeDef,
     HeaderOrderTypeDef,
     SingleHeaderTypeDef,
     SingleQueryArgumentTypeDef,
+    VisibilityConfigOutputTypeDef,
+    ForwardedIPConfigOutputTypeDef,
     ForwardedIPConfigTypeDef,
     GenerateMobileSdkReleaseUrlRequestRequestTypeDef,
-    GenerateMobileSdkReleaseUrlResponseTypeDef,
     GetDecryptedAPIKeyRequestRequestTypeDef,
-    GetDecryptedAPIKeyResponseTypeDef,
     GetIPSetRequestRequestTypeDef,
     IPSetTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetManagedRuleSetRequestRequestTypeDef,
     GetMobileSdkReleaseRequestRequestTypeDef,
     GetPermissionPolicyRequestRequestTypeDef,
-    GetPermissionPolicyResponseTypeDef,
     GetRateBasedStatementManagedKeysRequestRequestTypeDef,
     RateBasedStatementManagedKeysIPSetTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
     TimeWindowTypeDef,
+    TimeWindowOutputTypeDef,
     GetWebACLForResourceRequestRequestTypeDef,
     GetWebACLRequestRequestTypeDef,
     HTTPHeaderTypeDef,
+    HeaderMatchPatternOutputTypeDef,
     HeaderMatchPatternTypeDef,
+    IPSetForwardedIPConfigOutputTypeDef,
     IPSetForwardedIPConfigTypeDef,
+    JsonMatchPatternOutputTypeDef,
     JsonMatchPatternTypeDef,
+    LabelMatchStatementOutputTypeDef,
     LabelMatchStatementTypeDef,
+    LabelOutputTypeDef,
     LabelTypeDef,
     ListAPIKeysRequestRequestTypeDef,
     ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef,
     ManagedRuleGroupVersionTypeDef,
     ListAvailableManagedRuleGroupsRequestRequestTypeDef,
     ManagedRuleGroupSummaryTypeDef,
     ListIPSetsRequestRequestTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
     ListManagedRuleSetsRequestRequestTypeDef,
     ManagedRuleSetSummaryTypeDef,
     ListMobileSdkReleasesRequestRequestTypeDef,
     ReleaseSummaryTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     ListResourcesForWebACLRequestRequestTypeDef,
-    ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
+    PasswordFieldOutputTypeDef,
+    UsernameFieldOutputTypeDef,
     PasswordFieldTypeDef,
     UsernameFieldTypeDef,
     ManagedRuleSetVersionTypeDef,
+    TagOutputTypeDef,
+    NotStatementOutputTypeDef,
     NotStatementTypeDef,
+    OrStatementOutputTypeDef,
     OrStatementTypeDef,
+    PhoneNumberFieldOutputTypeDef,
     PhoneNumberFieldTypeDef,
     VersionToPublishTypeDef,
-    PutManagedRuleSetVersionsResponseTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
+    RateLimitLabelNamespaceOutputTypeDef,
     RateLimitLabelNamespaceTypeDef,
+    RegexOutputTypeDef,
+    ResponseInspectionBodyContainsOutputTypeDef,
     ResponseInspectionBodyContainsTypeDef,
+    ResponseInspectionHeaderOutputTypeDef,
     ResponseInspectionHeaderTypeDef,
+    ResponseInspectionJsonOutputTypeDef,
     ResponseInspectionJsonTypeDef,
+    ResponseInspectionStatusCodeOutputTypeDef,
     ResponseInspectionStatusCodeTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
-    UpdateIPSetResponseTypeDef,
     UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
-    UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
-    UpdateRegexPatternSetResponseTypeDef,
-    UpdateRuleGroupResponseTypeDef,
-    UpdateWebACLResponseTypeDef,
-    ListAPIKeysResponseTypeDef,
+    AssociationConfigOutputTypeDef,
     AssociationConfigTypeDef,
+    RateLimitCookieOutputTypeDef,
+    RateLimitHeaderOutputTypeDef,
+    RateLimitQueryArgumentOutputTypeDef,
+    RateLimitQueryStringOutputTypeDef,
+    RateLimitUriPathOutputTypeDef,
     RateLimitCookieTypeDef,
     RateLimitHeaderTypeDef,
     RateLimitQueryArgumentTypeDef,
     RateLimitQueryStringTypeDef,
+    RateLimitUriPathTypeDef,
+    CaptchaConfigOutputTypeDef,
+    ChallengeConfigOutputTypeDef,
     CaptchaConfigTypeDef,
     ChallengeConfigTypeDef,
+    CheckCapacityResponseTypeDef,
+    CreateAPIKeyResponseTypeDef,
+    DeleteFirewallManagerRuleGroupsResponseTypeDef,
+    GenerateMobileSdkReleaseUrlResponseTypeDef,
+    GetDecryptedAPIKeyResponseTypeDef,
+    GetPermissionPolicyResponseTypeDef,
+    ListAPIKeysResponseTypeDef,
+    ListResourcesForWebACLResponseTypeDef,
+    PutManagedRuleSetVersionsResponseTypeDef,
+    UpdateIPSetResponseTypeDef,
+    UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
+    UpdateRegexPatternSetResponseTypeDef,
+    UpdateRuleGroupResponseTypeDef,
+    UpdateWebACLResponseTypeDef,
+    ConditionOutputTypeDef,
     ConditionTypeDef,
+    CookiesOutputTypeDef,
     CookiesTypeDef,
     CreateIPSetRequestRequestTypeDef,
-    MobileSdkReleaseTypeDef,
-    TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIPSetResponseTypeDef,
     ListIPSetsResponseTypeDef,
     CreateRegexPatternSetRequestRequestTypeDef,
-    RegexPatternSetTypeDef,
     UpdateRegexPatternSetRequestRequestTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     ListRegexPatternSetsResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     CreateWebACLResponseTypeDef,
     ListWebACLsResponseTypeDef,
+    CustomRequestHandlingOutputTypeDef,
+    CustomResponseOutputTypeDef,
     CustomRequestHandlingTypeDef,
     CustomResponseTypeDef,
     DescribeAllManagedProductsResponseTypeDef,
     DescribeManagedProductsByVendorResponseTypeDef,
+    GeoMatchStatementOutputTypeDef,
     GeoMatchStatementTypeDef,
     GetIPSetResponseTypeDef,
     GetRateBasedStatementManagedKeysResponseTypeDef,
     GetSampledRequestsRequestRequestTypeDef,
     HTTPRequestTypeDef,
+    HeadersOutputTypeDef,
     HeadersTypeDef,
+    IPSetReferenceStatementOutputTypeDef,
     IPSetReferenceStatementTypeDef,
+    JsonBodyOutputTypeDef,
     JsonBodyTypeDef,
     ListAvailableManagedRuleGroupVersionsResponseTypeDef,
     ListAvailableManagedRuleGroupsResponseTypeDef,
     ListManagedRuleSetsResponseTypeDef,
     ListMobileSdkReleasesResponseTypeDef,
+    RequestInspectionOutputTypeDef,
     RequestInspectionTypeDef,
     ManagedRuleSetTypeDef,
+    MobileSdkReleaseTypeDef,
+    TagInfoForResourceTypeDef,
+    RequestInspectionACFPOutputTypeDef,
     RequestInspectionACFPTypeDef,
     PutManagedRuleSetVersionsRequestRequestTypeDef,
+    RegexPatternSetTypeDef,
+    ResponseInspectionOutputTypeDef,
     ResponseInspectionTypeDef,
+    RateBasedStatementCustomKeyOutputTypeDef,
     RateBasedStatementCustomKeyTypeDef,
+    FilterOutputTypeDef,
     FilterTypeDef,
-    GetMobileSdkReleaseResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    GetRegexPatternSetResponseTypeDef,
+    AllowActionOutputTypeDef,
+    CaptchaActionOutputTypeDef,
+    ChallengeActionOutputTypeDef,
+    CountActionOutputTypeDef,
+    BlockActionOutputTypeDef,
     AllowActionTypeDef,
     CaptchaActionTypeDef,
     ChallengeActionTypeDef,
     CountActionTypeDef,
     BlockActionTypeDef,
     SampledHTTPRequestTypeDef,
+    FieldToMatchOutputTypeDef,
     FieldToMatchTypeDef,
     GetManagedRuleSetResponseTypeDef,
+    GetMobileSdkReleaseResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    GetRegexPatternSetResponseTypeDef,
+    AWSManagedRulesACFPRuleSetOutputTypeDef,
+    AWSManagedRulesATPRuleSetOutputTypeDef,
     AWSManagedRulesACFPRuleSetTypeDef,
     AWSManagedRulesATPRuleSetTypeDef,
+    RateBasedStatementOutputTypeDef,
     RateBasedStatementTypeDef,
+    LoggingFilterOutputTypeDef,
     LoggingFilterTypeDef,
+    OverrideActionOutputTypeDef,
+    DefaultActionOutputTypeDef,
+    RuleActionOutputTypeDef,
     OverrideActionTypeDef,
     DefaultActionTypeDef,
     RuleActionTypeDef,
     GetSampledRequestsResponseTypeDef,
+    ByteMatchStatementOutputTypeDef,
+    RegexMatchStatementOutputTypeDef,
+    RegexPatternSetReferenceStatementOutputTypeDef,
+    SizeConstraintStatementOutputTypeDef,
+    SqliMatchStatementOutputTypeDef,
+    XssMatchStatementOutputTypeDef,
     ByteMatchStatementTypeDef,
     RegexMatchStatementTypeDef,
     RegexPatternSetReferenceStatementTypeDef,
     SizeConstraintStatementTypeDef,
     SqliMatchStatementTypeDef,
     XssMatchStatementTypeDef,
+    ManagedRuleGroupConfigOutputTypeDef,
     ManagedRuleGroupConfigTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
-    RuleActionOverrideTypeDef,
+    RuleActionOverrideOutputTypeDef,
+    RuleOutputTypeDef,
     RuleSummaryTypeDef,
+    RuleActionOverrideTypeDef,
     RuleTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
-    PutLoggingConfigurationRequestRequestTypeDef,
     PutLoggingConfigurationResponseTypeDef,
+    PutLoggingConfigurationRequestRequestTypeDef,
+    ManagedRuleGroupStatementOutputTypeDef,
+    RuleGroupReferenceStatementOutputTypeDef,
+    RuleGroupTypeDef,
+    DescribeManagedRuleGroupResponseTypeDef,
     ManagedRuleGroupStatementTypeDef,
     RuleGroupReferenceStatementTypeDef,
-    DescribeManagedRuleGroupResponseTypeDef,
     CheckCapacityRequestRequestTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     CreateWebACLRequestRequestTypeDef,
-    RuleGroupTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
     UpdateWebACLRequestRequestTypeDef,
     FirewallManagerStatementTypeDef,
-    StatementTypeDef,
+    StatementOutputTypeDef,
     GetRuleGroupResponseTypeDef,
+    StatementTypeDef,
     FirewallManagerRuleGroupTypeDef,
     WebACLTypeDef,
     GetWebACLForResourceResponseTypeDef,
     GetWebACLResponseTypeDef,
 )
```

### Comparing `mypy-boto3-wafv2-1.28.0/README.md` & `mypy-boto3-wafv2-1.28.12/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-wafv2"></a>
 
 # mypy-boto3-wafv2
 
 [![PyPI - mypy-boto3-wafv2](https://img.shields.io/pypi/v/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wafv2?color=blue)](https://pypistats.org/packages/mypy-boto3-wafv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wafv2)](https://pepy.tech/project/mypy-boto3-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[boto3.WAFV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
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
 [mypy-boto3-wafv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,217 +290,302 @@
 
 `mypy_boto3_wafv2.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_wafv2.type_defs import (
     APIKeySummaryTypeDef,
+    AWSManagedRulesBotControlRuleSetOutputTypeDef,
     AWSManagedRulesBotControlRuleSetTypeDef,
+    ActionConditionOutputTypeDef,
     ActionConditionTypeDef,
+    AddressFieldOutputTypeDef,
     AddressFieldTypeDef,
+    AndStatementOutputTypeDef,
     AndStatementTypeDef,
     AssociateWebACLRequestRequestTypeDef,
+    RequestBodyAssociatedResourceTypeConfigOutputTypeDef,
     RequestBodyAssociatedResourceTypeConfigTypeDef,
+    BodyOutputTypeDef,
     BodyTypeDef,
+    TextTransformationOutputTypeDef,
     TextTransformationTypeDef,
+    ImmunityTimePropertyOutputTypeDef,
     ImmunityTimePropertyTypeDef,
     CaptchaResponseTypeDef,
     ChallengeResponseTypeDef,
-    CheckCapacityResponseTypeDef,
+    ResponseMetadataTypeDef,
+    LabelNameConditionOutputTypeDef,
     LabelNameConditionTypeDef,
+    CookieMatchPatternOutputTypeDef,
     CookieMatchPatternTypeDef,
     CreateAPIKeyRequestRequestTypeDef,
-    CreateAPIKeyResponseTypeDef,
     TagTypeDef,
     IPSetSummaryTypeDef,
     RegexTypeDef,
     RegexPatternSetSummaryTypeDef,
     CustomResponseBodyTypeDef,
     VisibilityConfigTypeDef,
     RuleGroupSummaryTypeDef,
     WebACLSummaryTypeDef,
+    CustomHTTPHeaderOutputTypeDef,
     CustomHTTPHeaderTypeDef,
+    CustomResponseBodyOutputTypeDef,
     DeleteFirewallManagerRuleGroupsRequestRequestTypeDef,
-    DeleteFirewallManagerRuleGroupsResponseTypeDef,
     DeleteIPSetRequestRequestTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeletePermissionPolicyRequestRequestTypeDef,
     DeleteRegexPatternSetRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteWebACLRequestRequestTypeDef,
     DescribeAllManagedProductsRequestRequestTypeDef,
     ManagedProductDescriptorTypeDef,
     DescribeManagedProductsByVendorRequestRequestTypeDef,
     DescribeManagedRuleGroupRequestRequestTypeDef,
     LabelSummaryTypeDef,
     DisassociateWebACLRequestRequestTypeDef,
+    EmailFieldOutputTypeDef,
     EmailFieldTypeDef,
+    ExcludedRuleOutputTypeDef,
     ExcludedRuleTypeDef,
+    HeaderOrderOutputTypeDef,
+    SingleHeaderOutputTypeDef,
+    SingleQueryArgumentOutputTypeDef,
     HeaderOrderTypeDef,
     SingleHeaderTypeDef,
     SingleQueryArgumentTypeDef,
+    VisibilityConfigOutputTypeDef,
+    ForwardedIPConfigOutputTypeDef,
     ForwardedIPConfigTypeDef,
     GenerateMobileSdkReleaseUrlRequestRequestTypeDef,
-    GenerateMobileSdkReleaseUrlResponseTypeDef,
     GetDecryptedAPIKeyRequestRequestTypeDef,
-    GetDecryptedAPIKeyResponseTypeDef,
     GetIPSetRequestRequestTypeDef,
     IPSetTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetManagedRuleSetRequestRequestTypeDef,
     GetMobileSdkReleaseRequestRequestTypeDef,
     GetPermissionPolicyRequestRequestTypeDef,
-    GetPermissionPolicyResponseTypeDef,
     GetRateBasedStatementManagedKeysRequestRequestTypeDef,
     RateBasedStatementManagedKeysIPSetTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
     TimeWindowTypeDef,
+    TimeWindowOutputTypeDef,
     GetWebACLForResourceRequestRequestTypeDef,
     GetWebACLRequestRequestTypeDef,
     HTTPHeaderTypeDef,
+    HeaderMatchPatternOutputTypeDef,
     HeaderMatchPatternTypeDef,
+    IPSetForwardedIPConfigOutputTypeDef,
     IPSetForwardedIPConfigTypeDef,
+    JsonMatchPatternOutputTypeDef,
     JsonMatchPatternTypeDef,
+    LabelMatchStatementOutputTypeDef,
     LabelMatchStatementTypeDef,
+    LabelOutputTypeDef,
     LabelTypeDef,
     ListAPIKeysRequestRequestTypeDef,
     ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef,
     ManagedRuleGroupVersionTypeDef,
     ListAvailableManagedRuleGroupsRequestRequestTypeDef,
     ManagedRuleGroupSummaryTypeDef,
     ListIPSetsRequestRequestTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
     ListManagedRuleSetsRequestRequestTypeDef,
     ManagedRuleSetSummaryTypeDef,
     ListMobileSdkReleasesRequestRequestTypeDef,
     ReleaseSummaryTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     ListResourcesForWebACLRequestRequestTypeDef,
-    ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
+    PasswordFieldOutputTypeDef,
+    UsernameFieldOutputTypeDef,
     PasswordFieldTypeDef,
     UsernameFieldTypeDef,
     ManagedRuleSetVersionTypeDef,
+    TagOutputTypeDef,
+    NotStatementOutputTypeDef,
     NotStatementTypeDef,
+    OrStatementOutputTypeDef,
     OrStatementTypeDef,
+    PhoneNumberFieldOutputTypeDef,
     PhoneNumberFieldTypeDef,
     VersionToPublishTypeDef,
-    PutManagedRuleSetVersionsResponseTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
+    RateLimitLabelNamespaceOutputTypeDef,
     RateLimitLabelNamespaceTypeDef,
+    RegexOutputTypeDef,
+    ResponseInspectionBodyContainsOutputTypeDef,
     ResponseInspectionBodyContainsTypeDef,
+    ResponseInspectionHeaderOutputTypeDef,
     ResponseInspectionHeaderTypeDef,
+    ResponseInspectionJsonOutputTypeDef,
     ResponseInspectionJsonTypeDef,
+    ResponseInspectionStatusCodeOutputTypeDef,
     ResponseInspectionStatusCodeTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
-    UpdateIPSetResponseTypeDef,
     UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
-    UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
-    UpdateRegexPatternSetResponseTypeDef,
-    UpdateRuleGroupResponseTypeDef,
-    UpdateWebACLResponseTypeDef,
-    ListAPIKeysResponseTypeDef,
+    AssociationConfigOutputTypeDef,
     AssociationConfigTypeDef,
+    RateLimitCookieOutputTypeDef,
+    RateLimitHeaderOutputTypeDef,
+    RateLimitQueryArgumentOutputTypeDef,
+    RateLimitQueryStringOutputTypeDef,
+    RateLimitUriPathOutputTypeDef,
     RateLimitCookieTypeDef,
     RateLimitHeaderTypeDef,
     RateLimitQueryArgumentTypeDef,
     RateLimitQueryStringTypeDef,
+    RateLimitUriPathTypeDef,
+    CaptchaConfigOutputTypeDef,
+    ChallengeConfigOutputTypeDef,
     CaptchaConfigTypeDef,
     ChallengeConfigTypeDef,
+    CheckCapacityResponseTypeDef,
+    CreateAPIKeyResponseTypeDef,
+    DeleteFirewallManagerRuleGroupsResponseTypeDef,
+    GenerateMobileSdkReleaseUrlResponseTypeDef,
+    GetDecryptedAPIKeyResponseTypeDef,
+    GetPermissionPolicyResponseTypeDef,
+    ListAPIKeysResponseTypeDef,
+    ListResourcesForWebACLResponseTypeDef,
+    PutManagedRuleSetVersionsResponseTypeDef,
+    UpdateIPSetResponseTypeDef,
+    UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
+    UpdateRegexPatternSetResponseTypeDef,
+    UpdateRuleGroupResponseTypeDef,
+    UpdateWebACLResponseTypeDef,
+    ConditionOutputTypeDef,
     ConditionTypeDef,
+    CookiesOutputTypeDef,
     CookiesTypeDef,
     CreateIPSetRequestRequestTypeDef,
-    MobileSdkReleaseTypeDef,
-    TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIPSetResponseTypeDef,
     ListIPSetsResponseTypeDef,
     CreateRegexPatternSetRequestRequestTypeDef,
-    RegexPatternSetTypeDef,
     UpdateRegexPatternSetRequestRequestTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     ListRegexPatternSetsResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     CreateWebACLResponseTypeDef,
     ListWebACLsResponseTypeDef,
+    CustomRequestHandlingOutputTypeDef,
+    CustomResponseOutputTypeDef,
     CustomRequestHandlingTypeDef,
     CustomResponseTypeDef,
     DescribeAllManagedProductsResponseTypeDef,
     DescribeManagedProductsByVendorResponseTypeDef,
+    GeoMatchStatementOutputTypeDef,
     GeoMatchStatementTypeDef,
     GetIPSetResponseTypeDef,
     GetRateBasedStatementManagedKeysResponseTypeDef,
     GetSampledRequestsRequestRequestTypeDef,
     HTTPRequestTypeDef,
+    HeadersOutputTypeDef,
     HeadersTypeDef,
+    IPSetReferenceStatementOutputTypeDef,
     IPSetReferenceStatementTypeDef,
+    JsonBodyOutputTypeDef,
     JsonBodyTypeDef,
     ListAvailableManagedRuleGroupVersionsResponseTypeDef,
     ListAvailableManagedRuleGroupsResponseTypeDef,
     ListManagedRuleSetsResponseTypeDef,
     ListMobileSdkReleasesResponseTypeDef,
+    RequestInspectionOutputTypeDef,
     RequestInspectionTypeDef,
     ManagedRuleSetTypeDef,
+    MobileSdkReleaseTypeDef,
+    TagInfoForResourceTypeDef,
+    RequestInspectionACFPOutputTypeDef,
     RequestInspectionACFPTypeDef,
     PutManagedRuleSetVersionsRequestRequestTypeDef,
+    RegexPatternSetTypeDef,
+    ResponseInspectionOutputTypeDef,
     ResponseInspectionTypeDef,
+    RateBasedStatementCustomKeyOutputTypeDef,
     RateBasedStatementCustomKeyTypeDef,
+    FilterOutputTypeDef,
     FilterTypeDef,
-    GetMobileSdkReleaseResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    GetRegexPatternSetResponseTypeDef,
+    AllowActionOutputTypeDef,
+    CaptchaActionOutputTypeDef,
+    ChallengeActionOutputTypeDef,
+    CountActionOutputTypeDef,
+    BlockActionOutputTypeDef,
     AllowActionTypeDef,
     CaptchaActionTypeDef,
     ChallengeActionTypeDef,
     CountActionTypeDef,
     BlockActionTypeDef,
     SampledHTTPRequestTypeDef,
+    FieldToMatchOutputTypeDef,
     FieldToMatchTypeDef,
     GetManagedRuleSetResponseTypeDef,
+    GetMobileSdkReleaseResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    GetRegexPatternSetResponseTypeDef,
+    AWSManagedRulesACFPRuleSetOutputTypeDef,
+    AWSManagedRulesATPRuleSetOutputTypeDef,
     AWSManagedRulesACFPRuleSetTypeDef,
     AWSManagedRulesATPRuleSetTypeDef,
+    RateBasedStatementOutputTypeDef,
     RateBasedStatementTypeDef,
+    LoggingFilterOutputTypeDef,
     LoggingFilterTypeDef,
+    OverrideActionOutputTypeDef,
+    DefaultActionOutputTypeDef,
+    RuleActionOutputTypeDef,
     OverrideActionTypeDef,
     DefaultActionTypeDef,
     RuleActionTypeDef,
     GetSampledRequestsResponseTypeDef,
+    ByteMatchStatementOutputTypeDef,
+    RegexMatchStatementOutputTypeDef,
+    RegexPatternSetReferenceStatementOutputTypeDef,
+    SizeConstraintStatementOutputTypeDef,
+    SqliMatchStatementOutputTypeDef,
+    XssMatchStatementOutputTypeDef,
     ByteMatchStatementTypeDef,
     RegexMatchStatementTypeDef,
     RegexPatternSetReferenceStatementTypeDef,
     SizeConstraintStatementTypeDef,
     SqliMatchStatementTypeDef,
     XssMatchStatementTypeDef,
+    ManagedRuleGroupConfigOutputTypeDef,
     ManagedRuleGroupConfigTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
-    RuleActionOverrideTypeDef,
+    RuleActionOverrideOutputTypeDef,
+    RuleOutputTypeDef,
     RuleSummaryTypeDef,
+    RuleActionOverrideTypeDef,
     RuleTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
-    PutLoggingConfigurationRequestRequestTypeDef,
     PutLoggingConfigurationResponseTypeDef,
+    PutLoggingConfigurationRequestRequestTypeDef,
+    ManagedRuleGroupStatementOutputTypeDef,
+    RuleGroupReferenceStatementOutputTypeDef,
+    RuleGroupTypeDef,
+    DescribeManagedRuleGroupResponseTypeDef,
     ManagedRuleGroupStatementTypeDef,
     RuleGroupReferenceStatementTypeDef,
-    DescribeManagedRuleGroupResponseTypeDef,
     CheckCapacityRequestRequestTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     CreateWebACLRequestRequestTypeDef,
-    RuleGroupTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
     UpdateWebACLRequestRequestTypeDef,
     FirewallManagerStatementTypeDef,
-    StatementTypeDef,
+    StatementOutputTypeDef,
     GetRuleGroupResponseTypeDef,
+    StatementTypeDef,
     FirewallManagerRuleGroupTypeDef,
     WebACLTypeDef,
     GetWebACLForResourceResponseTypeDef,
     GetWebACLResponseTypeDef,
 )
```

### Comparing `mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/__main__.py` & `mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WAFV2 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.WAFV2 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2\nOther"
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

### Comparing `mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/client.py` & `mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/client.pyi` & `mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/literals.py` & `mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -479,14 +479,15 @@
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
@@ -565,26 +566,28 @@
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

### Comparing `mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/literals.pyi` & `mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -477,14 +477,15 @@
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
@@ -563,26 +564,28 @@
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

### Comparing `mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/type_defs.py` & `mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/type_defs.py`

 * *Files 26% similar despite different names*

```diff
@@ -53,217 +53,302 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "APIKeySummaryTypeDef",
+    "AWSManagedRulesBotControlRuleSetOutputTypeDef",
     "AWSManagedRulesBotControlRuleSetTypeDef",
+    "ActionConditionOutputTypeDef",
     "ActionConditionTypeDef",
+    "AddressFieldOutputTypeDef",
     "AddressFieldTypeDef",
+    "AndStatementOutputTypeDef",
     "AndStatementTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
+    "RequestBodyAssociatedResourceTypeConfigOutputTypeDef",
     "RequestBodyAssociatedResourceTypeConfigTypeDef",
+    "BodyOutputTypeDef",
     "BodyTypeDef",
+    "TextTransformationOutputTypeDef",
     "TextTransformationTypeDef",
+    "ImmunityTimePropertyOutputTypeDef",
     "ImmunityTimePropertyTypeDef",
     "CaptchaResponseTypeDef",
     "ChallengeResponseTypeDef",
-    "CheckCapacityResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "LabelNameConditionOutputTypeDef",
     "LabelNameConditionTypeDef",
+    "CookieMatchPatternOutputTypeDef",
     "CookieMatchPatternTypeDef",
     "CreateAPIKeyRequestRequestTypeDef",
-    "CreateAPIKeyResponseTypeDef",
     "TagTypeDef",
     "IPSetSummaryTypeDef",
     "RegexTypeDef",
     "RegexPatternSetSummaryTypeDef",
     "CustomResponseBodyTypeDef",
     "VisibilityConfigTypeDef",
     "RuleGroupSummaryTypeDef",
     "WebACLSummaryTypeDef",
+    "CustomHTTPHeaderOutputTypeDef",
     "CustomHTTPHeaderTypeDef",
+    "CustomResponseBodyOutputTypeDef",
     "DeleteFirewallManagerRuleGroupsRequestRequestTypeDef",
-    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
     "DeleteIPSetRequestRequestTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeletePermissionPolicyRequestRequestTypeDef",
     "DeleteRegexPatternSetRequestRequestTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
     "DeleteWebACLRequestRequestTypeDef",
     "DescribeAllManagedProductsRequestRequestTypeDef",
     "ManagedProductDescriptorTypeDef",
     "DescribeManagedProductsByVendorRequestRequestTypeDef",
     "DescribeManagedRuleGroupRequestRequestTypeDef",
     "LabelSummaryTypeDef",
     "DisassociateWebACLRequestRequestTypeDef",
+    "EmailFieldOutputTypeDef",
     "EmailFieldTypeDef",
+    "ExcludedRuleOutputTypeDef",
     "ExcludedRuleTypeDef",
+    "HeaderOrderOutputTypeDef",
+    "SingleHeaderOutputTypeDef",
+    "SingleQueryArgumentOutputTypeDef",
     "HeaderOrderTypeDef",
     "SingleHeaderTypeDef",
     "SingleQueryArgumentTypeDef",
+    "VisibilityConfigOutputTypeDef",
+    "ForwardedIPConfigOutputTypeDef",
     "ForwardedIPConfigTypeDef",
     "GenerateMobileSdkReleaseUrlRequestRequestTypeDef",
-    "GenerateMobileSdkReleaseUrlResponseTypeDef",
     "GetDecryptedAPIKeyRequestRequestTypeDef",
-    "GetDecryptedAPIKeyResponseTypeDef",
     "GetIPSetRequestRequestTypeDef",
     "IPSetTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
     "GetManagedRuleSetRequestRequestTypeDef",
     "GetMobileSdkReleaseRequestRequestTypeDef",
     "GetPermissionPolicyRequestRequestTypeDef",
-    "GetPermissionPolicyResponseTypeDef",
     "GetRateBasedStatementManagedKeysRequestRequestTypeDef",
     "RateBasedStatementManagedKeysIPSetTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
     "TimeWindowTypeDef",
+    "TimeWindowOutputTypeDef",
     "GetWebACLForResourceRequestRequestTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
+    "HeaderMatchPatternOutputTypeDef",
     "HeaderMatchPatternTypeDef",
+    "IPSetForwardedIPConfigOutputTypeDef",
     "IPSetForwardedIPConfigTypeDef",
+    "JsonMatchPatternOutputTypeDef",
     "JsonMatchPatternTypeDef",
+    "LabelMatchStatementOutputTypeDef",
     "LabelMatchStatementTypeDef",
+    "LabelOutputTypeDef",
     "LabelTypeDef",
     "ListAPIKeysRequestRequestTypeDef",
     "ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef",
     "ManagedRuleGroupVersionTypeDef",
     "ListAvailableManagedRuleGroupsRequestRequestTypeDef",
     "ManagedRuleGroupSummaryTypeDef",
     "ListIPSetsRequestRequestTypeDef",
     "ListLoggingConfigurationsRequestRequestTypeDef",
     "ListManagedRuleSetsRequestRequestTypeDef",
     "ManagedRuleSetSummaryTypeDef",
     "ListMobileSdkReleasesRequestRequestTypeDef",
     "ReleaseSummaryTypeDef",
     "ListRegexPatternSetsRequestRequestTypeDef",
     "ListResourcesForWebACLRequestRequestTypeDef",
-    "ListResourcesForWebACLResponseTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
+    "PasswordFieldOutputTypeDef",
+    "UsernameFieldOutputTypeDef",
     "PasswordFieldTypeDef",
     "UsernameFieldTypeDef",
     "ManagedRuleSetVersionTypeDef",
+    "TagOutputTypeDef",
+    "NotStatementOutputTypeDef",
     "NotStatementTypeDef",
+    "OrStatementOutputTypeDef",
     "OrStatementTypeDef",
+    "PhoneNumberFieldOutputTypeDef",
     "PhoneNumberFieldTypeDef",
     "VersionToPublishTypeDef",
-    "PutManagedRuleSetVersionsResponseTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
+    "RateLimitLabelNamespaceOutputTypeDef",
     "RateLimitLabelNamespaceTypeDef",
+    "RegexOutputTypeDef",
+    "ResponseInspectionBodyContainsOutputTypeDef",
     "ResponseInspectionBodyContainsTypeDef",
+    "ResponseInspectionHeaderOutputTypeDef",
     "ResponseInspectionHeaderTypeDef",
+    "ResponseInspectionJsonOutputTypeDef",
     "ResponseInspectionJsonTypeDef",
+    "ResponseInspectionStatusCodeOutputTypeDef",
     "ResponseInspectionStatusCodeTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
-    "UpdateIPSetResponseTypeDef",
     "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
-    "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
-    "UpdateRegexPatternSetResponseTypeDef",
-    "UpdateRuleGroupResponseTypeDef",
-    "UpdateWebACLResponseTypeDef",
-    "ListAPIKeysResponseTypeDef",
+    "AssociationConfigOutputTypeDef",
     "AssociationConfigTypeDef",
+    "RateLimitCookieOutputTypeDef",
+    "RateLimitHeaderOutputTypeDef",
+    "RateLimitQueryArgumentOutputTypeDef",
+    "RateLimitQueryStringOutputTypeDef",
+    "RateLimitUriPathOutputTypeDef",
     "RateLimitCookieTypeDef",
     "RateLimitHeaderTypeDef",
     "RateLimitQueryArgumentTypeDef",
     "RateLimitQueryStringTypeDef",
+    "RateLimitUriPathTypeDef",
+    "CaptchaConfigOutputTypeDef",
+    "ChallengeConfigOutputTypeDef",
     "CaptchaConfigTypeDef",
     "ChallengeConfigTypeDef",
+    "CheckCapacityResponseTypeDef",
+    "CreateAPIKeyResponseTypeDef",
+    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
+    "GenerateMobileSdkReleaseUrlResponseTypeDef",
+    "GetDecryptedAPIKeyResponseTypeDef",
+    "GetPermissionPolicyResponseTypeDef",
+    "ListAPIKeysResponseTypeDef",
+    "ListResourcesForWebACLResponseTypeDef",
+    "PutManagedRuleSetVersionsResponseTypeDef",
+    "UpdateIPSetResponseTypeDef",
+    "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
+    "UpdateRegexPatternSetResponseTypeDef",
+    "UpdateRuleGroupResponseTypeDef",
+    "UpdateWebACLResponseTypeDef",
+    "ConditionOutputTypeDef",
     "ConditionTypeDef",
+    "CookiesOutputTypeDef",
     "CookiesTypeDef",
     "CreateIPSetRequestRequestTypeDef",
-    "MobileSdkReleaseTypeDef",
-    "TagInfoForResourceTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIPSetResponseTypeDef",
     "ListIPSetsResponseTypeDef",
     "CreateRegexPatternSetRequestRequestTypeDef",
-    "RegexPatternSetTypeDef",
     "UpdateRegexPatternSetRequestRequestTypeDef",
     "CreateRegexPatternSetResponseTypeDef",
     "ListRegexPatternSetsResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "ListRuleGroupsResponseTypeDef",
     "CreateWebACLResponseTypeDef",
     "ListWebACLsResponseTypeDef",
+    "CustomRequestHandlingOutputTypeDef",
+    "CustomResponseOutputTypeDef",
     "CustomRequestHandlingTypeDef",
     "CustomResponseTypeDef",
     "DescribeAllManagedProductsResponseTypeDef",
     "DescribeManagedProductsByVendorResponseTypeDef",
+    "GeoMatchStatementOutputTypeDef",
     "GeoMatchStatementTypeDef",
     "GetIPSetResponseTypeDef",
     "GetRateBasedStatementManagedKeysResponseTypeDef",
     "GetSampledRequestsRequestRequestTypeDef",
     "HTTPRequestTypeDef",
+    "HeadersOutputTypeDef",
     "HeadersTypeDef",
+    "IPSetReferenceStatementOutputTypeDef",
     "IPSetReferenceStatementTypeDef",
+    "JsonBodyOutputTypeDef",
     "JsonBodyTypeDef",
     "ListAvailableManagedRuleGroupVersionsResponseTypeDef",
     "ListAvailableManagedRuleGroupsResponseTypeDef",
     "ListManagedRuleSetsResponseTypeDef",
     "ListMobileSdkReleasesResponseTypeDef",
+    "RequestInspectionOutputTypeDef",
     "RequestInspectionTypeDef",
     "ManagedRuleSetTypeDef",
+    "MobileSdkReleaseTypeDef",
+    "TagInfoForResourceTypeDef",
+    "RequestInspectionACFPOutputTypeDef",
     "RequestInspectionACFPTypeDef",
     "PutManagedRuleSetVersionsRequestRequestTypeDef",
+    "RegexPatternSetTypeDef",
+    "ResponseInspectionOutputTypeDef",
     "ResponseInspectionTypeDef",
+    "RateBasedStatementCustomKeyOutputTypeDef",
     "RateBasedStatementCustomKeyTypeDef",
+    "FilterOutputTypeDef",
     "FilterTypeDef",
-    "GetMobileSdkReleaseResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "GetRegexPatternSetResponseTypeDef",
+    "AllowActionOutputTypeDef",
+    "CaptchaActionOutputTypeDef",
+    "ChallengeActionOutputTypeDef",
+    "CountActionOutputTypeDef",
+    "BlockActionOutputTypeDef",
     "AllowActionTypeDef",
     "CaptchaActionTypeDef",
     "ChallengeActionTypeDef",
     "CountActionTypeDef",
     "BlockActionTypeDef",
     "SampledHTTPRequestTypeDef",
+    "FieldToMatchOutputTypeDef",
     "FieldToMatchTypeDef",
     "GetManagedRuleSetResponseTypeDef",
+    "GetMobileSdkReleaseResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "GetRegexPatternSetResponseTypeDef",
+    "AWSManagedRulesACFPRuleSetOutputTypeDef",
+    "AWSManagedRulesATPRuleSetOutputTypeDef",
     "AWSManagedRulesACFPRuleSetTypeDef",
     "AWSManagedRulesATPRuleSetTypeDef",
+    "RateBasedStatementOutputTypeDef",
     "RateBasedStatementTypeDef",
+    "LoggingFilterOutputTypeDef",
     "LoggingFilterTypeDef",
+    "OverrideActionOutputTypeDef",
+    "DefaultActionOutputTypeDef",
+    "RuleActionOutputTypeDef",
     "OverrideActionTypeDef",
     "DefaultActionTypeDef",
     "RuleActionTypeDef",
     "GetSampledRequestsResponseTypeDef",
+    "ByteMatchStatementOutputTypeDef",
+    "RegexMatchStatementOutputTypeDef",
+    "RegexPatternSetReferenceStatementOutputTypeDef",
+    "SizeConstraintStatementOutputTypeDef",
+    "SqliMatchStatementOutputTypeDef",
+    "XssMatchStatementOutputTypeDef",
     "ByteMatchStatementTypeDef",
     "RegexMatchStatementTypeDef",
     "RegexPatternSetReferenceStatementTypeDef",
     "SizeConstraintStatementTypeDef",
     "SqliMatchStatementTypeDef",
     "XssMatchStatementTypeDef",
+    "ManagedRuleGroupConfigOutputTypeDef",
     "ManagedRuleGroupConfigTypeDef",
+    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
-    "RuleActionOverrideTypeDef",
+    "RuleActionOverrideOutputTypeDef",
+    "RuleOutputTypeDef",
     "RuleSummaryTypeDef",
+    "RuleActionOverrideTypeDef",
     "RuleTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
-    "PutLoggingConfigurationRequestRequestTypeDef",
     "PutLoggingConfigurationResponseTypeDef",
+    "PutLoggingConfigurationRequestRequestTypeDef",
+    "ManagedRuleGroupStatementOutputTypeDef",
+    "RuleGroupReferenceStatementOutputTypeDef",
+    "RuleGroupTypeDef",
+    "DescribeManagedRuleGroupResponseTypeDef",
     "ManagedRuleGroupStatementTypeDef",
     "RuleGroupReferenceStatementTypeDef",
-    "DescribeManagedRuleGroupResponseTypeDef",
     "CheckCapacityRequestRequestTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
     "CreateWebACLRequestRequestTypeDef",
-    "RuleGroupTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
     "UpdateWebACLRequestRequestTypeDef",
     "FirewallManagerStatementTypeDef",
-    "StatementTypeDef",
+    "StatementOutputTypeDef",
     "GetRuleGroupResponseTypeDef",
+    "StatementTypeDef",
     "FirewallManagerRuleGroupTypeDef",
     "WebACLTypeDef",
     "GetWebACLForResourceResponseTypeDef",
     "GetWebACLResponseTypeDef",
 )
 
 APIKeySummaryTypeDef = TypedDict(
@@ -273,35 +358,63 @@
         "APIKey": str,
         "CreationTimestamp": datetime,
         "Version": int,
     },
     total=False,
 )
 
+AWSManagedRulesBotControlRuleSetOutputTypeDef = TypedDict(
+    "AWSManagedRulesBotControlRuleSetOutputTypeDef",
+    {
+        "InspectionLevel": InspectionLevelType,
+    },
+)
+
 AWSManagedRulesBotControlRuleSetTypeDef = TypedDict(
     "AWSManagedRulesBotControlRuleSetTypeDef",
     {
         "InspectionLevel": InspectionLevelType,
     },
 )
 
+ActionConditionOutputTypeDef = TypedDict(
+    "ActionConditionOutputTypeDef",
+    {
+        "Action": ActionValueType,
+    },
+)
+
 ActionConditionTypeDef = TypedDict(
     "ActionConditionTypeDef",
     {
         "Action": ActionValueType,
     },
 )
 
+AddressFieldOutputTypeDef = TypedDict(
+    "AddressFieldOutputTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+
 AddressFieldTypeDef = TypedDict(
     "AddressFieldTypeDef",
     {
         "Identifier": str,
     },
 )
 
+AndStatementOutputTypeDef = TypedDict(
+    "AndStatementOutputTypeDef",
+    {
+        "Statements": List["StatementOutputTypeDef"],
+    },
+)
+
 AndStatementTypeDef = TypedDict(
     "AndStatementTypeDef",
     {
         "Statements": Sequence["StatementTypeDef"],
     },
 )
 
@@ -309,37 +422,67 @@
     "AssociateWebACLRequestRequestTypeDef",
     {
         "WebACLArn": str,
         "ResourceArn": str,
     },
 )
 
+RequestBodyAssociatedResourceTypeConfigOutputTypeDef = TypedDict(
+    "RequestBodyAssociatedResourceTypeConfigOutputTypeDef",
+    {
+        "DefaultSizeInspectionLimit": SizeInspectionLimitType,
+    },
+)
+
 RequestBodyAssociatedResourceTypeConfigTypeDef = TypedDict(
     "RequestBodyAssociatedResourceTypeConfigTypeDef",
     {
         "DefaultSizeInspectionLimit": SizeInspectionLimitType,
     },
 )
 
+BodyOutputTypeDef = TypedDict(
+    "BodyOutputTypeDef",
+    {
+        "OversizeHandling": OversizeHandlingType,
+    },
+    total=False,
+)
+
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "OversizeHandling": OversizeHandlingType,
     },
     total=False,
 )
 
+TextTransformationOutputTypeDef = TypedDict(
+    "TextTransformationOutputTypeDef",
+    {
+        "Priority": int,
+        "Type": TextTransformationTypeType,
+    },
+)
+
 TextTransformationTypeDef = TypedDict(
     "TextTransformationTypeDef",
     {
         "Priority": int,
         "Type": TextTransformationTypeType,
     },
 )
 
+ImmunityTimePropertyOutputTypeDef = TypedDict(
+    "ImmunityTimePropertyOutputTypeDef",
+    {
+        "ImmunityTime": int,
+    },
+)
+
 ImmunityTimePropertyTypeDef = TypedDict(
     "ImmunityTimePropertyTypeDef",
     {
         "ImmunityTime": int,
     },
 )
 
@@ -359,29 +502,49 @@
         "ResponseCode": int,
         "SolveTimestamp": int,
         "FailureReason": FailureReasonType,
     },
     total=False,
 )
 
-CheckCapacityResponseTypeDef = TypedDict(
-    "CheckCapacityResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Capacity": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+LabelNameConditionOutputTypeDef = TypedDict(
+    "LabelNameConditionOutputTypeDef",
+    {
+        "LabelName": str,
     },
 )
 
 LabelNameConditionTypeDef = TypedDict(
     "LabelNameConditionTypeDef",
     {
         "LabelName": str,
     },
 )
 
+CookieMatchPatternOutputTypeDef = TypedDict(
+    "CookieMatchPatternOutputTypeDef",
+    {
+        "All": Dict[str, Any],
+        "IncludedCookies": List[str],
+        "ExcludedCookies": List[str],
+    },
+    total=False,
+)
+
 CookieMatchPatternTypeDef = TypedDict(
     "CookieMatchPatternTypeDef",
     {
         "All": Mapping[str, Any],
         "IncludedCookies": Sequence[str],
         "ExcludedCookies": Sequence[str],
     },
@@ -392,22 +555,14 @@
     "CreateAPIKeyRequestRequestTypeDef",
     {
         "Scope": ScopeType,
         "TokenDomains": Sequence[str],
     },
 )
 
-CreateAPIKeyResponseTypeDef = TypedDict(
-    "CreateAPIKeyResponseTypeDef",
-    {
-        "APIKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -481,35 +636,43 @@
         "Description": str,
         "LockToken": str,
         "ARN": str,
     },
     total=False,
 )
 
+CustomHTTPHeaderOutputTypeDef = TypedDict(
+    "CustomHTTPHeaderOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
+
 CustomHTTPHeaderTypeDef = TypedDict(
     "CustomHTTPHeaderTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-DeleteFirewallManagerRuleGroupsRequestRequestTypeDef = TypedDict(
-    "DeleteFirewallManagerRuleGroupsRequestRequestTypeDef",
+CustomResponseBodyOutputTypeDef = TypedDict(
+    "CustomResponseBodyOutputTypeDef",
     {
-        "WebACLArn": str,
-        "WebACLLockToken": str,
+        "ContentType": ResponseContentTypeType,
+        "Content": str,
     },
 )
 
-DeleteFirewallManagerRuleGroupsResponseTypeDef = TypedDict(
-    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
+DeleteFirewallManagerRuleGroupsRequestRequestTypeDef = TypedDict(
+    "DeleteFirewallManagerRuleGroupsRequestRequestTypeDef",
     {
-        "NextWebACLLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "WebACLArn": str,
+        "WebACLLockToken": str,
     },
 )
 
 DeleteIPSetRequestRequestTypeDef = TypedDict(
     "DeleteIPSetRequestRequestTypeDef",
     {
         "Name": str,
@@ -629,28 +792,63 @@
 DisassociateWebACLRequestRequestTypeDef = TypedDict(
     "DisassociateWebACLRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+EmailFieldOutputTypeDef = TypedDict(
+    "EmailFieldOutputTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+
 EmailFieldTypeDef = TypedDict(
     "EmailFieldTypeDef",
     {
         "Identifier": str,
     },
 )
 
+ExcludedRuleOutputTypeDef = TypedDict(
+    "ExcludedRuleOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 ExcludedRuleTypeDef = TypedDict(
     "ExcludedRuleTypeDef",
     {
         "Name": str,
     },
 )
 
+HeaderOrderOutputTypeDef = TypedDict(
+    "HeaderOrderOutputTypeDef",
+    {
+        "OversizeHandling": OversizeHandlingType,
+    },
+)
+
+SingleHeaderOutputTypeDef = TypedDict(
+    "SingleHeaderOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+
+SingleQueryArgumentOutputTypeDef = TypedDict(
+    "SingleQueryArgumentOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 HeaderOrderTypeDef = TypedDict(
     "HeaderOrderTypeDef",
     {
         "OversizeHandling": OversizeHandlingType,
     },
 )
 
@@ -664,14 +862,31 @@
 SingleQueryArgumentTypeDef = TypedDict(
     "SingleQueryArgumentTypeDef",
     {
         "Name": str,
     },
 )
 
+VisibilityConfigOutputTypeDef = TypedDict(
+    "VisibilityConfigOutputTypeDef",
+    {
+        "SampledRequestsEnabled": bool,
+        "CloudWatchMetricsEnabled": bool,
+        "MetricName": str,
+    },
+)
+
+ForwardedIPConfigOutputTypeDef = TypedDict(
+    "ForwardedIPConfigOutputTypeDef",
+    {
+        "HeaderName": str,
+        "FallbackBehavior": FallbackBehaviorType,
+    },
+)
+
 ForwardedIPConfigTypeDef = TypedDict(
     "ForwardedIPConfigTypeDef",
     {
         "HeaderName": str,
         "FallbackBehavior": FallbackBehaviorType,
     },
 )
@@ -680,39 +895,22 @@
     "GenerateMobileSdkReleaseUrlRequestRequestTypeDef",
     {
         "Platform": PlatformType,
         "ReleaseVersion": str,
     },
 )
 
-GenerateMobileSdkReleaseUrlResponseTypeDef = TypedDict(
-    "GenerateMobileSdkReleaseUrlResponseTypeDef",
-    {
-        "Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDecryptedAPIKeyRequestRequestTypeDef = TypedDict(
     "GetDecryptedAPIKeyRequestRequestTypeDef",
     {
         "Scope": ScopeType,
         "APIKey": str,
     },
 )
 
-GetDecryptedAPIKeyResponseTypeDef = TypedDict(
-    "GetDecryptedAPIKeyResponseTypeDef",
-    {
-        "TokenDomains": List[str],
-        "CreationTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetIPSetRequestRequestTypeDef = TypedDict(
     "GetIPSetRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
     },
@@ -768,22 +966,14 @@
 GetPermissionPolicyRequestRequestTypeDef = TypedDict(
     "GetPermissionPolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetPermissionPolicyResponseTypeDef = TypedDict(
-    "GetPermissionPolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRateBasedStatementManagedKeysRequestRequestTypeDef = TypedDict(
     "_RequiredGetRateBasedStatementManagedKeysRequestRequestTypeDef",
     {
         "Scope": ScopeType,
         "WebACLName": str,
         "WebACLId": str,
         "RuleName": str,
@@ -838,14 +1028,22 @@
     "TimeWindowTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
 )
 
+TimeWindowOutputTypeDef = TypedDict(
+    "TimeWindowOutputTypeDef",
+    {
+        "StartTime": datetime,
+        "EndTime": datetime,
+    },
+)
+
 GetWebACLForResourceRequestRequestTypeDef = TypedDict(
     "GetWebACLForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -863,50 +1061,93 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
+HeaderMatchPatternOutputTypeDef = TypedDict(
+    "HeaderMatchPatternOutputTypeDef",
+    {
+        "All": Dict[str, Any],
+        "IncludedHeaders": List[str],
+        "ExcludedHeaders": List[str],
+    },
+    total=False,
+)
+
 HeaderMatchPatternTypeDef = TypedDict(
     "HeaderMatchPatternTypeDef",
     {
         "All": Mapping[str, Any],
         "IncludedHeaders": Sequence[str],
         "ExcludedHeaders": Sequence[str],
     },
     total=False,
 )
 
+IPSetForwardedIPConfigOutputTypeDef = TypedDict(
+    "IPSetForwardedIPConfigOutputTypeDef",
+    {
+        "HeaderName": str,
+        "FallbackBehavior": FallbackBehaviorType,
+        "Position": ForwardedIPPositionType,
+    },
+)
+
 IPSetForwardedIPConfigTypeDef = TypedDict(
     "IPSetForwardedIPConfigTypeDef",
     {
         "HeaderName": str,
         "FallbackBehavior": FallbackBehaviorType,
         "Position": ForwardedIPPositionType,
     },
 )
 
+JsonMatchPatternOutputTypeDef = TypedDict(
+    "JsonMatchPatternOutputTypeDef",
+    {
+        "All": Dict[str, Any],
+        "IncludedPaths": List[str],
+    },
+    total=False,
+)
+
 JsonMatchPatternTypeDef = TypedDict(
     "JsonMatchPatternTypeDef",
     {
         "All": Mapping[str, Any],
         "IncludedPaths": Sequence[str],
     },
     total=False,
 )
 
+LabelMatchStatementOutputTypeDef = TypedDict(
+    "LabelMatchStatementOutputTypeDef",
+    {
+        "Scope": LabelMatchScopeType,
+        "Key": str,
+    },
+)
+
 LabelMatchStatementTypeDef = TypedDict(
     "LabelMatchStatementTypeDef",
     {
         "Scope": LabelMatchScopeType,
         "Key": str,
     },
 )
 
+LabelOutputTypeDef = TypedDict(
+    "LabelOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 LabelTypeDef = TypedDict(
     "LabelTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1154,22 +1395,14 @@
 class ListResourcesForWebACLRequestRequestTypeDef(
     _RequiredListResourcesForWebACLRequestRequestTypeDef,
     _OptionalListResourcesForWebACLRequestRequestTypeDef,
 ):
     pass
 
 
-ListResourcesForWebACLResponseTypeDef = TypedDict(
-    "ListResourcesForWebACLResponseTypeDef",
-    {
-        "ResourceArns": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListRuleGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListRuleGroupsRequestRequestTypeDef",
     {
         "Scope": ScopeType,
     },
 )
 _OptionalListRuleGroupsRequestRequestTypeDef = TypedDict(
@@ -1229,14 +1462,28 @@
 
 class ListWebACLsRequestRequestTypeDef(
     _RequiredListWebACLsRequestRequestTypeDef, _OptionalListWebACLsRequestRequestTypeDef
 ):
     pass
 
 
+PasswordFieldOutputTypeDef = TypedDict(
+    "PasswordFieldOutputTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+
+UsernameFieldOutputTypeDef = TypedDict(
+    "UsernameFieldOutputTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+
 PasswordFieldTypeDef = TypedDict(
     "PasswordFieldTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -1256,28 +1503,57 @@
         "PublishTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
         "ExpiryTimestamp": datetime,
     },
     total=False,
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+NotStatementOutputTypeDef = TypedDict(
+    "NotStatementOutputTypeDef",
+    {
+        "Statement": "StatementOutputTypeDef",
+    },
+)
+
 NotStatementTypeDef = TypedDict(
     "NotStatementTypeDef",
     {
         "Statement": "StatementTypeDef",
     },
 )
 
+OrStatementOutputTypeDef = TypedDict(
+    "OrStatementOutputTypeDef",
+    {
+        "Statements": List["StatementOutputTypeDef"],
+    },
+)
+
 OrStatementTypeDef = TypedDict(
     "OrStatementTypeDef",
     {
         "Statements": Sequence[Dict[str, Any]],
     },
 )
 
+PhoneNumberFieldOutputTypeDef = TypedDict(
+    "PhoneNumberFieldOutputTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+
 PhoneNumberFieldTypeDef = TypedDict(
     "PhoneNumberFieldTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -1286,79 +1562,109 @@
     {
         "AssociatedRuleGroupArn": str,
         "ForecastedLifetime": int,
     },
     total=False,
 )
 
-PutManagedRuleSetVersionsResponseTypeDef = TypedDict(
-    "PutManagedRuleSetVersionsResponseTypeDef",
-    {
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutPermissionPolicyRequestRequestTypeDef = TypedDict(
     "PutPermissionPolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Policy": str,
     },
 )
 
+RateLimitLabelNamespaceOutputTypeDef = TypedDict(
+    "RateLimitLabelNamespaceOutputTypeDef",
+    {
+        "Namespace": str,
+    },
+)
+
 RateLimitLabelNamespaceTypeDef = TypedDict(
     "RateLimitLabelNamespaceTypeDef",
     {
         "Namespace": str,
     },
 )
 
+RegexOutputTypeDef = TypedDict(
+    "RegexOutputTypeDef",
+    {
+        "RegexString": str,
+    },
+    total=False,
+)
+
+ResponseInspectionBodyContainsOutputTypeDef = TypedDict(
+    "ResponseInspectionBodyContainsOutputTypeDef",
+    {
+        "SuccessStrings": List[str],
+        "FailureStrings": List[str],
+    },
+)
+
 ResponseInspectionBodyContainsTypeDef = TypedDict(
     "ResponseInspectionBodyContainsTypeDef",
     {
         "SuccessStrings": Sequence[str],
         "FailureStrings": Sequence[str],
     },
 )
 
+ResponseInspectionHeaderOutputTypeDef = TypedDict(
+    "ResponseInspectionHeaderOutputTypeDef",
+    {
+        "Name": str,
+        "SuccessValues": List[str],
+        "FailureValues": List[str],
+    },
+)
+
 ResponseInspectionHeaderTypeDef = TypedDict(
     "ResponseInspectionHeaderTypeDef",
     {
         "Name": str,
         "SuccessValues": Sequence[str],
         "FailureValues": Sequence[str],
     },
 )
 
+ResponseInspectionJsonOutputTypeDef = TypedDict(
+    "ResponseInspectionJsonOutputTypeDef",
+    {
+        "Identifier": str,
+        "SuccessValues": List[str],
+        "FailureValues": List[str],
+    },
+)
+
 ResponseInspectionJsonTypeDef = TypedDict(
     "ResponseInspectionJsonTypeDef",
     {
         "Identifier": str,
         "SuccessValues": Sequence[str],
         "FailureValues": Sequence[str],
     },
 )
 
-ResponseInspectionStatusCodeTypeDef = TypedDict(
-    "ResponseInspectionStatusCodeTypeDef",
+ResponseInspectionStatusCodeOutputTypeDef = TypedDict(
+    "ResponseInspectionStatusCodeOutputTypeDef",
     {
-        "SuccessCodes": Sequence[int],
-        "FailureCodes": Sequence[int],
+        "SuccessCodes": List[int],
+        "FailureCodes": List[int],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ResponseInspectionStatusCodeTypeDef = TypedDict(
+    "ResponseInspectionStatusCodeTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "SuccessCodes": Sequence[int],
+        "FailureCodes": Sequence[int],
     },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -1387,86 +1693,82 @@
 
 class UpdateIPSetRequestRequestTypeDef(
     _RequiredUpdateIPSetRequestRequestTypeDef, _OptionalUpdateIPSetRequestRequestTypeDef
 ):
     pass
 
 
-UpdateIPSetResponseTypeDef = TypedDict(
-    "UpdateIPSetResponseTypeDef",
-    {
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef = TypedDict(
     "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "LockToken": str,
         "VersionToExpire": str,
         "ExpiryTimestamp": Union[datetime, str],
     },
 )
 
-UpdateManagedRuleSetVersionExpiryDateResponseTypeDef = TypedDict(
-    "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
+AssociationConfigOutputTypeDef = TypedDict(
+    "AssociationConfigOutputTypeDef",
     {
-        "ExpiringVersion": str,
-        "ExpiryTimestamp": datetime,
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestBody": Dict[
+            Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigOutputTypeDef
+        ],
     },
+    total=False,
 )
 
-UpdateRegexPatternSetResponseTypeDef = TypedDict(
-    "UpdateRegexPatternSetResponseTypeDef",
+AssociationConfigTypeDef = TypedDict(
+    "AssociationConfigTypeDef",
     {
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestBody": Mapping[
+            Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef
+        ],
     },
+    total=False,
 )
 
-UpdateRuleGroupResponseTypeDef = TypedDict(
-    "UpdateRuleGroupResponseTypeDef",
+RateLimitCookieOutputTypeDef = TypedDict(
+    "RateLimitCookieOutputTypeDef",
     {
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
+        "TextTransformations": List[TextTransformationOutputTypeDef],
     },
 )
 
-UpdateWebACLResponseTypeDef = TypedDict(
-    "UpdateWebACLResponseTypeDef",
+RateLimitHeaderOutputTypeDef = TypedDict(
+    "RateLimitHeaderOutputTypeDef",
     {
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
+        "TextTransformations": List[TextTransformationOutputTypeDef],
     },
 )
 
-ListAPIKeysResponseTypeDef = TypedDict(
-    "ListAPIKeysResponseTypeDef",
+RateLimitQueryArgumentOutputTypeDef = TypedDict(
+    "RateLimitQueryArgumentOutputTypeDef",
     {
-        "NextMarker": str,
-        "APIKeySummaries": List[APIKeySummaryTypeDef],
-        "ApplicationIntegrationURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
+        "TextTransformations": List[TextTransformationOutputTypeDef],
     },
 )
 
-AssociationConfigTypeDef = TypedDict(
-    "AssociationConfigTypeDef",
+RateLimitQueryStringOutputTypeDef = TypedDict(
+    "RateLimitQueryStringOutputTypeDef",
     {
-        "RequestBody": Mapping[
-            Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef
-        ],
+        "TextTransformations": List[TextTransformationOutputTypeDef],
+    },
+)
+
+RateLimitUriPathOutputTypeDef = TypedDict(
+    "RateLimitUriPathOutputTypeDef",
+    {
+        "TextTransformations": List[TextTransformationOutputTypeDef],
     },
-    total=False,
 )
 
 RateLimitCookieTypeDef = TypedDict(
     "RateLimitCookieTypeDef",
     {
         "Name": str,
         "TextTransformations": Sequence[TextTransformationTypeDef],
@@ -1492,14 +1794,37 @@
 RateLimitQueryStringTypeDef = TypedDict(
     "RateLimitQueryStringTypeDef",
     {
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
+RateLimitUriPathTypeDef = TypedDict(
+    "RateLimitUriPathTypeDef",
+    {
+        "TextTransformations": Sequence[TextTransformationTypeDef],
+    },
+)
+
+CaptchaConfigOutputTypeDef = TypedDict(
+    "CaptchaConfigOutputTypeDef",
+    {
+        "ImmunityTimeProperty": ImmunityTimePropertyOutputTypeDef,
+    },
+    total=False,
+)
+
+ChallengeConfigOutputTypeDef = TypedDict(
+    "ChallengeConfigOutputTypeDef",
+    {
+        "ImmunityTimeProperty": ImmunityTimePropertyOutputTypeDef,
+    },
+    total=False,
+)
+
 CaptchaConfigTypeDef = TypedDict(
     "CaptchaConfigTypeDef",
     {
         "ImmunityTimeProperty": ImmunityTimePropertyTypeDef,
     },
     total=False,
 )
@@ -1508,23 +1833,158 @@
     "ChallengeConfigTypeDef",
     {
         "ImmunityTimeProperty": ImmunityTimePropertyTypeDef,
     },
     total=False,
 )
 
+CheckCapacityResponseTypeDef = TypedDict(
+    "CheckCapacityResponseTypeDef",
+    {
+        "Capacity": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAPIKeyResponseTypeDef = TypedDict(
+    "CreateAPIKeyResponseTypeDef",
+    {
+        "APIKey": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFirewallManagerRuleGroupsResponseTypeDef = TypedDict(
+    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
+    {
+        "NextWebACLLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateMobileSdkReleaseUrlResponseTypeDef = TypedDict(
+    "GenerateMobileSdkReleaseUrlResponseTypeDef",
+    {
+        "Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDecryptedAPIKeyResponseTypeDef = TypedDict(
+    "GetDecryptedAPIKeyResponseTypeDef",
+    {
+        "TokenDomains": List[str],
+        "CreationTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPermissionPolicyResponseTypeDef = TypedDict(
+    "GetPermissionPolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAPIKeysResponseTypeDef = TypedDict(
+    "ListAPIKeysResponseTypeDef",
+    {
+        "NextMarker": str,
+        "APIKeySummaries": List[APIKeySummaryTypeDef],
+        "ApplicationIntegrationURL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListResourcesForWebACLResponseTypeDef = TypedDict(
+    "ListResourcesForWebACLResponseTypeDef",
+    {
+        "ResourceArns": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutManagedRuleSetVersionsResponseTypeDef = TypedDict(
+    "PutManagedRuleSetVersionsResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateIPSetResponseTypeDef = TypedDict(
+    "UpdateIPSetResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateManagedRuleSetVersionExpiryDateResponseTypeDef = TypedDict(
+    "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
+    {
+        "ExpiringVersion": str,
+        "ExpiryTimestamp": datetime,
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRegexPatternSetResponseTypeDef = TypedDict(
+    "UpdateRegexPatternSetResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRuleGroupResponseTypeDef = TypedDict(
+    "UpdateRuleGroupResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWebACLResponseTypeDef = TypedDict(
+    "UpdateWebACLResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConditionOutputTypeDef = TypedDict(
+    "ConditionOutputTypeDef",
+    {
+        "ActionCondition": ActionConditionOutputTypeDef,
+        "LabelNameCondition": LabelNameConditionOutputTypeDef,
+    },
+    total=False,
+)
+
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "ActionCondition": ActionConditionTypeDef,
         "LabelNameCondition": LabelNameConditionTypeDef,
     },
     total=False,
 )
 
+CookiesOutputTypeDef = TypedDict(
+    "CookiesOutputTypeDef",
+    {
+        "MatchPattern": CookieMatchPatternOutputTypeDef,
+        "MatchScope": MapMatchScopeType,
+        "OversizeHandling": OversizeHandlingType,
+    },
+)
+
 CookiesTypeDef = TypedDict(
     "CookiesTypeDef",
     {
         "MatchPattern": CookieMatchPatternTypeDef,
         "MatchScope": MapMatchScopeType,
         "OversizeHandling": OversizeHandlingType,
     },
@@ -1551,56 +2011,36 @@
 
 class CreateIPSetRequestRequestTypeDef(
     _RequiredCreateIPSetRequestRequestTypeDef, _OptionalCreateIPSetRequestRequestTypeDef
 ):
     pass
 
 
-MobileSdkReleaseTypeDef = TypedDict(
-    "MobileSdkReleaseTypeDef",
-    {
-        "ReleaseVersion": str,
-        "Timestamp": datetime,
-        "ReleaseNotes": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-TagInfoForResourceTypeDef = TypedDict(
-    "TagInfoForResourceTypeDef",
-    {
-        "ResourceARN": str,
-        "TagList": List[TagTypeDef],
-    },
-    total=False,
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 CreateIPSetResponseTypeDef = TypedDict(
     "CreateIPSetResponseTypeDef",
     {
         "Summary": IPSetSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIPSetsResponseTypeDef = TypedDict(
     "ListIPSetsResponseTypeDef",
     {
         "NextMarker": str,
         "IPSets": List[IPSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateRegexPatternSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRegexPatternSetRequestRequestTypeDef",
     {
         "Name": str,
@@ -1621,26 +2061,14 @@
 class CreateRegexPatternSetRequestRequestTypeDef(
     _RequiredCreateRegexPatternSetRequestRequestTypeDef,
     _OptionalCreateRegexPatternSetRequestRequestTypeDef,
 ):
     pass
 
 
-RegexPatternSetTypeDef = TypedDict(
-    "RegexPatternSetTypeDef",
-    {
-        "Name": str,
-        "Id": str,
-        "ARN": str,
-        "Description": str,
-        "RegularExpressionList": List[RegexTypeDef],
-    },
-    total=False,
-)
-
 _RequiredUpdateRegexPatternSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRegexPatternSetRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "RegularExpressionList": Sequence[RegexTypeDef],
@@ -1663,61 +2091,90 @@
     pass
 
 
 CreateRegexPatternSetResponseTypeDef = TypedDict(
     "CreateRegexPatternSetResponseTypeDef",
     {
         "Summary": RegexPatternSetSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRegexPatternSetsResponseTypeDef = TypedDict(
     "ListRegexPatternSetsResponseTypeDef",
     {
         "NextMarker": str,
         "RegexPatternSets": List[RegexPatternSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRuleGroupResponseTypeDef = TypedDict(
     "CreateRuleGroupResponseTypeDef",
     {
         "Summary": RuleGroupSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRuleGroupsResponseTypeDef = TypedDict(
     "ListRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "RuleGroups": List[RuleGroupSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWebACLResponseTypeDef = TypedDict(
     "CreateWebACLResponseTypeDef",
     {
         "Summary": WebACLSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWebACLsResponseTypeDef = TypedDict(
     "ListWebACLsResponseTypeDef",
     {
         "NextMarker": str,
         "WebACLs": List[WebACLSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CustomRequestHandlingOutputTypeDef = TypedDict(
+    "CustomRequestHandlingOutputTypeDef",
+    {
+        "InsertHeaders": List[CustomHTTPHeaderOutputTypeDef],
     },
 )
 
+_RequiredCustomResponseOutputTypeDef = TypedDict(
+    "_RequiredCustomResponseOutputTypeDef",
+    {
+        "ResponseCode": int,
+    },
+)
+_OptionalCustomResponseOutputTypeDef = TypedDict(
+    "_OptionalCustomResponseOutputTypeDef",
+    {
+        "CustomResponseBodyKey": str,
+        "ResponseHeaders": List[CustomHTTPHeaderOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class CustomResponseOutputTypeDef(
+    _RequiredCustomResponseOutputTypeDef, _OptionalCustomResponseOutputTypeDef
+):
+    pass
+
+
 CustomRequestHandlingTypeDef = TypedDict(
     "CustomRequestHandlingTypeDef",
     {
         "InsertHeaders": Sequence[CustomHTTPHeaderTypeDef],
     },
 )
 
@@ -1741,24 +2198,33 @@
     pass
 
 
 DescribeAllManagedProductsResponseTypeDef = TypedDict(
     "DescribeAllManagedProductsResponseTypeDef",
     {
         "ManagedProducts": List[ManagedProductDescriptorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeManagedProductsByVendorResponseTypeDef = TypedDict(
     "DescribeManagedProductsByVendorResponseTypeDef",
     {
         "ManagedProducts": List[ManagedProductDescriptorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GeoMatchStatementOutputTypeDef = TypedDict(
+    "GeoMatchStatementOutputTypeDef",
+    {
+        "CountryCodes": List[CountryCodeType],
+        "ForwardedIPConfig": ForwardedIPConfigOutputTypeDef,
     },
+    total=False,
 )
 
 GeoMatchStatementTypeDef = TypedDict(
     "GeoMatchStatementTypeDef",
     {
         "CountryCodes": Sequence[CountryCodeType],
         "ForwardedIPConfig": ForwardedIPConfigTypeDef,
@@ -1767,24 +2233,24 @@
 )
 
 GetIPSetResponseTypeDef = TypedDict(
     "GetIPSetResponseTypeDef",
     {
         "IPSet": IPSetTypeDef,
         "LockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRateBasedStatementManagedKeysResponseTypeDef = TypedDict(
     "GetRateBasedStatementManagedKeysResponseTypeDef",
     {
         "ManagedKeysIPV4": RateBasedStatementManagedKeysIPSetTypeDef,
         "ManagedKeysIPV6": RateBasedStatementManagedKeysIPSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSampledRequestsRequestRequestTypeDef = TypedDict(
     "GetSampledRequestsRequestRequestTypeDef",
     {
         "WebAclArn": str,
@@ -1804,23 +2270,53 @@
         "Method": str,
         "HTTPVersion": str,
         "Headers": List[HTTPHeaderTypeDef],
     },
     total=False,
 )
 
+HeadersOutputTypeDef = TypedDict(
+    "HeadersOutputTypeDef",
+    {
+        "MatchPattern": HeaderMatchPatternOutputTypeDef,
+        "MatchScope": MapMatchScopeType,
+        "OversizeHandling": OversizeHandlingType,
+    },
+)
+
 HeadersTypeDef = TypedDict(
     "HeadersTypeDef",
     {
         "MatchPattern": HeaderMatchPatternTypeDef,
         "MatchScope": MapMatchScopeType,
         "OversizeHandling": OversizeHandlingType,
     },
 )
 
+_RequiredIPSetReferenceStatementOutputTypeDef = TypedDict(
+    "_RequiredIPSetReferenceStatementOutputTypeDef",
+    {
+        "ARN": str,
+    },
+)
+_OptionalIPSetReferenceStatementOutputTypeDef = TypedDict(
+    "_OptionalIPSetReferenceStatementOutputTypeDef",
+    {
+        "IPSetForwardedIPConfig": IPSetForwardedIPConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class IPSetReferenceStatementOutputTypeDef(
+    _RequiredIPSetReferenceStatementOutputTypeDef, _OptionalIPSetReferenceStatementOutputTypeDef
+):
+    pass
+
+
 _RequiredIPSetReferenceStatementTypeDef = TypedDict(
     "_RequiredIPSetReferenceStatementTypeDef",
     {
         "ARN": str,
     },
 )
 _OptionalIPSetReferenceStatementTypeDef = TypedDict(
@@ -1834,14 +2330,35 @@
 
 class IPSetReferenceStatementTypeDef(
     _RequiredIPSetReferenceStatementTypeDef, _OptionalIPSetReferenceStatementTypeDef
 ):
     pass
 
 
+_RequiredJsonBodyOutputTypeDef = TypedDict(
+    "_RequiredJsonBodyOutputTypeDef",
+    {
+        "MatchPattern": JsonMatchPatternOutputTypeDef,
+        "MatchScope": JsonMatchScopeType,
+    },
+)
+_OptionalJsonBodyOutputTypeDef = TypedDict(
+    "_OptionalJsonBodyOutputTypeDef",
+    {
+        "InvalidFallbackBehavior": BodyParsingFallbackBehaviorType,
+        "OversizeHandling": OversizeHandlingType,
+    },
+    total=False,
+)
+
+
+class JsonBodyOutputTypeDef(_RequiredJsonBodyOutputTypeDef, _OptionalJsonBodyOutputTypeDef):
+    pass
+
+
 _RequiredJsonBodyTypeDef = TypedDict(
     "_RequiredJsonBodyTypeDef",
     {
         "MatchPattern": JsonMatchPatternTypeDef,
         "MatchScope": JsonMatchScopeType,
     },
 )
@@ -1861,42 +2378,51 @@
 
 ListAvailableManagedRuleGroupVersionsResponseTypeDef = TypedDict(
     "ListAvailableManagedRuleGroupVersionsResponseTypeDef",
     {
         "NextMarker": str,
         "Versions": List[ManagedRuleGroupVersionTypeDef],
         "CurrentDefaultVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAvailableManagedRuleGroupsResponseTypeDef = TypedDict(
     "ListAvailableManagedRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "ManagedRuleGroups": List[ManagedRuleGroupSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListManagedRuleSetsResponseTypeDef = TypedDict(
     "ListManagedRuleSetsResponseTypeDef",
     {
         "NextMarker": str,
         "ManagedRuleSets": List[ManagedRuleSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMobileSdkReleasesResponseTypeDef = TypedDict(
     "ListMobileSdkReleasesResponseTypeDef",
     {
         "ReleaseSummaries": List[ReleaseSummaryTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RequestInspectionOutputTypeDef = TypedDict(
+    "RequestInspectionOutputTypeDef",
+    {
+        "PayloadType": PayloadTypeType,
+        "UsernameField": UsernameFieldOutputTypeDef,
+        "PasswordField": PasswordFieldOutputTypeDef,
     },
 )
 
 RequestInspectionTypeDef = TypedDict(
     "RequestInspectionTypeDef",
     {
         "PayloadType": PayloadTypeType,
@@ -1925,14 +2451,59 @@
 )
 
 
 class ManagedRuleSetTypeDef(_RequiredManagedRuleSetTypeDef, _OptionalManagedRuleSetTypeDef):
     pass
 
 
+MobileSdkReleaseTypeDef = TypedDict(
+    "MobileSdkReleaseTypeDef",
+    {
+        "ReleaseVersion": str,
+        "Timestamp": datetime,
+        "ReleaseNotes": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+TagInfoForResourceTypeDef = TypedDict(
+    "TagInfoForResourceTypeDef",
+    {
+        "ResourceARN": str,
+        "TagList": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+_RequiredRequestInspectionACFPOutputTypeDef = TypedDict(
+    "_RequiredRequestInspectionACFPOutputTypeDef",
+    {
+        "PayloadType": PayloadTypeType,
+    },
+)
+_OptionalRequestInspectionACFPOutputTypeDef = TypedDict(
+    "_OptionalRequestInspectionACFPOutputTypeDef",
+    {
+        "UsernameField": UsernameFieldOutputTypeDef,
+        "PasswordField": PasswordFieldOutputTypeDef,
+        "EmailField": EmailFieldOutputTypeDef,
+        "PhoneNumberFields": List[PhoneNumberFieldOutputTypeDef],
+        "AddressFields": List[AddressFieldOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class RequestInspectionACFPOutputTypeDef(
+    _RequiredRequestInspectionACFPOutputTypeDef, _OptionalRequestInspectionACFPOutputTypeDef
+):
+    pass
+
+
 _RequiredRequestInspectionACFPTypeDef = TypedDict(
     "_RequiredRequestInspectionACFPTypeDef",
     {
         "PayloadType": PayloadTypeType,
     },
 )
 _OptionalRequestInspectionACFPTypeDef = TypedDict(
@@ -1976,73 +2547,136 @@
 class PutManagedRuleSetVersionsRequestRequestTypeDef(
     _RequiredPutManagedRuleSetVersionsRequestRequestTypeDef,
     _OptionalPutManagedRuleSetVersionsRequestRequestTypeDef,
 ):
     pass
 
 
+RegexPatternSetTypeDef = TypedDict(
+    "RegexPatternSetTypeDef",
+    {
+        "Name": str,
+        "Id": str,
+        "ARN": str,
+        "Description": str,
+        "RegularExpressionList": List[RegexOutputTypeDef],
+    },
+    total=False,
+)
+
+ResponseInspectionOutputTypeDef = TypedDict(
+    "ResponseInspectionOutputTypeDef",
+    {
+        "StatusCode": ResponseInspectionStatusCodeOutputTypeDef,
+        "Header": ResponseInspectionHeaderOutputTypeDef,
+        "BodyContains": ResponseInspectionBodyContainsOutputTypeDef,
+        "Json": ResponseInspectionJsonOutputTypeDef,
+    },
+    total=False,
+)
+
 ResponseInspectionTypeDef = TypedDict(
     "ResponseInspectionTypeDef",
     {
         "StatusCode": ResponseInspectionStatusCodeTypeDef,
         "Header": ResponseInspectionHeaderTypeDef,
         "BodyContains": ResponseInspectionBodyContainsTypeDef,
         "Json": ResponseInspectionJsonTypeDef,
     },
     total=False,
 )
 
+RateBasedStatementCustomKeyOutputTypeDef = TypedDict(
+    "RateBasedStatementCustomKeyOutputTypeDef",
+    {
+        "Header": RateLimitHeaderOutputTypeDef,
+        "Cookie": RateLimitCookieOutputTypeDef,
+        "QueryArgument": RateLimitQueryArgumentOutputTypeDef,
+        "QueryString": RateLimitQueryStringOutputTypeDef,
+        "HTTPMethod": Dict[str, Any],
+        "ForwardedIP": Dict[str, Any],
+        "IP": Dict[str, Any],
+        "LabelNamespace": RateLimitLabelNamespaceOutputTypeDef,
+        "UriPath": RateLimitUriPathOutputTypeDef,
+    },
+    total=False,
+)
+
 RateBasedStatementCustomKeyTypeDef = TypedDict(
     "RateBasedStatementCustomKeyTypeDef",
     {
         "Header": RateLimitHeaderTypeDef,
         "Cookie": RateLimitCookieTypeDef,
         "QueryArgument": RateLimitQueryArgumentTypeDef,
         "QueryString": RateLimitQueryStringTypeDef,
         "HTTPMethod": Mapping[str, Any],
         "ForwardedIP": Mapping[str, Any],
         "IP": Mapping[str, Any],
         "LabelNamespace": RateLimitLabelNamespaceTypeDef,
+        "UriPath": RateLimitUriPathTypeDef,
     },
     total=False,
 )
 
+FilterOutputTypeDef = TypedDict(
+    "FilterOutputTypeDef",
+    {
+        "Behavior": FilterBehaviorType,
+        "Requirement": FilterRequirementType,
+        "Conditions": List[ConditionOutputTypeDef],
+    },
+)
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Behavior": FilterBehaviorType,
         "Requirement": FilterRequirementType,
-        "Conditions": List[ConditionTypeDef],
+        "Conditions": Sequence[ConditionTypeDef],
     },
 )
 
-GetMobileSdkReleaseResponseTypeDef = TypedDict(
-    "GetMobileSdkReleaseResponseTypeDef",
+AllowActionOutputTypeDef = TypedDict(
+    "AllowActionOutputTypeDef",
     {
-        "MobileSdkRelease": MobileSdkReleaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
     },
+    total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+CaptchaActionOutputTypeDef = TypedDict(
+    "CaptchaActionOutputTypeDef",
     {
-        "NextMarker": str,
-        "TagInfoForResource": TagInfoForResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
     },
+    total=False,
 )
 
-GetRegexPatternSetResponseTypeDef = TypedDict(
-    "GetRegexPatternSetResponseTypeDef",
+ChallengeActionOutputTypeDef = TypedDict(
+    "ChallengeActionOutputTypeDef",
     {
-        "RegexPatternSet": RegexPatternSetTypeDef,
-        "LockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
     },
+    total=False,
+)
+
+CountActionOutputTypeDef = TypedDict(
+    "CountActionOutputTypeDef",
+    {
+        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
+    },
+    total=False,
+)
+
+BlockActionOutputTypeDef = TypedDict(
+    "BlockActionOutputTypeDef",
+    {
+        "CustomResponse": CustomResponseOutputTypeDef,
+    },
+    total=False,
 )
 
 AllowActionTypeDef = TypedDict(
     "AllowActionTypeDef",
     {
         "CustomRequestHandling": CustomRequestHandlingTypeDef,
     },
@@ -2092,29 +2726,47 @@
     "_OptionalSampledHTTPRequestTypeDef",
     {
         "Timestamp": datetime,
         "Action": str,
         "RuleNameWithinRuleGroup": str,
         "RequestHeadersInserted": List[HTTPHeaderTypeDef],
         "ResponseCodeSent": int,
-        "Labels": List[LabelTypeDef],
+        "Labels": List[LabelOutputTypeDef],
         "CaptchaResponse": CaptchaResponseTypeDef,
         "ChallengeResponse": ChallengeResponseTypeDef,
         "OverriddenAction": str,
     },
     total=False,
 )
 
 
 class SampledHTTPRequestTypeDef(
     _RequiredSampledHTTPRequestTypeDef, _OptionalSampledHTTPRequestTypeDef
 ):
     pass
 
 
+FieldToMatchOutputTypeDef = TypedDict(
+    "FieldToMatchOutputTypeDef",
+    {
+        "SingleHeader": SingleHeaderOutputTypeDef,
+        "SingleQueryArgument": SingleQueryArgumentOutputTypeDef,
+        "AllQueryArguments": Dict[str, Any],
+        "UriPath": Dict[str, Any],
+        "QueryString": Dict[str, Any],
+        "Body": BodyOutputTypeDef,
+        "Method": Dict[str, Any],
+        "JsonBody": JsonBodyOutputTypeDef,
+        "Headers": HeadersOutputTypeDef,
+        "Cookies": CookiesOutputTypeDef,
+        "HeaderOrder": HeaderOrderOutputTypeDef,
+    },
+    total=False,
+)
+
 FieldToMatchTypeDef = TypedDict(
     "FieldToMatchTypeDef",
     {
         "SingleHeader": SingleHeaderTypeDef,
         "SingleQueryArgument": SingleQueryArgumentTypeDef,
         "AllQueryArguments": Mapping[str, Any],
         "UriPath": Mapping[str, Any],
@@ -2130,18 +2782,92 @@
 )
 
 GetManagedRuleSetResponseTypeDef = TypedDict(
     "GetManagedRuleSetResponseTypeDef",
     {
         "ManagedRuleSet": ManagedRuleSetTypeDef,
         "LockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMobileSdkReleaseResponseTypeDef = TypedDict(
+    "GetMobileSdkReleaseResponseTypeDef",
+    {
+        "MobileSdkRelease": MobileSdkReleaseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "NextMarker": str,
+        "TagInfoForResource": TagInfoForResourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRegexPatternSetResponseTypeDef = TypedDict(
+    "GetRegexPatternSetResponseTypeDef",
+    {
+        "RegexPatternSet": RegexPatternSetTypeDef,
+        "LockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredAWSManagedRulesACFPRuleSetOutputTypeDef = TypedDict(
+    "_RequiredAWSManagedRulesACFPRuleSetOutputTypeDef",
+    {
+        "CreationPath": str,
+        "RegistrationPagePath": str,
+        "RequestInspection": RequestInspectionACFPOutputTypeDef,
+    },
+)
+_OptionalAWSManagedRulesACFPRuleSetOutputTypeDef = TypedDict(
+    "_OptionalAWSManagedRulesACFPRuleSetOutputTypeDef",
+    {
+        "ResponseInspection": ResponseInspectionOutputTypeDef,
+        "EnableRegexInPath": bool,
+    },
+    total=False,
+)
+
+
+class AWSManagedRulesACFPRuleSetOutputTypeDef(
+    _RequiredAWSManagedRulesACFPRuleSetOutputTypeDef,
+    _OptionalAWSManagedRulesACFPRuleSetOutputTypeDef,
+):
+    pass
+
+
+_RequiredAWSManagedRulesATPRuleSetOutputTypeDef = TypedDict(
+    "_RequiredAWSManagedRulesATPRuleSetOutputTypeDef",
+    {
+        "LoginPath": str,
+    },
+)
+_OptionalAWSManagedRulesATPRuleSetOutputTypeDef = TypedDict(
+    "_OptionalAWSManagedRulesATPRuleSetOutputTypeDef",
+    {
+        "RequestInspection": RequestInspectionOutputTypeDef,
+        "ResponseInspection": ResponseInspectionOutputTypeDef,
+        "EnableRegexInPath": bool,
     },
+    total=False,
 )
 
+
+class AWSManagedRulesATPRuleSetOutputTypeDef(
+    _RequiredAWSManagedRulesATPRuleSetOutputTypeDef, _OptionalAWSManagedRulesATPRuleSetOutputTypeDef
+):
+    pass
+
+
 _RequiredAWSManagedRulesACFPRuleSetTypeDef = TypedDict(
     "_RequiredAWSManagedRulesACFPRuleSetTypeDef",
     {
         "CreationPath": str,
         "RegistrationPagePath": str,
         "RequestInspection": RequestInspectionACFPTypeDef,
     },
@@ -2181,14 +2907,38 @@
 
 class AWSManagedRulesATPRuleSetTypeDef(
     _RequiredAWSManagedRulesATPRuleSetTypeDef, _OptionalAWSManagedRulesATPRuleSetTypeDef
 ):
     pass
 
 
+_RequiredRateBasedStatementOutputTypeDef = TypedDict(
+    "_RequiredRateBasedStatementOutputTypeDef",
+    {
+        "Limit": int,
+        "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
+    },
+)
+_OptionalRateBasedStatementOutputTypeDef = TypedDict(
+    "_OptionalRateBasedStatementOutputTypeDef",
+    {
+        "ScopeDownStatement": "StatementOutputTypeDef",
+        "ForwardedIPConfig": ForwardedIPConfigOutputTypeDef,
+        "CustomKeys": List[RateBasedStatementCustomKeyOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class RateBasedStatementOutputTypeDef(
+    _RequiredRateBasedStatementOutputTypeDef, _OptionalRateBasedStatementOutputTypeDef
+):
+    pass
+
+
 _RequiredRateBasedStatementTypeDef = TypedDict(
     "_RequiredRateBasedStatementTypeDef",
     {
         "Limit": int,
         "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
     },
 )
@@ -2205,22 +2955,60 @@
 
 class RateBasedStatementTypeDef(
     _RequiredRateBasedStatementTypeDef, _OptionalRateBasedStatementTypeDef
 ):
     pass
 
 
+LoggingFilterOutputTypeDef = TypedDict(
+    "LoggingFilterOutputTypeDef",
+    {
+        "Filters": List[FilterOutputTypeDef],
+        "DefaultBehavior": FilterBehaviorType,
+    },
+)
+
 LoggingFilterTypeDef = TypedDict(
     "LoggingFilterTypeDef",
     {
-        "Filters": List[FilterTypeDef],
+        "Filters": Sequence[FilterTypeDef],
         "DefaultBehavior": FilterBehaviorType,
     },
 )
 
+OverrideActionOutputTypeDef = TypedDict(
+    "OverrideActionOutputTypeDef",
+    {
+        "Count": CountActionOutputTypeDef,
+        "None": Dict[str, Any],
+    },
+    total=False,
+)
+
+DefaultActionOutputTypeDef = TypedDict(
+    "DefaultActionOutputTypeDef",
+    {
+        "Block": BlockActionOutputTypeDef,
+        "Allow": AllowActionOutputTypeDef,
+    },
+    total=False,
+)
+
+RuleActionOutputTypeDef = TypedDict(
+    "RuleActionOutputTypeDef",
+    {
+        "Block": BlockActionOutputTypeDef,
+        "Allow": AllowActionOutputTypeDef,
+        "Count": CountActionOutputTypeDef,
+        "Captcha": CaptchaActionOutputTypeDef,
+        "Challenge": ChallengeActionOutputTypeDef,
+    },
+    total=False,
+)
+
 OverrideActionTypeDef = TypedDict(
     "OverrideActionTypeDef",
     {
         "Count": CountActionTypeDef,
         "None": Mapping[str, Any],
     },
     total=False,
@@ -2248,16 +3036,84 @@
 )
 
 GetSampledRequestsResponseTypeDef = TypedDict(
     "GetSampledRequestsResponseTypeDef",
     {
         "SampledRequests": List[SampledHTTPRequestTypeDef],
         "PopulationSize": int,
-        "TimeWindow": TimeWindowTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TimeWindow": TimeWindowOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ByteMatchStatementOutputTypeDef = TypedDict(
+    "ByteMatchStatementOutputTypeDef",
+    {
+        "SearchString": bytes,
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformations": List[TextTransformationOutputTypeDef],
+        "PositionalConstraint": PositionalConstraintType,
+    },
+)
+
+RegexMatchStatementOutputTypeDef = TypedDict(
+    "RegexMatchStatementOutputTypeDef",
+    {
+        "RegexString": str,
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformations": List[TextTransformationOutputTypeDef],
+    },
+)
+
+RegexPatternSetReferenceStatementOutputTypeDef = TypedDict(
+    "RegexPatternSetReferenceStatementOutputTypeDef",
+    {
+        "ARN": str,
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformations": List[TextTransformationOutputTypeDef],
+    },
+)
+
+SizeConstraintStatementOutputTypeDef = TypedDict(
+    "SizeConstraintStatementOutputTypeDef",
+    {
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "ComparisonOperator": ComparisonOperatorType,
+        "Size": int,
+        "TextTransformations": List[TextTransformationOutputTypeDef],
+    },
+)
+
+_RequiredSqliMatchStatementOutputTypeDef = TypedDict(
+    "_RequiredSqliMatchStatementOutputTypeDef",
+    {
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformations": List[TextTransformationOutputTypeDef],
+    },
+)
+_OptionalSqliMatchStatementOutputTypeDef = TypedDict(
+    "_OptionalSqliMatchStatementOutputTypeDef",
+    {
+        "SensitivityLevel": SensitivityLevelType,
+    },
+    total=False,
+)
+
+
+class SqliMatchStatementOutputTypeDef(
+    _RequiredSqliMatchStatementOutputTypeDef, _OptionalSqliMatchStatementOutputTypeDef
+):
+    pass
+
+
+XssMatchStatementOutputTypeDef = TypedDict(
+    "XssMatchStatementOutputTypeDef",
+    {
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformations": List[TextTransformationOutputTypeDef],
     },
 )
 
 ByteMatchStatementTypeDef = TypedDict(
     "ByteMatchStatementTypeDef",
     {
         "SearchString": Union[str, bytes, IO[Any], StreamingBody],
@@ -2321,69 +3177,141 @@
     "XssMatchStatementTypeDef",
     {
         "FieldToMatch": FieldToMatchTypeDef,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
+ManagedRuleGroupConfigOutputTypeDef = TypedDict(
+    "ManagedRuleGroupConfigOutputTypeDef",
+    {
+        "LoginPath": str,
+        "PayloadType": PayloadTypeType,
+        "UsernameField": UsernameFieldOutputTypeDef,
+        "PasswordField": PasswordFieldOutputTypeDef,
+        "AWSManagedRulesBotControlRuleSet": AWSManagedRulesBotControlRuleSetOutputTypeDef,
+        "AWSManagedRulesATPRuleSet": AWSManagedRulesATPRuleSetOutputTypeDef,
+        "AWSManagedRulesACFPRuleSet": AWSManagedRulesACFPRuleSetOutputTypeDef,
+    },
+    total=False,
+)
+
 ManagedRuleGroupConfigTypeDef = TypedDict(
     "ManagedRuleGroupConfigTypeDef",
     {
         "LoginPath": str,
         "PayloadType": PayloadTypeType,
         "UsernameField": UsernameFieldTypeDef,
         "PasswordField": PasswordFieldTypeDef,
         "AWSManagedRulesBotControlRuleSet": AWSManagedRulesBotControlRuleSetTypeDef,
         "AWSManagedRulesATPRuleSet": AWSManagedRulesATPRuleSetTypeDef,
         "AWSManagedRulesACFPRuleSet": AWSManagedRulesACFPRuleSetTypeDef,
     },
     total=False,
 )
 
+_RequiredLoggingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredLoggingConfigurationOutputTypeDef",
+    {
+        "ResourceArn": str,
+        "LogDestinationConfigs": List[str],
+    },
+)
+_OptionalLoggingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalLoggingConfigurationOutputTypeDef",
+    {
+        "RedactedFields": List[FieldToMatchOutputTypeDef],
+        "ManagedByFirewallManager": bool,
+        "LoggingFilter": LoggingFilterOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class LoggingConfigurationOutputTypeDef(
+    _RequiredLoggingConfigurationOutputTypeDef, _OptionalLoggingConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredLoggingConfigurationTypeDef = TypedDict(
     "_RequiredLoggingConfigurationTypeDef",
     {
         "ResourceArn": str,
-        "LogDestinationConfigs": List[str],
+        "LogDestinationConfigs": Sequence[str],
     },
 )
 _OptionalLoggingConfigurationTypeDef = TypedDict(
     "_OptionalLoggingConfigurationTypeDef",
     {
-        "RedactedFields": List[FieldToMatchTypeDef],
+        "RedactedFields": Sequence[FieldToMatchTypeDef],
         "ManagedByFirewallManager": bool,
         "LoggingFilter": LoggingFilterTypeDef,
     },
     total=False,
 )
 
 
 class LoggingConfigurationTypeDef(
     _RequiredLoggingConfigurationTypeDef, _OptionalLoggingConfigurationTypeDef
 ):
     pass
 
 
-RuleActionOverrideTypeDef = TypedDict(
-    "RuleActionOverrideTypeDef",
+RuleActionOverrideOutputTypeDef = TypedDict(
+    "RuleActionOverrideOutputTypeDef",
     {
         "Name": str,
-        "ActionToUse": RuleActionTypeDef,
+        "ActionToUse": RuleActionOutputTypeDef,
     },
 )
 
+_RequiredRuleOutputTypeDef = TypedDict(
+    "_RequiredRuleOutputTypeDef",
+    {
+        "Name": str,
+        "Priority": int,
+        "Statement": "StatementOutputTypeDef",
+        "VisibilityConfig": VisibilityConfigOutputTypeDef,
+    },
+)
+_OptionalRuleOutputTypeDef = TypedDict(
+    "_OptionalRuleOutputTypeDef",
+    {
+        "Action": RuleActionOutputTypeDef,
+        "OverrideAction": OverrideActionOutputTypeDef,
+        "RuleLabels": List[LabelOutputTypeDef],
+        "CaptchaConfig": CaptchaConfigOutputTypeDef,
+        "ChallengeConfig": ChallengeConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class RuleOutputTypeDef(_RequiredRuleOutputTypeDef, _OptionalRuleOutputTypeDef):
+    pass
+
+
 RuleSummaryTypeDef = TypedDict(
     "RuleSummaryTypeDef",
     {
         "Name": str,
-        "Action": RuleActionTypeDef,
+        "Action": RuleActionOutputTypeDef,
     },
     total=False,
 )
 
+RuleActionOverrideTypeDef = TypedDict(
+    "RuleActionOverrideTypeDef",
+    {
+        "Name": str,
+        "ActionToUse": RuleActionTypeDef,
+    },
+)
+
 _RequiredRuleTypeDef = TypedDict(
     "_RequiredRuleTypeDef",
     {
         "Name": str,
         "Priority": int,
         "Statement": "StatementTypeDef",
         "VisibilityConfig": VisibilityConfigTypeDef,
@@ -2405,40 +3333,131 @@
 class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
 
 GetLoggingConfigurationResponseTypeDef = TypedDict(
     "GetLoggingConfigurationResponseTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLoggingConfigurationsResponseTypeDef = TypedDict(
     "ListLoggingConfigurationsResponseTypeDef",
     {
-        "LoggingConfigurations": List[LoggingConfigurationTypeDef],
+        "LoggingConfigurations": List[LoggingConfigurationOutputTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutLoggingConfigurationResponseTypeDef = TypedDict(
+    "PutLoggingConfigurationResponseTypeDef",
+    {
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "PutLoggingConfigurationRequestRequestTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
 )
 
-PutLoggingConfigurationResponseTypeDef = TypedDict(
-    "PutLoggingConfigurationResponseTypeDef",
+_RequiredManagedRuleGroupStatementOutputTypeDef = TypedDict(
+    "_RequiredManagedRuleGroupStatementOutputTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VendorName": str,
+        "Name": str,
+    },
+)
+_OptionalManagedRuleGroupStatementOutputTypeDef = TypedDict(
+    "_OptionalManagedRuleGroupStatementOutputTypeDef",
+    {
+        "Version": str,
+        "ExcludedRules": List[ExcludedRuleOutputTypeDef],
+        "ScopeDownStatement": Dict[str, Any],
+        "ManagedRuleGroupConfigs": List[ManagedRuleGroupConfigOutputTypeDef],
+        "RuleActionOverrides": List[RuleActionOverrideOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class ManagedRuleGroupStatementOutputTypeDef(
+    _RequiredManagedRuleGroupStatementOutputTypeDef, _OptionalManagedRuleGroupStatementOutputTypeDef
+):
+    pass
+
+
+_RequiredRuleGroupReferenceStatementOutputTypeDef = TypedDict(
+    "_RequiredRuleGroupReferenceStatementOutputTypeDef",
+    {
+        "ARN": str,
+    },
+)
+_OptionalRuleGroupReferenceStatementOutputTypeDef = TypedDict(
+    "_OptionalRuleGroupReferenceStatementOutputTypeDef",
+    {
+        "ExcludedRules": List[ExcludedRuleOutputTypeDef],
+        "RuleActionOverrides": List[RuleActionOverrideOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class RuleGroupReferenceStatementOutputTypeDef(
+    _RequiredRuleGroupReferenceStatementOutputTypeDef,
+    _OptionalRuleGroupReferenceStatementOutputTypeDef,
+):
+    pass
+
+
+_RequiredRuleGroupTypeDef = TypedDict(
+    "_RequiredRuleGroupTypeDef",
+    {
+        "Name": str,
+        "Id": str,
+        "Capacity": int,
+        "ARN": str,
+        "VisibilityConfig": VisibilityConfigOutputTypeDef,
+    },
+)
+_OptionalRuleGroupTypeDef = TypedDict(
+    "_OptionalRuleGroupTypeDef",
+    {
+        "Description": str,
+        "Rules": List[RuleOutputTypeDef],
+        "LabelNamespace": str,
+        "CustomResponseBodies": Dict[str, CustomResponseBodyOutputTypeDef],
+        "AvailableLabels": List[LabelSummaryTypeDef],
+        "ConsumedLabels": List[LabelSummaryTypeDef],
+    },
+    total=False,
+)
+
+
+class RuleGroupTypeDef(_RequiredRuleGroupTypeDef, _OptionalRuleGroupTypeDef):
+    pass
+
+
+DescribeManagedRuleGroupResponseTypeDef = TypedDict(
+    "DescribeManagedRuleGroupResponseTypeDef",
+    {
+        "VersionName": str,
+        "SnsTopicArn": str,
+        "Capacity": int,
+        "Rules": List[RuleSummaryTypeDef],
+        "LabelNamespace": str,
+        "AvailableLabels": List[LabelSummaryTypeDef],
+        "ConsumedLabels": List[LabelSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredManagedRuleGroupStatementTypeDef = TypedDict(
     "_RequiredManagedRuleGroupStatementTypeDef",
     {
         "VendorName": str,
@@ -2482,28 +3501,14 @@
 
 class RuleGroupReferenceStatementTypeDef(
     _RequiredRuleGroupReferenceStatementTypeDef, _OptionalRuleGroupReferenceStatementTypeDef
 ):
     pass
 
 
-DescribeManagedRuleGroupResponseTypeDef = TypedDict(
-    "DescribeManagedRuleGroupResponseTypeDef",
-    {
-        "VersionName": str,
-        "SnsTopicArn": str,
-        "Capacity": int,
-        "Rules": List[RuleSummaryTypeDef],
-        "LabelNamespace": str,
-        "AvailableLabels": List[LabelSummaryTypeDef],
-        "ConsumedLabels": List[LabelSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CheckCapacityRequestRequestTypeDef = TypedDict(
     "CheckCapacityRequestRequestTypeDef",
     {
         "Scope": ScopeType,
         "Rules": Sequence[RuleTypeDef],
     },
 )
@@ -2562,42 +3567,14 @@
 
 class CreateWebACLRequestRequestTypeDef(
     _RequiredCreateWebACLRequestRequestTypeDef, _OptionalCreateWebACLRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredRuleGroupTypeDef = TypedDict(
-    "_RequiredRuleGroupTypeDef",
-    {
-        "Name": str,
-        "Id": str,
-        "Capacity": int,
-        "ARN": str,
-        "VisibilityConfig": VisibilityConfigTypeDef,
-    },
-)
-_OptionalRuleGroupTypeDef = TypedDict(
-    "_OptionalRuleGroupTypeDef",
-    {
-        "Description": str,
-        "Rules": List[RuleTypeDef],
-        "LabelNamespace": str,
-        "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
-        "AvailableLabels": List[LabelSummaryTypeDef],
-        "ConsumedLabels": List[LabelSummaryTypeDef],
-    },
-    total=False,
-)
-
-
-class RuleGroupTypeDef(_RequiredRuleGroupTypeDef, _OptionalRuleGroupTypeDef):
-    pass
-
-
 _RequiredUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleGroupRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "VisibilityConfig": VisibilityConfigTypeDef,
@@ -2652,20 +3629,51 @@
 ):
     pass
 
 
 FirewallManagerStatementTypeDef = TypedDict(
     "FirewallManagerStatementTypeDef",
     {
-        "ManagedRuleGroupStatement": ManagedRuleGroupStatementTypeDef,
-        "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
+        "ManagedRuleGroupStatement": ManagedRuleGroupStatementOutputTypeDef,
+        "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
+    },
+    total=False,
+)
+
+StatementOutputTypeDef = TypedDict(
+    "StatementOutputTypeDef",
+    {
+        "ByteMatchStatement": ByteMatchStatementOutputTypeDef,
+        "SqliMatchStatement": SqliMatchStatementOutputTypeDef,
+        "XssMatchStatement": XssMatchStatementOutputTypeDef,
+        "SizeConstraintStatement": SizeConstraintStatementOutputTypeDef,
+        "GeoMatchStatement": GeoMatchStatementOutputTypeDef,
+        "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
+        "IPSetReferenceStatement": IPSetReferenceStatementOutputTypeDef,
+        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementOutputTypeDef,
+        "RateBasedStatement": Dict[str, Any],
+        "AndStatement": Dict[str, Any],
+        "OrStatement": Dict[str, Any],
+        "NotStatement": Dict[str, Any],
+        "ManagedRuleGroupStatement": Dict[str, Any],
+        "LabelMatchStatement": LabelMatchStatementOutputTypeDef,
+        "RegexMatchStatement": RegexMatchStatementOutputTypeDef,
     },
     total=False,
 )
 
+GetRuleGroupResponseTypeDef = TypedDict(
+    "GetRuleGroupResponseTypeDef",
+    {
+        "RuleGroup": RuleGroupTypeDef,
+        "LockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 StatementTypeDef = TypedDict(
     "StatementTypeDef",
     {
         "ByteMatchStatement": ByteMatchStatementTypeDef,
         "SqliMatchStatement": SqliMatchStatementTypeDef,
         "XssMatchStatement": XssMatchStatementTypeDef,
         "SizeConstraintStatement": SizeConstraintStatementTypeDef,
@@ -2680,78 +3688,69 @@
         "ManagedRuleGroupStatement": Dict[str, Any],
         "LabelMatchStatement": LabelMatchStatementTypeDef,
         "RegexMatchStatement": RegexMatchStatementTypeDef,
     },
     total=False,
 )
 
-GetRuleGroupResponseTypeDef = TypedDict(
-    "GetRuleGroupResponseTypeDef",
-    {
-        "RuleGroup": RuleGroupTypeDef,
-        "LockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FirewallManagerRuleGroupTypeDef = TypedDict(
     "FirewallManagerRuleGroupTypeDef",
     {
         "Name": str,
         "Priority": int,
         "FirewallManagerStatement": FirewallManagerStatementTypeDef,
-        "OverrideAction": OverrideActionTypeDef,
-        "VisibilityConfig": VisibilityConfigTypeDef,
+        "OverrideAction": OverrideActionOutputTypeDef,
+        "VisibilityConfig": VisibilityConfigOutputTypeDef,
     },
 )
 
 _RequiredWebACLTypeDef = TypedDict(
     "_RequiredWebACLTypeDef",
     {
         "Name": str,
         "Id": str,
         "ARN": str,
-        "DefaultAction": DefaultActionTypeDef,
-        "VisibilityConfig": VisibilityConfigTypeDef,
+        "DefaultAction": DefaultActionOutputTypeDef,
+        "VisibilityConfig": VisibilityConfigOutputTypeDef,
     },
 )
 _OptionalWebACLTypeDef = TypedDict(
     "_OptionalWebACLTypeDef",
     {
         "Description": str,
-        "Rules": List[RuleTypeDef],
+        "Rules": List[RuleOutputTypeDef],
         "Capacity": int,
         "PreProcessFirewallManagerRuleGroups": List[FirewallManagerRuleGroupTypeDef],
         "PostProcessFirewallManagerRuleGroups": List[FirewallManagerRuleGroupTypeDef],
         "ManagedByFirewallManager": bool,
         "LabelNamespace": str,
-        "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
-        "CaptchaConfig": CaptchaConfigTypeDef,
-        "ChallengeConfig": ChallengeConfigTypeDef,
+        "CustomResponseBodies": Dict[str, CustomResponseBodyOutputTypeDef],
+        "CaptchaConfig": CaptchaConfigOutputTypeDef,
+        "ChallengeConfig": ChallengeConfigOutputTypeDef,
         "TokenDomains": List[str],
-        "AssociationConfig": AssociationConfigTypeDef,
+        "AssociationConfig": AssociationConfigOutputTypeDef,
     },
     total=False,
 )
 
 
 class WebACLTypeDef(_RequiredWebACLTypeDef, _OptionalWebACLTypeDef):
     pass
 
 
 GetWebACLForResourceResponseTypeDef = TypedDict(
     "GetWebACLForResourceResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWebACLResponseTypeDef = TypedDict(
     "GetWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
         "LockToken": str,
         "ApplicationIntegrationURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/type_defs.pyi` & `mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/type_defs.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -52,217 +52,302 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "APIKeySummaryTypeDef",
+    "AWSManagedRulesBotControlRuleSetOutputTypeDef",
     "AWSManagedRulesBotControlRuleSetTypeDef",
+    "ActionConditionOutputTypeDef",
     "ActionConditionTypeDef",
+    "AddressFieldOutputTypeDef",
     "AddressFieldTypeDef",
+    "AndStatementOutputTypeDef",
     "AndStatementTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
+    "RequestBodyAssociatedResourceTypeConfigOutputTypeDef",
     "RequestBodyAssociatedResourceTypeConfigTypeDef",
+    "BodyOutputTypeDef",
     "BodyTypeDef",
+    "TextTransformationOutputTypeDef",
     "TextTransformationTypeDef",
+    "ImmunityTimePropertyOutputTypeDef",
     "ImmunityTimePropertyTypeDef",
     "CaptchaResponseTypeDef",
     "ChallengeResponseTypeDef",
-    "CheckCapacityResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "LabelNameConditionOutputTypeDef",
     "LabelNameConditionTypeDef",
+    "CookieMatchPatternOutputTypeDef",
     "CookieMatchPatternTypeDef",
     "CreateAPIKeyRequestRequestTypeDef",
-    "CreateAPIKeyResponseTypeDef",
     "TagTypeDef",
     "IPSetSummaryTypeDef",
     "RegexTypeDef",
     "RegexPatternSetSummaryTypeDef",
     "CustomResponseBodyTypeDef",
     "VisibilityConfigTypeDef",
     "RuleGroupSummaryTypeDef",
     "WebACLSummaryTypeDef",
+    "CustomHTTPHeaderOutputTypeDef",
     "CustomHTTPHeaderTypeDef",
+    "CustomResponseBodyOutputTypeDef",
     "DeleteFirewallManagerRuleGroupsRequestRequestTypeDef",
-    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
     "DeleteIPSetRequestRequestTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeletePermissionPolicyRequestRequestTypeDef",
     "DeleteRegexPatternSetRequestRequestTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
     "DeleteWebACLRequestRequestTypeDef",
     "DescribeAllManagedProductsRequestRequestTypeDef",
     "ManagedProductDescriptorTypeDef",
     "DescribeManagedProductsByVendorRequestRequestTypeDef",
     "DescribeManagedRuleGroupRequestRequestTypeDef",
     "LabelSummaryTypeDef",
     "DisassociateWebACLRequestRequestTypeDef",
+    "EmailFieldOutputTypeDef",
     "EmailFieldTypeDef",
+    "ExcludedRuleOutputTypeDef",
     "ExcludedRuleTypeDef",
+    "HeaderOrderOutputTypeDef",
+    "SingleHeaderOutputTypeDef",
+    "SingleQueryArgumentOutputTypeDef",
     "HeaderOrderTypeDef",
     "SingleHeaderTypeDef",
     "SingleQueryArgumentTypeDef",
+    "VisibilityConfigOutputTypeDef",
+    "ForwardedIPConfigOutputTypeDef",
     "ForwardedIPConfigTypeDef",
     "GenerateMobileSdkReleaseUrlRequestRequestTypeDef",
-    "GenerateMobileSdkReleaseUrlResponseTypeDef",
     "GetDecryptedAPIKeyRequestRequestTypeDef",
-    "GetDecryptedAPIKeyResponseTypeDef",
     "GetIPSetRequestRequestTypeDef",
     "IPSetTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
     "GetManagedRuleSetRequestRequestTypeDef",
     "GetMobileSdkReleaseRequestRequestTypeDef",
     "GetPermissionPolicyRequestRequestTypeDef",
-    "GetPermissionPolicyResponseTypeDef",
     "GetRateBasedStatementManagedKeysRequestRequestTypeDef",
     "RateBasedStatementManagedKeysIPSetTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
     "TimeWindowTypeDef",
+    "TimeWindowOutputTypeDef",
     "GetWebACLForResourceRequestRequestTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
+    "HeaderMatchPatternOutputTypeDef",
     "HeaderMatchPatternTypeDef",
+    "IPSetForwardedIPConfigOutputTypeDef",
     "IPSetForwardedIPConfigTypeDef",
+    "JsonMatchPatternOutputTypeDef",
     "JsonMatchPatternTypeDef",
+    "LabelMatchStatementOutputTypeDef",
     "LabelMatchStatementTypeDef",
+    "LabelOutputTypeDef",
     "LabelTypeDef",
     "ListAPIKeysRequestRequestTypeDef",
     "ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef",
     "ManagedRuleGroupVersionTypeDef",
     "ListAvailableManagedRuleGroupsRequestRequestTypeDef",
     "ManagedRuleGroupSummaryTypeDef",
     "ListIPSetsRequestRequestTypeDef",
     "ListLoggingConfigurationsRequestRequestTypeDef",
     "ListManagedRuleSetsRequestRequestTypeDef",
     "ManagedRuleSetSummaryTypeDef",
     "ListMobileSdkReleasesRequestRequestTypeDef",
     "ReleaseSummaryTypeDef",
     "ListRegexPatternSetsRequestRequestTypeDef",
     "ListResourcesForWebACLRequestRequestTypeDef",
-    "ListResourcesForWebACLResponseTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
+    "PasswordFieldOutputTypeDef",
+    "UsernameFieldOutputTypeDef",
     "PasswordFieldTypeDef",
     "UsernameFieldTypeDef",
     "ManagedRuleSetVersionTypeDef",
+    "TagOutputTypeDef",
+    "NotStatementOutputTypeDef",
     "NotStatementTypeDef",
+    "OrStatementOutputTypeDef",
     "OrStatementTypeDef",
+    "PhoneNumberFieldOutputTypeDef",
     "PhoneNumberFieldTypeDef",
     "VersionToPublishTypeDef",
-    "PutManagedRuleSetVersionsResponseTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
+    "RateLimitLabelNamespaceOutputTypeDef",
     "RateLimitLabelNamespaceTypeDef",
+    "RegexOutputTypeDef",
+    "ResponseInspectionBodyContainsOutputTypeDef",
     "ResponseInspectionBodyContainsTypeDef",
+    "ResponseInspectionHeaderOutputTypeDef",
     "ResponseInspectionHeaderTypeDef",
+    "ResponseInspectionJsonOutputTypeDef",
     "ResponseInspectionJsonTypeDef",
+    "ResponseInspectionStatusCodeOutputTypeDef",
     "ResponseInspectionStatusCodeTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
-    "UpdateIPSetResponseTypeDef",
     "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
-    "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
-    "UpdateRegexPatternSetResponseTypeDef",
-    "UpdateRuleGroupResponseTypeDef",
-    "UpdateWebACLResponseTypeDef",
-    "ListAPIKeysResponseTypeDef",
+    "AssociationConfigOutputTypeDef",
     "AssociationConfigTypeDef",
+    "RateLimitCookieOutputTypeDef",
+    "RateLimitHeaderOutputTypeDef",
+    "RateLimitQueryArgumentOutputTypeDef",
+    "RateLimitQueryStringOutputTypeDef",
+    "RateLimitUriPathOutputTypeDef",
     "RateLimitCookieTypeDef",
     "RateLimitHeaderTypeDef",
     "RateLimitQueryArgumentTypeDef",
     "RateLimitQueryStringTypeDef",
+    "RateLimitUriPathTypeDef",
+    "CaptchaConfigOutputTypeDef",
+    "ChallengeConfigOutputTypeDef",
     "CaptchaConfigTypeDef",
     "ChallengeConfigTypeDef",
+    "CheckCapacityResponseTypeDef",
+    "CreateAPIKeyResponseTypeDef",
+    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
+    "GenerateMobileSdkReleaseUrlResponseTypeDef",
+    "GetDecryptedAPIKeyResponseTypeDef",
+    "GetPermissionPolicyResponseTypeDef",
+    "ListAPIKeysResponseTypeDef",
+    "ListResourcesForWebACLResponseTypeDef",
+    "PutManagedRuleSetVersionsResponseTypeDef",
+    "UpdateIPSetResponseTypeDef",
+    "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
+    "UpdateRegexPatternSetResponseTypeDef",
+    "UpdateRuleGroupResponseTypeDef",
+    "UpdateWebACLResponseTypeDef",
+    "ConditionOutputTypeDef",
     "ConditionTypeDef",
+    "CookiesOutputTypeDef",
     "CookiesTypeDef",
     "CreateIPSetRequestRequestTypeDef",
-    "MobileSdkReleaseTypeDef",
-    "TagInfoForResourceTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIPSetResponseTypeDef",
     "ListIPSetsResponseTypeDef",
     "CreateRegexPatternSetRequestRequestTypeDef",
-    "RegexPatternSetTypeDef",
     "UpdateRegexPatternSetRequestRequestTypeDef",
     "CreateRegexPatternSetResponseTypeDef",
     "ListRegexPatternSetsResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "ListRuleGroupsResponseTypeDef",
     "CreateWebACLResponseTypeDef",
     "ListWebACLsResponseTypeDef",
+    "CustomRequestHandlingOutputTypeDef",
+    "CustomResponseOutputTypeDef",
     "CustomRequestHandlingTypeDef",
     "CustomResponseTypeDef",
     "DescribeAllManagedProductsResponseTypeDef",
     "DescribeManagedProductsByVendorResponseTypeDef",
+    "GeoMatchStatementOutputTypeDef",
     "GeoMatchStatementTypeDef",
     "GetIPSetResponseTypeDef",
     "GetRateBasedStatementManagedKeysResponseTypeDef",
     "GetSampledRequestsRequestRequestTypeDef",
     "HTTPRequestTypeDef",
+    "HeadersOutputTypeDef",
     "HeadersTypeDef",
+    "IPSetReferenceStatementOutputTypeDef",
     "IPSetReferenceStatementTypeDef",
+    "JsonBodyOutputTypeDef",
     "JsonBodyTypeDef",
     "ListAvailableManagedRuleGroupVersionsResponseTypeDef",
     "ListAvailableManagedRuleGroupsResponseTypeDef",
     "ListManagedRuleSetsResponseTypeDef",
     "ListMobileSdkReleasesResponseTypeDef",
+    "RequestInspectionOutputTypeDef",
     "RequestInspectionTypeDef",
     "ManagedRuleSetTypeDef",
+    "MobileSdkReleaseTypeDef",
+    "TagInfoForResourceTypeDef",
+    "RequestInspectionACFPOutputTypeDef",
     "RequestInspectionACFPTypeDef",
     "PutManagedRuleSetVersionsRequestRequestTypeDef",
+    "RegexPatternSetTypeDef",
+    "ResponseInspectionOutputTypeDef",
     "ResponseInspectionTypeDef",
+    "RateBasedStatementCustomKeyOutputTypeDef",
     "RateBasedStatementCustomKeyTypeDef",
+    "FilterOutputTypeDef",
     "FilterTypeDef",
-    "GetMobileSdkReleaseResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "GetRegexPatternSetResponseTypeDef",
+    "AllowActionOutputTypeDef",
+    "CaptchaActionOutputTypeDef",
+    "ChallengeActionOutputTypeDef",
+    "CountActionOutputTypeDef",
+    "BlockActionOutputTypeDef",
     "AllowActionTypeDef",
     "CaptchaActionTypeDef",
     "ChallengeActionTypeDef",
     "CountActionTypeDef",
     "BlockActionTypeDef",
     "SampledHTTPRequestTypeDef",
+    "FieldToMatchOutputTypeDef",
     "FieldToMatchTypeDef",
     "GetManagedRuleSetResponseTypeDef",
+    "GetMobileSdkReleaseResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "GetRegexPatternSetResponseTypeDef",
+    "AWSManagedRulesACFPRuleSetOutputTypeDef",
+    "AWSManagedRulesATPRuleSetOutputTypeDef",
     "AWSManagedRulesACFPRuleSetTypeDef",
     "AWSManagedRulesATPRuleSetTypeDef",
+    "RateBasedStatementOutputTypeDef",
     "RateBasedStatementTypeDef",
+    "LoggingFilterOutputTypeDef",
     "LoggingFilterTypeDef",
+    "OverrideActionOutputTypeDef",
+    "DefaultActionOutputTypeDef",
+    "RuleActionOutputTypeDef",
     "OverrideActionTypeDef",
     "DefaultActionTypeDef",
     "RuleActionTypeDef",
     "GetSampledRequestsResponseTypeDef",
+    "ByteMatchStatementOutputTypeDef",
+    "RegexMatchStatementOutputTypeDef",
+    "RegexPatternSetReferenceStatementOutputTypeDef",
+    "SizeConstraintStatementOutputTypeDef",
+    "SqliMatchStatementOutputTypeDef",
+    "XssMatchStatementOutputTypeDef",
     "ByteMatchStatementTypeDef",
     "RegexMatchStatementTypeDef",
     "RegexPatternSetReferenceStatementTypeDef",
     "SizeConstraintStatementTypeDef",
     "SqliMatchStatementTypeDef",
     "XssMatchStatementTypeDef",
+    "ManagedRuleGroupConfigOutputTypeDef",
     "ManagedRuleGroupConfigTypeDef",
+    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
-    "RuleActionOverrideTypeDef",
+    "RuleActionOverrideOutputTypeDef",
+    "RuleOutputTypeDef",
     "RuleSummaryTypeDef",
+    "RuleActionOverrideTypeDef",
     "RuleTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
-    "PutLoggingConfigurationRequestRequestTypeDef",
     "PutLoggingConfigurationResponseTypeDef",
+    "PutLoggingConfigurationRequestRequestTypeDef",
+    "ManagedRuleGroupStatementOutputTypeDef",
+    "RuleGroupReferenceStatementOutputTypeDef",
+    "RuleGroupTypeDef",
+    "DescribeManagedRuleGroupResponseTypeDef",
     "ManagedRuleGroupStatementTypeDef",
     "RuleGroupReferenceStatementTypeDef",
-    "DescribeManagedRuleGroupResponseTypeDef",
     "CheckCapacityRequestRequestTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
     "CreateWebACLRequestRequestTypeDef",
-    "RuleGroupTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
     "UpdateWebACLRequestRequestTypeDef",
     "FirewallManagerStatementTypeDef",
-    "StatementTypeDef",
+    "StatementOutputTypeDef",
     "GetRuleGroupResponseTypeDef",
+    "StatementTypeDef",
     "FirewallManagerRuleGroupTypeDef",
     "WebACLTypeDef",
     "GetWebACLForResourceResponseTypeDef",
     "GetWebACLResponseTypeDef",
 )
 
 APIKeySummaryTypeDef = TypedDict(
@@ -272,35 +357,63 @@
         "APIKey": str,
         "CreationTimestamp": datetime,
         "Version": int,
     },
     total=False,
 )
 
+AWSManagedRulesBotControlRuleSetOutputTypeDef = TypedDict(
+    "AWSManagedRulesBotControlRuleSetOutputTypeDef",
+    {
+        "InspectionLevel": InspectionLevelType,
+    },
+)
+
 AWSManagedRulesBotControlRuleSetTypeDef = TypedDict(
     "AWSManagedRulesBotControlRuleSetTypeDef",
     {
         "InspectionLevel": InspectionLevelType,
     },
 )
 
+ActionConditionOutputTypeDef = TypedDict(
+    "ActionConditionOutputTypeDef",
+    {
+        "Action": ActionValueType,
+    },
+)
+
 ActionConditionTypeDef = TypedDict(
     "ActionConditionTypeDef",
     {
         "Action": ActionValueType,
     },
 )
 
+AddressFieldOutputTypeDef = TypedDict(
+    "AddressFieldOutputTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+
 AddressFieldTypeDef = TypedDict(
     "AddressFieldTypeDef",
     {
         "Identifier": str,
     },
 )
 
+AndStatementOutputTypeDef = TypedDict(
+    "AndStatementOutputTypeDef",
+    {
+        "Statements": List["StatementOutputTypeDef"],
+    },
+)
+
 AndStatementTypeDef = TypedDict(
     "AndStatementTypeDef",
     {
         "Statements": Sequence["StatementTypeDef"],
     },
 )
 
@@ -308,37 +421,67 @@
     "AssociateWebACLRequestRequestTypeDef",
     {
         "WebACLArn": str,
         "ResourceArn": str,
     },
 )
 
+RequestBodyAssociatedResourceTypeConfigOutputTypeDef = TypedDict(
+    "RequestBodyAssociatedResourceTypeConfigOutputTypeDef",
+    {
+        "DefaultSizeInspectionLimit": SizeInspectionLimitType,
+    },
+)
+
 RequestBodyAssociatedResourceTypeConfigTypeDef = TypedDict(
     "RequestBodyAssociatedResourceTypeConfigTypeDef",
     {
         "DefaultSizeInspectionLimit": SizeInspectionLimitType,
     },
 )
 
+BodyOutputTypeDef = TypedDict(
+    "BodyOutputTypeDef",
+    {
+        "OversizeHandling": OversizeHandlingType,
+    },
+    total=False,
+)
+
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "OversizeHandling": OversizeHandlingType,
     },
     total=False,
 )
 
+TextTransformationOutputTypeDef = TypedDict(
+    "TextTransformationOutputTypeDef",
+    {
+        "Priority": int,
+        "Type": TextTransformationTypeType,
+    },
+)
+
 TextTransformationTypeDef = TypedDict(
     "TextTransformationTypeDef",
     {
         "Priority": int,
         "Type": TextTransformationTypeType,
     },
 )
 
+ImmunityTimePropertyOutputTypeDef = TypedDict(
+    "ImmunityTimePropertyOutputTypeDef",
+    {
+        "ImmunityTime": int,
+    },
+)
+
 ImmunityTimePropertyTypeDef = TypedDict(
     "ImmunityTimePropertyTypeDef",
     {
         "ImmunityTime": int,
     },
 )
 
@@ -358,29 +501,49 @@
         "ResponseCode": int,
         "SolveTimestamp": int,
         "FailureReason": FailureReasonType,
     },
     total=False,
 )
 
-CheckCapacityResponseTypeDef = TypedDict(
-    "CheckCapacityResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Capacity": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+LabelNameConditionOutputTypeDef = TypedDict(
+    "LabelNameConditionOutputTypeDef",
+    {
+        "LabelName": str,
     },
 )
 
 LabelNameConditionTypeDef = TypedDict(
     "LabelNameConditionTypeDef",
     {
         "LabelName": str,
     },
 )
 
+CookieMatchPatternOutputTypeDef = TypedDict(
+    "CookieMatchPatternOutputTypeDef",
+    {
+        "All": Dict[str, Any],
+        "IncludedCookies": List[str],
+        "ExcludedCookies": List[str],
+    },
+    total=False,
+)
+
 CookieMatchPatternTypeDef = TypedDict(
     "CookieMatchPatternTypeDef",
     {
         "All": Mapping[str, Any],
         "IncludedCookies": Sequence[str],
         "ExcludedCookies": Sequence[str],
     },
@@ -391,22 +554,14 @@
     "CreateAPIKeyRequestRequestTypeDef",
     {
         "Scope": ScopeType,
         "TokenDomains": Sequence[str],
     },
 )
 
-CreateAPIKeyResponseTypeDef = TypedDict(
-    "CreateAPIKeyResponseTypeDef",
-    {
-        "APIKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -480,35 +635,43 @@
         "Description": str,
         "LockToken": str,
         "ARN": str,
     },
     total=False,
 )
 
+CustomHTTPHeaderOutputTypeDef = TypedDict(
+    "CustomHTTPHeaderOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
+
 CustomHTTPHeaderTypeDef = TypedDict(
     "CustomHTTPHeaderTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-DeleteFirewallManagerRuleGroupsRequestRequestTypeDef = TypedDict(
-    "DeleteFirewallManagerRuleGroupsRequestRequestTypeDef",
+CustomResponseBodyOutputTypeDef = TypedDict(
+    "CustomResponseBodyOutputTypeDef",
     {
-        "WebACLArn": str,
-        "WebACLLockToken": str,
+        "ContentType": ResponseContentTypeType,
+        "Content": str,
     },
 )
 
-DeleteFirewallManagerRuleGroupsResponseTypeDef = TypedDict(
-    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
+DeleteFirewallManagerRuleGroupsRequestRequestTypeDef = TypedDict(
+    "DeleteFirewallManagerRuleGroupsRequestRequestTypeDef",
     {
-        "NextWebACLLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "WebACLArn": str,
+        "WebACLLockToken": str,
     },
 )
 
 DeleteIPSetRequestRequestTypeDef = TypedDict(
     "DeleteIPSetRequestRequestTypeDef",
     {
         "Name": str,
@@ -626,28 +789,63 @@
 DisassociateWebACLRequestRequestTypeDef = TypedDict(
     "DisassociateWebACLRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+EmailFieldOutputTypeDef = TypedDict(
+    "EmailFieldOutputTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+
 EmailFieldTypeDef = TypedDict(
     "EmailFieldTypeDef",
     {
         "Identifier": str,
     },
 )
 
+ExcludedRuleOutputTypeDef = TypedDict(
+    "ExcludedRuleOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 ExcludedRuleTypeDef = TypedDict(
     "ExcludedRuleTypeDef",
     {
         "Name": str,
     },
 )
 
+HeaderOrderOutputTypeDef = TypedDict(
+    "HeaderOrderOutputTypeDef",
+    {
+        "OversizeHandling": OversizeHandlingType,
+    },
+)
+
+SingleHeaderOutputTypeDef = TypedDict(
+    "SingleHeaderOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+
+SingleQueryArgumentOutputTypeDef = TypedDict(
+    "SingleQueryArgumentOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 HeaderOrderTypeDef = TypedDict(
     "HeaderOrderTypeDef",
     {
         "OversizeHandling": OversizeHandlingType,
     },
 )
 
@@ -661,14 +859,31 @@
 SingleQueryArgumentTypeDef = TypedDict(
     "SingleQueryArgumentTypeDef",
     {
         "Name": str,
     },
 )
 
+VisibilityConfigOutputTypeDef = TypedDict(
+    "VisibilityConfigOutputTypeDef",
+    {
+        "SampledRequestsEnabled": bool,
+        "CloudWatchMetricsEnabled": bool,
+        "MetricName": str,
+    },
+)
+
+ForwardedIPConfigOutputTypeDef = TypedDict(
+    "ForwardedIPConfigOutputTypeDef",
+    {
+        "HeaderName": str,
+        "FallbackBehavior": FallbackBehaviorType,
+    },
+)
+
 ForwardedIPConfigTypeDef = TypedDict(
     "ForwardedIPConfigTypeDef",
     {
         "HeaderName": str,
         "FallbackBehavior": FallbackBehaviorType,
     },
 )
@@ -677,39 +892,22 @@
     "GenerateMobileSdkReleaseUrlRequestRequestTypeDef",
     {
         "Platform": PlatformType,
         "ReleaseVersion": str,
     },
 )
 
-GenerateMobileSdkReleaseUrlResponseTypeDef = TypedDict(
-    "GenerateMobileSdkReleaseUrlResponseTypeDef",
-    {
-        "Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDecryptedAPIKeyRequestRequestTypeDef = TypedDict(
     "GetDecryptedAPIKeyRequestRequestTypeDef",
     {
         "Scope": ScopeType,
         "APIKey": str,
     },
 )
 
-GetDecryptedAPIKeyResponseTypeDef = TypedDict(
-    "GetDecryptedAPIKeyResponseTypeDef",
-    {
-        "TokenDomains": List[str],
-        "CreationTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetIPSetRequestRequestTypeDef = TypedDict(
     "GetIPSetRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
     },
@@ -763,22 +961,14 @@
 GetPermissionPolicyRequestRequestTypeDef = TypedDict(
     "GetPermissionPolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetPermissionPolicyResponseTypeDef = TypedDict(
-    "GetPermissionPolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRateBasedStatementManagedKeysRequestRequestTypeDef = TypedDict(
     "_RequiredGetRateBasedStatementManagedKeysRequestRequestTypeDef",
     {
         "Scope": ScopeType,
         "WebACLName": str,
         "WebACLId": str,
         "RuleName": str,
@@ -831,14 +1021,22 @@
     "TimeWindowTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
 )
 
+TimeWindowOutputTypeDef = TypedDict(
+    "TimeWindowOutputTypeDef",
+    {
+        "StartTime": datetime,
+        "EndTime": datetime,
+    },
+)
+
 GetWebACLForResourceRequestRequestTypeDef = TypedDict(
     "GetWebACLForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -856,50 +1054,93 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
+HeaderMatchPatternOutputTypeDef = TypedDict(
+    "HeaderMatchPatternOutputTypeDef",
+    {
+        "All": Dict[str, Any],
+        "IncludedHeaders": List[str],
+        "ExcludedHeaders": List[str],
+    },
+    total=False,
+)
+
 HeaderMatchPatternTypeDef = TypedDict(
     "HeaderMatchPatternTypeDef",
     {
         "All": Mapping[str, Any],
         "IncludedHeaders": Sequence[str],
         "ExcludedHeaders": Sequence[str],
     },
     total=False,
 )
 
+IPSetForwardedIPConfigOutputTypeDef = TypedDict(
+    "IPSetForwardedIPConfigOutputTypeDef",
+    {
+        "HeaderName": str,
+        "FallbackBehavior": FallbackBehaviorType,
+        "Position": ForwardedIPPositionType,
+    },
+)
+
 IPSetForwardedIPConfigTypeDef = TypedDict(
     "IPSetForwardedIPConfigTypeDef",
     {
         "HeaderName": str,
         "FallbackBehavior": FallbackBehaviorType,
         "Position": ForwardedIPPositionType,
     },
 )
 
+JsonMatchPatternOutputTypeDef = TypedDict(
+    "JsonMatchPatternOutputTypeDef",
+    {
+        "All": Dict[str, Any],
+        "IncludedPaths": List[str],
+    },
+    total=False,
+)
+
 JsonMatchPatternTypeDef = TypedDict(
     "JsonMatchPatternTypeDef",
     {
         "All": Mapping[str, Any],
         "IncludedPaths": Sequence[str],
     },
     total=False,
 )
 
+LabelMatchStatementOutputTypeDef = TypedDict(
+    "LabelMatchStatementOutputTypeDef",
+    {
+        "Scope": LabelMatchScopeType,
+        "Key": str,
+    },
+)
+
 LabelMatchStatementTypeDef = TypedDict(
     "LabelMatchStatementTypeDef",
     {
         "Scope": LabelMatchScopeType,
         "Key": str,
     },
 )
 
+LabelOutputTypeDef = TypedDict(
+    "LabelOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 LabelTypeDef = TypedDict(
     "LabelTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1129,22 +1370,14 @@
 
 class ListResourcesForWebACLRequestRequestTypeDef(
     _RequiredListResourcesForWebACLRequestRequestTypeDef,
     _OptionalListResourcesForWebACLRequestRequestTypeDef,
 ):
     pass
 
-ListResourcesForWebACLResponseTypeDef = TypedDict(
-    "ListResourcesForWebACLResponseTypeDef",
-    {
-        "ResourceArns": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListRuleGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListRuleGroupsRequestRequestTypeDef",
     {
         "Scope": ScopeType,
     },
 )
 _OptionalListRuleGroupsRequestRequestTypeDef = TypedDict(
@@ -1198,14 +1431,28 @@
 )
 
 class ListWebACLsRequestRequestTypeDef(
     _RequiredListWebACLsRequestRequestTypeDef, _OptionalListWebACLsRequestRequestTypeDef
 ):
     pass
 
+PasswordFieldOutputTypeDef = TypedDict(
+    "PasswordFieldOutputTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+
+UsernameFieldOutputTypeDef = TypedDict(
+    "UsernameFieldOutputTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+
 PasswordFieldTypeDef = TypedDict(
     "PasswordFieldTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -1225,28 +1472,57 @@
         "PublishTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
         "ExpiryTimestamp": datetime,
     },
     total=False,
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+NotStatementOutputTypeDef = TypedDict(
+    "NotStatementOutputTypeDef",
+    {
+        "Statement": "StatementOutputTypeDef",
+    },
+)
+
 NotStatementTypeDef = TypedDict(
     "NotStatementTypeDef",
     {
         "Statement": "StatementTypeDef",
     },
 )
 
+OrStatementOutputTypeDef = TypedDict(
+    "OrStatementOutputTypeDef",
+    {
+        "Statements": List["StatementOutputTypeDef"],
+    },
+)
+
 OrStatementTypeDef = TypedDict(
     "OrStatementTypeDef",
     {
         "Statements": Sequence[Dict[str, Any]],
     },
 )
 
+PhoneNumberFieldOutputTypeDef = TypedDict(
+    "PhoneNumberFieldOutputTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+
 PhoneNumberFieldTypeDef = TypedDict(
     "PhoneNumberFieldTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -1255,79 +1531,109 @@
     {
         "AssociatedRuleGroupArn": str,
         "ForecastedLifetime": int,
     },
     total=False,
 )
 
-PutManagedRuleSetVersionsResponseTypeDef = TypedDict(
-    "PutManagedRuleSetVersionsResponseTypeDef",
-    {
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutPermissionPolicyRequestRequestTypeDef = TypedDict(
     "PutPermissionPolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Policy": str,
     },
 )
 
+RateLimitLabelNamespaceOutputTypeDef = TypedDict(
+    "RateLimitLabelNamespaceOutputTypeDef",
+    {
+        "Namespace": str,
+    },
+)
+
 RateLimitLabelNamespaceTypeDef = TypedDict(
     "RateLimitLabelNamespaceTypeDef",
     {
         "Namespace": str,
     },
 )
 
+RegexOutputTypeDef = TypedDict(
+    "RegexOutputTypeDef",
+    {
+        "RegexString": str,
+    },
+    total=False,
+)
+
+ResponseInspectionBodyContainsOutputTypeDef = TypedDict(
+    "ResponseInspectionBodyContainsOutputTypeDef",
+    {
+        "SuccessStrings": List[str],
+        "FailureStrings": List[str],
+    },
+)
+
 ResponseInspectionBodyContainsTypeDef = TypedDict(
     "ResponseInspectionBodyContainsTypeDef",
     {
         "SuccessStrings": Sequence[str],
         "FailureStrings": Sequence[str],
     },
 )
 
+ResponseInspectionHeaderOutputTypeDef = TypedDict(
+    "ResponseInspectionHeaderOutputTypeDef",
+    {
+        "Name": str,
+        "SuccessValues": List[str],
+        "FailureValues": List[str],
+    },
+)
+
 ResponseInspectionHeaderTypeDef = TypedDict(
     "ResponseInspectionHeaderTypeDef",
     {
         "Name": str,
         "SuccessValues": Sequence[str],
         "FailureValues": Sequence[str],
     },
 )
 
+ResponseInspectionJsonOutputTypeDef = TypedDict(
+    "ResponseInspectionJsonOutputTypeDef",
+    {
+        "Identifier": str,
+        "SuccessValues": List[str],
+        "FailureValues": List[str],
+    },
+)
+
 ResponseInspectionJsonTypeDef = TypedDict(
     "ResponseInspectionJsonTypeDef",
     {
         "Identifier": str,
         "SuccessValues": Sequence[str],
         "FailureValues": Sequence[str],
     },
 )
 
-ResponseInspectionStatusCodeTypeDef = TypedDict(
-    "ResponseInspectionStatusCodeTypeDef",
+ResponseInspectionStatusCodeOutputTypeDef = TypedDict(
+    "ResponseInspectionStatusCodeOutputTypeDef",
     {
-        "SuccessCodes": Sequence[int],
-        "FailureCodes": Sequence[int],
+        "SuccessCodes": List[int],
+        "FailureCodes": List[int],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ResponseInspectionStatusCodeTypeDef = TypedDict(
+    "ResponseInspectionStatusCodeTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "SuccessCodes": Sequence[int],
+        "FailureCodes": Sequence[int],
     },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -1354,86 +1660,82 @@
 )
 
 class UpdateIPSetRequestRequestTypeDef(
     _RequiredUpdateIPSetRequestRequestTypeDef, _OptionalUpdateIPSetRequestRequestTypeDef
 ):
     pass
 
-UpdateIPSetResponseTypeDef = TypedDict(
-    "UpdateIPSetResponseTypeDef",
-    {
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef = TypedDict(
     "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "LockToken": str,
         "VersionToExpire": str,
         "ExpiryTimestamp": Union[datetime, str],
     },
 )
 
-UpdateManagedRuleSetVersionExpiryDateResponseTypeDef = TypedDict(
-    "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
+AssociationConfigOutputTypeDef = TypedDict(
+    "AssociationConfigOutputTypeDef",
     {
-        "ExpiringVersion": str,
-        "ExpiryTimestamp": datetime,
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestBody": Dict[
+            Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigOutputTypeDef
+        ],
     },
+    total=False,
 )
 
-UpdateRegexPatternSetResponseTypeDef = TypedDict(
-    "UpdateRegexPatternSetResponseTypeDef",
+AssociationConfigTypeDef = TypedDict(
+    "AssociationConfigTypeDef",
     {
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestBody": Mapping[
+            Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef
+        ],
     },
+    total=False,
 )
 
-UpdateRuleGroupResponseTypeDef = TypedDict(
-    "UpdateRuleGroupResponseTypeDef",
+RateLimitCookieOutputTypeDef = TypedDict(
+    "RateLimitCookieOutputTypeDef",
     {
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
+        "TextTransformations": List[TextTransformationOutputTypeDef],
     },
 )
 
-UpdateWebACLResponseTypeDef = TypedDict(
-    "UpdateWebACLResponseTypeDef",
+RateLimitHeaderOutputTypeDef = TypedDict(
+    "RateLimitHeaderOutputTypeDef",
     {
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
+        "TextTransformations": List[TextTransformationOutputTypeDef],
     },
 )
 
-ListAPIKeysResponseTypeDef = TypedDict(
-    "ListAPIKeysResponseTypeDef",
+RateLimitQueryArgumentOutputTypeDef = TypedDict(
+    "RateLimitQueryArgumentOutputTypeDef",
     {
-        "NextMarker": str,
-        "APIKeySummaries": List[APIKeySummaryTypeDef],
-        "ApplicationIntegrationURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
+        "TextTransformations": List[TextTransformationOutputTypeDef],
     },
 )
 
-AssociationConfigTypeDef = TypedDict(
-    "AssociationConfigTypeDef",
+RateLimitQueryStringOutputTypeDef = TypedDict(
+    "RateLimitQueryStringOutputTypeDef",
     {
-        "RequestBody": Mapping[
-            Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef
-        ],
+        "TextTransformations": List[TextTransformationOutputTypeDef],
+    },
+)
+
+RateLimitUriPathOutputTypeDef = TypedDict(
+    "RateLimitUriPathOutputTypeDef",
+    {
+        "TextTransformations": List[TextTransformationOutputTypeDef],
     },
-    total=False,
 )
 
 RateLimitCookieTypeDef = TypedDict(
     "RateLimitCookieTypeDef",
     {
         "Name": str,
         "TextTransformations": Sequence[TextTransformationTypeDef],
@@ -1459,14 +1761,37 @@
 RateLimitQueryStringTypeDef = TypedDict(
     "RateLimitQueryStringTypeDef",
     {
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
+RateLimitUriPathTypeDef = TypedDict(
+    "RateLimitUriPathTypeDef",
+    {
+        "TextTransformations": Sequence[TextTransformationTypeDef],
+    },
+)
+
+CaptchaConfigOutputTypeDef = TypedDict(
+    "CaptchaConfigOutputTypeDef",
+    {
+        "ImmunityTimeProperty": ImmunityTimePropertyOutputTypeDef,
+    },
+    total=False,
+)
+
+ChallengeConfigOutputTypeDef = TypedDict(
+    "ChallengeConfigOutputTypeDef",
+    {
+        "ImmunityTimeProperty": ImmunityTimePropertyOutputTypeDef,
+    },
+    total=False,
+)
+
 CaptchaConfigTypeDef = TypedDict(
     "CaptchaConfigTypeDef",
     {
         "ImmunityTimeProperty": ImmunityTimePropertyTypeDef,
     },
     total=False,
 )
@@ -1475,23 +1800,158 @@
     "ChallengeConfigTypeDef",
     {
         "ImmunityTimeProperty": ImmunityTimePropertyTypeDef,
     },
     total=False,
 )
 
+CheckCapacityResponseTypeDef = TypedDict(
+    "CheckCapacityResponseTypeDef",
+    {
+        "Capacity": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAPIKeyResponseTypeDef = TypedDict(
+    "CreateAPIKeyResponseTypeDef",
+    {
+        "APIKey": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFirewallManagerRuleGroupsResponseTypeDef = TypedDict(
+    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
+    {
+        "NextWebACLLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateMobileSdkReleaseUrlResponseTypeDef = TypedDict(
+    "GenerateMobileSdkReleaseUrlResponseTypeDef",
+    {
+        "Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDecryptedAPIKeyResponseTypeDef = TypedDict(
+    "GetDecryptedAPIKeyResponseTypeDef",
+    {
+        "TokenDomains": List[str],
+        "CreationTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPermissionPolicyResponseTypeDef = TypedDict(
+    "GetPermissionPolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAPIKeysResponseTypeDef = TypedDict(
+    "ListAPIKeysResponseTypeDef",
+    {
+        "NextMarker": str,
+        "APIKeySummaries": List[APIKeySummaryTypeDef],
+        "ApplicationIntegrationURL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListResourcesForWebACLResponseTypeDef = TypedDict(
+    "ListResourcesForWebACLResponseTypeDef",
+    {
+        "ResourceArns": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutManagedRuleSetVersionsResponseTypeDef = TypedDict(
+    "PutManagedRuleSetVersionsResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateIPSetResponseTypeDef = TypedDict(
+    "UpdateIPSetResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateManagedRuleSetVersionExpiryDateResponseTypeDef = TypedDict(
+    "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
+    {
+        "ExpiringVersion": str,
+        "ExpiryTimestamp": datetime,
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRegexPatternSetResponseTypeDef = TypedDict(
+    "UpdateRegexPatternSetResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRuleGroupResponseTypeDef = TypedDict(
+    "UpdateRuleGroupResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWebACLResponseTypeDef = TypedDict(
+    "UpdateWebACLResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConditionOutputTypeDef = TypedDict(
+    "ConditionOutputTypeDef",
+    {
+        "ActionCondition": ActionConditionOutputTypeDef,
+        "LabelNameCondition": LabelNameConditionOutputTypeDef,
+    },
+    total=False,
+)
+
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "ActionCondition": ActionConditionTypeDef,
         "LabelNameCondition": LabelNameConditionTypeDef,
     },
     total=False,
 )
 
+CookiesOutputTypeDef = TypedDict(
+    "CookiesOutputTypeDef",
+    {
+        "MatchPattern": CookieMatchPatternOutputTypeDef,
+        "MatchScope": MapMatchScopeType,
+        "OversizeHandling": OversizeHandlingType,
+    },
+)
+
 CookiesTypeDef = TypedDict(
     "CookiesTypeDef",
     {
         "MatchPattern": CookieMatchPatternTypeDef,
         "MatchScope": MapMatchScopeType,
         "OversizeHandling": OversizeHandlingType,
     },
@@ -1516,56 +1976,36 @@
 )
 
 class CreateIPSetRequestRequestTypeDef(
     _RequiredCreateIPSetRequestRequestTypeDef, _OptionalCreateIPSetRequestRequestTypeDef
 ):
     pass
 
-MobileSdkReleaseTypeDef = TypedDict(
-    "MobileSdkReleaseTypeDef",
-    {
-        "ReleaseVersion": str,
-        "Timestamp": datetime,
-        "ReleaseNotes": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-TagInfoForResourceTypeDef = TypedDict(
-    "TagInfoForResourceTypeDef",
-    {
-        "ResourceARN": str,
-        "TagList": List[TagTypeDef],
-    },
-    total=False,
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 CreateIPSetResponseTypeDef = TypedDict(
     "CreateIPSetResponseTypeDef",
     {
         "Summary": IPSetSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIPSetsResponseTypeDef = TypedDict(
     "ListIPSetsResponseTypeDef",
     {
         "NextMarker": str,
         "IPSets": List[IPSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateRegexPatternSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRegexPatternSetRequestRequestTypeDef",
     {
         "Name": str,
@@ -1584,26 +2024,14 @@
 
 class CreateRegexPatternSetRequestRequestTypeDef(
     _RequiredCreateRegexPatternSetRequestRequestTypeDef,
     _OptionalCreateRegexPatternSetRequestRequestTypeDef,
 ):
     pass
 
-RegexPatternSetTypeDef = TypedDict(
-    "RegexPatternSetTypeDef",
-    {
-        "Name": str,
-        "Id": str,
-        "ARN": str,
-        "Description": str,
-        "RegularExpressionList": List[RegexTypeDef],
-    },
-    total=False,
-)
-
 _RequiredUpdateRegexPatternSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRegexPatternSetRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "RegularExpressionList": Sequence[RegexTypeDef],
@@ -1624,61 +2052,88 @@
 ):
     pass
 
 CreateRegexPatternSetResponseTypeDef = TypedDict(
     "CreateRegexPatternSetResponseTypeDef",
     {
         "Summary": RegexPatternSetSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRegexPatternSetsResponseTypeDef = TypedDict(
     "ListRegexPatternSetsResponseTypeDef",
     {
         "NextMarker": str,
         "RegexPatternSets": List[RegexPatternSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRuleGroupResponseTypeDef = TypedDict(
     "CreateRuleGroupResponseTypeDef",
     {
         "Summary": RuleGroupSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRuleGroupsResponseTypeDef = TypedDict(
     "ListRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "RuleGroups": List[RuleGroupSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWebACLResponseTypeDef = TypedDict(
     "CreateWebACLResponseTypeDef",
     {
         "Summary": WebACLSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWebACLsResponseTypeDef = TypedDict(
     "ListWebACLsResponseTypeDef",
     {
         "NextMarker": str,
         "WebACLs": List[WebACLSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CustomRequestHandlingOutputTypeDef = TypedDict(
+    "CustomRequestHandlingOutputTypeDef",
+    {
+        "InsertHeaders": List[CustomHTTPHeaderOutputTypeDef],
+    },
+)
+
+_RequiredCustomResponseOutputTypeDef = TypedDict(
+    "_RequiredCustomResponseOutputTypeDef",
+    {
+        "ResponseCode": int,
+    },
+)
+_OptionalCustomResponseOutputTypeDef = TypedDict(
+    "_OptionalCustomResponseOutputTypeDef",
+    {
+        "CustomResponseBodyKey": str,
+        "ResponseHeaders": List[CustomHTTPHeaderOutputTypeDef],
     },
+    total=False,
 )
 
+class CustomResponseOutputTypeDef(
+    _RequiredCustomResponseOutputTypeDef, _OptionalCustomResponseOutputTypeDef
+):
+    pass
+
 CustomRequestHandlingTypeDef = TypedDict(
     "CustomRequestHandlingTypeDef",
     {
         "InsertHeaders": Sequence[CustomHTTPHeaderTypeDef],
     },
 )
 
@@ -1700,50 +2155,59 @@
 class CustomResponseTypeDef(_RequiredCustomResponseTypeDef, _OptionalCustomResponseTypeDef):
     pass
 
 DescribeAllManagedProductsResponseTypeDef = TypedDict(
     "DescribeAllManagedProductsResponseTypeDef",
     {
         "ManagedProducts": List[ManagedProductDescriptorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeManagedProductsByVendorResponseTypeDef = TypedDict(
     "DescribeManagedProductsByVendorResponseTypeDef",
     {
         "ManagedProducts": List[ManagedProductDescriptorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GeoMatchStatementOutputTypeDef = TypedDict(
+    "GeoMatchStatementOutputTypeDef",
+    {
+        "CountryCodes": List[CountryCodeType],
+        "ForwardedIPConfig": ForwardedIPConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 GeoMatchStatementTypeDef = TypedDict(
     "GeoMatchStatementTypeDef",
     {
         "CountryCodes": Sequence[CountryCodeType],
         "ForwardedIPConfig": ForwardedIPConfigTypeDef,
     },
     total=False,
 )
 
 GetIPSetResponseTypeDef = TypedDict(
     "GetIPSetResponseTypeDef",
     {
         "IPSet": IPSetTypeDef,
         "LockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRateBasedStatementManagedKeysResponseTypeDef = TypedDict(
     "GetRateBasedStatementManagedKeysResponseTypeDef",
     {
         "ManagedKeysIPV4": RateBasedStatementManagedKeysIPSetTypeDef,
         "ManagedKeysIPV6": RateBasedStatementManagedKeysIPSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSampledRequestsRequestRequestTypeDef = TypedDict(
     "GetSampledRequestsRequestRequestTypeDef",
     {
         "WebAclArn": str,
@@ -1763,23 +2227,51 @@
         "Method": str,
         "HTTPVersion": str,
         "Headers": List[HTTPHeaderTypeDef],
     },
     total=False,
 )
 
+HeadersOutputTypeDef = TypedDict(
+    "HeadersOutputTypeDef",
+    {
+        "MatchPattern": HeaderMatchPatternOutputTypeDef,
+        "MatchScope": MapMatchScopeType,
+        "OversizeHandling": OversizeHandlingType,
+    },
+)
+
 HeadersTypeDef = TypedDict(
     "HeadersTypeDef",
     {
         "MatchPattern": HeaderMatchPatternTypeDef,
         "MatchScope": MapMatchScopeType,
         "OversizeHandling": OversizeHandlingType,
     },
 )
 
+_RequiredIPSetReferenceStatementOutputTypeDef = TypedDict(
+    "_RequiredIPSetReferenceStatementOutputTypeDef",
+    {
+        "ARN": str,
+    },
+)
+_OptionalIPSetReferenceStatementOutputTypeDef = TypedDict(
+    "_OptionalIPSetReferenceStatementOutputTypeDef",
+    {
+        "IPSetForwardedIPConfig": IPSetForwardedIPConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class IPSetReferenceStatementOutputTypeDef(
+    _RequiredIPSetReferenceStatementOutputTypeDef, _OptionalIPSetReferenceStatementOutputTypeDef
+):
+    pass
+
 _RequiredIPSetReferenceStatementTypeDef = TypedDict(
     "_RequiredIPSetReferenceStatementTypeDef",
     {
         "ARN": str,
     },
 )
 _OptionalIPSetReferenceStatementTypeDef = TypedDict(
@@ -1791,14 +2283,33 @@
 )
 
 class IPSetReferenceStatementTypeDef(
     _RequiredIPSetReferenceStatementTypeDef, _OptionalIPSetReferenceStatementTypeDef
 ):
     pass
 
+_RequiredJsonBodyOutputTypeDef = TypedDict(
+    "_RequiredJsonBodyOutputTypeDef",
+    {
+        "MatchPattern": JsonMatchPatternOutputTypeDef,
+        "MatchScope": JsonMatchScopeType,
+    },
+)
+_OptionalJsonBodyOutputTypeDef = TypedDict(
+    "_OptionalJsonBodyOutputTypeDef",
+    {
+        "InvalidFallbackBehavior": BodyParsingFallbackBehaviorType,
+        "OversizeHandling": OversizeHandlingType,
+    },
+    total=False,
+)
+
+class JsonBodyOutputTypeDef(_RequiredJsonBodyOutputTypeDef, _OptionalJsonBodyOutputTypeDef):
+    pass
+
 _RequiredJsonBodyTypeDef = TypedDict(
     "_RequiredJsonBodyTypeDef",
     {
         "MatchPattern": JsonMatchPatternTypeDef,
         "MatchScope": JsonMatchScopeType,
     },
 )
@@ -1816,42 +2327,51 @@
 
 ListAvailableManagedRuleGroupVersionsResponseTypeDef = TypedDict(
     "ListAvailableManagedRuleGroupVersionsResponseTypeDef",
     {
         "NextMarker": str,
         "Versions": List[ManagedRuleGroupVersionTypeDef],
         "CurrentDefaultVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAvailableManagedRuleGroupsResponseTypeDef = TypedDict(
     "ListAvailableManagedRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "ManagedRuleGroups": List[ManagedRuleGroupSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListManagedRuleSetsResponseTypeDef = TypedDict(
     "ListManagedRuleSetsResponseTypeDef",
     {
         "NextMarker": str,
         "ManagedRuleSets": List[ManagedRuleSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMobileSdkReleasesResponseTypeDef = TypedDict(
     "ListMobileSdkReleasesResponseTypeDef",
     {
         "ReleaseSummaries": List[ReleaseSummaryTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RequestInspectionOutputTypeDef = TypedDict(
+    "RequestInspectionOutputTypeDef",
+    {
+        "PayloadType": PayloadTypeType,
+        "UsernameField": UsernameFieldOutputTypeDef,
+        "PasswordField": PasswordFieldOutputTypeDef,
     },
 )
 
 RequestInspectionTypeDef = TypedDict(
     "RequestInspectionTypeDef",
     {
         "PayloadType": PayloadTypeType,
@@ -1878,14 +2398,57 @@
     },
     total=False,
 )
 
 class ManagedRuleSetTypeDef(_RequiredManagedRuleSetTypeDef, _OptionalManagedRuleSetTypeDef):
     pass
 
+MobileSdkReleaseTypeDef = TypedDict(
+    "MobileSdkReleaseTypeDef",
+    {
+        "ReleaseVersion": str,
+        "Timestamp": datetime,
+        "ReleaseNotes": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+TagInfoForResourceTypeDef = TypedDict(
+    "TagInfoForResourceTypeDef",
+    {
+        "ResourceARN": str,
+        "TagList": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+_RequiredRequestInspectionACFPOutputTypeDef = TypedDict(
+    "_RequiredRequestInspectionACFPOutputTypeDef",
+    {
+        "PayloadType": PayloadTypeType,
+    },
+)
+_OptionalRequestInspectionACFPOutputTypeDef = TypedDict(
+    "_OptionalRequestInspectionACFPOutputTypeDef",
+    {
+        "UsernameField": UsernameFieldOutputTypeDef,
+        "PasswordField": PasswordFieldOutputTypeDef,
+        "EmailField": EmailFieldOutputTypeDef,
+        "PhoneNumberFields": List[PhoneNumberFieldOutputTypeDef],
+        "AddressFields": List[AddressFieldOutputTypeDef],
+    },
+    total=False,
+)
+
+class RequestInspectionACFPOutputTypeDef(
+    _RequiredRequestInspectionACFPOutputTypeDef, _OptionalRequestInspectionACFPOutputTypeDef
+):
+    pass
+
 _RequiredRequestInspectionACFPTypeDef = TypedDict(
     "_RequiredRequestInspectionACFPTypeDef",
     {
         "PayloadType": PayloadTypeType,
     },
 )
 _OptionalRequestInspectionACFPTypeDef = TypedDict(
@@ -1925,73 +2488,136 @@
 
 class PutManagedRuleSetVersionsRequestRequestTypeDef(
     _RequiredPutManagedRuleSetVersionsRequestRequestTypeDef,
     _OptionalPutManagedRuleSetVersionsRequestRequestTypeDef,
 ):
     pass
 
+RegexPatternSetTypeDef = TypedDict(
+    "RegexPatternSetTypeDef",
+    {
+        "Name": str,
+        "Id": str,
+        "ARN": str,
+        "Description": str,
+        "RegularExpressionList": List[RegexOutputTypeDef],
+    },
+    total=False,
+)
+
+ResponseInspectionOutputTypeDef = TypedDict(
+    "ResponseInspectionOutputTypeDef",
+    {
+        "StatusCode": ResponseInspectionStatusCodeOutputTypeDef,
+        "Header": ResponseInspectionHeaderOutputTypeDef,
+        "BodyContains": ResponseInspectionBodyContainsOutputTypeDef,
+        "Json": ResponseInspectionJsonOutputTypeDef,
+    },
+    total=False,
+)
+
 ResponseInspectionTypeDef = TypedDict(
     "ResponseInspectionTypeDef",
     {
         "StatusCode": ResponseInspectionStatusCodeTypeDef,
         "Header": ResponseInspectionHeaderTypeDef,
         "BodyContains": ResponseInspectionBodyContainsTypeDef,
         "Json": ResponseInspectionJsonTypeDef,
     },
     total=False,
 )
 
+RateBasedStatementCustomKeyOutputTypeDef = TypedDict(
+    "RateBasedStatementCustomKeyOutputTypeDef",
+    {
+        "Header": RateLimitHeaderOutputTypeDef,
+        "Cookie": RateLimitCookieOutputTypeDef,
+        "QueryArgument": RateLimitQueryArgumentOutputTypeDef,
+        "QueryString": RateLimitQueryStringOutputTypeDef,
+        "HTTPMethod": Dict[str, Any],
+        "ForwardedIP": Dict[str, Any],
+        "IP": Dict[str, Any],
+        "LabelNamespace": RateLimitLabelNamespaceOutputTypeDef,
+        "UriPath": RateLimitUriPathOutputTypeDef,
+    },
+    total=False,
+)
+
 RateBasedStatementCustomKeyTypeDef = TypedDict(
     "RateBasedStatementCustomKeyTypeDef",
     {
         "Header": RateLimitHeaderTypeDef,
         "Cookie": RateLimitCookieTypeDef,
         "QueryArgument": RateLimitQueryArgumentTypeDef,
         "QueryString": RateLimitQueryStringTypeDef,
         "HTTPMethod": Mapping[str, Any],
         "ForwardedIP": Mapping[str, Any],
         "IP": Mapping[str, Any],
         "LabelNamespace": RateLimitLabelNamespaceTypeDef,
+        "UriPath": RateLimitUriPathTypeDef,
     },
     total=False,
 )
 
+FilterOutputTypeDef = TypedDict(
+    "FilterOutputTypeDef",
+    {
+        "Behavior": FilterBehaviorType,
+        "Requirement": FilterRequirementType,
+        "Conditions": List[ConditionOutputTypeDef],
+    },
+)
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Behavior": FilterBehaviorType,
         "Requirement": FilterRequirementType,
-        "Conditions": List[ConditionTypeDef],
+        "Conditions": Sequence[ConditionTypeDef],
     },
 )
 
-GetMobileSdkReleaseResponseTypeDef = TypedDict(
-    "GetMobileSdkReleaseResponseTypeDef",
+AllowActionOutputTypeDef = TypedDict(
+    "AllowActionOutputTypeDef",
     {
-        "MobileSdkRelease": MobileSdkReleaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
     },
+    total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+CaptchaActionOutputTypeDef = TypedDict(
+    "CaptchaActionOutputTypeDef",
     {
-        "NextMarker": str,
-        "TagInfoForResource": TagInfoForResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
     },
+    total=False,
 )
 
-GetRegexPatternSetResponseTypeDef = TypedDict(
-    "GetRegexPatternSetResponseTypeDef",
+ChallengeActionOutputTypeDef = TypedDict(
+    "ChallengeActionOutputTypeDef",
     {
-        "RegexPatternSet": RegexPatternSetTypeDef,
-        "LockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
+    },
+    total=False,
+)
+
+CountActionOutputTypeDef = TypedDict(
+    "CountActionOutputTypeDef",
+    {
+        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
     },
+    total=False,
+)
+
+BlockActionOutputTypeDef = TypedDict(
+    "BlockActionOutputTypeDef",
+    {
+        "CustomResponse": CustomResponseOutputTypeDef,
+    },
+    total=False,
 )
 
 AllowActionTypeDef = TypedDict(
     "AllowActionTypeDef",
     {
         "CustomRequestHandling": CustomRequestHandlingTypeDef,
     },
@@ -2041,27 +2667,45 @@
     "_OptionalSampledHTTPRequestTypeDef",
     {
         "Timestamp": datetime,
         "Action": str,
         "RuleNameWithinRuleGroup": str,
         "RequestHeadersInserted": List[HTTPHeaderTypeDef],
         "ResponseCodeSent": int,
-        "Labels": List[LabelTypeDef],
+        "Labels": List[LabelOutputTypeDef],
         "CaptchaResponse": CaptchaResponseTypeDef,
         "ChallengeResponse": ChallengeResponseTypeDef,
         "OverriddenAction": str,
     },
     total=False,
 )
 
 class SampledHTTPRequestTypeDef(
     _RequiredSampledHTTPRequestTypeDef, _OptionalSampledHTTPRequestTypeDef
 ):
     pass
 
+FieldToMatchOutputTypeDef = TypedDict(
+    "FieldToMatchOutputTypeDef",
+    {
+        "SingleHeader": SingleHeaderOutputTypeDef,
+        "SingleQueryArgument": SingleQueryArgumentOutputTypeDef,
+        "AllQueryArguments": Dict[str, Any],
+        "UriPath": Dict[str, Any],
+        "QueryString": Dict[str, Any],
+        "Body": BodyOutputTypeDef,
+        "Method": Dict[str, Any],
+        "JsonBody": JsonBodyOutputTypeDef,
+        "Headers": HeadersOutputTypeDef,
+        "Cookies": CookiesOutputTypeDef,
+        "HeaderOrder": HeaderOrderOutputTypeDef,
+    },
+    total=False,
+)
+
 FieldToMatchTypeDef = TypedDict(
     "FieldToMatchTypeDef",
     {
         "SingleHeader": SingleHeaderTypeDef,
         "SingleQueryArgument": SingleQueryArgumentTypeDef,
         "AllQueryArguments": Mapping[str, Any],
         "UriPath": Mapping[str, Any],
@@ -2077,18 +2721,88 @@
 )
 
 GetManagedRuleSetResponseTypeDef = TypedDict(
     "GetManagedRuleSetResponseTypeDef",
     {
         "ManagedRuleSet": ManagedRuleSetTypeDef,
         "LockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetMobileSdkReleaseResponseTypeDef = TypedDict(
+    "GetMobileSdkReleaseResponseTypeDef",
+    {
+        "MobileSdkRelease": MobileSdkReleaseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "NextMarker": str,
+        "TagInfoForResource": TagInfoForResourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRegexPatternSetResponseTypeDef = TypedDict(
+    "GetRegexPatternSetResponseTypeDef",
+    {
+        "RegexPatternSet": RegexPatternSetTypeDef,
+        "LockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredAWSManagedRulesACFPRuleSetOutputTypeDef = TypedDict(
+    "_RequiredAWSManagedRulesACFPRuleSetOutputTypeDef",
+    {
+        "CreationPath": str,
+        "RegistrationPagePath": str,
+        "RequestInspection": RequestInspectionACFPOutputTypeDef,
+    },
+)
+_OptionalAWSManagedRulesACFPRuleSetOutputTypeDef = TypedDict(
+    "_OptionalAWSManagedRulesACFPRuleSetOutputTypeDef",
+    {
+        "ResponseInspection": ResponseInspectionOutputTypeDef,
+        "EnableRegexInPath": bool,
+    },
+    total=False,
+)
+
+class AWSManagedRulesACFPRuleSetOutputTypeDef(
+    _RequiredAWSManagedRulesACFPRuleSetOutputTypeDef,
+    _OptionalAWSManagedRulesACFPRuleSetOutputTypeDef,
+):
+    pass
+
+_RequiredAWSManagedRulesATPRuleSetOutputTypeDef = TypedDict(
+    "_RequiredAWSManagedRulesATPRuleSetOutputTypeDef",
+    {
+        "LoginPath": str,
+    },
+)
+_OptionalAWSManagedRulesATPRuleSetOutputTypeDef = TypedDict(
+    "_OptionalAWSManagedRulesATPRuleSetOutputTypeDef",
+    {
+        "RequestInspection": RequestInspectionOutputTypeDef,
+        "ResponseInspection": ResponseInspectionOutputTypeDef,
+        "EnableRegexInPath": bool,
+    },
+    total=False,
+)
+
+class AWSManagedRulesATPRuleSetOutputTypeDef(
+    _RequiredAWSManagedRulesATPRuleSetOutputTypeDef, _OptionalAWSManagedRulesATPRuleSetOutputTypeDef
+):
+    pass
+
 _RequiredAWSManagedRulesACFPRuleSetTypeDef = TypedDict(
     "_RequiredAWSManagedRulesACFPRuleSetTypeDef",
     {
         "CreationPath": str,
         "RegistrationPagePath": str,
         "RequestInspection": RequestInspectionACFPTypeDef,
     },
@@ -2124,14 +2838,36 @@
 )
 
 class AWSManagedRulesATPRuleSetTypeDef(
     _RequiredAWSManagedRulesATPRuleSetTypeDef, _OptionalAWSManagedRulesATPRuleSetTypeDef
 ):
     pass
 
+_RequiredRateBasedStatementOutputTypeDef = TypedDict(
+    "_RequiredRateBasedStatementOutputTypeDef",
+    {
+        "Limit": int,
+        "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
+    },
+)
+_OptionalRateBasedStatementOutputTypeDef = TypedDict(
+    "_OptionalRateBasedStatementOutputTypeDef",
+    {
+        "ScopeDownStatement": "StatementOutputTypeDef",
+        "ForwardedIPConfig": ForwardedIPConfigOutputTypeDef,
+        "CustomKeys": List[RateBasedStatementCustomKeyOutputTypeDef],
+    },
+    total=False,
+)
+
+class RateBasedStatementOutputTypeDef(
+    _RequiredRateBasedStatementOutputTypeDef, _OptionalRateBasedStatementOutputTypeDef
+):
+    pass
+
 _RequiredRateBasedStatementTypeDef = TypedDict(
     "_RequiredRateBasedStatementTypeDef",
     {
         "Limit": int,
         "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
     },
 )
@@ -2146,22 +2882,60 @@
 )
 
 class RateBasedStatementTypeDef(
     _RequiredRateBasedStatementTypeDef, _OptionalRateBasedStatementTypeDef
 ):
     pass
 
+LoggingFilterOutputTypeDef = TypedDict(
+    "LoggingFilterOutputTypeDef",
+    {
+        "Filters": List[FilterOutputTypeDef],
+        "DefaultBehavior": FilterBehaviorType,
+    },
+)
+
 LoggingFilterTypeDef = TypedDict(
     "LoggingFilterTypeDef",
     {
-        "Filters": List[FilterTypeDef],
+        "Filters": Sequence[FilterTypeDef],
         "DefaultBehavior": FilterBehaviorType,
     },
 )
 
+OverrideActionOutputTypeDef = TypedDict(
+    "OverrideActionOutputTypeDef",
+    {
+        "Count": CountActionOutputTypeDef,
+        "None": Dict[str, Any],
+    },
+    total=False,
+)
+
+DefaultActionOutputTypeDef = TypedDict(
+    "DefaultActionOutputTypeDef",
+    {
+        "Block": BlockActionOutputTypeDef,
+        "Allow": AllowActionOutputTypeDef,
+    },
+    total=False,
+)
+
+RuleActionOutputTypeDef = TypedDict(
+    "RuleActionOutputTypeDef",
+    {
+        "Block": BlockActionOutputTypeDef,
+        "Allow": AllowActionOutputTypeDef,
+        "Count": CountActionOutputTypeDef,
+        "Captcha": CaptchaActionOutputTypeDef,
+        "Challenge": ChallengeActionOutputTypeDef,
+    },
+    total=False,
+)
+
 OverrideActionTypeDef = TypedDict(
     "OverrideActionTypeDef",
     {
         "Count": CountActionTypeDef,
         "None": Mapping[str, Any],
     },
     total=False,
@@ -2189,16 +2963,82 @@
 )
 
 GetSampledRequestsResponseTypeDef = TypedDict(
     "GetSampledRequestsResponseTypeDef",
     {
         "SampledRequests": List[SampledHTTPRequestTypeDef],
         "PopulationSize": int,
-        "TimeWindow": TimeWindowTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TimeWindow": TimeWindowOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ByteMatchStatementOutputTypeDef = TypedDict(
+    "ByteMatchStatementOutputTypeDef",
+    {
+        "SearchString": bytes,
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformations": List[TextTransformationOutputTypeDef],
+        "PositionalConstraint": PositionalConstraintType,
+    },
+)
+
+RegexMatchStatementOutputTypeDef = TypedDict(
+    "RegexMatchStatementOutputTypeDef",
+    {
+        "RegexString": str,
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformations": List[TextTransformationOutputTypeDef],
+    },
+)
+
+RegexPatternSetReferenceStatementOutputTypeDef = TypedDict(
+    "RegexPatternSetReferenceStatementOutputTypeDef",
+    {
+        "ARN": str,
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformations": List[TextTransformationOutputTypeDef],
+    },
+)
+
+SizeConstraintStatementOutputTypeDef = TypedDict(
+    "SizeConstraintStatementOutputTypeDef",
+    {
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "ComparisonOperator": ComparisonOperatorType,
+        "Size": int,
+        "TextTransformations": List[TextTransformationOutputTypeDef],
+    },
+)
+
+_RequiredSqliMatchStatementOutputTypeDef = TypedDict(
+    "_RequiredSqliMatchStatementOutputTypeDef",
+    {
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformations": List[TextTransformationOutputTypeDef],
+    },
+)
+_OptionalSqliMatchStatementOutputTypeDef = TypedDict(
+    "_OptionalSqliMatchStatementOutputTypeDef",
+    {
+        "SensitivityLevel": SensitivityLevelType,
+    },
+    total=False,
+)
+
+class SqliMatchStatementOutputTypeDef(
+    _RequiredSqliMatchStatementOutputTypeDef, _OptionalSqliMatchStatementOutputTypeDef
+):
+    pass
+
+XssMatchStatementOutputTypeDef = TypedDict(
+    "XssMatchStatementOutputTypeDef",
+    {
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformations": List[TextTransformationOutputTypeDef],
     },
 )
 
 ByteMatchStatementTypeDef = TypedDict(
     "ByteMatchStatementTypeDef",
     {
         "SearchString": Union[str, bytes, IO[Any], StreamingBody],
@@ -2260,67 +3100,135 @@
     "XssMatchStatementTypeDef",
     {
         "FieldToMatch": FieldToMatchTypeDef,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
+ManagedRuleGroupConfigOutputTypeDef = TypedDict(
+    "ManagedRuleGroupConfigOutputTypeDef",
+    {
+        "LoginPath": str,
+        "PayloadType": PayloadTypeType,
+        "UsernameField": UsernameFieldOutputTypeDef,
+        "PasswordField": PasswordFieldOutputTypeDef,
+        "AWSManagedRulesBotControlRuleSet": AWSManagedRulesBotControlRuleSetOutputTypeDef,
+        "AWSManagedRulesATPRuleSet": AWSManagedRulesATPRuleSetOutputTypeDef,
+        "AWSManagedRulesACFPRuleSet": AWSManagedRulesACFPRuleSetOutputTypeDef,
+    },
+    total=False,
+)
+
 ManagedRuleGroupConfigTypeDef = TypedDict(
     "ManagedRuleGroupConfigTypeDef",
     {
         "LoginPath": str,
         "PayloadType": PayloadTypeType,
         "UsernameField": UsernameFieldTypeDef,
         "PasswordField": PasswordFieldTypeDef,
         "AWSManagedRulesBotControlRuleSet": AWSManagedRulesBotControlRuleSetTypeDef,
         "AWSManagedRulesATPRuleSet": AWSManagedRulesATPRuleSetTypeDef,
         "AWSManagedRulesACFPRuleSet": AWSManagedRulesACFPRuleSetTypeDef,
     },
     total=False,
 )
 
+_RequiredLoggingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredLoggingConfigurationOutputTypeDef",
+    {
+        "ResourceArn": str,
+        "LogDestinationConfigs": List[str],
+    },
+)
+_OptionalLoggingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalLoggingConfigurationOutputTypeDef",
+    {
+        "RedactedFields": List[FieldToMatchOutputTypeDef],
+        "ManagedByFirewallManager": bool,
+        "LoggingFilter": LoggingFilterOutputTypeDef,
+    },
+    total=False,
+)
+
+class LoggingConfigurationOutputTypeDef(
+    _RequiredLoggingConfigurationOutputTypeDef, _OptionalLoggingConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredLoggingConfigurationTypeDef = TypedDict(
     "_RequiredLoggingConfigurationTypeDef",
     {
         "ResourceArn": str,
-        "LogDestinationConfigs": List[str],
+        "LogDestinationConfigs": Sequence[str],
     },
 )
 _OptionalLoggingConfigurationTypeDef = TypedDict(
     "_OptionalLoggingConfigurationTypeDef",
     {
-        "RedactedFields": List[FieldToMatchTypeDef],
+        "RedactedFields": Sequence[FieldToMatchTypeDef],
         "ManagedByFirewallManager": bool,
         "LoggingFilter": LoggingFilterTypeDef,
     },
     total=False,
 )
 
 class LoggingConfigurationTypeDef(
     _RequiredLoggingConfigurationTypeDef, _OptionalLoggingConfigurationTypeDef
 ):
     pass
 
-RuleActionOverrideTypeDef = TypedDict(
-    "RuleActionOverrideTypeDef",
+RuleActionOverrideOutputTypeDef = TypedDict(
+    "RuleActionOverrideOutputTypeDef",
     {
         "Name": str,
-        "ActionToUse": RuleActionTypeDef,
+        "ActionToUse": RuleActionOutputTypeDef,
+    },
+)
+
+_RequiredRuleOutputTypeDef = TypedDict(
+    "_RequiredRuleOutputTypeDef",
+    {
+        "Name": str,
+        "Priority": int,
+        "Statement": "StatementOutputTypeDef",
+        "VisibilityConfig": VisibilityConfigOutputTypeDef,
+    },
+)
+_OptionalRuleOutputTypeDef = TypedDict(
+    "_OptionalRuleOutputTypeDef",
+    {
+        "Action": RuleActionOutputTypeDef,
+        "OverrideAction": OverrideActionOutputTypeDef,
+        "RuleLabels": List[LabelOutputTypeDef],
+        "CaptchaConfig": CaptchaConfigOutputTypeDef,
+        "ChallengeConfig": ChallengeConfigOutputTypeDef,
     },
+    total=False,
 )
 
+class RuleOutputTypeDef(_RequiredRuleOutputTypeDef, _OptionalRuleOutputTypeDef):
+    pass
+
 RuleSummaryTypeDef = TypedDict(
     "RuleSummaryTypeDef",
     {
         "Name": str,
-        "Action": RuleActionTypeDef,
+        "Action": RuleActionOutputTypeDef,
     },
     total=False,
 )
 
+RuleActionOverrideTypeDef = TypedDict(
+    "RuleActionOverrideTypeDef",
+    {
+        "Name": str,
+        "ActionToUse": RuleActionTypeDef,
+    },
+)
+
 _RequiredRuleTypeDef = TypedDict(
     "_RequiredRuleTypeDef",
     {
         "Name": str,
         "Priority": int,
         "Statement": "StatementTypeDef",
         "VisibilityConfig": VisibilityConfigTypeDef,
@@ -2340,40 +3248,125 @@
 
 class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
 GetLoggingConfigurationResponseTypeDef = TypedDict(
     "GetLoggingConfigurationResponseTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLoggingConfigurationsResponseTypeDef = TypedDict(
     "ListLoggingConfigurationsResponseTypeDef",
     {
-        "LoggingConfigurations": List[LoggingConfigurationTypeDef],
+        "LoggingConfigurations": List[LoggingConfigurationOutputTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutLoggingConfigurationResponseTypeDef = TypedDict(
+    "PutLoggingConfigurationResponseTypeDef",
+    {
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "PutLoggingConfigurationRequestRequestTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
 )
 
-PutLoggingConfigurationResponseTypeDef = TypedDict(
-    "PutLoggingConfigurationResponseTypeDef",
+_RequiredManagedRuleGroupStatementOutputTypeDef = TypedDict(
+    "_RequiredManagedRuleGroupStatementOutputTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VendorName": str,
+        "Name": str,
+    },
+)
+_OptionalManagedRuleGroupStatementOutputTypeDef = TypedDict(
+    "_OptionalManagedRuleGroupStatementOutputTypeDef",
+    {
+        "Version": str,
+        "ExcludedRules": List[ExcludedRuleOutputTypeDef],
+        "ScopeDownStatement": Dict[str, Any],
+        "ManagedRuleGroupConfigs": List[ManagedRuleGroupConfigOutputTypeDef],
+        "RuleActionOverrides": List[RuleActionOverrideOutputTypeDef],
+    },
+    total=False,
+)
+
+class ManagedRuleGroupStatementOutputTypeDef(
+    _RequiredManagedRuleGroupStatementOutputTypeDef, _OptionalManagedRuleGroupStatementOutputTypeDef
+):
+    pass
+
+_RequiredRuleGroupReferenceStatementOutputTypeDef = TypedDict(
+    "_RequiredRuleGroupReferenceStatementOutputTypeDef",
+    {
+        "ARN": str,
+    },
+)
+_OptionalRuleGroupReferenceStatementOutputTypeDef = TypedDict(
+    "_OptionalRuleGroupReferenceStatementOutputTypeDef",
+    {
+        "ExcludedRules": List[ExcludedRuleOutputTypeDef],
+        "RuleActionOverrides": List[RuleActionOverrideOutputTypeDef],
+    },
+    total=False,
+)
+
+class RuleGroupReferenceStatementOutputTypeDef(
+    _RequiredRuleGroupReferenceStatementOutputTypeDef,
+    _OptionalRuleGroupReferenceStatementOutputTypeDef,
+):
+    pass
+
+_RequiredRuleGroupTypeDef = TypedDict(
+    "_RequiredRuleGroupTypeDef",
+    {
+        "Name": str,
+        "Id": str,
+        "Capacity": int,
+        "ARN": str,
+        "VisibilityConfig": VisibilityConfigOutputTypeDef,
+    },
+)
+_OptionalRuleGroupTypeDef = TypedDict(
+    "_OptionalRuleGroupTypeDef",
+    {
+        "Description": str,
+        "Rules": List[RuleOutputTypeDef],
+        "LabelNamespace": str,
+        "CustomResponseBodies": Dict[str, CustomResponseBodyOutputTypeDef],
+        "AvailableLabels": List[LabelSummaryTypeDef],
+        "ConsumedLabels": List[LabelSummaryTypeDef],
+    },
+    total=False,
+)
+
+class RuleGroupTypeDef(_RequiredRuleGroupTypeDef, _OptionalRuleGroupTypeDef):
+    pass
+
+DescribeManagedRuleGroupResponseTypeDef = TypedDict(
+    "DescribeManagedRuleGroupResponseTypeDef",
+    {
+        "VersionName": str,
+        "SnsTopicArn": str,
+        "Capacity": int,
+        "Rules": List[RuleSummaryTypeDef],
+        "LabelNamespace": str,
+        "AvailableLabels": List[LabelSummaryTypeDef],
+        "ConsumedLabels": List[LabelSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredManagedRuleGroupStatementTypeDef = TypedDict(
     "_RequiredManagedRuleGroupStatementTypeDef",
     {
         "VendorName": str,
@@ -2413,28 +3406,14 @@
 )
 
 class RuleGroupReferenceStatementTypeDef(
     _RequiredRuleGroupReferenceStatementTypeDef, _OptionalRuleGroupReferenceStatementTypeDef
 ):
     pass
 
-DescribeManagedRuleGroupResponseTypeDef = TypedDict(
-    "DescribeManagedRuleGroupResponseTypeDef",
-    {
-        "VersionName": str,
-        "SnsTopicArn": str,
-        "Capacity": int,
-        "Rules": List[RuleSummaryTypeDef],
-        "LabelNamespace": str,
-        "AvailableLabels": List[LabelSummaryTypeDef],
-        "ConsumedLabels": List[LabelSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CheckCapacityRequestRequestTypeDef = TypedDict(
     "CheckCapacityRequestRequestTypeDef",
     {
         "Scope": ScopeType,
         "Rules": Sequence[RuleTypeDef],
     },
 )
@@ -2489,40 +3468,14 @@
 )
 
 class CreateWebACLRequestRequestTypeDef(
     _RequiredCreateWebACLRequestRequestTypeDef, _OptionalCreateWebACLRequestRequestTypeDef
 ):
     pass
 
-_RequiredRuleGroupTypeDef = TypedDict(
-    "_RequiredRuleGroupTypeDef",
-    {
-        "Name": str,
-        "Id": str,
-        "Capacity": int,
-        "ARN": str,
-        "VisibilityConfig": VisibilityConfigTypeDef,
-    },
-)
-_OptionalRuleGroupTypeDef = TypedDict(
-    "_OptionalRuleGroupTypeDef",
-    {
-        "Description": str,
-        "Rules": List[RuleTypeDef],
-        "LabelNamespace": str,
-        "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
-        "AvailableLabels": List[LabelSummaryTypeDef],
-        "ConsumedLabels": List[LabelSummaryTypeDef],
-    },
-    total=False,
-)
-
-class RuleGroupTypeDef(_RequiredRuleGroupTypeDef, _OptionalRuleGroupTypeDef):
-    pass
-
 _RequiredUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleGroupRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "VisibilityConfig": VisibilityConfigTypeDef,
@@ -2573,20 +3526,51 @@
     _RequiredUpdateWebACLRequestRequestTypeDef, _OptionalUpdateWebACLRequestRequestTypeDef
 ):
     pass
 
 FirewallManagerStatementTypeDef = TypedDict(
     "FirewallManagerStatementTypeDef",
     {
-        "ManagedRuleGroupStatement": ManagedRuleGroupStatementTypeDef,
-        "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
+        "ManagedRuleGroupStatement": ManagedRuleGroupStatementOutputTypeDef,
+        "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
+    },
+    total=False,
+)
+
+StatementOutputTypeDef = TypedDict(
+    "StatementOutputTypeDef",
+    {
+        "ByteMatchStatement": ByteMatchStatementOutputTypeDef,
+        "SqliMatchStatement": SqliMatchStatementOutputTypeDef,
+        "XssMatchStatement": XssMatchStatementOutputTypeDef,
+        "SizeConstraintStatement": SizeConstraintStatementOutputTypeDef,
+        "GeoMatchStatement": GeoMatchStatementOutputTypeDef,
+        "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
+        "IPSetReferenceStatement": IPSetReferenceStatementOutputTypeDef,
+        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementOutputTypeDef,
+        "RateBasedStatement": Dict[str, Any],
+        "AndStatement": Dict[str, Any],
+        "OrStatement": Dict[str, Any],
+        "NotStatement": Dict[str, Any],
+        "ManagedRuleGroupStatement": Dict[str, Any],
+        "LabelMatchStatement": LabelMatchStatementOutputTypeDef,
+        "RegexMatchStatement": RegexMatchStatementOutputTypeDef,
     },
     total=False,
 )
 
+GetRuleGroupResponseTypeDef = TypedDict(
+    "GetRuleGroupResponseTypeDef",
+    {
+        "RuleGroup": RuleGroupTypeDef,
+        "LockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 StatementTypeDef = TypedDict(
     "StatementTypeDef",
     {
         "ByteMatchStatement": ByteMatchStatementTypeDef,
         "SqliMatchStatement": SqliMatchStatementTypeDef,
         "XssMatchStatement": XssMatchStatementTypeDef,
         "SizeConstraintStatement": SizeConstraintStatementTypeDef,
@@ -2601,76 +3585,67 @@
         "ManagedRuleGroupStatement": Dict[str, Any],
         "LabelMatchStatement": LabelMatchStatementTypeDef,
         "RegexMatchStatement": RegexMatchStatementTypeDef,
     },
     total=False,
 )
 
-GetRuleGroupResponseTypeDef = TypedDict(
-    "GetRuleGroupResponseTypeDef",
-    {
-        "RuleGroup": RuleGroupTypeDef,
-        "LockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FirewallManagerRuleGroupTypeDef = TypedDict(
     "FirewallManagerRuleGroupTypeDef",
     {
         "Name": str,
         "Priority": int,
         "FirewallManagerStatement": FirewallManagerStatementTypeDef,
-        "OverrideAction": OverrideActionTypeDef,
-        "VisibilityConfig": VisibilityConfigTypeDef,
+        "OverrideAction": OverrideActionOutputTypeDef,
+        "VisibilityConfig": VisibilityConfigOutputTypeDef,
     },
 )
 
 _RequiredWebACLTypeDef = TypedDict(
     "_RequiredWebACLTypeDef",
     {
         "Name": str,
         "Id": str,
         "ARN": str,
-        "DefaultAction": DefaultActionTypeDef,
-        "VisibilityConfig": VisibilityConfigTypeDef,
+        "DefaultAction": DefaultActionOutputTypeDef,
+        "VisibilityConfig": VisibilityConfigOutputTypeDef,
     },
 )
 _OptionalWebACLTypeDef = TypedDict(
     "_OptionalWebACLTypeDef",
     {
         "Description": str,
-        "Rules": List[RuleTypeDef],
+        "Rules": List[RuleOutputTypeDef],
         "Capacity": int,
         "PreProcessFirewallManagerRuleGroups": List[FirewallManagerRuleGroupTypeDef],
         "PostProcessFirewallManagerRuleGroups": List[FirewallManagerRuleGroupTypeDef],
         "ManagedByFirewallManager": bool,
         "LabelNamespace": str,
-        "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
-        "CaptchaConfig": CaptchaConfigTypeDef,
-        "ChallengeConfig": ChallengeConfigTypeDef,
+        "CustomResponseBodies": Dict[str, CustomResponseBodyOutputTypeDef],
+        "CaptchaConfig": CaptchaConfigOutputTypeDef,
+        "ChallengeConfig": ChallengeConfigOutputTypeDef,
         "TokenDomains": List[str],
-        "AssociationConfig": AssociationConfigTypeDef,
+        "AssociationConfig": AssociationConfigOutputTypeDef,
     },
     total=False,
 )
 
 class WebACLTypeDef(_RequiredWebACLTypeDef, _OptionalWebACLTypeDef):
     pass
 
 GetWebACLForResourceResponseTypeDef = TypedDict(
     "GetWebACLForResourceResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWebACLResponseTypeDef = TypedDict(
     "GetWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
         "LockToken": str,
         "ApplicationIntegrationURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2.egg-info/PKG-INFO` & `mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wafv2
-Version: 1.28.0
-Summary: Type annotations for boto3.WAFV2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.WAFV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-wafv2"></a>
 
 # mypy-boto3-wafv2
 
 [![PyPI - mypy-boto3-wafv2](https://img.shields.io/pypi/v/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wafv2?color=blue)](https://pypistats.org/packages/mypy-boto3-wafv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wafv2)](https://pepy.tech/project/mypy-boto3-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[boto3.WAFV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
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
 [mypy-boto3-wafv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,217 +322,302 @@
 
 `mypy_boto3_wafv2.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_wafv2.type_defs import (
     APIKeySummaryTypeDef,
+    AWSManagedRulesBotControlRuleSetOutputTypeDef,
     AWSManagedRulesBotControlRuleSetTypeDef,
+    ActionConditionOutputTypeDef,
     ActionConditionTypeDef,
+    AddressFieldOutputTypeDef,
     AddressFieldTypeDef,
+    AndStatementOutputTypeDef,
     AndStatementTypeDef,
     AssociateWebACLRequestRequestTypeDef,
+    RequestBodyAssociatedResourceTypeConfigOutputTypeDef,
     RequestBodyAssociatedResourceTypeConfigTypeDef,
+    BodyOutputTypeDef,
     BodyTypeDef,
+    TextTransformationOutputTypeDef,
     TextTransformationTypeDef,
+    ImmunityTimePropertyOutputTypeDef,
     ImmunityTimePropertyTypeDef,
     CaptchaResponseTypeDef,
     ChallengeResponseTypeDef,
-    CheckCapacityResponseTypeDef,
+    ResponseMetadataTypeDef,
+    LabelNameConditionOutputTypeDef,
     LabelNameConditionTypeDef,
+    CookieMatchPatternOutputTypeDef,
     CookieMatchPatternTypeDef,
     CreateAPIKeyRequestRequestTypeDef,
-    CreateAPIKeyResponseTypeDef,
     TagTypeDef,
     IPSetSummaryTypeDef,
     RegexTypeDef,
     RegexPatternSetSummaryTypeDef,
     CustomResponseBodyTypeDef,
     VisibilityConfigTypeDef,
     RuleGroupSummaryTypeDef,
     WebACLSummaryTypeDef,
+    CustomHTTPHeaderOutputTypeDef,
     CustomHTTPHeaderTypeDef,
+    CustomResponseBodyOutputTypeDef,
     DeleteFirewallManagerRuleGroupsRequestRequestTypeDef,
-    DeleteFirewallManagerRuleGroupsResponseTypeDef,
     DeleteIPSetRequestRequestTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeletePermissionPolicyRequestRequestTypeDef,
     DeleteRegexPatternSetRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteWebACLRequestRequestTypeDef,
     DescribeAllManagedProductsRequestRequestTypeDef,
     ManagedProductDescriptorTypeDef,
     DescribeManagedProductsByVendorRequestRequestTypeDef,
     DescribeManagedRuleGroupRequestRequestTypeDef,
     LabelSummaryTypeDef,
     DisassociateWebACLRequestRequestTypeDef,
+    EmailFieldOutputTypeDef,
     EmailFieldTypeDef,
+    ExcludedRuleOutputTypeDef,
     ExcludedRuleTypeDef,
+    HeaderOrderOutputTypeDef,
+    SingleHeaderOutputTypeDef,
+    SingleQueryArgumentOutputTypeDef,
     HeaderOrderTypeDef,
     SingleHeaderTypeDef,
     SingleQueryArgumentTypeDef,
+    VisibilityConfigOutputTypeDef,
+    ForwardedIPConfigOutputTypeDef,
     ForwardedIPConfigTypeDef,
     GenerateMobileSdkReleaseUrlRequestRequestTypeDef,
-    GenerateMobileSdkReleaseUrlResponseTypeDef,
     GetDecryptedAPIKeyRequestRequestTypeDef,
-    GetDecryptedAPIKeyResponseTypeDef,
     GetIPSetRequestRequestTypeDef,
     IPSetTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetManagedRuleSetRequestRequestTypeDef,
     GetMobileSdkReleaseRequestRequestTypeDef,
     GetPermissionPolicyRequestRequestTypeDef,
-    GetPermissionPolicyResponseTypeDef,
     GetRateBasedStatementManagedKeysRequestRequestTypeDef,
     RateBasedStatementManagedKeysIPSetTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
     TimeWindowTypeDef,
+    TimeWindowOutputTypeDef,
     GetWebACLForResourceRequestRequestTypeDef,
     GetWebACLRequestRequestTypeDef,
     HTTPHeaderTypeDef,
+    HeaderMatchPatternOutputTypeDef,
     HeaderMatchPatternTypeDef,
+    IPSetForwardedIPConfigOutputTypeDef,
     IPSetForwardedIPConfigTypeDef,
+    JsonMatchPatternOutputTypeDef,
     JsonMatchPatternTypeDef,
+    LabelMatchStatementOutputTypeDef,
     LabelMatchStatementTypeDef,
+    LabelOutputTypeDef,
     LabelTypeDef,
     ListAPIKeysRequestRequestTypeDef,
     ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef,
     ManagedRuleGroupVersionTypeDef,
     ListAvailableManagedRuleGroupsRequestRequestTypeDef,
     ManagedRuleGroupSummaryTypeDef,
     ListIPSetsRequestRequestTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
     ListManagedRuleSetsRequestRequestTypeDef,
     ManagedRuleSetSummaryTypeDef,
     ListMobileSdkReleasesRequestRequestTypeDef,
     ReleaseSummaryTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     ListResourcesForWebACLRequestRequestTypeDef,
-    ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
+    PasswordFieldOutputTypeDef,
+    UsernameFieldOutputTypeDef,
     PasswordFieldTypeDef,
     UsernameFieldTypeDef,
     ManagedRuleSetVersionTypeDef,
+    TagOutputTypeDef,
+    NotStatementOutputTypeDef,
     NotStatementTypeDef,
+    OrStatementOutputTypeDef,
     OrStatementTypeDef,
+    PhoneNumberFieldOutputTypeDef,
     PhoneNumberFieldTypeDef,
     VersionToPublishTypeDef,
-    PutManagedRuleSetVersionsResponseTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
+    RateLimitLabelNamespaceOutputTypeDef,
     RateLimitLabelNamespaceTypeDef,
+    RegexOutputTypeDef,
+    ResponseInspectionBodyContainsOutputTypeDef,
     ResponseInspectionBodyContainsTypeDef,
+    ResponseInspectionHeaderOutputTypeDef,
     ResponseInspectionHeaderTypeDef,
+    ResponseInspectionJsonOutputTypeDef,
     ResponseInspectionJsonTypeDef,
+    ResponseInspectionStatusCodeOutputTypeDef,
     ResponseInspectionStatusCodeTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
-    UpdateIPSetResponseTypeDef,
     UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
-    UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
-    UpdateRegexPatternSetResponseTypeDef,
-    UpdateRuleGroupResponseTypeDef,
-    UpdateWebACLResponseTypeDef,
-    ListAPIKeysResponseTypeDef,
+    AssociationConfigOutputTypeDef,
     AssociationConfigTypeDef,
+    RateLimitCookieOutputTypeDef,
+    RateLimitHeaderOutputTypeDef,
+    RateLimitQueryArgumentOutputTypeDef,
+    RateLimitQueryStringOutputTypeDef,
+    RateLimitUriPathOutputTypeDef,
     RateLimitCookieTypeDef,
     RateLimitHeaderTypeDef,
     RateLimitQueryArgumentTypeDef,
     RateLimitQueryStringTypeDef,
+    RateLimitUriPathTypeDef,
+    CaptchaConfigOutputTypeDef,
+    ChallengeConfigOutputTypeDef,
     CaptchaConfigTypeDef,
     ChallengeConfigTypeDef,
+    CheckCapacityResponseTypeDef,
+    CreateAPIKeyResponseTypeDef,
+    DeleteFirewallManagerRuleGroupsResponseTypeDef,
+    GenerateMobileSdkReleaseUrlResponseTypeDef,
+    GetDecryptedAPIKeyResponseTypeDef,
+    GetPermissionPolicyResponseTypeDef,
+    ListAPIKeysResponseTypeDef,
+    ListResourcesForWebACLResponseTypeDef,
+    PutManagedRuleSetVersionsResponseTypeDef,
+    UpdateIPSetResponseTypeDef,
+    UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
+    UpdateRegexPatternSetResponseTypeDef,
+    UpdateRuleGroupResponseTypeDef,
+    UpdateWebACLResponseTypeDef,
+    ConditionOutputTypeDef,
     ConditionTypeDef,
+    CookiesOutputTypeDef,
     CookiesTypeDef,
     CreateIPSetRequestRequestTypeDef,
-    MobileSdkReleaseTypeDef,
-    TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIPSetResponseTypeDef,
     ListIPSetsResponseTypeDef,
     CreateRegexPatternSetRequestRequestTypeDef,
-    RegexPatternSetTypeDef,
     UpdateRegexPatternSetRequestRequestTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     ListRegexPatternSetsResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     CreateWebACLResponseTypeDef,
     ListWebACLsResponseTypeDef,
+    CustomRequestHandlingOutputTypeDef,
+    CustomResponseOutputTypeDef,
     CustomRequestHandlingTypeDef,
     CustomResponseTypeDef,
     DescribeAllManagedProductsResponseTypeDef,
     DescribeManagedProductsByVendorResponseTypeDef,
+    GeoMatchStatementOutputTypeDef,
     GeoMatchStatementTypeDef,
     GetIPSetResponseTypeDef,
     GetRateBasedStatementManagedKeysResponseTypeDef,
     GetSampledRequestsRequestRequestTypeDef,
     HTTPRequestTypeDef,
+    HeadersOutputTypeDef,
     HeadersTypeDef,
+    IPSetReferenceStatementOutputTypeDef,
     IPSetReferenceStatementTypeDef,
+    JsonBodyOutputTypeDef,
     JsonBodyTypeDef,
     ListAvailableManagedRuleGroupVersionsResponseTypeDef,
     ListAvailableManagedRuleGroupsResponseTypeDef,
     ListManagedRuleSetsResponseTypeDef,
     ListMobileSdkReleasesResponseTypeDef,
+    RequestInspectionOutputTypeDef,
     RequestInspectionTypeDef,
     ManagedRuleSetTypeDef,
+    MobileSdkReleaseTypeDef,
+    TagInfoForResourceTypeDef,
+    RequestInspectionACFPOutputTypeDef,
     RequestInspectionACFPTypeDef,
     PutManagedRuleSetVersionsRequestRequestTypeDef,
+    RegexPatternSetTypeDef,
+    ResponseInspectionOutputTypeDef,
     ResponseInspectionTypeDef,
+    RateBasedStatementCustomKeyOutputTypeDef,
     RateBasedStatementCustomKeyTypeDef,
+    FilterOutputTypeDef,
     FilterTypeDef,
-    GetMobileSdkReleaseResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    GetRegexPatternSetResponseTypeDef,
+    AllowActionOutputTypeDef,
+    CaptchaActionOutputTypeDef,
+    ChallengeActionOutputTypeDef,
+    CountActionOutputTypeDef,
+    BlockActionOutputTypeDef,
     AllowActionTypeDef,
     CaptchaActionTypeDef,
     ChallengeActionTypeDef,
     CountActionTypeDef,
     BlockActionTypeDef,
     SampledHTTPRequestTypeDef,
+    FieldToMatchOutputTypeDef,
     FieldToMatchTypeDef,
     GetManagedRuleSetResponseTypeDef,
+    GetMobileSdkReleaseResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    GetRegexPatternSetResponseTypeDef,
+    AWSManagedRulesACFPRuleSetOutputTypeDef,
+    AWSManagedRulesATPRuleSetOutputTypeDef,
     AWSManagedRulesACFPRuleSetTypeDef,
     AWSManagedRulesATPRuleSetTypeDef,
+    RateBasedStatementOutputTypeDef,
     RateBasedStatementTypeDef,
+    LoggingFilterOutputTypeDef,
     LoggingFilterTypeDef,
+    OverrideActionOutputTypeDef,
+    DefaultActionOutputTypeDef,
+    RuleActionOutputTypeDef,
     OverrideActionTypeDef,
     DefaultActionTypeDef,
     RuleActionTypeDef,
     GetSampledRequestsResponseTypeDef,
+    ByteMatchStatementOutputTypeDef,
+    RegexMatchStatementOutputTypeDef,
+    RegexPatternSetReferenceStatementOutputTypeDef,
+    SizeConstraintStatementOutputTypeDef,
+    SqliMatchStatementOutputTypeDef,
+    XssMatchStatementOutputTypeDef,
     ByteMatchStatementTypeDef,
     RegexMatchStatementTypeDef,
     RegexPatternSetReferenceStatementTypeDef,
     SizeConstraintStatementTypeDef,
     SqliMatchStatementTypeDef,
     XssMatchStatementTypeDef,
+    ManagedRuleGroupConfigOutputTypeDef,
     ManagedRuleGroupConfigTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
-    RuleActionOverrideTypeDef,
+    RuleActionOverrideOutputTypeDef,
+    RuleOutputTypeDef,
     RuleSummaryTypeDef,
+    RuleActionOverrideTypeDef,
     RuleTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
-    PutLoggingConfigurationRequestRequestTypeDef,
     PutLoggingConfigurationResponseTypeDef,
+    PutLoggingConfigurationRequestRequestTypeDef,
+    ManagedRuleGroupStatementOutputTypeDef,
+    RuleGroupReferenceStatementOutputTypeDef,
+    RuleGroupTypeDef,
+    DescribeManagedRuleGroupResponseTypeDef,
     ManagedRuleGroupStatementTypeDef,
     RuleGroupReferenceStatementTypeDef,
-    DescribeManagedRuleGroupResponseTypeDef,
     CheckCapacityRequestRequestTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     CreateWebACLRequestRequestTypeDef,
-    RuleGroupTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
     UpdateWebACLRequestRequestTypeDef,
     FirewallManagerStatementTypeDef,
-    StatementTypeDef,
+    StatementOutputTypeDef,
     GetRuleGroupResponseTypeDef,
+    StatementTypeDef,
     FirewallManagerRuleGroupTypeDef,
     WebACLTypeDef,
     GetWebACLForResourceResponseTypeDef,
     GetWebACLResponseTypeDef,
 )
```

### Comparing `mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2.egg-info/SOURCES.txt` & `mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.28.0/setup.py` & `mypy-boto3-wafv2-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-wafv2",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_wafv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WAFV2 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.WAFV2 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

