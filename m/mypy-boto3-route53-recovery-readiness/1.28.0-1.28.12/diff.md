# Comparing `tmp/mypy-boto3-route53-recovery-readiness-1.28.0.tar.gz` & `tmp/mypy-boto3-route53-recovery-readiness-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53-recovery-readiness-1.28.0.tar", last modified: Thu Jul  6 21:00:29 2023, max compression
+gzip compressed data, was "mypy-boto3-route53-recovery-readiness-1.28.12.tar", last modified: Thu Jul 27 11:49:32 2023, max compression
```

## Comparing `mypy-boto3-route53-recovery-readiness-1.28.0.tar` & `mypy-boto3-route53-recovery-readiness-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:29.094414 mypy-boto3-route53-recovery-readiness-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:53:38.000000 mypy-boto3-route53-recovery-readiness-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19034 2023-07-06 21:00:29.094414 mypy-boto3-route53-recovery-readiness-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17475 2023-07-06 20:53:38.000000 mypy-boto3-route53-recovery-readiness-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:29.074414 mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-06 20:53:38.000000 mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-06 20:53:38.000000 mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-06 20:53:38.000000 mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-07-06 20:53:38.000000 mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28483 2023-07-06 20:53:38.000000 mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-07-06 20:53:39.000000 mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-07-06 20:53:38.000000 mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-07-06 20:53:38.000000 mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13228 2023-07-06 20:53:38.000000 mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:53:38.000000 mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29827 2023-07-06 20:53:39.000000 mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29790 2023-07-06 20:53:39.000000 mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:53:38.000000 mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:29.094414 mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19034 2023-07-06 21:00:28.000000 mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-06 21:00:28.000000 mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:28.000000 mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:28.000000 mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:28.000000 mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:28.000000 mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:29.094414 mypy-boto3-route53-recovery-readiness-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-06 20:53:38.000000 mypy-boto3-route53-recovery-readiness-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:32.973238 mypy-boto3-route53-recovery-readiness-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19183 2023-07-27 11:49:32.973238 mypy-boto3-route53-recovery-readiness-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17622 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:32.973238 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28483 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    30991 2023-07-27 11:44:53.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30954 2023-07-27 11:44:52.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:32.973238 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19183 2023-07-27 11:49:32.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-27 11:49:32.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:32.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:32.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:32.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:32.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:32.973238 mypy-boto3-route53-recovery-readiness-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/setup.py
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.0/LICENSE` & `mypy-boto3-route53-recovery-readiness-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.0/PKG-INFO` & `mypy-boto3-route53-recovery-readiness-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53-recovery-readiness
-Version: 1.28.0
-Summary: Type annotations for boto3.Route53RecoveryReadiness 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Route53RecoveryReadiness 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-route53-recovery-readiness"></a>
 
 # mypy-boto3-route53-recovery-readiness
 
 [![PyPI - mypy-boto3-route53-recovery-readiness](https://img.shields.io/pypi/v/mypy-boto3-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-readiness)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-readiness)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53-recovery-readiness?color=blue)](https://pypistats.org/packages/mypy-boto3-route53-recovery-readiness)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53-recovery-readiness)](https://pepy.tech/project/mypy-boto3-route53-recovery-readiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryReadiness 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
+[boto3.Route53RecoveryReadiness 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
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
 [mypy-boto3-route53-recovery-readiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/).
 
 See how it helps to find and fix potential bugs:
 
@@ -365,96 +365,101 @@
 `mypy_boto3_route53_recovery_readiness.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53_recovery_readiness.type_defs import (
     CellOutputTypeDef,
     CreateCellRequestRequestTypeDef,
-    CreateCellResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateCrossAccountAuthorizationRequestRequestTypeDef,
-    CreateCrossAccountAuthorizationResponseTypeDef,
     CreateReadinessCheckRequestRequestTypeDef,
-    CreateReadinessCheckResponseTypeDef,
     CreateRecoveryGroupRequestRequestTypeDef,
-    CreateRecoveryGroupResponseTypeDef,
     DeleteCellRequestRequestTypeDef,
     DeleteCrossAccountAuthorizationRequestRequestTypeDef,
     DeleteReadinessCheckRequestRequestTypeDef,
     DeleteRecoveryGroupRequestRequestTypeDef,
     DeleteResourceSetRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetArchitectureRecommendationsRequestRequestTypeDef,
     RecommendationTypeDef,
-    GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetCellReadinessSummaryRequestRequestTypeDef,
     ReadinessCheckSummaryTypeDef,
     GetCellRequestRequestTypeDef,
-    GetCellResponseTypeDef,
     GetReadinessCheckRequestRequestTypeDef,
-    GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
     GetReadinessCheckResourceStatusRequestRequestTypeDef,
-    GetReadinessCheckResponseTypeDef,
-    GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
     GetReadinessCheckStatusRequestRequestTypeDef,
     MessageTypeDef,
     ResourceResultTypeDef,
-    GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
     GetRecoveryGroupReadinessSummaryRequestRequestTypeDef,
     GetRecoveryGroupRequestRequestTypeDef,
-    GetRecoveryGroupResponseTypeDef,
     GetResourceSetRequestRequestTypeDef,
-    ListCellsRequestListCellsPaginateTypeDef,
     ListCellsRequestRequestTypeDef,
-    ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef,
     ListCrossAccountAuthorizationsRequestRequestTypeDef,
-    ListCrossAccountAuthorizationsResponseTypeDef,
-    ListReadinessChecksRequestListReadinessChecksPaginateTypeDef,
     ListReadinessChecksRequestRequestTypeDef,
     ReadinessCheckOutputTypeDef,
-    ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef,
     ListRecoveryGroupsRequestRequestTypeDef,
     RecoveryGroupOutputTypeDef,
-    ListResourceSetsRequestListResourceSetsPaginateTypeDef,
     ListResourceSetsRequestRequestTypeDef,
     ListRulesOutputTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     ListTagsForResourcesRequestRequestTypeDef,
-    ListTagsForResourcesResponseTypeDef,
+    NLBResourceOutputTypeDef,
     NLBResourceTypeDef,
-    PaginatorConfigTypeDef,
+    R53ResourceRecordOutputTypeDef,
     R53ResourceRecordTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCellRequestRequestTypeDef,
-    UpdateCellResponseTypeDef,
     UpdateReadinessCheckRequestRequestTypeDef,
-    UpdateReadinessCheckResponseTypeDef,
     UpdateRecoveryGroupRequestRequestTypeDef,
-    UpdateRecoveryGroupResponseTypeDef,
+    CreateCellResponseTypeDef,
+    CreateCrossAccountAuthorizationResponseTypeDef,
+    CreateReadinessCheckResponseTypeDef,
+    CreateRecoveryGroupResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCellResponseTypeDef,
+    GetReadinessCheckResponseTypeDef,
+    GetRecoveryGroupResponseTypeDef,
     ListCellsResponseTypeDef,
+    ListCrossAccountAuthorizationsResponseTypeDef,
+    ListTagsForResourcesResponseTypeDef,
+    UpdateCellResponseTypeDef,
+    UpdateReadinessCheckResponseTypeDef,
+    UpdateRecoveryGroupResponseTypeDef,
     GetArchitectureRecommendationsResponseTypeDef,
+    GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
+    GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
+    GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
+    GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
+    ListCellsRequestListCellsPaginateTypeDef,
+    ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef,
+    ListReadinessChecksRequestListReadinessChecksPaginateTypeDef,
+    ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef,
+    ListResourceSetsRequestListResourceSetsPaginateTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
     GetCellReadinessSummaryResponseTypeDef,
     GetRecoveryGroupReadinessSummaryResponseTypeDef,
     RuleResultTypeDef,
     GetReadinessCheckStatusResponseTypeDef,
     ListReadinessChecksResponseTypeDef,
     ListRecoveryGroupsResponseTypeDef,
     ListRulesResponseTypeDef,
+    TargetResourceOutputTypeDef,
     TargetResourceTypeDef,
     GetReadinessCheckResourceStatusResponseTypeDef,
+    DNSTargetResourceOutputTypeDef,
     DNSTargetResourceTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
-    CreateResourceSetRequestRequestTypeDef,
     CreateResourceSetResponseTypeDef,
     GetResourceSetResponseTypeDef,
     ResourceSetOutputTypeDef,
-    UpdateResourceSetRequestRequestTypeDef,
     UpdateResourceSetResponseTypeDef,
+    CreateResourceSetRequestRequestTypeDef,
+    UpdateResourceSetRequestRequestTypeDef,
     ListResourceSetsResponseTypeDef,
 )
 
 
 def get_structure() -> CellOutputTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.0/README.md` & `mypy-boto3-route53-recovery-readiness-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-route53-recovery-readiness"></a>
 
 # mypy-boto3-route53-recovery-readiness
 
 [![PyPI - mypy-boto3-route53-recovery-readiness](https://img.shields.io/pypi/v/mypy-boto3-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-readiness)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-readiness)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53-recovery-readiness?color=blue)](https://pypistats.org/packages/mypy-boto3-route53-recovery-readiness)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53-recovery-readiness)](https://pepy.tech/project/mypy-boto3-route53-recovery-readiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryReadiness 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
+[boto3.Route53RecoveryReadiness 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
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
 [mypy-boto3-route53-recovery-readiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,96 +333,101 @@
 `mypy_boto3_route53_recovery_readiness.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53_recovery_readiness.type_defs import (
     CellOutputTypeDef,
     CreateCellRequestRequestTypeDef,
-    CreateCellResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateCrossAccountAuthorizationRequestRequestTypeDef,
-    CreateCrossAccountAuthorizationResponseTypeDef,
     CreateReadinessCheckRequestRequestTypeDef,
-    CreateReadinessCheckResponseTypeDef,
     CreateRecoveryGroupRequestRequestTypeDef,
-    CreateRecoveryGroupResponseTypeDef,
     DeleteCellRequestRequestTypeDef,
     DeleteCrossAccountAuthorizationRequestRequestTypeDef,
     DeleteReadinessCheckRequestRequestTypeDef,
     DeleteRecoveryGroupRequestRequestTypeDef,
     DeleteResourceSetRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetArchitectureRecommendationsRequestRequestTypeDef,
     RecommendationTypeDef,
-    GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetCellReadinessSummaryRequestRequestTypeDef,
     ReadinessCheckSummaryTypeDef,
     GetCellRequestRequestTypeDef,
-    GetCellResponseTypeDef,
     GetReadinessCheckRequestRequestTypeDef,
-    GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
     GetReadinessCheckResourceStatusRequestRequestTypeDef,
-    GetReadinessCheckResponseTypeDef,
-    GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
     GetReadinessCheckStatusRequestRequestTypeDef,
     MessageTypeDef,
     ResourceResultTypeDef,
-    GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
     GetRecoveryGroupReadinessSummaryRequestRequestTypeDef,
     GetRecoveryGroupRequestRequestTypeDef,
-    GetRecoveryGroupResponseTypeDef,
     GetResourceSetRequestRequestTypeDef,
-    ListCellsRequestListCellsPaginateTypeDef,
     ListCellsRequestRequestTypeDef,
-    ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef,
     ListCrossAccountAuthorizationsRequestRequestTypeDef,
-    ListCrossAccountAuthorizationsResponseTypeDef,
-    ListReadinessChecksRequestListReadinessChecksPaginateTypeDef,
     ListReadinessChecksRequestRequestTypeDef,
     ReadinessCheckOutputTypeDef,
-    ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef,
     ListRecoveryGroupsRequestRequestTypeDef,
     RecoveryGroupOutputTypeDef,
-    ListResourceSetsRequestListResourceSetsPaginateTypeDef,
     ListResourceSetsRequestRequestTypeDef,
     ListRulesOutputTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     ListTagsForResourcesRequestRequestTypeDef,
-    ListTagsForResourcesResponseTypeDef,
+    NLBResourceOutputTypeDef,
     NLBResourceTypeDef,
-    PaginatorConfigTypeDef,
+    R53ResourceRecordOutputTypeDef,
     R53ResourceRecordTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCellRequestRequestTypeDef,
-    UpdateCellResponseTypeDef,
     UpdateReadinessCheckRequestRequestTypeDef,
-    UpdateReadinessCheckResponseTypeDef,
     UpdateRecoveryGroupRequestRequestTypeDef,
-    UpdateRecoveryGroupResponseTypeDef,
+    CreateCellResponseTypeDef,
+    CreateCrossAccountAuthorizationResponseTypeDef,
+    CreateReadinessCheckResponseTypeDef,
+    CreateRecoveryGroupResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCellResponseTypeDef,
+    GetReadinessCheckResponseTypeDef,
+    GetRecoveryGroupResponseTypeDef,
     ListCellsResponseTypeDef,
+    ListCrossAccountAuthorizationsResponseTypeDef,
+    ListTagsForResourcesResponseTypeDef,
+    UpdateCellResponseTypeDef,
+    UpdateReadinessCheckResponseTypeDef,
+    UpdateRecoveryGroupResponseTypeDef,
     GetArchitectureRecommendationsResponseTypeDef,
+    GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
+    GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
+    GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
+    GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
+    ListCellsRequestListCellsPaginateTypeDef,
+    ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef,
+    ListReadinessChecksRequestListReadinessChecksPaginateTypeDef,
+    ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef,
+    ListResourceSetsRequestListResourceSetsPaginateTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
     GetCellReadinessSummaryResponseTypeDef,
     GetRecoveryGroupReadinessSummaryResponseTypeDef,
     RuleResultTypeDef,
     GetReadinessCheckStatusResponseTypeDef,
     ListReadinessChecksResponseTypeDef,
     ListRecoveryGroupsResponseTypeDef,
     ListRulesResponseTypeDef,
+    TargetResourceOutputTypeDef,
     TargetResourceTypeDef,
     GetReadinessCheckResourceStatusResponseTypeDef,
+    DNSTargetResourceOutputTypeDef,
     DNSTargetResourceTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
-    CreateResourceSetRequestRequestTypeDef,
     CreateResourceSetResponseTypeDef,
     GetResourceSetResponseTypeDef,
     ResourceSetOutputTypeDef,
-    UpdateResourceSetRequestRequestTypeDef,
     UpdateResourceSetResponseTypeDef,
+    CreateResourceSetRequestRequestTypeDef,
+    UpdateResourceSetRequestRequestTypeDef,
     ListResourceSetsResponseTypeDef,
 )
 
 
 def get_structure() -> CellOutputTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/__init__.py` & `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/__init__.pyi` & `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/__main__.py` & `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53RecoveryReadiness 1.28.0\nVersion:        "
-        " 1.28.0\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.Route53RecoveryReadiness 1.28.12\nVersion:        "
+        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness\nOther"
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

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/client.py` & `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/client.pyi` & `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/literals.py` & `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,15 @@
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
@@ -251,26 +252,28 @@
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

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/literals.pyi` & `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,15 @@
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
@@ -249,26 +250,28 @@
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

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/paginator.py` & `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 class GetCellReadinessSummaryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetCellReadinessSummary)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getcellreadinesssummarypaginator)
     """
 
     def paginate(
-        self, *, CellName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CellName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetCellReadinessSummaryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetCellReadinessSummary.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getcellreadinesssummarypaginator)
         """
 
 
@@ -101,133 +101,133 @@
     """
 
     def paginate(
         self,
         *,
         ReadinessCheckName: str,
         ResourceIdentifier: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetReadinessCheckResourceStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetReadinessCheckResourceStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getreadinesscheckresourcestatuspaginator)
         """
 
 
 class GetReadinessCheckStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetReadinessCheckStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getreadinesscheckstatuspaginator)
     """
 
     def paginate(
-        self, *, ReadinessCheckName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ReadinessCheckName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetReadinessCheckStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetReadinessCheckStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getreadinesscheckstatuspaginator)
         """
 
 
 class GetRecoveryGroupReadinessSummaryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetRecoveryGroupReadinessSummary)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getrecoverygroupreadinesssummarypaginator)
     """
 
     def paginate(
-        self, *, RecoveryGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RecoveryGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRecoveryGroupReadinessSummaryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetRecoveryGroupReadinessSummary.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getrecoverygroupreadinesssummarypaginator)
         """
 
 
 class ListCellsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListCells)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listcellspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCellsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListCells.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listcellspaginator)
         """
 
 
 class ListCrossAccountAuthorizationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListCrossAccountAuthorizations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listcrossaccountauthorizationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCrossAccountAuthorizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListCrossAccountAuthorizations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listcrossaccountauthorizationspaginator)
         """
 
 
 class ListReadinessChecksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListReadinessChecks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listreadinesscheckspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReadinessChecksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListReadinessChecks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listreadinesscheckspaginator)
         """
 
 
 class ListRecoveryGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListRecoveryGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listrecoverygroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecoveryGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListRecoveryGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listrecoverygroupspaginator)
         """
 
 
 class ListResourceSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListResourceSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listresourcesetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListResourceSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listresourcesetspaginator)
         """
 
 
 class ListRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listrulespaginator)
     """
 
     def paginate(
-        self, *, ResourceType: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceType: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listrulespaginator)
         """
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/paginator.pyi` & `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 class GetCellReadinessSummaryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetCellReadinessSummary)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getcellreadinesssummarypaginator)
     """
 
     def paginate(
-        self, *, CellName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CellName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetCellReadinessSummaryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetCellReadinessSummary.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getcellreadinesssummarypaginator)
         """
 
 class GetReadinessCheckResourceStatusPaginator(Paginator):
@@ -97,125 +97,125 @@
     """
 
     def paginate(
         self,
         *,
         ReadinessCheckName: str,
         ResourceIdentifier: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetReadinessCheckResourceStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetReadinessCheckResourceStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getreadinesscheckresourcestatuspaginator)
         """
 
 class GetReadinessCheckStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetReadinessCheckStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getreadinesscheckstatuspaginator)
     """
 
     def paginate(
-        self, *, ReadinessCheckName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ReadinessCheckName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetReadinessCheckStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetReadinessCheckStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getreadinesscheckstatuspaginator)
         """
 
 class GetRecoveryGroupReadinessSummaryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetRecoveryGroupReadinessSummary)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getrecoverygroupreadinesssummarypaginator)
     """
 
     def paginate(
-        self, *, RecoveryGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RecoveryGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRecoveryGroupReadinessSummaryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetRecoveryGroupReadinessSummary.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#getrecoverygroupreadinesssummarypaginator)
         """
 
 class ListCellsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListCells)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listcellspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCellsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListCells.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listcellspaginator)
         """
 
 class ListCrossAccountAuthorizationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListCrossAccountAuthorizations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listcrossaccountauthorizationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCrossAccountAuthorizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListCrossAccountAuthorizations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listcrossaccountauthorizationspaginator)
         """
 
 class ListReadinessChecksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListReadinessChecks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listreadinesscheckspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReadinessChecksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListReadinessChecks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listreadinesscheckspaginator)
         """
 
 class ListRecoveryGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListRecoveryGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listrecoverygroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecoveryGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListRecoveryGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listrecoverygroupspaginator)
         """
 
 class ListResourceSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListResourceSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listresourcesetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListResourceSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listresourcesetspaginator)
         """
 
 class ListRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listrulespaginator)
     """
 
     def paginate(
-        self, *, ResourceType: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceType: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/paginators/#listrulespaginator)
         """
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/type_defs.py` & `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -18,100 +18,104 @@
 from .literals import ReadinessType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CellOutputTypeDef",
     "CreateCellRequestRequestTypeDef",
-    "CreateCellResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateCrossAccountAuthorizationRequestRequestTypeDef",
-    "CreateCrossAccountAuthorizationResponseTypeDef",
     "CreateReadinessCheckRequestRequestTypeDef",
-    "CreateReadinessCheckResponseTypeDef",
     "CreateRecoveryGroupRequestRequestTypeDef",
-    "CreateRecoveryGroupResponseTypeDef",
     "DeleteCellRequestRequestTypeDef",
     "DeleteCrossAccountAuthorizationRequestRequestTypeDef",
     "DeleteReadinessCheckRequestRequestTypeDef",
     "DeleteRecoveryGroupRequestRequestTypeDef",
     "DeleteResourceSetRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetArchitectureRecommendationsRequestRequestTypeDef",
     "RecommendationTypeDef",
-    "GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetCellReadinessSummaryRequestRequestTypeDef",
     "ReadinessCheckSummaryTypeDef",
     "GetCellRequestRequestTypeDef",
-    "GetCellResponseTypeDef",
     "GetReadinessCheckRequestRequestTypeDef",
-    "GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
     "GetReadinessCheckResourceStatusRequestRequestTypeDef",
-    "GetReadinessCheckResponseTypeDef",
-    "GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
     "GetReadinessCheckStatusRequestRequestTypeDef",
     "MessageTypeDef",
     "ResourceResultTypeDef",
-    "GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
     "GetRecoveryGroupReadinessSummaryRequestRequestTypeDef",
     "GetRecoveryGroupRequestRequestTypeDef",
-    "GetRecoveryGroupResponseTypeDef",
     "GetResourceSetRequestRequestTypeDef",
-    "ListCellsRequestListCellsPaginateTypeDef",
     "ListCellsRequestRequestTypeDef",
-    "ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef",
     "ListCrossAccountAuthorizationsRequestRequestTypeDef",
-    "ListCrossAccountAuthorizationsResponseTypeDef",
-    "ListReadinessChecksRequestListReadinessChecksPaginateTypeDef",
     "ListReadinessChecksRequestRequestTypeDef",
     "ReadinessCheckOutputTypeDef",
-    "ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef",
     "ListRecoveryGroupsRequestRequestTypeDef",
     "RecoveryGroupOutputTypeDef",
-    "ListResourceSetsRequestListResourceSetsPaginateTypeDef",
     "ListResourceSetsRequestRequestTypeDef",
     "ListRulesOutputTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
     "ListTagsForResourcesRequestRequestTypeDef",
-    "ListTagsForResourcesResponseTypeDef",
+    "NLBResourceOutputTypeDef",
     "NLBResourceTypeDef",
-    "PaginatorConfigTypeDef",
+    "R53ResourceRecordOutputTypeDef",
     "R53ResourceRecordTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCellRequestRequestTypeDef",
-    "UpdateCellResponseTypeDef",
     "UpdateReadinessCheckRequestRequestTypeDef",
-    "UpdateReadinessCheckResponseTypeDef",
     "UpdateRecoveryGroupRequestRequestTypeDef",
-    "UpdateRecoveryGroupResponseTypeDef",
+    "CreateCellResponseTypeDef",
+    "CreateCrossAccountAuthorizationResponseTypeDef",
+    "CreateReadinessCheckResponseTypeDef",
+    "CreateRecoveryGroupResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCellResponseTypeDef",
+    "GetReadinessCheckResponseTypeDef",
+    "GetRecoveryGroupResponseTypeDef",
     "ListCellsResponseTypeDef",
+    "ListCrossAccountAuthorizationsResponseTypeDef",
+    "ListTagsForResourcesResponseTypeDef",
+    "UpdateCellResponseTypeDef",
+    "UpdateReadinessCheckResponseTypeDef",
+    "UpdateRecoveryGroupResponseTypeDef",
     "GetArchitectureRecommendationsResponseTypeDef",
+    "GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
+    "GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
+    "GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
+    "GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
+    "ListCellsRequestListCellsPaginateTypeDef",
+    "ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef",
+    "ListReadinessChecksRequestListReadinessChecksPaginateTypeDef",
+    "ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef",
+    "ListResourceSetsRequestListResourceSetsPaginateTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
     "GetCellReadinessSummaryResponseTypeDef",
     "GetRecoveryGroupReadinessSummaryResponseTypeDef",
     "RuleResultTypeDef",
     "GetReadinessCheckStatusResponseTypeDef",
     "ListReadinessChecksResponseTypeDef",
     "ListRecoveryGroupsResponseTypeDef",
     "ListRulesResponseTypeDef",
+    "TargetResourceOutputTypeDef",
     "TargetResourceTypeDef",
     "GetReadinessCheckResourceStatusResponseTypeDef",
+    "DNSTargetResourceOutputTypeDef",
     "DNSTargetResourceTypeDef",
+    "ResourceOutputTypeDef",
     "ResourceTypeDef",
-    "CreateResourceSetRequestRequestTypeDef",
     "CreateResourceSetResponseTypeDef",
     "GetResourceSetResponseTypeDef",
     "ResourceSetOutputTypeDef",
-    "UpdateResourceSetRequestRequestTypeDef",
     "UpdateResourceSetResponseTypeDef",
+    "CreateResourceSetRequestRequestTypeDef",
+    "UpdateResourceSetRequestRequestTypeDef",
     "ListResourceSetsResponseTypeDef",
 )
 
 _RequiredCellOutputTypeDef = TypedDict(
     "_RequiredCellOutputTypeDef",
     {
         "CellArn": str,
@@ -124,19 +128,17 @@
     "_OptionalCellOutputTypeDef",
     {
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class CellOutputTypeDef(_RequiredCellOutputTypeDef, _OptionalCellOutputTypeDef):
     pass
 
-
 _RequiredCreateCellRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCellRequestRequestTypeDef",
     {
         "CellName": str,
     },
 )
 _OptionalCreateCellRequestRequestTypeDef = TypedDict(
@@ -144,48 +146,37 @@
     {
         "Cells": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateCellRequestRequestTypeDef(
     _RequiredCreateCellRequestRequestTypeDef, _OptionalCreateCellRequestRequestTypeDef
 ):
     pass
 
-
-CreateCellResponseTypeDef = TypedDict(
-    "CreateCellResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "CellArn": str,
-        "CellName": str,
-        "Cells": List[str],
-        "ParentReadinessScopes": List[str],
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CreateCrossAccountAuthorizationRequestRequestTypeDef = TypedDict(
     "CreateCrossAccountAuthorizationRequestRequestTypeDef",
     {
         "CrossAccountAuthorization": str,
     },
 )
 
-CreateCrossAccountAuthorizationResponseTypeDef = TypedDict(
-    "CreateCrossAccountAuthorizationResponseTypeDef",
-    {
-        "CrossAccountAuthorization": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateReadinessCheckRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReadinessCheckRequestRequestTypeDef",
     {
         "ReadinessCheckName": str,
         "ResourceSetName": str,
     },
 )
@@ -193,33 +184,20 @@
     "_OptionalCreateReadinessCheckRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateReadinessCheckRequestRequestTypeDef(
     _RequiredCreateReadinessCheckRequestRequestTypeDef,
     _OptionalCreateReadinessCheckRequestRequestTypeDef,
 ):
     pass
 
-
-CreateReadinessCheckResponseTypeDef = TypedDict(
-    "CreateReadinessCheckResponseTypeDef",
-    {
-        "ReadinessCheckArn": str,
-        "ReadinessCheckName": str,
-        "ResourceSet": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateRecoveryGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRecoveryGroupRequestRequestTypeDef",
     {
         "RecoveryGroupName": str,
     },
 )
 _OptionalCreateRecoveryGroupRequestRequestTypeDef = TypedDict(
@@ -227,33 +205,20 @@
     {
         "Cells": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateRecoveryGroupRequestRequestTypeDef(
     _RequiredCreateRecoveryGroupRequestRequestTypeDef,
     _OptionalCreateRecoveryGroupRequestRequestTypeDef,
 ):
     pass
 
-
-CreateRecoveryGroupResponseTypeDef = TypedDict(
-    "CreateRecoveryGroupResponseTypeDef",
-    {
-        "Cells": List[str],
-        "RecoveryGroupArn": str,
-        "RecoveryGroupName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteCellRequestRequestTypeDef = TypedDict(
     "DeleteCellRequestRequestTypeDef",
     {
         "CellName": str,
     },
 )
 
@@ -281,21 +246,14 @@
 DeleteResourceSetRequestRequestTypeDef = TypedDict(
     "DeleteResourceSetRequestRequestTypeDef",
     {
         "ResourceSetName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetArchitectureRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetArchitectureRecommendationsRequestRequestTypeDef",
     {
         "RecoveryGroupName": str,
     },
 )
 _OptionalGetArchitectureRecommendationsRequestRequestTypeDef = TypedDict(
@@ -303,51 +261,37 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetArchitectureRecommendationsRequestRequestTypeDef(
     _RequiredGetArchitectureRecommendationsRequestRequestTypeDef,
     _OptionalGetArchitectureRecommendationsRequestRequestTypeDef,
 ):
     pass
 
-
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "RecommendationText": str,
     },
 )
 
-_RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef = TypedDict(
-    "_RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
-    {
-        "CellName": str,
-    },
-)
-_OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef = TypedDict(
-    "_OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
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
-class GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef(
-    _RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
-    _OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetCellReadinessSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetCellReadinessSummaryRequestRequestTypeDef",
     {
         "CellName": str,
     },
 )
 _OptionalGetCellReadinessSummaryRequestRequestTypeDef = TypedDict(
@@ -355,22 +299,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetCellReadinessSummaryRequestRequestTypeDef(
     _RequiredGetCellReadinessSummaryRequestRequestTypeDef,
     _OptionalGetCellReadinessSummaryRequestRequestTypeDef,
 ):
     pass
 
-
 ReadinessCheckSummaryTypeDef = TypedDict(
     "ReadinessCheckSummaryTypeDef",
     {
         "Readiness": ReadinessType,
         "ReadinessCheckName": str,
     },
     total=False,
@@ -379,56 +321,21 @@
 GetCellRequestRequestTypeDef = TypedDict(
     "GetCellRequestRequestTypeDef",
     {
         "CellName": str,
     },
 )
 
-GetCellResponseTypeDef = TypedDict(
-    "GetCellResponseTypeDef",
-    {
-        "CellArn": str,
-        "CellName": str,
-        "Cells": List[str],
-        "ParentReadinessScopes": List[str],
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetReadinessCheckRequestRequestTypeDef = TypedDict(
     "GetReadinessCheckRequestRequestTypeDef",
     {
         "ReadinessCheckName": str,
     },
 )
 
-_RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef = TypedDict(
-    "_RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
-    {
-        "ReadinessCheckName": str,
-        "ResourceIdentifier": str,
-    },
-)
-_OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef = TypedDict(
-    "_OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef(
-    _RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
-    _OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetReadinessCheckResourceStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetReadinessCheckResourceStatusRequestRequestTypeDef",
     {
         "ReadinessCheckName": str,
         "ResourceIdentifier": str,
     },
 )
@@ -437,55 +344,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetReadinessCheckResourceStatusRequestRequestTypeDef(
     _RequiredGetReadinessCheckResourceStatusRequestRequestTypeDef,
     _OptionalGetReadinessCheckResourceStatusRequestRequestTypeDef,
 ):
     pass
 
-
-GetReadinessCheckResponseTypeDef = TypedDict(
-    "GetReadinessCheckResponseTypeDef",
-    {
-        "ReadinessCheckArn": str,
-        "ReadinessCheckName": str,
-        "ResourceSet": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef = TypedDict(
-    "_RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
-    {
-        "ReadinessCheckName": str,
-    },
-)
-_OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef = TypedDict(
-    "_OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef(
-    _RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
-    _OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetReadinessCheckStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetReadinessCheckStatusRequestRequestTypeDef",
     {
         "ReadinessCheckName": str,
     },
 )
 _OptionalGetReadinessCheckStatusRequestRequestTypeDef = TypedDict(
@@ -493,22 +365,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetReadinessCheckStatusRequestRequestTypeDef(
     _RequiredGetReadinessCheckStatusRequestRequestTypeDef,
     _OptionalGetReadinessCheckStatusRequestRequestTypeDef,
 ):
     pass
 
-
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "MessageText": str,
     },
     total=False,
 )
@@ -525,41 +395,17 @@
     {
         "ComponentId": str,
         "ResourceArn": str,
     },
     total=False,
 )
 
-
 class ResourceResultTypeDef(_RequiredResourceResultTypeDef, _OptionalResourceResultTypeDef):
     pass
 
-
-_RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef = TypedDict(
-    "_RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
-    {
-        "RecoveryGroupName": str,
-    },
-)
-_OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef = TypedDict(
-    "_OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef(
-    _RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
-    _OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetRecoveryGroupReadinessSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetRecoveryGroupReadinessSummaryRequestRequestTypeDef",
     {
         "RecoveryGroupName": str,
     },
 )
 _OptionalGetRecoveryGroupReadinessSummaryRequestRequestTypeDef = TypedDict(
@@ -567,98 +413,52 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetRecoveryGroupReadinessSummaryRequestRequestTypeDef(
     _RequiredGetRecoveryGroupReadinessSummaryRequestRequestTypeDef,
     _OptionalGetRecoveryGroupReadinessSummaryRequestRequestTypeDef,
 ):
     pass
 
-
 GetRecoveryGroupRequestRequestTypeDef = TypedDict(
     "GetRecoveryGroupRequestRequestTypeDef",
     {
         "RecoveryGroupName": str,
     },
 )
 
-GetRecoveryGroupResponseTypeDef = TypedDict(
-    "GetRecoveryGroupResponseTypeDef",
-    {
-        "Cells": List[str],
-        "RecoveryGroupArn": str,
-        "RecoveryGroupName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResourceSetRequestRequestTypeDef = TypedDict(
     "GetResourceSetRequestRequestTypeDef",
     {
         "ResourceSetName": str,
     },
 )
 
-ListCellsRequestListCellsPaginateTypeDef = TypedDict(
-    "ListCellsRequestListCellsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCellsRequestRequestTypeDef = TypedDict(
     "ListCellsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef = TypedDict(
-    "ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCrossAccountAuthorizationsRequestRequestTypeDef = TypedDict(
     "ListCrossAccountAuthorizationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListCrossAccountAuthorizationsResponseTypeDef = TypedDict(
-    "ListCrossAccountAuthorizationsResponseTypeDef",
-    {
-        "CrossAccountAuthorizations": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListReadinessChecksRequestListReadinessChecksPaginateTypeDef = TypedDict(
-    "ListReadinessChecksRequestListReadinessChecksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListReadinessChecksRequestRequestTypeDef = TypedDict(
     "ListReadinessChecksRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -676,29 +476,19 @@
     {
         "ReadinessCheckName": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class ReadinessCheckOutputTypeDef(
     _RequiredReadinessCheckOutputTypeDef, _OptionalReadinessCheckOutputTypeDef
 ):
     pass
 
-
-ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef = TypedDict(
-    "ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRecoveryGroupsRequestRequestTypeDef = TypedDict(
     "ListRecoveryGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -716,29 +506,19 @@
     "_OptionalRecoveryGroupOutputTypeDef",
     {
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class RecoveryGroupOutputTypeDef(
     _RequiredRecoveryGroupOutputTypeDef, _OptionalRecoveryGroupOutputTypeDef
 ):
     pass
 
-
-ListResourceSetsRequestListResourceSetsPaginateTypeDef = TypedDict(
-    "ListResourceSetsRequestListResourceSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResourceSetsRequestRequestTypeDef = TypedDict(
     "ListResourceSetsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -749,23 +529,14 @@
     {
         "ResourceType": str,
         "RuleDescription": str,
         "RuleId": str,
     },
 )
 
-ListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "ListRulesRequestListRulesPaginateTypeDef",
-    {
-        "ResourceType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRulesRequestRequestTypeDef = TypedDict(
     "ListRulesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "ResourceType": str,
     },
@@ -775,60 +546,48 @@
 ListTagsForResourcesRequestRequestTypeDef = TypedDict(
     "ListTagsForResourcesRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourcesResponseTypeDef = TypedDict(
-    "ListTagsForResourcesResponseTypeDef",
+NLBResourceOutputTypeDef = TypedDict(
+    "NLBResourceOutputTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Arn": str,
     },
+    total=False,
 )
 
 NLBResourceTypeDef = TypedDict(
     "NLBResourceTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+R53ResourceRecordOutputTypeDef = TypedDict(
+    "R53ResourceRecordOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "DomainName": str,
+        "RecordSetId": str,
     },
     total=False,
 )
 
 R53ResourceRecordTypeDef = TypedDict(
     "R53ResourceRecordTypeDef",
     {
         "DomainName": str,
         "RecordSetId": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -845,100 +604,330 @@
     "UpdateCellRequestRequestTypeDef",
     {
         "CellName": str,
         "Cells": Sequence[str],
     },
 )
 
-UpdateCellResponseTypeDef = TypedDict(
-    "UpdateCellResponseTypeDef",
+UpdateReadinessCheckRequestRequestTypeDef = TypedDict(
+    "UpdateReadinessCheckRequestRequestTypeDef",
+    {
+        "ReadinessCheckName": str,
+        "ResourceSetName": str,
+    },
+)
+
+UpdateRecoveryGroupRequestRequestTypeDef = TypedDict(
+    "UpdateRecoveryGroupRequestRequestTypeDef",
+    {
+        "Cells": Sequence[str],
+        "RecoveryGroupName": str,
+    },
+)
+
+CreateCellResponseTypeDef = TypedDict(
+    "CreateCellResponseTypeDef",
     {
         "CellArn": str,
         "CellName": str,
         "Cells": List[str],
         "ParentReadinessScopes": List[str],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateReadinessCheckRequestRequestTypeDef = TypedDict(
-    "UpdateReadinessCheckRequestRequestTypeDef",
+CreateCrossAccountAuthorizationResponseTypeDef = TypedDict(
+    "CreateCrossAccountAuthorizationResponseTypeDef",
     {
-        "ReadinessCheckName": str,
-        "ResourceSetName": str,
+        "CrossAccountAuthorization": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateReadinessCheckResponseTypeDef = TypedDict(
-    "UpdateReadinessCheckResponseTypeDef",
+CreateReadinessCheckResponseTypeDef = TypedDict(
+    "CreateReadinessCheckResponseTypeDef",
     {
         "ReadinessCheckArn": str,
         "ReadinessCheckName": str,
         "ResourceSet": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateRecoveryGroupRequestRequestTypeDef = TypedDict(
-    "UpdateRecoveryGroupRequestRequestTypeDef",
+CreateRecoveryGroupResponseTypeDef = TypedDict(
+    "CreateRecoveryGroupResponseTypeDef",
     {
-        "Cells": Sequence[str],
+        "Cells": List[str],
+        "RecoveryGroupArn": str,
         "RecoveryGroupName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateRecoveryGroupResponseTypeDef = TypedDict(
-    "UpdateRecoveryGroupResponseTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCellResponseTypeDef = TypedDict(
+    "GetCellResponseTypeDef",
+    {
+        "CellArn": str,
+        "CellName": str,
+        "Cells": List[str],
+        "ParentReadinessScopes": List[str],
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetReadinessCheckResponseTypeDef = TypedDict(
+    "GetReadinessCheckResponseTypeDef",
+    {
+        "ReadinessCheckArn": str,
+        "ReadinessCheckName": str,
+        "ResourceSet": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRecoveryGroupResponseTypeDef = TypedDict(
+    "GetRecoveryGroupResponseTypeDef",
     {
         "Cells": List[str],
         "RecoveryGroupArn": str,
         "RecoveryGroupName": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCellsResponseTypeDef = TypedDict(
     "ListCellsResponseTypeDef",
     {
         "Cells": List[CellOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCrossAccountAuthorizationsResponseTypeDef = TypedDict(
+    "ListCrossAccountAuthorizationsResponseTypeDef",
+    {
+        "CrossAccountAuthorizations": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourcesResponseTypeDef = TypedDict(
+    "ListTagsForResourcesResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateCellResponseTypeDef = TypedDict(
+    "UpdateCellResponseTypeDef",
+    {
+        "CellArn": str,
+        "CellName": str,
+        "Cells": List[str],
+        "ParentReadinessScopes": List[str],
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateReadinessCheckResponseTypeDef = TypedDict(
+    "UpdateReadinessCheckResponseTypeDef",
+    {
+        "ReadinessCheckArn": str,
+        "ReadinessCheckName": str,
+        "ResourceSet": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRecoveryGroupResponseTypeDef = TypedDict(
+    "UpdateRecoveryGroupResponseTypeDef",
+    {
+        "Cells": List[str],
+        "RecoveryGroupArn": str,
+        "RecoveryGroupName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetArchitectureRecommendationsResponseTypeDef = TypedDict(
     "GetArchitectureRecommendationsResponseTypeDef",
     {
         "LastAuditTimestamp": datetime,
         "NextToken": str,
         "Recommendations": List[RecommendationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef = TypedDict(
+    "_RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
+    {
+        "CellName": str,
+    },
+)
+_OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef = TypedDict(
+    "_OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef(
+    _RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
+    _OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
+):
+    pass
+
+_RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef = TypedDict(
+    "_RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
+    {
+        "ReadinessCheckName": str,
+        "ResourceIdentifier": str,
+    },
+)
+_OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef = TypedDict(
+    "_OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef(
+    _RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
+    _OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
+):
+    pass
+
+_RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef = TypedDict(
+    "_RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
+    {
+        "ReadinessCheckName": str,
+    },
+)
+_OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef = TypedDict(
+    "_OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef(
+    _RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
+    _OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
+):
+    pass
+
+_RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef = TypedDict(
+    "_RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
+    {
+        "RecoveryGroupName": str,
+    },
+)
+_OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef = TypedDict(
+    "_OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef(
+    _RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
+    _OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
+):
+    pass
+
+ListCellsRequestListCellsPaginateTypeDef = TypedDict(
+    "ListCellsRequestListCellsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef = TypedDict(
+    "ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListReadinessChecksRequestListReadinessChecksPaginateTypeDef = TypedDict(
+    "ListReadinessChecksRequestListReadinessChecksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef = TypedDict(
+    "ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResourceSetsRequestListResourceSetsPaginateTypeDef = TypedDict(
+    "ListResourceSetsRequestListResourceSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "ListRulesRequestListRulesPaginateTypeDef",
+    {
+        "ResourceType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 GetCellReadinessSummaryResponseTypeDef = TypedDict(
     "GetCellReadinessSummaryResponseTypeDef",
     {
         "NextToken": str,
         "Readiness": ReadinessType,
         "ReadinessChecks": List[ReadinessCheckSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecoveryGroupReadinessSummaryResponseTypeDef = TypedDict(
     "GetRecoveryGroupReadinessSummaryResponseTypeDef",
     {
         "NextToken": str,
         "Readiness": ReadinessType,
         "ReadinessChecks": List[ReadinessCheckSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RuleResultTypeDef = TypedDict(
     "RuleResultTypeDef",
     {
         "LastCheckedTimestamp": datetime,
@@ -951,43 +940,52 @@
 GetReadinessCheckStatusResponseTypeDef = TypedDict(
     "GetReadinessCheckStatusResponseTypeDef",
     {
         "Messages": List[MessageTypeDef],
         "NextToken": str,
         "Readiness": ReadinessType,
         "Resources": List[ResourceResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReadinessChecksResponseTypeDef = TypedDict(
     "ListReadinessChecksResponseTypeDef",
     {
         "NextToken": str,
         "ReadinessChecks": List[ReadinessCheckOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecoveryGroupsResponseTypeDef = TypedDict(
     "ListRecoveryGroupsResponseTypeDef",
     {
         "NextToken": str,
         "RecoveryGroups": List[RecoveryGroupOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "NextToken": str,
         "Rules": List[ListRulesOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TargetResourceOutputTypeDef = TypedDict(
+    "TargetResourceOutputTypeDef",
+    {
+        "NLBResource": NLBResourceOutputTypeDef,
+        "R53Resource": R53ResourceRecordOutputTypeDef,
     },
+    total=False,
 )
 
 TargetResourceTypeDef = TypedDict(
     "TargetResourceTypeDef",
     {
         "NLBResource": NLBResourceTypeDef,
         "R53Resource": R53ResourceRecordTypeDef,
@@ -997,134 +995,153 @@
 
 GetReadinessCheckResourceStatusResponseTypeDef = TypedDict(
     "GetReadinessCheckResourceStatusResponseTypeDef",
     {
         "NextToken": str,
         "Readiness": ReadinessType,
         "Rules": List[RuleResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DNSTargetResourceOutputTypeDef = TypedDict(
+    "DNSTargetResourceOutputTypeDef",
+    {
+        "DomainName": str,
+        "HostedZoneArn": str,
+        "RecordSetId": str,
+        "RecordType": str,
+        "TargetResource": TargetResourceOutputTypeDef,
     },
+    total=False,
 )
 
 DNSTargetResourceTypeDef = TypedDict(
     "DNSTargetResourceTypeDef",
     {
         "DomainName": str,
         "HostedZoneArn": str,
         "RecordSetId": str,
         "RecordType": str,
         "TargetResource": TargetResourceTypeDef,
     },
     total=False,
 )
 
-ResourceTypeDef = TypedDict(
-    "ResourceTypeDef",
+ResourceOutputTypeDef = TypedDict(
+    "ResourceOutputTypeDef",
     {
         "ComponentId": str,
-        "DnsTargetResource": DNSTargetResourceTypeDef,
-        "ReadinessScopes": Sequence[str],
+        "DnsTargetResource": DNSTargetResourceOutputTypeDef,
+        "ReadinessScopes": List[str],
         "ResourceArn": str,
     },
     total=False,
 )
 
-_RequiredCreateResourceSetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateResourceSetRequestRequestTypeDef",
-    {
-        "ResourceSetName": str,
-        "ResourceSetType": str,
-        "Resources": Sequence[ResourceTypeDef],
-    },
-)
-_OptionalCreateResourceSetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateResourceSetRequestRequestTypeDef",
+ResourceTypeDef = TypedDict(
+    "ResourceTypeDef",
     {
-        "Tags": Mapping[str, str],
+        "ComponentId": str,
+        "DnsTargetResource": DNSTargetResourceTypeDef,
+        "ReadinessScopes": Sequence[str],
+        "ResourceArn": str,
     },
     total=False,
 )
 
-
-class CreateResourceSetRequestRequestTypeDef(
-    _RequiredCreateResourceSetRequestRequestTypeDef, _OptionalCreateResourceSetRequestRequestTypeDef
-):
-    pass
-
-
 CreateResourceSetResponseTypeDef = TypedDict(
     "CreateResourceSetResponseTypeDef",
     {
         "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": List[ResourceTypeDef],
+        "Resources": List[ResourceOutputTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceSetResponseTypeDef = TypedDict(
     "GetResourceSetResponseTypeDef",
     {
         "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": List[ResourceTypeDef],
+        "Resources": List[ResourceOutputTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredResourceSetOutputTypeDef = TypedDict(
     "_RequiredResourceSetOutputTypeDef",
     {
         "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": List[ResourceTypeDef],
+        "Resources": List[ResourceOutputTypeDef],
     },
 )
 _OptionalResourceSetOutputTypeDef = TypedDict(
     "_OptionalResourceSetOutputTypeDef",
     {
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class ResourceSetOutputTypeDef(
     _RequiredResourceSetOutputTypeDef, _OptionalResourceSetOutputTypeDef
 ):
     pass
 
+UpdateResourceSetResponseTypeDef = TypedDict(
+    "UpdateResourceSetResponseTypeDef",
+    {
+        "ResourceSetArn": str,
+        "ResourceSetName": str,
+        "ResourceSetType": str,
+        "Resources": List[ResourceOutputTypeDef],
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-UpdateResourceSetRequestRequestTypeDef = TypedDict(
-    "UpdateResourceSetRequestRequestTypeDef",
+_RequiredCreateResourceSetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateResourceSetRequestRequestTypeDef",
     {
         "ResourceSetName": str,
         "ResourceSetType": str,
         "Resources": Sequence[ResourceTypeDef],
     },
 )
+_OptionalCreateResourceSetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateResourceSetRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
 
-UpdateResourceSetResponseTypeDef = TypedDict(
-    "UpdateResourceSetResponseTypeDef",
+class CreateResourceSetRequestRequestTypeDef(
+    _RequiredCreateResourceSetRequestRequestTypeDef, _OptionalCreateResourceSetRequestRequestTypeDef
+):
+    pass
+
+UpdateResourceSetRequestRequestTypeDef = TypedDict(
+    "UpdateResourceSetRequestRequestTypeDef",
     {
-        "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": List[ResourceTypeDef],
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Resources": Sequence[ResourceTypeDef],
     },
 )
 
 ListResourceSetsResponseTypeDef = TypedDict(
     "ListResourceSetsResponseTypeDef",
     {
         "NextToken": str,
         "ResourceSets": List[ResourceSetOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness/type_defs.pyi` & `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/type_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,99 +18,105 @@
 from .literals import ReadinessType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CellOutputTypeDef",
     "CreateCellRequestRequestTypeDef",
-    "CreateCellResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateCrossAccountAuthorizationRequestRequestTypeDef",
-    "CreateCrossAccountAuthorizationResponseTypeDef",
     "CreateReadinessCheckRequestRequestTypeDef",
-    "CreateReadinessCheckResponseTypeDef",
     "CreateRecoveryGroupRequestRequestTypeDef",
-    "CreateRecoveryGroupResponseTypeDef",
     "DeleteCellRequestRequestTypeDef",
     "DeleteCrossAccountAuthorizationRequestRequestTypeDef",
     "DeleteReadinessCheckRequestRequestTypeDef",
     "DeleteRecoveryGroupRequestRequestTypeDef",
     "DeleteResourceSetRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetArchitectureRecommendationsRequestRequestTypeDef",
     "RecommendationTypeDef",
-    "GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetCellReadinessSummaryRequestRequestTypeDef",
     "ReadinessCheckSummaryTypeDef",
     "GetCellRequestRequestTypeDef",
-    "GetCellResponseTypeDef",
     "GetReadinessCheckRequestRequestTypeDef",
-    "GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
     "GetReadinessCheckResourceStatusRequestRequestTypeDef",
-    "GetReadinessCheckResponseTypeDef",
-    "GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
     "GetReadinessCheckStatusRequestRequestTypeDef",
     "MessageTypeDef",
     "ResourceResultTypeDef",
-    "GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
     "GetRecoveryGroupReadinessSummaryRequestRequestTypeDef",
     "GetRecoveryGroupRequestRequestTypeDef",
-    "GetRecoveryGroupResponseTypeDef",
     "GetResourceSetRequestRequestTypeDef",
-    "ListCellsRequestListCellsPaginateTypeDef",
     "ListCellsRequestRequestTypeDef",
-    "ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef",
     "ListCrossAccountAuthorizationsRequestRequestTypeDef",
-    "ListCrossAccountAuthorizationsResponseTypeDef",
-    "ListReadinessChecksRequestListReadinessChecksPaginateTypeDef",
     "ListReadinessChecksRequestRequestTypeDef",
     "ReadinessCheckOutputTypeDef",
-    "ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef",
     "ListRecoveryGroupsRequestRequestTypeDef",
     "RecoveryGroupOutputTypeDef",
-    "ListResourceSetsRequestListResourceSetsPaginateTypeDef",
     "ListResourceSetsRequestRequestTypeDef",
     "ListRulesOutputTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
     "ListTagsForResourcesRequestRequestTypeDef",
-    "ListTagsForResourcesResponseTypeDef",
+    "NLBResourceOutputTypeDef",
     "NLBResourceTypeDef",
-    "PaginatorConfigTypeDef",
+    "R53ResourceRecordOutputTypeDef",
     "R53ResourceRecordTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCellRequestRequestTypeDef",
-    "UpdateCellResponseTypeDef",
     "UpdateReadinessCheckRequestRequestTypeDef",
-    "UpdateReadinessCheckResponseTypeDef",
     "UpdateRecoveryGroupRequestRequestTypeDef",
-    "UpdateRecoveryGroupResponseTypeDef",
+    "CreateCellResponseTypeDef",
+    "CreateCrossAccountAuthorizationResponseTypeDef",
+    "CreateReadinessCheckResponseTypeDef",
+    "CreateRecoveryGroupResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCellResponseTypeDef",
+    "GetReadinessCheckResponseTypeDef",
+    "GetRecoveryGroupResponseTypeDef",
     "ListCellsResponseTypeDef",
+    "ListCrossAccountAuthorizationsResponseTypeDef",
+    "ListTagsForResourcesResponseTypeDef",
+    "UpdateCellResponseTypeDef",
+    "UpdateReadinessCheckResponseTypeDef",
+    "UpdateRecoveryGroupResponseTypeDef",
     "GetArchitectureRecommendationsResponseTypeDef",
+    "GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
+    "GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
+    "GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
+    "GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
+    "ListCellsRequestListCellsPaginateTypeDef",
+    "ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef",
+    "ListReadinessChecksRequestListReadinessChecksPaginateTypeDef",
+    "ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef",
+    "ListResourceSetsRequestListResourceSetsPaginateTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
     "GetCellReadinessSummaryResponseTypeDef",
     "GetRecoveryGroupReadinessSummaryResponseTypeDef",
     "RuleResultTypeDef",
     "GetReadinessCheckStatusResponseTypeDef",
     "ListReadinessChecksResponseTypeDef",
     "ListRecoveryGroupsResponseTypeDef",
     "ListRulesResponseTypeDef",
+    "TargetResourceOutputTypeDef",
     "TargetResourceTypeDef",
     "GetReadinessCheckResourceStatusResponseTypeDef",
+    "DNSTargetResourceOutputTypeDef",
     "DNSTargetResourceTypeDef",
+    "ResourceOutputTypeDef",
     "ResourceTypeDef",
-    "CreateResourceSetRequestRequestTypeDef",
     "CreateResourceSetResponseTypeDef",
     "GetResourceSetResponseTypeDef",
     "ResourceSetOutputTypeDef",
-    "UpdateResourceSetRequestRequestTypeDef",
     "UpdateResourceSetResponseTypeDef",
+    "CreateResourceSetRequestRequestTypeDef",
+    "UpdateResourceSetRequestRequestTypeDef",
     "ListResourceSetsResponseTypeDef",
 )
 
 _RequiredCellOutputTypeDef = TypedDict(
     "_RequiredCellOutputTypeDef",
     {
         "CellArn": str,
@@ -123,17 +129,19 @@
     "_OptionalCellOutputTypeDef",
     {
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class CellOutputTypeDef(_RequiredCellOutputTypeDef, _OptionalCellOutputTypeDef):
     pass
 
+
 _RequiredCreateCellRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCellRequestRequestTypeDef",
     {
         "CellName": str,
     },
 )
 _OptionalCreateCellRequestRequestTypeDef = TypedDict(
@@ -141,46 +149,39 @@
     {
         "Cells": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateCellRequestRequestTypeDef(
     _RequiredCreateCellRequestRequestTypeDef, _OptionalCreateCellRequestRequestTypeDef
 ):
     pass
 
-CreateCellResponseTypeDef = TypedDict(
-    "CreateCellResponseTypeDef",
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "CellArn": str,
-        "CellName": str,
-        "Cells": List[str],
-        "ParentReadinessScopes": List[str],
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CreateCrossAccountAuthorizationRequestRequestTypeDef = TypedDict(
     "CreateCrossAccountAuthorizationRequestRequestTypeDef",
     {
         "CrossAccountAuthorization": str,
     },
 )
 
-CreateCrossAccountAuthorizationResponseTypeDef = TypedDict(
-    "CreateCrossAccountAuthorizationResponseTypeDef",
-    {
-        "CrossAccountAuthorization": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateReadinessCheckRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReadinessCheckRequestRequestTypeDef",
     {
         "ReadinessCheckName": str,
         "ResourceSetName": str,
     },
 )
@@ -188,30 +189,21 @@
     "_OptionalCreateReadinessCheckRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateReadinessCheckRequestRequestTypeDef(
     _RequiredCreateReadinessCheckRequestRequestTypeDef,
     _OptionalCreateReadinessCheckRequestRequestTypeDef,
 ):
     pass
 
-CreateReadinessCheckResponseTypeDef = TypedDict(
-    "CreateReadinessCheckResponseTypeDef",
-    {
-        "ReadinessCheckArn": str,
-        "ReadinessCheckName": str,
-        "ResourceSet": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreateRecoveryGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRecoveryGroupRequestRequestTypeDef",
     {
         "RecoveryGroupName": str,
     },
 )
@@ -220,30 +212,21 @@
     {
         "Cells": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateRecoveryGroupRequestRequestTypeDef(
     _RequiredCreateRecoveryGroupRequestRequestTypeDef,
     _OptionalCreateRecoveryGroupRequestRequestTypeDef,
 ):
     pass
 
-CreateRecoveryGroupResponseTypeDef = TypedDict(
-    "CreateRecoveryGroupResponseTypeDef",
-    {
-        "Cells": List[str],
-        "RecoveryGroupArn": str,
-        "RecoveryGroupName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeleteCellRequestRequestTypeDef = TypedDict(
     "DeleteCellRequestRequestTypeDef",
     {
         "CellName": str,
     },
 )
@@ -272,21 +255,14 @@
 DeleteResourceSetRequestRequestTypeDef = TypedDict(
     "DeleteResourceSetRequestRequestTypeDef",
     {
         "ResourceSetName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetArchitectureRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetArchitectureRecommendationsRequestRequestTypeDef",
     {
         "RecoveryGroupName": str,
     },
 )
 _OptionalGetArchitectureRecommendationsRequestRequestTypeDef = TypedDict(
@@ -294,47 +270,39 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetArchitectureRecommendationsRequestRequestTypeDef(
     _RequiredGetArchitectureRecommendationsRequestRequestTypeDef,
     _OptionalGetArchitectureRecommendationsRequestRequestTypeDef,
 ):
     pass
 
+
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "RecommendationText": str,
     },
 )
 
-_RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef = TypedDict(
-    "_RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
-    {
-        "CellName": str,
-    },
-)
-_OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef = TypedDict(
-    "_OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
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
 
-class GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef(
-    _RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
-    _OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
-):
-    pass
-
 _RequiredGetCellReadinessSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetCellReadinessSummaryRequestRequestTypeDef",
     {
         "CellName": str,
     },
 )
 _OptionalGetCellReadinessSummaryRequestRequestTypeDef = TypedDict(
@@ -342,20 +310,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetCellReadinessSummaryRequestRequestTypeDef(
     _RequiredGetCellReadinessSummaryRequestRequestTypeDef,
     _OptionalGetCellReadinessSummaryRequestRequestTypeDef,
 ):
     pass
 
+
 ReadinessCheckSummaryTypeDef = TypedDict(
     "ReadinessCheckSummaryTypeDef",
     {
         "Readiness": ReadinessType,
         "ReadinessCheckName": str,
     },
     total=False,
@@ -364,54 +334,21 @@
 GetCellRequestRequestTypeDef = TypedDict(
     "GetCellRequestRequestTypeDef",
     {
         "CellName": str,
     },
 )
 
-GetCellResponseTypeDef = TypedDict(
-    "GetCellResponseTypeDef",
-    {
-        "CellArn": str,
-        "CellName": str,
-        "Cells": List[str],
-        "ParentReadinessScopes": List[str],
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetReadinessCheckRequestRequestTypeDef = TypedDict(
     "GetReadinessCheckRequestRequestTypeDef",
     {
         "ReadinessCheckName": str,
     },
 )
 
-_RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef = TypedDict(
-    "_RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
-    {
-        "ReadinessCheckName": str,
-        "ResourceIdentifier": str,
-    },
-)
-_OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef = TypedDict(
-    "_OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef(
-    _RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
-    _OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
-):
-    pass
-
 _RequiredGetReadinessCheckResourceStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetReadinessCheckResourceStatusRequestRequestTypeDef",
     {
         "ReadinessCheckName": str,
         "ResourceIdentifier": str,
     },
 )
@@ -420,50 +357,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetReadinessCheckResourceStatusRequestRequestTypeDef(
     _RequiredGetReadinessCheckResourceStatusRequestRequestTypeDef,
     _OptionalGetReadinessCheckResourceStatusRequestRequestTypeDef,
 ):
     pass
 
-GetReadinessCheckResponseTypeDef = TypedDict(
-    "GetReadinessCheckResponseTypeDef",
-    {
-        "ReadinessCheckArn": str,
-        "ReadinessCheckName": str,
-        "ResourceSet": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef = TypedDict(
-    "_RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
-    {
-        "ReadinessCheckName": str,
-    },
-)
-_OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef = TypedDict(
-    "_OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef(
-    _RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
-    _OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
-):
-    pass
 
 _RequiredGetReadinessCheckStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetReadinessCheckStatusRequestRequestTypeDef",
     {
         "ReadinessCheckName": str,
     },
 )
@@ -472,20 +380,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetReadinessCheckStatusRequestRequestTypeDef(
     _RequiredGetReadinessCheckStatusRequestRequestTypeDef,
     _OptionalGetReadinessCheckStatusRequestRequestTypeDef,
 ):
     pass
 
+
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "MessageText": str,
     },
     total=False,
 )
@@ -502,36 +412,18 @@
     {
         "ComponentId": str,
         "ResourceArn": str,
     },
     total=False,
 )
 
+
 class ResourceResultTypeDef(_RequiredResourceResultTypeDef, _OptionalResourceResultTypeDef):
     pass
 
-_RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef = TypedDict(
-    "_RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
-    {
-        "RecoveryGroupName": str,
-    },
-)
-_OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef = TypedDict(
-    "_OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef(
-    _RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
-    _OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
-):
-    pass
 
 _RequiredGetRecoveryGroupReadinessSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetRecoveryGroupReadinessSummaryRequestRequestTypeDef",
     {
         "RecoveryGroupName": str,
     },
 )
@@ -540,96 +432,54 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetRecoveryGroupReadinessSummaryRequestRequestTypeDef(
     _RequiredGetRecoveryGroupReadinessSummaryRequestRequestTypeDef,
     _OptionalGetRecoveryGroupReadinessSummaryRequestRequestTypeDef,
 ):
     pass
 
+
 GetRecoveryGroupRequestRequestTypeDef = TypedDict(
     "GetRecoveryGroupRequestRequestTypeDef",
     {
         "RecoveryGroupName": str,
     },
 )
 
-GetRecoveryGroupResponseTypeDef = TypedDict(
-    "GetRecoveryGroupResponseTypeDef",
-    {
-        "Cells": List[str],
-        "RecoveryGroupArn": str,
-        "RecoveryGroupName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResourceSetRequestRequestTypeDef = TypedDict(
     "GetResourceSetRequestRequestTypeDef",
     {
         "ResourceSetName": str,
     },
 )
 
-ListCellsRequestListCellsPaginateTypeDef = TypedDict(
-    "ListCellsRequestListCellsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCellsRequestRequestTypeDef = TypedDict(
     "ListCellsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef = TypedDict(
-    "ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCrossAccountAuthorizationsRequestRequestTypeDef = TypedDict(
     "ListCrossAccountAuthorizationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListCrossAccountAuthorizationsResponseTypeDef = TypedDict(
-    "ListCrossAccountAuthorizationsResponseTypeDef",
-    {
-        "CrossAccountAuthorizations": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListReadinessChecksRequestListReadinessChecksPaginateTypeDef = TypedDict(
-    "ListReadinessChecksRequestListReadinessChecksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListReadinessChecksRequestRequestTypeDef = TypedDict(
     "ListReadinessChecksRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -647,26 +497,20 @@
     {
         "ReadinessCheckName": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class ReadinessCheckOutputTypeDef(
     _RequiredReadinessCheckOutputTypeDef, _OptionalReadinessCheckOutputTypeDef
 ):
     pass
 
-ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef = TypedDict(
-    "ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListRecoveryGroupsRequestRequestTypeDef = TypedDict(
     "ListRecoveryGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
@@ -685,26 +529,20 @@
     "_OptionalRecoveryGroupOutputTypeDef",
     {
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class RecoveryGroupOutputTypeDef(
     _RequiredRecoveryGroupOutputTypeDef, _OptionalRecoveryGroupOutputTypeDef
 ):
     pass
 
-ListResourceSetsRequestListResourceSetsPaginateTypeDef = TypedDict(
-    "ListResourceSetsRequestListResourceSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListResourceSetsRequestRequestTypeDef = TypedDict(
     "ListResourceSetsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
@@ -716,23 +554,14 @@
     {
         "ResourceType": str,
         "RuleDescription": str,
         "RuleId": str,
     },
 )
 
-ListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "ListRulesRequestListRulesPaginateTypeDef",
-    {
-        "ResourceType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRulesRequestRequestTypeDef = TypedDict(
     "ListRulesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "ResourceType": str,
     },
@@ -742,60 +571,48 @@
 ListTagsForResourcesRequestRequestTypeDef = TypedDict(
     "ListTagsForResourcesRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourcesResponseTypeDef = TypedDict(
-    "ListTagsForResourcesResponseTypeDef",
+NLBResourceOutputTypeDef = TypedDict(
+    "NLBResourceOutputTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Arn": str,
     },
+    total=False,
 )
 
 NLBResourceTypeDef = TypedDict(
     "NLBResourceTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+R53ResourceRecordOutputTypeDef = TypedDict(
+    "R53ResourceRecordOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "DomainName": str,
+        "RecordSetId": str,
     },
     total=False,
 )
 
 R53ResourceRecordTypeDef = TypedDict(
     "R53ResourceRecordTypeDef",
     {
         "DomainName": str,
         "RecordSetId": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -812,100 +629,338 @@
     "UpdateCellRequestRequestTypeDef",
     {
         "CellName": str,
         "Cells": Sequence[str],
     },
 )
 
-UpdateCellResponseTypeDef = TypedDict(
-    "UpdateCellResponseTypeDef",
+UpdateReadinessCheckRequestRequestTypeDef = TypedDict(
+    "UpdateReadinessCheckRequestRequestTypeDef",
+    {
+        "ReadinessCheckName": str,
+        "ResourceSetName": str,
+    },
+)
+
+UpdateRecoveryGroupRequestRequestTypeDef = TypedDict(
+    "UpdateRecoveryGroupRequestRequestTypeDef",
+    {
+        "Cells": Sequence[str],
+        "RecoveryGroupName": str,
+    },
+)
+
+CreateCellResponseTypeDef = TypedDict(
+    "CreateCellResponseTypeDef",
     {
         "CellArn": str,
         "CellName": str,
         "Cells": List[str],
         "ParentReadinessScopes": List[str],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateReadinessCheckRequestRequestTypeDef = TypedDict(
-    "UpdateReadinessCheckRequestRequestTypeDef",
+CreateCrossAccountAuthorizationResponseTypeDef = TypedDict(
+    "CreateCrossAccountAuthorizationResponseTypeDef",
     {
-        "ReadinessCheckName": str,
-        "ResourceSetName": str,
+        "CrossAccountAuthorization": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateReadinessCheckResponseTypeDef = TypedDict(
-    "UpdateReadinessCheckResponseTypeDef",
+CreateReadinessCheckResponseTypeDef = TypedDict(
+    "CreateReadinessCheckResponseTypeDef",
     {
         "ReadinessCheckArn": str,
         "ReadinessCheckName": str,
         "ResourceSet": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateRecoveryGroupRequestRequestTypeDef = TypedDict(
-    "UpdateRecoveryGroupRequestRequestTypeDef",
+CreateRecoveryGroupResponseTypeDef = TypedDict(
+    "CreateRecoveryGroupResponseTypeDef",
     {
-        "Cells": Sequence[str],
+        "Cells": List[str],
+        "RecoveryGroupArn": str,
         "RecoveryGroupName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateRecoveryGroupResponseTypeDef = TypedDict(
-    "UpdateRecoveryGroupResponseTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCellResponseTypeDef = TypedDict(
+    "GetCellResponseTypeDef",
+    {
+        "CellArn": str,
+        "CellName": str,
+        "Cells": List[str],
+        "ParentReadinessScopes": List[str],
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetReadinessCheckResponseTypeDef = TypedDict(
+    "GetReadinessCheckResponseTypeDef",
+    {
+        "ReadinessCheckArn": str,
+        "ReadinessCheckName": str,
+        "ResourceSet": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRecoveryGroupResponseTypeDef = TypedDict(
+    "GetRecoveryGroupResponseTypeDef",
     {
         "Cells": List[str],
         "RecoveryGroupArn": str,
         "RecoveryGroupName": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCellsResponseTypeDef = TypedDict(
     "ListCellsResponseTypeDef",
     {
         "Cells": List[CellOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCrossAccountAuthorizationsResponseTypeDef = TypedDict(
+    "ListCrossAccountAuthorizationsResponseTypeDef",
+    {
+        "CrossAccountAuthorizations": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourcesResponseTypeDef = TypedDict(
+    "ListTagsForResourcesResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateCellResponseTypeDef = TypedDict(
+    "UpdateCellResponseTypeDef",
+    {
+        "CellArn": str,
+        "CellName": str,
+        "Cells": List[str],
+        "ParentReadinessScopes": List[str],
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateReadinessCheckResponseTypeDef = TypedDict(
+    "UpdateReadinessCheckResponseTypeDef",
+    {
+        "ReadinessCheckArn": str,
+        "ReadinessCheckName": str,
+        "ResourceSet": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRecoveryGroupResponseTypeDef = TypedDict(
+    "UpdateRecoveryGroupResponseTypeDef",
+    {
+        "Cells": List[str],
+        "RecoveryGroupArn": str,
+        "RecoveryGroupName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetArchitectureRecommendationsResponseTypeDef = TypedDict(
     "GetArchitectureRecommendationsResponseTypeDef",
     {
         "LastAuditTimestamp": datetime,
         "NextToken": str,
         "Recommendations": List[RecommendationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef = TypedDict(
+    "_RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
+    {
+        "CellName": str,
+    },
+)
+_OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef = TypedDict(
+    "_OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef(
+    _RequiredGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
+    _OptionalGetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef = TypedDict(
+    "_RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
+    {
+        "ReadinessCheckName": str,
+        "ResourceIdentifier": str,
+    },
+)
+_OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef = TypedDict(
+    "_OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef(
+    _RequiredGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
+    _OptionalGetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef = TypedDict(
+    "_RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
+    {
+        "ReadinessCheckName": str,
+    },
+)
+_OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef = TypedDict(
+    "_OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef(
+    _RequiredGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
+    _OptionalGetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef = TypedDict(
+    "_RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
+    {
+        "RecoveryGroupName": str,
     },
 )
+_OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef = TypedDict(
+    "_OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef(
+    _RequiredGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
+    _OptionalGetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
+):
+    pass
+
+
+ListCellsRequestListCellsPaginateTypeDef = TypedDict(
+    "ListCellsRequestListCellsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef = TypedDict(
+    "ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListReadinessChecksRequestListReadinessChecksPaginateTypeDef = TypedDict(
+    "ListReadinessChecksRequestListReadinessChecksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef = TypedDict(
+    "ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResourceSetsRequestListResourceSetsPaginateTypeDef = TypedDict(
+    "ListResourceSetsRequestListResourceSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "ListRulesRequestListRulesPaginateTypeDef",
+    {
+        "ResourceType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 GetCellReadinessSummaryResponseTypeDef = TypedDict(
     "GetCellReadinessSummaryResponseTypeDef",
     {
         "NextToken": str,
         "Readiness": ReadinessType,
         "ReadinessChecks": List[ReadinessCheckSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecoveryGroupReadinessSummaryResponseTypeDef = TypedDict(
     "GetRecoveryGroupReadinessSummaryResponseTypeDef",
     {
         "NextToken": str,
         "Readiness": ReadinessType,
         "ReadinessChecks": List[ReadinessCheckSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RuleResultTypeDef = TypedDict(
     "RuleResultTypeDef",
     {
         "LastCheckedTimestamp": datetime,
@@ -918,45 +973,54 @@
 GetReadinessCheckStatusResponseTypeDef = TypedDict(
     "GetReadinessCheckStatusResponseTypeDef",
     {
         "Messages": List[MessageTypeDef],
         "NextToken": str,
         "Readiness": ReadinessType,
         "Resources": List[ResourceResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReadinessChecksResponseTypeDef = TypedDict(
     "ListReadinessChecksResponseTypeDef",
     {
         "NextToken": str,
         "ReadinessChecks": List[ReadinessCheckOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecoveryGroupsResponseTypeDef = TypedDict(
     "ListRecoveryGroupsResponseTypeDef",
     {
         "NextToken": str,
         "RecoveryGroups": List[RecoveryGroupOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "NextToken": str,
         "Rules": List[ListRulesOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+TargetResourceOutputTypeDef = TypedDict(
+    "TargetResourceOutputTypeDef",
+    {
+        "NLBResource": NLBResourceOutputTypeDef,
+        "R53Resource": R53ResourceRecordOutputTypeDef,
+    },
+    total=False,
+)
+
 TargetResourceTypeDef = TypedDict(
     "TargetResourceTypeDef",
     {
         "NLBResource": NLBResourceTypeDef,
         "R53Resource": R53ResourceRecordTypeDef,
     },
     total=False,
@@ -964,130 +1028,157 @@
 
 GetReadinessCheckResourceStatusResponseTypeDef = TypedDict(
     "GetReadinessCheckResourceStatusResponseTypeDef",
     {
         "NextToken": str,
         "Readiness": ReadinessType,
         "Rules": List[RuleResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DNSTargetResourceOutputTypeDef = TypedDict(
+    "DNSTargetResourceOutputTypeDef",
+    {
+        "DomainName": str,
+        "HostedZoneArn": str,
+        "RecordSetId": str,
+        "RecordType": str,
+        "TargetResource": TargetResourceOutputTypeDef,
     },
+    total=False,
 )
 
 DNSTargetResourceTypeDef = TypedDict(
     "DNSTargetResourceTypeDef",
     {
         "DomainName": str,
         "HostedZoneArn": str,
         "RecordSetId": str,
         "RecordType": str,
         "TargetResource": TargetResourceTypeDef,
     },
     total=False,
 )
 
-ResourceTypeDef = TypedDict(
-    "ResourceTypeDef",
+ResourceOutputTypeDef = TypedDict(
+    "ResourceOutputTypeDef",
     {
         "ComponentId": str,
-        "DnsTargetResource": DNSTargetResourceTypeDef,
-        "ReadinessScopes": Sequence[str],
+        "DnsTargetResource": DNSTargetResourceOutputTypeDef,
+        "ReadinessScopes": List[str],
         "ResourceArn": str,
     },
     total=False,
 )
 
-_RequiredCreateResourceSetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateResourceSetRequestRequestTypeDef",
-    {
-        "ResourceSetName": str,
-        "ResourceSetType": str,
-        "Resources": Sequence[ResourceTypeDef],
-    },
-)
-_OptionalCreateResourceSetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateResourceSetRequestRequestTypeDef",
+ResourceTypeDef = TypedDict(
+    "ResourceTypeDef",
     {
-        "Tags": Mapping[str, str],
+        "ComponentId": str,
+        "DnsTargetResource": DNSTargetResourceTypeDef,
+        "ReadinessScopes": Sequence[str],
+        "ResourceArn": str,
     },
     total=False,
 )
 
-class CreateResourceSetRequestRequestTypeDef(
-    _RequiredCreateResourceSetRequestRequestTypeDef, _OptionalCreateResourceSetRequestRequestTypeDef
-):
-    pass
-
 CreateResourceSetResponseTypeDef = TypedDict(
     "CreateResourceSetResponseTypeDef",
     {
         "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": List[ResourceTypeDef],
+        "Resources": List[ResourceOutputTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceSetResponseTypeDef = TypedDict(
     "GetResourceSetResponseTypeDef",
     {
         "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": List[ResourceTypeDef],
+        "Resources": List[ResourceOutputTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredResourceSetOutputTypeDef = TypedDict(
     "_RequiredResourceSetOutputTypeDef",
     {
         "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": List[ResourceTypeDef],
+        "Resources": List[ResourceOutputTypeDef],
     },
 )
 _OptionalResourceSetOutputTypeDef = TypedDict(
     "_OptionalResourceSetOutputTypeDef",
     {
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class ResourceSetOutputTypeDef(
     _RequiredResourceSetOutputTypeDef, _OptionalResourceSetOutputTypeDef
 ):
     pass
 
-UpdateResourceSetRequestRequestTypeDef = TypedDict(
-    "UpdateResourceSetRequestRequestTypeDef",
+
+UpdateResourceSetResponseTypeDef = TypedDict(
+    "UpdateResourceSetResponseTypeDef",
+    {
+        "ResourceSetArn": str,
+        "ResourceSetName": str,
+        "ResourceSetType": str,
+        "Resources": List[ResourceOutputTypeDef],
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateResourceSetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateResourceSetRequestRequestTypeDef",
     {
         "ResourceSetName": str,
         "ResourceSetType": str,
         "Resources": Sequence[ResourceTypeDef],
     },
 )
+_OptionalCreateResourceSetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateResourceSetRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
 
-UpdateResourceSetResponseTypeDef = TypedDict(
-    "UpdateResourceSetResponseTypeDef",
+
+class CreateResourceSetRequestRequestTypeDef(
+    _RequiredCreateResourceSetRequestRequestTypeDef, _OptionalCreateResourceSetRequestRequestTypeDef
+):
+    pass
+
+
+UpdateResourceSetRequestRequestTypeDef = TypedDict(
+    "UpdateResourceSetRequestRequestTypeDef",
     {
-        "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": List[ResourceTypeDef],
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Resources": Sequence[ResourceTypeDef],
     },
 )
 
 ListResourceSetsResponseTypeDef = TypedDict(
     "ListResourceSetsResponseTypeDef",
     {
         "NextToken": str,
         "ResourceSets": List[ResourceSetOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness.egg-info/PKG-INFO` & `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53-recovery-readiness
-Version: 1.28.0
-Summary: Type annotations for boto3.Route53RecoveryReadiness 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Route53RecoveryReadiness 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-route53-recovery-readiness"></a>
 
 # mypy-boto3-route53-recovery-readiness
 
 [![PyPI - mypy-boto3-route53-recovery-readiness](https://img.shields.io/pypi/v/mypy-boto3-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-readiness)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-readiness)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53-recovery-readiness?color=blue)](https://pypistats.org/packages/mypy-boto3-route53-recovery-readiness)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53-recovery-readiness)](https://pepy.tech/project/mypy-boto3-route53-recovery-readiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryReadiness 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
+[boto3.Route53RecoveryReadiness 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
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
 [mypy-boto3-route53-recovery-readiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/).
 
 See how it helps to find and fix potential bugs:
 
@@ -365,96 +365,101 @@
 `mypy_boto3_route53_recovery_readiness.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53_recovery_readiness.type_defs import (
     CellOutputTypeDef,
     CreateCellRequestRequestTypeDef,
-    CreateCellResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateCrossAccountAuthorizationRequestRequestTypeDef,
-    CreateCrossAccountAuthorizationResponseTypeDef,
     CreateReadinessCheckRequestRequestTypeDef,
-    CreateReadinessCheckResponseTypeDef,
     CreateRecoveryGroupRequestRequestTypeDef,
-    CreateRecoveryGroupResponseTypeDef,
     DeleteCellRequestRequestTypeDef,
     DeleteCrossAccountAuthorizationRequestRequestTypeDef,
     DeleteReadinessCheckRequestRequestTypeDef,
     DeleteRecoveryGroupRequestRequestTypeDef,
     DeleteResourceSetRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetArchitectureRecommendationsRequestRequestTypeDef,
     RecommendationTypeDef,
-    GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetCellReadinessSummaryRequestRequestTypeDef,
     ReadinessCheckSummaryTypeDef,
     GetCellRequestRequestTypeDef,
-    GetCellResponseTypeDef,
     GetReadinessCheckRequestRequestTypeDef,
-    GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
     GetReadinessCheckResourceStatusRequestRequestTypeDef,
-    GetReadinessCheckResponseTypeDef,
-    GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
     GetReadinessCheckStatusRequestRequestTypeDef,
     MessageTypeDef,
     ResourceResultTypeDef,
-    GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
     GetRecoveryGroupReadinessSummaryRequestRequestTypeDef,
     GetRecoveryGroupRequestRequestTypeDef,
-    GetRecoveryGroupResponseTypeDef,
     GetResourceSetRequestRequestTypeDef,
-    ListCellsRequestListCellsPaginateTypeDef,
     ListCellsRequestRequestTypeDef,
-    ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef,
     ListCrossAccountAuthorizationsRequestRequestTypeDef,
-    ListCrossAccountAuthorizationsResponseTypeDef,
-    ListReadinessChecksRequestListReadinessChecksPaginateTypeDef,
     ListReadinessChecksRequestRequestTypeDef,
     ReadinessCheckOutputTypeDef,
-    ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef,
     ListRecoveryGroupsRequestRequestTypeDef,
     RecoveryGroupOutputTypeDef,
-    ListResourceSetsRequestListResourceSetsPaginateTypeDef,
     ListResourceSetsRequestRequestTypeDef,
     ListRulesOutputTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     ListTagsForResourcesRequestRequestTypeDef,
-    ListTagsForResourcesResponseTypeDef,
+    NLBResourceOutputTypeDef,
     NLBResourceTypeDef,
-    PaginatorConfigTypeDef,
+    R53ResourceRecordOutputTypeDef,
     R53ResourceRecordTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCellRequestRequestTypeDef,
-    UpdateCellResponseTypeDef,
     UpdateReadinessCheckRequestRequestTypeDef,
-    UpdateReadinessCheckResponseTypeDef,
     UpdateRecoveryGroupRequestRequestTypeDef,
-    UpdateRecoveryGroupResponseTypeDef,
+    CreateCellResponseTypeDef,
+    CreateCrossAccountAuthorizationResponseTypeDef,
+    CreateReadinessCheckResponseTypeDef,
+    CreateRecoveryGroupResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCellResponseTypeDef,
+    GetReadinessCheckResponseTypeDef,
+    GetRecoveryGroupResponseTypeDef,
     ListCellsResponseTypeDef,
+    ListCrossAccountAuthorizationsResponseTypeDef,
+    ListTagsForResourcesResponseTypeDef,
+    UpdateCellResponseTypeDef,
+    UpdateReadinessCheckResponseTypeDef,
+    UpdateRecoveryGroupResponseTypeDef,
     GetArchitectureRecommendationsResponseTypeDef,
+    GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef,
+    GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef,
+    GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef,
+    GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef,
+    ListCellsRequestListCellsPaginateTypeDef,
+    ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef,
+    ListReadinessChecksRequestListReadinessChecksPaginateTypeDef,
+    ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef,
+    ListResourceSetsRequestListResourceSetsPaginateTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
     GetCellReadinessSummaryResponseTypeDef,
     GetRecoveryGroupReadinessSummaryResponseTypeDef,
     RuleResultTypeDef,
     GetReadinessCheckStatusResponseTypeDef,
     ListReadinessChecksResponseTypeDef,
     ListRecoveryGroupsResponseTypeDef,
     ListRulesResponseTypeDef,
+    TargetResourceOutputTypeDef,
     TargetResourceTypeDef,
     GetReadinessCheckResourceStatusResponseTypeDef,
+    DNSTargetResourceOutputTypeDef,
     DNSTargetResourceTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
-    CreateResourceSetRequestRequestTypeDef,
     CreateResourceSetResponseTypeDef,
     GetResourceSetResponseTypeDef,
     ResourceSetOutputTypeDef,
-    UpdateResourceSetRequestRequestTypeDef,
     UpdateResourceSetResponseTypeDef,
+    CreateResourceSetRequestRequestTypeDef,
+    UpdateResourceSetRequestRequestTypeDef,
     ListResourceSetsResponseTypeDef,
 )
 
 
 def get_structure() -> CellOutputTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.0/mypy_boto3_route53_recovery_readiness.egg-info/SOURCES.txt` & `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.0/setup.py` & `mypy-boto3-route53-recovery-readiness-1.28.12/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53-recovery-readiness",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_route53_recovery_readiness"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Route53RecoveryReadiness 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Route53RecoveryReadiness 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

