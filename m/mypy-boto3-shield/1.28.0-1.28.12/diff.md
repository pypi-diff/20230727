# Comparing `tmp/mypy-boto3-shield-1.28.0.tar.gz` & `tmp/mypy-boto3-shield-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-shield-1.28.0.tar", last modified: Thu Jul  6 21:00:39 2023, max compression
+gzip compressed data, was "mypy-boto3-shield-1.28.12.tar", last modified: Thu Jul 27 11:49:39 2023, max compression
```

## Comparing `mypy-boto3-shield-1.28.0.tar` & `mypy-boto3-shield-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:39.030434 mypy-boto3-shield-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:55:54.000000 mypy-boto3-shield-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-07-06 21:00:39.026434 mypy-boto3-shield-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14280 2023-07-06 20:55:54.000000 mypy-boto3-shield-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:39.022434 mypy-boto3-shield-1.28.0/mypy_boto3_shield/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-06 20:55:54.000000 mypy-boto3-shield-1.28.0/mypy_boto3_shield/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-06 20:55:54.000000 mypy-boto3-shield-1.28.0/mypy_boto3_shield/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-06 20:55:54.000000 mypy-boto3-shield-1.28.0/mypy_boto3_shield/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25575 2023-07-06 20:55:58.000000 mypy-boto3-shield-1.28.0/mypy_boto3_shield/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25530 2023-07-06 20:55:54.000000 mypy-boto3-shield-1.28.0/mypy_boto3_shield/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-07-06 20:55:58.000000 mypy-boto3-shield-1.28.0/mypy_boto3_shield/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-06 20:55:58.000000 mypy-boto3-shield-1.28.0/mypy_boto3_shield/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-06 20:55:58.000000 mypy-boto3-shield-1.28.0/mypy_boto3_shield/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-06 20:55:58.000000 mypy-boto3-shield-1.28.0/mypy_boto3_shield/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:55:54.000000 mypy-boto3-shield-1.28.0/mypy_boto3_shield/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-07-06 20:55:59.000000 mypy-boto3-shield-1.28.0/mypy_boto3_shield/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22168 2023-07-06 20:55:58.000000 mypy-boto3-shield-1.28.0/mypy_boto3_shield/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:55:54.000000 mypy-boto3-shield-1.28.0/mypy_boto3_shield/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:39.026434 mypy-boto3-shield-1.28.0/mypy_boto3_shield.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-07-06 21:00:38.000000 mypy-boto3-shield-1.28.0/mypy_boto3_shield.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-06 21:00:38.000000 mypy-boto3-shield-1.28.0/mypy_boto3_shield.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:38.000000 mypy-boto3-shield-1.28.0/mypy_boto3_shield.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:38.000000 mypy-boto3-shield-1.28.0/mypy_boto3_shield.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:38.000000 mypy-boto3-shield-1.28.0/mypy_boto3_shield.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 21:00:38.000000 mypy-boto3-shield-1.28.0/mypy_boto3_shield.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:39.030434 mypy-boto3-shield-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-06 20:55:54.000000 mypy-boto3-shield-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:39.525300 mypy-boto3-shield-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-07-27 11:49:39.525300 mypy-boto3-shield-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14389 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:39.521300 mypy-boto3-shield-1.28.12/mypy_boto3_shield/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25575 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25530 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-07-27 11:46:59.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-07-27 11:46:59.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23299 2023-07-27 11:46:59.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23278 2023-07-27 11:46:59.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:39.525300 mypy-boto3-shield-1.28.12/mypy_boto3_shield.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-07-27 11:49:39.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 11:49:39.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:39.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:39.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:39.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 11:49:39.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:39.525300 mypy-boto3-shield-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 11:46:56.000000 mypy-boto3-shield-1.28.12/setup.py
```

### Comparing `mypy-boto3-shield-1.28.0/LICENSE` & `mypy-boto3-shield-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.0/PKG-INFO` & `mypy-boto3-shield-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-shield
-Version: 1.28.0
-Summary: Type annotations for boto3.Shield 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Shield 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-shield"></a>
 
 # mypy-boto3-shield
 
 [![PyPI - mypy-boto3-shield](https://img.shields.io/pypi/v/mypy-boto3-shield.svg?color=blue)](https://pypi.org/project/mypy-boto3-shield)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-shield.svg?color=blue)](https://pypi.org/project/mypy-boto3-shield)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-shield?color=blue)](https://pypistats.org/packages/mypy-boto3-shield)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-shield)](https://pepy.tech/project/mypy-boto3-shield)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Shield 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
+[boto3.Shield 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
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
 [mypy-boto3-shield docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,72 +330,76 @@
 ### Typed dictionaries
 
 `mypy_boto3_shield.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_shield.type_defs import (
-    ResponseActionTypeDef,
+    ResponseActionOutputTypeDef,
     AssociateDRTLogBucketRequestRequestTypeDef,
     AssociateDRTRoleRequestRequestTypeDef,
     AssociateHealthCheckRequestRequestTypeDef,
     EmergencyContactTypeDef,
     MitigationTypeDef,
     SummarizedCounterTypeDef,
     ContributorTypeDef,
     AttackVectorDescriptionTypeDef,
     AttackVolumeStatisticsTypeDef,
     TagTypeDef,
-    CreateProtectionResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteProtectionGroupRequestRequestTypeDef,
     DeleteProtectionRequestRequestTypeDef,
     DescribeAttackRequestRequestTypeDef,
-    TimeRangeTypeDef,
-    DescribeDRTAccessResponseTypeDef,
+    TimeRangeOutputTypeDef,
+    EmergencyContactOutputTypeDef,
     DescribeProtectionGroupRequestRequestTypeDef,
     ProtectionGroupTypeDef,
     DescribeProtectionRequestRequestTypeDef,
     DisableApplicationLayerAutomaticResponseRequestRequestTypeDef,
     DisassociateDRTLogBucketRequestRequestTypeDef,
     DisassociateHealthCheckRequestRequestTypeDef,
-    GetSubscriptionStateResponseTypeDef,
+    ResponseActionTypeDef,
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     LimitTypeDef,
+    PaginatorConfigTypeDef,
+    TimeRangeTypeDef,
     ListResourcesInProtectionGroupRequestRequestTypeDef,
-    ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     ProtectionGroupArbitraryPatternLimitsTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProtectionGroupRequestRequestTypeDef,
     UpdateSubscriptionRequestRequestTypeDef,
     ApplicationLayerAutomaticResponseConfigurationTypeDef,
-    EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
-    UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
     AssociateProactiveEngagementDetailsRequestRequestTypeDef,
-    DescribeEmergencyContactSettingsResponseTypeDef,
     UpdateEmergencyContactSettingsRequestRequestTypeDef,
     SummarizedAttackVectorTypeDef,
     AttackPropertyTypeDef,
     AttackSummaryTypeDef,
     AttackVolumeTypeDef,
     CreateProtectionGroupRequestRequestTypeDef,
     CreateProtectionRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    ListAttacksRequestListAttacksPaginateTypeDef,
-    ListAttacksRequestRequestTypeDef,
+    CreateProtectionResponseTypeDef,
+    DescribeDRTAccessResponseTypeDef,
+    GetSubscriptionStateResponseTypeDef,
+    ListResourcesInProtectionGroupResponseTypeDef,
+    DescribeEmergencyContactSettingsResponseTypeDef,
     DescribeProtectionGroupResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
-    ListProtectionsRequestListProtectionsPaginateTypeDef,
+    EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
+    UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
     ListProtectionsRequestRequestTypeDef,
     ListProtectionGroupsRequestRequestTypeDef,
     ProtectionLimitsTypeDef,
+    ListProtectionsRequestListProtectionsPaginateTypeDef,
+    ListAttacksRequestListAttacksPaginateTypeDef,
+    ListAttacksRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ProtectionGroupPatternTypeLimitsTypeDef,
     ProtectionTypeDef,
     SubResourceSummaryTypeDef,
     ListAttacksResponseTypeDef,
     AttackStatisticsDataItemTypeDef,
     ProtectionGroupLimitsTypeDef,
     DescribeProtectionResponseTypeDef,
@@ -405,15 +409,15 @@
     SubscriptionLimitsTypeDef,
     DescribeAttackResponseTypeDef,
     SubscriptionTypeDef,
     DescribeSubscriptionResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseActionTypeDef:
+def get_structure() -> ResponseActionOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-shield-1.28.0/README.md` & `mypy-boto3-shield-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-shield"></a>
 
 # mypy-boto3-shield
 
 [![PyPI - mypy-boto3-shield](https://img.shields.io/pypi/v/mypy-boto3-shield.svg?color=blue)](https://pypi.org/project/mypy-boto3-shield)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-shield.svg?color=blue)](https://pypi.org/project/mypy-boto3-shield)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-shield?color=blue)](https://pypistats.org/packages/mypy-boto3-shield)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-shield)](https://pepy.tech/project/mypy-boto3-shield)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Shield 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
+[boto3.Shield 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
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
 [mypy-boto3-shield docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,72 +298,76 @@
 ### Typed dictionaries
 
 `mypy_boto3_shield.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_shield.type_defs import (
-    ResponseActionTypeDef,
+    ResponseActionOutputTypeDef,
     AssociateDRTLogBucketRequestRequestTypeDef,
     AssociateDRTRoleRequestRequestTypeDef,
     AssociateHealthCheckRequestRequestTypeDef,
     EmergencyContactTypeDef,
     MitigationTypeDef,
     SummarizedCounterTypeDef,
     ContributorTypeDef,
     AttackVectorDescriptionTypeDef,
     AttackVolumeStatisticsTypeDef,
     TagTypeDef,
-    CreateProtectionResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteProtectionGroupRequestRequestTypeDef,
     DeleteProtectionRequestRequestTypeDef,
     DescribeAttackRequestRequestTypeDef,
-    TimeRangeTypeDef,
-    DescribeDRTAccessResponseTypeDef,
+    TimeRangeOutputTypeDef,
+    EmergencyContactOutputTypeDef,
     DescribeProtectionGroupRequestRequestTypeDef,
     ProtectionGroupTypeDef,
     DescribeProtectionRequestRequestTypeDef,
     DisableApplicationLayerAutomaticResponseRequestRequestTypeDef,
     DisassociateDRTLogBucketRequestRequestTypeDef,
     DisassociateHealthCheckRequestRequestTypeDef,
-    GetSubscriptionStateResponseTypeDef,
+    ResponseActionTypeDef,
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     LimitTypeDef,
+    PaginatorConfigTypeDef,
+    TimeRangeTypeDef,
     ListResourcesInProtectionGroupRequestRequestTypeDef,
-    ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     ProtectionGroupArbitraryPatternLimitsTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProtectionGroupRequestRequestTypeDef,
     UpdateSubscriptionRequestRequestTypeDef,
     ApplicationLayerAutomaticResponseConfigurationTypeDef,
-    EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
-    UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
     AssociateProactiveEngagementDetailsRequestRequestTypeDef,
-    DescribeEmergencyContactSettingsResponseTypeDef,
     UpdateEmergencyContactSettingsRequestRequestTypeDef,
     SummarizedAttackVectorTypeDef,
     AttackPropertyTypeDef,
     AttackSummaryTypeDef,
     AttackVolumeTypeDef,
     CreateProtectionGroupRequestRequestTypeDef,
     CreateProtectionRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    ListAttacksRequestListAttacksPaginateTypeDef,
-    ListAttacksRequestRequestTypeDef,
+    CreateProtectionResponseTypeDef,
+    DescribeDRTAccessResponseTypeDef,
+    GetSubscriptionStateResponseTypeDef,
+    ListResourcesInProtectionGroupResponseTypeDef,
+    DescribeEmergencyContactSettingsResponseTypeDef,
     DescribeProtectionGroupResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
-    ListProtectionsRequestListProtectionsPaginateTypeDef,
+    EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
+    UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
     ListProtectionsRequestRequestTypeDef,
     ListProtectionGroupsRequestRequestTypeDef,
     ProtectionLimitsTypeDef,
+    ListProtectionsRequestListProtectionsPaginateTypeDef,
+    ListAttacksRequestListAttacksPaginateTypeDef,
+    ListAttacksRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ProtectionGroupPatternTypeLimitsTypeDef,
     ProtectionTypeDef,
     SubResourceSummaryTypeDef,
     ListAttacksResponseTypeDef,
     AttackStatisticsDataItemTypeDef,
     ProtectionGroupLimitsTypeDef,
     DescribeProtectionResponseTypeDef,
@@ -373,15 +377,15 @@
     SubscriptionLimitsTypeDef,
     DescribeAttackResponseTypeDef,
     SubscriptionTypeDef,
     DescribeSubscriptionResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseActionTypeDef:
+def get_structure() -> ResponseActionOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-shield-1.28.0/mypy_boto3_shield/__init__.py` & `mypy-boto3-shield-1.28.12/mypy_boto3_shield/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.0/mypy_boto3_shield/__init__.pyi` & `mypy-boto3-shield-1.28.12/mypy_boto3_shield/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.0/mypy_boto3_shield/__main__.py` & `mypy-boto3-shield-1.28.12/mypy_boto3_shield/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Shield 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Shield 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield\nOther"
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

### Comparing `mypy-boto3-shield-1.28.0/mypy_boto3_shield/client.py` & `mypy-boto3-shield-1.28.12/mypy_boto3_shield/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.0/mypy_boto3_shield/client.pyi` & `mypy-boto3-shield-1.28.12/mypy_boto3_shield/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.0/mypy_boto3_shield/literals.py` & `mypy-boto3-shield-1.28.12/mypy_boto3_shield/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,14 +185,15 @@
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
@@ -271,26 +272,28 @@
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

### Comparing `mypy-boto3-shield-1.28.0/mypy_boto3_shield/literals.pyi` & `mypy-boto3-shield-1.28.12/mypy_boto3_shield/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -183,14 +183,15 @@
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
@@ -269,26 +270,28 @@
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

### Comparing `mypy-boto3-shield-1.28.0/mypy_boto3_shield/paginator.py` & `mypy-boto3-shield-1.28.12/mypy_boto3_shield/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
     def paginate(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
         StartTime: TimeRangeTypeDef = ...,
         EndTime: TimeRangeTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAttacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listattackspaginator)
         """
 
 
@@ -72,13 +72,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listprotectionspaginator)
     """
 
     def paginate(
         self,
         *,
         InclusionFilters: InclusionProtectionFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProtectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListProtections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listprotectionspaginator)
         """
```

### Comparing `mypy-boto3-shield-1.28.0/mypy_boto3_shield/paginator.pyi` & `mypy-boto3-shield-1.28.12/mypy_boto3_shield/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     def paginate(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
         StartTime: TimeRangeTypeDef = ...,
         EndTime: TimeRangeTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAttacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listattackspaginator)
         """
 
 class ListProtectionsPaginator(Paginator):
@@ -68,13 +68,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listprotectionspaginator)
     """
 
     def paginate(
         self,
         *,
         InclusionFilters: InclusionProtectionFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProtectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListProtections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listprotectionspaginator)
         """
```

### Comparing `mypy-boto3-shield-1.28.0/mypy_boto3_shield/type_defs.py` & `mypy-boto3-shield-1.28.12/mypy_boto3_shield/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for shield service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_shield.type_defs import ResponseActionTypeDef
+    from mypy_boto3_shield.type_defs import ResponseActionOutputTypeDef
 
-    data: ResponseActionTypeDef = {...}
+    data: ResponseActionOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ApplicationLayerAutomaticResponseStatusType,
     AttackLayerType,
     AttackPropertyIdentifierType,
     AutoRenewType,
     ProactiveEngagementStatusType,
@@ -32,72 +32,76 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ResponseActionTypeDef",
+    "ResponseActionOutputTypeDef",
     "AssociateDRTLogBucketRequestRequestTypeDef",
     "AssociateDRTRoleRequestRequestTypeDef",
     "AssociateHealthCheckRequestRequestTypeDef",
     "EmergencyContactTypeDef",
     "MitigationTypeDef",
     "SummarizedCounterTypeDef",
     "ContributorTypeDef",
     "AttackVectorDescriptionTypeDef",
     "AttackVolumeStatisticsTypeDef",
     "TagTypeDef",
-    "CreateProtectionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteProtectionGroupRequestRequestTypeDef",
     "DeleteProtectionRequestRequestTypeDef",
     "DescribeAttackRequestRequestTypeDef",
-    "TimeRangeTypeDef",
-    "DescribeDRTAccessResponseTypeDef",
+    "TimeRangeOutputTypeDef",
+    "EmergencyContactOutputTypeDef",
     "DescribeProtectionGroupRequestRequestTypeDef",
     "ProtectionGroupTypeDef",
     "DescribeProtectionRequestRequestTypeDef",
     "DisableApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "DisassociateDRTLogBucketRequestRequestTypeDef",
     "DisassociateHealthCheckRequestRequestTypeDef",
-    "GetSubscriptionStateResponseTypeDef",
+    "ResponseActionTypeDef",
     "InclusionProtectionFiltersTypeDef",
     "InclusionProtectionGroupFiltersTypeDef",
     "LimitTypeDef",
+    "PaginatorConfigTypeDef",
+    "TimeRangeTypeDef",
     "ListResourcesInProtectionGroupRequestRequestTypeDef",
-    "ListResourcesInProtectionGroupResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProtectionGroupRequestRequestTypeDef",
     "UpdateSubscriptionRequestRequestTypeDef",
     "ApplicationLayerAutomaticResponseConfigurationTypeDef",
-    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
-    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "AssociateProactiveEngagementDetailsRequestRequestTypeDef",
-    "DescribeEmergencyContactSettingsResponseTypeDef",
     "UpdateEmergencyContactSettingsRequestRequestTypeDef",
     "SummarizedAttackVectorTypeDef",
     "AttackPropertyTypeDef",
     "AttackSummaryTypeDef",
     "AttackVolumeTypeDef",
     "CreateProtectionGroupRequestRequestTypeDef",
     "CreateProtectionRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "ListAttacksRequestListAttacksPaginateTypeDef",
-    "ListAttacksRequestRequestTypeDef",
+    "CreateProtectionResponseTypeDef",
+    "DescribeDRTAccessResponseTypeDef",
+    "GetSubscriptionStateResponseTypeDef",
+    "ListResourcesInProtectionGroupResponseTypeDef",
+    "DescribeEmergencyContactSettingsResponseTypeDef",
     "DescribeProtectionGroupResponseTypeDef",
     "ListProtectionGroupsResponseTypeDef",
-    "ListProtectionsRequestListProtectionsPaginateTypeDef",
+    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
+    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "ListProtectionsRequestRequestTypeDef",
     "ListProtectionGroupsRequestRequestTypeDef",
     "ProtectionLimitsTypeDef",
+    "ListProtectionsRequestListProtectionsPaginateTypeDef",
+    "ListAttacksRequestListAttacksPaginateTypeDef",
+    "ListAttacksRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ProtectionGroupPatternTypeLimitsTypeDef",
     "ProtectionTypeDef",
     "SubResourceSummaryTypeDef",
     "ListAttacksResponseTypeDef",
     "AttackStatisticsDataItemTypeDef",
     "ProtectionGroupLimitsTypeDef",
     "DescribeProtectionResponseTypeDef",
@@ -106,16 +110,16 @@
     "DescribeAttackStatisticsResponseTypeDef",
     "SubscriptionLimitsTypeDef",
     "DescribeAttackResponseTypeDef",
     "SubscriptionTypeDef",
     "DescribeSubscriptionResponseTypeDef",
 )
 
-ResponseActionTypeDef = TypedDict(
-    "ResponseActionTypeDef",
+ResponseActionOutputTypeDef = TypedDict(
+    "ResponseActionOutputTypeDef",
     {
         "Block": Dict[str, Any],
         "Count": Dict[str, Any],
     },
     total=False,
 )
 
@@ -210,19 +214,22 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-CreateProtectionResponseTypeDef = TypedDict(
-    "CreateProtectionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ProtectionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteProtectionGroupRequestRequestTypeDef = TypedDict(
     "DeleteProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
@@ -239,32 +246,45 @@
 DescribeAttackRequestRequestTypeDef = TypedDict(
     "DescribeAttackRequestRequestTypeDef",
     {
         "AttackId": str,
     },
 )
 
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
+TimeRangeOutputTypeDef = TypedDict(
+    "TimeRangeOutputTypeDef",
     {
         "FromInclusive": datetime,
         "ToExclusive": datetime,
     },
     total=False,
 )
 
-DescribeDRTAccessResponseTypeDef = TypedDict(
-    "DescribeDRTAccessResponseTypeDef",
+_RequiredEmergencyContactOutputTypeDef = TypedDict(
+    "_RequiredEmergencyContactOutputTypeDef",
     {
-        "RoleArn": str,
-        "LogBucketList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EmailAddress": str,
+    },
+)
+_OptionalEmergencyContactOutputTypeDef = TypedDict(
+    "_OptionalEmergencyContactOutputTypeDef",
+    {
+        "PhoneNumber": str,
+        "ContactNotes": str,
     },
+    total=False,
 )
 
+
+class EmergencyContactOutputTypeDef(
+    _RequiredEmergencyContactOutputTypeDef, _OptionalEmergencyContactOutputTypeDef
+):
+    pass
+
+
 DescribeProtectionGroupRequestRequestTypeDef = TypedDict(
     "DescribeProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
     },
 )
 
@@ -318,20 +338,21 @@
     "DisassociateHealthCheckRequestRequestTypeDef",
     {
         "ProtectionId": str,
         "HealthCheckArn": str,
     },
 )
 
-GetSubscriptionStateResponseTypeDef = TypedDict(
-    "GetSubscriptionStateResponseTypeDef",
+ResponseActionTypeDef = TypedDict(
+    "ResponseActionTypeDef",
     {
-        "SubscriptionState": SubscriptionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Block": Mapping[str, Any],
+        "Count": Mapping[str, Any],
     },
+    total=False,
 )
 
 InclusionProtectionFiltersTypeDef = TypedDict(
     "InclusionProtectionFiltersTypeDef",
     {
         "ResourceArns": Sequence[str],
         "ProtectionNames": Sequence[str],
@@ -356,14 +377,33 @@
     {
         "Type": str,
         "Max": int,
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
+TimeRangeTypeDef = TypedDict(
+    "TimeRangeTypeDef",
+    {
+        "FromInclusive": Union[datetime, str],
+        "ToExclusive": Union[datetime, str],
+    },
+    total=False,
+)
+
 _RequiredListResourcesInProtectionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesInProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
     },
 )
 _OptionalListResourcesInProtectionGroupRequestRequestTypeDef = TypedDict(
@@ -379,58 +419,37 @@
 class ListResourcesInProtectionGroupRequestRequestTypeDef(
     _RequiredListResourcesInProtectionGroupRequestRequestTypeDef,
     _OptionalListResourcesInProtectionGroupRequestRequestTypeDef,
 ):
     pass
 
 
-ListResourcesInProtectionGroupResponseTypeDef = TypedDict(
-    "ListResourcesInProtectionGroupResponseTypeDef",
-    {
-        "ResourceArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 
 ProtectionGroupArbitraryPatternLimitsTypeDef = TypedDict(
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
     {
         "MaxMembers": int,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -468,49 +487,25 @@
     total=False,
 )
 
 ApplicationLayerAutomaticResponseConfigurationTypeDef = TypedDict(
     "ApplicationLayerAutomaticResponseConfigurationTypeDef",
     {
         "Status": ApplicationLayerAutomaticResponseStatusType,
-        "Action": ResponseActionTypeDef,
-    },
-)
-
-EnableApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
-    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Action": ResponseActionTypeDef,
-    },
-)
-
-UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
-    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Action": ResponseActionTypeDef,
+        "Action": ResponseActionOutputTypeDef,
     },
 )
 
 AssociateProactiveEngagementDetailsRequestRequestTypeDef = TypedDict(
     "AssociateProactiveEngagementDetailsRequestRequestTypeDef",
     {
         "EmergencyContactList": Sequence[EmergencyContactTypeDef],
     },
 )
 
-DescribeEmergencyContactSettingsResponseTypeDef = TypedDict(
-    "DescribeEmergencyContactSettingsResponseTypeDef",
-    {
-        "EmergencyContactList": List[EmergencyContactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateEmergencyContactSettingsRequestRequestTypeDef = TypedDict(
     "UpdateEmergencyContactSettingsRequestRequestTypeDef",
     {
         "EmergencyContactList": Sequence[EmergencyContactTypeDef],
     },
     total=False,
 )
@@ -614,77 +609,95 @@
 
 class CreateProtectionRequestRequestTypeDef(
     _RequiredCreateProtectionRequestRequestTypeDef, _OptionalCreateProtectionRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-ListAttacksRequestListAttacksPaginateTypeDef = TypedDict(
-    "ListAttacksRequestListAttacksPaginateTypeDef",
+CreateProtectionResponseTypeDef = TypedDict(
+    "CreateProtectionResponseTypeDef",
     {
-        "ResourceArns": Sequence[str],
-        "StartTime": TimeRangeTypeDef,
-        "EndTime": TimeRangeTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ProtectionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ListAttacksRequestRequestTypeDef = TypedDict(
-    "ListAttacksRequestRequestTypeDef",
+DescribeDRTAccessResponseTypeDef = TypedDict(
+    "DescribeDRTAccessResponseTypeDef",
     {
-        "ResourceArns": Sequence[str],
-        "StartTime": TimeRangeTypeDef,
-        "EndTime": TimeRangeTypeDef,
+        "RoleArn": str,
+        "LogBucketList": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSubscriptionStateResponseTypeDef = TypedDict(
+    "GetSubscriptionStateResponseTypeDef",
+    {
+        "SubscriptionState": SubscriptionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListResourcesInProtectionGroupResponseTypeDef = TypedDict(
+    "ListResourcesInProtectionGroupResponseTypeDef",
+    {
+        "ResourceArns": List[str],
         "NextToken": str,
-        "MaxResults": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEmergencyContactSettingsResponseTypeDef = TypedDict(
+    "DescribeEmergencyContactSettingsResponseTypeDef",
+    {
+        "EmergencyContactList": List[EmergencyContactOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DescribeProtectionGroupResponseTypeDef = TypedDict(
     "DescribeProtectionGroupResponseTypeDef",
     {
         "ProtectionGroup": ProtectionGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProtectionGroupsResponseTypeDef = TypedDict(
     "ListProtectionGroupsResponseTypeDef",
     {
         "ProtectionGroups": List[ProtectionGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListProtectionsRequestListProtectionsPaginateTypeDef = TypedDict(
-    "ListProtectionsRequestListProtectionsPaginateTypeDef",
+EnableApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
+    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
     {
-        "InclusionFilters": InclusionProtectionFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ResourceArn": str,
+        "Action": ResponseActionTypeDef,
+    },
+)
+
+UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
+    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Action": ResponseActionTypeDef,
     },
-    total=False,
 )
 
 ListProtectionsRequestRequestTypeDef = TypedDict(
     "ListProtectionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -706,14 +719,54 @@
 ProtectionLimitsTypeDef = TypedDict(
     "ProtectionLimitsTypeDef",
     {
         "ProtectedResourceTypeLimits": List[LimitTypeDef],
     },
 )
 
+ListProtectionsRequestListProtectionsPaginateTypeDef = TypedDict(
+    "ListProtectionsRequestListProtectionsPaginateTypeDef",
+    {
+        "InclusionFilters": InclusionProtectionFiltersTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAttacksRequestListAttacksPaginateTypeDef = TypedDict(
+    "ListAttacksRequestListAttacksPaginateTypeDef",
+    {
+        "ResourceArns": Sequence[str],
+        "StartTime": TimeRangeTypeDef,
+        "EndTime": TimeRangeTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAttacksRequestRequestTypeDef = TypedDict(
+    "ListAttacksRequestRequestTypeDef",
+    {
+        "ResourceArns": Sequence[str],
+        "StartTime": TimeRangeTypeDef,
+        "EndTime": TimeRangeTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ProtectionGroupPatternTypeLimitsTypeDef = TypedDict(
     "ProtectionGroupPatternTypeLimitsTypeDef",
     {
         "ArbitraryPatternLimits": ProtectionGroupArbitraryPatternLimitsTypeDef,
     },
 )
 
@@ -744,15 +797,15 @@
 )
 
 ListAttacksResponseTypeDef = TypedDict(
     "ListAttacksResponseTypeDef",
     {
         "AttackSummaries": List[AttackSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAttackStatisticsDataItemTypeDef = TypedDict(
     "_RequiredAttackStatisticsDataItemTypeDef",
     {
         "AttackCount": int,
@@ -781,24 +834,24 @@
     },
 )
 
 DescribeProtectionResponseTypeDef = TypedDict(
     "DescribeProtectionResponseTypeDef",
     {
         "Protection": ProtectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProtectionsResponseTypeDef = TypedDict(
     "ListProtectionsResponseTypeDef",
     {
         "Protections": List[ProtectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttackDetailTypeDef = TypedDict(
     "AttackDetailTypeDef",
     {
         "AttackId": str,
@@ -812,17 +865,17 @@
     },
     total=False,
 )
 
 DescribeAttackStatisticsResponseTypeDef = TypedDict(
     "DescribeAttackStatisticsResponseTypeDef",
     {
-        "TimeRange": TimeRangeTypeDef,
+        "TimeRange": TimeRangeOutputTypeDef,
         "DataItems": List[AttackStatisticsDataItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubscriptionLimitsTypeDef = TypedDict(
     "SubscriptionLimitsTypeDef",
     {
         "ProtectionLimits": ProtectionLimitsTypeDef,
@@ -830,15 +883,15 @@
     },
 )
 
 DescribeAttackResponseTypeDef = TypedDict(
     "DescribeAttackResponseTypeDef",
     {
         "Attack": AttackDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSubscriptionTypeDef = TypedDict(
     "_RequiredSubscriptionTypeDef",
     {
         "SubscriptionLimits": SubscriptionLimitsTypeDef,
@@ -863,10 +916,10 @@
     pass
 
 
 DescribeSubscriptionResponseTypeDef = TypedDict(
     "DescribeSubscriptionResponseTypeDef",
     {
         "Subscription": SubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-shield-1.28.0/mypy_boto3_shield/type_defs.pyi` & `mypy-boto3-shield-1.28.12/mypy_boto3_shield/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for shield service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_shield.type_defs import ResponseActionTypeDef
+    from mypy_boto3_shield.type_defs import ResponseActionOutputTypeDef
 
-    data: ResponseActionTypeDef = {...}
+    data: ResponseActionOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ApplicationLayerAutomaticResponseStatusType,
     AttackLayerType,
     AttackPropertyIdentifierType,
     AutoRenewType,
     ProactiveEngagementStatusType,
@@ -31,72 +31,76 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ResponseActionTypeDef",
+    "ResponseActionOutputTypeDef",
     "AssociateDRTLogBucketRequestRequestTypeDef",
     "AssociateDRTRoleRequestRequestTypeDef",
     "AssociateHealthCheckRequestRequestTypeDef",
     "EmergencyContactTypeDef",
     "MitigationTypeDef",
     "SummarizedCounterTypeDef",
     "ContributorTypeDef",
     "AttackVectorDescriptionTypeDef",
     "AttackVolumeStatisticsTypeDef",
     "TagTypeDef",
-    "CreateProtectionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteProtectionGroupRequestRequestTypeDef",
     "DeleteProtectionRequestRequestTypeDef",
     "DescribeAttackRequestRequestTypeDef",
-    "TimeRangeTypeDef",
-    "DescribeDRTAccessResponseTypeDef",
+    "TimeRangeOutputTypeDef",
+    "EmergencyContactOutputTypeDef",
     "DescribeProtectionGroupRequestRequestTypeDef",
     "ProtectionGroupTypeDef",
     "DescribeProtectionRequestRequestTypeDef",
     "DisableApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "DisassociateDRTLogBucketRequestRequestTypeDef",
     "DisassociateHealthCheckRequestRequestTypeDef",
-    "GetSubscriptionStateResponseTypeDef",
+    "ResponseActionTypeDef",
     "InclusionProtectionFiltersTypeDef",
     "InclusionProtectionGroupFiltersTypeDef",
     "LimitTypeDef",
+    "PaginatorConfigTypeDef",
+    "TimeRangeTypeDef",
     "ListResourcesInProtectionGroupRequestRequestTypeDef",
-    "ListResourcesInProtectionGroupResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProtectionGroupRequestRequestTypeDef",
     "UpdateSubscriptionRequestRequestTypeDef",
     "ApplicationLayerAutomaticResponseConfigurationTypeDef",
-    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
-    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "AssociateProactiveEngagementDetailsRequestRequestTypeDef",
-    "DescribeEmergencyContactSettingsResponseTypeDef",
     "UpdateEmergencyContactSettingsRequestRequestTypeDef",
     "SummarizedAttackVectorTypeDef",
     "AttackPropertyTypeDef",
     "AttackSummaryTypeDef",
     "AttackVolumeTypeDef",
     "CreateProtectionGroupRequestRequestTypeDef",
     "CreateProtectionRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "ListAttacksRequestListAttacksPaginateTypeDef",
-    "ListAttacksRequestRequestTypeDef",
+    "CreateProtectionResponseTypeDef",
+    "DescribeDRTAccessResponseTypeDef",
+    "GetSubscriptionStateResponseTypeDef",
+    "ListResourcesInProtectionGroupResponseTypeDef",
+    "DescribeEmergencyContactSettingsResponseTypeDef",
     "DescribeProtectionGroupResponseTypeDef",
     "ListProtectionGroupsResponseTypeDef",
-    "ListProtectionsRequestListProtectionsPaginateTypeDef",
+    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
+    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "ListProtectionsRequestRequestTypeDef",
     "ListProtectionGroupsRequestRequestTypeDef",
     "ProtectionLimitsTypeDef",
+    "ListProtectionsRequestListProtectionsPaginateTypeDef",
+    "ListAttacksRequestListAttacksPaginateTypeDef",
+    "ListAttacksRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ProtectionGroupPatternTypeLimitsTypeDef",
     "ProtectionTypeDef",
     "SubResourceSummaryTypeDef",
     "ListAttacksResponseTypeDef",
     "AttackStatisticsDataItemTypeDef",
     "ProtectionGroupLimitsTypeDef",
     "DescribeProtectionResponseTypeDef",
@@ -105,16 +109,16 @@
     "DescribeAttackStatisticsResponseTypeDef",
     "SubscriptionLimitsTypeDef",
     "DescribeAttackResponseTypeDef",
     "SubscriptionTypeDef",
     "DescribeSubscriptionResponseTypeDef",
 )
 
-ResponseActionTypeDef = TypedDict(
-    "ResponseActionTypeDef",
+ResponseActionOutputTypeDef = TypedDict(
+    "ResponseActionOutputTypeDef",
     {
         "Block": Dict[str, Any],
         "Count": Dict[str, Any],
     },
     total=False,
 )
 
@@ -207,19 +211,22 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-CreateProtectionResponseTypeDef = TypedDict(
-    "CreateProtectionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ProtectionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteProtectionGroupRequestRequestTypeDef = TypedDict(
     "DeleteProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
@@ -236,32 +243,43 @@
 DescribeAttackRequestRequestTypeDef = TypedDict(
     "DescribeAttackRequestRequestTypeDef",
     {
         "AttackId": str,
     },
 )
 
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
+TimeRangeOutputTypeDef = TypedDict(
+    "TimeRangeOutputTypeDef",
     {
         "FromInclusive": datetime,
         "ToExclusive": datetime,
     },
     total=False,
 )
 
-DescribeDRTAccessResponseTypeDef = TypedDict(
-    "DescribeDRTAccessResponseTypeDef",
+_RequiredEmergencyContactOutputTypeDef = TypedDict(
+    "_RequiredEmergencyContactOutputTypeDef",
     {
-        "RoleArn": str,
-        "LogBucketList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EmailAddress": str,
+    },
+)
+_OptionalEmergencyContactOutputTypeDef = TypedDict(
+    "_OptionalEmergencyContactOutputTypeDef",
+    {
+        "PhoneNumber": str,
+        "ContactNotes": str,
     },
+    total=False,
 )
 
+class EmergencyContactOutputTypeDef(
+    _RequiredEmergencyContactOutputTypeDef, _OptionalEmergencyContactOutputTypeDef
+):
+    pass
+
 DescribeProtectionGroupRequestRequestTypeDef = TypedDict(
     "DescribeProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
     },
 )
 
@@ -313,20 +331,21 @@
     "DisassociateHealthCheckRequestRequestTypeDef",
     {
         "ProtectionId": str,
         "HealthCheckArn": str,
     },
 )
 
-GetSubscriptionStateResponseTypeDef = TypedDict(
-    "GetSubscriptionStateResponseTypeDef",
+ResponseActionTypeDef = TypedDict(
+    "ResponseActionTypeDef",
     {
-        "SubscriptionState": SubscriptionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Block": Mapping[str, Any],
+        "Count": Mapping[str, Any],
     },
+    total=False,
 )
 
 InclusionProtectionFiltersTypeDef = TypedDict(
     "InclusionProtectionFiltersTypeDef",
     {
         "ResourceArns": Sequence[str],
         "ProtectionNames": Sequence[str],
@@ -351,14 +370,33 @@
     {
         "Type": str,
         "Max": int,
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
+TimeRangeTypeDef = TypedDict(
+    "TimeRangeTypeDef",
+    {
+        "FromInclusive": Union[datetime, str],
+        "ToExclusive": Union[datetime, str],
+    },
+    total=False,
+)
+
 _RequiredListResourcesInProtectionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesInProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
     },
 )
 _OptionalListResourcesInProtectionGroupRequestRequestTypeDef = TypedDict(
@@ -372,58 +410,37 @@
 
 class ListResourcesInProtectionGroupRequestRequestTypeDef(
     _RequiredListResourcesInProtectionGroupRequestRequestTypeDef,
     _OptionalListResourcesInProtectionGroupRequestRequestTypeDef,
 ):
     pass
 
-ListResourcesInProtectionGroupResponseTypeDef = TypedDict(
-    "ListResourcesInProtectionGroupResponseTypeDef",
-    {
-        "ResourceArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 
 ProtectionGroupArbitraryPatternLimitsTypeDef = TypedDict(
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
     {
         "MaxMembers": int,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -459,49 +476,25 @@
     total=False,
 )
 
 ApplicationLayerAutomaticResponseConfigurationTypeDef = TypedDict(
     "ApplicationLayerAutomaticResponseConfigurationTypeDef",
     {
         "Status": ApplicationLayerAutomaticResponseStatusType,
-        "Action": ResponseActionTypeDef,
-    },
-)
-
-EnableApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
-    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Action": ResponseActionTypeDef,
-    },
-)
-
-UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
-    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Action": ResponseActionTypeDef,
+        "Action": ResponseActionOutputTypeDef,
     },
 )
 
 AssociateProactiveEngagementDetailsRequestRequestTypeDef = TypedDict(
     "AssociateProactiveEngagementDetailsRequestRequestTypeDef",
     {
         "EmergencyContactList": Sequence[EmergencyContactTypeDef],
     },
 )
 
-DescribeEmergencyContactSettingsResponseTypeDef = TypedDict(
-    "DescribeEmergencyContactSettingsResponseTypeDef",
-    {
-        "EmergencyContactList": List[EmergencyContactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateEmergencyContactSettingsRequestRequestTypeDef = TypedDict(
     "UpdateEmergencyContactSettingsRequestRequestTypeDef",
     {
         "EmergencyContactList": Sequence[EmergencyContactTypeDef],
     },
     total=False,
 )
@@ -599,77 +592,95 @@
 )
 
 class CreateProtectionRequestRequestTypeDef(
     _RequiredCreateProtectionRequestRequestTypeDef, _OptionalCreateProtectionRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-ListAttacksRequestListAttacksPaginateTypeDef = TypedDict(
-    "ListAttacksRequestListAttacksPaginateTypeDef",
+CreateProtectionResponseTypeDef = TypedDict(
+    "CreateProtectionResponseTypeDef",
     {
-        "ResourceArns": Sequence[str],
-        "StartTime": TimeRangeTypeDef,
-        "EndTime": TimeRangeTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ProtectionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ListAttacksRequestRequestTypeDef = TypedDict(
-    "ListAttacksRequestRequestTypeDef",
+DescribeDRTAccessResponseTypeDef = TypedDict(
+    "DescribeDRTAccessResponseTypeDef",
     {
-        "ResourceArns": Sequence[str],
-        "StartTime": TimeRangeTypeDef,
-        "EndTime": TimeRangeTypeDef,
+        "RoleArn": str,
+        "LogBucketList": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSubscriptionStateResponseTypeDef = TypedDict(
+    "GetSubscriptionStateResponseTypeDef",
+    {
+        "SubscriptionState": SubscriptionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListResourcesInProtectionGroupResponseTypeDef = TypedDict(
+    "ListResourcesInProtectionGroupResponseTypeDef",
+    {
+        "ResourceArns": List[str],
         "NextToken": str,
-        "MaxResults": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEmergencyContactSettingsResponseTypeDef = TypedDict(
+    "DescribeEmergencyContactSettingsResponseTypeDef",
+    {
+        "EmergencyContactList": List[EmergencyContactOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DescribeProtectionGroupResponseTypeDef = TypedDict(
     "DescribeProtectionGroupResponseTypeDef",
     {
         "ProtectionGroup": ProtectionGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProtectionGroupsResponseTypeDef = TypedDict(
     "ListProtectionGroupsResponseTypeDef",
     {
         "ProtectionGroups": List[ProtectionGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListProtectionsRequestListProtectionsPaginateTypeDef = TypedDict(
-    "ListProtectionsRequestListProtectionsPaginateTypeDef",
+EnableApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
+    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
     {
-        "InclusionFilters": InclusionProtectionFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ResourceArn": str,
+        "Action": ResponseActionTypeDef,
+    },
+)
+
+UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
+    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Action": ResponseActionTypeDef,
     },
-    total=False,
 )
 
 ListProtectionsRequestRequestTypeDef = TypedDict(
     "ListProtectionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -691,14 +702,54 @@
 ProtectionLimitsTypeDef = TypedDict(
     "ProtectionLimitsTypeDef",
     {
         "ProtectedResourceTypeLimits": List[LimitTypeDef],
     },
 )
 
+ListProtectionsRequestListProtectionsPaginateTypeDef = TypedDict(
+    "ListProtectionsRequestListProtectionsPaginateTypeDef",
+    {
+        "InclusionFilters": InclusionProtectionFiltersTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAttacksRequestListAttacksPaginateTypeDef = TypedDict(
+    "ListAttacksRequestListAttacksPaginateTypeDef",
+    {
+        "ResourceArns": Sequence[str],
+        "StartTime": TimeRangeTypeDef,
+        "EndTime": TimeRangeTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAttacksRequestRequestTypeDef = TypedDict(
+    "ListAttacksRequestRequestTypeDef",
+    {
+        "ResourceArns": Sequence[str],
+        "StartTime": TimeRangeTypeDef,
+        "EndTime": TimeRangeTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ProtectionGroupPatternTypeLimitsTypeDef = TypedDict(
     "ProtectionGroupPatternTypeLimitsTypeDef",
     {
         "ArbitraryPatternLimits": ProtectionGroupArbitraryPatternLimitsTypeDef,
     },
 )
 
@@ -729,15 +780,15 @@
 )
 
 ListAttacksResponseTypeDef = TypedDict(
     "ListAttacksResponseTypeDef",
     {
         "AttackSummaries": List[AttackSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAttackStatisticsDataItemTypeDef = TypedDict(
     "_RequiredAttackStatisticsDataItemTypeDef",
     {
         "AttackCount": int,
@@ -764,24 +815,24 @@
     },
 )
 
 DescribeProtectionResponseTypeDef = TypedDict(
     "DescribeProtectionResponseTypeDef",
     {
         "Protection": ProtectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProtectionsResponseTypeDef = TypedDict(
     "ListProtectionsResponseTypeDef",
     {
         "Protections": List[ProtectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttackDetailTypeDef = TypedDict(
     "AttackDetailTypeDef",
     {
         "AttackId": str,
@@ -795,17 +846,17 @@
     },
     total=False,
 )
 
 DescribeAttackStatisticsResponseTypeDef = TypedDict(
     "DescribeAttackStatisticsResponseTypeDef",
     {
-        "TimeRange": TimeRangeTypeDef,
+        "TimeRange": TimeRangeOutputTypeDef,
         "DataItems": List[AttackStatisticsDataItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubscriptionLimitsTypeDef = TypedDict(
     "SubscriptionLimitsTypeDef",
     {
         "ProtectionLimits": ProtectionLimitsTypeDef,
@@ -813,15 +864,15 @@
     },
 )
 
 DescribeAttackResponseTypeDef = TypedDict(
     "DescribeAttackResponseTypeDef",
     {
         "Attack": AttackDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSubscriptionTypeDef = TypedDict(
     "_RequiredSubscriptionTypeDef",
     {
         "SubscriptionLimits": SubscriptionLimitsTypeDef,
@@ -844,10 +895,10 @@
 class SubscriptionTypeDef(_RequiredSubscriptionTypeDef, _OptionalSubscriptionTypeDef):
     pass
 
 DescribeSubscriptionResponseTypeDef = TypedDict(
     "DescribeSubscriptionResponseTypeDef",
     {
         "Subscription": SubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-shield-1.28.0/mypy_boto3_shield.egg-info/PKG-INFO` & `mypy-boto3-shield-1.28.12/mypy_boto3_shield.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-shield
-Version: 1.28.0
-Summary: Type annotations for boto3.Shield 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Shield 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-shield"></a>
 
 # mypy-boto3-shield
 
 [![PyPI - mypy-boto3-shield](https://img.shields.io/pypi/v/mypy-boto3-shield.svg?color=blue)](https://pypi.org/project/mypy-boto3-shield)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-shield.svg?color=blue)](https://pypi.org/project/mypy-boto3-shield)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-shield?color=blue)](https://pypistats.org/packages/mypy-boto3-shield)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-shield)](https://pepy.tech/project/mypy-boto3-shield)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Shield 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
+[boto3.Shield 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
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
 [mypy-boto3-shield docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,72 +330,76 @@
 ### Typed dictionaries
 
 `mypy_boto3_shield.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_shield.type_defs import (
-    ResponseActionTypeDef,
+    ResponseActionOutputTypeDef,
     AssociateDRTLogBucketRequestRequestTypeDef,
     AssociateDRTRoleRequestRequestTypeDef,
     AssociateHealthCheckRequestRequestTypeDef,
     EmergencyContactTypeDef,
     MitigationTypeDef,
     SummarizedCounterTypeDef,
     ContributorTypeDef,
     AttackVectorDescriptionTypeDef,
     AttackVolumeStatisticsTypeDef,
     TagTypeDef,
-    CreateProtectionResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteProtectionGroupRequestRequestTypeDef,
     DeleteProtectionRequestRequestTypeDef,
     DescribeAttackRequestRequestTypeDef,
-    TimeRangeTypeDef,
-    DescribeDRTAccessResponseTypeDef,
+    TimeRangeOutputTypeDef,
+    EmergencyContactOutputTypeDef,
     DescribeProtectionGroupRequestRequestTypeDef,
     ProtectionGroupTypeDef,
     DescribeProtectionRequestRequestTypeDef,
     DisableApplicationLayerAutomaticResponseRequestRequestTypeDef,
     DisassociateDRTLogBucketRequestRequestTypeDef,
     DisassociateHealthCheckRequestRequestTypeDef,
-    GetSubscriptionStateResponseTypeDef,
+    ResponseActionTypeDef,
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     LimitTypeDef,
+    PaginatorConfigTypeDef,
+    TimeRangeTypeDef,
     ListResourcesInProtectionGroupRequestRequestTypeDef,
-    ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     ProtectionGroupArbitraryPatternLimitsTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProtectionGroupRequestRequestTypeDef,
     UpdateSubscriptionRequestRequestTypeDef,
     ApplicationLayerAutomaticResponseConfigurationTypeDef,
-    EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
-    UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
     AssociateProactiveEngagementDetailsRequestRequestTypeDef,
-    DescribeEmergencyContactSettingsResponseTypeDef,
     UpdateEmergencyContactSettingsRequestRequestTypeDef,
     SummarizedAttackVectorTypeDef,
     AttackPropertyTypeDef,
     AttackSummaryTypeDef,
     AttackVolumeTypeDef,
     CreateProtectionGroupRequestRequestTypeDef,
     CreateProtectionRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    ListAttacksRequestListAttacksPaginateTypeDef,
-    ListAttacksRequestRequestTypeDef,
+    CreateProtectionResponseTypeDef,
+    DescribeDRTAccessResponseTypeDef,
+    GetSubscriptionStateResponseTypeDef,
+    ListResourcesInProtectionGroupResponseTypeDef,
+    DescribeEmergencyContactSettingsResponseTypeDef,
     DescribeProtectionGroupResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
-    ListProtectionsRequestListProtectionsPaginateTypeDef,
+    EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
+    UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
     ListProtectionsRequestRequestTypeDef,
     ListProtectionGroupsRequestRequestTypeDef,
     ProtectionLimitsTypeDef,
+    ListProtectionsRequestListProtectionsPaginateTypeDef,
+    ListAttacksRequestListAttacksPaginateTypeDef,
+    ListAttacksRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ProtectionGroupPatternTypeLimitsTypeDef,
     ProtectionTypeDef,
     SubResourceSummaryTypeDef,
     ListAttacksResponseTypeDef,
     AttackStatisticsDataItemTypeDef,
     ProtectionGroupLimitsTypeDef,
     DescribeProtectionResponseTypeDef,
@@ -405,15 +409,15 @@
     SubscriptionLimitsTypeDef,
     DescribeAttackResponseTypeDef,
     SubscriptionTypeDef,
     DescribeSubscriptionResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseActionTypeDef:
+def get_structure() -> ResponseActionOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-shield-1.28.0/mypy_boto3_shield.egg-info/SOURCES.txt` & `mypy-boto3-shield-1.28.12/mypy_boto3_shield.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.0/setup.py` & `mypy-boto3-shield-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-shield",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_shield"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Shield 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Shield 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

