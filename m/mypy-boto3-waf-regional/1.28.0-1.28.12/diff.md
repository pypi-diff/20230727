# Comparing `tmp/mypy-boto3-waf-regional-1.28.0.tar.gz` & `tmp/mypy-boto3-waf-regional-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-waf-regional-1.28.0.tar", last modified: Thu Jul  6 21:00:50 2023, max compression
+gzip compressed data, was "mypy-boto3-waf-regional-1.28.12.tar", last modified: Thu Jul 27 11:49:49 2023, max compression
```

## Comparing `mypy-boto3-waf-regional-1.28.0.tar` & `mypy-boto3-waf-regional-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:50.446457 mypy-boto3-waf-regional-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:57:45.000000 mypy-boto3-waf-regional-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20419 2023-07-06 21:00:50.446457 mypy-boto3-waf-regional-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-07-06 20:57:45.000000 mypy-boto3-waf-regional-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:50.446457 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-06 20:57:45.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-06 20:57:45.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-06 20:57:45.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46208 2023-07-06 20:57:45.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    46120 2023-07-06 20:57:45.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-07-06 20:57:46.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-07-06 20:57:46.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:57:45.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55486 2023-07-06 20:57:47.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55439 2023-07-06 20:57:47.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:57:45.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:50.446457 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20419 2023-07-06 21:00:50.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-06 21:00:50.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:50.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:50.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:50.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 21:00:50.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:50.446457 mypy-boto3-waf-regional-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-06 20:57:45.000000 mypy-boto3-waf-regional-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.193489 mypy-boto3-waf-regional-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:27.000000 mypy-boto3-waf-regional-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20932 2023-07-27 11:49:49.189489 mypy-boto3-waf-regional-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-07-27 11:48:27.000000 mypy-boto3-waf-regional-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.185489 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-27 11:48:27.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-27 11:48:27.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-27 11:48:27.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46208 2023-07-27 11:48:28.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46120 2023-07-27 11:48:27.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-27 11:48:28.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-07-27 11:48:28.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:27.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59977 2023-07-27 11:48:29.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59924 2023-07-27 11:48:29.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:27.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.189489 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20932 2023-07-27 11:49:48.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-27 11:49:49.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:48.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:48.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:48.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 11:49:48.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:49.193489 mypy-boto3-waf-regional-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-27 11:48:27.000000 mypy-boto3-waf-regional-1.28.12/setup.py
```

### Comparing `mypy-boto3-waf-regional-1.28.0/LICENSE` & `mypy-boto3-waf-regional-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.28.0/PKG-INFO` & `mypy-boto3-waf-regional-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-waf-regional
-Version: 1.28.0
-Summary: Type annotations for boto3.WAFRegional 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.WAFRegional 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-waf-regional"></a>
 
 # mypy-boto3-waf-regional
 
 [![PyPI - mypy-boto3-waf-regional](https://img.shields.io/pypi/v/mypy-boto3-waf-regional.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf-regional)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf-regional.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf-regional)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-waf-regional?color=blue)](https://pypistats.org/packages/mypy-boto3-waf-regional)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-waf-regional)](https://pepy.tech/project/mypy-boto3-waf-regional)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFRegional 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
+[boto3.WAFRegional 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
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
 [mypy-boto3-waf-regional docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,144 +311,159 @@
 ### Typed dictionaries
 
 `mypy_boto3_waf_regional.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_waf_regional.type_defs import (
+    ExcludedRuleOutputTypeDef,
+    WafActionOutputTypeDef,
+    WafOverrideActionOutputTypeDef,
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
     AssociateWebACLRequestRequestTypeDef,
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
     DisassociateWebACLRequestRequestTypeDef,
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
     GetWebACLForResourceRequestRequestTypeDef,
     WebACLSummaryTypeDef,
     GetWebACLRequestRequestTypeDef,
     GetXssMatchSetRequestRequestTypeDef,
     HTTPHeaderTypeDef,
+    IPSetDescriptorOutputTypeDef,
     IPSetDescriptorTypeDef,
     IPSetSummaryTypeDef,
     ListActivatedRulesInRuleGroupRequestRequestTypeDef,
     ListByteMatchSetsRequestRequestTypeDef,
     ListGeoMatchSetsRequestRequestTypeDef,
     ListIPSetsRequestRequestTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
     ListRateBasedRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
     ListRegexMatchSetsRequestRequestTypeDef,
     RegexMatchSetSummaryTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     RegexPatternSetSummaryTypeDef,
     ListResourcesForWebACLRequestRequestTypeDef,
-    ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupSummaryTypeDef,
     ListRulesRequestRequestTypeDef,
     ListSizeConstraintSetsRequestRequestTypeDef,
     SizeConstraintSetSummaryTypeDef,
     ListSqlInjectionMatchSetsRequestRequestTypeDef,
     SqlInjectionMatchSetSummaryTypeDef,
     ListSubscribedRuleGroupsRequestRequestTypeDef,
     SubscribedRuleGroupSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     ListXssMatchSetsRequestRequestTypeDef,
     XssMatchSetSummaryTypeDef,
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
+    ListResourcesForWebACLResponseTypeDef,
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
@@ -469,70 +484,71 @@
     ListSqlInjectionMatchSetsResponseTypeDef,
     ListSubscribedRuleGroupsResponseTypeDef,
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

### Comparing `mypy-boto3-waf-regional-1.28.0/README.md` & `mypy-boto3-waf-regional-1.28.12/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-waf-regional"></a>
 
 # mypy-boto3-waf-regional
 
 [![PyPI - mypy-boto3-waf-regional](https://img.shields.io/pypi/v/mypy-boto3-waf-regional.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf-regional)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf-regional.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf-regional)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-waf-regional?color=blue)](https://pypistats.org/packages/mypy-boto3-waf-regional)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-waf-regional)](https://pepy.tech/project/mypy-boto3-waf-regional)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFRegional 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
+[boto3.WAFRegional 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
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
 [mypy-boto3-waf-regional docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/).
 
 See how it helps to find and fix potential bugs:
 
@@ -279,144 +279,159 @@
 ### Typed dictionaries
 
 `mypy_boto3_waf_regional.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_waf_regional.type_defs import (
+    ExcludedRuleOutputTypeDef,
+    WafActionOutputTypeDef,
+    WafOverrideActionOutputTypeDef,
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
     AssociateWebACLRequestRequestTypeDef,
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
     DisassociateWebACLRequestRequestTypeDef,
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
     GetWebACLForResourceRequestRequestTypeDef,
     WebACLSummaryTypeDef,
     GetWebACLRequestRequestTypeDef,
     GetXssMatchSetRequestRequestTypeDef,
     HTTPHeaderTypeDef,
+    IPSetDescriptorOutputTypeDef,
     IPSetDescriptorTypeDef,
     IPSetSummaryTypeDef,
     ListActivatedRulesInRuleGroupRequestRequestTypeDef,
     ListByteMatchSetsRequestRequestTypeDef,
     ListGeoMatchSetsRequestRequestTypeDef,
     ListIPSetsRequestRequestTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
     ListRateBasedRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
     ListRegexMatchSetsRequestRequestTypeDef,
     RegexMatchSetSummaryTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     RegexPatternSetSummaryTypeDef,
     ListResourcesForWebACLRequestRequestTypeDef,
-    ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupSummaryTypeDef,
     ListRulesRequestRequestTypeDef,
     ListSizeConstraintSetsRequestRequestTypeDef,
     SizeConstraintSetSummaryTypeDef,
     ListSqlInjectionMatchSetsRequestRequestTypeDef,
     SqlInjectionMatchSetSummaryTypeDef,
     ListSubscribedRuleGroupsRequestRequestTypeDef,
     SubscribedRuleGroupSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     ListXssMatchSetsRequestRequestTypeDef,
     XssMatchSetSummaryTypeDef,
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
+    ListResourcesForWebACLResponseTypeDef,
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
@@ -437,70 +452,71 @@
     ListSqlInjectionMatchSetsResponseTypeDef,
     ListSubscribedRuleGroupsResponseTypeDef,
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

### Comparing `mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/__main__.py` & `mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WAFRegional 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.WAFRegional 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional\nOther"
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

### Comparing `mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/client.py` & `mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/client.pyi` & `mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/literals.py` & `mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -437,14 +437,15 @@
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
@@ -523,26 +524,28 @@
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

### Comparing `mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/literals.pyi` & `mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -435,14 +435,15 @@
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
@@ -521,26 +522,28 @@
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

### Comparing `mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/type_defs.py` & `mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 Type annotations for waf-regional service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_waf_regional.type_defs import ExcludedRuleTypeDef
+    from mypy_boto3_waf_regional.type_defs import ExcludedRuleOutputTypeDef
 
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
@@ -38,144 +40,159 @@
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
     "AssociateWebACLRequestRequestTypeDef",
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
     "DisassociateWebACLRequestRequestTypeDef",
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
     "GetWebACLForResourceRequestRequestTypeDef",
     "WebACLSummaryTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "GetXssMatchSetRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
+    "IPSetDescriptorOutputTypeDef",
     "IPSetDescriptorTypeDef",
     "IPSetSummaryTypeDef",
     "ListActivatedRulesInRuleGroupRequestRequestTypeDef",
     "ListByteMatchSetsRequestRequestTypeDef",
     "ListGeoMatchSetsRequestRequestTypeDef",
     "ListIPSetsRequestRequestTypeDef",
     "ListLoggingConfigurationsRequestRequestTypeDef",
     "ListRateBasedRulesRequestRequestTypeDef",
     "RuleSummaryTypeDef",
     "ListRegexMatchSetsRequestRequestTypeDef",
     "RegexMatchSetSummaryTypeDef",
     "ListRegexPatternSetsRequestRequestTypeDef",
     "RegexPatternSetSummaryTypeDef",
     "ListResourcesForWebACLRequestRequestTypeDef",
-    "ListResourcesForWebACLResponseTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "RuleGroupSummaryTypeDef",
     "ListRulesRequestRequestTypeDef",
     "ListSizeConstraintSetsRequestRequestTypeDef",
     "SizeConstraintSetSummaryTypeDef",
     "ListSqlInjectionMatchSetsRequestRequestTypeDef",
     "SqlInjectionMatchSetSummaryTypeDef",
     "ListSubscribedRuleGroupsRequestRequestTypeDef",
     "SubscribedRuleGroupSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "ListXssMatchSetsRequestRequestTypeDef",
     "XssMatchSetSummaryTypeDef",
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
+    "ListResourcesForWebACLResponseTypeDef",
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
@@ -196,68 +213,90 @@
     "ListSqlInjectionMatchSetsResponseTypeDef",
     "ListSubscribedRuleGroupsResponseTypeDef",
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
 
@@ -287,14 +326,35 @@
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
@@ -314,14 +374,25 @@
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
@@ -419,22 +490,14 @@
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
@@ -443,54 +506,30 @@
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
 
@@ -505,154 +544,90 @@
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
+DisassociateWebACLRequestRequestTypeDef = TypedDict(
+    "DisassociateWebACLRequestRequestTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceArn": str,
     },
 )
 
-DisassociateWebACLRequestRequestTypeDef = TypedDict(
-    "DisassociateWebACLRequestRequestTypeDef",
+GeoMatchConstraintOutputTypeDef = TypedDict(
+    "GeoMatchConstraintOutputTypeDef",
     {
-        "ResourceArn": str,
+        "Type": Literal["Country"],
+        "Value": GeoMatchConstraintValueType,
     },
 )
 
 GeoMatchConstraintTypeDef = TypedDict(
     "GeoMatchConstraintTypeDef",
     {
         "Type": Literal["Country"],
@@ -671,37 +646,21 @@
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
 
@@ -722,22 +681,14 @@
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
 _RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef = TypedDict(
     "_RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef",
     {
         "RuleId": str,
     },
 )
 _OptionalGetRateBasedRuleManagedKeysRequestRequestTypeDef = TypedDict(
@@ -752,23 +703,14 @@
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
 
@@ -804,14 +746,22 @@
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
 
@@ -856,14 +806,22 @@
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
@@ -991,22 +949,14 @@
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
 ListRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListRuleGroupsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1126,14 +1076,23 @@
     "XssMatchSetSummaryTypeDef",
     {
         "XssMatchSetId": str,
         "Name": str,
     },
 )
 
+PredicateOutputTypeDef = TypedDict(
+    "PredicateOutputTypeDef",
+    {
+        "Negated": bool,
+        "Type": PredicateTypeType,
+        "DataId": str,
+    },
+)
+
 PredicateTypeDef = TypedDict(
     "PredicateTypeDef",
     {
         "Negated": bool,
         "Type": PredicateTypeType,
         "DataId": str,
     },
@@ -1151,182 +1110,166 @@
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
@@ -1365,14 +1308,264 @@
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
+ListResourcesForWebACLResponseTypeDef = TypedDict(
+    "ListResourcesForWebACLResponseTypeDef",
+    {
+        "ResourceArns": List[str],
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
@@ -1461,70 +1654,61 @@
 
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
@@ -1545,15 +1729,15 @@
 )
 
 ListGeoMatchSetsResponseTypeDef = TypedDict(
     "ListGeoMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "GeoMatchSets": List[GeoMatchSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSampledRequestsRequestRequestTypeDef = TypedDict(
     "GetSampledRequestsRequestRequestTypeDef",
     {
         "WebAclId": str,
@@ -1563,24 +1747,24 @@
     },
 )
 
 GetWebACLForResourceResponseTypeDef = TypedDict(
     "GetWebACLForResourceResponseTypeDef",
     {
         "WebACLSummary": WebACLSummaryTypeDef,
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
 
 HTTPRequestTypeDef = TypedDict(
     "HTTPRequestTypeDef",
     {
         "ClientIP": str,
@@ -1593,15 +1777,15 @@
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
@@ -1622,104 +1806,104 @@
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
@@ -1734,15 +1918,15 @@
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
@@ -1768,37 +1952,38 @@
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
@@ -1808,27 +1993,35 @@
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
@@ -1836,77 +2029,54 @@
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
@@ -1916,27 +2086,19 @@
 
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
@@ -1946,27 +2108,19 @@
 
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
@@ -1974,45 +2128,75 @@
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
@@ -2046,23 +2230,23 @@
 
 
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
@@ -2072,40 +2256,40 @@
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
@@ -2120,37 +2304,46 @@
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
@@ -2174,127 +2367,127 @@
 
 
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
@@ -2304,11 +2497,11 @@
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

### Comparing `mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/type_defs.pyi` & `mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 Type annotations for waf-regional service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_waf_regional.type_defs import ExcludedRuleTypeDef
+    from mypy_boto3_waf_regional.type_defs import ExcludedRuleOutputTypeDef
 
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
@@ -37,144 +39,159 @@
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
     "AssociateWebACLRequestRequestTypeDef",
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
     "DisassociateWebACLRequestRequestTypeDef",
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
     "GetWebACLForResourceRequestRequestTypeDef",
     "WebACLSummaryTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "GetXssMatchSetRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
+    "IPSetDescriptorOutputTypeDef",
     "IPSetDescriptorTypeDef",
     "IPSetSummaryTypeDef",
     "ListActivatedRulesInRuleGroupRequestRequestTypeDef",
     "ListByteMatchSetsRequestRequestTypeDef",
     "ListGeoMatchSetsRequestRequestTypeDef",
     "ListIPSetsRequestRequestTypeDef",
     "ListLoggingConfigurationsRequestRequestTypeDef",
     "ListRateBasedRulesRequestRequestTypeDef",
     "RuleSummaryTypeDef",
     "ListRegexMatchSetsRequestRequestTypeDef",
     "RegexMatchSetSummaryTypeDef",
     "ListRegexPatternSetsRequestRequestTypeDef",
     "RegexPatternSetSummaryTypeDef",
     "ListResourcesForWebACLRequestRequestTypeDef",
-    "ListResourcesForWebACLResponseTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "RuleGroupSummaryTypeDef",
     "ListRulesRequestRequestTypeDef",
     "ListSizeConstraintSetsRequestRequestTypeDef",
     "SizeConstraintSetSummaryTypeDef",
     "ListSqlInjectionMatchSetsRequestRequestTypeDef",
     "SqlInjectionMatchSetSummaryTypeDef",
     "ListSubscribedRuleGroupsRequestRequestTypeDef",
     "SubscribedRuleGroupSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "ListXssMatchSetsRequestRequestTypeDef",
     "XssMatchSetSummaryTypeDef",
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
+    "ListResourcesForWebACLResponseTypeDef",
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
@@ -195,68 +212,90 @@
     "ListSqlInjectionMatchSetsResponseTypeDef",
     "ListSubscribedRuleGroupsResponseTypeDef",
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
 
@@ -286,14 +325,33 @@
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
@@ -311,14 +369,25 @@
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
@@ -412,22 +481,14 @@
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
@@ -436,54 +497,30 @@
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
 
@@ -498,154 +535,90 @@
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
+DisassociateWebACLRequestRequestTypeDef = TypedDict(
+    "DisassociateWebACLRequestRequestTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceArn": str,
     },
 )
 
-DisassociateWebACLRequestRequestTypeDef = TypedDict(
-    "DisassociateWebACLRequestRequestTypeDef",
+GeoMatchConstraintOutputTypeDef = TypedDict(
+    "GeoMatchConstraintOutputTypeDef",
     {
-        "ResourceArn": str,
+        "Type": Literal["Country"],
+        "Value": GeoMatchConstraintValueType,
     },
 )
 
 GeoMatchConstraintTypeDef = TypedDict(
     "GeoMatchConstraintTypeDef",
     {
         "Type": Literal["Country"],
@@ -664,37 +637,21 @@
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
 
@@ -715,22 +672,14 @@
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
 _RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef = TypedDict(
     "_RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef",
     {
         "RuleId": str,
     },
 )
 _OptionalGetRateBasedRuleManagedKeysRequestRequestTypeDef = TypedDict(
@@ -743,23 +692,14 @@
 
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
 
@@ -795,14 +735,22 @@
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
 
@@ -847,14 +795,22 @@
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
@@ -980,22 +936,14 @@
 
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
 ListRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListRuleGroupsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1113,14 +1061,23 @@
     "XssMatchSetSummaryTypeDef",
     {
         "XssMatchSetId": str,
         "Name": str,
     },
 )
 
+PredicateOutputTypeDef = TypedDict(
+    "PredicateOutputTypeDef",
+    {
+        "Negated": bool,
+        "Type": PredicateTypeType,
+        "DataId": str,
+    },
+)
+
 PredicateTypeDef = TypedDict(
     "PredicateTypeDef",
     {
         "Negated": bool,
         "Type": PredicateTypeType,
         "DataId": str,
     },
@@ -1138,180 +1095,160 @@
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
@@ -1348,14 +1285,264 @@
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
+ListResourcesForWebACLResponseTypeDef = TypedDict(
+    "ListResourcesForWebACLResponseTypeDef",
+    {
+        "ResourceArns": List[str],
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
@@ -1436,70 +1623,61 @@
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
@@ -1518,15 +1696,15 @@
 )
 
 ListGeoMatchSetsResponseTypeDef = TypedDict(
     "ListGeoMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "GeoMatchSets": List[GeoMatchSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSampledRequestsRequestRequestTypeDef = TypedDict(
     "GetSampledRequestsRequestRequestTypeDef",
     {
         "WebAclId": str,
@@ -1536,24 +1714,24 @@
     },
 )
 
 GetWebACLForResourceResponseTypeDef = TypedDict(
     "GetWebACLForResourceResponseTypeDef",
     {
         "WebACLSummary": WebACLSummaryTypeDef,
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
 
 HTTPRequestTypeDef = TypedDict(
     "HTTPRequestTypeDef",
     {
         "ClientIP": str,
@@ -1566,15 +1744,15 @@
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
@@ -1593,104 +1771,104 @@
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
@@ -1703,15 +1881,15 @@
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
@@ -1735,37 +1913,38 @@
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
@@ -1773,103 +1952,88 @@
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
@@ -1877,27 +2041,19 @@
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
@@ -1905,71 +2061,93 @@
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
@@ -2001,23 +2179,23 @@
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
@@ -2027,40 +2205,40 @@
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
@@ -2075,37 +2253,46 @@
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
@@ -2127,127 +2314,127 @@
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
@@ -2257,11 +2444,11 @@
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

### Comparing `mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional.egg-info/PKG-INFO` & `mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-waf-regional
-Version: 1.28.0
-Summary: Type annotations for boto3.WAFRegional 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.WAFRegional 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-waf-regional"></a>
 
 # mypy-boto3-waf-regional
 
 [![PyPI - mypy-boto3-waf-regional](https://img.shields.io/pypi/v/mypy-boto3-waf-regional.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf-regional)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf-regional.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf-regional)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-waf-regional?color=blue)](https://pypistats.org/packages/mypy-boto3-waf-regional)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-waf-regional)](https://pepy.tech/project/mypy-boto3-waf-regional)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFRegional 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
+[boto3.WAFRegional 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
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
 [mypy-boto3-waf-regional docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,144 +311,159 @@
 ### Typed dictionaries
 
 `mypy_boto3_waf_regional.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_waf_regional.type_defs import (
+    ExcludedRuleOutputTypeDef,
+    WafActionOutputTypeDef,
+    WafOverrideActionOutputTypeDef,
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
     AssociateWebACLRequestRequestTypeDef,
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
     DisassociateWebACLRequestRequestTypeDef,
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
     GetWebACLForResourceRequestRequestTypeDef,
     WebACLSummaryTypeDef,
     GetWebACLRequestRequestTypeDef,
     GetXssMatchSetRequestRequestTypeDef,
     HTTPHeaderTypeDef,
+    IPSetDescriptorOutputTypeDef,
     IPSetDescriptorTypeDef,
     IPSetSummaryTypeDef,
     ListActivatedRulesInRuleGroupRequestRequestTypeDef,
     ListByteMatchSetsRequestRequestTypeDef,
     ListGeoMatchSetsRequestRequestTypeDef,
     ListIPSetsRequestRequestTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
     ListRateBasedRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
     ListRegexMatchSetsRequestRequestTypeDef,
     RegexMatchSetSummaryTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     RegexPatternSetSummaryTypeDef,
     ListResourcesForWebACLRequestRequestTypeDef,
-    ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupSummaryTypeDef,
     ListRulesRequestRequestTypeDef,
     ListSizeConstraintSetsRequestRequestTypeDef,
     SizeConstraintSetSummaryTypeDef,
     ListSqlInjectionMatchSetsRequestRequestTypeDef,
     SqlInjectionMatchSetSummaryTypeDef,
     ListSubscribedRuleGroupsRequestRequestTypeDef,
     SubscribedRuleGroupSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     ListXssMatchSetsRequestRequestTypeDef,
     XssMatchSetSummaryTypeDef,
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
+    ListResourcesForWebACLResponseTypeDef,
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
@@ -469,70 +484,71 @@
     ListSqlInjectionMatchSetsResponseTypeDef,
     ListSubscribedRuleGroupsResponseTypeDef,
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

### Comparing `mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional.egg-info/SOURCES.txt` & `mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.28.0/setup.py` & `mypy-boto3-waf-regional-1.28.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-waf-regional",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_waf_regional"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WAFRegional 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.WAFRegional 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

