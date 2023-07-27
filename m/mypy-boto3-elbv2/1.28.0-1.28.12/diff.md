# Comparing `tmp/mypy-boto3-elbv2-1.28.0.tar.gz` & `tmp/mypy-boto3-elbv2-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elbv2-1.28.0.tar", last modified: Thu Jul  6 20:59:33 2023, max compression
+gzip compressed data, was "mypy-boto3-elbv2-1.28.12.tar", last modified: Thu Jul 27 05:34:39 2023, max compression
```

## Comparing `mypy-boto3-elbv2-1.28.0.tar` & `mypy-boto3-elbv2-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:33.178298 mypy-boto3-elbv2-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:40:29.000000 mypy-boto3-elbv2-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19879 2023-07-06 20:59:33.178298 mypy-boto3-elbv2-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-07-06 20:40:29.000000 mypy-boto3-elbv2-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:33.166298 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-06 20:40:29.000000 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-06 20:40:29.000000 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-06 20:40:29.000000 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33888 2023-07-06 20:40:29.000000 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33835 2023-07-06 20:40:29.000000 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-07-06 20:40:30.000000 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-07-06 20:40:30.000000 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-07-06 20:40:29.000000 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-07-06 20:40:29.000000 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:40:29.000000 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    38668 2023-07-06 20:40:32.000000 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38627 2023-07-06 20:40:32.000000 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:40:29.000000 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-07-06 20:40:29.000000 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-06 20:40:29.000000 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:33.178298 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19879 2023-07-06 20:59:32.000000 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 20:59:32.000000 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:32.000000 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:32.000000 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:32.000000 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 20:59:32.000000 mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:33.178298 mypy-boto3-elbv2-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-06 20:40:29.000000 mypy-boto3-elbv2-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:39.964516 mypy-boto3-elbv2-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20734 2023-07-27 05:34:39.964516 mypy-boto3-elbv2-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19238 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:39.964516 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33888 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33835 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    47068 2023-07-27 05:21:56.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47013 2023-07-27 05:21:56.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:39.964516 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20734 2023-07-27 05:34:39.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-27 05:34:39.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:39.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:39.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:39.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 05:34:39.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:39.964516 mypy-boto3-elbv2-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/setup.py
```

### Comparing `mypy-boto3-elbv2-1.28.0/LICENSE` & `mypy-boto3-elbv2-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.0/PKG-INFO` & `mypy-boto3-elbv2-1.28.12/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elbv2
-Version: 1.28.0
-Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-elbv2"></a>
 
 # mypy-boto3-elbv2
 
 [![PyPI - mypy-boto3-elbv2](https://img.shields.io/pypi/v/mypy-boto3-elbv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-elbv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elbv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-elbv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elbv2?color=blue)](https://pypistats.org/packages/mypy-boto3-elbv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elbv2)](https://pepy.tech/project/mypy-boto3-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancingv2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
+[boto3.ElasticLoadBalancingv2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
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
 [mypy-boto3-elbv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -404,19 +404,24 @@
 ### Typed dictionaries
 
 `mypy_boto3_elbv2.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elbv2.type_defs import (
+    AuthenticateCognitoActionConfigOutputTypeDef,
+    AuthenticateOidcActionConfigOutputTypeDef,
+    FixedResponseActionConfigOutputTypeDef,
+    RedirectActionConfigOutputTypeDef,
     AuthenticateCognitoActionConfigTypeDef,
     AuthenticateOidcActionConfigTypeDef,
     FixedResponseActionConfigTypeDef,
     RedirectActionConfigTypeDef,
     CertificateTypeDef,
+    CertificateOutputTypeDef,
     TagTypeDef,
     LoadBalancerAddressTypeDef,
     CipherTypeDef,
     SubnetMappingTypeDef,
     MatcherTypeDef,
     DeleteListenerInputRequestTypeDef,
     DeleteLoadBalancerInputRequestTypeDef,
@@ -427,106 +432,123 @@
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
     DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
     DescribeListenerCertificatesInputRequestTypeDef,
     DescribeListenersInputDescribeListenersPaginateTypeDef,
     DescribeListenersInputRequestTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
-    LoadBalancerAttributeTypeDef,
+    LoadBalancerAttributeOutputTypeDef,
     DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeLoadBalancersInputRequestTypeDef,
     DescribeRulesInputDescribeRulesPaginateTypeDef,
     DescribeRulesInputRequestTypeDef,
     DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef,
     DescribeSSLPoliciesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DescribeTargetGroupAttributesInputRequestTypeDef,
-    TargetGroupAttributeTypeDef,
+    TargetGroupAttributeOutputTypeDef,
     DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef,
     DescribeTargetGroupsInputRequestTypeDef,
+    TargetGroupStickinessConfigOutputTypeDef,
+    TargetGroupTupleOutputTypeDef,
     TargetGroupStickinessConfigTypeDef,
     TargetGroupTupleTypeDef,
+    HostHeaderConditionConfigOutputTypeDef,
     HostHeaderConditionConfigTypeDef,
+    HttpHeaderConditionConfigOutputTypeDef,
     HttpHeaderConditionConfigTypeDef,
+    HttpRequestMethodConditionConfigOutputTypeDef,
     HttpRequestMethodConditionConfigTypeDef,
+    LoadBalancerAttributeTypeDef,
     LoadBalancerStateTypeDef,
+    MatcherOutputTypeDef,
+    TargetGroupAttributeTypeDef,
     PaginatorConfigTypeDef,
+    PathPatternConditionConfigOutputTypeDef,
     PathPatternConditionConfigTypeDef,
+    QueryStringKeyValuePairOutputTypeDef,
     QueryStringKeyValuePairTypeDef,
     RemoveTagsInputRequestTypeDef,
     ResponseMetadataTypeDef,
+    SourceIpConditionConfigOutputTypeDef,
     SourceIpConditionConfigTypeDef,
     RulePriorityPairTypeDef,
     SetIpAddressTypeInputRequestTypeDef,
     SetIpAddressTypeOutputTypeDef,
     SetSecurityGroupsInputRequestTypeDef,
     SetSecurityGroupsOutputTypeDef,
+    TagOutputTypeDef,
+    TargetDescriptionOutputTypeDef,
     TargetHealthTypeDef,
     AddListenerCertificatesInputRequestTypeDef,
+    RemoveListenerCertificatesInputRequestTypeDef,
     AddListenerCertificatesOutputTypeDef,
     DescribeListenerCertificatesOutputTypeDef,
-    RemoveListenerCertificatesInputRequestTypeDef,
     AddTagsInputRequestTypeDef,
-    TagDescriptionTypeDef,
     AvailabilityZoneTypeDef,
     SslPolicyTypeDef,
     CreateLoadBalancerInputRequestTypeDef,
     SetSubnetsInputRequestTypeDef,
     CreateTargetGroupInputRequestTypeDef,
     ModifyTargetGroupInputRequestTypeDef,
-    TargetGroupTypeDef,
     DeregisterTargetsInputRequestTypeDef,
     DescribeTargetHealthInputRequestTypeDef,
     RegisterTargetsInputRequestTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeLoadBalancerAttributesOutputTypeDef,
-    ModifyLoadBalancerAttributesInputRequestTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef,
     DescribeTargetHealthInputTargetDeregisteredWaitTypeDef,
     DescribeTargetHealthInputTargetInServiceWaitTypeDef,
     DescribeTargetGroupAttributesOutputTypeDef,
-    ModifyTargetGroupAttributesInputRequestTypeDef,
     ModifyTargetGroupAttributesOutputTypeDef,
+    ForwardActionConfigOutputTypeDef,
     ForwardActionConfigTypeDef,
+    ModifyLoadBalancerAttributesInputRequestTypeDef,
+    TargetGroupTypeDef,
+    ModifyTargetGroupAttributesInputRequestTypeDef,
+    QueryStringConditionConfigOutputTypeDef,
     QueryStringConditionConfigTypeDef,
     SetRulePrioritiesInputRequestTypeDef,
+    TagDescriptionTypeDef,
     TargetHealthDescriptionTypeDef,
-    DescribeTagsOutputTypeDef,
     LoadBalancerTypeDef,
     SetSubnetsOutputTypeDef,
     DescribeSSLPoliciesOutputTypeDef,
+    ActionOutputTypeDef,
+    ActionTypeDef,
     CreateTargetGroupOutputTypeDef,
     DescribeTargetGroupsOutputTypeDef,
     ModifyTargetGroupOutputTypeDef,
-    ActionTypeDef,
+    RuleConditionOutputTypeDef,
     RuleConditionTypeDef,
+    DescribeTagsOutputTypeDef,
     DescribeTargetHealthOutputTypeDef,
     CreateLoadBalancerOutputTypeDef,
     DescribeLoadBalancersOutputTypeDef,
-    CreateListenerInputRequestTypeDef,
     ListenerTypeDef,
+    CreateListenerInputRequestTypeDef,
     ModifyListenerInputRequestTypeDef,
+    RuleTypeDef,
     CreateRuleInputRequestTypeDef,
     ModifyRuleInputRequestTypeDef,
-    RuleTypeDef,
     CreateListenerOutputTypeDef,
     DescribeListenersOutputTypeDef,
     ModifyListenerOutputTypeDef,
     CreateRuleOutputTypeDef,
     DescribeRulesOutputTypeDef,
     ModifyRuleOutputTypeDef,
     SetRulePrioritiesOutputTypeDef,
 )
 
 
-def get_structure() -> AuthenticateCognitoActionConfigTypeDef:
+def get_structure() -> AuthenticateCognitoActionConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elbv2-1.28.0/README.md` & `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-elbv2
+Version: 1.28.12
+Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 elbv2 type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-elbv2"></a>
 
 # mypy-boto3-elbv2
 
 [![PyPI - mypy-boto3-elbv2](https://img.shields.io/pypi/v/mypy-boto3-elbv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-elbv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elbv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-elbv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elbv2?color=blue)](https://pypistats.org/packages/mypy-boto3-elbv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elbv2)](https://pepy.tech/project/mypy-boto3-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancingv2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
+[boto3.ElasticLoadBalancingv2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
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
 [mypy-boto3-elbv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -372,19 +404,24 @@
 ### Typed dictionaries
 
 `mypy_boto3_elbv2.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elbv2.type_defs import (
+    AuthenticateCognitoActionConfigOutputTypeDef,
+    AuthenticateOidcActionConfigOutputTypeDef,
+    FixedResponseActionConfigOutputTypeDef,
+    RedirectActionConfigOutputTypeDef,
     AuthenticateCognitoActionConfigTypeDef,
     AuthenticateOidcActionConfigTypeDef,
     FixedResponseActionConfigTypeDef,
     RedirectActionConfigTypeDef,
     CertificateTypeDef,
+    CertificateOutputTypeDef,
     TagTypeDef,
     LoadBalancerAddressTypeDef,
     CipherTypeDef,
     SubnetMappingTypeDef,
     MatcherTypeDef,
     DeleteListenerInputRequestTypeDef,
     DeleteLoadBalancerInputRequestTypeDef,
@@ -395,106 +432,123 @@
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
     DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
     DescribeListenerCertificatesInputRequestTypeDef,
     DescribeListenersInputDescribeListenersPaginateTypeDef,
     DescribeListenersInputRequestTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
-    LoadBalancerAttributeTypeDef,
+    LoadBalancerAttributeOutputTypeDef,
     DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeLoadBalancersInputRequestTypeDef,
     DescribeRulesInputDescribeRulesPaginateTypeDef,
     DescribeRulesInputRequestTypeDef,
     DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef,
     DescribeSSLPoliciesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DescribeTargetGroupAttributesInputRequestTypeDef,
-    TargetGroupAttributeTypeDef,
+    TargetGroupAttributeOutputTypeDef,
     DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef,
     DescribeTargetGroupsInputRequestTypeDef,
+    TargetGroupStickinessConfigOutputTypeDef,
+    TargetGroupTupleOutputTypeDef,
     TargetGroupStickinessConfigTypeDef,
     TargetGroupTupleTypeDef,
+    HostHeaderConditionConfigOutputTypeDef,
     HostHeaderConditionConfigTypeDef,
+    HttpHeaderConditionConfigOutputTypeDef,
     HttpHeaderConditionConfigTypeDef,
+    HttpRequestMethodConditionConfigOutputTypeDef,
     HttpRequestMethodConditionConfigTypeDef,
+    LoadBalancerAttributeTypeDef,
     LoadBalancerStateTypeDef,
+    MatcherOutputTypeDef,
+    TargetGroupAttributeTypeDef,
     PaginatorConfigTypeDef,
+    PathPatternConditionConfigOutputTypeDef,
     PathPatternConditionConfigTypeDef,
+    QueryStringKeyValuePairOutputTypeDef,
     QueryStringKeyValuePairTypeDef,
     RemoveTagsInputRequestTypeDef,
     ResponseMetadataTypeDef,
+    SourceIpConditionConfigOutputTypeDef,
     SourceIpConditionConfigTypeDef,
     RulePriorityPairTypeDef,
     SetIpAddressTypeInputRequestTypeDef,
     SetIpAddressTypeOutputTypeDef,
     SetSecurityGroupsInputRequestTypeDef,
     SetSecurityGroupsOutputTypeDef,
+    TagOutputTypeDef,
+    TargetDescriptionOutputTypeDef,
     TargetHealthTypeDef,
     AddListenerCertificatesInputRequestTypeDef,
+    RemoveListenerCertificatesInputRequestTypeDef,
     AddListenerCertificatesOutputTypeDef,
     DescribeListenerCertificatesOutputTypeDef,
-    RemoveListenerCertificatesInputRequestTypeDef,
     AddTagsInputRequestTypeDef,
-    TagDescriptionTypeDef,
     AvailabilityZoneTypeDef,
     SslPolicyTypeDef,
     CreateLoadBalancerInputRequestTypeDef,
     SetSubnetsInputRequestTypeDef,
     CreateTargetGroupInputRequestTypeDef,
     ModifyTargetGroupInputRequestTypeDef,
-    TargetGroupTypeDef,
     DeregisterTargetsInputRequestTypeDef,
     DescribeTargetHealthInputRequestTypeDef,
     RegisterTargetsInputRequestTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeLoadBalancerAttributesOutputTypeDef,
-    ModifyLoadBalancerAttributesInputRequestTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef,
     DescribeTargetHealthInputTargetDeregisteredWaitTypeDef,
     DescribeTargetHealthInputTargetInServiceWaitTypeDef,
     DescribeTargetGroupAttributesOutputTypeDef,
-    ModifyTargetGroupAttributesInputRequestTypeDef,
     ModifyTargetGroupAttributesOutputTypeDef,
+    ForwardActionConfigOutputTypeDef,
     ForwardActionConfigTypeDef,
+    ModifyLoadBalancerAttributesInputRequestTypeDef,
+    TargetGroupTypeDef,
+    ModifyTargetGroupAttributesInputRequestTypeDef,
+    QueryStringConditionConfigOutputTypeDef,
     QueryStringConditionConfigTypeDef,
     SetRulePrioritiesInputRequestTypeDef,
+    TagDescriptionTypeDef,
     TargetHealthDescriptionTypeDef,
-    DescribeTagsOutputTypeDef,
     LoadBalancerTypeDef,
     SetSubnetsOutputTypeDef,
     DescribeSSLPoliciesOutputTypeDef,
+    ActionOutputTypeDef,
+    ActionTypeDef,
     CreateTargetGroupOutputTypeDef,
     DescribeTargetGroupsOutputTypeDef,
     ModifyTargetGroupOutputTypeDef,
-    ActionTypeDef,
+    RuleConditionOutputTypeDef,
     RuleConditionTypeDef,
+    DescribeTagsOutputTypeDef,
     DescribeTargetHealthOutputTypeDef,
     CreateLoadBalancerOutputTypeDef,
     DescribeLoadBalancersOutputTypeDef,
-    CreateListenerInputRequestTypeDef,
     ListenerTypeDef,
+    CreateListenerInputRequestTypeDef,
     ModifyListenerInputRequestTypeDef,
+    RuleTypeDef,
     CreateRuleInputRequestTypeDef,
     ModifyRuleInputRequestTypeDef,
-    RuleTypeDef,
     CreateListenerOutputTypeDef,
     DescribeListenersOutputTypeDef,
     ModifyListenerOutputTypeDef,
     CreateRuleOutputTypeDef,
     DescribeRulesOutputTypeDef,
     ModifyRuleOutputTypeDef,
     SetRulePrioritiesOutputTypeDef,
 )
 
 
-def get_structure() -> AuthenticateCognitoActionConfigTypeDef:
+def get_structure() -> AuthenticateCognitoActionConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/__init__.py` & `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/__init__.pyi` & `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/__main__.py` & `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElasticLoadBalancingv2 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ElasticLoadBalancingv2 1.28.12\nVersion:        "
+        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2\nOther"
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

### Comparing `mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/client.py` & `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/client.pyi` & `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/literals.py` & `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,14 +212,15 @@
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
@@ -298,26 +299,28 @@
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

### Comparing `mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/literals.pyi` & `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -210,14 +210,15 @@
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
@@ -296,26 +297,28 @@
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

### Comparing `mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/paginator.py` & `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/paginator.pyi` & `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/type_defs.py` & `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for elbv2 service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_elbv2.type_defs import AuthenticateCognitoActionConfigTypeDef
+    from mypy_boto3_elbv2.type_defs import AuthenticateCognitoActionConfigOutputTypeDef
 
-    data: AuthenticateCognitoActionConfigTypeDef = {...}
+    data: AuthenticateCognitoActionConfigOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -32,21 +32,25 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "AuthenticateCognitoActionConfigOutputTypeDef",
+    "AuthenticateOidcActionConfigOutputTypeDef",
+    "FixedResponseActionConfigOutputTypeDef",
+    "RedirectActionConfigOutputTypeDef",
     "AuthenticateCognitoActionConfigTypeDef",
     "AuthenticateOidcActionConfigTypeDef",
     "FixedResponseActionConfigTypeDef",
     "RedirectActionConfigTypeDef",
     "CertificateTypeDef",
+    "CertificateOutputTypeDef",
     "TagTypeDef",
     "LoadBalancerAddressTypeDef",
     "CipherTypeDef",
     "SubnetMappingTypeDef",
     "MatcherTypeDef",
     "DeleteListenerInputRequestTypeDef",
     "DeleteLoadBalancerInputRequestTypeDef",
@@ -57,104 +61,220 @@
     "DescribeAccountLimitsInputRequestTypeDef",
     "LimitTypeDef",
     "DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
     "DescribeListenerCertificatesInputRequestTypeDef",
     "DescribeListenersInputDescribeListenersPaginateTypeDef",
     "DescribeListenersInputRequestTypeDef",
     "DescribeLoadBalancerAttributesInputRequestTypeDef",
-    "LoadBalancerAttributeTypeDef",
+    "LoadBalancerAttributeOutputTypeDef",
     "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
     "WaiterConfigTypeDef",
     "DescribeLoadBalancersInputRequestTypeDef",
     "DescribeRulesInputDescribeRulesPaginateTypeDef",
     "DescribeRulesInputRequestTypeDef",
     "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
     "DescribeSSLPoliciesInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "DescribeTargetGroupAttributesInputRequestTypeDef",
-    "TargetGroupAttributeTypeDef",
+    "TargetGroupAttributeOutputTypeDef",
     "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
     "DescribeTargetGroupsInputRequestTypeDef",
+    "TargetGroupStickinessConfigOutputTypeDef",
+    "TargetGroupTupleOutputTypeDef",
     "TargetGroupStickinessConfigTypeDef",
     "TargetGroupTupleTypeDef",
+    "HostHeaderConditionConfigOutputTypeDef",
     "HostHeaderConditionConfigTypeDef",
+    "HttpHeaderConditionConfigOutputTypeDef",
     "HttpHeaderConditionConfigTypeDef",
+    "HttpRequestMethodConditionConfigOutputTypeDef",
     "HttpRequestMethodConditionConfigTypeDef",
+    "LoadBalancerAttributeTypeDef",
     "LoadBalancerStateTypeDef",
+    "MatcherOutputTypeDef",
+    "TargetGroupAttributeTypeDef",
     "PaginatorConfigTypeDef",
+    "PathPatternConditionConfigOutputTypeDef",
     "PathPatternConditionConfigTypeDef",
+    "QueryStringKeyValuePairOutputTypeDef",
     "QueryStringKeyValuePairTypeDef",
     "RemoveTagsInputRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "SourceIpConditionConfigOutputTypeDef",
     "SourceIpConditionConfigTypeDef",
     "RulePriorityPairTypeDef",
     "SetIpAddressTypeInputRequestTypeDef",
     "SetIpAddressTypeOutputTypeDef",
     "SetSecurityGroupsInputRequestTypeDef",
     "SetSecurityGroupsOutputTypeDef",
+    "TagOutputTypeDef",
+    "TargetDescriptionOutputTypeDef",
     "TargetHealthTypeDef",
     "AddListenerCertificatesInputRequestTypeDef",
+    "RemoveListenerCertificatesInputRequestTypeDef",
     "AddListenerCertificatesOutputTypeDef",
     "DescribeListenerCertificatesOutputTypeDef",
-    "RemoveListenerCertificatesInputRequestTypeDef",
     "AddTagsInputRequestTypeDef",
-    "TagDescriptionTypeDef",
     "AvailabilityZoneTypeDef",
     "SslPolicyTypeDef",
     "CreateLoadBalancerInputRequestTypeDef",
     "SetSubnetsInputRequestTypeDef",
     "CreateTargetGroupInputRequestTypeDef",
     "ModifyTargetGroupInputRequestTypeDef",
-    "TargetGroupTypeDef",
     "DeregisterTargetsInputRequestTypeDef",
     "DescribeTargetHealthInputRequestTypeDef",
     "RegisterTargetsInputRequestTypeDef",
     "DescribeAccountLimitsOutputTypeDef",
     "DescribeLoadBalancerAttributesOutputTypeDef",
-    "ModifyLoadBalancerAttributesInputRequestTypeDef",
     "ModifyLoadBalancerAttributesOutputTypeDef",
     "DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef",
     "DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef",
     "DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef",
     "DescribeTargetHealthInputTargetDeregisteredWaitTypeDef",
     "DescribeTargetHealthInputTargetInServiceWaitTypeDef",
     "DescribeTargetGroupAttributesOutputTypeDef",
-    "ModifyTargetGroupAttributesInputRequestTypeDef",
     "ModifyTargetGroupAttributesOutputTypeDef",
+    "ForwardActionConfigOutputTypeDef",
     "ForwardActionConfigTypeDef",
+    "ModifyLoadBalancerAttributesInputRequestTypeDef",
+    "TargetGroupTypeDef",
+    "ModifyTargetGroupAttributesInputRequestTypeDef",
+    "QueryStringConditionConfigOutputTypeDef",
     "QueryStringConditionConfigTypeDef",
     "SetRulePrioritiesInputRequestTypeDef",
+    "TagDescriptionTypeDef",
     "TargetHealthDescriptionTypeDef",
-    "DescribeTagsOutputTypeDef",
     "LoadBalancerTypeDef",
     "SetSubnetsOutputTypeDef",
     "DescribeSSLPoliciesOutputTypeDef",
+    "ActionOutputTypeDef",
+    "ActionTypeDef",
     "CreateTargetGroupOutputTypeDef",
     "DescribeTargetGroupsOutputTypeDef",
     "ModifyTargetGroupOutputTypeDef",
-    "ActionTypeDef",
+    "RuleConditionOutputTypeDef",
     "RuleConditionTypeDef",
+    "DescribeTagsOutputTypeDef",
     "DescribeTargetHealthOutputTypeDef",
     "CreateLoadBalancerOutputTypeDef",
     "DescribeLoadBalancersOutputTypeDef",
-    "CreateListenerInputRequestTypeDef",
     "ListenerTypeDef",
+    "CreateListenerInputRequestTypeDef",
     "ModifyListenerInputRequestTypeDef",
+    "RuleTypeDef",
     "CreateRuleInputRequestTypeDef",
     "ModifyRuleInputRequestTypeDef",
-    "RuleTypeDef",
     "CreateListenerOutputTypeDef",
     "DescribeListenersOutputTypeDef",
     "ModifyListenerOutputTypeDef",
     "CreateRuleOutputTypeDef",
     "DescribeRulesOutputTypeDef",
     "ModifyRuleOutputTypeDef",
     "SetRulePrioritiesOutputTypeDef",
 )
 
+_RequiredAuthenticateCognitoActionConfigOutputTypeDef = TypedDict(
+    "_RequiredAuthenticateCognitoActionConfigOutputTypeDef",
+    {
+        "UserPoolArn": str,
+        "UserPoolClientId": str,
+        "UserPoolDomain": str,
+    },
+)
+_OptionalAuthenticateCognitoActionConfigOutputTypeDef = TypedDict(
+    "_OptionalAuthenticateCognitoActionConfigOutputTypeDef",
+    {
+        "SessionCookieName": str,
+        "Scope": str,
+        "SessionTimeout": int,
+        "AuthenticationRequestExtraParams": Dict[str, str],
+        "OnUnauthenticatedRequest": AuthenticateCognitoActionConditionalBehaviorEnumType,
+    },
+    total=False,
+)
+
+class AuthenticateCognitoActionConfigOutputTypeDef(
+    _RequiredAuthenticateCognitoActionConfigOutputTypeDef,
+    _OptionalAuthenticateCognitoActionConfigOutputTypeDef,
+):
+    pass
+
+_RequiredAuthenticateOidcActionConfigOutputTypeDef = TypedDict(
+    "_RequiredAuthenticateOidcActionConfigOutputTypeDef",
+    {
+        "Issuer": str,
+        "AuthorizationEndpoint": str,
+        "TokenEndpoint": str,
+        "UserInfoEndpoint": str,
+        "ClientId": str,
+    },
+)
+_OptionalAuthenticateOidcActionConfigOutputTypeDef = TypedDict(
+    "_OptionalAuthenticateOidcActionConfigOutputTypeDef",
+    {
+        "ClientSecret": str,
+        "SessionCookieName": str,
+        "Scope": str,
+        "SessionTimeout": int,
+        "AuthenticationRequestExtraParams": Dict[str, str],
+        "OnUnauthenticatedRequest": AuthenticateOidcActionConditionalBehaviorEnumType,
+        "UseExistingClientSecret": bool,
+    },
+    total=False,
+)
+
+class AuthenticateOidcActionConfigOutputTypeDef(
+    _RequiredAuthenticateOidcActionConfigOutputTypeDef,
+    _OptionalAuthenticateOidcActionConfigOutputTypeDef,
+):
+    pass
+
+_RequiredFixedResponseActionConfigOutputTypeDef = TypedDict(
+    "_RequiredFixedResponseActionConfigOutputTypeDef",
+    {
+        "StatusCode": str,
+    },
+)
+_OptionalFixedResponseActionConfigOutputTypeDef = TypedDict(
+    "_OptionalFixedResponseActionConfigOutputTypeDef",
+    {
+        "MessageBody": str,
+        "ContentType": str,
+    },
+    total=False,
+)
+
+class FixedResponseActionConfigOutputTypeDef(
+    _RequiredFixedResponseActionConfigOutputTypeDef, _OptionalFixedResponseActionConfigOutputTypeDef
+):
+    pass
+
+_RequiredRedirectActionConfigOutputTypeDef = TypedDict(
+    "_RequiredRedirectActionConfigOutputTypeDef",
+    {
+        "StatusCode": RedirectActionStatusCodeEnumType,
+    },
+)
+_OptionalRedirectActionConfigOutputTypeDef = TypedDict(
+    "_OptionalRedirectActionConfigOutputTypeDef",
+    {
+        "Protocol": str,
+        "Port": str,
+        "Host": str,
+        "Path": str,
+        "Query": str,
+    },
+    total=False,
+)
+
+class RedirectActionConfigOutputTypeDef(
+    _RequiredRedirectActionConfigOutputTypeDef, _OptionalRedirectActionConfigOutputTypeDef
+):
+    pass
+
 _RequiredAuthenticateCognitoActionConfigTypeDef = TypedDict(
     "_RequiredAuthenticateCognitoActionConfigTypeDef",
     {
         "UserPoolArn": str,
         "UserPoolClientId": str,
         "UserPoolDomain": str,
     },
@@ -167,21 +287,19 @@
         "SessionTimeout": int,
         "AuthenticationRequestExtraParams": Mapping[str, str],
         "OnUnauthenticatedRequest": AuthenticateCognitoActionConditionalBehaviorEnumType,
     },
     total=False,
 )
 
-
 class AuthenticateCognitoActionConfigTypeDef(
     _RequiredAuthenticateCognitoActionConfigTypeDef, _OptionalAuthenticateCognitoActionConfigTypeDef
 ):
     pass
 
-
 _RequiredAuthenticateOidcActionConfigTypeDef = TypedDict(
     "_RequiredAuthenticateOidcActionConfigTypeDef",
     {
         "Issuer": str,
         "AuthorizationEndpoint": str,
         "TokenEndpoint": str,
         "UserInfoEndpoint": str,
@@ -198,21 +316,19 @@
         "AuthenticationRequestExtraParams": Mapping[str, str],
         "OnUnauthenticatedRequest": AuthenticateOidcActionConditionalBehaviorEnumType,
         "UseExistingClientSecret": bool,
     },
     total=False,
 )
 
-
 class AuthenticateOidcActionConfigTypeDef(
     _RequiredAuthenticateOidcActionConfigTypeDef, _OptionalAuthenticateOidcActionConfigTypeDef
 ):
     pass
 
-
 _RequiredFixedResponseActionConfigTypeDef = TypedDict(
     "_RequiredFixedResponseActionConfigTypeDef",
     {
         "StatusCode": str,
     },
 )
 _OptionalFixedResponseActionConfigTypeDef = TypedDict(
@@ -220,21 +336,19 @@
     {
         "MessageBody": str,
         "ContentType": str,
     },
     total=False,
 )
 
-
 class FixedResponseActionConfigTypeDef(
     _RequiredFixedResponseActionConfigTypeDef, _OptionalFixedResponseActionConfigTypeDef
 ):
     pass
 
-
 _RequiredRedirectActionConfigTypeDef = TypedDict(
     "_RequiredRedirectActionConfigTypeDef",
     {
         "StatusCode": RedirectActionStatusCodeEnumType,
     },
 )
 _OptionalRedirectActionConfigTypeDef = TypedDict(
@@ -245,49 +359,54 @@
         "Host": str,
         "Path": str,
         "Query": str,
     },
     total=False,
 )
 
-
 class RedirectActionConfigTypeDef(
     _RequiredRedirectActionConfigTypeDef, _OptionalRedirectActionConfigTypeDef
 ):
     pass
 
-
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "CertificateArn": str,
         "IsDefault": bool,
     },
     total=False,
 )
 
+CertificateOutputTypeDef = TypedDict(
+    "CertificateOutputTypeDef",
+    {
+        "CertificateArn": str,
+        "IsDefault": bool,
+    },
+    total=False,
+)
+
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-
 LoadBalancerAddressTypeDef = TypedDict(
     "LoadBalancerAddressTypeDef",
     {
         "IpAddress": str,
         "AllocationId": str,
         "PrivateIPv4Address": str,
         "IPv6Address": str,
@@ -363,21 +482,19 @@
     {
         "Port": int,
         "AvailabilityZone": str,
     },
     total=False,
 )
 
-
 class TargetDescriptionTypeDef(
     _RequiredTargetDescriptionTypeDef, _OptionalTargetDescriptionTypeDef
 ):
     pass
 
-
 DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
     "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -410,22 +527,20 @@
     "_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef(
     _RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
     _OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeListenerCertificatesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeListenerCertificatesInputRequestTypeDef",
     {
         "ListenerArn": str,
     },
 )
 _OptionalDescribeListenerCertificatesInputRequestTypeDef = TypedDict(
@@ -433,22 +548,20 @@
     {
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
-
 class DescribeListenerCertificatesInputRequestTypeDef(
     _RequiredDescribeListenerCertificatesInputRequestTypeDef,
     _OptionalDescribeListenerCertificatesInputRequestTypeDef,
 ):
     pass
 
-
 DescribeListenersInputDescribeListenersPaginateTypeDef = TypedDict(
     "DescribeListenersInputDescribeListenersPaginateTypeDef",
     {
         "LoadBalancerArn": str,
         "ListenerArns": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -469,16 +582,16 @@
 DescribeLoadBalancerAttributesInputRequestTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
     },
 )
 
-LoadBalancerAttributeTypeDef = TypedDict(
-    "LoadBalancerAttributeTypeDef",
+LoadBalancerAttributeOutputTypeDef = TypedDict(
+    "LoadBalancerAttributeOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
@@ -564,16 +677,16 @@
 DescribeTargetGroupAttributesInputRequestTypeDef = TypedDict(
     "DescribeTargetGroupAttributesInputRequestTypeDef",
     {
         "TargetGroupArn": str,
     },
 )
 
-TargetGroupAttributeTypeDef = TypedDict(
-    "TargetGroupAttributeTypeDef",
+TargetGroupAttributeOutputTypeDef = TypedDict(
+    "TargetGroupAttributeOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
@@ -596,14 +709,32 @@
         "Names": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
+TargetGroupStickinessConfigOutputTypeDef = TypedDict(
+    "TargetGroupStickinessConfigOutputTypeDef",
+    {
+        "Enabled": bool,
+        "DurationSeconds": int,
+    },
+    total=False,
+)
+
+TargetGroupTupleOutputTypeDef = TypedDict(
+    "TargetGroupTupleOutputTypeDef",
+    {
+        "TargetGroupArn": str,
+        "Weight": int,
+    },
+    total=False,
+)
+
 TargetGroupStickinessConfigTypeDef = TypedDict(
     "TargetGroupStickinessConfigTypeDef",
     {
         "Enabled": bool,
         "DurationSeconds": int,
     },
     total=False,
@@ -614,66 +745,135 @@
     {
         "TargetGroupArn": str,
         "Weight": int,
     },
     total=False,
 )
 
+HostHeaderConditionConfigOutputTypeDef = TypedDict(
+    "HostHeaderConditionConfigOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+    total=False,
+)
+
 HostHeaderConditionConfigTypeDef = TypedDict(
     "HostHeaderConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
 
+HttpHeaderConditionConfigOutputTypeDef = TypedDict(
+    "HttpHeaderConditionConfigOutputTypeDef",
+    {
+        "HttpHeaderName": str,
+        "Values": List[str],
+    },
+    total=False,
+)
+
 HttpHeaderConditionConfigTypeDef = TypedDict(
     "HttpHeaderConditionConfigTypeDef",
     {
         "HttpHeaderName": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
+HttpRequestMethodConditionConfigOutputTypeDef = TypedDict(
+    "HttpRequestMethodConditionConfigOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+    total=False,
+)
+
 HttpRequestMethodConditionConfigTypeDef = TypedDict(
     "HttpRequestMethodConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
 
+LoadBalancerAttributeTypeDef = TypedDict(
+    "LoadBalancerAttributeTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 LoadBalancerStateTypeDef = TypedDict(
     "LoadBalancerStateTypeDef",
     {
         "Code": LoadBalancerStateEnumType,
         "Reason": str,
     },
     total=False,
 )
 
+MatcherOutputTypeDef = TypedDict(
+    "MatcherOutputTypeDef",
+    {
+        "HttpCode": str,
+        "GrpcCode": str,
+    },
+    total=False,
+)
+
+TargetGroupAttributeTypeDef = TypedDict(
+    "TargetGroupAttributeTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+PathPatternConditionConfigOutputTypeDef = TypedDict(
+    "PathPatternConditionConfigOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+    total=False,
+)
+
 PathPatternConditionConfigTypeDef = TypedDict(
     "PathPatternConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
 
+QueryStringKeyValuePairOutputTypeDef = TypedDict(
+    "QueryStringKeyValuePairOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 QueryStringKeyValuePairTypeDef = TypedDict(
     "QueryStringKeyValuePairTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -694,14 +894,22 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+SourceIpConditionConfigOutputTypeDef = TypedDict(
+    "SourceIpConditionConfigOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+    total=False,
+)
+
 SourceIpConditionConfigTypeDef = TypedDict(
     "SourceIpConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
@@ -743,14 +951,51 @@
     "SetSecurityGroupsOutputTypeDef",
     {
         "SecurityGroupIds": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
+    pass
+
+_RequiredTargetDescriptionOutputTypeDef = TypedDict(
+    "_RequiredTargetDescriptionOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalTargetDescriptionOutputTypeDef = TypedDict(
+    "_OptionalTargetDescriptionOutputTypeDef",
+    {
+        "Port": int,
+        "AvailabilityZone": str,
+    },
+    total=False,
+)
+
+class TargetDescriptionOutputTypeDef(
+    _RequiredTargetDescriptionOutputTypeDef, _OptionalTargetDescriptionOutputTypeDef
+):
+    pass
+
 TargetHealthTypeDef = TypedDict(
     "TargetHealthTypeDef",
     {
         "State": TargetHealthStateEnumType,
         "Reason": TargetHealthReasonEnumType,
         "Description": str,
     },
@@ -761,56 +1006,47 @@
     "AddListenerCertificatesInputRequestTypeDef",
     {
         "ListenerArn": str,
         "Certificates": Sequence[CertificateTypeDef],
     },
 )
 
+RemoveListenerCertificatesInputRequestTypeDef = TypedDict(
+    "RemoveListenerCertificatesInputRequestTypeDef",
+    {
+        "ListenerArn": str,
+        "Certificates": Sequence[CertificateTypeDef],
+    },
+)
+
 AddListenerCertificatesOutputTypeDef = TypedDict(
     "AddListenerCertificatesOutputTypeDef",
     {
-        "Certificates": List[CertificateTypeDef],
+        "Certificates": List[CertificateOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeListenerCertificatesOutputTypeDef = TypedDict(
     "DescribeListenerCertificatesOutputTypeDef",
     {
-        "Certificates": List[CertificateTypeDef],
+        "Certificates": List[CertificateOutputTypeDef],
         "NextMarker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RemoveListenerCertificatesInputRequestTypeDef = TypedDict(
-    "RemoveListenerCertificatesInputRequestTypeDef",
-    {
-        "ListenerArn": str,
-        "Certificates": Sequence[CertificateTypeDef],
-    },
-)
-
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "ResourceArns": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-TagDescriptionTypeDef = TypedDict(
-    "TagDescriptionTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "ZoneName": str,
         "SubnetId": str,
         "OutpostId": str,
         "LoadBalancerAddresses": List[LoadBalancerAddressTypeDef],
@@ -846,21 +1082,19 @@
         "Type": LoadBalancerTypeEnumType,
         "IpAddressType": IpAddressTypeType,
         "CustomerOwnedIpv4Pool": str,
     },
     total=False,
 )
 
-
 class CreateLoadBalancerInputRequestTypeDef(
     _RequiredCreateLoadBalancerInputRequestTypeDef, _OptionalCreateLoadBalancerInputRequestTypeDef
 ):
     pass
 
-
 _RequiredSetSubnetsInputRequestTypeDef = TypedDict(
     "_RequiredSetSubnetsInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
     },
 )
 _OptionalSetSubnetsInputRequestTypeDef = TypedDict(
@@ -869,21 +1103,19 @@
         "Subnets": Sequence[str],
         "SubnetMappings": Sequence[SubnetMappingTypeDef],
         "IpAddressType": IpAddressTypeType,
     },
     total=False,
 )
 
-
 class SetSubnetsInputRequestTypeDef(
     _RequiredSetSubnetsInputRequestTypeDef, _OptionalSetSubnetsInputRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateTargetGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateTargetGroupInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateTargetGroupInputRequestTypeDef = TypedDict(
@@ -905,21 +1137,19 @@
         "TargetType": TargetTypeEnumType,
         "Tags": Sequence[TagTypeDef],
         "IpAddressType": TargetGroupIpAddressTypeEnumType,
     },
     total=False,
 )
 
-
 class CreateTargetGroupInputRequestTypeDef(
     _RequiredCreateTargetGroupInputRequestTypeDef, _OptionalCreateTargetGroupInputRequestTypeDef
 ):
     pass
 
-
 _RequiredModifyTargetGroupInputRequestTypeDef = TypedDict(
     "_RequiredModifyTargetGroupInputRequestTypeDef",
     {
         "TargetGroupArn": str,
     },
 )
 _OptionalModifyTargetGroupInputRequestTypeDef = TypedDict(
@@ -934,46 +1164,19 @@
         "HealthyThresholdCount": int,
         "UnhealthyThresholdCount": int,
         "Matcher": MatcherTypeDef,
     },
     total=False,
 )
 
-
 class ModifyTargetGroupInputRequestTypeDef(
     _RequiredModifyTargetGroupInputRequestTypeDef, _OptionalModifyTargetGroupInputRequestTypeDef
 ):
     pass
 
-
-TargetGroupTypeDef = TypedDict(
-    "TargetGroupTypeDef",
-    {
-        "TargetGroupArn": str,
-        "TargetGroupName": str,
-        "Protocol": ProtocolEnumType,
-        "Port": int,
-        "VpcId": str,
-        "HealthCheckProtocol": ProtocolEnumType,
-        "HealthCheckPort": str,
-        "HealthCheckEnabled": bool,
-        "HealthCheckIntervalSeconds": int,
-        "HealthCheckTimeoutSeconds": int,
-        "HealthyThresholdCount": int,
-        "UnhealthyThresholdCount": int,
-        "HealthCheckPath": str,
-        "Matcher": MatcherTypeDef,
-        "LoadBalancerArns": List[str],
-        "TargetType": TargetTypeEnumType,
-        "ProtocolVersion": str,
-        "IpAddressType": TargetGroupIpAddressTypeEnumType,
-    },
-    total=False,
-)
-
 DeregisterTargetsInputRequestTypeDef = TypedDict(
     "DeregisterTargetsInputRequestTypeDef",
     {
         "TargetGroupArn": str,
         "Targets": Sequence[TargetDescriptionTypeDef],
     },
 )
@@ -988,22 +1191,20 @@
     "_OptionalDescribeTargetHealthInputRequestTypeDef",
     {
         "Targets": Sequence[TargetDescriptionTypeDef],
     },
     total=False,
 )
 
-
 class DescribeTargetHealthInputRequestTypeDef(
     _RequiredDescribeTargetHealthInputRequestTypeDef,
     _OptionalDescribeTargetHealthInputRequestTypeDef,
 ):
     pass
 
-
 RegisterTargetsInputRequestTypeDef = TypedDict(
     "RegisterTargetsInputRequestTypeDef",
     {
         "TargetGroupArn": str,
         "Targets": Sequence[TargetDescriptionTypeDef],
     },
 )
@@ -1016,31 +1217,23 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLoadBalancerAttributesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesOutputTypeDef",
     {
-        "Attributes": List[LoadBalancerAttributeTypeDef],
+        "Attributes": List[LoadBalancerAttributeOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
-    "ModifyLoadBalancerAttributesInputRequestTypeDef",
-    {
-        "LoadBalancerArn": str,
-        "Attributes": Sequence[LoadBalancerAttributeTypeDef],
-    },
-)
-
 ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
     "ModifyLoadBalancerAttributesOutputTypeDef",
     {
-        "Attributes": List[LoadBalancerAttributeTypeDef],
+        "Attributes": List[LoadBalancerAttributeOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef = TypedDict(
     "DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef",
     {
@@ -1088,22 +1281,20 @@
     {
         "Targets": Sequence[TargetDescriptionTypeDef],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeTargetHealthInputTargetDeregisteredWaitTypeDef(
     _RequiredDescribeTargetHealthInputTargetDeregisteredWaitTypeDef,
     _OptionalDescribeTargetHealthInputTargetDeregisteredWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeTargetHealthInputTargetInServiceWaitTypeDef = TypedDict(
     "_RequiredDescribeTargetHealthInputTargetInServiceWaitTypeDef",
     {
         "TargetGroupArn": str,
     },
 )
 _OptionalDescribeTargetHealthInputTargetInServiceWaitTypeDef = TypedDict(
@@ -1111,55 +1302,103 @@
     {
         "Targets": Sequence[TargetDescriptionTypeDef],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeTargetHealthInputTargetInServiceWaitTypeDef(
     _RequiredDescribeTargetHealthInputTargetInServiceWaitTypeDef,
     _OptionalDescribeTargetHealthInputTargetInServiceWaitTypeDef,
 ):
     pass
 
-
 DescribeTargetGroupAttributesOutputTypeDef = TypedDict(
     "DescribeTargetGroupAttributesOutputTypeDef",
     {
-        "Attributes": List[TargetGroupAttributeTypeDef],
+        "Attributes": List[TargetGroupAttributeOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyTargetGroupAttributesInputRequestTypeDef = TypedDict(
-    "ModifyTargetGroupAttributesInputRequestTypeDef",
+ModifyTargetGroupAttributesOutputTypeDef = TypedDict(
+    "ModifyTargetGroupAttributesOutputTypeDef",
     {
-        "TargetGroupArn": str,
-        "Attributes": Sequence[TargetGroupAttributeTypeDef],
+        "Attributes": List[TargetGroupAttributeOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyTargetGroupAttributesOutputTypeDef = TypedDict(
-    "ModifyTargetGroupAttributesOutputTypeDef",
+ForwardActionConfigOutputTypeDef = TypedDict(
+    "ForwardActionConfigOutputTypeDef",
     {
-        "Attributes": List[TargetGroupAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TargetGroups": List[TargetGroupTupleOutputTypeDef],
+        "TargetGroupStickinessConfig": TargetGroupStickinessConfigOutputTypeDef,
     },
+    total=False,
 )
 
 ForwardActionConfigTypeDef = TypedDict(
     "ForwardActionConfigTypeDef",
     {
         "TargetGroups": Sequence[TargetGroupTupleTypeDef],
         "TargetGroupStickinessConfig": TargetGroupStickinessConfigTypeDef,
     },
     total=False,
 )
 
+ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
+    "ModifyLoadBalancerAttributesInputRequestTypeDef",
+    {
+        "LoadBalancerArn": str,
+        "Attributes": Sequence[LoadBalancerAttributeTypeDef],
+    },
+)
+
+TargetGroupTypeDef = TypedDict(
+    "TargetGroupTypeDef",
+    {
+        "TargetGroupArn": str,
+        "TargetGroupName": str,
+        "Protocol": ProtocolEnumType,
+        "Port": int,
+        "VpcId": str,
+        "HealthCheckProtocol": ProtocolEnumType,
+        "HealthCheckPort": str,
+        "HealthCheckEnabled": bool,
+        "HealthCheckIntervalSeconds": int,
+        "HealthCheckTimeoutSeconds": int,
+        "HealthyThresholdCount": int,
+        "UnhealthyThresholdCount": int,
+        "HealthCheckPath": str,
+        "Matcher": MatcherOutputTypeDef,
+        "LoadBalancerArns": List[str],
+        "TargetType": TargetTypeEnumType,
+        "ProtocolVersion": str,
+        "IpAddressType": TargetGroupIpAddressTypeEnumType,
+    },
+    total=False,
+)
+
+ModifyTargetGroupAttributesInputRequestTypeDef = TypedDict(
+    "ModifyTargetGroupAttributesInputRequestTypeDef",
+    {
+        "TargetGroupArn": str,
+        "Attributes": Sequence[TargetGroupAttributeTypeDef],
+    },
+)
+
+QueryStringConditionConfigOutputTypeDef = TypedDict(
+    "QueryStringConditionConfigOutputTypeDef",
+    {
+        "Values": List[QueryStringKeyValuePairOutputTypeDef],
+    },
+    total=False,
+)
+
 QueryStringConditionConfigTypeDef = TypedDict(
     "QueryStringConditionConfigTypeDef",
     {
         "Values": Sequence[QueryStringKeyValuePairTypeDef],
     },
     total=False,
 )
@@ -1167,30 +1406,31 @@
 SetRulePrioritiesInputRequestTypeDef = TypedDict(
     "SetRulePrioritiesInputRequestTypeDef",
     {
         "RulePriorities": Sequence[RulePriorityPairTypeDef],
     },
 )
 
-TargetHealthDescriptionTypeDef = TypedDict(
-    "TargetHealthDescriptionTypeDef",
+TagDescriptionTypeDef = TypedDict(
+    "TagDescriptionTypeDef",
     {
-        "Target": TargetDescriptionTypeDef,
-        "HealthCheckPort": str,
-        "TargetHealth": TargetHealthTypeDef,
+        "ResourceArn": str,
+        "Tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
-DescribeTagsOutputTypeDef = TypedDict(
-    "DescribeTagsOutputTypeDef",
+TargetHealthDescriptionTypeDef = TypedDict(
+    "TargetHealthDescriptionTypeDef",
     {
-        "TagDescriptions": List[TagDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Target": TargetDescriptionOutputTypeDef,
+        "HealthCheckPort": str,
+        "TargetHealth": TargetHealthTypeDef,
     },
+    total=False,
 )
 
 LoadBalancerTypeDef = TypedDict(
     "LoadBalancerTypeDef",
     {
         "LoadBalancerArn": str,
         "DNSName": str,
@@ -1223,38 +1463,36 @@
     {
         "SslPolicies": List[SslPolicyTypeDef],
         "NextMarker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateTargetGroupOutputTypeDef = TypedDict(
-    "CreateTargetGroupOutputTypeDef",
+_RequiredActionOutputTypeDef = TypedDict(
+    "_RequiredActionOutputTypeDef",
     {
-        "TargetGroups": List[TargetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Type": ActionTypeEnumType,
     },
 )
-
-DescribeTargetGroupsOutputTypeDef = TypedDict(
-    "DescribeTargetGroupsOutputTypeDef",
+_OptionalActionOutputTypeDef = TypedDict(
+    "_OptionalActionOutputTypeDef",
     {
-        "TargetGroups": List[TargetGroupTypeDef],
-        "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TargetGroupArn": str,
+        "AuthenticateOidcConfig": AuthenticateOidcActionConfigOutputTypeDef,
+        "AuthenticateCognitoConfig": AuthenticateCognitoActionConfigOutputTypeDef,
+        "Order": int,
+        "RedirectConfig": RedirectActionConfigOutputTypeDef,
+        "FixedResponseConfig": FixedResponseActionConfigOutputTypeDef,
+        "ForwardConfig": ForwardActionConfigOutputTypeDef,
     },
+    total=False,
 )
 
-ModifyTargetGroupOutputTypeDef = TypedDict(
-    "ModifyTargetGroupOutputTypeDef",
-    {
-        "TargetGroups": List[TargetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+class ActionOutputTypeDef(_RequiredActionOutputTypeDef, _OptionalActionOutputTypeDef):
+    pass
 
 _RequiredActionTypeDef = TypedDict(
     "_RequiredActionTypeDef",
     {
         "Type": ActionTypeEnumType,
     },
 )
@@ -1268,18 +1506,56 @@
         "RedirectConfig": RedirectActionConfigTypeDef,
         "FixedResponseConfig": FixedResponseActionConfigTypeDef,
         "ForwardConfig": ForwardActionConfigTypeDef,
     },
     total=False,
 )
 
-
 class ActionTypeDef(_RequiredActionTypeDef, _OptionalActionTypeDef):
     pass
 
+CreateTargetGroupOutputTypeDef = TypedDict(
+    "CreateTargetGroupOutputTypeDef",
+    {
+        "TargetGroups": List[TargetGroupTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeTargetGroupsOutputTypeDef = TypedDict(
+    "DescribeTargetGroupsOutputTypeDef",
+    {
+        "TargetGroups": List[TargetGroupTypeDef],
+        "NextMarker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ModifyTargetGroupOutputTypeDef = TypedDict(
+    "ModifyTargetGroupOutputTypeDef",
+    {
+        "TargetGroups": List[TargetGroupTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RuleConditionOutputTypeDef = TypedDict(
+    "RuleConditionOutputTypeDef",
+    {
+        "Field": str,
+        "Values": List[str],
+        "HostHeaderConfig": HostHeaderConditionConfigOutputTypeDef,
+        "PathPatternConfig": PathPatternConditionConfigOutputTypeDef,
+        "HttpHeaderConfig": HttpHeaderConditionConfigOutputTypeDef,
+        "QueryStringConfig": QueryStringConditionConfigOutputTypeDef,
+        "HttpRequestMethodConfig": HttpRequestMethodConditionConfigOutputTypeDef,
+        "SourceIpConfig": SourceIpConditionConfigOutputTypeDef,
+    },
+    total=False,
+)
 
 RuleConditionTypeDef = TypedDict(
     "RuleConditionTypeDef",
     {
         "Field": str,
         "Values": Sequence[str],
         "HostHeaderConfig": HostHeaderConditionConfigTypeDef,
@@ -1288,14 +1564,22 @@
         "QueryStringConfig": QueryStringConditionConfigTypeDef,
         "HttpRequestMethodConfig": HttpRequestMethodConditionConfigTypeDef,
         "SourceIpConfig": SourceIpConditionConfigTypeDef,
     },
     total=False,
 )
 
+DescribeTagsOutputTypeDef = TypedDict(
+    "DescribeTagsOutputTypeDef",
+    {
+        "TagDescriptions": List[TagDescriptionTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeTargetHealthOutputTypeDef = TypedDict(
     "DescribeTargetHealthOutputTypeDef",
     {
         "TargetHealthDescriptions": List[TargetHealthDescriptionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1313,14 +1597,29 @@
     {
         "LoadBalancers": List[LoadBalancerTypeDef],
         "NextMarker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListenerTypeDef = TypedDict(
+    "ListenerTypeDef",
+    {
+        "ListenerArn": str,
+        "LoadBalancerArn": str,
+        "Port": int,
+        "Protocol": ProtocolEnumType,
+        "Certificates": List[CertificateOutputTypeDef],
+        "SslPolicy": str,
+        "DefaultActions": List[ActionOutputTypeDef],
+        "AlpnPolicy": List[str],
+    },
+    total=False,
+)
+
 _RequiredCreateListenerInputRequestTypeDef = TypedDict(
     "_RequiredCreateListenerInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "DefaultActions": Sequence[ActionTypeDef],
     },
 )
@@ -1333,36 +1632,19 @@
         "Certificates": Sequence[CertificateTypeDef],
         "AlpnPolicy": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateListenerInputRequestTypeDef(
     _RequiredCreateListenerInputRequestTypeDef, _OptionalCreateListenerInputRequestTypeDef
 ):
     pass
 
-
-ListenerTypeDef = TypedDict(
-    "ListenerTypeDef",
-    {
-        "ListenerArn": str,
-        "LoadBalancerArn": str,
-        "Port": int,
-        "Protocol": ProtocolEnumType,
-        "Certificates": List[CertificateTypeDef],
-        "SslPolicy": str,
-        "DefaultActions": List[ActionTypeDef],
-        "AlpnPolicy": List[str],
-    },
-    total=False,
-)
-
 _RequiredModifyListenerInputRequestTypeDef = TypedDict(
     "_RequiredModifyListenerInputRequestTypeDef",
     {
         "ListenerArn": str,
     },
 )
 _OptionalModifyListenerInputRequestTypeDef = TypedDict(
@@ -1374,20 +1656,30 @@
         "Certificates": Sequence[CertificateTypeDef],
         "DefaultActions": Sequence[ActionTypeDef],
         "AlpnPolicy": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyListenerInputRequestTypeDef(
     _RequiredModifyListenerInputRequestTypeDef, _OptionalModifyListenerInputRequestTypeDef
 ):
     pass
 
+RuleTypeDef = TypedDict(
+    "RuleTypeDef",
+    {
+        "RuleArn": str,
+        "Priority": str,
+        "Conditions": List[RuleConditionOutputTypeDef],
+        "Actions": List[ActionOutputTypeDef],
+        "IsDefault": bool,
+    },
+    total=False,
+)
 
 _RequiredCreateRuleInputRequestTypeDef = TypedDict(
     "_RequiredCreateRuleInputRequestTypeDef",
     {
         "ListenerArn": str,
         "Conditions": Sequence[RuleConditionTypeDef],
         "Priority": int,
@@ -1398,21 +1690,19 @@
     "_OptionalCreateRuleInputRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateRuleInputRequestTypeDef(
     _RequiredCreateRuleInputRequestTypeDef, _OptionalCreateRuleInputRequestTypeDef
 ):
     pass
 
-
 _RequiredModifyRuleInputRequestTypeDef = TypedDict(
     "_RequiredModifyRuleInputRequestTypeDef",
     {
         "RuleArn": str,
     },
 )
 _OptionalModifyRuleInputRequestTypeDef = TypedDict(
@@ -1420,33 +1710,19 @@
     {
         "Conditions": Sequence[RuleConditionTypeDef],
         "Actions": Sequence[ActionTypeDef],
     },
     total=False,
 )
 
-
 class ModifyRuleInputRequestTypeDef(
     _RequiredModifyRuleInputRequestTypeDef, _OptionalModifyRuleInputRequestTypeDef
 ):
     pass
 
-
-RuleTypeDef = TypedDict(
-    "RuleTypeDef",
-    {
-        "RuleArn": str,
-        "Priority": str,
-        "Conditions": List[RuleConditionTypeDef],
-        "Actions": List[ActionTypeDef],
-        "IsDefault": bool,
-    },
-    total=False,
-)
-
 CreateListenerOutputTypeDef = TypedDict(
     "CreateListenerOutputTypeDef",
     {
         "Listeners": List[ListenerTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/type_defs.pyi` & `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for elbv2 service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_elbv2.type_defs import AuthenticateCognitoActionConfigTypeDef
+    from mypy_boto3_elbv2.type_defs import AuthenticateCognitoActionConfigOutputTypeDef
 
-    data: AuthenticateCognitoActionConfigTypeDef = {...}
+    data: AuthenticateCognitoActionConfigOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -32,20 +32,26 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "AuthenticateCognitoActionConfigOutputTypeDef",
+    "AuthenticateOidcActionConfigOutputTypeDef",
+    "FixedResponseActionConfigOutputTypeDef",
+    "RedirectActionConfigOutputTypeDef",
     "AuthenticateCognitoActionConfigTypeDef",
     "AuthenticateOidcActionConfigTypeDef",
     "FixedResponseActionConfigTypeDef",
     "RedirectActionConfigTypeDef",
     "CertificateTypeDef",
+    "CertificateOutputTypeDef",
     "TagTypeDef",
     "LoadBalancerAddressTypeDef",
     "CipherTypeDef",
     "SubnetMappingTypeDef",
     "MatcherTypeDef",
     "DeleteListenerInputRequestTypeDef",
     "DeleteLoadBalancerInputRequestTypeDef",
@@ -56,104 +62,228 @@
     "DescribeAccountLimitsInputRequestTypeDef",
     "LimitTypeDef",
     "DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
     "DescribeListenerCertificatesInputRequestTypeDef",
     "DescribeListenersInputDescribeListenersPaginateTypeDef",
     "DescribeListenersInputRequestTypeDef",
     "DescribeLoadBalancerAttributesInputRequestTypeDef",
-    "LoadBalancerAttributeTypeDef",
+    "LoadBalancerAttributeOutputTypeDef",
     "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
     "WaiterConfigTypeDef",
     "DescribeLoadBalancersInputRequestTypeDef",
     "DescribeRulesInputDescribeRulesPaginateTypeDef",
     "DescribeRulesInputRequestTypeDef",
     "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
     "DescribeSSLPoliciesInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "DescribeTargetGroupAttributesInputRequestTypeDef",
-    "TargetGroupAttributeTypeDef",
+    "TargetGroupAttributeOutputTypeDef",
     "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
     "DescribeTargetGroupsInputRequestTypeDef",
+    "TargetGroupStickinessConfigOutputTypeDef",
+    "TargetGroupTupleOutputTypeDef",
     "TargetGroupStickinessConfigTypeDef",
     "TargetGroupTupleTypeDef",
+    "HostHeaderConditionConfigOutputTypeDef",
     "HostHeaderConditionConfigTypeDef",
+    "HttpHeaderConditionConfigOutputTypeDef",
     "HttpHeaderConditionConfigTypeDef",
+    "HttpRequestMethodConditionConfigOutputTypeDef",
     "HttpRequestMethodConditionConfigTypeDef",
+    "LoadBalancerAttributeTypeDef",
     "LoadBalancerStateTypeDef",
+    "MatcherOutputTypeDef",
+    "TargetGroupAttributeTypeDef",
     "PaginatorConfigTypeDef",
+    "PathPatternConditionConfigOutputTypeDef",
     "PathPatternConditionConfigTypeDef",
+    "QueryStringKeyValuePairOutputTypeDef",
     "QueryStringKeyValuePairTypeDef",
     "RemoveTagsInputRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "SourceIpConditionConfigOutputTypeDef",
     "SourceIpConditionConfigTypeDef",
     "RulePriorityPairTypeDef",
     "SetIpAddressTypeInputRequestTypeDef",
     "SetIpAddressTypeOutputTypeDef",
     "SetSecurityGroupsInputRequestTypeDef",
     "SetSecurityGroupsOutputTypeDef",
+    "TagOutputTypeDef",
+    "TargetDescriptionOutputTypeDef",
     "TargetHealthTypeDef",
     "AddListenerCertificatesInputRequestTypeDef",
+    "RemoveListenerCertificatesInputRequestTypeDef",
     "AddListenerCertificatesOutputTypeDef",
     "DescribeListenerCertificatesOutputTypeDef",
-    "RemoveListenerCertificatesInputRequestTypeDef",
     "AddTagsInputRequestTypeDef",
-    "TagDescriptionTypeDef",
     "AvailabilityZoneTypeDef",
     "SslPolicyTypeDef",
     "CreateLoadBalancerInputRequestTypeDef",
     "SetSubnetsInputRequestTypeDef",
     "CreateTargetGroupInputRequestTypeDef",
     "ModifyTargetGroupInputRequestTypeDef",
-    "TargetGroupTypeDef",
     "DeregisterTargetsInputRequestTypeDef",
     "DescribeTargetHealthInputRequestTypeDef",
     "RegisterTargetsInputRequestTypeDef",
     "DescribeAccountLimitsOutputTypeDef",
     "DescribeLoadBalancerAttributesOutputTypeDef",
-    "ModifyLoadBalancerAttributesInputRequestTypeDef",
     "ModifyLoadBalancerAttributesOutputTypeDef",
     "DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef",
     "DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef",
     "DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef",
     "DescribeTargetHealthInputTargetDeregisteredWaitTypeDef",
     "DescribeTargetHealthInputTargetInServiceWaitTypeDef",
     "DescribeTargetGroupAttributesOutputTypeDef",
-    "ModifyTargetGroupAttributesInputRequestTypeDef",
     "ModifyTargetGroupAttributesOutputTypeDef",
+    "ForwardActionConfigOutputTypeDef",
     "ForwardActionConfigTypeDef",
+    "ModifyLoadBalancerAttributesInputRequestTypeDef",
+    "TargetGroupTypeDef",
+    "ModifyTargetGroupAttributesInputRequestTypeDef",
+    "QueryStringConditionConfigOutputTypeDef",
     "QueryStringConditionConfigTypeDef",
     "SetRulePrioritiesInputRequestTypeDef",
+    "TagDescriptionTypeDef",
     "TargetHealthDescriptionTypeDef",
-    "DescribeTagsOutputTypeDef",
     "LoadBalancerTypeDef",
     "SetSubnetsOutputTypeDef",
     "DescribeSSLPoliciesOutputTypeDef",
+    "ActionOutputTypeDef",
+    "ActionTypeDef",
     "CreateTargetGroupOutputTypeDef",
     "DescribeTargetGroupsOutputTypeDef",
     "ModifyTargetGroupOutputTypeDef",
-    "ActionTypeDef",
+    "RuleConditionOutputTypeDef",
     "RuleConditionTypeDef",
+    "DescribeTagsOutputTypeDef",
     "DescribeTargetHealthOutputTypeDef",
     "CreateLoadBalancerOutputTypeDef",
     "DescribeLoadBalancersOutputTypeDef",
-    "CreateListenerInputRequestTypeDef",
     "ListenerTypeDef",
+    "CreateListenerInputRequestTypeDef",
     "ModifyListenerInputRequestTypeDef",
+    "RuleTypeDef",
     "CreateRuleInputRequestTypeDef",
     "ModifyRuleInputRequestTypeDef",
-    "RuleTypeDef",
     "CreateListenerOutputTypeDef",
     "DescribeListenersOutputTypeDef",
     "ModifyListenerOutputTypeDef",
     "CreateRuleOutputTypeDef",
     "DescribeRulesOutputTypeDef",
     "ModifyRuleOutputTypeDef",
     "SetRulePrioritiesOutputTypeDef",
 )
 
+_RequiredAuthenticateCognitoActionConfigOutputTypeDef = TypedDict(
+    "_RequiredAuthenticateCognitoActionConfigOutputTypeDef",
+    {
+        "UserPoolArn": str,
+        "UserPoolClientId": str,
+        "UserPoolDomain": str,
+    },
+)
+_OptionalAuthenticateCognitoActionConfigOutputTypeDef = TypedDict(
+    "_OptionalAuthenticateCognitoActionConfigOutputTypeDef",
+    {
+        "SessionCookieName": str,
+        "Scope": str,
+        "SessionTimeout": int,
+        "AuthenticationRequestExtraParams": Dict[str, str],
+        "OnUnauthenticatedRequest": AuthenticateCognitoActionConditionalBehaviorEnumType,
+    },
+    total=False,
+)
+
+
+class AuthenticateCognitoActionConfigOutputTypeDef(
+    _RequiredAuthenticateCognitoActionConfigOutputTypeDef,
+    _OptionalAuthenticateCognitoActionConfigOutputTypeDef,
+):
+    pass
+
+
+_RequiredAuthenticateOidcActionConfigOutputTypeDef = TypedDict(
+    "_RequiredAuthenticateOidcActionConfigOutputTypeDef",
+    {
+        "Issuer": str,
+        "AuthorizationEndpoint": str,
+        "TokenEndpoint": str,
+        "UserInfoEndpoint": str,
+        "ClientId": str,
+    },
+)
+_OptionalAuthenticateOidcActionConfigOutputTypeDef = TypedDict(
+    "_OptionalAuthenticateOidcActionConfigOutputTypeDef",
+    {
+        "ClientSecret": str,
+        "SessionCookieName": str,
+        "Scope": str,
+        "SessionTimeout": int,
+        "AuthenticationRequestExtraParams": Dict[str, str],
+        "OnUnauthenticatedRequest": AuthenticateOidcActionConditionalBehaviorEnumType,
+        "UseExistingClientSecret": bool,
+    },
+    total=False,
+)
+
+
+class AuthenticateOidcActionConfigOutputTypeDef(
+    _RequiredAuthenticateOidcActionConfigOutputTypeDef,
+    _OptionalAuthenticateOidcActionConfigOutputTypeDef,
+):
+    pass
+
+
+_RequiredFixedResponseActionConfigOutputTypeDef = TypedDict(
+    "_RequiredFixedResponseActionConfigOutputTypeDef",
+    {
+        "StatusCode": str,
+    },
+)
+_OptionalFixedResponseActionConfigOutputTypeDef = TypedDict(
+    "_OptionalFixedResponseActionConfigOutputTypeDef",
+    {
+        "MessageBody": str,
+        "ContentType": str,
+    },
+    total=False,
+)
+
+
+class FixedResponseActionConfigOutputTypeDef(
+    _RequiredFixedResponseActionConfigOutputTypeDef, _OptionalFixedResponseActionConfigOutputTypeDef
+):
+    pass
+
+
+_RequiredRedirectActionConfigOutputTypeDef = TypedDict(
+    "_RequiredRedirectActionConfigOutputTypeDef",
+    {
+        "StatusCode": RedirectActionStatusCodeEnumType,
+    },
+)
+_OptionalRedirectActionConfigOutputTypeDef = TypedDict(
+    "_OptionalRedirectActionConfigOutputTypeDef",
+    {
+        "Protocol": str,
+        "Port": str,
+        "Host": str,
+        "Path": str,
+        "Query": str,
+    },
+    total=False,
+)
+
+
+class RedirectActionConfigOutputTypeDef(
+    _RequiredRedirectActionConfigOutputTypeDef, _OptionalRedirectActionConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredAuthenticateCognitoActionConfigTypeDef = TypedDict(
     "_RequiredAuthenticateCognitoActionConfigTypeDef",
     {
         "UserPoolArn": str,
         "UserPoolClientId": str,
         "UserPoolDomain": str,
     },
@@ -166,19 +296,21 @@
         "SessionTimeout": int,
         "AuthenticationRequestExtraParams": Mapping[str, str],
         "OnUnauthenticatedRequest": AuthenticateCognitoActionConditionalBehaviorEnumType,
     },
     total=False,
 )
 
+
 class AuthenticateCognitoActionConfigTypeDef(
     _RequiredAuthenticateCognitoActionConfigTypeDef, _OptionalAuthenticateCognitoActionConfigTypeDef
 ):
     pass
 
+
 _RequiredAuthenticateOidcActionConfigTypeDef = TypedDict(
     "_RequiredAuthenticateOidcActionConfigTypeDef",
     {
         "Issuer": str,
         "AuthorizationEndpoint": str,
         "TokenEndpoint": str,
         "UserInfoEndpoint": str,
@@ -195,19 +327,21 @@
         "AuthenticationRequestExtraParams": Mapping[str, str],
         "OnUnauthenticatedRequest": AuthenticateOidcActionConditionalBehaviorEnumType,
         "UseExistingClientSecret": bool,
     },
     total=False,
 )
 
+
 class AuthenticateOidcActionConfigTypeDef(
     _RequiredAuthenticateOidcActionConfigTypeDef, _OptionalAuthenticateOidcActionConfigTypeDef
 ):
     pass
 
+
 _RequiredFixedResponseActionConfigTypeDef = TypedDict(
     "_RequiredFixedResponseActionConfigTypeDef",
     {
         "StatusCode": str,
     },
 )
 _OptionalFixedResponseActionConfigTypeDef = TypedDict(
@@ -215,19 +349,21 @@
     {
         "MessageBody": str,
         "ContentType": str,
     },
     total=False,
 )
 
+
 class FixedResponseActionConfigTypeDef(
     _RequiredFixedResponseActionConfigTypeDef, _OptionalFixedResponseActionConfigTypeDef
 ):
     pass
 
+
 _RequiredRedirectActionConfigTypeDef = TypedDict(
     "_RequiredRedirectActionConfigTypeDef",
     {
         "StatusCode": RedirectActionStatusCodeEnumType,
     },
 )
 _OptionalRedirectActionConfigTypeDef = TypedDict(
@@ -238,45 +374,58 @@
         "Host": str,
         "Path": str,
         "Query": str,
     },
     total=False,
 )
 
+
 class RedirectActionConfigTypeDef(
     _RequiredRedirectActionConfigTypeDef, _OptionalRedirectActionConfigTypeDef
 ):
     pass
 
+
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "CertificateArn": str,
         "IsDefault": bool,
     },
     total=False,
 )
 
+CertificateOutputTypeDef = TypedDict(
+    "CertificateOutputTypeDef",
+    {
+        "CertificateArn": str,
+        "IsDefault": bool,
+    },
+    total=False,
+)
+
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+
 LoadBalancerAddressTypeDef = TypedDict(
     "LoadBalancerAddressTypeDef",
     {
         "IpAddress": str,
         "AllocationId": str,
         "PrivateIPv4Address": str,
         "IPv6Address": str,
@@ -352,19 +501,21 @@
     {
         "Port": int,
         "AvailabilityZone": str,
     },
     total=False,
 )
 
+
 class TargetDescriptionTypeDef(
     _RequiredTargetDescriptionTypeDef, _OptionalTargetDescriptionTypeDef
 ):
     pass
 
+
 DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
     "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -397,20 +548,22 @@
     "_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef(
     _RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
     _OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeListenerCertificatesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeListenerCertificatesInputRequestTypeDef",
     {
         "ListenerArn": str,
     },
 )
 _OptionalDescribeListenerCertificatesInputRequestTypeDef = TypedDict(
@@ -418,20 +571,22 @@
     {
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
+
 class DescribeListenerCertificatesInputRequestTypeDef(
     _RequiredDescribeListenerCertificatesInputRequestTypeDef,
     _OptionalDescribeListenerCertificatesInputRequestTypeDef,
 ):
     pass
 
+
 DescribeListenersInputDescribeListenersPaginateTypeDef = TypedDict(
     "DescribeListenersInputDescribeListenersPaginateTypeDef",
     {
         "LoadBalancerArn": str,
         "ListenerArns": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -452,16 +607,16 @@
 DescribeLoadBalancerAttributesInputRequestTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
     },
 )
 
-LoadBalancerAttributeTypeDef = TypedDict(
-    "LoadBalancerAttributeTypeDef",
+LoadBalancerAttributeOutputTypeDef = TypedDict(
+    "LoadBalancerAttributeOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
@@ -547,16 +702,16 @@
 DescribeTargetGroupAttributesInputRequestTypeDef = TypedDict(
     "DescribeTargetGroupAttributesInputRequestTypeDef",
     {
         "TargetGroupArn": str,
     },
 )
 
-TargetGroupAttributeTypeDef = TypedDict(
-    "TargetGroupAttributeTypeDef",
+TargetGroupAttributeOutputTypeDef = TypedDict(
+    "TargetGroupAttributeOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
@@ -579,14 +734,32 @@
         "Names": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
+TargetGroupStickinessConfigOutputTypeDef = TypedDict(
+    "TargetGroupStickinessConfigOutputTypeDef",
+    {
+        "Enabled": bool,
+        "DurationSeconds": int,
+    },
+    total=False,
+)
+
+TargetGroupTupleOutputTypeDef = TypedDict(
+    "TargetGroupTupleOutputTypeDef",
+    {
+        "TargetGroupArn": str,
+        "Weight": int,
+    },
+    total=False,
+)
+
 TargetGroupStickinessConfigTypeDef = TypedDict(
     "TargetGroupStickinessConfigTypeDef",
     {
         "Enabled": bool,
         "DurationSeconds": int,
     },
     total=False,
@@ -597,66 +770,135 @@
     {
         "TargetGroupArn": str,
         "Weight": int,
     },
     total=False,
 )
 
+HostHeaderConditionConfigOutputTypeDef = TypedDict(
+    "HostHeaderConditionConfigOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+    total=False,
+)
+
 HostHeaderConditionConfigTypeDef = TypedDict(
     "HostHeaderConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
 
+HttpHeaderConditionConfigOutputTypeDef = TypedDict(
+    "HttpHeaderConditionConfigOutputTypeDef",
+    {
+        "HttpHeaderName": str,
+        "Values": List[str],
+    },
+    total=False,
+)
+
 HttpHeaderConditionConfigTypeDef = TypedDict(
     "HttpHeaderConditionConfigTypeDef",
     {
         "HttpHeaderName": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
+HttpRequestMethodConditionConfigOutputTypeDef = TypedDict(
+    "HttpRequestMethodConditionConfigOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+    total=False,
+)
+
 HttpRequestMethodConditionConfigTypeDef = TypedDict(
     "HttpRequestMethodConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
 
+LoadBalancerAttributeTypeDef = TypedDict(
+    "LoadBalancerAttributeTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 LoadBalancerStateTypeDef = TypedDict(
     "LoadBalancerStateTypeDef",
     {
         "Code": LoadBalancerStateEnumType,
         "Reason": str,
     },
     total=False,
 )
 
+MatcherOutputTypeDef = TypedDict(
+    "MatcherOutputTypeDef",
+    {
+        "HttpCode": str,
+        "GrpcCode": str,
+    },
+    total=False,
+)
+
+TargetGroupAttributeTypeDef = TypedDict(
+    "TargetGroupAttributeTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+PathPatternConditionConfigOutputTypeDef = TypedDict(
+    "PathPatternConditionConfigOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+    total=False,
+)
+
 PathPatternConditionConfigTypeDef = TypedDict(
     "PathPatternConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
 
+QueryStringKeyValuePairOutputTypeDef = TypedDict(
+    "QueryStringKeyValuePairOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 QueryStringKeyValuePairTypeDef = TypedDict(
     "QueryStringKeyValuePairTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -677,14 +919,22 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+SourceIpConditionConfigOutputTypeDef = TypedDict(
+    "SourceIpConditionConfigOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+    total=False,
+)
+
 SourceIpConditionConfigTypeDef = TypedDict(
     "SourceIpConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
@@ -726,14 +976,55 @@
     "SetSecurityGroupsOutputTypeDef",
     {
         "SecurityGroupIds": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
+    pass
+
+
+_RequiredTargetDescriptionOutputTypeDef = TypedDict(
+    "_RequiredTargetDescriptionOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalTargetDescriptionOutputTypeDef = TypedDict(
+    "_OptionalTargetDescriptionOutputTypeDef",
+    {
+        "Port": int,
+        "AvailabilityZone": str,
+    },
+    total=False,
+)
+
+
+class TargetDescriptionOutputTypeDef(
+    _RequiredTargetDescriptionOutputTypeDef, _OptionalTargetDescriptionOutputTypeDef
+):
+    pass
+
+
 TargetHealthTypeDef = TypedDict(
     "TargetHealthTypeDef",
     {
         "State": TargetHealthStateEnumType,
         "Reason": TargetHealthReasonEnumType,
         "Description": str,
     },
@@ -744,56 +1035,47 @@
     "AddListenerCertificatesInputRequestTypeDef",
     {
         "ListenerArn": str,
         "Certificates": Sequence[CertificateTypeDef],
     },
 )
 
+RemoveListenerCertificatesInputRequestTypeDef = TypedDict(
+    "RemoveListenerCertificatesInputRequestTypeDef",
+    {
+        "ListenerArn": str,
+        "Certificates": Sequence[CertificateTypeDef],
+    },
+)
+
 AddListenerCertificatesOutputTypeDef = TypedDict(
     "AddListenerCertificatesOutputTypeDef",
     {
-        "Certificates": List[CertificateTypeDef],
+        "Certificates": List[CertificateOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeListenerCertificatesOutputTypeDef = TypedDict(
     "DescribeListenerCertificatesOutputTypeDef",
     {
-        "Certificates": List[CertificateTypeDef],
+        "Certificates": List[CertificateOutputTypeDef],
         "NextMarker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RemoveListenerCertificatesInputRequestTypeDef = TypedDict(
-    "RemoveListenerCertificatesInputRequestTypeDef",
-    {
-        "ListenerArn": str,
-        "Certificates": Sequence[CertificateTypeDef],
-    },
-)
-
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "ResourceArns": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-TagDescriptionTypeDef = TypedDict(
-    "TagDescriptionTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "ZoneName": str,
         "SubnetId": str,
         "OutpostId": str,
         "LoadBalancerAddresses": List[LoadBalancerAddressTypeDef],
@@ -829,19 +1111,21 @@
         "Type": LoadBalancerTypeEnumType,
         "IpAddressType": IpAddressTypeType,
         "CustomerOwnedIpv4Pool": str,
     },
     total=False,
 )
 
+
 class CreateLoadBalancerInputRequestTypeDef(
     _RequiredCreateLoadBalancerInputRequestTypeDef, _OptionalCreateLoadBalancerInputRequestTypeDef
 ):
     pass
 
+
 _RequiredSetSubnetsInputRequestTypeDef = TypedDict(
     "_RequiredSetSubnetsInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
     },
 )
 _OptionalSetSubnetsInputRequestTypeDef = TypedDict(
@@ -850,19 +1134,21 @@
         "Subnets": Sequence[str],
         "SubnetMappings": Sequence[SubnetMappingTypeDef],
         "IpAddressType": IpAddressTypeType,
     },
     total=False,
 )
 
+
 class SetSubnetsInputRequestTypeDef(
     _RequiredSetSubnetsInputRequestTypeDef, _OptionalSetSubnetsInputRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateTargetGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateTargetGroupInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateTargetGroupInputRequestTypeDef = TypedDict(
@@ -884,19 +1170,21 @@
         "TargetType": TargetTypeEnumType,
         "Tags": Sequence[TagTypeDef],
         "IpAddressType": TargetGroupIpAddressTypeEnumType,
     },
     total=False,
 )
 
+
 class CreateTargetGroupInputRequestTypeDef(
     _RequiredCreateTargetGroupInputRequestTypeDef, _OptionalCreateTargetGroupInputRequestTypeDef
 ):
     pass
 
+
 _RequiredModifyTargetGroupInputRequestTypeDef = TypedDict(
     "_RequiredModifyTargetGroupInputRequestTypeDef",
     {
         "TargetGroupArn": str,
     },
 )
 _OptionalModifyTargetGroupInputRequestTypeDef = TypedDict(
@@ -911,43 +1199,20 @@
         "HealthyThresholdCount": int,
         "UnhealthyThresholdCount": int,
         "Matcher": MatcherTypeDef,
     },
     total=False,
 )
 
+
 class ModifyTargetGroupInputRequestTypeDef(
     _RequiredModifyTargetGroupInputRequestTypeDef, _OptionalModifyTargetGroupInputRequestTypeDef
 ):
     pass
 
-TargetGroupTypeDef = TypedDict(
-    "TargetGroupTypeDef",
-    {
-        "TargetGroupArn": str,
-        "TargetGroupName": str,
-        "Protocol": ProtocolEnumType,
-        "Port": int,
-        "VpcId": str,
-        "HealthCheckProtocol": ProtocolEnumType,
-        "HealthCheckPort": str,
-        "HealthCheckEnabled": bool,
-        "HealthCheckIntervalSeconds": int,
-        "HealthCheckTimeoutSeconds": int,
-        "HealthyThresholdCount": int,
-        "UnhealthyThresholdCount": int,
-        "HealthCheckPath": str,
-        "Matcher": MatcherTypeDef,
-        "LoadBalancerArns": List[str],
-        "TargetType": TargetTypeEnumType,
-        "ProtocolVersion": str,
-        "IpAddressType": TargetGroupIpAddressTypeEnumType,
-    },
-    total=False,
-)
 
 DeregisterTargetsInputRequestTypeDef = TypedDict(
     "DeregisterTargetsInputRequestTypeDef",
     {
         "TargetGroupArn": str,
         "Targets": Sequence[TargetDescriptionTypeDef],
     },
@@ -963,20 +1228,22 @@
     "_OptionalDescribeTargetHealthInputRequestTypeDef",
     {
         "Targets": Sequence[TargetDescriptionTypeDef],
     },
     total=False,
 )
 
+
 class DescribeTargetHealthInputRequestTypeDef(
     _RequiredDescribeTargetHealthInputRequestTypeDef,
     _OptionalDescribeTargetHealthInputRequestTypeDef,
 ):
     pass
 
+
 RegisterTargetsInputRequestTypeDef = TypedDict(
     "RegisterTargetsInputRequestTypeDef",
     {
         "TargetGroupArn": str,
         "Targets": Sequence[TargetDescriptionTypeDef],
     },
 )
@@ -989,31 +1256,23 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLoadBalancerAttributesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesOutputTypeDef",
     {
-        "Attributes": List[LoadBalancerAttributeTypeDef],
+        "Attributes": List[LoadBalancerAttributeOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
-    "ModifyLoadBalancerAttributesInputRequestTypeDef",
-    {
-        "LoadBalancerArn": str,
-        "Attributes": Sequence[LoadBalancerAttributeTypeDef],
-    },
-)
-
 ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
     "ModifyLoadBalancerAttributesOutputTypeDef",
     {
-        "Attributes": List[LoadBalancerAttributeTypeDef],
+        "Attributes": List[LoadBalancerAttributeOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef = TypedDict(
     "DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef",
     {
@@ -1061,20 +1320,22 @@
     {
         "Targets": Sequence[TargetDescriptionTypeDef],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeTargetHealthInputTargetDeregisteredWaitTypeDef(
     _RequiredDescribeTargetHealthInputTargetDeregisteredWaitTypeDef,
     _OptionalDescribeTargetHealthInputTargetDeregisteredWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeTargetHealthInputTargetInServiceWaitTypeDef = TypedDict(
     "_RequiredDescribeTargetHealthInputTargetInServiceWaitTypeDef",
     {
         "TargetGroupArn": str,
     },
 )
 _OptionalDescribeTargetHealthInputTargetInServiceWaitTypeDef = TypedDict(
@@ -1082,53 +1343,105 @@
     {
         "Targets": Sequence[TargetDescriptionTypeDef],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeTargetHealthInputTargetInServiceWaitTypeDef(
     _RequiredDescribeTargetHealthInputTargetInServiceWaitTypeDef,
     _OptionalDescribeTargetHealthInputTargetInServiceWaitTypeDef,
 ):
     pass
 
+
 DescribeTargetGroupAttributesOutputTypeDef = TypedDict(
     "DescribeTargetGroupAttributesOutputTypeDef",
     {
-        "Attributes": List[TargetGroupAttributeTypeDef],
+        "Attributes": List[TargetGroupAttributeOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyTargetGroupAttributesInputRequestTypeDef = TypedDict(
-    "ModifyTargetGroupAttributesInputRequestTypeDef",
+ModifyTargetGroupAttributesOutputTypeDef = TypedDict(
+    "ModifyTargetGroupAttributesOutputTypeDef",
     {
-        "TargetGroupArn": str,
-        "Attributes": Sequence[TargetGroupAttributeTypeDef],
+        "Attributes": List[TargetGroupAttributeOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyTargetGroupAttributesOutputTypeDef = TypedDict(
-    "ModifyTargetGroupAttributesOutputTypeDef",
+ForwardActionConfigOutputTypeDef = TypedDict(
+    "ForwardActionConfigOutputTypeDef",
     {
-        "Attributes": List[TargetGroupAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TargetGroups": List[TargetGroupTupleOutputTypeDef],
+        "TargetGroupStickinessConfig": TargetGroupStickinessConfigOutputTypeDef,
     },
+    total=False,
 )
 
 ForwardActionConfigTypeDef = TypedDict(
     "ForwardActionConfigTypeDef",
     {
         "TargetGroups": Sequence[TargetGroupTupleTypeDef],
         "TargetGroupStickinessConfig": TargetGroupStickinessConfigTypeDef,
     },
     total=False,
 )
 
+ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
+    "ModifyLoadBalancerAttributesInputRequestTypeDef",
+    {
+        "LoadBalancerArn": str,
+        "Attributes": Sequence[LoadBalancerAttributeTypeDef],
+    },
+)
+
+TargetGroupTypeDef = TypedDict(
+    "TargetGroupTypeDef",
+    {
+        "TargetGroupArn": str,
+        "TargetGroupName": str,
+        "Protocol": ProtocolEnumType,
+        "Port": int,
+        "VpcId": str,
+        "HealthCheckProtocol": ProtocolEnumType,
+        "HealthCheckPort": str,
+        "HealthCheckEnabled": bool,
+        "HealthCheckIntervalSeconds": int,
+        "HealthCheckTimeoutSeconds": int,
+        "HealthyThresholdCount": int,
+        "UnhealthyThresholdCount": int,
+        "HealthCheckPath": str,
+        "Matcher": MatcherOutputTypeDef,
+        "LoadBalancerArns": List[str],
+        "TargetType": TargetTypeEnumType,
+        "ProtocolVersion": str,
+        "IpAddressType": TargetGroupIpAddressTypeEnumType,
+    },
+    total=False,
+)
+
+ModifyTargetGroupAttributesInputRequestTypeDef = TypedDict(
+    "ModifyTargetGroupAttributesInputRequestTypeDef",
+    {
+        "TargetGroupArn": str,
+        "Attributes": Sequence[TargetGroupAttributeTypeDef],
+    },
+)
+
+QueryStringConditionConfigOutputTypeDef = TypedDict(
+    "QueryStringConditionConfigOutputTypeDef",
+    {
+        "Values": List[QueryStringKeyValuePairOutputTypeDef],
+    },
+    total=False,
+)
+
 QueryStringConditionConfigTypeDef = TypedDict(
     "QueryStringConditionConfigTypeDef",
     {
         "Values": Sequence[QueryStringKeyValuePairTypeDef],
     },
     total=False,
 )
@@ -1136,30 +1449,31 @@
 SetRulePrioritiesInputRequestTypeDef = TypedDict(
     "SetRulePrioritiesInputRequestTypeDef",
     {
         "RulePriorities": Sequence[RulePriorityPairTypeDef],
     },
 )
 
-TargetHealthDescriptionTypeDef = TypedDict(
-    "TargetHealthDescriptionTypeDef",
+TagDescriptionTypeDef = TypedDict(
+    "TagDescriptionTypeDef",
     {
-        "Target": TargetDescriptionTypeDef,
-        "HealthCheckPort": str,
-        "TargetHealth": TargetHealthTypeDef,
+        "ResourceArn": str,
+        "Tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
-DescribeTagsOutputTypeDef = TypedDict(
-    "DescribeTagsOutputTypeDef",
+TargetHealthDescriptionTypeDef = TypedDict(
+    "TargetHealthDescriptionTypeDef",
     {
-        "TagDescriptions": List[TagDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Target": TargetDescriptionOutputTypeDef,
+        "HealthCheckPort": str,
+        "TargetHealth": TargetHealthTypeDef,
     },
+    total=False,
 )
 
 LoadBalancerTypeDef = TypedDict(
     "LoadBalancerTypeDef",
     {
         "LoadBalancerArn": str,
         "DNSName": str,
@@ -1192,38 +1506,38 @@
     {
         "SslPolicies": List[SslPolicyTypeDef],
         "NextMarker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateTargetGroupOutputTypeDef = TypedDict(
-    "CreateTargetGroupOutputTypeDef",
+_RequiredActionOutputTypeDef = TypedDict(
+    "_RequiredActionOutputTypeDef",
     {
-        "TargetGroups": List[TargetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Type": ActionTypeEnumType,
     },
 )
-
-DescribeTargetGroupsOutputTypeDef = TypedDict(
-    "DescribeTargetGroupsOutputTypeDef",
+_OptionalActionOutputTypeDef = TypedDict(
+    "_OptionalActionOutputTypeDef",
     {
-        "TargetGroups": List[TargetGroupTypeDef],
-        "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TargetGroupArn": str,
+        "AuthenticateOidcConfig": AuthenticateOidcActionConfigOutputTypeDef,
+        "AuthenticateCognitoConfig": AuthenticateCognitoActionConfigOutputTypeDef,
+        "Order": int,
+        "RedirectConfig": RedirectActionConfigOutputTypeDef,
+        "FixedResponseConfig": FixedResponseActionConfigOutputTypeDef,
+        "ForwardConfig": ForwardActionConfigOutputTypeDef,
     },
+    total=False,
 )
 
-ModifyTargetGroupOutputTypeDef = TypedDict(
-    "ModifyTargetGroupOutputTypeDef",
-    {
-        "TargetGroups": List[TargetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+
+class ActionOutputTypeDef(_RequiredActionOutputTypeDef, _OptionalActionOutputTypeDef):
+    pass
+
 
 _RequiredActionTypeDef = TypedDict(
     "_RequiredActionTypeDef",
     {
         "Type": ActionTypeEnumType,
     },
 )
@@ -1237,17 +1551,59 @@
         "RedirectConfig": RedirectActionConfigTypeDef,
         "FixedResponseConfig": FixedResponseActionConfigTypeDef,
         "ForwardConfig": ForwardActionConfigTypeDef,
     },
     total=False,
 )
 
+
 class ActionTypeDef(_RequiredActionTypeDef, _OptionalActionTypeDef):
     pass
 
+
+CreateTargetGroupOutputTypeDef = TypedDict(
+    "CreateTargetGroupOutputTypeDef",
+    {
+        "TargetGroups": List[TargetGroupTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeTargetGroupsOutputTypeDef = TypedDict(
+    "DescribeTargetGroupsOutputTypeDef",
+    {
+        "TargetGroups": List[TargetGroupTypeDef],
+        "NextMarker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ModifyTargetGroupOutputTypeDef = TypedDict(
+    "ModifyTargetGroupOutputTypeDef",
+    {
+        "TargetGroups": List[TargetGroupTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RuleConditionOutputTypeDef = TypedDict(
+    "RuleConditionOutputTypeDef",
+    {
+        "Field": str,
+        "Values": List[str],
+        "HostHeaderConfig": HostHeaderConditionConfigOutputTypeDef,
+        "PathPatternConfig": PathPatternConditionConfigOutputTypeDef,
+        "HttpHeaderConfig": HttpHeaderConditionConfigOutputTypeDef,
+        "QueryStringConfig": QueryStringConditionConfigOutputTypeDef,
+        "HttpRequestMethodConfig": HttpRequestMethodConditionConfigOutputTypeDef,
+        "SourceIpConfig": SourceIpConditionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 RuleConditionTypeDef = TypedDict(
     "RuleConditionTypeDef",
     {
         "Field": str,
         "Values": Sequence[str],
         "HostHeaderConfig": HostHeaderConditionConfigTypeDef,
         "PathPatternConfig": PathPatternConditionConfigTypeDef,
@@ -1255,14 +1611,22 @@
         "QueryStringConfig": QueryStringConditionConfigTypeDef,
         "HttpRequestMethodConfig": HttpRequestMethodConditionConfigTypeDef,
         "SourceIpConfig": SourceIpConditionConfigTypeDef,
     },
     total=False,
 )
 
+DescribeTagsOutputTypeDef = TypedDict(
+    "DescribeTagsOutputTypeDef",
+    {
+        "TagDescriptions": List[TagDescriptionTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeTargetHealthOutputTypeDef = TypedDict(
     "DescribeTargetHealthOutputTypeDef",
     {
         "TargetHealthDescriptions": List[TargetHealthDescriptionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1280,14 +1644,29 @@
     {
         "LoadBalancers": List[LoadBalancerTypeDef],
         "NextMarker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListenerTypeDef = TypedDict(
+    "ListenerTypeDef",
+    {
+        "ListenerArn": str,
+        "LoadBalancerArn": str,
+        "Port": int,
+        "Protocol": ProtocolEnumType,
+        "Certificates": List[CertificateOutputTypeDef],
+        "SslPolicy": str,
+        "DefaultActions": List[ActionOutputTypeDef],
+        "AlpnPolicy": List[str],
+    },
+    total=False,
+)
+
 _RequiredCreateListenerInputRequestTypeDef = TypedDict(
     "_RequiredCreateListenerInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "DefaultActions": Sequence[ActionTypeDef],
     },
 )
@@ -1300,33 +1679,20 @@
         "Certificates": Sequence[CertificateTypeDef],
         "AlpnPolicy": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateListenerInputRequestTypeDef(
     _RequiredCreateListenerInputRequestTypeDef, _OptionalCreateListenerInputRequestTypeDef
 ):
     pass
 
-ListenerTypeDef = TypedDict(
-    "ListenerTypeDef",
-    {
-        "ListenerArn": str,
-        "LoadBalancerArn": str,
-        "Port": int,
-        "Protocol": ProtocolEnumType,
-        "Certificates": List[CertificateTypeDef],
-        "SslPolicy": str,
-        "DefaultActions": List[ActionTypeDef],
-        "AlpnPolicy": List[str],
-    },
-    total=False,
-)
 
 _RequiredModifyListenerInputRequestTypeDef = TypedDict(
     "_RequiredModifyListenerInputRequestTypeDef",
     {
         "ListenerArn": str,
     },
 )
@@ -1339,19 +1705,33 @@
         "Certificates": Sequence[CertificateTypeDef],
         "DefaultActions": Sequence[ActionTypeDef],
         "AlpnPolicy": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyListenerInputRequestTypeDef(
     _RequiredModifyListenerInputRequestTypeDef, _OptionalModifyListenerInputRequestTypeDef
 ):
     pass
 
+
+RuleTypeDef = TypedDict(
+    "RuleTypeDef",
+    {
+        "RuleArn": str,
+        "Priority": str,
+        "Conditions": List[RuleConditionOutputTypeDef],
+        "Actions": List[ActionOutputTypeDef],
+        "IsDefault": bool,
+    },
+    total=False,
+)
+
 _RequiredCreateRuleInputRequestTypeDef = TypedDict(
     "_RequiredCreateRuleInputRequestTypeDef",
     {
         "ListenerArn": str,
         "Conditions": Sequence[RuleConditionTypeDef],
         "Priority": int,
         "Actions": Sequence[ActionTypeDef],
@@ -1361,19 +1741,21 @@
     "_OptionalCreateRuleInputRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateRuleInputRequestTypeDef(
     _RequiredCreateRuleInputRequestTypeDef, _OptionalCreateRuleInputRequestTypeDef
 ):
     pass
 
+
 _RequiredModifyRuleInputRequestTypeDef = TypedDict(
     "_RequiredModifyRuleInputRequestTypeDef",
     {
         "RuleArn": str,
     },
 )
 _OptionalModifyRuleInputRequestTypeDef = TypedDict(
@@ -1381,30 +1763,20 @@
     {
         "Conditions": Sequence[RuleConditionTypeDef],
         "Actions": Sequence[ActionTypeDef],
     },
     total=False,
 )
 
+
 class ModifyRuleInputRequestTypeDef(
     _RequiredModifyRuleInputRequestTypeDef, _OptionalModifyRuleInputRequestTypeDef
 ):
     pass
 
-RuleTypeDef = TypedDict(
-    "RuleTypeDef",
-    {
-        "RuleArn": str,
-        "Priority": str,
-        "Conditions": List[RuleConditionTypeDef],
-        "Actions": List[ActionTypeDef],
-        "IsDefault": bool,
-    },
-    total=False,
-)
 
 CreateListenerOutputTypeDef = TypedDict(
     "CreateListenerOutputTypeDef",
     {
         "Listeners": List[ListenerTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/waiter.py` & `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2/waiter.pyi` & `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2.egg-info/PKG-INFO` & `mypy-boto3-elbv2-1.28.12/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-elbv2
-Version: 1.28.0
-Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 elbv2 type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-elbv2"></a>
 
 # mypy-boto3-elbv2
 
 [![PyPI - mypy-boto3-elbv2](https://img.shields.io/pypi/v/mypy-boto3-elbv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-elbv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elbv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-elbv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elbv2?color=blue)](https://pypistats.org/packages/mypy-boto3-elbv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elbv2)](https://pepy.tech/project/mypy-boto3-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancingv2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
+[boto3.ElasticLoadBalancingv2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
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
 [mypy-boto3-elbv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -404,19 +372,24 @@
 ### Typed dictionaries
 
 `mypy_boto3_elbv2.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elbv2.type_defs import (
+    AuthenticateCognitoActionConfigOutputTypeDef,
+    AuthenticateOidcActionConfigOutputTypeDef,
+    FixedResponseActionConfigOutputTypeDef,
+    RedirectActionConfigOutputTypeDef,
     AuthenticateCognitoActionConfigTypeDef,
     AuthenticateOidcActionConfigTypeDef,
     FixedResponseActionConfigTypeDef,
     RedirectActionConfigTypeDef,
     CertificateTypeDef,
+    CertificateOutputTypeDef,
     TagTypeDef,
     LoadBalancerAddressTypeDef,
     CipherTypeDef,
     SubnetMappingTypeDef,
     MatcherTypeDef,
     DeleteListenerInputRequestTypeDef,
     DeleteLoadBalancerInputRequestTypeDef,
@@ -427,106 +400,123 @@
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
     DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
     DescribeListenerCertificatesInputRequestTypeDef,
     DescribeListenersInputDescribeListenersPaginateTypeDef,
     DescribeListenersInputRequestTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
-    LoadBalancerAttributeTypeDef,
+    LoadBalancerAttributeOutputTypeDef,
     DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeLoadBalancersInputRequestTypeDef,
     DescribeRulesInputDescribeRulesPaginateTypeDef,
     DescribeRulesInputRequestTypeDef,
     DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef,
     DescribeSSLPoliciesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DescribeTargetGroupAttributesInputRequestTypeDef,
-    TargetGroupAttributeTypeDef,
+    TargetGroupAttributeOutputTypeDef,
     DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef,
     DescribeTargetGroupsInputRequestTypeDef,
+    TargetGroupStickinessConfigOutputTypeDef,
+    TargetGroupTupleOutputTypeDef,
     TargetGroupStickinessConfigTypeDef,
     TargetGroupTupleTypeDef,
+    HostHeaderConditionConfigOutputTypeDef,
     HostHeaderConditionConfigTypeDef,
+    HttpHeaderConditionConfigOutputTypeDef,
     HttpHeaderConditionConfigTypeDef,
+    HttpRequestMethodConditionConfigOutputTypeDef,
     HttpRequestMethodConditionConfigTypeDef,
+    LoadBalancerAttributeTypeDef,
     LoadBalancerStateTypeDef,
+    MatcherOutputTypeDef,
+    TargetGroupAttributeTypeDef,
     PaginatorConfigTypeDef,
+    PathPatternConditionConfigOutputTypeDef,
     PathPatternConditionConfigTypeDef,
+    QueryStringKeyValuePairOutputTypeDef,
     QueryStringKeyValuePairTypeDef,
     RemoveTagsInputRequestTypeDef,
     ResponseMetadataTypeDef,
+    SourceIpConditionConfigOutputTypeDef,
     SourceIpConditionConfigTypeDef,
     RulePriorityPairTypeDef,
     SetIpAddressTypeInputRequestTypeDef,
     SetIpAddressTypeOutputTypeDef,
     SetSecurityGroupsInputRequestTypeDef,
     SetSecurityGroupsOutputTypeDef,
+    TagOutputTypeDef,
+    TargetDescriptionOutputTypeDef,
     TargetHealthTypeDef,
     AddListenerCertificatesInputRequestTypeDef,
+    RemoveListenerCertificatesInputRequestTypeDef,
     AddListenerCertificatesOutputTypeDef,
     DescribeListenerCertificatesOutputTypeDef,
-    RemoveListenerCertificatesInputRequestTypeDef,
     AddTagsInputRequestTypeDef,
-    TagDescriptionTypeDef,
     AvailabilityZoneTypeDef,
     SslPolicyTypeDef,
     CreateLoadBalancerInputRequestTypeDef,
     SetSubnetsInputRequestTypeDef,
     CreateTargetGroupInputRequestTypeDef,
     ModifyTargetGroupInputRequestTypeDef,
-    TargetGroupTypeDef,
     DeregisterTargetsInputRequestTypeDef,
     DescribeTargetHealthInputRequestTypeDef,
     RegisterTargetsInputRequestTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeLoadBalancerAttributesOutputTypeDef,
-    ModifyLoadBalancerAttributesInputRequestTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef,
     DescribeTargetHealthInputTargetDeregisteredWaitTypeDef,
     DescribeTargetHealthInputTargetInServiceWaitTypeDef,
     DescribeTargetGroupAttributesOutputTypeDef,
-    ModifyTargetGroupAttributesInputRequestTypeDef,
     ModifyTargetGroupAttributesOutputTypeDef,
+    ForwardActionConfigOutputTypeDef,
     ForwardActionConfigTypeDef,
+    ModifyLoadBalancerAttributesInputRequestTypeDef,
+    TargetGroupTypeDef,
+    ModifyTargetGroupAttributesInputRequestTypeDef,
+    QueryStringConditionConfigOutputTypeDef,
     QueryStringConditionConfigTypeDef,
     SetRulePrioritiesInputRequestTypeDef,
+    TagDescriptionTypeDef,
     TargetHealthDescriptionTypeDef,
-    DescribeTagsOutputTypeDef,
     LoadBalancerTypeDef,
     SetSubnetsOutputTypeDef,
     DescribeSSLPoliciesOutputTypeDef,
+    ActionOutputTypeDef,
+    ActionTypeDef,
     CreateTargetGroupOutputTypeDef,
     DescribeTargetGroupsOutputTypeDef,
     ModifyTargetGroupOutputTypeDef,
-    ActionTypeDef,
+    RuleConditionOutputTypeDef,
     RuleConditionTypeDef,
+    DescribeTagsOutputTypeDef,
     DescribeTargetHealthOutputTypeDef,
     CreateLoadBalancerOutputTypeDef,
     DescribeLoadBalancersOutputTypeDef,
-    CreateListenerInputRequestTypeDef,
     ListenerTypeDef,
+    CreateListenerInputRequestTypeDef,
     ModifyListenerInputRequestTypeDef,
+    RuleTypeDef,
     CreateRuleInputRequestTypeDef,
     ModifyRuleInputRequestTypeDef,
-    RuleTypeDef,
     CreateListenerOutputTypeDef,
     DescribeListenersOutputTypeDef,
     ModifyListenerOutputTypeDef,
     CreateRuleOutputTypeDef,
     DescribeRulesOutputTypeDef,
     ModifyRuleOutputTypeDef,
     SetRulePrioritiesOutputTypeDef,
 )
 
 
-def get_structure() -> AuthenticateCognitoActionConfigTypeDef:
+def get_structure() -> AuthenticateCognitoActionConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elbv2-1.28.0/mypy_boto3_elbv2.egg-info/SOURCES.txt` & `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.0/setup.py` & `mypy-boto3-elbv2-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elbv2",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_elbv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElasticLoadBalancingv2 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ElasticLoadBalancingv2 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

