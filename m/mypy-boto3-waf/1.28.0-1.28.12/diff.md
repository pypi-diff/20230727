# Comparing `tmp/mypy-boto3-waf-1.28.0.tar.gz` & `tmp/mypy-boto3-waf-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-waf-1.28.0.tar", last modified: Thu Jul  6 21:00:49 2023, max compression
+gzip compressed data, was "mypy-boto3-waf-1.28.12.tar", last modified: Thu Jul 27 11:49:49 2023, max compression
```

## Comparing `mypy-boto3-waf-1.28.0.tar` & `mypy-boto3-waf-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:49.914456 mypy-boto3-waf-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:57:37.000000 mypy-boto3-waf-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24240 2023-07-06 21:00:49.914456 mypy-boto3-waf-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22771 2023-07-06 20:57:37.000000 mypy-boto3-waf-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:49.914456 mypy-boto3-waf-1.28.0/mypy_boto3_waf/
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-06 20:57:37.000000 mypy-boto3-waf-1.28.0/mypy_boto3_waf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-06 20:57:37.000000 mypy-boto3-waf-1.28.0/mypy_boto3_waf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:57:37.000000 mypy-boto3-waf-1.28.0/mypy_boto3_waf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49442 2023-07-06 20:57:41.000000 mypy-boto3-waf-1.28.0/mypy_boto3_waf/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49342 2023-07-06 20:57:38.000000 mypy-boto3-waf-1.28.0/mypy_boto3_waf/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13676 2023-07-06 20:57:42.000000 mypy-boto3-waf-1.28.0/mypy_boto3_waf/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-07-06 20:57:42.000000 mypy-boto3-waf-1.28.0/mypy_boto3_waf/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17671 2023-07-06 20:57:42.000000 mypy-boto3-waf-1.28.0/mypy_boto3_waf/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-07-06 20:57:41.000000 mypy-boto3-waf-1.28.0/mypy_boto3_waf/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:57:37.000000 mypy-boto3-waf-1.28.0/mypy_boto3_waf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59242 2023-07-06 20:57:44.000000 mypy-boto3-waf-1.28.0/mypy_boto3_waf/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59195 2023-07-06 20:57:43.000000 mypy-boto3-waf-1.28.0/mypy_boto3_waf/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:57:37.000000 mypy-boto3-waf-1.28.0/mypy_boto3_waf/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:49.914456 mypy-boto3-waf-1.28.0/mypy_boto3_waf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24240 2023-07-06 21:00:49.000000 mypy-boto3-waf-1.28.0/mypy_boto3_waf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 21:00:49.000000 mypy-boto3-waf-1.28.0/mypy_boto3_waf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:49.000000 mypy-boto3-waf-1.28.0/mypy_boto3_waf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:49.000000 mypy-boto3-waf-1.28.0/mypy_boto3_waf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:49.000000 mypy-boto3-waf-1.28.0/mypy_boto3_waf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 21:00:49.000000 mypy-boto3-waf-1.28.0/mypy_boto3_waf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:49.914456 mypy-boto3-waf-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:57:37.000000 mypy-boto3-waf-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.097488 mypy-boto3-waf-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:22.000000 mypy-boto3-waf-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24753 2023-07-27 11:49:49.097488 mypy-boto3-waf-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23282 2023-07-27 11:48:22.000000 mypy-boto3-waf-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.097488 mypy-boto3-waf-1.28.12/mypy_boto3_waf/
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-27 11:48:22.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-27 11:48:22.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 11:48:22.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49442 2023-07-27 11:48:24.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49342 2023-07-27 11:48:24.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-07-27 11:48:25.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-27 11:48:25.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17639 2023-07-27 11:48:24.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17621 2023-07-27 11:48:24.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:22.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63705 2023-07-27 11:48:26.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63652 2023-07-27 11:48:25.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:22.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.097488 mypy-boto3-waf-1.28.12/mypy_boto3_waf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24753 2023-07-27 11:49:48.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 11:49:48.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:48.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:48.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:48.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:48.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:49.097488 mypy-boto3-waf-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 11:48:22.000000 mypy-boto3-waf-1.28.12/setup.py
```

### Comparing `mypy-boto3-waf-1.28.0/LICENSE` & `mypy-boto3-waf-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.0/PKG-INFO` & `mypy-boto3-waf-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-waf
-Version: 1.28.0
-Summary: Type annotations for boto3.WAF 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.WAF 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-waf"></a>
 
 # mypy-boto3-waf
 
 [![PyPI - mypy-boto3-waf](https://img.shields.io/pypi/v/mypy-boto3-waf.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-waf?color=blue)](https://pypistats.org/packages/mypy-boto3-waf)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-waf)](https://pepy.tech/project/mypy-boto3-waf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAF 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
+[boto3.WAF 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
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
 [mypy-boto3-waf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/).
 
 See how it helps to find and fix potential bugs:
 
@@ -401,164 +401,179 @@
 ### Typed dictionaries
 
 `mypy_boto3_waf.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_waf.type_defs import (
+    ExcludedRuleOutputTypeDef,
+    WafActionOutputTypeDef,
+    WafOverrideActionOutputTypeDef,
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
     ByteMatchSetSummaryTypeDef,
+    FieldToMatchOutputTypeDef,
     FieldToMatchTypeDef,
     CreateByteMatchSetRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateGeoMatchSetRequestRequestTypeDef,
     CreateIPSetRequestRequestTypeDef,
     TagTypeDef,
     CreateRegexMatchSetRequestRequestTypeDef,
     CreateRegexPatternSetRequestRequestTypeDef,
     RegexPatternSetTypeDef,
     RuleGroupTypeDef,
     CreateSizeConstraintSetRequestRequestTypeDef,
     CreateSqlInjectionMatchSetRequestRequestTypeDef,
     CreateWebACLMigrationStackRequestRequestTypeDef,
-    CreateWebACLMigrationStackResponseTypeDef,
     CreateXssMatchSetRequestRequestTypeDef,
     DeleteByteMatchSetRequestRequestTypeDef,
-    DeleteByteMatchSetResponseTypeDef,
     DeleteGeoMatchSetRequestRequestTypeDef,
-    DeleteGeoMatchSetResponseTypeDef,
     DeleteIPSetRequestRequestTypeDef,
-    DeleteIPSetResponseTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeletePermissionPolicyRequestRequestTypeDef,
     DeleteRateBasedRuleRequestRequestTypeDef,
-    DeleteRateBasedRuleResponseTypeDef,
     DeleteRegexMatchSetRequestRequestTypeDef,
-    DeleteRegexMatchSetResponseTypeDef,
     DeleteRegexPatternSetRequestRequestTypeDef,
-    DeleteRegexPatternSetResponseTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
-    DeleteRuleGroupResponseTypeDef,
     DeleteRuleRequestRequestTypeDef,
-    DeleteRuleResponseTypeDef,
     DeleteSizeConstraintSetRequestRequestTypeDef,
-    DeleteSizeConstraintSetResponseTypeDef,
     DeleteSqlInjectionMatchSetRequestRequestTypeDef,
-    DeleteSqlInjectionMatchSetResponseTypeDef,
     DeleteWebACLRequestRequestTypeDef,
-    DeleteWebACLResponseTypeDef,
     DeleteXssMatchSetRequestRequestTypeDef,
-    DeleteXssMatchSetResponseTypeDef,
+    GeoMatchConstraintOutputTypeDef,
     GeoMatchConstraintTypeDef,
     GeoMatchSetSummaryTypeDef,
     GetByteMatchSetRequestRequestTypeDef,
-    GetChangeTokenResponseTypeDef,
     GetChangeTokenStatusRequestRequestTypeDef,
-    GetChangeTokenStatusResponseTypeDef,
     GetGeoMatchSetRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetPermissionPolicyRequestRequestTypeDef,
-    GetPermissionPolicyResponseTypeDef,
-    GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetRateBasedRuleManagedKeysRequestRequestTypeDef,
-    GetRateBasedRuleManagedKeysResponseTypeDef,
     GetRateBasedRuleRequestRequestTypeDef,
     GetRegexMatchSetRequestRequestTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
     TimeWindowTypeDef,
+    TimeWindowOutputTypeDef,
     GetSizeConstraintSetRequestRequestTypeDef,
     GetSqlInjectionMatchSetRequestRequestTypeDef,
     GetWebACLRequestRequestTypeDef,
     GetXssMatchSetRequestRequestTypeDef,
     HTTPHeaderTypeDef,
+    IPSetDescriptorOutputTypeDef,
     IPSetDescriptorTypeDef,
     IPSetSummaryTypeDef,
-    ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef,
     ListActivatedRulesInRuleGroupRequestRequestTypeDef,
-    ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef,
     ListByteMatchSetsRequestRequestTypeDef,
-    ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef,
     ListGeoMatchSetsRequestRequestTypeDef,
-    ListIPSetsRequestListIPSetsPaginateTypeDef,
     ListIPSetsRequestRequestTypeDef,
-    ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
-    ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef,
     ListRateBasedRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
-    ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef,
     ListRegexMatchSetsRequestRequestTypeDef,
     RegexMatchSetSummaryTypeDef,
-    ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     RegexPatternSetSummaryTypeDef,
-    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupSummaryTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
-    ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef,
     ListSizeConstraintSetsRequestRequestTypeDef,
     SizeConstraintSetSummaryTypeDef,
-    ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef,
     ListSqlInjectionMatchSetsRequestRequestTypeDef,
     SqlInjectionMatchSetSummaryTypeDef,
-    ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef,
     ListSubscribedRuleGroupsRequestRequestTypeDef,
     SubscribedRuleGroupSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListWebACLsRequestListWebACLsPaginateTypeDef,
     ListWebACLsRequestRequestTypeDef,
     WebACLSummaryTypeDef,
-    ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef,
     ListXssMatchSetsRequestRequestTypeDef,
     XssMatchSetSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    PredicateOutputTypeDef,
     PredicateTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
     RegexPatternSetUpdateTypeDef,
-    ResponseMetadataTypeDef,
+    TagOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
+    ActivatedRuleOutputTypeDef,
+    ActivatedRuleTypeDef,
+    ByteMatchTupleOutputTypeDef,
+    LoggingConfigurationOutputTypeDef,
+    RegexMatchTupleOutputTypeDef,
+    SizeConstraintOutputTypeDef,
+    SqlInjectionMatchTupleOutputTypeDef,
+    XssMatchTupleOutputTypeDef,
+    ByteMatchTupleTypeDef,
+    LoggingConfigurationTypeDef,
+    RegexMatchTupleTypeDef,
+    SizeConstraintTypeDef,
+    SqlInjectionMatchTupleTypeDef,
+    XssMatchTupleTypeDef,
+    CreateWebACLMigrationStackResponseTypeDef,
+    DeleteByteMatchSetResponseTypeDef,
+    DeleteGeoMatchSetResponseTypeDef,
+    DeleteIPSetResponseTypeDef,
+    DeleteRateBasedRuleResponseTypeDef,
+    DeleteRegexMatchSetResponseTypeDef,
+    DeleteRegexPatternSetResponseTypeDef,
+    DeleteRuleGroupResponseTypeDef,
+    DeleteRuleResponseTypeDef,
+    DeleteSizeConstraintSetResponseTypeDef,
+    DeleteSqlInjectionMatchSetResponseTypeDef,
+    DeleteWebACLResponseTypeDef,
+    DeleteXssMatchSetResponseTypeDef,
+    GetChangeTokenResponseTypeDef,
+    GetChangeTokenStatusResponseTypeDef,
+    GetPermissionPolicyResponseTypeDef,
+    GetRateBasedRuleManagedKeysResponseTypeDef,
+    ListByteMatchSetsResponseTypeDef,
     UpdateByteMatchSetResponseTypeDef,
     UpdateGeoMatchSetResponseTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateRateBasedRuleResponseTypeDef,
     UpdateRegexMatchSetResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateRuleResponseTypeDef,
     UpdateSizeConstraintSetResponseTypeDef,
     UpdateSqlInjectionMatchSetResponseTypeDef,
     UpdateWebACLResponseTypeDef,
     UpdateXssMatchSetResponseTypeDef,
-    ActivatedRuleTypeDef,
-    ListByteMatchSetsResponseTypeDef,
-    ByteMatchTupleTypeDef,
-    LoggingConfigurationTypeDef,
-    RegexMatchTupleTypeDef,
-    SizeConstraintTypeDef,
-    SqlInjectionMatchTupleTypeDef,
-    XssMatchTupleTypeDef,
     CreateRateBasedRuleRequestRequestTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateWebACLRequestRequestTypeDef,
-    TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     GetRuleGroupResponseTypeDef,
     GeoMatchSetTypeDef,
     GeoMatchSetUpdateTypeDef,
     ListGeoMatchSetsResponseTypeDef,
+    GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
+    ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef,
+    ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef,
+    ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef,
+    ListIPSetsRequestListIPSetsPaginateTypeDef,
+    ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef,
+    ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef,
+    ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef,
+    ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef,
+    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
+    ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef,
+    ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef,
+    ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef,
+    ListWebACLsRequestListWebACLsPaginateTypeDef,
+    ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef,
     GetSampledRequestsRequestRequestTypeDef,
     HTTPRequestTypeDef,
     IPSetTypeDef,
     IPSetUpdateTypeDef,
     ListIPSetsResponseTypeDef,
     ListRateBasedRulesResponseTypeDef,
     ListRulesResponseTypeDef,
@@ -570,70 +585,71 @@
     ListSubscribedRuleGroupsResponseTypeDef,
     ListWebACLsResponseTypeDef,
     ListXssMatchSetsResponseTypeDef,
     RateBasedRuleTypeDef,
     RuleTypeDef,
     RuleUpdateTypeDef,
     UpdateRegexPatternSetRequestRequestTypeDef,
+    TagInfoForResourceTypeDef,
     ListActivatedRulesInRuleGroupResponseTypeDef,
-    RuleGroupUpdateTypeDef,
     WebACLTypeDef,
+    RuleGroupUpdateTypeDef,
     WebACLUpdateTypeDef,
     ByteMatchSetTypeDef,
-    ByteMatchSetUpdateTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
-    PutLoggingConfigurationRequestRequestTypeDef,
     PutLoggingConfigurationResponseTypeDef,
     RegexMatchSetTypeDef,
-    RegexMatchSetUpdateTypeDef,
     SizeConstraintSetTypeDef,
-    SizeConstraintSetUpdateTypeDef,
     SqlInjectionMatchSetTypeDef,
-    SqlInjectionMatchSetUpdateTypeDef,
     XssMatchSetTypeDef,
+    ByteMatchSetUpdateTypeDef,
+    PutLoggingConfigurationRequestRequestTypeDef,
+    RegexMatchSetUpdateTypeDef,
+    SizeConstraintSetUpdateTypeDef,
+    SqlInjectionMatchSetUpdateTypeDef,
     XssMatchSetUpdateTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CreateGeoMatchSetResponseTypeDef,
     GetGeoMatchSetResponseTypeDef,
     UpdateGeoMatchSetRequestRequestTypeDef,
     SampledHTTPRequestTypeDef,
     CreateIPSetResponseTypeDef,
     GetIPSetResponseTypeDef,
     UpdateIPSetRequestRequestTypeDef,
     CreateRateBasedRuleResponseTypeDef,
     GetRateBasedRuleResponseTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     UpdateRateBasedRuleRequestRequestTypeDef,
     UpdateRuleRequestRequestTypeDef,
-    UpdateRuleGroupRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateWebACLResponseTypeDef,
     GetWebACLResponseTypeDef,
+    UpdateRuleGroupRequestRequestTypeDef,
     UpdateWebACLRequestRequestTypeDef,
     CreateByteMatchSetResponseTypeDef,
     GetByteMatchSetResponseTypeDef,
-    UpdateByteMatchSetRequestRequestTypeDef,
     CreateRegexMatchSetResponseTypeDef,
     GetRegexMatchSetResponseTypeDef,
-    UpdateRegexMatchSetRequestRequestTypeDef,
     CreateSizeConstraintSetResponseTypeDef,
     GetSizeConstraintSetResponseTypeDef,
-    UpdateSizeConstraintSetRequestRequestTypeDef,
     CreateSqlInjectionMatchSetResponseTypeDef,
     GetSqlInjectionMatchSetResponseTypeDef,
-    UpdateSqlInjectionMatchSetRequestRequestTypeDef,
     CreateXssMatchSetResponseTypeDef,
     GetXssMatchSetResponseTypeDef,
+    UpdateByteMatchSetRequestRequestTypeDef,
+    UpdateRegexMatchSetRequestRequestTypeDef,
+    UpdateSizeConstraintSetRequestRequestTypeDef,
+    UpdateSqlInjectionMatchSetRequestRequestTypeDef,
     UpdateXssMatchSetRequestRequestTypeDef,
     GetSampledRequestsResponseTypeDef,
 )
 
 
-def get_structure() -> ExcludedRuleTypeDef:
+def get_structure() -> ExcludedRuleOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-waf-1.28.0/README.md` & `mypy-boto3-waf-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-waf"></a>
 
 # mypy-boto3-waf
 
 [![PyPI - mypy-boto3-waf](https://img.shields.io/pypi/v/mypy-boto3-waf.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-waf?color=blue)](https://pypistats.org/packages/mypy-boto3-waf)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-waf)](https://pepy.tech/project/mypy-boto3-waf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAF 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
+[boto3.WAF 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
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
 [mypy-boto3-waf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/).
 
 See how it helps to find and fix potential bugs:
 
@@ -369,164 +369,179 @@
 ### Typed dictionaries
 
 `mypy_boto3_waf.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_waf.type_defs import (
+    ExcludedRuleOutputTypeDef,
+    WafActionOutputTypeDef,
+    WafOverrideActionOutputTypeDef,
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
     ByteMatchSetSummaryTypeDef,
+    FieldToMatchOutputTypeDef,
     FieldToMatchTypeDef,
     CreateByteMatchSetRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateGeoMatchSetRequestRequestTypeDef,
     CreateIPSetRequestRequestTypeDef,
     TagTypeDef,
     CreateRegexMatchSetRequestRequestTypeDef,
     CreateRegexPatternSetRequestRequestTypeDef,
     RegexPatternSetTypeDef,
     RuleGroupTypeDef,
     CreateSizeConstraintSetRequestRequestTypeDef,
     CreateSqlInjectionMatchSetRequestRequestTypeDef,
     CreateWebACLMigrationStackRequestRequestTypeDef,
-    CreateWebACLMigrationStackResponseTypeDef,
     CreateXssMatchSetRequestRequestTypeDef,
     DeleteByteMatchSetRequestRequestTypeDef,
-    DeleteByteMatchSetResponseTypeDef,
     DeleteGeoMatchSetRequestRequestTypeDef,
-    DeleteGeoMatchSetResponseTypeDef,
     DeleteIPSetRequestRequestTypeDef,
-    DeleteIPSetResponseTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeletePermissionPolicyRequestRequestTypeDef,
     DeleteRateBasedRuleRequestRequestTypeDef,
-    DeleteRateBasedRuleResponseTypeDef,
     DeleteRegexMatchSetRequestRequestTypeDef,
-    DeleteRegexMatchSetResponseTypeDef,
     DeleteRegexPatternSetRequestRequestTypeDef,
-    DeleteRegexPatternSetResponseTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
-    DeleteRuleGroupResponseTypeDef,
     DeleteRuleRequestRequestTypeDef,
-    DeleteRuleResponseTypeDef,
     DeleteSizeConstraintSetRequestRequestTypeDef,
-    DeleteSizeConstraintSetResponseTypeDef,
     DeleteSqlInjectionMatchSetRequestRequestTypeDef,
-    DeleteSqlInjectionMatchSetResponseTypeDef,
     DeleteWebACLRequestRequestTypeDef,
-    DeleteWebACLResponseTypeDef,
     DeleteXssMatchSetRequestRequestTypeDef,
-    DeleteXssMatchSetResponseTypeDef,
+    GeoMatchConstraintOutputTypeDef,
     GeoMatchConstraintTypeDef,
     GeoMatchSetSummaryTypeDef,
     GetByteMatchSetRequestRequestTypeDef,
-    GetChangeTokenResponseTypeDef,
     GetChangeTokenStatusRequestRequestTypeDef,
-    GetChangeTokenStatusResponseTypeDef,
     GetGeoMatchSetRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetPermissionPolicyRequestRequestTypeDef,
-    GetPermissionPolicyResponseTypeDef,
-    GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetRateBasedRuleManagedKeysRequestRequestTypeDef,
-    GetRateBasedRuleManagedKeysResponseTypeDef,
     GetRateBasedRuleRequestRequestTypeDef,
     GetRegexMatchSetRequestRequestTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
     TimeWindowTypeDef,
+    TimeWindowOutputTypeDef,
     GetSizeConstraintSetRequestRequestTypeDef,
     GetSqlInjectionMatchSetRequestRequestTypeDef,
     GetWebACLRequestRequestTypeDef,
     GetXssMatchSetRequestRequestTypeDef,
     HTTPHeaderTypeDef,
+    IPSetDescriptorOutputTypeDef,
     IPSetDescriptorTypeDef,
     IPSetSummaryTypeDef,
-    ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef,
     ListActivatedRulesInRuleGroupRequestRequestTypeDef,
-    ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef,
     ListByteMatchSetsRequestRequestTypeDef,
-    ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef,
     ListGeoMatchSetsRequestRequestTypeDef,
-    ListIPSetsRequestListIPSetsPaginateTypeDef,
     ListIPSetsRequestRequestTypeDef,
-    ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
-    ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef,
     ListRateBasedRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
-    ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef,
     ListRegexMatchSetsRequestRequestTypeDef,
     RegexMatchSetSummaryTypeDef,
-    ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     RegexPatternSetSummaryTypeDef,
-    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupSummaryTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
-    ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef,
     ListSizeConstraintSetsRequestRequestTypeDef,
     SizeConstraintSetSummaryTypeDef,
-    ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef,
     ListSqlInjectionMatchSetsRequestRequestTypeDef,
     SqlInjectionMatchSetSummaryTypeDef,
-    ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef,
     ListSubscribedRuleGroupsRequestRequestTypeDef,
     SubscribedRuleGroupSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListWebACLsRequestListWebACLsPaginateTypeDef,
     ListWebACLsRequestRequestTypeDef,
     WebACLSummaryTypeDef,
-    ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef,
     ListXssMatchSetsRequestRequestTypeDef,
     XssMatchSetSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    PredicateOutputTypeDef,
     PredicateTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
     RegexPatternSetUpdateTypeDef,
-    ResponseMetadataTypeDef,
+    TagOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
+    ActivatedRuleOutputTypeDef,
+    ActivatedRuleTypeDef,
+    ByteMatchTupleOutputTypeDef,
+    LoggingConfigurationOutputTypeDef,
+    RegexMatchTupleOutputTypeDef,
+    SizeConstraintOutputTypeDef,
+    SqlInjectionMatchTupleOutputTypeDef,
+    XssMatchTupleOutputTypeDef,
+    ByteMatchTupleTypeDef,
+    LoggingConfigurationTypeDef,
+    RegexMatchTupleTypeDef,
+    SizeConstraintTypeDef,
+    SqlInjectionMatchTupleTypeDef,
+    XssMatchTupleTypeDef,
+    CreateWebACLMigrationStackResponseTypeDef,
+    DeleteByteMatchSetResponseTypeDef,
+    DeleteGeoMatchSetResponseTypeDef,
+    DeleteIPSetResponseTypeDef,
+    DeleteRateBasedRuleResponseTypeDef,
+    DeleteRegexMatchSetResponseTypeDef,
+    DeleteRegexPatternSetResponseTypeDef,
+    DeleteRuleGroupResponseTypeDef,
+    DeleteRuleResponseTypeDef,
+    DeleteSizeConstraintSetResponseTypeDef,
+    DeleteSqlInjectionMatchSetResponseTypeDef,
+    DeleteWebACLResponseTypeDef,
+    DeleteXssMatchSetResponseTypeDef,
+    GetChangeTokenResponseTypeDef,
+    GetChangeTokenStatusResponseTypeDef,
+    GetPermissionPolicyResponseTypeDef,
+    GetRateBasedRuleManagedKeysResponseTypeDef,
+    ListByteMatchSetsResponseTypeDef,
     UpdateByteMatchSetResponseTypeDef,
     UpdateGeoMatchSetResponseTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateRateBasedRuleResponseTypeDef,
     UpdateRegexMatchSetResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateRuleResponseTypeDef,
     UpdateSizeConstraintSetResponseTypeDef,
     UpdateSqlInjectionMatchSetResponseTypeDef,
     UpdateWebACLResponseTypeDef,
     UpdateXssMatchSetResponseTypeDef,
-    ActivatedRuleTypeDef,
-    ListByteMatchSetsResponseTypeDef,
-    ByteMatchTupleTypeDef,
-    LoggingConfigurationTypeDef,
-    RegexMatchTupleTypeDef,
-    SizeConstraintTypeDef,
-    SqlInjectionMatchTupleTypeDef,
-    XssMatchTupleTypeDef,
     CreateRateBasedRuleRequestRequestTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateWebACLRequestRequestTypeDef,
-    TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     GetRuleGroupResponseTypeDef,
     GeoMatchSetTypeDef,
     GeoMatchSetUpdateTypeDef,
     ListGeoMatchSetsResponseTypeDef,
+    GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
+    ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef,
+    ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef,
+    ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef,
+    ListIPSetsRequestListIPSetsPaginateTypeDef,
+    ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef,
+    ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef,
+    ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef,
+    ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef,
+    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
+    ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef,
+    ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef,
+    ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef,
+    ListWebACLsRequestListWebACLsPaginateTypeDef,
+    ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef,
     GetSampledRequestsRequestRequestTypeDef,
     HTTPRequestTypeDef,
     IPSetTypeDef,
     IPSetUpdateTypeDef,
     ListIPSetsResponseTypeDef,
     ListRateBasedRulesResponseTypeDef,
     ListRulesResponseTypeDef,
@@ -538,70 +553,71 @@
     ListSubscribedRuleGroupsResponseTypeDef,
     ListWebACLsResponseTypeDef,
     ListXssMatchSetsResponseTypeDef,
     RateBasedRuleTypeDef,
     RuleTypeDef,
     RuleUpdateTypeDef,
     UpdateRegexPatternSetRequestRequestTypeDef,
+    TagInfoForResourceTypeDef,
     ListActivatedRulesInRuleGroupResponseTypeDef,
-    RuleGroupUpdateTypeDef,
     WebACLTypeDef,
+    RuleGroupUpdateTypeDef,
     WebACLUpdateTypeDef,
     ByteMatchSetTypeDef,
-    ByteMatchSetUpdateTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
-    PutLoggingConfigurationRequestRequestTypeDef,
     PutLoggingConfigurationResponseTypeDef,
     RegexMatchSetTypeDef,
-    RegexMatchSetUpdateTypeDef,
     SizeConstraintSetTypeDef,
-    SizeConstraintSetUpdateTypeDef,
     SqlInjectionMatchSetTypeDef,
-    SqlInjectionMatchSetUpdateTypeDef,
     XssMatchSetTypeDef,
+    ByteMatchSetUpdateTypeDef,
+    PutLoggingConfigurationRequestRequestTypeDef,
+    RegexMatchSetUpdateTypeDef,
+    SizeConstraintSetUpdateTypeDef,
+    SqlInjectionMatchSetUpdateTypeDef,
     XssMatchSetUpdateTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CreateGeoMatchSetResponseTypeDef,
     GetGeoMatchSetResponseTypeDef,
     UpdateGeoMatchSetRequestRequestTypeDef,
     SampledHTTPRequestTypeDef,
     CreateIPSetResponseTypeDef,
     GetIPSetResponseTypeDef,
     UpdateIPSetRequestRequestTypeDef,
     CreateRateBasedRuleResponseTypeDef,
     GetRateBasedRuleResponseTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     UpdateRateBasedRuleRequestRequestTypeDef,
     UpdateRuleRequestRequestTypeDef,
-    UpdateRuleGroupRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateWebACLResponseTypeDef,
     GetWebACLResponseTypeDef,
+    UpdateRuleGroupRequestRequestTypeDef,
     UpdateWebACLRequestRequestTypeDef,
     CreateByteMatchSetResponseTypeDef,
     GetByteMatchSetResponseTypeDef,
-    UpdateByteMatchSetRequestRequestTypeDef,
     CreateRegexMatchSetResponseTypeDef,
     GetRegexMatchSetResponseTypeDef,
-    UpdateRegexMatchSetRequestRequestTypeDef,
     CreateSizeConstraintSetResponseTypeDef,
     GetSizeConstraintSetResponseTypeDef,
-    UpdateSizeConstraintSetRequestRequestTypeDef,
     CreateSqlInjectionMatchSetResponseTypeDef,
     GetSqlInjectionMatchSetResponseTypeDef,
-    UpdateSqlInjectionMatchSetRequestRequestTypeDef,
     CreateXssMatchSetResponseTypeDef,
     GetXssMatchSetResponseTypeDef,
+    UpdateByteMatchSetRequestRequestTypeDef,
+    UpdateRegexMatchSetRequestRequestTypeDef,
+    UpdateSizeConstraintSetRequestRequestTypeDef,
+    UpdateSqlInjectionMatchSetRequestRequestTypeDef,
     UpdateXssMatchSetRequestRequestTypeDef,
     GetSampledRequestsResponseTypeDef,
 )
 
 
-def get_structure() -> ExcludedRuleTypeDef:
+def get_structure() -> ExcludedRuleOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-waf-1.28.0/mypy_boto3_waf/__init__.py` & `mypy-boto3-waf-1.28.12/mypy_boto3_waf/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.0/mypy_boto3_waf/__init__.pyi` & `mypy-boto3-waf-1.28.12/mypy_boto3_waf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.0/mypy_boto3_waf/__main__.py` & `mypy-boto3-waf-1.28.12/mypy_boto3_waf/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WAF 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.WAF 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF\nOther"
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

### Comparing `mypy-boto3-waf-1.28.0/mypy_boto3_waf/client.py` & `mypy-boto3-waf-1.28.12/mypy_boto3_waf/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.0/mypy_boto3_waf/client.pyi` & `mypy-boto3-waf-1.28.12/mypy_boto3_waf/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.0/mypy_boto3_waf/literals.py` & `mypy-boto3-waf-1.28.12/mypy_boto3_waf/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -467,14 +467,15 @@
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
@@ -553,26 +554,28 @@
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

### Comparing `mypy-boto3-waf-1.28.0/mypy_boto3_waf/literals.pyi` & `mypy-boto3-waf-1.28.12/mypy_boto3_waf/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -465,14 +465,15 @@
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
@@ -551,26 +552,28 @@
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

### Comparing `mypy-boto3-waf-1.28.0/mypy_boto3_waf/paginator.py` & `mypy-boto3-waf-1.28.12/mypy_boto3_waf/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -88,256 +88,238 @@
     "ListSizeConstraintSetsPaginator",
     "ListSqlInjectionMatchSetsPaginator",
     "ListSubscribedRuleGroupsPaginator",
     "ListWebACLsPaginator",
     "ListXssMatchSetsPaginator",
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
 class GetRateBasedRuleManagedKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.GetRateBasedRuleManagedKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#getratebasedrulemanagedkeyspaginator)
     """
 
     def paginate(
-        self, *, RuleId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RuleId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRateBasedRuleManagedKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.GetRateBasedRuleManagedKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#getratebasedrulemanagedkeyspaginator)
         """
 
-
 class ListActivatedRulesInRuleGroupPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListActivatedRulesInRuleGroup)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listactivatedrulesinrulegrouppaginator)
     """
 
     def paginate(
-        self, *, RuleGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RuleGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListActivatedRulesInRuleGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListActivatedRulesInRuleGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listactivatedrulesinrulegrouppaginator)
         """
 
-
 class ListByteMatchSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListByteMatchSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listbytematchsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListByteMatchSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListByteMatchSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listbytematchsetspaginator)
         """
 
-
 class ListGeoMatchSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListGeoMatchSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listgeomatchsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGeoMatchSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListGeoMatchSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listgeomatchsetspaginator)
         """
 
-
 class ListIPSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListIPSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listipsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIPSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListIPSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listipsetspaginator)
         """
 
-
 class ListLoggingConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListLoggingConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listloggingconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLoggingConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListLoggingConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listloggingconfigurationspaginator)
         """
 
-
 class ListRateBasedRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRateBasedRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listratebasedrulespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRateBasedRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRateBasedRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listratebasedrulespaginator)
         """
 
-
 class ListRegexMatchSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRegexMatchSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listregexmatchsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRegexMatchSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRegexMatchSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listregexmatchsetspaginator)
         """
 
-
 class ListRegexPatternSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRegexPatternSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listregexpatternsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRegexPatternSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRegexPatternSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listregexpatternsetspaginator)
         """
 
-
 class ListRuleGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRuleGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listrulegroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRuleGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRuleGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listrulegroupspaginator)
         """
 
-
 class ListRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listrulespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listrulespaginator)
         """
 
-
 class ListSizeConstraintSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSizeConstraintSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listsizeconstraintsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSizeConstraintSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSizeConstraintSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listsizeconstraintsetspaginator)
         """
 
-
 class ListSqlInjectionMatchSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSqlInjectionMatchSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listsqlinjectionmatchsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSqlInjectionMatchSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSqlInjectionMatchSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listsqlinjectionmatchsetspaginator)
         """
 
-
 class ListSubscribedRuleGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSubscribedRuleGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listsubscribedrulegroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSubscribedRuleGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSubscribedRuleGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listsubscribedrulegroupspaginator)
         """
 
-
 class ListWebACLsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListWebACLs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listwebaclspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWebACLsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListWebACLs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listwebaclspaginator)
         """
 
-
 class ListXssMatchSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListXssMatchSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listxssmatchsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListXssMatchSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListXssMatchSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listxssmatchsetspaginator)
         """
```

### Comparing `mypy-boto3-waf-1.28.0/mypy_boto3_waf/paginator.pyi` & `mypy-boto3-waf-1.28.12/mypy_boto3_waf/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,238 +88,256 @@
     "ListSizeConstraintSetsPaginator",
     "ListSqlInjectionMatchSetsPaginator",
     "ListSubscribedRuleGroupsPaginator",
     "ListWebACLsPaginator",
     "ListXssMatchSetsPaginator",
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
 class GetRateBasedRuleManagedKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.GetRateBasedRuleManagedKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#getratebasedrulemanagedkeyspaginator)
     """
 
     def paginate(
-        self, *, RuleId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RuleId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRateBasedRuleManagedKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.GetRateBasedRuleManagedKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#getratebasedrulemanagedkeyspaginator)
         """
 
+
 class ListActivatedRulesInRuleGroupPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListActivatedRulesInRuleGroup)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listactivatedrulesinrulegrouppaginator)
     """
 
     def paginate(
-        self, *, RuleGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RuleGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListActivatedRulesInRuleGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListActivatedRulesInRuleGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listactivatedrulesinrulegrouppaginator)
         """
 
+
 class ListByteMatchSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListByteMatchSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listbytematchsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListByteMatchSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListByteMatchSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listbytematchsetspaginator)
         """
 
+
 class ListGeoMatchSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListGeoMatchSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listgeomatchsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGeoMatchSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListGeoMatchSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listgeomatchsetspaginator)
         """
 
+
 class ListIPSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListIPSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listipsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIPSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListIPSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listipsetspaginator)
         """
 
+
 class ListLoggingConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListLoggingConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listloggingconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLoggingConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListLoggingConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listloggingconfigurationspaginator)
         """
 
+
 class ListRateBasedRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRateBasedRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listratebasedrulespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRateBasedRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRateBasedRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listratebasedrulespaginator)
         """
 
+
 class ListRegexMatchSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRegexMatchSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listregexmatchsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRegexMatchSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRegexMatchSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listregexmatchsetspaginator)
         """
 
+
 class ListRegexPatternSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRegexPatternSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listregexpatternsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRegexPatternSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRegexPatternSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listregexpatternsetspaginator)
         """
 
+
 class ListRuleGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRuleGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listrulegroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRuleGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRuleGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listrulegroupspaginator)
         """
 
+
 class ListRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listrulespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listrulespaginator)
         """
 
+
 class ListSizeConstraintSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSizeConstraintSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listsizeconstraintsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSizeConstraintSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSizeConstraintSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listsizeconstraintsetspaginator)
         """
 
+
 class ListSqlInjectionMatchSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSqlInjectionMatchSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listsqlinjectionmatchsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSqlInjectionMatchSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSqlInjectionMatchSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listsqlinjectionmatchsetspaginator)
         """
 
+
 class ListSubscribedRuleGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSubscribedRuleGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listsubscribedrulegroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSubscribedRuleGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSubscribedRuleGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listsubscribedrulegroupspaginator)
         """
 
+
 class ListWebACLsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListWebACLs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listwebaclspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWebACLsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListWebACLs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listwebaclspaginator)
         """
 
+
 class ListXssMatchSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListXssMatchSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listxssmatchsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListXssMatchSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListXssMatchSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/paginators/#listxssmatchsetspaginator)
         """
```

### Comparing `mypy-boto3-waf-1.28.0/mypy_boto3_waf/type_defs.py` & `mypy-boto3-waf-1.28.12/mypy_boto3_waf/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 Type annotations for waf service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_waf.type_defs import ExcludedRuleTypeDef
+    from mypy_boto3_waf.type_defs import ExcludedRuleOutputTypeDef
 
-    data: ExcludedRuleTypeDef = {...}
+    data: ExcludedRuleOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import IO, Any, Dict, List, Sequence, Union
+
+from botocore.response import StreamingBody
 
 from .literals import (
     ChangeActionType,
     ChangeTokenStatusType,
     ComparisonOperatorType,
     GeoMatchConstraintValueType,
     IPSetDescriptorTypeType,
@@ -37,164 +39,179 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "ExcludedRuleOutputTypeDef",
+    "WafActionOutputTypeDef",
+    "WafOverrideActionOutputTypeDef",
     "ExcludedRuleTypeDef",
     "WafActionTypeDef",
     "WafOverrideActionTypeDef",
     "ByteMatchSetSummaryTypeDef",
+    "FieldToMatchOutputTypeDef",
     "FieldToMatchTypeDef",
     "CreateByteMatchSetRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateGeoMatchSetRequestRequestTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "TagTypeDef",
     "CreateRegexMatchSetRequestRequestTypeDef",
     "CreateRegexPatternSetRequestRequestTypeDef",
     "RegexPatternSetTypeDef",
     "RuleGroupTypeDef",
     "CreateSizeConstraintSetRequestRequestTypeDef",
     "CreateSqlInjectionMatchSetRequestRequestTypeDef",
     "CreateWebACLMigrationStackRequestRequestTypeDef",
-    "CreateWebACLMigrationStackResponseTypeDef",
     "CreateXssMatchSetRequestRequestTypeDef",
     "DeleteByteMatchSetRequestRequestTypeDef",
-    "DeleteByteMatchSetResponseTypeDef",
     "DeleteGeoMatchSetRequestRequestTypeDef",
-    "DeleteGeoMatchSetResponseTypeDef",
     "DeleteIPSetRequestRequestTypeDef",
-    "DeleteIPSetResponseTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeletePermissionPolicyRequestRequestTypeDef",
     "DeleteRateBasedRuleRequestRequestTypeDef",
-    "DeleteRateBasedRuleResponseTypeDef",
     "DeleteRegexMatchSetRequestRequestTypeDef",
-    "DeleteRegexMatchSetResponseTypeDef",
     "DeleteRegexPatternSetRequestRequestTypeDef",
-    "DeleteRegexPatternSetResponseTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
-    "DeleteRuleGroupResponseTypeDef",
     "DeleteRuleRequestRequestTypeDef",
-    "DeleteRuleResponseTypeDef",
     "DeleteSizeConstraintSetRequestRequestTypeDef",
-    "DeleteSizeConstraintSetResponseTypeDef",
     "DeleteSqlInjectionMatchSetRequestRequestTypeDef",
-    "DeleteSqlInjectionMatchSetResponseTypeDef",
     "DeleteWebACLRequestRequestTypeDef",
-    "DeleteWebACLResponseTypeDef",
     "DeleteXssMatchSetRequestRequestTypeDef",
-    "DeleteXssMatchSetResponseTypeDef",
+    "GeoMatchConstraintOutputTypeDef",
     "GeoMatchConstraintTypeDef",
     "GeoMatchSetSummaryTypeDef",
     "GetByteMatchSetRequestRequestTypeDef",
-    "GetChangeTokenResponseTypeDef",
     "GetChangeTokenStatusRequestRequestTypeDef",
-    "GetChangeTokenStatusResponseTypeDef",
     "GetGeoMatchSetRequestRequestTypeDef",
     "GetIPSetRequestRequestTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
     "GetPermissionPolicyRequestRequestTypeDef",
-    "GetPermissionPolicyResponseTypeDef",
-    "GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetRateBasedRuleManagedKeysRequestRequestTypeDef",
-    "GetRateBasedRuleManagedKeysResponseTypeDef",
     "GetRateBasedRuleRequestRequestTypeDef",
     "GetRegexMatchSetRequestRequestTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
     "GetRuleRequestRequestTypeDef",
     "TimeWindowTypeDef",
+    "TimeWindowOutputTypeDef",
     "GetSizeConstraintSetRequestRequestTypeDef",
     "GetSqlInjectionMatchSetRequestRequestTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "GetXssMatchSetRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
+    "IPSetDescriptorOutputTypeDef",
     "IPSetDescriptorTypeDef",
     "IPSetSummaryTypeDef",
-    "ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef",
     "ListActivatedRulesInRuleGroupRequestRequestTypeDef",
-    "ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef",
     "ListByteMatchSetsRequestRequestTypeDef",
-    "ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef",
     "ListGeoMatchSetsRequestRequestTypeDef",
-    "ListIPSetsRequestListIPSetsPaginateTypeDef",
     "ListIPSetsRequestRequestTypeDef",
-    "ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef",
     "ListLoggingConfigurationsRequestRequestTypeDef",
-    "ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef",
     "ListRateBasedRulesRequestRequestTypeDef",
     "RuleSummaryTypeDef",
-    "ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef",
     "ListRegexMatchSetsRequestRequestTypeDef",
     "RegexMatchSetSummaryTypeDef",
-    "ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef",
     "ListRegexPatternSetsRequestRequestTypeDef",
     "RegexPatternSetSummaryTypeDef",
-    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "RuleGroupSummaryTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
-    "ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef",
     "ListSizeConstraintSetsRequestRequestTypeDef",
     "SizeConstraintSetSummaryTypeDef",
-    "ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef",
     "ListSqlInjectionMatchSetsRequestRequestTypeDef",
     "SqlInjectionMatchSetSummaryTypeDef",
-    "ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef",
     "ListSubscribedRuleGroupsRequestRequestTypeDef",
     "SubscribedRuleGroupSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListWebACLsRequestListWebACLsPaginateTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "WebACLSummaryTypeDef",
-    "ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef",
     "ListXssMatchSetsRequestRequestTypeDef",
     "XssMatchSetSummaryTypeDef",
-    "PaginatorConfigTypeDef",
+    "PredicateOutputTypeDef",
     "PredicateTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
     "RegexPatternSetUpdateTypeDef",
-    "ResponseMetadataTypeDef",
+    "TagOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "ActivatedRuleOutputTypeDef",
+    "ActivatedRuleTypeDef",
+    "ByteMatchTupleOutputTypeDef",
+    "LoggingConfigurationOutputTypeDef",
+    "RegexMatchTupleOutputTypeDef",
+    "SizeConstraintOutputTypeDef",
+    "SqlInjectionMatchTupleOutputTypeDef",
+    "XssMatchTupleOutputTypeDef",
+    "ByteMatchTupleTypeDef",
+    "LoggingConfigurationTypeDef",
+    "RegexMatchTupleTypeDef",
+    "SizeConstraintTypeDef",
+    "SqlInjectionMatchTupleTypeDef",
+    "XssMatchTupleTypeDef",
+    "CreateWebACLMigrationStackResponseTypeDef",
+    "DeleteByteMatchSetResponseTypeDef",
+    "DeleteGeoMatchSetResponseTypeDef",
+    "DeleteIPSetResponseTypeDef",
+    "DeleteRateBasedRuleResponseTypeDef",
+    "DeleteRegexMatchSetResponseTypeDef",
+    "DeleteRegexPatternSetResponseTypeDef",
+    "DeleteRuleGroupResponseTypeDef",
+    "DeleteRuleResponseTypeDef",
+    "DeleteSizeConstraintSetResponseTypeDef",
+    "DeleteSqlInjectionMatchSetResponseTypeDef",
+    "DeleteWebACLResponseTypeDef",
+    "DeleteXssMatchSetResponseTypeDef",
+    "GetChangeTokenResponseTypeDef",
+    "GetChangeTokenStatusResponseTypeDef",
+    "GetPermissionPolicyResponseTypeDef",
+    "GetRateBasedRuleManagedKeysResponseTypeDef",
+    "ListByteMatchSetsResponseTypeDef",
     "UpdateByteMatchSetResponseTypeDef",
     "UpdateGeoMatchSetResponseTypeDef",
     "UpdateIPSetResponseTypeDef",
     "UpdateRateBasedRuleResponseTypeDef",
     "UpdateRegexMatchSetResponseTypeDef",
     "UpdateRegexPatternSetResponseTypeDef",
     "UpdateRuleGroupResponseTypeDef",
     "UpdateRuleResponseTypeDef",
     "UpdateSizeConstraintSetResponseTypeDef",
     "UpdateSqlInjectionMatchSetResponseTypeDef",
     "UpdateWebACLResponseTypeDef",
     "UpdateXssMatchSetResponseTypeDef",
-    "ActivatedRuleTypeDef",
-    "ListByteMatchSetsResponseTypeDef",
-    "ByteMatchTupleTypeDef",
-    "LoggingConfigurationTypeDef",
-    "RegexMatchTupleTypeDef",
-    "SizeConstraintTypeDef",
-    "SqlInjectionMatchTupleTypeDef",
-    "XssMatchTupleTypeDef",
     "CreateRateBasedRuleRequestRequestTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
     "CreateRuleRequestRequestTypeDef",
     "CreateWebACLRequestRequestTypeDef",
-    "TagInfoForResourceTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateRegexPatternSetResponseTypeDef",
     "GetRegexPatternSetResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "GetRuleGroupResponseTypeDef",
     "GeoMatchSetTypeDef",
     "GeoMatchSetUpdateTypeDef",
     "ListGeoMatchSetsResponseTypeDef",
+    "GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
+    "ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef",
+    "ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef",
+    "ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef",
+    "ListIPSetsRequestListIPSetsPaginateTypeDef",
+    "ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef",
+    "ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef",
+    "ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef",
+    "ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef",
+    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
+    "ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef",
+    "ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef",
+    "ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef",
+    "ListWebACLsRequestListWebACLsPaginateTypeDef",
+    "ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef",
     "GetSampledRequestsRequestRequestTypeDef",
     "HTTPRequestTypeDef",
     "IPSetTypeDef",
     "IPSetUpdateTypeDef",
     "ListIPSetsResponseTypeDef",
     "ListRateBasedRulesResponseTypeDef",
     "ListRulesResponseTypeDef",
@@ -206,68 +223,90 @@
     "ListSubscribedRuleGroupsResponseTypeDef",
     "ListWebACLsResponseTypeDef",
     "ListXssMatchSetsResponseTypeDef",
     "RateBasedRuleTypeDef",
     "RuleTypeDef",
     "RuleUpdateTypeDef",
     "UpdateRegexPatternSetRequestRequestTypeDef",
+    "TagInfoForResourceTypeDef",
     "ListActivatedRulesInRuleGroupResponseTypeDef",
-    "RuleGroupUpdateTypeDef",
     "WebACLTypeDef",
+    "RuleGroupUpdateTypeDef",
     "WebACLUpdateTypeDef",
     "ByteMatchSetTypeDef",
-    "ByteMatchSetUpdateTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
-    "PutLoggingConfigurationRequestRequestTypeDef",
     "PutLoggingConfigurationResponseTypeDef",
     "RegexMatchSetTypeDef",
-    "RegexMatchSetUpdateTypeDef",
     "SizeConstraintSetTypeDef",
-    "SizeConstraintSetUpdateTypeDef",
     "SqlInjectionMatchSetTypeDef",
-    "SqlInjectionMatchSetUpdateTypeDef",
     "XssMatchSetTypeDef",
+    "ByteMatchSetUpdateTypeDef",
+    "PutLoggingConfigurationRequestRequestTypeDef",
+    "RegexMatchSetUpdateTypeDef",
+    "SizeConstraintSetUpdateTypeDef",
+    "SqlInjectionMatchSetUpdateTypeDef",
     "XssMatchSetUpdateTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "CreateGeoMatchSetResponseTypeDef",
     "GetGeoMatchSetResponseTypeDef",
     "UpdateGeoMatchSetRequestRequestTypeDef",
     "SampledHTTPRequestTypeDef",
     "CreateIPSetResponseTypeDef",
     "GetIPSetResponseTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
     "CreateRateBasedRuleResponseTypeDef",
     "GetRateBasedRuleResponseTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "UpdateRateBasedRuleRequestRequestTypeDef",
     "UpdateRuleRequestRequestTypeDef",
-    "UpdateRuleGroupRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateWebACLResponseTypeDef",
     "GetWebACLResponseTypeDef",
+    "UpdateRuleGroupRequestRequestTypeDef",
     "UpdateWebACLRequestRequestTypeDef",
     "CreateByteMatchSetResponseTypeDef",
     "GetByteMatchSetResponseTypeDef",
-    "UpdateByteMatchSetRequestRequestTypeDef",
     "CreateRegexMatchSetResponseTypeDef",
     "GetRegexMatchSetResponseTypeDef",
-    "UpdateRegexMatchSetRequestRequestTypeDef",
     "CreateSizeConstraintSetResponseTypeDef",
     "GetSizeConstraintSetResponseTypeDef",
-    "UpdateSizeConstraintSetRequestRequestTypeDef",
     "CreateSqlInjectionMatchSetResponseTypeDef",
     "GetSqlInjectionMatchSetResponseTypeDef",
-    "UpdateSqlInjectionMatchSetRequestRequestTypeDef",
     "CreateXssMatchSetResponseTypeDef",
     "GetXssMatchSetResponseTypeDef",
+    "UpdateByteMatchSetRequestRequestTypeDef",
+    "UpdateRegexMatchSetRequestRequestTypeDef",
+    "UpdateSizeConstraintSetRequestRequestTypeDef",
+    "UpdateSqlInjectionMatchSetRequestRequestTypeDef",
     "UpdateXssMatchSetRequestRequestTypeDef",
     "GetSampledRequestsResponseTypeDef",
 )
 
+ExcludedRuleOutputTypeDef = TypedDict(
+    "ExcludedRuleOutputTypeDef",
+    {
+        "RuleId": str,
+    },
+)
+
+WafActionOutputTypeDef = TypedDict(
+    "WafActionOutputTypeDef",
+    {
+        "Type": WafActionTypeType,
+    },
+)
+
+WafOverrideActionOutputTypeDef = TypedDict(
+    "WafOverrideActionOutputTypeDef",
+    {
+        "Type": WafOverrideActionTypeType,
+    },
+)
+
 ExcludedRuleTypeDef = TypedDict(
     "ExcludedRuleTypeDef",
     {
         "RuleId": str,
     },
 )
 
@@ -289,14 +328,35 @@
     "ByteMatchSetSummaryTypeDef",
     {
         "ByteMatchSetId": str,
         "Name": str,
     },
 )
 
+_RequiredFieldToMatchOutputTypeDef = TypedDict(
+    "_RequiredFieldToMatchOutputTypeDef",
+    {
+        "Type": MatchFieldTypeType,
+    },
+)
+_OptionalFieldToMatchOutputTypeDef = TypedDict(
+    "_OptionalFieldToMatchOutputTypeDef",
+    {
+        "Data": str,
+    },
+    total=False,
+)
+
+
+class FieldToMatchOutputTypeDef(
+    _RequiredFieldToMatchOutputTypeDef, _OptionalFieldToMatchOutputTypeDef
+):
+    pass
+
+
 _RequiredFieldToMatchTypeDef = TypedDict(
     "_RequiredFieldToMatchTypeDef",
     {
         "Type": MatchFieldTypeType,
     },
 )
 _OptionalFieldToMatchTypeDef = TypedDict(
@@ -316,14 +376,25 @@
     "CreateByteMatchSetRequestRequestTypeDef",
     {
         "Name": str,
         "ChangeToken": str,
     },
 )
 
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
 CreateGeoMatchSetRequestRequestTypeDef = TypedDict(
     "CreateGeoMatchSetRequestRequestTypeDef",
     {
         "Name": str,
         "ChangeToken": str,
     },
 )
@@ -421,22 +492,14 @@
     {
         "WebACLId": str,
         "S3BucketName": str,
         "IgnoreUnsupportedType": bool,
     },
 )
 
-CreateWebACLMigrationStackResponseTypeDef = TypedDict(
-    "CreateWebACLMigrationStackResponseTypeDef",
-    {
-        "S3ObjectUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateXssMatchSetRequestRequestTypeDef = TypedDict(
     "CreateXssMatchSetRequestRequestTypeDef",
     {
         "Name": str,
         "ChangeToken": str,
     },
 )
@@ -445,54 +508,30 @@
     "DeleteByteMatchSetRequestRequestTypeDef",
     {
         "ByteMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteByteMatchSetResponseTypeDef = TypedDict(
-    "DeleteByteMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteGeoMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteGeoMatchSetRequestRequestTypeDef",
     {
         "GeoMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteGeoMatchSetResponseTypeDef = TypedDict(
-    "DeleteGeoMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteIPSetRequestRequestTypeDef = TypedDict(
     "DeleteIPSetRequestRequestTypeDef",
     {
         "IPSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteIPSetResponseTypeDef = TypedDict(
-    "DeleteIPSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -507,147 +546,83 @@
     "DeleteRateBasedRuleRequestRequestTypeDef",
     {
         "RuleId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteRateBasedRuleResponseTypeDef = TypedDict(
-    "DeleteRateBasedRuleResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRegexMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteRegexMatchSetRequestRequestTypeDef",
     {
         "RegexMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteRegexMatchSetResponseTypeDef = TypedDict(
-    "DeleteRegexMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRegexPatternSetRequestRequestTypeDef = TypedDict(
     "DeleteRegexPatternSetRequestRequestTypeDef",
     {
         "RegexPatternSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteRegexPatternSetResponseTypeDef = TypedDict(
-    "DeleteRegexPatternSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRuleGroupRequestRequestTypeDef = TypedDict(
     "DeleteRuleGroupRequestRequestTypeDef",
     {
         "RuleGroupId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteRuleGroupResponseTypeDef = TypedDict(
-    "DeleteRuleGroupResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "RuleId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteRuleResponseTypeDef = TypedDict(
-    "DeleteRuleResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSizeConstraintSetRequestRequestTypeDef = TypedDict(
     "DeleteSizeConstraintSetRequestRequestTypeDef",
     {
         "SizeConstraintSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteSizeConstraintSetResponseTypeDef = TypedDict(
-    "DeleteSizeConstraintSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSqlInjectionMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteSqlInjectionMatchSetRequestRequestTypeDef",
     {
         "SqlInjectionMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteSqlInjectionMatchSetResponseTypeDef = TypedDict(
-    "DeleteSqlInjectionMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWebACLRequestRequestTypeDef = TypedDict(
     "DeleteWebACLRequestRequestTypeDef",
     {
         "WebACLId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteWebACLResponseTypeDef = TypedDict(
-    "DeleteWebACLResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteXssMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteXssMatchSetRequestRequestTypeDef",
     {
         "XssMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteXssMatchSetResponseTypeDef = TypedDict(
-    "DeleteXssMatchSetResponseTypeDef",
+GeoMatchConstraintOutputTypeDef = TypedDict(
+    "GeoMatchConstraintOutputTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Type": Literal["Country"],
+        "Value": GeoMatchConstraintValueType,
     },
 )
 
 GeoMatchConstraintTypeDef = TypedDict(
     "GeoMatchConstraintTypeDef",
     {
         "Type": Literal["Country"],
@@ -666,37 +641,21 @@
 GetByteMatchSetRequestRequestTypeDef = TypedDict(
     "GetByteMatchSetRequestRequestTypeDef",
     {
         "ByteMatchSetId": str,
     },
 )
 
-GetChangeTokenResponseTypeDef = TypedDict(
-    "GetChangeTokenResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetChangeTokenStatusRequestRequestTypeDef = TypedDict(
     "GetChangeTokenStatusRequestRequestTypeDef",
     {
         "ChangeToken": str,
     },
 )
 
-GetChangeTokenStatusResponseTypeDef = TypedDict(
-    "GetChangeTokenStatusResponseTypeDef",
-    {
-        "ChangeTokenStatus": ChangeTokenStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetGeoMatchSetRequestRequestTypeDef = TypedDict(
     "GetGeoMatchSetRequestRequestTypeDef",
     {
         "GeoMatchSetId": str,
     },
 )
 
@@ -717,44 +676,24 @@
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
-_RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef = TypedDict(
-    "_RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
-    {
-        "RuleId": str,
-    },
-)
-_OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef = TypedDict(
-    "_OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
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
-class GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef(
-    _RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
-    _OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef = TypedDict(
     "_RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef",
     {
         "RuleId": str,
     },
 )
 _OptionalGetRateBasedRuleManagedKeysRequestRequestTypeDef = TypedDict(
@@ -769,23 +708,14 @@
 class GetRateBasedRuleManagedKeysRequestRequestTypeDef(
     _RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef,
     _OptionalGetRateBasedRuleManagedKeysRequestRequestTypeDef,
 ):
     pass
 
 
-GetRateBasedRuleManagedKeysResponseTypeDef = TypedDict(
-    "GetRateBasedRuleManagedKeysResponseTypeDef",
-    {
-        "ManagedKeys": List[str],
-        "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRateBasedRuleRequestRequestTypeDef = TypedDict(
     "GetRateBasedRuleRequestRequestTypeDef",
     {
         "RuleId": str,
     },
 )
 
@@ -821,14 +751,22 @@
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
 GetSizeConstraintSetRequestRequestTypeDef = TypedDict(
     "GetSizeConstraintSetRequestRequestTypeDef",
     {
         "SizeConstraintSetId": str,
     },
 )
 
@@ -858,14 +796,22 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
+IPSetDescriptorOutputTypeDef = TypedDict(
+    "IPSetDescriptorOutputTypeDef",
+    {
+        "Type": IPSetDescriptorTypeType,
+        "Value": str,
+    },
+)
+
 IPSetDescriptorTypeDef = TypedDict(
     "IPSetDescriptorTypeDef",
     {
         "Type": IPSetDescriptorTypeType,
         "Value": str,
     },
 )
@@ -874,109 +820,60 @@
     "IPSetSummaryTypeDef",
     {
         "IPSetId": str,
         "Name": str,
     },
 )
 
-ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef = TypedDict(
-    "ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef",
-    {
-        "RuleGroupId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListActivatedRulesInRuleGroupRequestRequestTypeDef = TypedDict(
     "ListActivatedRulesInRuleGroupRequestRequestTypeDef",
     {
         "RuleGroupId": str,
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef = TypedDict(
-    "ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListByteMatchSetsRequestRequestTypeDef = TypedDict(
     "ListByteMatchSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef = TypedDict(
-    "ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGeoMatchSetsRequestRequestTypeDef = TypedDict(
     "ListGeoMatchSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
-    "ListIPSetsRequestListIPSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListIPSetsRequestRequestTypeDef = TypedDict(
     "ListIPSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef = TypedDict(
-    "ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLoggingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListLoggingConfigurationsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef = TypedDict(
-    "ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRateBasedRulesRequestRequestTypeDef = TypedDict(
     "ListRateBasedRulesRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -986,22 +883,14 @@
     "RuleSummaryTypeDef",
     {
         "RuleId": str,
         "Name": str,
     },
 )
 
-ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef = TypedDict(
-    "ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRegexMatchSetsRequestRequestTypeDef = TypedDict(
     "ListRegexMatchSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1011,22 +900,14 @@
     "RegexMatchSetSummaryTypeDef",
     {
         "RegexMatchSetId": str,
         "Name": str,
     },
 )
 
-ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef = TypedDict(
-    "ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRegexPatternSetsRequestRequestTypeDef = TypedDict(
     "ListRegexPatternSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1036,22 +917,14 @@
     "RegexPatternSetSummaryTypeDef",
     {
         "RegexPatternSetId": str,
         "Name": str,
     },
 )
 
-ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = TypedDict(
-    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListRuleGroupsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1061,39 +934,23 @@
     "RuleGroupSummaryTypeDef",
     {
         "RuleGroupId": str,
         "Name": str,
     },
 )
 
-ListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "ListRulesRequestListRulesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRulesRequestRequestTypeDef = TypedDict(
     "ListRulesRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef = TypedDict(
-    "ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSizeConstraintSetsRequestRequestTypeDef = TypedDict(
     "ListSizeConstraintSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1103,22 +960,14 @@
     "SizeConstraintSetSummaryTypeDef",
     {
         "SizeConstraintSetId": str,
         "Name": str,
     },
 )
 
-ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef = TypedDict(
-    "ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSqlInjectionMatchSetsRequestRequestTypeDef = TypedDict(
     "ListSqlInjectionMatchSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1128,22 +977,14 @@
     "SqlInjectionMatchSetSummaryTypeDef",
     {
         "SqlInjectionMatchSetId": str,
         "Name": str,
     },
 )
 
-ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef = TypedDict(
-    "ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSubscribedRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListSubscribedRuleGroupsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1177,22 +1018,14 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-ListWebACLsRequestListWebACLsPaginateTypeDef = TypedDict(
-    "ListWebACLsRequestListWebACLsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWebACLsRequestRequestTypeDef = TypedDict(
     "ListWebACLsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1202,22 +1035,14 @@
     "WebACLSummaryTypeDef",
     {
         "WebACLId": str,
         "Name": str,
     },
 )
 
-ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef = TypedDict(
-    "ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListXssMatchSetsRequestRequestTypeDef = TypedDict(
     "ListXssMatchSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1227,22 +1052,21 @@
     "XssMatchSetSummaryTypeDef",
     {
         "XssMatchSetId": str,
         "Name": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+PredicateOutputTypeDef = TypedDict(
+    "PredicateOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Negated": bool,
+        "Type": PredicateTypeType,
+        "DataId": str,
     },
-    total=False,
 )
 
 PredicateTypeDef = TypedDict(
     "PredicateTypeDef",
     {
         "Negated": bool,
         "Type": PredicateTypeType,
@@ -1262,182 +1086,166 @@
     "RegexPatternSetUpdateTypeDef",
     {
         "Action": ChangeActionType,
         "RegexPatternString": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Key": str,
+        "Value": str,
     },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateByteMatchSetResponseTypeDef = TypedDict(
-    "UpdateByteMatchSetResponseTypeDef",
+_RequiredActivatedRuleOutputTypeDef = TypedDict(
+    "_RequiredActivatedRuleOutputTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Priority": int,
+        "RuleId": str,
     },
 )
-
-UpdateGeoMatchSetResponseTypeDef = TypedDict(
-    "UpdateGeoMatchSetResponseTypeDef",
+_OptionalActivatedRuleOutputTypeDef = TypedDict(
+    "_OptionalActivatedRuleOutputTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Action": WafActionOutputTypeDef,
+        "OverrideAction": WafOverrideActionOutputTypeDef,
+        "Type": WafRuleTypeType,
+        "ExcludedRules": List[ExcludedRuleOutputTypeDef],
     },
+    total=False,
 )
 
-UpdateIPSetResponseTypeDef = TypedDict(
-    "UpdateIPSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-UpdateRateBasedRuleResponseTypeDef = TypedDict(
-    "UpdateRateBasedRuleResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+class ActivatedRuleOutputTypeDef(
+    _RequiredActivatedRuleOutputTypeDef, _OptionalActivatedRuleOutputTypeDef
+):
+    pass
 
-UpdateRegexMatchSetResponseTypeDef = TypedDict(
-    "UpdateRegexMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-UpdateRegexPatternSetResponseTypeDef = TypedDict(
-    "UpdateRegexPatternSetResponseTypeDef",
+_RequiredActivatedRuleTypeDef = TypedDict(
+    "_RequiredActivatedRuleTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Priority": int,
+        "RuleId": str,
     },
 )
-
-UpdateRuleGroupResponseTypeDef = TypedDict(
-    "UpdateRuleGroupResponseTypeDef",
+_OptionalActivatedRuleTypeDef = TypedDict(
+    "_OptionalActivatedRuleTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Action": WafActionTypeDef,
+        "OverrideAction": WafOverrideActionTypeDef,
+        "Type": WafRuleTypeType,
+        "ExcludedRules": Sequence[ExcludedRuleTypeDef],
     },
+    total=False,
 )
 
-UpdateRuleResponseTypeDef = TypedDict(
-    "UpdateRuleResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-UpdateSizeConstraintSetResponseTypeDef = TypedDict(
-    "UpdateSizeConstraintSetResponseTypeDef",
+class ActivatedRuleTypeDef(_RequiredActivatedRuleTypeDef, _OptionalActivatedRuleTypeDef):
+    pass
+
+
+ByteMatchTupleOutputTypeDef = TypedDict(
+    "ByteMatchTupleOutputTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TargetString": bytes,
+        "TextTransformation": TextTransformationType,
+        "PositionalConstraint": PositionalConstraintType,
     },
 )
 
-UpdateSqlInjectionMatchSetResponseTypeDef = TypedDict(
-    "UpdateSqlInjectionMatchSetResponseTypeDef",
+_RequiredLoggingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredLoggingConfigurationOutputTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceArn": str,
+        "LogDestinationConfigs": List[str],
     },
 )
-
-UpdateWebACLResponseTypeDef = TypedDict(
-    "UpdateWebACLResponseTypeDef",
+_OptionalLoggingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalLoggingConfigurationOutputTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RedactedFields": List[FieldToMatchOutputTypeDef],
     },
+    total=False,
 )
 
-UpdateXssMatchSetResponseTypeDef = TypedDict(
-    "UpdateXssMatchSetResponseTypeDef",
+
+class LoggingConfigurationOutputTypeDef(
+    _RequiredLoggingConfigurationOutputTypeDef, _OptionalLoggingConfigurationOutputTypeDef
+):
+    pass
+
+
+RegexMatchTupleOutputTypeDef = TypedDict(
+    "RegexMatchTupleOutputTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformation": TextTransformationType,
+        "RegexPatternSetId": str,
     },
 )
 
-_RequiredActivatedRuleTypeDef = TypedDict(
-    "_RequiredActivatedRuleTypeDef",
+SizeConstraintOutputTypeDef = TypedDict(
+    "SizeConstraintOutputTypeDef",
     {
-        "Priority": int,
-        "RuleId": str,
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformation": TextTransformationType,
+        "ComparisonOperator": ComparisonOperatorType,
+        "Size": int,
     },
 )
-_OptionalActivatedRuleTypeDef = TypedDict(
-    "_OptionalActivatedRuleTypeDef",
+
+SqlInjectionMatchTupleOutputTypeDef = TypedDict(
+    "SqlInjectionMatchTupleOutputTypeDef",
     {
-        "Action": WafActionTypeDef,
-        "OverrideAction": WafOverrideActionTypeDef,
-        "Type": WafRuleTypeType,
-        "ExcludedRules": List[ExcludedRuleTypeDef],
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformation": TextTransformationType,
     },
-    total=False,
 )
 
-
-class ActivatedRuleTypeDef(_RequiredActivatedRuleTypeDef, _OptionalActivatedRuleTypeDef):
-    pass
-
-
-ListByteMatchSetsResponseTypeDef = TypedDict(
-    "ListByteMatchSetsResponseTypeDef",
+XssMatchTupleOutputTypeDef = TypedDict(
+    "XssMatchTupleOutputTypeDef",
     {
-        "NextMarker": str,
-        "ByteMatchSets": List[ByteMatchSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformation": TextTransformationType,
     },
 )
 
 ByteMatchTupleTypeDef = TypedDict(
     "ByteMatchTupleTypeDef",
     {
         "FieldToMatch": FieldToMatchTypeDef,
-        "TargetString": bytes,
+        "TargetString": Union[str, bytes, IO[Any], StreamingBody],
         "TextTransformation": TextTransformationType,
         "PositionalConstraint": PositionalConstraintType,
     },
 )
 
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
     },
     total=False,
 )
 
 
 class LoggingConfigurationTypeDef(
     _RequiredLoggingConfigurationTypeDef, _OptionalLoggingConfigurationTypeDef
@@ -1476,14 +1284,256 @@
     "XssMatchTupleTypeDef",
     {
         "FieldToMatch": FieldToMatchTypeDef,
         "TextTransformation": TextTransformationType,
     },
 )
 
+CreateWebACLMigrationStackResponseTypeDef = TypedDict(
+    "CreateWebACLMigrationStackResponseTypeDef",
+    {
+        "S3ObjectUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteByteMatchSetResponseTypeDef = TypedDict(
+    "DeleteByteMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteGeoMatchSetResponseTypeDef = TypedDict(
+    "DeleteGeoMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteIPSetResponseTypeDef = TypedDict(
+    "DeleteIPSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRateBasedRuleResponseTypeDef = TypedDict(
+    "DeleteRateBasedRuleResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRegexMatchSetResponseTypeDef = TypedDict(
+    "DeleteRegexMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRegexPatternSetResponseTypeDef = TypedDict(
+    "DeleteRegexPatternSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRuleGroupResponseTypeDef = TypedDict(
+    "DeleteRuleGroupResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRuleResponseTypeDef = TypedDict(
+    "DeleteRuleResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSizeConstraintSetResponseTypeDef = TypedDict(
+    "DeleteSizeConstraintSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSqlInjectionMatchSetResponseTypeDef = TypedDict(
+    "DeleteSqlInjectionMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteWebACLResponseTypeDef = TypedDict(
+    "DeleteWebACLResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteXssMatchSetResponseTypeDef = TypedDict(
+    "DeleteXssMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetChangeTokenResponseTypeDef = TypedDict(
+    "GetChangeTokenResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetChangeTokenStatusResponseTypeDef = TypedDict(
+    "GetChangeTokenStatusResponseTypeDef",
+    {
+        "ChangeTokenStatus": ChangeTokenStatusType,
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
+GetRateBasedRuleManagedKeysResponseTypeDef = TypedDict(
+    "GetRateBasedRuleManagedKeysResponseTypeDef",
+    {
+        "ManagedKeys": List[str],
+        "NextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListByteMatchSetsResponseTypeDef = TypedDict(
+    "ListByteMatchSetsResponseTypeDef",
+    {
+        "NextMarker": str,
+        "ByteMatchSets": List[ByteMatchSetSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateByteMatchSetResponseTypeDef = TypedDict(
+    "UpdateByteMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGeoMatchSetResponseTypeDef = TypedDict(
+    "UpdateGeoMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateIPSetResponseTypeDef = TypedDict(
+    "UpdateIPSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRateBasedRuleResponseTypeDef = TypedDict(
+    "UpdateRateBasedRuleResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRegexMatchSetResponseTypeDef = TypedDict(
+    "UpdateRegexMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRegexPatternSetResponseTypeDef = TypedDict(
+    "UpdateRegexPatternSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRuleGroupResponseTypeDef = TypedDict(
+    "UpdateRuleGroupResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRuleResponseTypeDef = TypedDict(
+    "UpdateRuleResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSizeConstraintSetResponseTypeDef = TypedDict(
+    "UpdateSizeConstraintSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSqlInjectionMatchSetResponseTypeDef = TypedDict(
+    "UpdateSqlInjectionMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWebACLResponseTypeDef = TypedDict(
+    "UpdateWebACLResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateXssMatchSetResponseTypeDef = TypedDict(
+    "UpdateXssMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateRateBasedRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRateBasedRuleRequestRequestTypeDef",
     {
         "Name": str,
         "MetricName": str,
         "RateKey": Literal["IP"],
         "RateLimit": int,
@@ -1572,70 +1622,61 @@
 
 class CreateWebACLRequestRequestTypeDef(
     _RequiredCreateWebACLRequestRequestTypeDef, _OptionalCreateWebACLRequestRequestTypeDef
 ):
     pass
 
 
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
 
 CreateRegexPatternSetResponseTypeDef = TypedDict(
     "CreateRegexPatternSetResponseTypeDef",
     {
         "RegexPatternSet": RegexPatternSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRegexPatternSetResponseTypeDef = TypedDict(
     "GetRegexPatternSetResponseTypeDef",
     {
         "RegexPatternSet": RegexPatternSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRuleGroupResponseTypeDef = TypedDict(
     "CreateRuleGroupResponseTypeDef",
     {
         "RuleGroup": RuleGroupTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRuleGroupResponseTypeDef = TypedDict(
     "GetRuleGroupResponseTypeDef",
     {
         "RuleGroup": RuleGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGeoMatchSetTypeDef = TypedDict(
     "_RequiredGeoMatchSetTypeDef",
     {
         "GeoMatchSetId": str,
-        "GeoMatchConstraints": List[GeoMatchConstraintTypeDef],
+        "GeoMatchConstraints": List[GeoMatchConstraintOutputTypeDef],
     },
 )
 _OptionalGeoMatchSetTypeDef = TypedDict(
     "_OptionalGeoMatchSetTypeDef",
     {
         "Name": str,
     },
@@ -1656,16 +1697,159 @@
 )
 
 ListGeoMatchSetsResponseTypeDef = TypedDict(
     "ListGeoMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "GeoMatchSets": List[GeoMatchSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef = TypedDict(
+    "_RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
+    {
+        "RuleId": str,
+    },
+)
+_OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef = TypedDict(
+    "_OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef(
+    _RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
+    _OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
+):
+    pass
+
+
+ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef = TypedDict(
+    "ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef",
+    {
+        "RuleGroupId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef = TypedDict(
+    "ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef = TypedDict(
+    "ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
+    "ListIPSetsRequestListIPSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef = TypedDict(
+    "ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef = TypedDict(
+    "ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef = TypedDict(
+    "ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef = TypedDict(
+    "ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = TypedDict(
+    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "ListRulesRequestListRulesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef = TypedDict(
+    "ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef = TypedDict(
+    "ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef = TypedDict(
+    "ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWebACLsRequestListWebACLsPaginateTypeDef = TypedDict(
+    "ListWebACLsRequestListWebACLsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef = TypedDict(
+    "ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 GetSampledRequestsRequestRequestTypeDef = TypedDict(
     "GetSampledRequestsRequestRequestTypeDef",
     {
         "WebAclId": str,
         "RuleId": str,
@@ -1687,15 +1871,15 @@
     total=False,
 )
 
 _RequiredIPSetTypeDef = TypedDict(
     "_RequiredIPSetTypeDef",
     {
         "IPSetId": str,
-        "IPSetDescriptors": List[IPSetDescriptorTypeDef],
+        "IPSetDescriptors": List[IPSetDescriptorOutputTypeDef],
     },
 )
 _OptionalIPSetTypeDef = TypedDict(
     "_OptionalIPSetTypeDef",
     {
         "Name": str,
     },
@@ -1716,113 +1900,113 @@
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
 
 ListRateBasedRulesResponseTypeDef = TypedDict(
     "ListRateBasedRulesResponseTypeDef",
     {
         "NextMarker": str,
         "Rules": List[RuleSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "NextMarker": str,
         "Rules": List[RuleSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRegexMatchSetsResponseTypeDef = TypedDict(
     "ListRegexMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "RegexMatchSets": List[RegexMatchSetSummaryTypeDef],
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
 
 ListRuleGroupsResponseTypeDef = TypedDict(
     "ListRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "RuleGroups": List[RuleGroupSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSizeConstraintSetsResponseTypeDef = TypedDict(
     "ListSizeConstraintSetsResponseTypeDef",
     {
         "NextMarker": str,
         "SizeConstraintSets": List[SizeConstraintSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSqlInjectionMatchSetsResponseTypeDef = TypedDict(
     "ListSqlInjectionMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "SqlInjectionMatchSets": List[SqlInjectionMatchSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSubscribedRuleGroupsResponseTypeDef = TypedDict(
     "ListSubscribedRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "RuleGroups": List[SubscribedRuleGroupSummaryTypeDef],
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
     },
 )
 
 ListXssMatchSetsResponseTypeDef = TypedDict(
     "ListXssMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "XssMatchSets": List[XssMatchSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRateBasedRuleTypeDef = TypedDict(
     "_RequiredRateBasedRuleTypeDef",
     {
         "RuleId": str,
-        "MatchPredicates": List[PredicateTypeDef],
+        "MatchPredicates": List[PredicateOutputTypeDef],
         "RateKey": Literal["IP"],
         "RateLimit": int,
     },
 )
 _OptionalRateBasedRuleTypeDef = TypedDict(
     "_OptionalRateBasedRuleTypeDef",
     {
@@ -1837,15 +2021,15 @@
     pass
 
 
 _RequiredRuleTypeDef = TypedDict(
     "_RequiredRuleTypeDef",
     {
         "RuleId": str,
-        "Predicates": List[PredicateTypeDef],
+        "Predicates": List[PredicateOutputTypeDef],
     },
 )
 _OptionalRuleTypeDef = TypedDict(
     "_OptionalRuleTypeDef",
     {
         "Name": str,
         "MetricName": str,
@@ -1871,37 +2055,38 @@
     {
         "RegexPatternSetId": str,
         "Updates": Sequence[RegexPatternSetUpdateTypeDef],
         "ChangeToken": str,
     },
 )
 
-ListActivatedRulesInRuleGroupResponseTypeDef = TypedDict(
-    "ListActivatedRulesInRuleGroupResponseTypeDef",
+TagInfoForResourceTypeDef = TypedDict(
+    "TagInfoForResourceTypeDef",
     {
-        "NextMarker": str,
-        "ActivatedRules": List[ActivatedRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceARN": str,
+        "TagList": List[TagOutputTypeDef],
     },
+    total=False,
 )
 
-RuleGroupUpdateTypeDef = TypedDict(
-    "RuleGroupUpdateTypeDef",
+ListActivatedRulesInRuleGroupResponseTypeDef = TypedDict(
+    "ListActivatedRulesInRuleGroupResponseTypeDef",
     {
-        "Action": ChangeActionType,
-        "ActivatedRule": ActivatedRuleTypeDef,
+        "NextMarker": str,
+        "ActivatedRules": List[ActivatedRuleOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredWebACLTypeDef = TypedDict(
     "_RequiredWebACLTypeDef",
     {
         "WebACLId": str,
-        "DefaultAction": WafActionTypeDef,
-        "Rules": List[ActivatedRuleTypeDef],
+        "DefaultAction": WafActionOutputTypeDef,
+        "Rules": List[ActivatedRuleOutputTypeDef],
     },
 )
 _OptionalWebACLTypeDef = TypedDict(
     "_OptionalWebACLTypeDef",
     {
         "Name": str,
         "MetricName": str,
@@ -1911,27 +2096,35 @@
 )
 
 
 class WebACLTypeDef(_RequiredWebACLTypeDef, _OptionalWebACLTypeDef):
     pass
 
 
+RuleGroupUpdateTypeDef = TypedDict(
+    "RuleGroupUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "ActivatedRule": ActivatedRuleTypeDef,
+    },
+)
+
 WebACLUpdateTypeDef = TypedDict(
     "WebACLUpdateTypeDef",
     {
         "Action": ChangeActionType,
         "ActivatedRule": ActivatedRuleTypeDef,
     },
 )
 
 _RequiredByteMatchSetTypeDef = TypedDict(
     "_RequiredByteMatchSetTypeDef",
     {
         "ByteMatchSetId": str,
-        "ByteMatchTuples": List[ByteMatchTupleTypeDef],
+        "ByteMatchTuples": List[ByteMatchTupleOutputTypeDef],
     },
 )
 _OptionalByteMatchSetTypeDef = TypedDict(
     "_OptionalByteMatchSetTypeDef",
     {
         "Name": str,
     },
@@ -1939,77 +2132,54 @@
 )
 
 
 class ByteMatchSetTypeDef(_RequiredByteMatchSetTypeDef, _OptionalByteMatchSetTypeDef):
     pass
 
 
-ByteMatchSetUpdateTypeDef = TypedDict(
-    "ByteMatchSetUpdateTypeDef",
-    {
-        "Action": ChangeActionType,
-        "ByteMatchTuple": ByteMatchTupleTypeDef,
-    },
-)
-
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
-    },
-)
-
-PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutLoggingConfigurationRequestRequestTypeDef",
-    {
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutLoggingConfigurationResponseTypeDef = TypedDict(
     "PutLoggingConfigurationResponseTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegexMatchSetTypeDef = TypedDict(
     "RegexMatchSetTypeDef",
     {
         "RegexMatchSetId": str,
         "Name": str,
-        "RegexMatchTuples": List[RegexMatchTupleTypeDef],
+        "RegexMatchTuples": List[RegexMatchTupleOutputTypeDef],
     },
     total=False,
 )
 
-RegexMatchSetUpdateTypeDef = TypedDict(
-    "RegexMatchSetUpdateTypeDef",
-    {
-        "Action": ChangeActionType,
-        "RegexMatchTuple": RegexMatchTupleTypeDef,
-    },
-)
-
 _RequiredSizeConstraintSetTypeDef = TypedDict(
     "_RequiredSizeConstraintSetTypeDef",
     {
         "SizeConstraintSetId": str,
-        "SizeConstraints": List[SizeConstraintTypeDef],
+        "SizeConstraints": List[SizeConstraintOutputTypeDef],
     },
 )
 _OptionalSizeConstraintSetTypeDef = TypedDict(
     "_OptionalSizeConstraintSetTypeDef",
     {
         "Name": str,
     },
@@ -2019,27 +2189,19 @@
 
 class SizeConstraintSetTypeDef(
     _RequiredSizeConstraintSetTypeDef, _OptionalSizeConstraintSetTypeDef
 ):
     pass
 
 
-SizeConstraintSetUpdateTypeDef = TypedDict(
-    "SizeConstraintSetUpdateTypeDef",
-    {
-        "Action": ChangeActionType,
-        "SizeConstraint": SizeConstraintTypeDef,
-    },
-)
-
 _RequiredSqlInjectionMatchSetTypeDef = TypedDict(
     "_RequiredSqlInjectionMatchSetTypeDef",
     {
         "SqlInjectionMatchSetId": str,
-        "SqlInjectionMatchTuples": List[SqlInjectionMatchTupleTypeDef],
+        "SqlInjectionMatchTuples": List[SqlInjectionMatchTupleOutputTypeDef],
     },
 )
 _OptionalSqlInjectionMatchSetTypeDef = TypedDict(
     "_OptionalSqlInjectionMatchSetTypeDef",
     {
         "Name": str,
     },
@@ -2049,27 +2211,19 @@
 
 class SqlInjectionMatchSetTypeDef(
     _RequiredSqlInjectionMatchSetTypeDef, _OptionalSqlInjectionMatchSetTypeDef
 ):
     pass
 
 
-SqlInjectionMatchSetUpdateTypeDef = TypedDict(
-    "SqlInjectionMatchSetUpdateTypeDef",
-    {
-        "Action": ChangeActionType,
-        "SqlInjectionMatchTuple": SqlInjectionMatchTupleTypeDef,
-    },
-)
-
 _RequiredXssMatchSetTypeDef = TypedDict(
     "_RequiredXssMatchSetTypeDef",
     {
         "XssMatchSetId": str,
-        "XssMatchTuples": List[XssMatchTupleTypeDef],
+        "XssMatchTuples": List[XssMatchTupleOutputTypeDef],
     },
 )
 _OptionalXssMatchSetTypeDef = TypedDict(
     "_OptionalXssMatchSetTypeDef",
     {
         "Name": str,
     },
@@ -2077,45 +2231,75 @@
 )
 
 
 class XssMatchSetTypeDef(_RequiredXssMatchSetTypeDef, _OptionalXssMatchSetTypeDef):
     pass
 
 
-XssMatchSetUpdateTypeDef = TypedDict(
-    "XssMatchSetUpdateTypeDef",
+ByteMatchSetUpdateTypeDef = TypedDict(
+    "ByteMatchSetUpdateTypeDef",
     {
         "Action": ChangeActionType,
-        "XssMatchTuple": XssMatchTupleTypeDef,
+        "ByteMatchTuple": ByteMatchTupleTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutLoggingConfigurationRequestRequestTypeDef",
     {
-        "NextMarker": str,
-        "TagInfoForResource": TagInfoForResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
+    },
+)
+
+RegexMatchSetUpdateTypeDef = TypedDict(
+    "RegexMatchSetUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "RegexMatchTuple": RegexMatchTupleTypeDef,
+    },
+)
+
+SizeConstraintSetUpdateTypeDef = TypedDict(
+    "SizeConstraintSetUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "SizeConstraint": SizeConstraintTypeDef,
+    },
+)
+
+SqlInjectionMatchSetUpdateTypeDef = TypedDict(
+    "SqlInjectionMatchSetUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "SqlInjectionMatchTuple": SqlInjectionMatchTupleTypeDef,
+    },
+)
+
+XssMatchSetUpdateTypeDef = TypedDict(
+    "XssMatchSetUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "XssMatchTuple": XssMatchTupleTypeDef,
     },
 )
 
 CreateGeoMatchSetResponseTypeDef = TypedDict(
     "CreateGeoMatchSetResponseTypeDef",
     {
         "GeoMatchSet": GeoMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGeoMatchSetResponseTypeDef = TypedDict(
     "GetGeoMatchSetResponseTypeDef",
     {
         "GeoMatchSet": GeoMatchSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGeoMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateGeoMatchSetRequestRequestTypeDef",
     {
         "GeoMatchSetId": str,
@@ -2149,23 +2333,23 @@
 
 
 CreateIPSetResponseTypeDef = TypedDict(
     "CreateIPSetResponseTypeDef",
     {
         "IPSet": IPSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIPSetResponseTypeDef = TypedDict(
     "GetIPSetResponseTypeDef",
     {
         "IPSet": IPSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIPSetRequestRequestTypeDef = TypedDict(
     "UpdateIPSetRequestRequestTypeDef",
     {
         "IPSetId": str,
@@ -2175,40 +2359,40 @@
 )
 
 CreateRateBasedRuleResponseTypeDef = TypedDict(
     "CreateRateBasedRuleResponseTypeDef",
     {
         "Rule": RateBasedRuleTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRateBasedRuleResponseTypeDef = TypedDict(
     "GetRateBasedRuleResponseTypeDef",
     {
         "Rule": RateBasedRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRuleResponseTypeDef = TypedDict(
     "CreateRuleResponseTypeDef",
     {
         "Rule": RuleTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
         "Rule": RuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRateBasedRuleRequestRequestTypeDef = TypedDict(
     "UpdateRateBasedRuleRequestRequestTypeDef",
     {
         "RuleId": str,
@@ -2223,37 +2407,46 @@
     {
         "RuleId": str,
         "ChangeToken": str,
         "Updates": Sequence[RuleUpdateTypeDef],
     },
 )
 
-UpdateRuleGroupRequestRequestTypeDef = TypedDict(
-    "UpdateRuleGroupRequestRequestTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "RuleGroupId": str,
-        "Updates": Sequence[RuleGroupUpdateTypeDef],
-        "ChangeToken": str,
+        "NextMarker": str,
+        "TagInfoForResource": TagInfoForResourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWebACLResponseTypeDef = TypedDict(
     "CreateWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWebACLResponseTypeDef = TypedDict(
     "GetWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRuleGroupRequestRequestTypeDef = TypedDict(
+    "UpdateRuleGroupRequestRequestTypeDef",
+    {
+        "RuleGroupId": str,
+        "Updates": Sequence[RuleGroupUpdateTypeDef],
+        "ChangeToken": str,
     },
 )
 
 _RequiredUpdateWebACLRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWebACLRequestRequestTypeDef",
     {
         "WebACLId": str,
@@ -2277,127 +2470,127 @@
 
 
 CreateByteMatchSetResponseTypeDef = TypedDict(
     "CreateByteMatchSetResponseTypeDef",
     {
         "ByteMatchSet": ByteMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetByteMatchSetResponseTypeDef = TypedDict(
     "GetByteMatchSetResponseTypeDef",
     {
         "ByteMatchSet": ByteMatchSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateByteMatchSetRequestRequestTypeDef = TypedDict(
-    "UpdateByteMatchSetRequestRequestTypeDef",
-    {
-        "ByteMatchSetId": str,
-        "ChangeToken": str,
-        "Updates": Sequence[ByteMatchSetUpdateTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRegexMatchSetResponseTypeDef = TypedDict(
     "CreateRegexMatchSetResponseTypeDef",
     {
         "RegexMatchSet": RegexMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRegexMatchSetResponseTypeDef = TypedDict(
     "GetRegexMatchSetResponseTypeDef",
     {
         "RegexMatchSet": RegexMatchSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateRegexMatchSetRequestRequestTypeDef = TypedDict(
-    "UpdateRegexMatchSetRequestRequestTypeDef",
-    {
-        "RegexMatchSetId": str,
-        "Updates": Sequence[RegexMatchSetUpdateTypeDef],
-        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSizeConstraintSetResponseTypeDef = TypedDict(
     "CreateSizeConstraintSetResponseTypeDef",
     {
         "SizeConstraintSet": SizeConstraintSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSizeConstraintSetResponseTypeDef = TypedDict(
     "GetSizeConstraintSetResponseTypeDef",
     {
         "SizeConstraintSet": SizeConstraintSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSizeConstraintSetRequestRequestTypeDef = TypedDict(
-    "UpdateSizeConstraintSetRequestRequestTypeDef",
-    {
-        "SizeConstraintSetId": str,
-        "ChangeToken": str,
-        "Updates": Sequence[SizeConstraintSetUpdateTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSqlInjectionMatchSetResponseTypeDef = TypedDict(
     "CreateSqlInjectionMatchSetResponseTypeDef",
     {
         "SqlInjectionMatchSet": SqlInjectionMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSqlInjectionMatchSetResponseTypeDef = TypedDict(
     "GetSqlInjectionMatchSetResponseTypeDef",
     {
         "SqlInjectionMatchSet": SqlInjectionMatchSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSqlInjectionMatchSetRequestRequestTypeDef = TypedDict(
-    "UpdateSqlInjectionMatchSetRequestRequestTypeDef",
-    {
-        "SqlInjectionMatchSetId": str,
-        "ChangeToken": str,
-        "Updates": Sequence[SqlInjectionMatchSetUpdateTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateXssMatchSetResponseTypeDef = TypedDict(
     "CreateXssMatchSetResponseTypeDef",
     {
         "XssMatchSet": XssMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetXssMatchSetResponseTypeDef = TypedDict(
     "GetXssMatchSetResponseTypeDef",
     {
         "XssMatchSet": XssMatchSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateByteMatchSetRequestRequestTypeDef = TypedDict(
+    "UpdateByteMatchSetRequestRequestTypeDef",
+    {
+        "ByteMatchSetId": str,
+        "ChangeToken": str,
+        "Updates": Sequence[ByteMatchSetUpdateTypeDef],
+    },
+)
+
+UpdateRegexMatchSetRequestRequestTypeDef = TypedDict(
+    "UpdateRegexMatchSetRequestRequestTypeDef",
+    {
+        "RegexMatchSetId": str,
+        "Updates": Sequence[RegexMatchSetUpdateTypeDef],
+        "ChangeToken": str,
+    },
+)
+
+UpdateSizeConstraintSetRequestRequestTypeDef = TypedDict(
+    "UpdateSizeConstraintSetRequestRequestTypeDef",
+    {
+        "SizeConstraintSetId": str,
+        "ChangeToken": str,
+        "Updates": Sequence[SizeConstraintSetUpdateTypeDef],
+    },
+)
+
+UpdateSqlInjectionMatchSetRequestRequestTypeDef = TypedDict(
+    "UpdateSqlInjectionMatchSetRequestRequestTypeDef",
+    {
+        "SqlInjectionMatchSetId": str,
+        "ChangeToken": str,
+        "Updates": Sequence[SqlInjectionMatchSetUpdateTypeDef],
     },
 )
 
 UpdateXssMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateXssMatchSetRequestRequestTypeDef",
     {
         "XssMatchSetId": str,
@@ -2407,11 +2600,11 @@
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
     },
 )
```

### Comparing `mypy-boto3-waf-1.28.0/mypy_boto3_waf/type_defs.pyi` & `mypy-boto3-waf-1.28.12/mypy_boto3_waf/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 Type annotations for waf service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_waf.type_defs import ExcludedRuleTypeDef
+    from mypy_boto3_waf.type_defs import ExcludedRuleOutputTypeDef
 
-    data: ExcludedRuleTypeDef = {...}
+    data: ExcludedRuleOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import IO, Any, Dict, List, Sequence, Union
+
+from botocore.response import StreamingBody
 
 from .literals import (
     ChangeActionType,
     ChangeTokenStatusType,
     ComparisonOperatorType,
     GeoMatchConstraintValueType,
     IPSetDescriptorTypeType,
@@ -36,164 +38,179 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "ExcludedRuleOutputTypeDef",
+    "WafActionOutputTypeDef",
+    "WafOverrideActionOutputTypeDef",
     "ExcludedRuleTypeDef",
     "WafActionTypeDef",
     "WafOverrideActionTypeDef",
     "ByteMatchSetSummaryTypeDef",
+    "FieldToMatchOutputTypeDef",
     "FieldToMatchTypeDef",
     "CreateByteMatchSetRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateGeoMatchSetRequestRequestTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "TagTypeDef",
     "CreateRegexMatchSetRequestRequestTypeDef",
     "CreateRegexPatternSetRequestRequestTypeDef",
     "RegexPatternSetTypeDef",
     "RuleGroupTypeDef",
     "CreateSizeConstraintSetRequestRequestTypeDef",
     "CreateSqlInjectionMatchSetRequestRequestTypeDef",
     "CreateWebACLMigrationStackRequestRequestTypeDef",
-    "CreateWebACLMigrationStackResponseTypeDef",
     "CreateXssMatchSetRequestRequestTypeDef",
     "DeleteByteMatchSetRequestRequestTypeDef",
-    "DeleteByteMatchSetResponseTypeDef",
     "DeleteGeoMatchSetRequestRequestTypeDef",
-    "DeleteGeoMatchSetResponseTypeDef",
     "DeleteIPSetRequestRequestTypeDef",
-    "DeleteIPSetResponseTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeletePermissionPolicyRequestRequestTypeDef",
     "DeleteRateBasedRuleRequestRequestTypeDef",
-    "DeleteRateBasedRuleResponseTypeDef",
     "DeleteRegexMatchSetRequestRequestTypeDef",
-    "DeleteRegexMatchSetResponseTypeDef",
     "DeleteRegexPatternSetRequestRequestTypeDef",
-    "DeleteRegexPatternSetResponseTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
-    "DeleteRuleGroupResponseTypeDef",
     "DeleteRuleRequestRequestTypeDef",
-    "DeleteRuleResponseTypeDef",
     "DeleteSizeConstraintSetRequestRequestTypeDef",
-    "DeleteSizeConstraintSetResponseTypeDef",
     "DeleteSqlInjectionMatchSetRequestRequestTypeDef",
-    "DeleteSqlInjectionMatchSetResponseTypeDef",
     "DeleteWebACLRequestRequestTypeDef",
-    "DeleteWebACLResponseTypeDef",
     "DeleteXssMatchSetRequestRequestTypeDef",
-    "DeleteXssMatchSetResponseTypeDef",
+    "GeoMatchConstraintOutputTypeDef",
     "GeoMatchConstraintTypeDef",
     "GeoMatchSetSummaryTypeDef",
     "GetByteMatchSetRequestRequestTypeDef",
-    "GetChangeTokenResponseTypeDef",
     "GetChangeTokenStatusRequestRequestTypeDef",
-    "GetChangeTokenStatusResponseTypeDef",
     "GetGeoMatchSetRequestRequestTypeDef",
     "GetIPSetRequestRequestTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
     "GetPermissionPolicyRequestRequestTypeDef",
-    "GetPermissionPolicyResponseTypeDef",
-    "GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetRateBasedRuleManagedKeysRequestRequestTypeDef",
-    "GetRateBasedRuleManagedKeysResponseTypeDef",
     "GetRateBasedRuleRequestRequestTypeDef",
     "GetRegexMatchSetRequestRequestTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
     "GetRuleRequestRequestTypeDef",
     "TimeWindowTypeDef",
+    "TimeWindowOutputTypeDef",
     "GetSizeConstraintSetRequestRequestTypeDef",
     "GetSqlInjectionMatchSetRequestRequestTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "GetXssMatchSetRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
+    "IPSetDescriptorOutputTypeDef",
     "IPSetDescriptorTypeDef",
     "IPSetSummaryTypeDef",
-    "ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef",
     "ListActivatedRulesInRuleGroupRequestRequestTypeDef",
-    "ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef",
     "ListByteMatchSetsRequestRequestTypeDef",
-    "ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef",
     "ListGeoMatchSetsRequestRequestTypeDef",
-    "ListIPSetsRequestListIPSetsPaginateTypeDef",
     "ListIPSetsRequestRequestTypeDef",
-    "ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef",
     "ListLoggingConfigurationsRequestRequestTypeDef",
-    "ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef",
     "ListRateBasedRulesRequestRequestTypeDef",
     "RuleSummaryTypeDef",
-    "ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef",
     "ListRegexMatchSetsRequestRequestTypeDef",
     "RegexMatchSetSummaryTypeDef",
-    "ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef",
     "ListRegexPatternSetsRequestRequestTypeDef",
     "RegexPatternSetSummaryTypeDef",
-    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "RuleGroupSummaryTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
-    "ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef",
     "ListSizeConstraintSetsRequestRequestTypeDef",
     "SizeConstraintSetSummaryTypeDef",
-    "ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef",
     "ListSqlInjectionMatchSetsRequestRequestTypeDef",
     "SqlInjectionMatchSetSummaryTypeDef",
-    "ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef",
     "ListSubscribedRuleGroupsRequestRequestTypeDef",
     "SubscribedRuleGroupSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListWebACLsRequestListWebACLsPaginateTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "WebACLSummaryTypeDef",
-    "ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef",
     "ListXssMatchSetsRequestRequestTypeDef",
     "XssMatchSetSummaryTypeDef",
-    "PaginatorConfigTypeDef",
+    "PredicateOutputTypeDef",
     "PredicateTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
     "RegexPatternSetUpdateTypeDef",
-    "ResponseMetadataTypeDef",
+    "TagOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "ActivatedRuleOutputTypeDef",
+    "ActivatedRuleTypeDef",
+    "ByteMatchTupleOutputTypeDef",
+    "LoggingConfigurationOutputTypeDef",
+    "RegexMatchTupleOutputTypeDef",
+    "SizeConstraintOutputTypeDef",
+    "SqlInjectionMatchTupleOutputTypeDef",
+    "XssMatchTupleOutputTypeDef",
+    "ByteMatchTupleTypeDef",
+    "LoggingConfigurationTypeDef",
+    "RegexMatchTupleTypeDef",
+    "SizeConstraintTypeDef",
+    "SqlInjectionMatchTupleTypeDef",
+    "XssMatchTupleTypeDef",
+    "CreateWebACLMigrationStackResponseTypeDef",
+    "DeleteByteMatchSetResponseTypeDef",
+    "DeleteGeoMatchSetResponseTypeDef",
+    "DeleteIPSetResponseTypeDef",
+    "DeleteRateBasedRuleResponseTypeDef",
+    "DeleteRegexMatchSetResponseTypeDef",
+    "DeleteRegexPatternSetResponseTypeDef",
+    "DeleteRuleGroupResponseTypeDef",
+    "DeleteRuleResponseTypeDef",
+    "DeleteSizeConstraintSetResponseTypeDef",
+    "DeleteSqlInjectionMatchSetResponseTypeDef",
+    "DeleteWebACLResponseTypeDef",
+    "DeleteXssMatchSetResponseTypeDef",
+    "GetChangeTokenResponseTypeDef",
+    "GetChangeTokenStatusResponseTypeDef",
+    "GetPermissionPolicyResponseTypeDef",
+    "GetRateBasedRuleManagedKeysResponseTypeDef",
+    "ListByteMatchSetsResponseTypeDef",
     "UpdateByteMatchSetResponseTypeDef",
     "UpdateGeoMatchSetResponseTypeDef",
     "UpdateIPSetResponseTypeDef",
     "UpdateRateBasedRuleResponseTypeDef",
     "UpdateRegexMatchSetResponseTypeDef",
     "UpdateRegexPatternSetResponseTypeDef",
     "UpdateRuleGroupResponseTypeDef",
     "UpdateRuleResponseTypeDef",
     "UpdateSizeConstraintSetResponseTypeDef",
     "UpdateSqlInjectionMatchSetResponseTypeDef",
     "UpdateWebACLResponseTypeDef",
     "UpdateXssMatchSetResponseTypeDef",
-    "ActivatedRuleTypeDef",
-    "ListByteMatchSetsResponseTypeDef",
-    "ByteMatchTupleTypeDef",
-    "LoggingConfigurationTypeDef",
-    "RegexMatchTupleTypeDef",
-    "SizeConstraintTypeDef",
-    "SqlInjectionMatchTupleTypeDef",
-    "XssMatchTupleTypeDef",
     "CreateRateBasedRuleRequestRequestTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
     "CreateRuleRequestRequestTypeDef",
     "CreateWebACLRequestRequestTypeDef",
-    "TagInfoForResourceTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateRegexPatternSetResponseTypeDef",
     "GetRegexPatternSetResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "GetRuleGroupResponseTypeDef",
     "GeoMatchSetTypeDef",
     "GeoMatchSetUpdateTypeDef",
     "ListGeoMatchSetsResponseTypeDef",
+    "GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
+    "ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef",
+    "ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef",
+    "ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef",
+    "ListIPSetsRequestListIPSetsPaginateTypeDef",
+    "ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef",
+    "ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef",
+    "ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef",
+    "ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef",
+    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
+    "ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef",
+    "ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef",
+    "ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef",
+    "ListWebACLsRequestListWebACLsPaginateTypeDef",
+    "ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef",
     "GetSampledRequestsRequestRequestTypeDef",
     "HTTPRequestTypeDef",
     "IPSetTypeDef",
     "IPSetUpdateTypeDef",
     "ListIPSetsResponseTypeDef",
     "ListRateBasedRulesResponseTypeDef",
     "ListRulesResponseTypeDef",
@@ -205,68 +222,90 @@
     "ListSubscribedRuleGroupsResponseTypeDef",
     "ListWebACLsResponseTypeDef",
     "ListXssMatchSetsResponseTypeDef",
     "RateBasedRuleTypeDef",
     "RuleTypeDef",
     "RuleUpdateTypeDef",
     "UpdateRegexPatternSetRequestRequestTypeDef",
+    "TagInfoForResourceTypeDef",
     "ListActivatedRulesInRuleGroupResponseTypeDef",
-    "RuleGroupUpdateTypeDef",
     "WebACLTypeDef",
+    "RuleGroupUpdateTypeDef",
     "WebACLUpdateTypeDef",
     "ByteMatchSetTypeDef",
-    "ByteMatchSetUpdateTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
-    "PutLoggingConfigurationRequestRequestTypeDef",
     "PutLoggingConfigurationResponseTypeDef",
     "RegexMatchSetTypeDef",
-    "RegexMatchSetUpdateTypeDef",
     "SizeConstraintSetTypeDef",
-    "SizeConstraintSetUpdateTypeDef",
     "SqlInjectionMatchSetTypeDef",
-    "SqlInjectionMatchSetUpdateTypeDef",
     "XssMatchSetTypeDef",
+    "ByteMatchSetUpdateTypeDef",
+    "PutLoggingConfigurationRequestRequestTypeDef",
+    "RegexMatchSetUpdateTypeDef",
+    "SizeConstraintSetUpdateTypeDef",
+    "SqlInjectionMatchSetUpdateTypeDef",
     "XssMatchSetUpdateTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "CreateGeoMatchSetResponseTypeDef",
     "GetGeoMatchSetResponseTypeDef",
     "UpdateGeoMatchSetRequestRequestTypeDef",
     "SampledHTTPRequestTypeDef",
     "CreateIPSetResponseTypeDef",
     "GetIPSetResponseTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
     "CreateRateBasedRuleResponseTypeDef",
     "GetRateBasedRuleResponseTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "UpdateRateBasedRuleRequestRequestTypeDef",
     "UpdateRuleRequestRequestTypeDef",
-    "UpdateRuleGroupRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateWebACLResponseTypeDef",
     "GetWebACLResponseTypeDef",
+    "UpdateRuleGroupRequestRequestTypeDef",
     "UpdateWebACLRequestRequestTypeDef",
     "CreateByteMatchSetResponseTypeDef",
     "GetByteMatchSetResponseTypeDef",
-    "UpdateByteMatchSetRequestRequestTypeDef",
     "CreateRegexMatchSetResponseTypeDef",
     "GetRegexMatchSetResponseTypeDef",
-    "UpdateRegexMatchSetRequestRequestTypeDef",
     "CreateSizeConstraintSetResponseTypeDef",
     "GetSizeConstraintSetResponseTypeDef",
-    "UpdateSizeConstraintSetRequestRequestTypeDef",
     "CreateSqlInjectionMatchSetResponseTypeDef",
     "GetSqlInjectionMatchSetResponseTypeDef",
-    "UpdateSqlInjectionMatchSetRequestRequestTypeDef",
     "CreateXssMatchSetResponseTypeDef",
     "GetXssMatchSetResponseTypeDef",
+    "UpdateByteMatchSetRequestRequestTypeDef",
+    "UpdateRegexMatchSetRequestRequestTypeDef",
+    "UpdateSizeConstraintSetRequestRequestTypeDef",
+    "UpdateSqlInjectionMatchSetRequestRequestTypeDef",
     "UpdateXssMatchSetRequestRequestTypeDef",
     "GetSampledRequestsResponseTypeDef",
 )
 
+ExcludedRuleOutputTypeDef = TypedDict(
+    "ExcludedRuleOutputTypeDef",
+    {
+        "RuleId": str,
+    },
+)
+
+WafActionOutputTypeDef = TypedDict(
+    "WafActionOutputTypeDef",
+    {
+        "Type": WafActionTypeType,
+    },
+)
+
+WafOverrideActionOutputTypeDef = TypedDict(
+    "WafOverrideActionOutputTypeDef",
+    {
+        "Type": WafOverrideActionTypeType,
+    },
+)
+
 ExcludedRuleTypeDef = TypedDict(
     "ExcludedRuleTypeDef",
     {
         "RuleId": str,
     },
 )
 
@@ -288,14 +327,33 @@
     "ByteMatchSetSummaryTypeDef",
     {
         "ByteMatchSetId": str,
         "Name": str,
     },
 )
 
+_RequiredFieldToMatchOutputTypeDef = TypedDict(
+    "_RequiredFieldToMatchOutputTypeDef",
+    {
+        "Type": MatchFieldTypeType,
+    },
+)
+_OptionalFieldToMatchOutputTypeDef = TypedDict(
+    "_OptionalFieldToMatchOutputTypeDef",
+    {
+        "Data": str,
+    },
+    total=False,
+)
+
+class FieldToMatchOutputTypeDef(
+    _RequiredFieldToMatchOutputTypeDef, _OptionalFieldToMatchOutputTypeDef
+):
+    pass
+
 _RequiredFieldToMatchTypeDef = TypedDict(
     "_RequiredFieldToMatchTypeDef",
     {
         "Type": MatchFieldTypeType,
     },
 )
 _OptionalFieldToMatchTypeDef = TypedDict(
@@ -313,14 +371,25 @@
     "CreateByteMatchSetRequestRequestTypeDef",
     {
         "Name": str,
         "ChangeToken": str,
     },
 )
 
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
 CreateGeoMatchSetRequestRequestTypeDef = TypedDict(
     "CreateGeoMatchSetRequestRequestTypeDef",
     {
         "Name": str,
         "ChangeToken": str,
     },
 )
@@ -414,22 +483,14 @@
     {
         "WebACLId": str,
         "S3BucketName": str,
         "IgnoreUnsupportedType": bool,
     },
 )
 
-CreateWebACLMigrationStackResponseTypeDef = TypedDict(
-    "CreateWebACLMigrationStackResponseTypeDef",
-    {
-        "S3ObjectUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateXssMatchSetRequestRequestTypeDef = TypedDict(
     "CreateXssMatchSetRequestRequestTypeDef",
     {
         "Name": str,
         "ChangeToken": str,
     },
 )
@@ -438,54 +499,30 @@
     "DeleteByteMatchSetRequestRequestTypeDef",
     {
         "ByteMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteByteMatchSetResponseTypeDef = TypedDict(
-    "DeleteByteMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteGeoMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteGeoMatchSetRequestRequestTypeDef",
     {
         "GeoMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteGeoMatchSetResponseTypeDef = TypedDict(
-    "DeleteGeoMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteIPSetRequestRequestTypeDef = TypedDict(
     "DeleteIPSetRequestRequestTypeDef",
     {
         "IPSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteIPSetResponseTypeDef = TypedDict(
-    "DeleteIPSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -500,147 +537,83 @@
     "DeleteRateBasedRuleRequestRequestTypeDef",
     {
         "RuleId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteRateBasedRuleResponseTypeDef = TypedDict(
-    "DeleteRateBasedRuleResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRegexMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteRegexMatchSetRequestRequestTypeDef",
     {
         "RegexMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteRegexMatchSetResponseTypeDef = TypedDict(
-    "DeleteRegexMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRegexPatternSetRequestRequestTypeDef = TypedDict(
     "DeleteRegexPatternSetRequestRequestTypeDef",
     {
         "RegexPatternSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteRegexPatternSetResponseTypeDef = TypedDict(
-    "DeleteRegexPatternSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRuleGroupRequestRequestTypeDef = TypedDict(
     "DeleteRuleGroupRequestRequestTypeDef",
     {
         "RuleGroupId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteRuleGroupResponseTypeDef = TypedDict(
-    "DeleteRuleGroupResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "RuleId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteRuleResponseTypeDef = TypedDict(
-    "DeleteRuleResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSizeConstraintSetRequestRequestTypeDef = TypedDict(
     "DeleteSizeConstraintSetRequestRequestTypeDef",
     {
         "SizeConstraintSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteSizeConstraintSetResponseTypeDef = TypedDict(
-    "DeleteSizeConstraintSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSqlInjectionMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteSqlInjectionMatchSetRequestRequestTypeDef",
     {
         "SqlInjectionMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteSqlInjectionMatchSetResponseTypeDef = TypedDict(
-    "DeleteSqlInjectionMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWebACLRequestRequestTypeDef = TypedDict(
     "DeleteWebACLRequestRequestTypeDef",
     {
         "WebACLId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteWebACLResponseTypeDef = TypedDict(
-    "DeleteWebACLResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteXssMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteXssMatchSetRequestRequestTypeDef",
     {
         "XssMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteXssMatchSetResponseTypeDef = TypedDict(
-    "DeleteXssMatchSetResponseTypeDef",
+GeoMatchConstraintOutputTypeDef = TypedDict(
+    "GeoMatchConstraintOutputTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Type": Literal["Country"],
+        "Value": GeoMatchConstraintValueType,
     },
 )
 
 GeoMatchConstraintTypeDef = TypedDict(
     "GeoMatchConstraintTypeDef",
     {
         "Type": Literal["Country"],
@@ -659,37 +632,21 @@
 GetByteMatchSetRequestRequestTypeDef = TypedDict(
     "GetByteMatchSetRequestRequestTypeDef",
     {
         "ByteMatchSetId": str,
     },
 )
 
-GetChangeTokenResponseTypeDef = TypedDict(
-    "GetChangeTokenResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetChangeTokenStatusRequestRequestTypeDef = TypedDict(
     "GetChangeTokenStatusRequestRequestTypeDef",
     {
         "ChangeToken": str,
     },
 )
 
-GetChangeTokenStatusResponseTypeDef = TypedDict(
-    "GetChangeTokenStatusResponseTypeDef",
-    {
-        "ChangeTokenStatus": ChangeTokenStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetGeoMatchSetRequestRequestTypeDef = TypedDict(
     "GetGeoMatchSetRequestRequestTypeDef",
     {
         "GeoMatchSetId": str,
     },
 )
 
@@ -710,42 +667,24 @@
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
-_RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef = TypedDict(
-    "_RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
-    {
-        "RuleId": str,
-    },
-)
-_OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef = TypedDict(
-    "_OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
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
 
-class GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef(
-    _RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
-    _OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
-):
-    pass
-
 _RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef = TypedDict(
     "_RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef",
     {
         "RuleId": str,
     },
 )
 _OptionalGetRateBasedRuleManagedKeysRequestRequestTypeDef = TypedDict(
@@ -758,23 +697,14 @@
 
 class GetRateBasedRuleManagedKeysRequestRequestTypeDef(
     _RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef,
     _OptionalGetRateBasedRuleManagedKeysRequestRequestTypeDef,
 ):
     pass
 
-GetRateBasedRuleManagedKeysResponseTypeDef = TypedDict(
-    "GetRateBasedRuleManagedKeysResponseTypeDef",
-    {
-        "ManagedKeys": List[str],
-        "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRateBasedRuleRequestRequestTypeDef = TypedDict(
     "GetRateBasedRuleRequestRequestTypeDef",
     {
         "RuleId": str,
     },
 )
 
@@ -810,14 +740,22 @@
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
 GetSizeConstraintSetRequestRequestTypeDef = TypedDict(
     "GetSizeConstraintSetRequestRequestTypeDef",
     {
         "SizeConstraintSetId": str,
     },
 )
 
@@ -847,14 +785,22 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
+IPSetDescriptorOutputTypeDef = TypedDict(
+    "IPSetDescriptorOutputTypeDef",
+    {
+        "Type": IPSetDescriptorTypeType,
+        "Value": str,
+    },
+)
+
 IPSetDescriptorTypeDef = TypedDict(
     "IPSetDescriptorTypeDef",
     {
         "Type": IPSetDescriptorTypeType,
         "Value": str,
     },
 )
@@ -863,109 +809,60 @@
     "IPSetSummaryTypeDef",
     {
         "IPSetId": str,
         "Name": str,
     },
 )
 
-ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef = TypedDict(
-    "ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef",
-    {
-        "RuleGroupId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListActivatedRulesInRuleGroupRequestRequestTypeDef = TypedDict(
     "ListActivatedRulesInRuleGroupRequestRequestTypeDef",
     {
         "RuleGroupId": str,
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef = TypedDict(
-    "ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListByteMatchSetsRequestRequestTypeDef = TypedDict(
     "ListByteMatchSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef = TypedDict(
-    "ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGeoMatchSetsRequestRequestTypeDef = TypedDict(
     "ListGeoMatchSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
-    "ListIPSetsRequestListIPSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListIPSetsRequestRequestTypeDef = TypedDict(
     "ListIPSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef = TypedDict(
-    "ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLoggingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListLoggingConfigurationsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef = TypedDict(
-    "ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRateBasedRulesRequestRequestTypeDef = TypedDict(
     "ListRateBasedRulesRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -975,22 +872,14 @@
     "RuleSummaryTypeDef",
     {
         "RuleId": str,
         "Name": str,
     },
 )
 
-ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef = TypedDict(
-    "ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRegexMatchSetsRequestRequestTypeDef = TypedDict(
     "ListRegexMatchSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1000,22 +889,14 @@
     "RegexMatchSetSummaryTypeDef",
     {
         "RegexMatchSetId": str,
         "Name": str,
     },
 )
 
-ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef = TypedDict(
-    "ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRegexPatternSetsRequestRequestTypeDef = TypedDict(
     "ListRegexPatternSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1025,22 +906,14 @@
     "RegexPatternSetSummaryTypeDef",
     {
         "RegexPatternSetId": str,
         "Name": str,
     },
 )
 
-ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = TypedDict(
-    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListRuleGroupsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1050,39 +923,23 @@
     "RuleGroupSummaryTypeDef",
     {
         "RuleGroupId": str,
         "Name": str,
     },
 )
 
-ListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "ListRulesRequestListRulesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRulesRequestRequestTypeDef = TypedDict(
     "ListRulesRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef = TypedDict(
-    "ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSizeConstraintSetsRequestRequestTypeDef = TypedDict(
     "ListSizeConstraintSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1092,22 +949,14 @@
     "SizeConstraintSetSummaryTypeDef",
     {
         "SizeConstraintSetId": str,
         "Name": str,
     },
 )
 
-ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef = TypedDict(
-    "ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSqlInjectionMatchSetsRequestRequestTypeDef = TypedDict(
     "ListSqlInjectionMatchSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1117,22 +966,14 @@
     "SqlInjectionMatchSetSummaryTypeDef",
     {
         "SqlInjectionMatchSetId": str,
         "Name": str,
     },
 )
 
-ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef = TypedDict(
-    "ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSubscribedRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListSubscribedRuleGroupsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1164,22 +1005,14 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-ListWebACLsRequestListWebACLsPaginateTypeDef = TypedDict(
-    "ListWebACLsRequestListWebACLsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWebACLsRequestRequestTypeDef = TypedDict(
     "ListWebACLsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1189,22 +1022,14 @@
     "WebACLSummaryTypeDef",
     {
         "WebACLId": str,
         "Name": str,
     },
 )
 
-ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef = TypedDict(
-    "ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListXssMatchSetsRequestRequestTypeDef = TypedDict(
     "ListXssMatchSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1214,22 +1039,21 @@
     "XssMatchSetSummaryTypeDef",
     {
         "XssMatchSetId": str,
         "Name": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+PredicateOutputTypeDef = TypedDict(
+    "PredicateOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Negated": bool,
+        "Type": PredicateTypeType,
+        "DataId": str,
     },
-    total=False,
 )
 
 PredicateTypeDef = TypedDict(
     "PredicateTypeDef",
     {
         "Negated": bool,
         "Type": PredicateTypeType,
@@ -1249,180 +1073,160 @@
     "RegexPatternSetUpdateTypeDef",
     {
         "Action": ChangeActionType,
         "RegexPatternString": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Key": str,
+        "Value": str,
     },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateByteMatchSetResponseTypeDef = TypedDict(
-    "UpdateByteMatchSetResponseTypeDef",
+_RequiredActivatedRuleOutputTypeDef = TypedDict(
+    "_RequiredActivatedRuleOutputTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Priority": int,
+        "RuleId": str,
     },
 )
-
-UpdateGeoMatchSetResponseTypeDef = TypedDict(
-    "UpdateGeoMatchSetResponseTypeDef",
+_OptionalActivatedRuleOutputTypeDef = TypedDict(
+    "_OptionalActivatedRuleOutputTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Action": WafActionOutputTypeDef,
+        "OverrideAction": WafOverrideActionOutputTypeDef,
+        "Type": WafRuleTypeType,
+        "ExcludedRules": List[ExcludedRuleOutputTypeDef],
     },
+    total=False,
 )
 
-UpdateIPSetResponseTypeDef = TypedDict(
-    "UpdateIPSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+class ActivatedRuleOutputTypeDef(
+    _RequiredActivatedRuleOutputTypeDef, _OptionalActivatedRuleOutputTypeDef
+):
+    pass
 
-UpdateRateBasedRuleResponseTypeDef = TypedDict(
-    "UpdateRateBasedRuleResponseTypeDef",
+_RequiredActivatedRuleTypeDef = TypedDict(
+    "_RequiredActivatedRuleTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Priority": int,
+        "RuleId": str,
     },
 )
-
-UpdateRegexMatchSetResponseTypeDef = TypedDict(
-    "UpdateRegexMatchSetResponseTypeDef",
+_OptionalActivatedRuleTypeDef = TypedDict(
+    "_OptionalActivatedRuleTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Action": WafActionTypeDef,
+        "OverrideAction": WafOverrideActionTypeDef,
+        "Type": WafRuleTypeType,
+        "ExcludedRules": Sequence[ExcludedRuleTypeDef],
     },
+    total=False,
 )
 
-UpdateRegexPatternSetResponseTypeDef = TypedDict(
-    "UpdateRegexPatternSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+class ActivatedRuleTypeDef(_RequiredActivatedRuleTypeDef, _OptionalActivatedRuleTypeDef):
+    pass
 
-UpdateRuleGroupResponseTypeDef = TypedDict(
-    "UpdateRuleGroupResponseTypeDef",
+ByteMatchTupleOutputTypeDef = TypedDict(
+    "ByteMatchTupleOutputTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TargetString": bytes,
+        "TextTransformation": TextTransformationType,
+        "PositionalConstraint": PositionalConstraintType,
     },
 )
 
-UpdateRuleResponseTypeDef = TypedDict(
-    "UpdateRuleResponseTypeDef",
+_RequiredLoggingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredLoggingConfigurationOutputTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceArn": str,
+        "LogDestinationConfigs": List[str],
     },
 )
-
-UpdateSizeConstraintSetResponseTypeDef = TypedDict(
-    "UpdateSizeConstraintSetResponseTypeDef",
+_OptionalLoggingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalLoggingConfigurationOutputTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RedactedFields": List[FieldToMatchOutputTypeDef],
     },
+    total=False,
 )
 
-UpdateSqlInjectionMatchSetResponseTypeDef = TypedDict(
-    "UpdateSqlInjectionMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+class LoggingConfigurationOutputTypeDef(
+    _RequiredLoggingConfigurationOutputTypeDef, _OptionalLoggingConfigurationOutputTypeDef
+):
+    pass
 
-UpdateWebACLResponseTypeDef = TypedDict(
-    "UpdateWebACLResponseTypeDef",
+RegexMatchTupleOutputTypeDef = TypedDict(
+    "RegexMatchTupleOutputTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformation": TextTransformationType,
+        "RegexPatternSetId": str,
     },
 )
 
-UpdateXssMatchSetResponseTypeDef = TypedDict(
-    "UpdateXssMatchSetResponseTypeDef",
+SizeConstraintOutputTypeDef = TypedDict(
+    "SizeConstraintOutputTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformation": TextTransformationType,
+        "ComparisonOperator": ComparisonOperatorType,
+        "Size": int,
     },
 )
 
-_RequiredActivatedRuleTypeDef = TypedDict(
-    "_RequiredActivatedRuleTypeDef",
+SqlInjectionMatchTupleOutputTypeDef = TypedDict(
+    "SqlInjectionMatchTupleOutputTypeDef",
     {
-        "Priority": int,
-        "RuleId": str,
-    },
-)
-_OptionalActivatedRuleTypeDef = TypedDict(
-    "_OptionalActivatedRuleTypeDef",
-    {
-        "Action": WafActionTypeDef,
-        "OverrideAction": WafOverrideActionTypeDef,
-        "Type": WafRuleTypeType,
-        "ExcludedRules": List[ExcludedRuleTypeDef],
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformation": TextTransformationType,
     },
-    total=False,
 )
 
-class ActivatedRuleTypeDef(_RequiredActivatedRuleTypeDef, _OptionalActivatedRuleTypeDef):
-    pass
-
-ListByteMatchSetsResponseTypeDef = TypedDict(
-    "ListByteMatchSetsResponseTypeDef",
+XssMatchTupleOutputTypeDef = TypedDict(
+    "XssMatchTupleOutputTypeDef",
     {
-        "NextMarker": str,
-        "ByteMatchSets": List[ByteMatchSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformation": TextTransformationType,
     },
 )
 
 ByteMatchTupleTypeDef = TypedDict(
     "ByteMatchTupleTypeDef",
     {
         "FieldToMatch": FieldToMatchTypeDef,
-        "TargetString": bytes,
+        "TargetString": Union[str, bytes, IO[Any], StreamingBody],
         "TextTransformation": TextTransformationType,
         "PositionalConstraint": PositionalConstraintType,
     },
 )
 
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
     },
     total=False,
 )
 
 class LoggingConfigurationTypeDef(
     _RequiredLoggingConfigurationTypeDef, _OptionalLoggingConfigurationTypeDef
 ):
@@ -1459,14 +1263,256 @@
     "XssMatchTupleTypeDef",
     {
         "FieldToMatch": FieldToMatchTypeDef,
         "TextTransformation": TextTransformationType,
     },
 )
 
+CreateWebACLMigrationStackResponseTypeDef = TypedDict(
+    "CreateWebACLMigrationStackResponseTypeDef",
+    {
+        "S3ObjectUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteByteMatchSetResponseTypeDef = TypedDict(
+    "DeleteByteMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteGeoMatchSetResponseTypeDef = TypedDict(
+    "DeleteGeoMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteIPSetResponseTypeDef = TypedDict(
+    "DeleteIPSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRateBasedRuleResponseTypeDef = TypedDict(
+    "DeleteRateBasedRuleResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRegexMatchSetResponseTypeDef = TypedDict(
+    "DeleteRegexMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRegexPatternSetResponseTypeDef = TypedDict(
+    "DeleteRegexPatternSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRuleGroupResponseTypeDef = TypedDict(
+    "DeleteRuleGroupResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRuleResponseTypeDef = TypedDict(
+    "DeleteRuleResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSizeConstraintSetResponseTypeDef = TypedDict(
+    "DeleteSizeConstraintSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSqlInjectionMatchSetResponseTypeDef = TypedDict(
+    "DeleteSqlInjectionMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteWebACLResponseTypeDef = TypedDict(
+    "DeleteWebACLResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteXssMatchSetResponseTypeDef = TypedDict(
+    "DeleteXssMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetChangeTokenResponseTypeDef = TypedDict(
+    "GetChangeTokenResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetChangeTokenStatusResponseTypeDef = TypedDict(
+    "GetChangeTokenStatusResponseTypeDef",
+    {
+        "ChangeTokenStatus": ChangeTokenStatusType,
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
+GetRateBasedRuleManagedKeysResponseTypeDef = TypedDict(
+    "GetRateBasedRuleManagedKeysResponseTypeDef",
+    {
+        "ManagedKeys": List[str],
+        "NextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListByteMatchSetsResponseTypeDef = TypedDict(
+    "ListByteMatchSetsResponseTypeDef",
+    {
+        "NextMarker": str,
+        "ByteMatchSets": List[ByteMatchSetSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateByteMatchSetResponseTypeDef = TypedDict(
+    "UpdateByteMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGeoMatchSetResponseTypeDef = TypedDict(
+    "UpdateGeoMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateIPSetResponseTypeDef = TypedDict(
+    "UpdateIPSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRateBasedRuleResponseTypeDef = TypedDict(
+    "UpdateRateBasedRuleResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRegexMatchSetResponseTypeDef = TypedDict(
+    "UpdateRegexMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRegexPatternSetResponseTypeDef = TypedDict(
+    "UpdateRegexPatternSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRuleGroupResponseTypeDef = TypedDict(
+    "UpdateRuleGroupResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRuleResponseTypeDef = TypedDict(
+    "UpdateRuleResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSizeConstraintSetResponseTypeDef = TypedDict(
+    "UpdateSizeConstraintSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSqlInjectionMatchSetResponseTypeDef = TypedDict(
+    "UpdateSqlInjectionMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWebACLResponseTypeDef = TypedDict(
+    "UpdateWebACLResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateXssMatchSetResponseTypeDef = TypedDict(
+    "UpdateXssMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateRateBasedRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRateBasedRuleRequestRequestTypeDef",
     {
         "Name": str,
         "MetricName": str,
         "RateKey": Literal["IP"],
         "RateLimit": int,
@@ -1547,70 +1593,61 @@
 )
 
 class CreateWebACLRequestRequestTypeDef(
     _RequiredCreateWebACLRequestRequestTypeDef, _OptionalCreateWebACLRequestRequestTypeDef
 ):
     pass
 
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
 
 CreateRegexPatternSetResponseTypeDef = TypedDict(
     "CreateRegexPatternSetResponseTypeDef",
     {
         "RegexPatternSet": RegexPatternSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRegexPatternSetResponseTypeDef = TypedDict(
     "GetRegexPatternSetResponseTypeDef",
     {
         "RegexPatternSet": RegexPatternSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRuleGroupResponseTypeDef = TypedDict(
     "CreateRuleGroupResponseTypeDef",
     {
         "RuleGroup": RuleGroupTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRuleGroupResponseTypeDef = TypedDict(
     "GetRuleGroupResponseTypeDef",
     {
         "RuleGroup": RuleGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGeoMatchSetTypeDef = TypedDict(
     "_RequiredGeoMatchSetTypeDef",
     {
         "GeoMatchSetId": str,
-        "GeoMatchConstraints": List[GeoMatchConstraintTypeDef],
+        "GeoMatchConstraints": List[GeoMatchConstraintOutputTypeDef],
     },
 )
 _OptionalGeoMatchSetTypeDef = TypedDict(
     "_OptionalGeoMatchSetTypeDef",
     {
         "Name": str,
     },
@@ -1629,16 +1666,157 @@
 )
 
 ListGeoMatchSetsResponseTypeDef = TypedDict(
     "ListGeoMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "GeoMatchSets": List[GeoMatchSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef = TypedDict(
+    "_RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
+    {
+        "RuleId": str,
+    },
+)
+_OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef = TypedDict(
+    "_OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+class GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef(
+    _RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
+    _OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
+):
+    pass
+
+ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef = TypedDict(
+    "ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef",
+    {
+        "RuleGroupId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef = TypedDict(
+    "ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef = TypedDict(
+    "ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
+    "ListIPSetsRequestListIPSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef = TypedDict(
+    "ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef = TypedDict(
+    "ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef = TypedDict(
+    "ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef = TypedDict(
+    "ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = TypedDict(
+    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "ListRulesRequestListRulesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef = TypedDict(
+    "ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef = TypedDict(
+    "ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef = TypedDict(
+    "ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWebACLsRequestListWebACLsPaginateTypeDef = TypedDict(
+    "ListWebACLsRequestListWebACLsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef = TypedDict(
+    "ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 GetSampledRequestsRequestRequestTypeDef = TypedDict(
     "GetSampledRequestsRequestRequestTypeDef",
     {
         "WebAclId": str,
         "RuleId": str,
@@ -1660,15 +1838,15 @@
     total=False,
 )
 
 _RequiredIPSetTypeDef = TypedDict(
     "_RequiredIPSetTypeDef",
     {
         "IPSetId": str,
-        "IPSetDescriptors": List[IPSetDescriptorTypeDef],
+        "IPSetDescriptors": List[IPSetDescriptorOutputTypeDef],
     },
 )
 _OptionalIPSetTypeDef = TypedDict(
     "_OptionalIPSetTypeDef",
     {
         "Name": str,
     },
@@ -1687,113 +1865,113 @@
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
 
 ListRateBasedRulesResponseTypeDef = TypedDict(
     "ListRateBasedRulesResponseTypeDef",
     {
         "NextMarker": str,
         "Rules": List[RuleSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "NextMarker": str,
         "Rules": List[RuleSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRegexMatchSetsResponseTypeDef = TypedDict(
     "ListRegexMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "RegexMatchSets": List[RegexMatchSetSummaryTypeDef],
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
 
 ListRuleGroupsResponseTypeDef = TypedDict(
     "ListRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "RuleGroups": List[RuleGroupSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSizeConstraintSetsResponseTypeDef = TypedDict(
     "ListSizeConstraintSetsResponseTypeDef",
     {
         "NextMarker": str,
         "SizeConstraintSets": List[SizeConstraintSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSqlInjectionMatchSetsResponseTypeDef = TypedDict(
     "ListSqlInjectionMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "SqlInjectionMatchSets": List[SqlInjectionMatchSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSubscribedRuleGroupsResponseTypeDef = TypedDict(
     "ListSubscribedRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "RuleGroups": List[SubscribedRuleGroupSummaryTypeDef],
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
     },
 )
 
 ListXssMatchSetsResponseTypeDef = TypedDict(
     "ListXssMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "XssMatchSets": List[XssMatchSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRateBasedRuleTypeDef = TypedDict(
     "_RequiredRateBasedRuleTypeDef",
     {
         "RuleId": str,
-        "MatchPredicates": List[PredicateTypeDef],
+        "MatchPredicates": List[PredicateOutputTypeDef],
         "RateKey": Literal["IP"],
         "RateLimit": int,
     },
 )
 _OptionalRateBasedRuleTypeDef = TypedDict(
     "_OptionalRateBasedRuleTypeDef",
     {
@@ -1806,15 +1984,15 @@
 class RateBasedRuleTypeDef(_RequiredRateBasedRuleTypeDef, _OptionalRateBasedRuleTypeDef):
     pass
 
 _RequiredRuleTypeDef = TypedDict(
     "_RequiredRuleTypeDef",
     {
         "RuleId": str,
-        "Predicates": List[PredicateTypeDef],
+        "Predicates": List[PredicateOutputTypeDef],
     },
 )
 _OptionalRuleTypeDef = TypedDict(
     "_OptionalRuleTypeDef",
     {
         "Name": str,
         "MetricName": str,
@@ -1838,37 +2016,38 @@
     {
         "RegexPatternSetId": str,
         "Updates": Sequence[RegexPatternSetUpdateTypeDef],
         "ChangeToken": str,
     },
 )
 
-ListActivatedRulesInRuleGroupResponseTypeDef = TypedDict(
-    "ListActivatedRulesInRuleGroupResponseTypeDef",
+TagInfoForResourceTypeDef = TypedDict(
+    "TagInfoForResourceTypeDef",
     {
-        "NextMarker": str,
-        "ActivatedRules": List[ActivatedRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceARN": str,
+        "TagList": List[TagOutputTypeDef],
     },
+    total=False,
 )
 
-RuleGroupUpdateTypeDef = TypedDict(
-    "RuleGroupUpdateTypeDef",
+ListActivatedRulesInRuleGroupResponseTypeDef = TypedDict(
+    "ListActivatedRulesInRuleGroupResponseTypeDef",
     {
-        "Action": ChangeActionType,
-        "ActivatedRule": ActivatedRuleTypeDef,
+        "NextMarker": str,
+        "ActivatedRules": List[ActivatedRuleOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredWebACLTypeDef = TypedDict(
     "_RequiredWebACLTypeDef",
     {
         "WebACLId": str,
-        "DefaultAction": WafActionTypeDef,
-        "Rules": List[ActivatedRuleTypeDef],
+        "DefaultAction": WafActionOutputTypeDef,
+        "Rules": List[ActivatedRuleOutputTypeDef],
     },
 )
 _OptionalWebACLTypeDef = TypedDict(
     "_OptionalWebACLTypeDef",
     {
         "Name": str,
         "MetricName": str,
@@ -1876,103 +2055,88 @@
     },
     total=False,
 )
 
 class WebACLTypeDef(_RequiredWebACLTypeDef, _OptionalWebACLTypeDef):
     pass
 
+RuleGroupUpdateTypeDef = TypedDict(
+    "RuleGroupUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "ActivatedRule": ActivatedRuleTypeDef,
+    },
+)
+
 WebACLUpdateTypeDef = TypedDict(
     "WebACLUpdateTypeDef",
     {
         "Action": ChangeActionType,
         "ActivatedRule": ActivatedRuleTypeDef,
     },
 )
 
 _RequiredByteMatchSetTypeDef = TypedDict(
     "_RequiredByteMatchSetTypeDef",
     {
         "ByteMatchSetId": str,
-        "ByteMatchTuples": List[ByteMatchTupleTypeDef],
+        "ByteMatchTuples": List[ByteMatchTupleOutputTypeDef],
     },
 )
 _OptionalByteMatchSetTypeDef = TypedDict(
     "_OptionalByteMatchSetTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
 class ByteMatchSetTypeDef(_RequiredByteMatchSetTypeDef, _OptionalByteMatchSetTypeDef):
     pass
 
-ByteMatchSetUpdateTypeDef = TypedDict(
-    "ByteMatchSetUpdateTypeDef",
-    {
-        "Action": ChangeActionType,
-        "ByteMatchTuple": ByteMatchTupleTypeDef,
-    },
-)
-
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
-    },
-)
-
-PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutLoggingConfigurationRequestRequestTypeDef",
-    {
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutLoggingConfigurationResponseTypeDef = TypedDict(
     "PutLoggingConfigurationResponseTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegexMatchSetTypeDef = TypedDict(
     "RegexMatchSetTypeDef",
     {
         "RegexMatchSetId": str,
         "Name": str,
-        "RegexMatchTuples": List[RegexMatchTupleTypeDef],
+        "RegexMatchTuples": List[RegexMatchTupleOutputTypeDef],
     },
     total=False,
 )
 
-RegexMatchSetUpdateTypeDef = TypedDict(
-    "RegexMatchSetUpdateTypeDef",
-    {
-        "Action": ChangeActionType,
-        "RegexMatchTuple": RegexMatchTupleTypeDef,
-    },
-)
-
 _RequiredSizeConstraintSetTypeDef = TypedDict(
     "_RequiredSizeConstraintSetTypeDef",
     {
         "SizeConstraintSetId": str,
-        "SizeConstraints": List[SizeConstraintTypeDef],
+        "SizeConstraints": List[SizeConstraintOutputTypeDef],
     },
 )
 _OptionalSizeConstraintSetTypeDef = TypedDict(
     "_OptionalSizeConstraintSetTypeDef",
     {
         "Name": str,
     },
@@ -1980,27 +2144,19 @@
 )
 
 class SizeConstraintSetTypeDef(
     _RequiredSizeConstraintSetTypeDef, _OptionalSizeConstraintSetTypeDef
 ):
     pass
 
-SizeConstraintSetUpdateTypeDef = TypedDict(
-    "SizeConstraintSetUpdateTypeDef",
-    {
-        "Action": ChangeActionType,
-        "SizeConstraint": SizeConstraintTypeDef,
-    },
-)
-
 _RequiredSqlInjectionMatchSetTypeDef = TypedDict(
     "_RequiredSqlInjectionMatchSetTypeDef",
     {
         "SqlInjectionMatchSetId": str,
-        "SqlInjectionMatchTuples": List[SqlInjectionMatchTupleTypeDef],
+        "SqlInjectionMatchTuples": List[SqlInjectionMatchTupleOutputTypeDef],
     },
 )
 _OptionalSqlInjectionMatchSetTypeDef = TypedDict(
     "_OptionalSqlInjectionMatchSetTypeDef",
     {
         "Name": str,
     },
@@ -2008,71 +2164,93 @@
 )
 
 class SqlInjectionMatchSetTypeDef(
     _RequiredSqlInjectionMatchSetTypeDef, _OptionalSqlInjectionMatchSetTypeDef
 ):
     pass
 
-SqlInjectionMatchSetUpdateTypeDef = TypedDict(
-    "SqlInjectionMatchSetUpdateTypeDef",
-    {
-        "Action": ChangeActionType,
-        "SqlInjectionMatchTuple": SqlInjectionMatchTupleTypeDef,
-    },
-)
-
 _RequiredXssMatchSetTypeDef = TypedDict(
     "_RequiredXssMatchSetTypeDef",
     {
         "XssMatchSetId": str,
-        "XssMatchTuples": List[XssMatchTupleTypeDef],
+        "XssMatchTuples": List[XssMatchTupleOutputTypeDef],
     },
 )
 _OptionalXssMatchSetTypeDef = TypedDict(
     "_OptionalXssMatchSetTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
 class XssMatchSetTypeDef(_RequiredXssMatchSetTypeDef, _OptionalXssMatchSetTypeDef):
     pass
 
-XssMatchSetUpdateTypeDef = TypedDict(
-    "XssMatchSetUpdateTypeDef",
+ByteMatchSetUpdateTypeDef = TypedDict(
+    "ByteMatchSetUpdateTypeDef",
     {
         "Action": ChangeActionType,
-        "XssMatchTuple": XssMatchTupleTypeDef,
+        "ByteMatchTuple": ByteMatchTupleTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutLoggingConfigurationRequestRequestTypeDef",
     {
-        "NextMarker": str,
-        "TagInfoForResource": TagInfoForResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
+    },
+)
+
+RegexMatchSetUpdateTypeDef = TypedDict(
+    "RegexMatchSetUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "RegexMatchTuple": RegexMatchTupleTypeDef,
+    },
+)
+
+SizeConstraintSetUpdateTypeDef = TypedDict(
+    "SizeConstraintSetUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "SizeConstraint": SizeConstraintTypeDef,
+    },
+)
+
+SqlInjectionMatchSetUpdateTypeDef = TypedDict(
+    "SqlInjectionMatchSetUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "SqlInjectionMatchTuple": SqlInjectionMatchTupleTypeDef,
+    },
+)
+
+XssMatchSetUpdateTypeDef = TypedDict(
+    "XssMatchSetUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "XssMatchTuple": XssMatchTupleTypeDef,
     },
 )
 
 CreateGeoMatchSetResponseTypeDef = TypedDict(
     "CreateGeoMatchSetResponseTypeDef",
     {
         "GeoMatchSet": GeoMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGeoMatchSetResponseTypeDef = TypedDict(
     "GetGeoMatchSetResponseTypeDef",
     {
         "GeoMatchSet": GeoMatchSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGeoMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateGeoMatchSetRequestRequestTypeDef",
     {
         "GeoMatchSetId": str,
@@ -2104,23 +2282,23 @@
     pass
 
 CreateIPSetResponseTypeDef = TypedDict(
     "CreateIPSetResponseTypeDef",
     {
         "IPSet": IPSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIPSetResponseTypeDef = TypedDict(
     "GetIPSetResponseTypeDef",
     {
         "IPSet": IPSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIPSetRequestRequestTypeDef = TypedDict(
     "UpdateIPSetRequestRequestTypeDef",
     {
         "IPSetId": str,
@@ -2130,40 +2308,40 @@
 )
 
 CreateRateBasedRuleResponseTypeDef = TypedDict(
     "CreateRateBasedRuleResponseTypeDef",
     {
         "Rule": RateBasedRuleTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRateBasedRuleResponseTypeDef = TypedDict(
     "GetRateBasedRuleResponseTypeDef",
     {
         "Rule": RateBasedRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRuleResponseTypeDef = TypedDict(
     "CreateRuleResponseTypeDef",
     {
         "Rule": RuleTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
         "Rule": RuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRateBasedRuleRequestRequestTypeDef = TypedDict(
     "UpdateRateBasedRuleRequestRequestTypeDef",
     {
         "RuleId": str,
@@ -2178,37 +2356,46 @@
     {
         "RuleId": str,
         "ChangeToken": str,
         "Updates": Sequence[RuleUpdateTypeDef],
     },
 )
 
-UpdateRuleGroupRequestRequestTypeDef = TypedDict(
-    "UpdateRuleGroupRequestRequestTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "RuleGroupId": str,
-        "Updates": Sequence[RuleGroupUpdateTypeDef],
-        "ChangeToken": str,
+        "NextMarker": str,
+        "TagInfoForResource": TagInfoForResourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWebACLResponseTypeDef = TypedDict(
     "CreateWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWebACLResponseTypeDef = TypedDict(
     "GetWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRuleGroupRequestRequestTypeDef = TypedDict(
+    "UpdateRuleGroupRequestRequestTypeDef",
+    {
+        "RuleGroupId": str,
+        "Updates": Sequence[RuleGroupUpdateTypeDef],
+        "ChangeToken": str,
     },
 )
 
 _RequiredUpdateWebACLRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWebACLRequestRequestTypeDef",
     {
         "WebACLId": str,
@@ -2230,127 +2417,127 @@
     pass
 
 CreateByteMatchSetResponseTypeDef = TypedDict(
     "CreateByteMatchSetResponseTypeDef",
     {
         "ByteMatchSet": ByteMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetByteMatchSetResponseTypeDef = TypedDict(
     "GetByteMatchSetResponseTypeDef",
     {
         "ByteMatchSet": ByteMatchSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateByteMatchSetRequestRequestTypeDef = TypedDict(
-    "UpdateByteMatchSetRequestRequestTypeDef",
-    {
-        "ByteMatchSetId": str,
-        "ChangeToken": str,
-        "Updates": Sequence[ByteMatchSetUpdateTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRegexMatchSetResponseTypeDef = TypedDict(
     "CreateRegexMatchSetResponseTypeDef",
     {
         "RegexMatchSet": RegexMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRegexMatchSetResponseTypeDef = TypedDict(
     "GetRegexMatchSetResponseTypeDef",
     {
         "RegexMatchSet": RegexMatchSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateRegexMatchSetRequestRequestTypeDef = TypedDict(
-    "UpdateRegexMatchSetRequestRequestTypeDef",
-    {
-        "RegexMatchSetId": str,
-        "Updates": Sequence[RegexMatchSetUpdateTypeDef],
-        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSizeConstraintSetResponseTypeDef = TypedDict(
     "CreateSizeConstraintSetResponseTypeDef",
     {
         "SizeConstraintSet": SizeConstraintSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSizeConstraintSetResponseTypeDef = TypedDict(
     "GetSizeConstraintSetResponseTypeDef",
     {
         "SizeConstraintSet": SizeConstraintSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSizeConstraintSetRequestRequestTypeDef = TypedDict(
-    "UpdateSizeConstraintSetRequestRequestTypeDef",
-    {
-        "SizeConstraintSetId": str,
-        "ChangeToken": str,
-        "Updates": Sequence[SizeConstraintSetUpdateTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSqlInjectionMatchSetResponseTypeDef = TypedDict(
     "CreateSqlInjectionMatchSetResponseTypeDef",
     {
         "SqlInjectionMatchSet": SqlInjectionMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSqlInjectionMatchSetResponseTypeDef = TypedDict(
     "GetSqlInjectionMatchSetResponseTypeDef",
     {
         "SqlInjectionMatchSet": SqlInjectionMatchSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSqlInjectionMatchSetRequestRequestTypeDef = TypedDict(
-    "UpdateSqlInjectionMatchSetRequestRequestTypeDef",
-    {
-        "SqlInjectionMatchSetId": str,
-        "ChangeToken": str,
-        "Updates": Sequence[SqlInjectionMatchSetUpdateTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateXssMatchSetResponseTypeDef = TypedDict(
     "CreateXssMatchSetResponseTypeDef",
     {
         "XssMatchSet": XssMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetXssMatchSetResponseTypeDef = TypedDict(
     "GetXssMatchSetResponseTypeDef",
     {
         "XssMatchSet": XssMatchSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateByteMatchSetRequestRequestTypeDef = TypedDict(
+    "UpdateByteMatchSetRequestRequestTypeDef",
+    {
+        "ByteMatchSetId": str,
+        "ChangeToken": str,
+        "Updates": Sequence[ByteMatchSetUpdateTypeDef],
+    },
+)
+
+UpdateRegexMatchSetRequestRequestTypeDef = TypedDict(
+    "UpdateRegexMatchSetRequestRequestTypeDef",
+    {
+        "RegexMatchSetId": str,
+        "Updates": Sequence[RegexMatchSetUpdateTypeDef],
+        "ChangeToken": str,
+    },
+)
+
+UpdateSizeConstraintSetRequestRequestTypeDef = TypedDict(
+    "UpdateSizeConstraintSetRequestRequestTypeDef",
+    {
+        "SizeConstraintSetId": str,
+        "ChangeToken": str,
+        "Updates": Sequence[SizeConstraintSetUpdateTypeDef],
+    },
+)
+
+UpdateSqlInjectionMatchSetRequestRequestTypeDef = TypedDict(
+    "UpdateSqlInjectionMatchSetRequestRequestTypeDef",
+    {
+        "SqlInjectionMatchSetId": str,
+        "ChangeToken": str,
+        "Updates": Sequence[SqlInjectionMatchSetUpdateTypeDef],
     },
 )
 
 UpdateXssMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateXssMatchSetRequestRequestTypeDef",
     {
         "XssMatchSetId": str,
@@ -2360,11 +2547,11 @@
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
     },
 )
```

### Comparing `mypy-boto3-waf-1.28.0/mypy_boto3_waf.egg-info/PKG-INFO` & `mypy-boto3-waf-1.28.12/mypy_boto3_waf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-waf
-Version: 1.28.0
-Summary: Type annotations for boto3.WAF 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.WAF 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-waf"></a>
 
 # mypy-boto3-waf
 
 [![PyPI - mypy-boto3-waf](https://img.shields.io/pypi/v/mypy-boto3-waf.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-waf?color=blue)](https://pypistats.org/packages/mypy-boto3-waf)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-waf)](https://pepy.tech/project/mypy-boto3-waf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAF 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
+[boto3.WAF 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
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
 [mypy-boto3-waf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/).
 
 See how it helps to find and fix potential bugs:
 
@@ -401,164 +401,179 @@
 ### Typed dictionaries
 
 `mypy_boto3_waf.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_waf.type_defs import (
+    ExcludedRuleOutputTypeDef,
+    WafActionOutputTypeDef,
+    WafOverrideActionOutputTypeDef,
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
     ByteMatchSetSummaryTypeDef,
+    FieldToMatchOutputTypeDef,
     FieldToMatchTypeDef,
     CreateByteMatchSetRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateGeoMatchSetRequestRequestTypeDef,
     CreateIPSetRequestRequestTypeDef,
     TagTypeDef,
     CreateRegexMatchSetRequestRequestTypeDef,
     CreateRegexPatternSetRequestRequestTypeDef,
     RegexPatternSetTypeDef,
     RuleGroupTypeDef,
     CreateSizeConstraintSetRequestRequestTypeDef,
     CreateSqlInjectionMatchSetRequestRequestTypeDef,
     CreateWebACLMigrationStackRequestRequestTypeDef,
-    CreateWebACLMigrationStackResponseTypeDef,
     CreateXssMatchSetRequestRequestTypeDef,
     DeleteByteMatchSetRequestRequestTypeDef,
-    DeleteByteMatchSetResponseTypeDef,
     DeleteGeoMatchSetRequestRequestTypeDef,
-    DeleteGeoMatchSetResponseTypeDef,
     DeleteIPSetRequestRequestTypeDef,
-    DeleteIPSetResponseTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeletePermissionPolicyRequestRequestTypeDef,
     DeleteRateBasedRuleRequestRequestTypeDef,
-    DeleteRateBasedRuleResponseTypeDef,
     DeleteRegexMatchSetRequestRequestTypeDef,
-    DeleteRegexMatchSetResponseTypeDef,
     DeleteRegexPatternSetRequestRequestTypeDef,
-    DeleteRegexPatternSetResponseTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
-    DeleteRuleGroupResponseTypeDef,
     DeleteRuleRequestRequestTypeDef,
-    DeleteRuleResponseTypeDef,
     DeleteSizeConstraintSetRequestRequestTypeDef,
-    DeleteSizeConstraintSetResponseTypeDef,
     DeleteSqlInjectionMatchSetRequestRequestTypeDef,
-    DeleteSqlInjectionMatchSetResponseTypeDef,
     DeleteWebACLRequestRequestTypeDef,
-    DeleteWebACLResponseTypeDef,
     DeleteXssMatchSetRequestRequestTypeDef,
-    DeleteXssMatchSetResponseTypeDef,
+    GeoMatchConstraintOutputTypeDef,
     GeoMatchConstraintTypeDef,
     GeoMatchSetSummaryTypeDef,
     GetByteMatchSetRequestRequestTypeDef,
-    GetChangeTokenResponseTypeDef,
     GetChangeTokenStatusRequestRequestTypeDef,
-    GetChangeTokenStatusResponseTypeDef,
     GetGeoMatchSetRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetPermissionPolicyRequestRequestTypeDef,
-    GetPermissionPolicyResponseTypeDef,
-    GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetRateBasedRuleManagedKeysRequestRequestTypeDef,
-    GetRateBasedRuleManagedKeysResponseTypeDef,
     GetRateBasedRuleRequestRequestTypeDef,
     GetRegexMatchSetRequestRequestTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
     TimeWindowTypeDef,
+    TimeWindowOutputTypeDef,
     GetSizeConstraintSetRequestRequestTypeDef,
     GetSqlInjectionMatchSetRequestRequestTypeDef,
     GetWebACLRequestRequestTypeDef,
     GetXssMatchSetRequestRequestTypeDef,
     HTTPHeaderTypeDef,
+    IPSetDescriptorOutputTypeDef,
     IPSetDescriptorTypeDef,
     IPSetSummaryTypeDef,
-    ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef,
     ListActivatedRulesInRuleGroupRequestRequestTypeDef,
-    ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef,
     ListByteMatchSetsRequestRequestTypeDef,
-    ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef,
     ListGeoMatchSetsRequestRequestTypeDef,
-    ListIPSetsRequestListIPSetsPaginateTypeDef,
     ListIPSetsRequestRequestTypeDef,
-    ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
-    ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef,
     ListRateBasedRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
-    ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef,
     ListRegexMatchSetsRequestRequestTypeDef,
     RegexMatchSetSummaryTypeDef,
-    ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     RegexPatternSetSummaryTypeDef,
-    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupSummaryTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
-    ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef,
     ListSizeConstraintSetsRequestRequestTypeDef,
     SizeConstraintSetSummaryTypeDef,
-    ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef,
     ListSqlInjectionMatchSetsRequestRequestTypeDef,
     SqlInjectionMatchSetSummaryTypeDef,
-    ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef,
     ListSubscribedRuleGroupsRequestRequestTypeDef,
     SubscribedRuleGroupSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListWebACLsRequestListWebACLsPaginateTypeDef,
     ListWebACLsRequestRequestTypeDef,
     WebACLSummaryTypeDef,
-    ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef,
     ListXssMatchSetsRequestRequestTypeDef,
     XssMatchSetSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    PredicateOutputTypeDef,
     PredicateTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
     RegexPatternSetUpdateTypeDef,
-    ResponseMetadataTypeDef,
+    TagOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
+    ActivatedRuleOutputTypeDef,
+    ActivatedRuleTypeDef,
+    ByteMatchTupleOutputTypeDef,
+    LoggingConfigurationOutputTypeDef,
+    RegexMatchTupleOutputTypeDef,
+    SizeConstraintOutputTypeDef,
+    SqlInjectionMatchTupleOutputTypeDef,
+    XssMatchTupleOutputTypeDef,
+    ByteMatchTupleTypeDef,
+    LoggingConfigurationTypeDef,
+    RegexMatchTupleTypeDef,
+    SizeConstraintTypeDef,
+    SqlInjectionMatchTupleTypeDef,
+    XssMatchTupleTypeDef,
+    CreateWebACLMigrationStackResponseTypeDef,
+    DeleteByteMatchSetResponseTypeDef,
+    DeleteGeoMatchSetResponseTypeDef,
+    DeleteIPSetResponseTypeDef,
+    DeleteRateBasedRuleResponseTypeDef,
+    DeleteRegexMatchSetResponseTypeDef,
+    DeleteRegexPatternSetResponseTypeDef,
+    DeleteRuleGroupResponseTypeDef,
+    DeleteRuleResponseTypeDef,
+    DeleteSizeConstraintSetResponseTypeDef,
+    DeleteSqlInjectionMatchSetResponseTypeDef,
+    DeleteWebACLResponseTypeDef,
+    DeleteXssMatchSetResponseTypeDef,
+    GetChangeTokenResponseTypeDef,
+    GetChangeTokenStatusResponseTypeDef,
+    GetPermissionPolicyResponseTypeDef,
+    GetRateBasedRuleManagedKeysResponseTypeDef,
+    ListByteMatchSetsResponseTypeDef,
     UpdateByteMatchSetResponseTypeDef,
     UpdateGeoMatchSetResponseTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateRateBasedRuleResponseTypeDef,
     UpdateRegexMatchSetResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateRuleResponseTypeDef,
     UpdateSizeConstraintSetResponseTypeDef,
     UpdateSqlInjectionMatchSetResponseTypeDef,
     UpdateWebACLResponseTypeDef,
     UpdateXssMatchSetResponseTypeDef,
-    ActivatedRuleTypeDef,
-    ListByteMatchSetsResponseTypeDef,
-    ByteMatchTupleTypeDef,
-    LoggingConfigurationTypeDef,
-    RegexMatchTupleTypeDef,
-    SizeConstraintTypeDef,
-    SqlInjectionMatchTupleTypeDef,
-    XssMatchTupleTypeDef,
     CreateRateBasedRuleRequestRequestTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateWebACLRequestRequestTypeDef,
-    TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     GetRuleGroupResponseTypeDef,
     GeoMatchSetTypeDef,
     GeoMatchSetUpdateTypeDef,
     ListGeoMatchSetsResponseTypeDef,
+    GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
+    ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef,
+    ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef,
+    ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef,
+    ListIPSetsRequestListIPSetsPaginateTypeDef,
+    ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef,
+    ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef,
+    ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef,
+    ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef,
+    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
+    ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef,
+    ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef,
+    ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef,
+    ListWebACLsRequestListWebACLsPaginateTypeDef,
+    ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef,
     GetSampledRequestsRequestRequestTypeDef,
     HTTPRequestTypeDef,
     IPSetTypeDef,
     IPSetUpdateTypeDef,
     ListIPSetsResponseTypeDef,
     ListRateBasedRulesResponseTypeDef,
     ListRulesResponseTypeDef,
@@ -570,70 +585,71 @@
     ListSubscribedRuleGroupsResponseTypeDef,
     ListWebACLsResponseTypeDef,
     ListXssMatchSetsResponseTypeDef,
     RateBasedRuleTypeDef,
     RuleTypeDef,
     RuleUpdateTypeDef,
     UpdateRegexPatternSetRequestRequestTypeDef,
+    TagInfoForResourceTypeDef,
     ListActivatedRulesInRuleGroupResponseTypeDef,
-    RuleGroupUpdateTypeDef,
     WebACLTypeDef,
+    RuleGroupUpdateTypeDef,
     WebACLUpdateTypeDef,
     ByteMatchSetTypeDef,
-    ByteMatchSetUpdateTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
-    PutLoggingConfigurationRequestRequestTypeDef,
     PutLoggingConfigurationResponseTypeDef,
     RegexMatchSetTypeDef,
-    RegexMatchSetUpdateTypeDef,
     SizeConstraintSetTypeDef,
-    SizeConstraintSetUpdateTypeDef,
     SqlInjectionMatchSetTypeDef,
-    SqlInjectionMatchSetUpdateTypeDef,
     XssMatchSetTypeDef,
+    ByteMatchSetUpdateTypeDef,
+    PutLoggingConfigurationRequestRequestTypeDef,
+    RegexMatchSetUpdateTypeDef,
+    SizeConstraintSetUpdateTypeDef,
+    SqlInjectionMatchSetUpdateTypeDef,
     XssMatchSetUpdateTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CreateGeoMatchSetResponseTypeDef,
     GetGeoMatchSetResponseTypeDef,
     UpdateGeoMatchSetRequestRequestTypeDef,
     SampledHTTPRequestTypeDef,
     CreateIPSetResponseTypeDef,
     GetIPSetResponseTypeDef,
     UpdateIPSetRequestRequestTypeDef,
     CreateRateBasedRuleResponseTypeDef,
     GetRateBasedRuleResponseTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     UpdateRateBasedRuleRequestRequestTypeDef,
     UpdateRuleRequestRequestTypeDef,
-    UpdateRuleGroupRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateWebACLResponseTypeDef,
     GetWebACLResponseTypeDef,
+    UpdateRuleGroupRequestRequestTypeDef,
     UpdateWebACLRequestRequestTypeDef,
     CreateByteMatchSetResponseTypeDef,
     GetByteMatchSetResponseTypeDef,
-    UpdateByteMatchSetRequestRequestTypeDef,
     CreateRegexMatchSetResponseTypeDef,
     GetRegexMatchSetResponseTypeDef,
-    UpdateRegexMatchSetRequestRequestTypeDef,
     CreateSizeConstraintSetResponseTypeDef,
     GetSizeConstraintSetResponseTypeDef,
-    UpdateSizeConstraintSetRequestRequestTypeDef,
     CreateSqlInjectionMatchSetResponseTypeDef,
     GetSqlInjectionMatchSetResponseTypeDef,
-    UpdateSqlInjectionMatchSetRequestRequestTypeDef,
     CreateXssMatchSetResponseTypeDef,
     GetXssMatchSetResponseTypeDef,
+    UpdateByteMatchSetRequestRequestTypeDef,
+    UpdateRegexMatchSetRequestRequestTypeDef,
+    UpdateSizeConstraintSetRequestRequestTypeDef,
+    UpdateSqlInjectionMatchSetRequestRequestTypeDef,
     UpdateXssMatchSetRequestRequestTypeDef,
     GetSampledRequestsResponseTypeDef,
 )
 
 
-def get_structure() -> ExcludedRuleTypeDef:
+def get_structure() -> ExcludedRuleOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-waf-1.28.0/mypy_boto3_waf.egg-info/SOURCES.txt` & `mypy-boto3-waf-1.28.12/mypy_boto3_waf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.0/setup.py` & `mypy-boto3-waf-1.28.12/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-waf",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_waf"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WAF 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.WAF 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

