# Comparing `tmp/mypy-boto3-vpc-lattice-1.28.0.tar.gz` & `tmp/mypy-boto3-vpc-lattice-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-vpc-lattice-1.28.0.tar", last modified: Thu Jul  6 21:00:49 2023, max compression
+gzip compressed data, was "mypy-boto3-vpc-lattice-1.28.12.tar", last modified: Thu Jul 27 11:49:49 2023, max compression
```

## Comparing `mypy-boto3-vpc-lattice-1.28.0.tar` & `mypy-boto3-vpc-lattice-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:49.858456 mypy-boto3-vpc-lattice-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:57:34.000000 mypy-boto3-vpc-lattice-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20218 2023-07-06 21:00:49.854456 mypy-boto3-vpc-lattice-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18718 2023-07-06 20:57:34.000000 mypy-boto3-vpc-lattice-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:49.850456 mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-06 20:57:34.000000 mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-06 20:57:34.000000 mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-06 20:57:34.000000 mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38846 2023-07-06 20:57:34.000000 mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38778 2023-07-06 20:57:34.000000 mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-07-06 20:57:35.000000 mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10560 2023-07-06 20:57:34.000000 mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-07-06 20:57:34.000000 mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-07-06 20:57:34.000000 mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:57:34.000000 mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    48681 2023-07-06 20:57:36.000000 mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    48632 2023-07-06 20:57:35.000000 mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:57:34.000000 mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:49.854456 mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20218 2023-07-06 21:00:49.000000 mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-06 21:00:49.000000 mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:49.000000 mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:49.000000 mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:49.000000 mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 21:00:49.000000 mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:49.858456 mypy-boto3-vpc-lattice-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-06 20:57:34.000000 mypy-boto3-vpc-lattice-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.065487 mypy-boto3-vpc-lattice-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-07-27 11:49:49.065487 mypy-boto3-vpc-lattice-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19143 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.065487 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38846 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38778 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10640 2023-07-27 11:48:20.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-07-27 11:48:20.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53229 2023-07-27 11:48:21.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53170 2023-07-27 11:48:20.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.065487 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-07-27 11:49:48.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-27 11:49:48.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:48.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:48.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:48.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 11:49:48.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:49.065487 mypy-boto3-vpc-lattice-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/setup.py
```

### Comparing `mypy-boto3-vpc-lattice-1.28.0/LICENSE` & `mypy-boto3-vpc-lattice-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.0/PKG-INFO` & `mypy-boto3-vpc-lattice-1.28.12/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-vpc-lattice
-Version: 1.28.0
-Summary: Type annotations for boto3.VPCLattice 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.VPCLattice 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-vpc-lattice"></a>
 
 # mypy-boto3-vpc-lattice
 
 [![PyPI - mypy-boto3-vpc-lattice](https://img.shields.io/pypi/v/mypy-boto3-vpc-lattice.svg?color=blue)](https://pypi.org/project/mypy-boto3-vpc-lattice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-vpc-lattice.svg?color=blue)](https://pypi.org/project/mypy-boto3-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-vpc-lattice?color=blue)](https://pypistats.org/packages/mypy-boto3-vpc-lattice)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-vpc-lattice)](https://pepy.tech/project/mypy-boto3-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VPCLattice 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
+[boto3.VPCLattice 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
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
 [mypy-boto3-vpc-lattice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -366,145 +366,159 @@
 
 `mypy_boto3_vpc_lattice.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_vpc_lattice.type_defs import (
     AccessLogSubscriptionSummaryTypeDef,
+    ResponseMetadataTypeDef,
     RuleUpdateFailureTypeDef,
     CreateAccessLogSubscriptionRequestRequestTypeDef,
-    CreateAccessLogSubscriptionResponseTypeDef,
     CreateServiceNetworkRequestRequestTypeDef,
-    CreateServiceNetworkResponseTypeDef,
     CreateServiceNetworkServiceAssociationRequestRequestTypeDef,
     DnsEntryTypeDef,
     CreateServiceNetworkVpcAssociationRequestRequestTypeDef,
-    CreateServiceNetworkVpcAssociationResponseTypeDef,
     CreateServiceRequestRequestTypeDef,
     DeleteAccessLogSubscriptionRequestRequestTypeDef,
     DeleteAuthPolicyRequestRequestTypeDef,
     DeleteListenerRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DeleteServiceNetworkRequestRequestTypeDef,
     DeleteServiceNetworkServiceAssociationRequestRequestTypeDef,
-    DeleteServiceNetworkServiceAssociationResponseTypeDef,
     DeleteServiceNetworkVpcAssociationRequestRequestTypeDef,
-    DeleteServiceNetworkVpcAssociationResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
-    DeleteServiceResponseTypeDef,
     DeleteTargetGroupRequestRequestTypeDef,
-    DeleteTargetGroupResponseTypeDef,
     TargetTypeDef,
     TargetFailureTypeDef,
+    TargetOutputTypeDef,
+    FixedResponseActionOutputTypeDef,
     FixedResponseActionTypeDef,
+    WeightedTargetGroupOutputTypeDef,
     WeightedTargetGroupTypeDef,
     GetAccessLogSubscriptionRequestRequestTypeDef,
-    GetAccessLogSubscriptionResponseTypeDef,
     GetAuthPolicyRequestRequestTypeDef,
-    GetAuthPolicyResponseTypeDef,
     GetListenerRequestRequestTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetRuleRequestRequestTypeDef,
     GetServiceNetworkRequestRequestTypeDef,
-    GetServiceNetworkResponseTypeDef,
     GetServiceNetworkServiceAssociationRequestRequestTypeDef,
     GetServiceNetworkVpcAssociationRequestRequestTypeDef,
-    GetServiceNetworkVpcAssociationResponseTypeDef,
     GetServiceRequestRequestTypeDef,
     GetTargetGroupRequestRequestTypeDef,
+    HeaderMatchTypeOutputTypeDef,
     HeaderMatchTypeTypeDef,
+    MatcherOutputTypeDef,
     MatcherTypeDef,
-    ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessLogSubscriptionsRequestRequestTypeDef,
-    ListListenersRequestListListenersPaginateTypeDef,
     ListListenersRequestRequestTypeDef,
     ListenerSummaryTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
-    ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef,
     ListServiceNetworkServiceAssociationsRequestRequestTypeDef,
-    ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef,
     ListServiceNetworkVpcAssociationsRequestRequestTypeDef,
     ServiceNetworkVpcAssociationSummaryTypeDef,
-    ListServiceNetworksRequestListServiceNetworksPaginateTypeDef,
     ListServiceNetworksRequestRequestTypeDef,
     ServiceNetworkSummaryTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTargetGroupsRequestListTargetGroupsPaginateTypeDef,
     ListTargetGroupsRequestRequestTypeDef,
     TargetGroupSummaryTypeDef,
     TargetSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    PathMatchTypeOutputTypeDef,
     PathMatchTypeTypeDef,
     PutAuthPolicyRequestRequestTypeDef,
-    PutAuthPolicyResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccessLogSubscriptionRequestRequestTypeDef,
-    UpdateAccessLogSubscriptionResponseTypeDef,
     UpdateServiceNetworkRequestRequestTypeDef,
-    UpdateServiceNetworkResponseTypeDef,
     UpdateServiceNetworkVpcAssociationRequestRequestTypeDef,
-    UpdateServiceNetworkVpcAssociationResponseTypeDef,
     UpdateServiceRequestRequestTypeDef,
-    UpdateServiceResponseTypeDef,
+    CreateAccessLogSubscriptionResponseTypeDef,
+    CreateServiceNetworkResponseTypeDef,
+    CreateServiceNetworkVpcAssociationResponseTypeDef,
+    DeleteServiceNetworkServiceAssociationResponseTypeDef,
+    DeleteServiceNetworkVpcAssociationResponseTypeDef,
+    DeleteServiceResponseTypeDef,
+    DeleteTargetGroupResponseTypeDef,
+    GetAccessLogSubscriptionResponseTypeDef,
+    GetAuthPolicyResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    GetServiceNetworkResponseTypeDef,
+    GetServiceNetworkVpcAssociationResponseTypeDef,
     ListAccessLogSubscriptionsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutAuthPolicyResponseTypeDef,
+    UpdateAccessLogSubscriptionResponseTypeDef,
+    UpdateServiceNetworkResponseTypeDef,
+    UpdateServiceNetworkVpcAssociationResponseTypeDef,
+    UpdateServiceResponseTypeDef,
     CreateServiceNetworkServiceAssociationResponseTypeDef,
     CreateServiceResponseTypeDef,
     GetServiceNetworkServiceAssociationResponseTypeDef,
     GetServiceResponseTypeDef,
     ServiceNetworkServiceAssociationSummaryTypeDef,
     ServiceSummaryTypeDef,
     DeregisterTargetsRequestRequestTypeDef,
-    ListTargetsRequestListTargetsPaginateTypeDef,
     ListTargetsRequestRequestTypeDef,
     RegisterTargetsRequestRequestTypeDef,
     DeregisterTargetsResponseTypeDef,
     RegisterTargetsResponseTypeDef,
+    ForwardActionOutputTypeDef,
     ForwardActionTypeDef,
+    HeaderMatchOutputTypeDef,
     HeaderMatchTypeDef,
+    HealthCheckConfigOutputTypeDef,
     HealthCheckConfigTypeDef,
+    ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+    ListListenersRequestListListenersPaginateTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
+    ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef,
+    ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef,
+    ListServiceNetworksRequestListServiceNetworksPaginateTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
+    ListTargetGroupsRequestListTargetGroupsPaginateTypeDef,
+    ListTargetsRequestListTargetsPaginateTypeDef,
     ListListenersResponseTypeDef,
     ListRulesResponseTypeDef,
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServiceNetworksResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
+    PathMatchOutputTypeDef,
     PathMatchTypeDef,
     ListServiceNetworkServiceAssociationsResponseTypeDef,
     ListServicesResponseTypeDef,
+    RuleActionOutputTypeDef,
     RuleActionTypeDef,
+    TargetGroupConfigOutputTypeDef,
     TargetGroupConfigTypeDef,
     UpdateTargetGroupRequestRequestTypeDef,
+    HttpMatchOutputTypeDef,
     HttpMatchTypeDef,
-    CreateListenerRequestRequestTypeDef,
     CreateListenerResponseTypeDef,
     GetListenerResponseTypeDef,
-    UpdateListenerRequestRequestTypeDef,
     UpdateListenerResponseTypeDef,
-    CreateTargetGroupRequestRequestTypeDef,
+    CreateListenerRequestRequestTypeDef,
+    UpdateListenerRequestRequestTypeDef,
     CreateTargetGroupResponseTypeDef,
     GetTargetGroupResponseTypeDef,
     UpdateTargetGroupResponseTypeDef,
+    CreateTargetGroupRequestRequestTypeDef,
+    RuleMatchOutputTypeDef,
     RuleMatchTypeDef,
-    CreateRuleRequestRequestTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     RuleUpdateSuccessTypeDef,
+    UpdateRuleResponseTypeDef,
+    CreateRuleRequestRequestTypeDef,
     RuleUpdateTypeDef,
     UpdateRuleRequestRequestTypeDef,
-    UpdateRuleResponseTypeDef,
     BatchUpdateRuleResponseTypeDef,
     BatchUpdateRuleRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AccessLogSubscriptionSummaryTypeDef:
     return {...}
```

### Comparing `mypy-boto3-vpc-lattice-1.28.0/README.md` & `mypy-boto3-vpc-lattice-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-vpc-lattice"></a>
 
 # mypy-boto3-vpc-lattice
 
 [![PyPI - mypy-boto3-vpc-lattice](https://img.shields.io/pypi/v/mypy-boto3-vpc-lattice.svg?color=blue)](https://pypi.org/project/mypy-boto3-vpc-lattice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-vpc-lattice.svg?color=blue)](https://pypi.org/project/mypy-boto3-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-vpc-lattice?color=blue)](https://pypistats.org/packages/mypy-boto3-vpc-lattice)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-vpc-lattice)](https://pepy.tech/project/mypy-boto3-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VPCLattice 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
+[boto3.VPCLattice 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
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
 [mypy-boto3-vpc-lattice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,145 +334,159 @@
 
 `mypy_boto3_vpc_lattice.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_vpc_lattice.type_defs import (
     AccessLogSubscriptionSummaryTypeDef,
+    ResponseMetadataTypeDef,
     RuleUpdateFailureTypeDef,
     CreateAccessLogSubscriptionRequestRequestTypeDef,
-    CreateAccessLogSubscriptionResponseTypeDef,
     CreateServiceNetworkRequestRequestTypeDef,
-    CreateServiceNetworkResponseTypeDef,
     CreateServiceNetworkServiceAssociationRequestRequestTypeDef,
     DnsEntryTypeDef,
     CreateServiceNetworkVpcAssociationRequestRequestTypeDef,
-    CreateServiceNetworkVpcAssociationResponseTypeDef,
     CreateServiceRequestRequestTypeDef,
     DeleteAccessLogSubscriptionRequestRequestTypeDef,
     DeleteAuthPolicyRequestRequestTypeDef,
     DeleteListenerRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DeleteServiceNetworkRequestRequestTypeDef,
     DeleteServiceNetworkServiceAssociationRequestRequestTypeDef,
-    DeleteServiceNetworkServiceAssociationResponseTypeDef,
     DeleteServiceNetworkVpcAssociationRequestRequestTypeDef,
-    DeleteServiceNetworkVpcAssociationResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
-    DeleteServiceResponseTypeDef,
     DeleteTargetGroupRequestRequestTypeDef,
-    DeleteTargetGroupResponseTypeDef,
     TargetTypeDef,
     TargetFailureTypeDef,
+    TargetOutputTypeDef,
+    FixedResponseActionOutputTypeDef,
     FixedResponseActionTypeDef,
+    WeightedTargetGroupOutputTypeDef,
     WeightedTargetGroupTypeDef,
     GetAccessLogSubscriptionRequestRequestTypeDef,
-    GetAccessLogSubscriptionResponseTypeDef,
     GetAuthPolicyRequestRequestTypeDef,
-    GetAuthPolicyResponseTypeDef,
     GetListenerRequestRequestTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetRuleRequestRequestTypeDef,
     GetServiceNetworkRequestRequestTypeDef,
-    GetServiceNetworkResponseTypeDef,
     GetServiceNetworkServiceAssociationRequestRequestTypeDef,
     GetServiceNetworkVpcAssociationRequestRequestTypeDef,
-    GetServiceNetworkVpcAssociationResponseTypeDef,
     GetServiceRequestRequestTypeDef,
     GetTargetGroupRequestRequestTypeDef,
+    HeaderMatchTypeOutputTypeDef,
     HeaderMatchTypeTypeDef,
+    MatcherOutputTypeDef,
     MatcherTypeDef,
-    ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessLogSubscriptionsRequestRequestTypeDef,
-    ListListenersRequestListListenersPaginateTypeDef,
     ListListenersRequestRequestTypeDef,
     ListenerSummaryTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
-    ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef,
     ListServiceNetworkServiceAssociationsRequestRequestTypeDef,
-    ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef,
     ListServiceNetworkVpcAssociationsRequestRequestTypeDef,
     ServiceNetworkVpcAssociationSummaryTypeDef,
-    ListServiceNetworksRequestListServiceNetworksPaginateTypeDef,
     ListServiceNetworksRequestRequestTypeDef,
     ServiceNetworkSummaryTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTargetGroupsRequestListTargetGroupsPaginateTypeDef,
     ListTargetGroupsRequestRequestTypeDef,
     TargetGroupSummaryTypeDef,
     TargetSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    PathMatchTypeOutputTypeDef,
     PathMatchTypeTypeDef,
     PutAuthPolicyRequestRequestTypeDef,
-    PutAuthPolicyResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccessLogSubscriptionRequestRequestTypeDef,
-    UpdateAccessLogSubscriptionResponseTypeDef,
     UpdateServiceNetworkRequestRequestTypeDef,
-    UpdateServiceNetworkResponseTypeDef,
     UpdateServiceNetworkVpcAssociationRequestRequestTypeDef,
-    UpdateServiceNetworkVpcAssociationResponseTypeDef,
     UpdateServiceRequestRequestTypeDef,
-    UpdateServiceResponseTypeDef,
+    CreateAccessLogSubscriptionResponseTypeDef,
+    CreateServiceNetworkResponseTypeDef,
+    CreateServiceNetworkVpcAssociationResponseTypeDef,
+    DeleteServiceNetworkServiceAssociationResponseTypeDef,
+    DeleteServiceNetworkVpcAssociationResponseTypeDef,
+    DeleteServiceResponseTypeDef,
+    DeleteTargetGroupResponseTypeDef,
+    GetAccessLogSubscriptionResponseTypeDef,
+    GetAuthPolicyResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    GetServiceNetworkResponseTypeDef,
+    GetServiceNetworkVpcAssociationResponseTypeDef,
     ListAccessLogSubscriptionsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutAuthPolicyResponseTypeDef,
+    UpdateAccessLogSubscriptionResponseTypeDef,
+    UpdateServiceNetworkResponseTypeDef,
+    UpdateServiceNetworkVpcAssociationResponseTypeDef,
+    UpdateServiceResponseTypeDef,
     CreateServiceNetworkServiceAssociationResponseTypeDef,
     CreateServiceResponseTypeDef,
     GetServiceNetworkServiceAssociationResponseTypeDef,
     GetServiceResponseTypeDef,
     ServiceNetworkServiceAssociationSummaryTypeDef,
     ServiceSummaryTypeDef,
     DeregisterTargetsRequestRequestTypeDef,
-    ListTargetsRequestListTargetsPaginateTypeDef,
     ListTargetsRequestRequestTypeDef,
     RegisterTargetsRequestRequestTypeDef,
     DeregisterTargetsResponseTypeDef,
     RegisterTargetsResponseTypeDef,
+    ForwardActionOutputTypeDef,
     ForwardActionTypeDef,
+    HeaderMatchOutputTypeDef,
     HeaderMatchTypeDef,
+    HealthCheckConfigOutputTypeDef,
     HealthCheckConfigTypeDef,
+    ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+    ListListenersRequestListListenersPaginateTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
+    ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef,
+    ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef,
+    ListServiceNetworksRequestListServiceNetworksPaginateTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
+    ListTargetGroupsRequestListTargetGroupsPaginateTypeDef,
+    ListTargetsRequestListTargetsPaginateTypeDef,
     ListListenersResponseTypeDef,
     ListRulesResponseTypeDef,
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServiceNetworksResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
+    PathMatchOutputTypeDef,
     PathMatchTypeDef,
     ListServiceNetworkServiceAssociationsResponseTypeDef,
     ListServicesResponseTypeDef,
+    RuleActionOutputTypeDef,
     RuleActionTypeDef,
+    TargetGroupConfigOutputTypeDef,
     TargetGroupConfigTypeDef,
     UpdateTargetGroupRequestRequestTypeDef,
+    HttpMatchOutputTypeDef,
     HttpMatchTypeDef,
-    CreateListenerRequestRequestTypeDef,
     CreateListenerResponseTypeDef,
     GetListenerResponseTypeDef,
-    UpdateListenerRequestRequestTypeDef,
     UpdateListenerResponseTypeDef,
-    CreateTargetGroupRequestRequestTypeDef,
+    CreateListenerRequestRequestTypeDef,
+    UpdateListenerRequestRequestTypeDef,
     CreateTargetGroupResponseTypeDef,
     GetTargetGroupResponseTypeDef,
     UpdateTargetGroupResponseTypeDef,
+    CreateTargetGroupRequestRequestTypeDef,
+    RuleMatchOutputTypeDef,
     RuleMatchTypeDef,
-    CreateRuleRequestRequestTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     RuleUpdateSuccessTypeDef,
+    UpdateRuleResponseTypeDef,
+    CreateRuleRequestRequestTypeDef,
     RuleUpdateTypeDef,
     UpdateRuleRequestRequestTypeDef,
-    UpdateRuleResponseTypeDef,
     BatchUpdateRuleResponseTypeDef,
     BatchUpdateRuleRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AccessLogSubscriptionSummaryTypeDef:
     return {...}
```

### Comparing `mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/__init__.py` & `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/__init__.pyi` & `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/__main__.py` & `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.VPCLattice 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.VPCLattice 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice\nOther"
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

### Comparing `mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/client.py` & `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/client.pyi` & `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/literals.py` & `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,15 @@
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
@@ -290,26 +291,28 @@
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

### Comparing `mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/literals.pyi` & `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -202,14 +202,15 @@
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
@@ -288,26 +289,28 @@
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

### Comparing `mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/paginator.py` & `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,30 +80,30 @@
 class ListAccessLogSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListAccessLogSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listaccesslogsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, resourceIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessLogSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListAccessLogSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listaccesslogsubscriptionspaginator)
         """
 
 
 class ListListenersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListListeners)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listlistenerspaginator)
     """
 
     def paginate(
-        self, *, serviceIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, serviceIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListListenersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListListeners.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listlistenerspaginator)
         """
 
 
@@ -114,15 +114,15 @@
     """
 
     def paginate(
         self,
         *,
         listenerIdentifier: str,
         serviceIdentifier: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listrulespaginator)
         """
 
 
@@ -133,15 +133,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceIdentifier: str = ...,
         serviceNetworkIdentifier: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServiceNetworkServiceAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworkServiceAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicenetworkserviceassociationspaginator)
         """
 
 
@@ -152,45 +152,45 @@
     """
 
     def paginate(
         self,
         *,
         serviceNetworkIdentifier: str = ...,
         vpcIdentifier: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServiceNetworkVpcAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworkVpcAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicenetworkvpcassociationspaginator)
         """
 
 
 class ListServiceNetworksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicenetworkspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServiceNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicenetworkspaginator)
         """
 
 
 class ListServicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicespaginator)
         """
 
 
@@ -201,15 +201,15 @@
     """
 
     def paginate(
         self,
         *,
         targetGroupType: TargetGroupTypeType = ...,
         vpcIdentifier: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTargetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListTargetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listtargetgroupspaginator)
         """
 
 
@@ -220,13 +220,13 @@
     """
 
     def paginate(
         self,
         *,
         targetGroupIdentifier: str,
         targets: Sequence[TargetTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listtargetspaginator)
         """
```

### Comparing `mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/paginator.pyi` & `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -77,29 +77,29 @@
 class ListAccessLogSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListAccessLogSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listaccesslogsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, resourceIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessLogSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListAccessLogSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listaccesslogsubscriptionspaginator)
         """
 
 class ListListenersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListListeners)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listlistenerspaginator)
     """
 
     def paginate(
-        self, *, serviceIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, serviceIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListListenersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListListeners.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listlistenerspaginator)
         """
 
 class ListRulesPaginator(Paginator):
@@ -109,15 +109,15 @@
     """
 
     def paginate(
         self,
         *,
         listenerIdentifier: str,
         serviceIdentifier: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listrulespaginator)
         """
 
 class ListServiceNetworkServiceAssociationsPaginator(Paginator):
@@ -127,15 +127,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceIdentifier: str = ...,
         serviceNetworkIdentifier: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServiceNetworkServiceAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworkServiceAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicenetworkserviceassociationspaginator)
         """
 
 class ListServiceNetworkVpcAssociationsPaginator(Paginator):
@@ -145,43 +145,43 @@
     """
 
     def paginate(
         self,
         *,
         serviceNetworkIdentifier: str = ...,
         vpcIdentifier: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServiceNetworkVpcAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworkVpcAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicenetworkvpcassociationspaginator)
         """
 
 class ListServiceNetworksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicenetworkspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServiceNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicenetworkspaginator)
         """
 
 class ListServicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicespaginator)
         """
 
 class ListTargetGroupsPaginator(Paginator):
@@ -191,15 +191,15 @@
     """
 
     def paginate(
         self,
         *,
         targetGroupType: TargetGroupTypeType = ...,
         vpcIdentifier: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTargetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListTargetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listtargetgroupspaginator)
         """
 
 class ListTargetsPaginator(Paginator):
@@ -209,13 +209,13 @@
     """
 
     def paginate(
         self,
         *,
         targetGroupIdentifier: str,
         targets: Sequence[TargetTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listtargetspaginator)
         """
```

### Comparing `mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/type_defs.py` & `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,145 +35,159 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccessLogSubscriptionSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "RuleUpdateFailureTypeDef",
     "CreateAccessLogSubscriptionRequestRequestTypeDef",
-    "CreateAccessLogSubscriptionResponseTypeDef",
     "CreateServiceNetworkRequestRequestTypeDef",
-    "CreateServiceNetworkResponseTypeDef",
     "CreateServiceNetworkServiceAssociationRequestRequestTypeDef",
     "DnsEntryTypeDef",
     "CreateServiceNetworkVpcAssociationRequestRequestTypeDef",
-    "CreateServiceNetworkVpcAssociationResponseTypeDef",
     "CreateServiceRequestRequestTypeDef",
     "DeleteAccessLogSubscriptionRequestRequestTypeDef",
     "DeleteAuthPolicyRequestRequestTypeDef",
     "DeleteListenerRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "DeleteServiceNetworkRequestRequestTypeDef",
     "DeleteServiceNetworkServiceAssociationRequestRequestTypeDef",
-    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
     "DeleteServiceNetworkVpcAssociationRequestRequestTypeDef",
-    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
     "DeleteServiceRequestRequestTypeDef",
-    "DeleteServiceResponseTypeDef",
     "DeleteTargetGroupRequestRequestTypeDef",
-    "DeleteTargetGroupResponseTypeDef",
     "TargetTypeDef",
     "TargetFailureTypeDef",
+    "TargetOutputTypeDef",
+    "FixedResponseActionOutputTypeDef",
     "FixedResponseActionTypeDef",
+    "WeightedTargetGroupOutputTypeDef",
     "WeightedTargetGroupTypeDef",
     "GetAccessLogSubscriptionRequestRequestTypeDef",
-    "GetAccessLogSubscriptionResponseTypeDef",
     "GetAuthPolicyRequestRequestTypeDef",
-    "GetAuthPolicyResponseTypeDef",
     "GetListenerRequestRequestTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
     "GetRuleRequestRequestTypeDef",
     "GetServiceNetworkRequestRequestTypeDef",
-    "GetServiceNetworkResponseTypeDef",
     "GetServiceNetworkServiceAssociationRequestRequestTypeDef",
     "GetServiceNetworkVpcAssociationRequestRequestTypeDef",
-    "GetServiceNetworkVpcAssociationResponseTypeDef",
     "GetServiceRequestRequestTypeDef",
     "GetTargetGroupRequestRequestTypeDef",
+    "HeaderMatchTypeOutputTypeDef",
     "HeaderMatchTypeTypeDef",
+    "MatcherOutputTypeDef",
     "MatcherTypeDef",
-    "ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccessLogSubscriptionsRequestRequestTypeDef",
-    "ListListenersRequestListListenersPaginateTypeDef",
     "ListListenersRequestRequestTypeDef",
     "ListenerSummaryTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
     "RuleSummaryTypeDef",
-    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
     "ListServiceNetworkServiceAssociationsRequestRequestTypeDef",
-    "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
     "ListServiceNetworkVpcAssociationsRequestRequestTypeDef",
     "ServiceNetworkVpcAssociationSummaryTypeDef",
-    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
     "ListServiceNetworksRequestRequestTypeDef",
     "ServiceNetworkSummaryTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
     "ListTargetGroupsRequestRequestTypeDef",
     "TargetGroupSummaryTypeDef",
     "TargetSummaryTypeDef",
-    "PaginatorConfigTypeDef",
+    "PathMatchTypeOutputTypeDef",
     "PathMatchTypeTypeDef",
     "PutAuthPolicyRequestRequestTypeDef",
-    "PutAuthPolicyResponseTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccessLogSubscriptionRequestRequestTypeDef",
-    "UpdateAccessLogSubscriptionResponseTypeDef",
     "UpdateServiceNetworkRequestRequestTypeDef",
-    "UpdateServiceNetworkResponseTypeDef",
     "UpdateServiceNetworkVpcAssociationRequestRequestTypeDef",
-    "UpdateServiceNetworkVpcAssociationResponseTypeDef",
     "UpdateServiceRequestRequestTypeDef",
-    "UpdateServiceResponseTypeDef",
+    "CreateAccessLogSubscriptionResponseTypeDef",
+    "CreateServiceNetworkResponseTypeDef",
+    "CreateServiceNetworkVpcAssociationResponseTypeDef",
+    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
+    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
+    "DeleteServiceResponseTypeDef",
+    "DeleteTargetGroupResponseTypeDef",
+    "GetAccessLogSubscriptionResponseTypeDef",
+    "GetAuthPolicyResponseTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "GetServiceNetworkResponseTypeDef",
+    "GetServiceNetworkVpcAssociationResponseTypeDef",
     "ListAccessLogSubscriptionsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutAuthPolicyResponseTypeDef",
+    "UpdateAccessLogSubscriptionResponseTypeDef",
+    "UpdateServiceNetworkResponseTypeDef",
+    "UpdateServiceNetworkVpcAssociationResponseTypeDef",
+    "UpdateServiceResponseTypeDef",
     "CreateServiceNetworkServiceAssociationResponseTypeDef",
     "CreateServiceResponseTypeDef",
     "GetServiceNetworkServiceAssociationResponseTypeDef",
     "GetServiceResponseTypeDef",
     "ServiceNetworkServiceAssociationSummaryTypeDef",
     "ServiceSummaryTypeDef",
     "DeregisterTargetsRequestRequestTypeDef",
-    "ListTargetsRequestListTargetsPaginateTypeDef",
     "ListTargetsRequestRequestTypeDef",
     "RegisterTargetsRequestRequestTypeDef",
     "DeregisterTargetsResponseTypeDef",
     "RegisterTargetsResponseTypeDef",
+    "ForwardActionOutputTypeDef",
     "ForwardActionTypeDef",
+    "HeaderMatchOutputTypeDef",
     "HeaderMatchTypeDef",
+    "HealthCheckConfigOutputTypeDef",
     "HealthCheckConfigTypeDef",
+    "ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+    "ListListenersRequestListListenersPaginateTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
+    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
+    "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
+    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
+    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
+    "ListTargetsRequestListTargetsPaginateTypeDef",
     "ListListenersResponseTypeDef",
     "ListRulesResponseTypeDef",
     "ListServiceNetworkVpcAssociationsResponseTypeDef",
     "ListServiceNetworksResponseTypeDef",
     "ListTargetGroupsResponseTypeDef",
     "ListTargetsResponseTypeDef",
+    "PathMatchOutputTypeDef",
     "PathMatchTypeDef",
     "ListServiceNetworkServiceAssociationsResponseTypeDef",
     "ListServicesResponseTypeDef",
+    "RuleActionOutputTypeDef",
     "RuleActionTypeDef",
+    "TargetGroupConfigOutputTypeDef",
     "TargetGroupConfigTypeDef",
     "UpdateTargetGroupRequestRequestTypeDef",
+    "HttpMatchOutputTypeDef",
     "HttpMatchTypeDef",
-    "CreateListenerRequestRequestTypeDef",
     "CreateListenerResponseTypeDef",
     "GetListenerResponseTypeDef",
-    "UpdateListenerRequestRequestTypeDef",
     "UpdateListenerResponseTypeDef",
-    "CreateTargetGroupRequestRequestTypeDef",
+    "CreateListenerRequestRequestTypeDef",
+    "UpdateListenerRequestRequestTypeDef",
     "CreateTargetGroupResponseTypeDef",
     "GetTargetGroupResponseTypeDef",
     "UpdateTargetGroupResponseTypeDef",
+    "CreateTargetGroupRequestRequestTypeDef",
+    "RuleMatchOutputTypeDef",
     "RuleMatchTypeDef",
-    "CreateRuleRequestRequestTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "RuleUpdateSuccessTypeDef",
+    "UpdateRuleResponseTypeDef",
+    "CreateRuleRequestRequestTypeDef",
     "RuleUpdateTypeDef",
     "UpdateRuleRequestRequestTypeDef",
-    "UpdateRuleResponseTypeDef",
     "BatchUpdateRuleResponseTypeDef",
     "BatchUpdateRuleRequestRequestTypeDef",
 )
 
 AccessLogSubscriptionSummaryTypeDef = TypedDict(
     "AccessLogSubscriptionSummaryTypeDef",
     {
@@ -183,14 +197,25 @@
         "id": str,
         "lastUpdatedAt": datetime,
         "resourceArn": str,
         "resourceId": str,
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
 RuleUpdateFailureTypeDef = TypedDict(
     "RuleUpdateFailureTypeDef",
     {
         "failureCode": str,
         "failureMessage": str,
         "ruleIdentifier": str,
     },
@@ -217,26 +242,14 @@
 class CreateAccessLogSubscriptionRequestRequestTypeDef(
     _RequiredCreateAccessLogSubscriptionRequestRequestTypeDef,
     _OptionalCreateAccessLogSubscriptionRequestRequestTypeDef,
 ):
     pass
 
 
-CreateAccessLogSubscriptionResponseTypeDef = TypedDict(
-    "CreateAccessLogSubscriptionResponseTypeDef",
-    {
-        "arn": str,
-        "destinationArn": str,
-        "id": str,
-        "resourceArn": str,
-        "resourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateServiceNetworkRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceNetworkRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateServiceNetworkRequestRequestTypeDef = TypedDict(
@@ -253,25 +266,14 @@
 class CreateServiceNetworkRequestRequestTypeDef(
     _RequiredCreateServiceNetworkRequestRequestTypeDef,
     _OptionalCreateServiceNetworkRequestRequestTypeDef,
 ):
     pass
 
 
-CreateServiceNetworkResponseTypeDef = TypedDict(
-    "CreateServiceNetworkResponseTypeDef",
-    {
-        "arn": str,
-        "authType": AuthTypeType,
-        "id": str,
-        "name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateServiceNetworkServiceAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceNetworkServiceAssociationRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
         "serviceNetworkIdentifier": str,
     },
 )
@@ -322,26 +324,14 @@
 class CreateServiceNetworkVpcAssociationRequestRequestTypeDef(
     _RequiredCreateServiceNetworkVpcAssociationRequestRequestTypeDef,
     _OptionalCreateServiceNetworkVpcAssociationRequestRequestTypeDef,
 ):
     pass
 
 
-CreateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "CreateServiceNetworkVpcAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "createdBy": str,
-        "id": str,
-        "securityGroupIds": List[str],
-        "status": ServiceNetworkVpcAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateServiceRequestRequestTypeDef = TypedDict(
@@ -411,76 +401,35 @@
 DeleteServiceNetworkServiceAssociationRequestRequestTypeDef = TypedDict(
     "DeleteServiceNetworkServiceAssociationRequestRequestTypeDef",
     {
         "serviceNetworkServiceAssociationIdentifier": str,
     },
 )
 
-DeleteServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
-    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": ServiceNetworkServiceAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
     "DeleteServiceNetworkVpcAssociationRequestRequestTypeDef",
     {
         "serviceNetworkVpcAssociationIdentifier": str,
     },
 )
 
-DeleteServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": ServiceNetworkVpcAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteServiceRequestRequestTypeDef = TypedDict(
     "DeleteServiceRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
     },
 )
 
-DeleteServiceResponseTypeDef = TypedDict(
-    "DeleteServiceResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "status": ServiceStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTargetGroupRequestRequestTypeDef = TypedDict(
     "DeleteTargetGroupRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
     },
 )
 
-DeleteTargetGroupResponseTypeDef = TypedDict(
-    "DeleteTargetGroupResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": TargetGroupStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredTargetTypeDef = TypedDict(
     "_RequiredTargetTypeDef",
     {
         "id": str,
     },
 )
 _OptionalTargetTypeDef = TypedDict(
@@ -503,21 +452,68 @@
         "failureMessage": str,
         "id": str,
         "port": int,
     },
     total=False,
 )
 
+_RequiredTargetOutputTypeDef = TypedDict(
+    "_RequiredTargetOutputTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalTargetOutputTypeDef = TypedDict(
+    "_OptionalTargetOutputTypeDef",
+    {
+        "port": int,
+    },
+    total=False,
+)
+
+
+class TargetOutputTypeDef(_RequiredTargetOutputTypeDef, _OptionalTargetOutputTypeDef):
+    pass
+
+
+FixedResponseActionOutputTypeDef = TypedDict(
+    "FixedResponseActionOutputTypeDef",
+    {
+        "statusCode": int,
+    },
+)
+
 FixedResponseActionTypeDef = TypedDict(
     "FixedResponseActionTypeDef",
     {
         "statusCode": int,
     },
 )
 
+_RequiredWeightedTargetGroupOutputTypeDef = TypedDict(
+    "_RequiredWeightedTargetGroupOutputTypeDef",
+    {
+        "targetGroupIdentifier": str,
+    },
+)
+_OptionalWeightedTargetGroupOutputTypeDef = TypedDict(
+    "_OptionalWeightedTargetGroupOutputTypeDef",
+    {
+        "weight": int,
+    },
+    total=False,
+)
+
+
+class WeightedTargetGroupOutputTypeDef(
+    _RequiredWeightedTargetGroupOutputTypeDef, _OptionalWeightedTargetGroupOutputTypeDef
+):
+    pass
+
+
 _RequiredWeightedTargetGroupTypeDef = TypedDict(
     "_RequiredWeightedTargetGroupTypeDef",
     {
         "targetGroupIdentifier": str,
     },
 )
 _OptionalWeightedTargetGroupTypeDef = TypedDict(
@@ -538,46 +534,21 @@
 GetAccessLogSubscriptionRequestRequestTypeDef = TypedDict(
     "GetAccessLogSubscriptionRequestRequestTypeDef",
     {
         "accessLogSubscriptionIdentifier": str,
     },
 )
 
-GetAccessLogSubscriptionResponseTypeDef = TypedDict(
-    "GetAccessLogSubscriptionResponseTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "destinationArn": str,
-        "id": str,
-        "lastUpdatedAt": datetime,
-        "resourceArn": str,
-        "resourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAuthPolicyRequestRequestTypeDef = TypedDict(
     "GetAuthPolicyRequestRequestTypeDef",
     {
         "resourceIdentifier": str,
     },
 )
 
-GetAuthPolicyResponseTypeDef = TypedDict(
-    "GetAuthPolicyResponseTypeDef",
-    {
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "policy": str,
-        "state": AuthPolicyStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetListenerRequestRequestTypeDef = TypedDict(
     "GetListenerRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
         "serviceIdentifier": str,
     },
 )
@@ -585,22 +556,14 @@
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRuleRequestRequestTypeDef = TypedDict(
     "GetRuleRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
         "ruleIdentifier": str,
         "serviceIdentifier": str,
     },
@@ -609,117 +572,88 @@
 GetServiceNetworkRequestRequestTypeDef = TypedDict(
     "GetServiceNetworkRequestRequestTypeDef",
     {
         "serviceNetworkIdentifier": str,
     },
 )
 
-GetServiceNetworkResponseTypeDef = TypedDict(
-    "GetServiceNetworkResponseTypeDef",
-    {
-        "arn": str,
-        "authType": AuthTypeType,
-        "createdAt": datetime,
-        "id": str,
-        "lastUpdatedAt": datetime,
-        "name": str,
-        "numberOfAssociatedServices": int,
-        "numberOfAssociatedVPCs": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetServiceNetworkServiceAssociationRequestRequestTypeDef = TypedDict(
     "GetServiceNetworkServiceAssociationRequestRequestTypeDef",
     {
         "serviceNetworkServiceAssociationIdentifier": str,
     },
 )
 
 GetServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
     "GetServiceNetworkVpcAssociationRequestRequestTypeDef",
     {
         "serviceNetworkVpcAssociationIdentifier": str,
     },
 )
 
-GetServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "GetServiceNetworkVpcAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "createdBy": str,
-        "failureCode": str,
-        "failureMessage": str,
-        "id": str,
-        "lastUpdatedAt": datetime,
-        "securityGroupIds": List[str],
-        "serviceNetworkArn": str,
-        "serviceNetworkId": str,
-        "serviceNetworkName": str,
-        "status": ServiceNetworkVpcAssociationStatusType,
-        "vpcId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetServiceRequestRequestTypeDef = TypedDict(
     "GetServiceRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
     },
 )
 
 GetTargetGroupRequestRequestTypeDef = TypedDict(
     "GetTargetGroupRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
     },
 )
 
+HeaderMatchTypeOutputTypeDef = TypedDict(
+    "HeaderMatchTypeOutputTypeDef",
+    {
+        "contains": str,
+        "exact": str,
+        "prefix": str,
+    },
+    total=False,
+)
+
 HeaderMatchTypeTypeDef = TypedDict(
     "HeaderMatchTypeTypeDef",
     {
         "contains": str,
         "exact": str,
         "prefix": str,
     },
     total=False,
 )
 
-MatcherTypeDef = TypedDict(
-    "MatcherTypeDef",
+MatcherOutputTypeDef = TypedDict(
+    "MatcherOutputTypeDef",
     {
         "httpCode": str,
     },
     total=False,
 )
 
-_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
-    "_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+MatcherTypeDef = TypedDict(
+    "MatcherTypeDef",
     {
-        "resourceIdentifier": str,
+        "httpCode": str,
     },
+    total=False,
 )
-_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
-    "_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+
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
-class ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef(
-    _RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
-    _OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAccessLogSubscriptionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccessLogSubscriptionsRequestRequestTypeDef",
     {
         "resourceIdentifier": str,
     },
 )
 _OptionalListAccessLogSubscriptionsRequestRequestTypeDef = TypedDict(
@@ -735,36 +669,14 @@
 class ListAccessLogSubscriptionsRequestRequestTypeDef(
     _RequiredListAccessLogSubscriptionsRequestRequestTypeDef,
     _OptionalListAccessLogSubscriptionsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListListenersRequestListListenersPaginateTypeDef = TypedDict(
-    "_RequiredListListenersRequestListListenersPaginateTypeDef",
-    {
-        "serviceIdentifier": str,
-    },
-)
-_OptionalListListenersRequestListListenersPaginateTypeDef = TypedDict(
-    "_OptionalListListenersRequestListListenersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListListenersRequestListListenersPaginateTypeDef(
-    _RequiredListListenersRequestListListenersPaginateTypeDef,
-    _OptionalListListenersRequestListListenersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListListenersRequestRequestTypeDef = TypedDict(
     "_RequiredListListenersRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
     },
 )
 _OptionalListListenersRequestRequestTypeDef = TypedDict(
@@ -793,37 +705,14 @@
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
     },
     total=False,
 )
 
-_RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "_RequiredListRulesRequestListRulesPaginateTypeDef",
-    {
-        "listenerIdentifier": str,
-        "serviceIdentifier": str,
-    },
-)
-_OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "_OptionalListRulesRequestListRulesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRulesRequestListRulesPaginateTypeDef(
-    _RequiredListRulesRequestListRulesPaginateTypeDef,
-    _OptionalListRulesRequestListRulesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRulesRequestRequestTypeDef = TypedDict(
     "_RequiredListRulesRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
         "serviceIdentifier": str,
     },
 )
@@ -853,47 +742,25 @@
         "lastUpdatedAt": datetime,
         "name": str,
         "priority": int,
     },
     total=False,
 )
 
-ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef = TypedDict(
-    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
-    {
-        "serviceIdentifier": str,
-        "serviceNetworkIdentifier": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServiceNetworkServiceAssociationsRequestRequestTypeDef = TypedDict(
     "ListServiceNetworkServiceAssociationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "serviceIdentifier": str,
         "serviceNetworkIdentifier": str,
     },
     total=False,
 )
 
-ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef = (
-    TypedDict(
-        "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
-        {
-            "serviceNetworkIdentifier": str,
-            "vpcIdentifier": str,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
 ListServiceNetworkVpcAssociationsRequestRequestTypeDef = TypedDict(
     "ListServiceNetworkVpcAssociationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "serviceNetworkIdentifier": str,
         "vpcIdentifier": str,
@@ -914,22 +781,14 @@
         "serviceNetworkName": str,
         "status": ServiceNetworkVpcAssociationStatusType,
         "vpcId": str,
     },
     total=False,
 )
 
-ListServiceNetworksRequestListServiceNetworksPaginateTypeDef = TypedDict(
-    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServiceNetworksRequestRequestTypeDef = TypedDict(
     "ListServiceNetworksRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -945,22 +804,14 @@
         "name": str,
         "numberOfAssociatedServices": int,
         "numberOfAssociatedVPCs": int,
     },
     total=False,
 )
 
-ListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "ListServicesRequestListServicesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -969,32 +820,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTargetGroupsRequestListTargetGroupsPaginateTypeDef = TypedDict(
-    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
-    {
-        "targetGroupType": TargetGroupTypeType,
-        "vpcIdentifier": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTargetGroupsRequestRequestTypeDef = TypedDict(
     "ListTargetGroupsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "targetGroupType": TargetGroupTypeType,
         "vpcIdentifier": str,
@@ -1028,20 +861,19 @@
         "port": int,
         "reasonCode": str,
         "status": TargetStatusType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+PathMatchTypeOutputTypeDef = TypedDict(
+    "PathMatchTypeOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "exact": str,
+        "prefix": str,
     },
     total=False,
 )
 
 PathMatchTypeTypeDef = TypedDict(
     "PathMatchTypeTypeDef",
     {
@@ -1055,42 +887,22 @@
     "PutAuthPolicyRequestRequestTypeDef",
     {
         "policy": str,
         "resourceIdentifier": str,
     },
 )
 
-PutAuthPolicyResponseTypeDef = TypedDict(
-    "PutAuthPolicyResponseTypeDef",
-    {
-        "policy": str,
-        "state": AuthPolicyStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1107,134 +919,295 @@
     "UpdateAccessLogSubscriptionRequestRequestTypeDef",
     {
         "accessLogSubscriptionIdentifier": str,
         "destinationArn": str,
     },
 )
 
-UpdateAccessLogSubscriptionResponseTypeDef = TypedDict(
-    "UpdateAccessLogSubscriptionResponseTypeDef",
+UpdateServiceNetworkRequestRequestTypeDef = TypedDict(
+    "UpdateServiceNetworkRequestRequestTypeDef",
+    {
+        "authType": AuthTypeType,
+        "serviceNetworkIdentifier": str,
+    },
+)
+
+UpdateServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
+    "UpdateServiceNetworkVpcAssociationRequestRequestTypeDef",
+    {
+        "securityGroupIds": Sequence[str],
+        "serviceNetworkVpcAssociationIdentifier": str,
+    },
+)
+
+_RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateServiceRequestRequestTypeDef",
+    {
+        "serviceIdentifier": str,
+    },
+)
+_OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateServiceRequestRequestTypeDef",
+    {
+        "authType": AuthTypeType,
+        "certificateArn": str,
+    },
+    total=False,
+)
+
+
+class UpdateServiceRequestRequestTypeDef(
+    _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
+):
+    pass
+
+
+CreateAccessLogSubscriptionResponseTypeDef = TypedDict(
+    "CreateAccessLogSubscriptionResponseTypeDef",
     {
         "arn": str,
         "destinationArn": str,
         "id": str,
         "resourceArn": str,
         "resourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateServiceNetworkRequestRequestTypeDef = TypedDict(
-    "UpdateServiceNetworkRequestRequestTypeDef",
+CreateServiceNetworkResponseTypeDef = TypedDict(
+    "CreateServiceNetworkResponseTypeDef",
     {
+        "arn": str,
         "authType": AuthTypeType,
-        "serviceNetworkIdentifier": str,
+        "id": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateServiceNetworkResponseTypeDef = TypedDict(
-    "UpdateServiceNetworkResponseTypeDef",
+CreateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "CreateServiceNetworkVpcAssociationResponseTypeDef",
     {
         "arn": str,
-        "authType": AuthTypeType,
+        "createdBy": str,
         "id": str,
-        "name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "securityGroupIds": List[str],
+        "status": ServiceNetworkVpcAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
-    "UpdateServiceNetworkVpcAssociationRequestRequestTypeDef",
+DeleteServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
+    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
     {
-        "securityGroupIds": Sequence[str],
-        "serviceNetworkVpcAssociationIdentifier": str,
+        "arn": str,
+        "id": str,
+        "status": ServiceNetworkServiceAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "UpdateServiceNetworkVpcAssociationResponseTypeDef",
+DeleteServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
     {
         "arn": str,
-        "createdBy": str,
         "id": str,
-        "securityGroupIds": List[str],
         "status": ServiceNetworkVpcAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateServiceRequestRequestTypeDef",
+DeleteServiceResponseTypeDef = TypedDict(
+    "DeleteServiceResponseTypeDef",
     {
-        "serviceIdentifier": str,
+        "arn": str,
+        "id": str,
+        "name": str,
+        "status": ServiceStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateServiceRequestRequestTypeDef",
+
+DeleteTargetGroupResponseTypeDef = TypedDict(
+    "DeleteTargetGroupResponseTypeDef",
     {
-        "authType": AuthTypeType,
-        "certificateArn": str,
+        "arn": str,
+        "id": str,
+        "status": TargetGroupStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+GetAccessLogSubscriptionResponseTypeDef = TypedDict(
+    "GetAccessLogSubscriptionResponseTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "destinationArn": str,
+        "id": str,
+        "lastUpdatedAt": datetime,
+        "resourceArn": str,
+        "resourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class UpdateServiceRequestRequestTypeDef(
-    _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
-):
-    pass
+GetAuthPolicyResponseTypeDef = TypedDict(
+    "GetAuthPolicyResponseTypeDef",
+    {
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "policy": str,
+        "state": AuthPolicyStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-UpdateServiceResponseTypeDef = TypedDict(
-    "UpdateServiceResponseTypeDef",
+GetServiceNetworkResponseTypeDef = TypedDict(
+    "GetServiceNetworkResponseTypeDef",
     {
         "arn": str,
         "authType": AuthTypeType,
-        "certificateArn": str,
-        "customDomainName": str,
+        "createdAt": datetime,
         "id": str,
+        "lastUpdatedAt": datetime,
         "name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "numberOfAssociatedServices": int,
+        "numberOfAssociatedVPCs": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "GetServiceNetworkVpcAssociationResponseTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "createdBy": str,
+        "failureCode": str,
+        "failureMessage": str,
+        "id": str,
+        "lastUpdatedAt": datetime,
+        "securityGroupIds": List[str],
+        "serviceNetworkArn": str,
+        "serviceNetworkId": str,
+        "serviceNetworkName": str,
+        "status": ServiceNetworkVpcAssociationStatusType,
+        "vpcId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccessLogSubscriptionsResponseTypeDef = TypedDict(
     "ListAccessLogSubscriptionsResponseTypeDef",
     {
         "items": List[AccessLogSubscriptionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutAuthPolicyResponseTypeDef = TypedDict(
+    "PutAuthPolicyResponseTypeDef",
+    {
+        "policy": str,
+        "state": AuthPolicyStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAccessLogSubscriptionResponseTypeDef = TypedDict(
+    "UpdateAccessLogSubscriptionResponseTypeDef",
+    {
+        "arn": str,
+        "destinationArn": str,
+        "id": str,
+        "resourceArn": str,
+        "resourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateServiceNetworkResponseTypeDef = TypedDict(
+    "UpdateServiceNetworkResponseTypeDef",
+    {
+        "arn": str,
+        "authType": AuthTypeType,
+        "id": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "UpdateServiceNetworkVpcAssociationResponseTypeDef",
+    {
+        "arn": str,
+        "createdBy": str,
+        "id": str,
+        "securityGroupIds": List[str],
+        "status": ServiceNetworkVpcAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateServiceResponseTypeDef = TypedDict(
+    "UpdateServiceResponseTypeDef",
+    {
+        "arn": str,
+        "authType": AuthTypeType,
+        "certificateArn": str,
+        "customDomainName": str,
+        "id": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
     "CreateServiceNetworkServiceAssociationResponseTypeDef",
     {
         "arn": str,
         "createdBy": str,
         "customDomainName": str,
         "dnsEntry": DnsEntryTypeDef,
         "id": str,
         "status": ServiceNetworkServiceAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "arn": str,
         "authType": AuthTypeType,
         "certificateArn": str,
         "customDomainName": str,
         "dnsEntry": DnsEntryTypeDef,
         "id": str,
         "name": str,
         "status": ServiceStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
     "GetServiceNetworkServiceAssociationResponseTypeDef",
     {
         "arn": str,
@@ -1248,15 +1221,15 @@
         "serviceArn": str,
         "serviceId": str,
         "serviceName": str,
         "serviceNetworkArn": str,
         "serviceNetworkId": str,
         "serviceNetworkName": str,
         "status": ServiceNetworkServiceAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceResponseTypeDef = TypedDict(
     "GetServiceResponseTypeDef",
     {
         "arn": str,
@@ -1267,15 +1240,15 @@
         "dnsEntry": DnsEntryTypeDef,
         "failureCode": str,
         "failureMessage": str,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "status": ServiceStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ServiceNetworkServiceAssociationSummaryTypeDef = TypedDict(
     "ServiceNetworkServiceAssociationSummaryTypeDef",
     {
         "arn": str,
@@ -1314,37 +1287,14 @@
     "DeregisterTargetsRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
         "targets": Sequence[TargetTypeDef],
     },
 )
 
-_RequiredListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
-    "_RequiredListTargetsRequestListTargetsPaginateTypeDef",
-    {
-        "targetGroupIdentifier": str,
-    },
-)
-_OptionalListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
-    "_OptionalListTargetsRequestListTargetsPaginateTypeDef",
-    {
-        "targets": Sequence[TargetTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTargetsRequestListTargetsPaginateTypeDef(
-    _RequiredListTargetsRequestListTargetsPaginateTypeDef,
-    _OptionalListTargetsRequestListTargetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredListTargetsRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
     },
 )
 _OptionalListTargetsRequestRequestTypeDef = TypedDict(
@@ -1371,36 +1321,65 @@
         "targets": Sequence[TargetTypeDef],
     },
 )
 
 DeregisterTargetsResponseTypeDef = TypedDict(
     "DeregisterTargetsResponseTypeDef",
     {
-        "successful": List[TargetTypeDef],
+        "successful": List[TargetOutputTypeDef],
         "unsuccessful": List[TargetFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterTargetsResponseTypeDef = TypedDict(
     "RegisterTargetsResponseTypeDef",
     {
-        "successful": List[TargetTypeDef],
+        "successful": List[TargetOutputTypeDef],
         "unsuccessful": List[TargetFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ForwardActionOutputTypeDef = TypedDict(
+    "ForwardActionOutputTypeDef",
+    {
+        "targetGroups": List[WeightedTargetGroupOutputTypeDef],
     },
 )
 
 ForwardActionTypeDef = TypedDict(
     "ForwardActionTypeDef",
     {
         "targetGroups": Sequence[WeightedTargetGroupTypeDef],
     },
 )
 
+_RequiredHeaderMatchOutputTypeDef = TypedDict(
+    "_RequiredHeaderMatchOutputTypeDef",
+    {
+        "match": HeaderMatchTypeOutputTypeDef,
+        "name": str,
+    },
+)
+_OptionalHeaderMatchOutputTypeDef = TypedDict(
+    "_OptionalHeaderMatchOutputTypeDef",
+    {
+        "caseSensitive": bool,
+    },
+    total=False,
+)
+
+
+class HeaderMatchOutputTypeDef(
+    _RequiredHeaderMatchOutputTypeDef, _OptionalHeaderMatchOutputTypeDef
+):
+    pass
+
+
 _RequiredHeaderMatchTypeDef = TypedDict(
     "_RequiredHeaderMatchTypeDef",
     {
         "match": HeaderMatchTypeTypeDef,
         "name": str,
     },
 )
@@ -1413,14 +1392,31 @@
 )
 
 
 class HeaderMatchTypeDef(_RequiredHeaderMatchTypeDef, _OptionalHeaderMatchTypeDef):
     pass
 
 
+HealthCheckConfigOutputTypeDef = TypedDict(
+    "HealthCheckConfigOutputTypeDef",
+    {
+        "enabled": bool,
+        "healthCheckIntervalSeconds": int,
+        "healthCheckTimeoutSeconds": int,
+        "healthyThresholdCount": int,
+        "matcher": MatcherOutputTypeDef,
+        "path": str,
+        "port": int,
+        "protocol": TargetGroupProtocolType,
+        "protocolVersion": HealthCheckProtocolVersionType,
+        "unhealthyThresholdCount": int,
+    },
+    total=False,
+)
+
 HealthCheckConfigTypeDef = TypedDict(
     "HealthCheckConfigTypeDef",
     {
         "enabled": bool,
         "healthCheckIntervalSeconds": int,
         "healthCheckTimeoutSeconds": int,
         "healthyThresholdCount": int,
@@ -1430,68 +1426,225 @@
         "protocol": TargetGroupProtocolType,
         "protocolVersion": HealthCheckProtocolVersionType,
         "unhealthyThresholdCount": int,
     },
     total=False,
 )
 
+_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
+    "_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+    {
+        "resourceIdentifier": str,
+    },
+)
+_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
+    "_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef(
+    _RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+    _OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListListenersRequestListListenersPaginateTypeDef = TypedDict(
+    "_RequiredListListenersRequestListListenersPaginateTypeDef",
+    {
+        "serviceIdentifier": str,
+    },
+)
+_OptionalListListenersRequestListListenersPaginateTypeDef = TypedDict(
+    "_OptionalListListenersRequestListListenersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListListenersRequestListListenersPaginateTypeDef(
+    _RequiredListListenersRequestListListenersPaginateTypeDef,
+    _OptionalListListenersRequestListListenersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "_RequiredListRulesRequestListRulesPaginateTypeDef",
+    {
+        "listenerIdentifier": str,
+        "serviceIdentifier": str,
+    },
+)
+_OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "_OptionalListRulesRequestListRulesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRulesRequestListRulesPaginateTypeDef(
+    _RequiredListRulesRequestListRulesPaginateTypeDef,
+    _OptionalListRulesRequestListRulesPaginateTypeDef,
+):
+    pass
+
+
+ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef = TypedDict(
+    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
+    {
+        "serviceIdentifier": str,
+        "serviceNetworkIdentifier": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef = (
+    TypedDict(
+        "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
+        {
+            "serviceNetworkIdentifier": str,
+            "vpcIdentifier": str,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+ListServiceNetworksRequestListServiceNetworksPaginateTypeDef = TypedDict(
+    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "ListServicesRequestListServicesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTargetGroupsRequestListTargetGroupsPaginateTypeDef = TypedDict(
+    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
+    {
+        "targetGroupType": TargetGroupTypeType,
+        "vpcIdentifier": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
+    "_RequiredListTargetsRequestListTargetsPaginateTypeDef",
+    {
+        "targetGroupIdentifier": str,
+    },
+)
+_OptionalListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
+    "_OptionalListTargetsRequestListTargetsPaginateTypeDef",
+    {
+        "targets": Sequence[TargetTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTargetsRequestListTargetsPaginateTypeDef(
+    _RequiredListTargetsRequestListTargetsPaginateTypeDef,
+    _OptionalListTargetsRequestListTargetsPaginateTypeDef,
+):
+    pass
+
+
 ListListenersResponseTypeDef = TypedDict(
     "ListListenersResponseTypeDef",
     {
         "items": List[ListenerSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "items": List[RuleSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceNetworkVpcAssociationsResponseTypeDef = TypedDict(
     "ListServiceNetworkVpcAssociationsResponseTypeDef",
     {
         "items": List[ServiceNetworkVpcAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceNetworksResponseTypeDef = TypedDict(
     "ListServiceNetworksResponseTypeDef",
     {
         "items": List[ServiceNetworkSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetGroupsResponseTypeDef = TypedDict(
     "ListTargetGroupsResponseTypeDef",
     {
         "items": List[TargetGroupSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetsResponseTypeDef = TypedDict(
     "ListTargetsResponseTypeDef",
     {
         "items": List[TargetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPathMatchOutputTypeDef = TypedDict(
+    "_RequiredPathMatchOutputTypeDef",
+    {
+        "match": PathMatchTypeOutputTypeDef,
+    },
+)
+_OptionalPathMatchOutputTypeDef = TypedDict(
+    "_OptionalPathMatchOutputTypeDef",
+    {
+        "caseSensitive": bool,
+    },
+    total=False,
+)
+
+
+class PathMatchOutputTypeDef(_RequiredPathMatchOutputTypeDef, _OptionalPathMatchOutputTypeDef):
+    pass
+
+
 _RequiredPathMatchTypeDef = TypedDict(
     "_RequiredPathMatchTypeDef",
     {
         "match": PathMatchTypeTypeDef,
     },
 )
 _OptionalPathMatchTypeDef = TypedDict(
@@ -1508,36 +1661,70 @@
 
 
 ListServiceNetworkServiceAssociationsResponseTypeDef = TypedDict(
     "ListServiceNetworkServiceAssociationsResponseTypeDef",
     {
         "items": List[ServiceNetworkServiceAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "items": List[ServiceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RuleActionOutputTypeDef = TypedDict(
+    "RuleActionOutputTypeDef",
+    {
+        "fixedResponse": FixedResponseActionOutputTypeDef,
+        "forward": ForwardActionOutputTypeDef,
+    },
+    total=False,
+)
+
 RuleActionTypeDef = TypedDict(
     "RuleActionTypeDef",
     {
         "fixedResponse": FixedResponseActionTypeDef,
         "forward": ForwardActionTypeDef,
     },
     total=False,
 )
 
+_RequiredTargetGroupConfigOutputTypeDef = TypedDict(
+    "_RequiredTargetGroupConfigOutputTypeDef",
+    {
+        "port": int,
+        "protocol": TargetGroupProtocolType,
+        "vpcIdentifier": str,
+    },
+)
+_OptionalTargetGroupConfigOutputTypeDef = TypedDict(
+    "_OptionalTargetGroupConfigOutputTypeDef",
+    {
+        "healthCheck": HealthCheckConfigOutputTypeDef,
+        "ipAddressType": IpAddressTypeType,
+        "protocolVersion": TargetGroupProtocolVersionType,
+    },
+    total=False,
+)
+
+
+class TargetGroupConfigOutputTypeDef(
+    _RequiredTargetGroupConfigOutputTypeDef, _OptionalTargetGroupConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredTargetGroupConfigTypeDef = TypedDict(
     "_RequiredTargetGroupConfigTypeDef",
     {
         "port": int,
         "protocol": TargetGroupProtocolType,
         "vpcIdentifier": str,
     },
@@ -1563,252 +1750,284 @@
     "UpdateTargetGroupRequestRequestTypeDef",
     {
         "healthCheck": HealthCheckConfigTypeDef,
         "targetGroupIdentifier": str,
     },
 )
 
-HttpMatchTypeDef = TypedDict(
-    "HttpMatchTypeDef",
+HttpMatchOutputTypeDef = TypedDict(
+    "HttpMatchOutputTypeDef",
     {
-        "headerMatches": Sequence[HeaderMatchTypeDef],
+        "headerMatches": List[HeaderMatchOutputTypeDef],
         "method": str,
-        "pathMatch": PathMatchTypeDef,
+        "pathMatch": PathMatchOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateListenerRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateListenerRequestRequestTypeDef",
-    {
-        "defaultAction": RuleActionTypeDef,
-        "name": str,
-        "protocol": ListenerProtocolType,
-        "serviceIdentifier": str,
-    },
-)
-_OptionalCreateListenerRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateListenerRequestRequestTypeDef",
+HttpMatchTypeDef = TypedDict(
+    "HttpMatchTypeDef",
     {
-        "clientToken": str,
-        "port": int,
-        "tags": Mapping[str, str],
+        "headerMatches": Sequence[HeaderMatchTypeDef],
+        "method": str,
+        "pathMatch": PathMatchTypeDef,
     },
     total=False,
 )
 
-
-class CreateListenerRequestRequestTypeDef(
-    _RequiredCreateListenerRequestRequestTypeDef, _OptionalCreateListenerRequestRequestTypeDef
-):
-    pass
-
-
 CreateListenerResponseTypeDef = TypedDict(
     "CreateListenerResponseTypeDef",
     {
         "arn": str,
-        "defaultAction": RuleActionTypeDef,
+        "defaultAction": RuleActionOutputTypeDef,
         "id": str,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetListenerResponseTypeDef = TypedDict(
     "GetListenerResponseTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
-        "defaultAction": RuleActionTypeDef,
+        "defaultAction": RuleActionOutputTypeDef,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateListenerRequestRequestTypeDef = TypedDict(
-    "UpdateListenerRequestRequestTypeDef",
-    {
-        "defaultAction": RuleActionTypeDef,
-        "listenerIdentifier": str,
-        "serviceIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateListenerResponseTypeDef = TypedDict(
     "UpdateListenerResponseTypeDef",
     {
         "arn": str,
-        "defaultAction": RuleActionTypeDef,
+        "defaultAction": RuleActionOutputTypeDef,
         "id": str,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateTargetGroupRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTargetGroupRequestRequestTypeDef",
+_RequiredCreateListenerRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateListenerRequestRequestTypeDef",
     {
+        "defaultAction": RuleActionTypeDef,
         "name": str,
-        "type": TargetGroupTypeType,
+        "protocol": ListenerProtocolType,
+        "serviceIdentifier": str,
     },
 )
-_OptionalCreateTargetGroupRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTargetGroupRequestRequestTypeDef",
+_OptionalCreateListenerRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateListenerRequestRequestTypeDef",
     {
         "clientToken": str,
-        "config": TargetGroupConfigTypeDef,
+        "port": int,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class CreateTargetGroupRequestRequestTypeDef(
-    _RequiredCreateTargetGroupRequestRequestTypeDef, _OptionalCreateTargetGroupRequestRequestTypeDef
+class CreateListenerRequestRequestTypeDef(
+    _RequiredCreateListenerRequestRequestTypeDef, _OptionalCreateListenerRequestRequestTypeDef
 ):
     pass
 
 
+UpdateListenerRequestRequestTypeDef = TypedDict(
+    "UpdateListenerRequestRequestTypeDef",
+    {
+        "defaultAction": RuleActionTypeDef,
+        "listenerIdentifier": str,
+        "serviceIdentifier": str,
+    },
+)
+
 CreateTargetGroupResponseTypeDef = TypedDict(
     "CreateTargetGroupResponseTypeDef",
     {
         "arn": str,
-        "config": TargetGroupConfigTypeDef,
+        "config": TargetGroupConfigOutputTypeDef,
         "id": str,
         "name": str,
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTargetGroupResponseTypeDef = TypedDict(
     "GetTargetGroupResponseTypeDef",
     {
         "arn": str,
-        "config": TargetGroupConfigTypeDef,
+        "config": TargetGroupConfigOutputTypeDef,
         "createdAt": datetime,
         "failureCode": str,
         "failureMessage": str,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "serviceArns": List[str],
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTargetGroupResponseTypeDef = TypedDict(
     "UpdateTargetGroupResponseTypeDef",
     {
         "arn": str,
-        "config": TargetGroupConfigTypeDef,
+        "config": TargetGroupConfigOutputTypeDef,
         "id": str,
         "name": str,
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RuleMatchTypeDef = TypedDict(
-    "RuleMatchTypeDef",
-    {
-        "httpMatch": HttpMatchTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRuleRequestRequestTypeDef",
+_RequiredCreateTargetGroupRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTargetGroupRequestRequestTypeDef",
     {
-        "action": RuleActionTypeDef,
-        "listenerIdentifier": str,
-        "match": RuleMatchTypeDef,
         "name": str,
-        "priority": int,
-        "serviceIdentifier": str,
+        "type": TargetGroupTypeType,
     },
 )
-_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRuleRequestRequestTypeDef",
+_OptionalCreateTargetGroupRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTargetGroupRequestRequestTypeDef",
     {
         "clientToken": str,
+        "config": TargetGroupConfigTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class CreateRuleRequestRequestTypeDef(
-    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
+class CreateTargetGroupRequestRequestTypeDef(
+    _RequiredCreateTargetGroupRequestRequestTypeDef, _OptionalCreateTargetGroupRequestRequestTypeDef
 ):
     pass
 
 
+RuleMatchOutputTypeDef = TypedDict(
+    "RuleMatchOutputTypeDef",
+    {
+        "httpMatch": HttpMatchOutputTypeDef,
+    },
+    total=False,
+)
+
+RuleMatchTypeDef = TypedDict(
+    "RuleMatchTypeDef",
+    {
+        "httpMatch": HttpMatchTypeDef,
+    },
+    total=False,
+)
+
 CreateRuleResponseTypeDef = TypedDict(
     "CreateRuleResponseTypeDef",
     {
-        "action": RuleActionTypeDef,
+        "action": RuleActionOutputTypeDef,
         "arn": str,
         "id": str,
-        "match": RuleMatchTypeDef,
+        "match": RuleMatchOutputTypeDef,
         "name": str,
         "priority": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
-        "action": RuleActionTypeDef,
+        "action": RuleActionOutputTypeDef,
         "arn": str,
         "createdAt": datetime,
         "id": str,
         "isDefault": bool,
         "lastUpdatedAt": datetime,
-        "match": RuleMatchTypeDef,
+        "match": RuleMatchOutputTypeDef,
         "name": str,
         "priority": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RuleUpdateSuccessTypeDef = TypedDict(
     "RuleUpdateSuccessTypeDef",
     {
-        "action": RuleActionTypeDef,
+        "action": RuleActionOutputTypeDef,
         "arn": str,
         "id": str,
         "isDefault": bool,
+        "match": RuleMatchOutputTypeDef,
+        "name": str,
+        "priority": int,
+    },
+    total=False,
+)
+
+UpdateRuleResponseTypeDef = TypedDict(
+    "UpdateRuleResponseTypeDef",
+    {
+        "action": RuleActionOutputTypeDef,
+        "arn": str,
+        "id": str,
+        "isDefault": bool,
+        "match": RuleMatchOutputTypeDef,
+        "name": str,
+        "priority": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRuleRequestRequestTypeDef",
+    {
+        "action": RuleActionTypeDef,
+        "listenerIdentifier": str,
         "match": RuleMatchTypeDef,
         "name": str,
         "priority": int,
+        "serviceIdentifier": str,
+    },
+)
+_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRuleRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
+class CreateRuleRequestRequestTypeDef(
+    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredRuleUpdateTypeDef = TypedDict(
     "_RequiredRuleUpdateTypeDef",
     {
         "ruleIdentifier": str,
     },
 )
 _OptionalRuleUpdateTypeDef = TypedDict(
@@ -1847,34 +2066,20 @@
 
 class UpdateRuleRequestRequestTypeDef(
     _RequiredUpdateRuleRequestRequestTypeDef, _OptionalUpdateRuleRequestRequestTypeDef
 ):
     pass
 
 
-UpdateRuleResponseTypeDef = TypedDict(
-    "UpdateRuleResponseTypeDef",
-    {
-        "action": RuleActionTypeDef,
-        "arn": str,
-        "id": str,
-        "isDefault": bool,
-        "match": RuleMatchTypeDef,
-        "name": str,
-        "priority": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchUpdateRuleResponseTypeDef = TypedDict(
     "BatchUpdateRuleResponseTypeDef",
     {
         "successful": List[RuleUpdateSuccessTypeDef],
         "unsuccessful": List[RuleUpdateFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateRuleRequestRequestTypeDef = TypedDict(
     "BatchUpdateRuleRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
```

### Comparing `mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice/type_defs.pyi` & `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -34,145 +34,159 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessLogSubscriptionSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "RuleUpdateFailureTypeDef",
     "CreateAccessLogSubscriptionRequestRequestTypeDef",
-    "CreateAccessLogSubscriptionResponseTypeDef",
     "CreateServiceNetworkRequestRequestTypeDef",
-    "CreateServiceNetworkResponseTypeDef",
     "CreateServiceNetworkServiceAssociationRequestRequestTypeDef",
     "DnsEntryTypeDef",
     "CreateServiceNetworkVpcAssociationRequestRequestTypeDef",
-    "CreateServiceNetworkVpcAssociationResponseTypeDef",
     "CreateServiceRequestRequestTypeDef",
     "DeleteAccessLogSubscriptionRequestRequestTypeDef",
     "DeleteAuthPolicyRequestRequestTypeDef",
     "DeleteListenerRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "DeleteServiceNetworkRequestRequestTypeDef",
     "DeleteServiceNetworkServiceAssociationRequestRequestTypeDef",
-    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
     "DeleteServiceNetworkVpcAssociationRequestRequestTypeDef",
-    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
     "DeleteServiceRequestRequestTypeDef",
-    "DeleteServiceResponseTypeDef",
     "DeleteTargetGroupRequestRequestTypeDef",
-    "DeleteTargetGroupResponseTypeDef",
     "TargetTypeDef",
     "TargetFailureTypeDef",
+    "TargetOutputTypeDef",
+    "FixedResponseActionOutputTypeDef",
     "FixedResponseActionTypeDef",
+    "WeightedTargetGroupOutputTypeDef",
     "WeightedTargetGroupTypeDef",
     "GetAccessLogSubscriptionRequestRequestTypeDef",
-    "GetAccessLogSubscriptionResponseTypeDef",
     "GetAuthPolicyRequestRequestTypeDef",
-    "GetAuthPolicyResponseTypeDef",
     "GetListenerRequestRequestTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
     "GetRuleRequestRequestTypeDef",
     "GetServiceNetworkRequestRequestTypeDef",
-    "GetServiceNetworkResponseTypeDef",
     "GetServiceNetworkServiceAssociationRequestRequestTypeDef",
     "GetServiceNetworkVpcAssociationRequestRequestTypeDef",
-    "GetServiceNetworkVpcAssociationResponseTypeDef",
     "GetServiceRequestRequestTypeDef",
     "GetTargetGroupRequestRequestTypeDef",
+    "HeaderMatchTypeOutputTypeDef",
     "HeaderMatchTypeTypeDef",
+    "MatcherOutputTypeDef",
     "MatcherTypeDef",
-    "ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccessLogSubscriptionsRequestRequestTypeDef",
-    "ListListenersRequestListListenersPaginateTypeDef",
     "ListListenersRequestRequestTypeDef",
     "ListenerSummaryTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
     "RuleSummaryTypeDef",
-    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
     "ListServiceNetworkServiceAssociationsRequestRequestTypeDef",
-    "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
     "ListServiceNetworkVpcAssociationsRequestRequestTypeDef",
     "ServiceNetworkVpcAssociationSummaryTypeDef",
-    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
     "ListServiceNetworksRequestRequestTypeDef",
     "ServiceNetworkSummaryTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
     "ListTargetGroupsRequestRequestTypeDef",
     "TargetGroupSummaryTypeDef",
     "TargetSummaryTypeDef",
-    "PaginatorConfigTypeDef",
+    "PathMatchTypeOutputTypeDef",
     "PathMatchTypeTypeDef",
     "PutAuthPolicyRequestRequestTypeDef",
-    "PutAuthPolicyResponseTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccessLogSubscriptionRequestRequestTypeDef",
-    "UpdateAccessLogSubscriptionResponseTypeDef",
     "UpdateServiceNetworkRequestRequestTypeDef",
-    "UpdateServiceNetworkResponseTypeDef",
     "UpdateServiceNetworkVpcAssociationRequestRequestTypeDef",
-    "UpdateServiceNetworkVpcAssociationResponseTypeDef",
     "UpdateServiceRequestRequestTypeDef",
-    "UpdateServiceResponseTypeDef",
+    "CreateAccessLogSubscriptionResponseTypeDef",
+    "CreateServiceNetworkResponseTypeDef",
+    "CreateServiceNetworkVpcAssociationResponseTypeDef",
+    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
+    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
+    "DeleteServiceResponseTypeDef",
+    "DeleteTargetGroupResponseTypeDef",
+    "GetAccessLogSubscriptionResponseTypeDef",
+    "GetAuthPolicyResponseTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "GetServiceNetworkResponseTypeDef",
+    "GetServiceNetworkVpcAssociationResponseTypeDef",
     "ListAccessLogSubscriptionsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutAuthPolicyResponseTypeDef",
+    "UpdateAccessLogSubscriptionResponseTypeDef",
+    "UpdateServiceNetworkResponseTypeDef",
+    "UpdateServiceNetworkVpcAssociationResponseTypeDef",
+    "UpdateServiceResponseTypeDef",
     "CreateServiceNetworkServiceAssociationResponseTypeDef",
     "CreateServiceResponseTypeDef",
     "GetServiceNetworkServiceAssociationResponseTypeDef",
     "GetServiceResponseTypeDef",
     "ServiceNetworkServiceAssociationSummaryTypeDef",
     "ServiceSummaryTypeDef",
     "DeregisterTargetsRequestRequestTypeDef",
-    "ListTargetsRequestListTargetsPaginateTypeDef",
     "ListTargetsRequestRequestTypeDef",
     "RegisterTargetsRequestRequestTypeDef",
     "DeregisterTargetsResponseTypeDef",
     "RegisterTargetsResponseTypeDef",
+    "ForwardActionOutputTypeDef",
     "ForwardActionTypeDef",
+    "HeaderMatchOutputTypeDef",
     "HeaderMatchTypeDef",
+    "HealthCheckConfigOutputTypeDef",
     "HealthCheckConfigTypeDef",
+    "ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+    "ListListenersRequestListListenersPaginateTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
+    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
+    "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
+    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
+    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
+    "ListTargetsRequestListTargetsPaginateTypeDef",
     "ListListenersResponseTypeDef",
     "ListRulesResponseTypeDef",
     "ListServiceNetworkVpcAssociationsResponseTypeDef",
     "ListServiceNetworksResponseTypeDef",
     "ListTargetGroupsResponseTypeDef",
     "ListTargetsResponseTypeDef",
+    "PathMatchOutputTypeDef",
     "PathMatchTypeDef",
     "ListServiceNetworkServiceAssociationsResponseTypeDef",
     "ListServicesResponseTypeDef",
+    "RuleActionOutputTypeDef",
     "RuleActionTypeDef",
+    "TargetGroupConfigOutputTypeDef",
     "TargetGroupConfigTypeDef",
     "UpdateTargetGroupRequestRequestTypeDef",
+    "HttpMatchOutputTypeDef",
     "HttpMatchTypeDef",
-    "CreateListenerRequestRequestTypeDef",
     "CreateListenerResponseTypeDef",
     "GetListenerResponseTypeDef",
-    "UpdateListenerRequestRequestTypeDef",
     "UpdateListenerResponseTypeDef",
-    "CreateTargetGroupRequestRequestTypeDef",
+    "CreateListenerRequestRequestTypeDef",
+    "UpdateListenerRequestRequestTypeDef",
     "CreateTargetGroupResponseTypeDef",
     "GetTargetGroupResponseTypeDef",
     "UpdateTargetGroupResponseTypeDef",
+    "CreateTargetGroupRequestRequestTypeDef",
+    "RuleMatchOutputTypeDef",
     "RuleMatchTypeDef",
-    "CreateRuleRequestRequestTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "RuleUpdateSuccessTypeDef",
+    "UpdateRuleResponseTypeDef",
+    "CreateRuleRequestRequestTypeDef",
     "RuleUpdateTypeDef",
     "UpdateRuleRequestRequestTypeDef",
-    "UpdateRuleResponseTypeDef",
     "BatchUpdateRuleResponseTypeDef",
     "BatchUpdateRuleRequestRequestTypeDef",
 )
 
 AccessLogSubscriptionSummaryTypeDef = TypedDict(
     "AccessLogSubscriptionSummaryTypeDef",
     {
@@ -182,14 +196,25 @@
         "id": str,
         "lastUpdatedAt": datetime,
         "resourceArn": str,
         "resourceId": str,
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
 RuleUpdateFailureTypeDef = TypedDict(
     "RuleUpdateFailureTypeDef",
     {
         "failureCode": str,
         "failureMessage": str,
         "ruleIdentifier": str,
     },
@@ -214,26 +239,14 @@
 
 class CreateAccessLogSubscriptionRequestRequestTypeDef(
     _RequiredCreateAccessLogSubscriptionRequestRequestTypeDef,
     _OptionalCreateAccessLogSubscriptionRequestRequestTypeDef,
 ):
     pass
 
-CreateAccessLogSubscriptionResponseTypeDef = TypedDict(
-    "CreateAccessLogSubscriptionResponseTypeDef",
-    {
-        "arn": str,
-        "destinationArn": str,
-        "id": str,
-        "resourceArn": str,
-        "resourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateServiceNetworkRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceNetworkRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateServiceNetworkRequestRequestTypeDef = TypedDict(
@@ -248,25 +261,14 @@
 
 class CreateServiceNetworkRequestRequestTypeDef(
     _RequiredCreateServiceNetworkRequestRequestTypeDef,
     _OptionalCreateServiceNetworkRequestRequestTypeDef,
 ):
     pass
 
-CreateServiceNetworkResponseTypeDef = TypedDict(
-    "CreateServiceNetworkResponseTypeDef",
-    {
-        "arn": str,
-        "authType": AuthTypeType,
-        "id": str,
-        "name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateServiceNetworkServiceAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceNetworkServiceAssociationRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
         "serviceNetworkIdentifier": str,
     },
 )
@@ -313,26 +315,14 @@
 
 class CreateServiceNetworkVpcAssociationRequestRequestTypeDef(
     _RequiredCreateServiceNetworkVpcAssociationRequestRequestTypeDef,
     _OptionalCreateServiceNetworkVpcAssociationRequestRequestTypeDef,
 ):
     pass
 
-CreateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "CreateServiceNetworkVpcAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "createdBy": str,
-        "id": str,
-        "securityGroupIds": List[str],
-        "status": ServiceNetworkVpcAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateServiceRequestRequestTypeDef = TypedDict(
@@ -400,76 +390,35 @@
 DeleteServiceNetworkServiceAssociationRequestRequestTypeDef = TypedDict(
     "DeleteServiceNetworkServiceAssociationRequestRequestTypeDef",
     {
         "serviceNetworkServiceAssociationIdentifier": str,
     },
 )
 
-DeleteServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
-    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": ServiceNetworkServiceAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
     "DeleteServiceNetworkVpcAssociationRequestRequestTypeDef",
     {
         "serviceNetworkVpcAssociationIdentifier": str,
     },
 )
 
-DeleteServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": ServiceNetworkVpcAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteServiceRequestRequestTypeDef = TypedDict(
     "DeleteServiceRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
     },
 )
 
-DeleteServiceResponseTypeDef = TypedDict(
-    "DeleteServiceResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "status": ServiceStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTargetGroupRequestRequestTypeDef = TypedDict(
     "DeleteTargetGroupRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
     },
 )
 
-DeleteTargetGroupResponseTypeDef = TypedDict(
-    "DeleteTargetGroupResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": TargetGroupStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredTargetTypeDef = TypedDict(
     "_RequiredTargetTypeDef",
     {
         "id": str,
     },
 )
 _OptionalTargetTypeDef = TypedDict(
@@ -490,21 +439,64 @@
         "failureMessage": str,
         "id": str,
         "port": int,
     },
     total=False,
 )
 
+_RequiredTargetOutputTypeDef = TypedDict(
+    "_RequiredTargetOutputTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalTargetOutputTypeDef = TypedDict(
+    "_OptionalTargetOutputTypeDef",
+    {
+        "port": int,
+    },
+    total=False,
+)
+
+class TargetOutputTypeDef(_RequiredTargetOutputTypeDef, _OptionalTargetOutputTypeDef):
+    pass
+
+FixedResponseActionOutputTypeDef = TypedDict(
+    "FixedResponseActionOutputTypeDef",
+    {
+        "statusCode": int,
+    },
+)
+
 FixedResponseActionTypeDef = TypedDict(
     "FixedResponseActionTypeDef",
     {
         "statusCode": int,
     },
 )
 
+_RequiredWeightedTargetGroupOutputTypeDef = TypedDict(
+    "_RequiredWeightedTargetGroupOutputTypeDef",
+    {
+        "targetGroupIdentifier": str,
+    },
+)
+_OptionalWeightedTargetGroupOutputTypeDef = TypedDict(
+    "_OptionalWeightedTargetGroupOutputTypeDef",
+    {
+        "weight": int,
+    },
+    total=False,
+)
+
+class WeightedTargetGroupOutputTypeDef(
+    _RequiredWeightedTargetGroupOutputTypeDef, _OptionalWeightedTargetGroupOutputTypeDef
+):
+    pass
+
 _RequiredWeightedTargetGroupTypeDef = TypedDict(
     "_RequiredWeightedTargetGroupTypeDef",
     {
         "targetGroupIdentifier": str,
     },
 )
 _OptionalWeightedTargetGroupTypeDef = TypedDict(
@@ -523,46 +515,21 @@
 GetAccessLogSubscriptionRequestRequestTypeDef = TypedDict(
     "GetAccessLogSubscriptionRequestRequestTypeDef",
     {
         "accessLogSubscriptionIdentifier": str,
     },
 )
 
-GetAccessLogSubscriptionResponseTypeDef = TypedDict(
-    "GetAccessLogSubscriptionResponseTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "destinationArn": str,
-        "id": str,
-        "lastUpdatedAt": datetime,
-        "resourceArn": str,
-        "resourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAuthPolicyRequestRequestTypeDef = TypedDict(
     "GetAuthPolicyRequestRequestTypeDef",
     {
         "resourceIdentifier": str,
     },
 )
 
-GetAuthPolicyResponseTypeDef = TypedDict(
-    "GetAuthPolicyResponseTypeDef",
-    {
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "policy": str,
-        "state": AuthPolicyStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetListenerRequestRequestTypeDef = TypedDict(
     "GetListenerRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
         "serviceIdentifier": str,
     },
 )
@@ -570,22 +537,14 @@
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRuleRequestRequestTypeDef = TypedDict(
     "GetRuleRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
         "ruleIdentifier": str,
         "serviceIdentifier": str,
     },
@@ -594,115 +553,88 @@
 GetServiceNetworkRequestRequestTypeDef = TypedDict(
     "GetServiceNetworkRequestRequestTypeDef",
     {
         "serviceNetworkIdentifier": str,
     },
 )
 
-GetServiceNetworkResponseTypeDef = TypedDict(
-    "GetServiceNetworkResponseTypeDef",
-    {
-        "arn": str,
-        "authType": AuthTypeType,
-        "createdAt": datetime,
-        "id": str,
-        "lastUpdatedAt": datetime,
-        "name": str,
-        "numberOfAssociatedServices": int,
-        "numberOfAssociatedVPCs": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetServiceNetworkServiceAssociationRequestRequestTypeDef = TypedDict(
     "GetServiceNetworkServiceAssociationRequestRequestTypeDef",
     {
         "serviceNetworkServiceAssociationIdentifier": str,
     },
 )
 
 GetServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
     "GetServiceNetworkVpcAssociationRequestRequestTypeDef",
     {
         "serviceNetworkVpcAssociationIdentifier": str,
     },
 )
 
-GetServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "GetServiceNetworkVpcAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "createdBy": str,
-        "failureCode": str,
-        "failureMessage": str,
-        "id": str,
-        "lastUpdatedAt": datetime,
-        "securityGroupIds": List[str],
-        "serviceNetworkArn": str,
-        "serviceNetworkId": str,
-        "serviceNetworkName": str,
-        "status": ServiceNetworkVpcAssociationStatusType,
-        "vpcId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetServiceRequestRequestTypeDef = TypedDict(
     "GetServiceRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
     },
 )
 
 GetTargetGroupRequestRequestTypeDef = TypedDict(
     "GetTargetGroupRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
     },
 )
 
+HeaderMatchTypeOutputTypeDef = TypedDict(
+    "HeaderMatchTypeOutputTypeDef",
+    {
+        "contains": str,
+        "exact": str,
+        "prefix": str,
+    },
+    total=False,
+)
+
 HeaderMatchTypeTypeDef = TypedDict(
     "HeaderMatchTypeTypeDef",
     {
         "contains": str,
         "exact": str,
         "prefix": str,
     },
     total=False,
 )
 
-MatcherTypeDef = TypedDict(
-    "MatcherTypeDef",
+MatcherOutputTypeDef = TypedDict(
+    "MatcherOutputTypeDef",
     {
         "httpCode": str,
     },
     total=False,
 )
 
-_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
-    "_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+MatcherTypeDef = TypedDict(
+    "MatcherTypeDef",
     {
-        "resourceIdentifier": str,
+        "httpCode": str,
     },
+    total=False,
 )
-_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
-    "_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+
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
 
-class ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef(
-    _RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
-    _OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAccessLogSubscriptionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccessLogSubscriptionsRequestRequestTypeDef",
     {
         "resourceIdentifier": str,
     },
 )
 _OptionalListAccessLogSubscriptionsRequestRequestTypeDef = TypedDict(
@@ -716,34 +648,14 @@
 
 class ListAccessLogSubscriptionsRequestRequestTypeDef(
     _RequiredListAccessLogSubscriptionsRequestRequestTypeDef,
     _OptionalListAccessLogSubscriptionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListListenersRequestListListenersPaginateTypeDef = TypedDict(
-    "_RequiredListListenersRequestListListenersPaginateTypeDef",
-    {
-        "serviceIdentifier": str,
-    },
-)
-_OptionalListListenersRequestListListenersPaginateTypeDef = TypedDict(
-    "_OptionalListListenersRequestListListenersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListListenersRequestListListenersPaginateTypeDef(
-    _RequiredListListenersRequestListListenersPaginateTypeDef,
-    _OptionalListListenersRequestListListenersPaginateTypeDef,
-):
-    pass
-
 _RequiredListListenersRequestRequestTypeDef = TypedDict(
     "_RequiredListListenersRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
     },
 )
 _OptionalListListenersRequestRequestTypeDef = TypedDict(
@@ -770,35 +682,14 @@
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
     },
     total=False,
 )
 
-_RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "_RequiredListRulesRequestListRulesPaginateTypeDef",
-    {
-        "listenerIdentifier": str,
-        "serviceIdentifier": str,
-    },
-)
-_OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "_OptionalListRulesRequestListRulesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRulesRequestListRulesPaginateTypeDef(
-    _RequiredListRulesRequestListRulesPaginateTypeDef,
-    _OptionalListRulesRequestListRulesPaginateTypeDef,
-):
-    pass
-
 _RequiredListRulesRequestRequestTypeDef = TypedDict(
     "_RequiredListRulesRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
         "serviceIdentifier": str,
     },
 )
@@ -826,47 +717,25 @@
         "lastUpdatedAt": datetime,
         "name": str,
         "priority": int,
     },
     total=False,
 )
 
-ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef = TypedDict(
-    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
-    {
-        "serviceIdentifier": str,
-        "serviceNetworkIdentifier": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServiceNetworkServiceAssociationsRequestRequestTypeDef = TypedDict(
     "ListServiceNetworkServiceAssociationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "serviceIdentifier": str,
         "serviceNetworkIdentifier": str,
     },
     total=False,
 )
 
-ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef = (
-    TypedDict(
-        "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
-        {
-            "serviceNetworkIdentifier": str,
-            "vpcIdentifier": str,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
 ListServiceNetworkVpcAssociationsRequestRequestTypeDef = TypedDict(
     "ListServiceNetworkVpcAssociationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "serviceNetworkIdentifier": str,
         "vpcIdentifier": str,
@@ -887,22 +756,14 @@
         "serviceNetworkName": str,
         "status": ServiceNetworkVpcAssociationStatusType,
         "vpcId": str,
     },
     total=False,
 )
 
-ListServiceNetworksRequestListServiceNetworksPaginateTypeDef = TypedDict(
-    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServiceNetworksRequestRequestTypeDef = TypedDict(
     "ListServiceNetworksRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -918,22 +779,14 @@
         "name": str,
         "numberOfAssociatedServices": int,
         "numberOfAssociatedVPCs": int,
     },
     total=False,
 )
 
-ListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "ListServicesRequestListServicesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -942,32 +795,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTargetGroupsRequestListTargetGroupsPaginateTypeDef = TypedDict(
-    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
-    {
-        "targetGroupType": TargetGroupTypeType,
-        "vpcIdentifier": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTargetGroupsRequestRequestTypeDef = TypedDict(
     "ListTargetGroupsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "targetGroupType": TargetGroupTypeType,
         "vpcIdentifier": str,
@@ -1001,20 +836,19 @@
         "port": int,
         "reasonCode": str,
         "status": TargetStatusType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+PathMatchTypeOutputTypeDef = TypedDict(
+    "PathMatchTypeOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "exact": str,
+        "prefix": str,
     },
     total=False,
 )
 
 PathMatchTypeTypeDef = TypedDict(
     "PathMatchTypeTypeDef",
     {
@@ -1028,42 +862,22 @@
     "PutAuthPolicyRequestRequestTypeDef",
     {
         "policy": str,
         "resourceIdentifier": str,
     },
 )
 
-PutAuthPolicyResponseTypeDef = TypedDict(
-    "PutAuthPolicyResponseTypeDef",
-    {
-        "policy": str,
-        "state": AuthPolicyStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1080,132 +894,293 @@
     "UpdateAccessLogSubscriptionRequestRequestTypeDef",
     {
         "accessLogSubscriptionIdentifier": str,
         "destinationArn": str,
     },
 )
 
-UpdateAccessLogSubscriptionResponseTypeDef = TypedDict(
-    "UpdateAccessLogSubscriptionResponseTypeDef",
+UpdateServiceNetworkRequestRequestTypeDef = TypedDict(
+    "UpdateServiceNetworkRequestRequestTypeDef",
+    {
+        "authType": AuthTypeType,
+        "serviceNetworkIdentifier": str,
+    },
+)
+
+UpdateServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
+    "UpdateServiceNetworkVpcAssociationRequestRequestTypeDef",
+    {
+        "securityGroupIds": Sequence[str],
+        "serviceNetworkVpcAssociationIdentifier": str,
+    },
+)
+
+_RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateServiceRequestRequestTypeDef",
+    {
+        "serviceIdentifier": str,
+    },
+)
+_OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateServiceRequestRequestTypeDef",
+    {
+        "authType": AuthTypeType,
+        "certificateArn": str,
+    },
+    total=False,
+)
+
+class UpdateServiceRequestRequestTypeDef(
+    _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
+):
+    pass
+
+CreateAccessLogSubscriptionResponseTypeDef = TypedDict(
+    "CreateAccessLogSubscriptionResponseTypeDef",
     {
         "arn": str,
         "destinationArn": str,
         "id": str,
         "resourceArn": str,
         "resourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateServiceNetworkRequestRequestTypeDef = TypedDict(
-    "UpdateServiceNetworkRequestRequestTypeDef",
+CreateServiceNetworkResponseTypeDef = TypedDict(
+    "CreateServiceNetworkResponseTypeDef",
     {
+        "arn": str,
         "authType": AuthTypeType,
-        "serviceNetworkIdentifier": str,
+        "id": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateServiceNetworkResponseTypeDef = TypedDict(
-    "UpdateServiceNetworkResponseTypeDef",
+CreateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "CreateServiceNetworkVpcAssociationResponseTypeDef",
     {
         "arn": str,
-        "authType": AuthTypeType,
+        "createdBy": str,
         "id": str,
-        "name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "securityGroupIds": List[str],
+        "status": ServiceNetworkVpcAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
-    "UpdateServiceNetworkVpcAssociationRequestRequestTypeDef",
+DeleteServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
+    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
     {
-        "securityGroupIds": Sequence[str],
-        "serviceNetworkVpcAssociationIdentifier": str,
+        "arn": str,
+        "id": str,
+        "status": ServiceNetworkServiceAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "UpdateServiceNetworkVpcAssociationResponseTypeDef",
+DeleteServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
     {
         "arn": str,
-        "createdBy": str,
         "id": str,
-        "securityGroupIds": List[str],
         "status": ServiceNetworkVpcAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateServiceRequestRequestTypeDef",
+DeleteServiceResponseTypeDef = TypedDict(
+    "DeleteServiceResponseTypeDef",
     {
-        "serviceIdentifier": str,
+        "arn": str,
+        "id": str,
+        "name": str,
+        "status": ServiceStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateServiceRequestRequestTypeDef",
+
+DeleteTargetGroupResponseTypeDef = TypedDict(
+    "DeleteTargetGroupResponseTypeDef",
     {
-        "authType": AuthTypeType,
-        "certificateArn": str,
+        "arn": str,
+        "id": str,
+        "status": TargetGroupStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateServiceRequestRequestTypeDef(
-    _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
-):
-    pass
+GetAccessLogSubscriptionResponseTypeDef = TypedDict(
+    "GetAccessLogSubscriptionResponseTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "destinationArn": str,
+        "id": str,
+        "lastUpdatedAt": datetime,
+        "resourceArn": str,
+        "resourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-UpdateServiceResponseTypeDef = TypedDict(
-    "UpdateServiceResponseTypeDef",
+GetAuthPolicyResponseTypeDef = TypedDict(
+    "GetAuthPolicyResponseTypeDef",
+    {
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "policy": str,
+        "state": AuthPolicyStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetServiceNetworkResponseTypeDef = TypedDict(
+    "GetServiceNetworkResponseTypeDef",
     {
         "arn": str,
         "authType": AuthTypeType,
-        "certificateArn": str,
-        "customDomainName": str,
+        "createdAt": datetime,
         "id": str,
+        "lastUpdatedAt": datetime,
         "name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "numberOfAssociatedServices": int,
+        "numberOfAssociatedVPCs": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "GetServiceNetworkVpcAssociationResponseTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "createdBy": str,
+        "failureCode": str,
+        "failureMessage": str,
+        "id": str,
+        "lastUpdatedAt": datetime,
+        "securityGroupIds": List[str],
+        "serviceNetworkArn": str,
+        "serviceNetworkId": str,
+        "serviceNetworkName": str,
+        "status": ServiceNetworkVpcAssociationStatusType,
+        "vpcId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccessLogSubscriptionsResponseTypeDef = TypedDict(
     "ListAccessLogSubscriptionsResponseTypeDef",
     {
         "items": List[AccessLogSubscriptionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutAuthPolicyResponseTypeDef = TypedDict(
+    "PutAuthPolicyResponseTypeDef",
+    {
+        "policy": str,
+        "state": AuthPolicyStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAccessLogSubscriptionResponseTypeDef = TypedDict(
+    "UpdateAccessLogSubscriptionResponseTypeDef",
+    {
+        "arn": str,
+        "destinationArn": str,
+        "id": str,
+        "resourceArn": str,
+        "resourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateServiceNetworkResponseTypeDef = TypedDict(
+    "UpdateServiceNetworkResponseTypeDef",
+    {
+        "arn": str,
+        "authType": AuthTypeType,
+        "id": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "UpdateServiceNetworkVpcAssociationResponseTypeDef",
+    {
+        "arn": str,
+        "createdBy": str,
+        "id": str,
+        "securityGroupIds": List[str],
+        "status": ServiceNetworkVpcAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateServiceResponseTypeDef = TypedDict(
+    "UpdateServiceResponseTypeDef",
+    {
+        "arn": str,
+        "authType": AuthTypeType,
+        "certificateArn": str,
+        "customDomainName": str,
+        "id": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
     "CreateServiceNetworkServiceAssociationResponseTypeDef",
     {
         "arn": str,
         "createdBy": str,
         "customDomainName": str,
         "dnsEntry": DnsEntryTypeDef,
         "id": str,
         "status": ServiceNetworkServiceAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "arn": str,
         "authType": AuthTypeType,
         "certificateArn": str,
         "customDomainName": str,
         "dnsEntry": DnsEntryTypeDef,
         "id": str,
         "name": str,
         "status": ServiceStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
     "GetServiceNetworkServiceAssociationResponseTypeDef",
     {
         "arn": str,
@@ -1219,15 +1194,15 @@
         "serviceArn": str,
         "serviceId": str,
         "serviceName": str,
         "serviceNetworkArn": str,
         "serviceNetworkId": str,
         "serviceNetworkName": str,
         "status": ServiceNetworkServiceAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceResponseTypeDef = TypedDict(
     "GetServiceResponseTypeDef",
     {
         "arn": str,
@@ -1238,15 +1213,15 @@
         "dnsEntry": DnsEntryTypeDef,
         "failureCode": str,
         "failureMessage": str,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "status": ServiceStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ServiceNetworkServiceAssociationSummaryTypeDef = TypedDict(
     "ServiceNetworkServiceAssociationSummaryTypeDef",
     {
         "arn": str,
@@ -1285,35 +1260,14 @@
     "DeregisterTargetsRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
         "targets": Sequence[TargetTypeDef],
     },
 )
 
-_RequiredListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
-    "_RequiredListTargetsRequestListTargetsPaginateTypeDef",
-    {
-        "targetGroupIdentifier": str,
-    },
-)
-_OptionalListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
-    "_OptionalListTargetsRequestListTargetsPaginateTypeDef",
-    {
-        "targets": Sequence[TargetTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTargetsRequestListTargetsPaginateTypeDef(
-    _RequiredListTargetsRequestListTargetsPaginateTypeDef,
-    _OptionalListTargetsRequestListTargetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredListTargetsRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
     },
 )
 _OptionalListTargetsRequestRequestTypeDef = TypedDict(
@@ -1338,36 +1292,63 @@
         "targets": Sequence[TargetTypeDef],
     },
 )
 
 DeregisterTargetsResponseTypeDef = TypedDict(
     "DeregisterTargetsResponseTypeDef",
     {
-        "successful": List[TargetTypeDef],
+        "successful": List[TargetOutputTypeDef],
         "unsuccessful": List[TargetFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterTargetsResponseTypeDef = TypedDict(
     "RegisterTargetsResponseTypeDef",
     {
-        "successful": List[TargetTypeDef],
+        "successful": List[TargetOutputTypeDef],
         "unsuccessful": List[TargetFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ForwardActionOutputTypeDef = TypedDict(
+    "ForwardActionOutputTypeDef",
+    {
+        "targetGroups": List[WeightedTargetGroupOutputTypeDef],
     },
 )
 
 ForwardActionTypeDef = TypedDict(
     "ForwardActionTypeDef",
     {
         "targetGroups": Sequence[WeightedTargetGroupTypeDef],
     },
 )
 
+_RequiredHeaderMatchOutputTypeDef = TypedDict(
+    "_RequiredHeaderMatchOutputTypeDef",
+    {
+        "match": HeaderMatchTypeOutputTypeDef,
+        "name": str,
+    },
+)
+_OptionalHeaderMatchOutputTypeDef = TypedDict(
+    "_OptionalHeaderMatchOutputTypeDef",
+    {
+        "caseSensitive": bool,
+    },
+    total=False,
+)
+
+class HeaderMatchOutputTypeDef(
+    _RequiredHeaderMatchOutputTypeDef, _OptionalHeaderMatchOutputTypeDef
+):
+    pass
+
 _RequiredHeaderMatchTypeDef = TypedDict(
     "_RequiredHeaderMatchTypeDef",
     {
         "match": HeaderMatchTypeTypeDef,
         "name": str,
     },
 )
@@ -1378,14 +1359,31 @@
     },
     total=False,
 )
 
 class HeaderMatchTypeDef(_RequiredHeaderMatchTypeDef, _OptionalHeaderMatchTypeDef):
     pass
 
+HealthCheckConfigOutputTypeDef = TypedDict(
+    "HealthCheckConfigOutputTypeDef",
+    {
+        "enabled": bool,
+        "healthCheckIntervalSeconds": int,
+        "healthCheckTimeoutSeconds": int,
+        "healthyThresholdCount": int,
+        "matcher": MatcherOutputTypeDef,
+        "path": str,
+        "port": int,
+        "protocol": TargetGroupProtocolType,
+        "protocolVersion": HealthCheckProtocolVersionType,
+        "unhealthyThresholdCount": int,
+    },
+    total=False,
+)
+
 HealthCheckConfigTypeDef = TypedDict(
     "HealthCheckConfigTypeDef",
     {
         "enabled": bool,
         "healthCheckIntervalSeconds": int,
         "healthCheckTimeoutSeconds": int,
         "healthyThresholdCount": int,
@@ -1395,68 +1393,215 @@
         "protocol": TargetGroupProtocolType,
         "protocolVersion": HealthCheckProtocolVersionType,
         "unhealthyThresholdCount": int,
     },
     total=False,
 )
 
+_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
+    "_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+    {
+        "resourceIdentifier": str,
+    },
+)
+_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
+    "_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef(
+    _RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+    _OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListListenersRequestListListenersPaginateTypeDef = TypedDict(
+    "_RequiredListListenersRequestListListenersPaginateTypeDef",
+    {
+        "serviceIdentifier": str,
+    },
+)
+_OptionalListListenersRequestListListenersPaginateTypeDef = TypedDict(
+    "_OptionalListListenersRequestListListenersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListListenersRequestListListenersPaginateTypeDef(
+    _RequiredListListenersRequestListListenersPaginateTypeDef,
+    _OptionalListListenersRequestListListenersPaginateTypeDef,
+):
+    pass
+
+_RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "_RequiredListRulesRequestListRulesPaginateTypeDef",
+    {
+        "listenerIdentifier": str,
+        "serviceIdentifier": str,
+    },
+)
+_OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "_OptionalListRulesRequestListRulesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRulesRequestListRulesPaginateTypeDef(
+    _RequiredListRulesRequestListRulesPaginateTypeDef,
+    _OptionalListRulesRequestListRulesPaginateTypeDef,
+):
+    pass
+
+ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef = TypedDict(
+    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
+    {
+        "serviceIdentifier": str,
+        "serviceNetworkIdentifier": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef = (
+    TypedDict(
+        "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
+        {
+            "serviceNetworkIdentifier": str,
+            "vpcIdentifier": str,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+ListServiceNetworksRequestListServiceNetworksPaginateTypeDef = TypedDict(
+    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "ListServicesRequestListServicesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTargetGroupsRequestListTargetGroupsPaginateTypeDef = TypedDict(
+    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
+    {
+        "targetGroupType": TargetGroupTypeType,
+        "vpcIdentifier": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
+    "_RequiredListTargetsRequestListTargetsPaginateTypeDef",
+    {
+        "targetGroupIdentifier": str,
+    },
+)
+_OptionalListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
+    "_OptionalListTargetsRequestListTargetsPaginateTypeDef",
+    {
+        "targets": Sequence[TargetTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTargetsRequestListTargetsPaginateTypeDef(
+    _RequiredListTargetsRequestListTargetsPaginateTypeDef,
+    _OptionalListTargetsRequestListTargetsPaginateTypeDef,
+):
+    pass
+
 ListListenersResponseTypeDef = TypedDict(
     "ListListenersResponseTypeDef",
     {
         "items": List[ListenerSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "items": List[RuleSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceNetworkVpcAssociationsResponseTypeDef = TypedDict(
     "ListServiceNetworkVpcAssociationsResponseTypeDef",
     {
         "items": List[ServiceNetworkVpcAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceNetworksResponseTypeDef = TypedDict(
     "ListServiceNetworksResponseTypeDef",
     {
         "items": List[ServiceNetworkSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetGroupsResponseTypeDef = TypedDict(
     "ListTargetGroupsResponseTypeDef",
     {
         "items": List[TargetGroupSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetsResponseTypeDef = TypedDict(
     "ListTargetsResponseTypeDef",
     {
         "items": List[TargetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPathMatchOutputTypeDef = TypedDict(
+    "_RequiredPathMatchOutputTypeDef",
+    {
+        "match": PathMatchTypeOutputTypeDef,
+    },
+)
+_OptionalPathMatchOutputTypeDef = TypedDict(
+    "_OptionalPathMatchOutputTypeDef",
+    {
+        "caseSensitive": bool,
+    },
+    total=False,
+)
+
+class PathMatchOutputTypeDef(_RequiredPathMatchOutputTypeDef, _OptionalPathMatchOutputTypeDef):
+    pass
+
 _RequiredPathMatchTypeDef = TypedDict(
     "_RequiredPathMatchTypeDef",
     {
         "match": PathMatchTypeTypeDef,
     },
 )
 _OptionalPathMatchTypeDef = TypedDict(
@@ -1471,36 +1616,68 @@
     pass
 
 ListServiceNetworkServiceAssociationsResponseTypeDef = TypedDict(
     "ListServiceNetworkServiceAssociationsResponseTypeDef",
     {
         "items": List[ServiceNetworkServiceAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "items": List[ServiceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RuleActionOutputTypeDef = TypedDict(
+    "RuleActionOutputTypeDef",
+    {
+        "fixedResponse": FixedResponseActionOutputTypeDef,
+        "forward": ForwardActionOutputTypeDef,
+    },
+    total=False,
+)
+
 RuleActionTypeDef = TypedDict(
     "RuleActionTypeDef",
     {
         "fixedResponse": FixedResponseActionTypeDef,
         "forward": ForwardActionTypeDef,
     },
     total=False,
 )
 
+_RequiredTargetGroupConfigOutputTypeDef = TypedDict(
+    "_RequiredTargetGroupConfigOutputTypeDef",
+    {
+        "port": int,
+        "protocol": TargetGroupProtocolType,
+        "vpcIdentifier": str,
+    },
+)
+_OptionalTargetGroupConfigOutputTypeDef = TypedDict(
+    "_OptionalTargetGroupConfigOutputTypeDef",
+    {
+        "healthCheck": HealthCheckConfigOutputTypeDef,
+        "ipAddressType": IpAddressTypeType,
+        "protocolVersion": TargetGroupProtocolVersionType,
+    },
+    total=False,
+)
+
+class TargetGroupConfigOutputTypeDef(
+    _RequiredTargetGroupConfigOutputTypeDef, _OptionalTargetGroupConfigOutputTypeDef
+):
+    pass
+
 _RequiredTargetGroupConfigTypeDef = TypedDict(
     "_RequiredTargetGroupConfigTypeDef",
     {
         "port": int,
         "protocol": TargetGroupProtocolType,
         "vpcIdentifier": str,
     },
@@ -1524,246 +1701,278 @@
     "UpdateTargetGroupRequestRequestTypeDef",
     {
         "healthCheck": HealthCheckConfigTypeDef,
         "targetGroupIdentifier": str,
     },
 )
 
-HttpMatchTypeDef = TypedDict(
-    "HttpMatchTypeDef",
+HttpMatchOutputTypeDef = TypedDict(
+    "HttpMatchOutputTypeDef",
     {
-        "headerMatches": Sequence[HeaderMatchTypeDef],
+        "headerMatches": List[HeaderMatchOutputTypeDef],
         "method": str,
-        "pathMatch": PathMatchTypeDef,
+        "pathMatch": PathMatchOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateListenerRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateListenerRequestRequestTypeDef",
-    {
-        "defaultAction": RuleActionTypeDef,
-        "name": str,
-        "protocol": ListenerProtocolType,
-        "serviceIdentifier": str,
-    },
-)
-_OptionalCreateListenerRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateListenerRequestRequestTypeDef",
+HttpMatchTypeDef = TypedDict(
+    "HttpMatchTypeDef",
     {
-        "clientToken": str,
-        "port": int,
-        "tags": Mapping[str, str],
+        "headerMatches": Sequence[HeaderMatchTypeDef],
+        "method": str,
+        "pathMatch": PathMatchTypeDef,
     },
     total=False,
 )
 
-class CreateListenerRequestRequestTypeDef(
-    _RequiredCreateListenerRequestRequestTypeDef, _OptionalCreateListenerRequestRequestTypeDef
-):
-    pass
-
 CreateListenerResponseTypeDef = TypedDict(
     "CreateListenerResponseTypeDef",
     {
         "arn": str,
-        "defaultAction": RuleActionTypeDef,
+        "defaultAction": RuleActionOutputTypeDef,
         "id": str,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetListenerResponseTypeDef = TypedDict(
     "GetListenerResponseTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
-        "defaultAction": RuleActionTypeDef,
+        "defaultAction": RuleActionOutputTypeDef,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateListenerRequestRequestTypeDef = TypedDict(
-    "UpdateListenerRequestRequestTypeDef",
-    {
-        "defaultAction": RuleActionTypeDef,
-        "listenerIdentifier": str,
-        "serviceIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateListenerResponseTypeDef = TypedDict(
     "UpdateListenerResponseTypeDef",
     {
         "arn": str,
-        "defaultAction": RuleActionTypeDef,
+        "defaultAction": RuleActionOutputTypeDef,
         "id": str,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateTargetGroupRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTargetGroupRequestRequestTypeDef",
+_RequiredCreateListenerRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateListenerRequestRequestTypeDef",
     {
+        "defaultAction": RuleActionTypeDef,
         "name": str,
-        "type": TargetGroupTypeType,
+        "protocol": ListenerProtocolType,
+        "serviceIdentifier": str,
     },
 )
-_OptionalCreateTargetGroupRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTargetGroupRequestRequestTypeDef",
+_OptionalCreateListenerRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateListenerRequestRequestTypeDef",
     {
         "clientToken": str,
-        "config": TargetGroupConfigTypeDef,
+        "port": int,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class CreateTargetGroupRequestRequestTypeDef(
-    _RequiredCreateTargetGroupRequestRequestTypeDef, _OptionalCreateTargetGroupRequestRequestTypeDef
+class CreateListenerRequestRequestTypeDef(
+    _RequiredCreateListenerRequestRequestTypeDef, _OptionalCreateListenerRequestRequestTypeDef
 ):
     pass
 
+UpdateListenerRequestRequestTypeDef = TypedDict(
+    "UpdateListenerRequestRequestTypeDef",
+    {
+        "defaultAction": RuleActionTypeDef,
+        "listenerIdentifier": str,
+        "serviceIdentifier": str,
+    },
+)
+
 CreateTargetGroupResponseTypeDef = TypedDict(
     "CreateTargetGroupResponseTypeDef",
     {
         "arn": str,
-        "config": TargetGroupConfigTypeDef,
+        "config": TargetGroupConfigOutputTypeDef,
         "id": str,
         "name": str,
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTargetGroupResponseTypeDef = TypedDict(
     "GetTargetGroupResponseTypeDef",
     {
         "arn": str,
-        "config": TargetGroupConfigTypeDef,
+        "config": TargetGroupConfigOutputTypeDef,
         "createdAt": datetime,
         "failureCode": str,
         "failureMessage": str,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "serviceArns": List[str],
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTargetGroupResponseTypeDef = TypedDict(
     "UpdateTargetGroupResponseTypeDef",
     {
         "arn": str,
-        "config": TargetGroupConfigTypeDef,
+        "config": TargetGroupConfigOutputTypeDef,
         "id": str,
         "name": str,
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RuleMatchTypeDef = TypedDict(
-    "RuleMatchTypeDef",
-    {
-        "httpMatch": HttpMatchTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRuleRequestRequestTypeDef",
+_RequiredCreateTargetGroupRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTargetGroupRequestRequestTypeDef",
     {
-        "action": RuleActionTypeDef,
-        "listenerIdentifier": str,
-        "match": RuleMatchTypeDef,
         "name": str,
-        "priority": int,
-        "serviceIdentifier": str,
+        "type": TargetGroupTypeType,
     },
 )
-_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRuleRequestRequestTypeDef",
+_OptionalCreateTargetGroupRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTargetGroupRequestRequestTypeDef",
     {
         "clientToken": str,
+        "config": TargetGroupConfigTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class CreateRuleRequestRequestTypeDef(
-    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
+class CreateTargetGroupRequestRequestTypeDef(
+    _RequiredCreateTargetGroupRequestRequestTypeDef, _OptionalCreateTargetGroupRequestRequestTypeDef
 ):
     pass
 
+RuleMatchOutputTypeDef = TypedDict(
+    "RuleMatchOutputTypeDef",
+    {
+        "httpMatch": HttpMatchOutputTypeDef,
+    },
+    total=False,
+)
+
+RuleMatchTypeDef = TypedDict(
+    "RuleMatchTypeDef",
+    {
+        "httpMatch": HttpMatchTypeDef,
+    },
+    total=False,
+)
+
 CreateRuleResponseTypeDef = TypedDict(
     "CreateRuleResponseTypeDef",
     {
-        "action": RuleActionTypeDef,
+        "action": RuleActionOutputTypeDef,
         "arn": str,
         "id": str,
-        "match": RuleMatchTypeDef,
+        "match": RuleMatchOutputTypeDef,
         "name": str,
         "priority": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
-        "action": RuleActionTypeDef,
+        "action": RuleActionOutputTypeDef,
         "arn": str,
         "createdAt": datetime,
         "id": str,
         "isDefault": bool,
         "lastUpdatedAt": datetime,
-        "match": RuleMatchTypeDef,
+        "match": RuleMatchOutputTypeDef,
         "name": str,
         "priority": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RuleUpdateSuccessTypeDef = TypedDict(
     "RuleUpdateSuccessTypeDef",
     {
-        "action": RuleActionTypeDef,
+        "action": RuleActionOutputTypeDef,
+        "arn": str,
+        "id": str,
+        "isDefault": bool,
+        "match": RuleMatchOutputTypeDef,
+        "name": str,
+        "priority": int,
+    },
+    total=False,
+)
+
+UpdateRuleResponseTypeDef = TypedDict(
+    "UpdateRuleResponseTypeDef",
+    {
+        "action": RuleActionOutputTypeDef,
         "arn": str,
         "id": str,
         "isDefault": bool,
+        "match": RuleMatchOutputTypeDef,
+        "name": str,
+        "priority": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRuleRequestRequestTypeDef",
+    {
+        "action": RuleActionTypeDef,
+        "listenerIdentifier": str,
         "match": RuleMatchTypeDef,
         "name": str,
         "priority": int,
+        "serviceIdentifier": str,
+    },
+)
+_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRuleRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
+class CreateRuleRequestRequestTypeDef(
+    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
+):
+    pass
+
 _RequiredRuleUpdateTypeDef = TypedDict(
     "_RequiredRuleUpdateTypeDef",
     {
         "ruleIdentifier": str,
     },
 )
 _OptionalRuleUpdateTypeDef = TypedDict(
@@ -1798,34 +2007,20 @@
 )
 
 class UpdateRuleRequestRequestTypeDef(
     _RequiredUpdateRuleRequestRequestTypeDef, _OptionalUpdateRuleRequestRequestTypeDef
 ):
     pass
 
-UpdateRuleResponseTypeDef = TypedDict(
-    "UpdateRuleResponseTypeDef",
-    {
-        "action": RuleActionTypeDef,
-        "arn": str,
-        "id": str,
-        "isDefault": bool,
-        "match": RuleMatchTypeDef,
-        "name": str,
-        "priority": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchUpdateRuleResponseTypeDef = TypedDict(
     "BatchUpdateRuleResponseTypeDef",
     {
         "successful": List[RuleUpdateSuccessTypeDef],
         "unsuccessful": List[RuleUpdateFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateRuleRequestRequestTypeDef = TypedDict(
     "BatchUpdateRuleRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
```

### Comparing `mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice.egg-info/PKG-INFO` & `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-vpc-lattice
-Version: 1.28.0
-Summary: Type annotations for boto3.VPCLattice 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.VPCLattice 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-vpc-lattice"></a>
 
 # mypy-boto3-vpc-lattice
 
 [![PyPI - mypy-boto3-vpc-lattice](https://img.shields.io/pypi/v/mypy-boto3-vpc-lattice.svg?color=blue)](https://pypi.org/project/mypy-boto3-vpc-lattice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-vpc-lattice.svg?color=blue)](https://pypi.org/project/mypy-boto3-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-vpc-lattice?color=blue)](https://pypistats.org/packages/mypy-boto3-vpc-lattice)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-vpc-lattice)](https://pepy.tech/project/mypy-boto3-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VPCLattice 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
+[boto3.VPCLattice 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
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
 [mypy-boto3-vpc-lattice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -366,145 +366,159 @@
 
 `mypy_boto3_vpc_lattice.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_vpc_lattice.type_defs import (
     AccessLogSubscriptionSummaryTypeDef,
+    ResponseMetadataTypeDef,
     RuleUpdateFailureTypeDef,
     CreateAccessLogSubscriptionRequestRequestTypeDef,
-    CreateAccessLogSubscriptionResponseTypeDef,
     CreateServiceNetworkRequestRequestTypeDef,
-    CreateServiceNetworkResponseTypeDef,
     CreateServiceNetworkServiceAssociationRequestRequestTypeDef,
     DnsEntryTypeDef,
     CreateServiceNetworkVpcAssociationRequestRequestTypeDef,
-    CreateServiceNetworkVpcAssociationResponseTypeDef,
     CreateServiceRequestRequestTypeDef,
     DeleteAccessLogSubscriptionRequestRequestTypeDef,
     DeleteAuthPolicyRequestRequestTypeDef,
     DeleteListenerRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DeleteServiceNetworkRequestRequestTypeDef,
     DeleteServiceNetworkServiceAssociationRequestRequestTypeDef,
-    DeleteServiceNetworkServiceAssociationResponseTypeDef,
     DeleteServiceNetworkVpcAssociationRequestRequestTypeDef,
-    DeleteServiceNetworkVpcAssociationResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
-    DeleteServiceResponseTypeDef,
     DeleteTargetGroupRequestRequestTypeDef,
-    DeleteTargetGroupResponseTypeDef,
     TargetTypeDef,
     TargetFailureTypeDef,
+    TargetOutputTypeDef,
+    FixedResponseActionOutputTypeDef,
     FixedResponseActionTypeDef,
+    WeightedTargetGroupOutputTypeDef,
     WeightedTargetGroupTypeDef,
     GetAccessLogSubscriptionRequestRequestTypeDef,
-    GetAccessLogSubscriptionResponseTypeDef,
     GetAuthPolicyRequestRequestTypeDef,
-    GetAuthPolicyResponseTypeDef,
     GetListenerRequestRequestTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetRuleRequestRequestTypeDef,
     GetServiceNetworkRequestRequestTypeDef,
-    GetServiceNetworkResponseTypeDef,
     GetServiceNetworkServiceAssociationRequestRequestTypeDef,
     GetServiceNetworkVpcAssociationRequestRequestTypeDef,
-    GetServiceNetworkVpcAssociationResponseTypeDef,
     GetServiceRequestRequestTypeDef,
     GetTargetGroupRequestRequestTypeDef,
+    HeaderMatchTypeOutputTypeDef,
     HeaderMatchTypeTypeDef,
+    MatcherOutputTypeDef,
     MatcherTypeDef,
-    ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessLogSubscriptionsRequestRequestTypeDef,
-    ListListenersRequestListListenersPaginateTypeDef,
     ListListenersRequestRequestTypeDef,
     ListenerSummaryTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
-    ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef,
     ListServiceNetworkServiceAssociationsRequestRequestTypeDef,
-    ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef,
     ListServiceNetworkVpcAssociationsRequestRequestTypeDef,
     ServiceNetworkVpcAssociationSummaryTypeDef,
-    ListServiceNetworksRequestListServiceNetworksPaginateTypeDef,
     ListServiceNetworksRequestRequestTypeDef,
     ServiceNetworkSummaryTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTargetGroupsRequestListTargetGroupsPaginateTypeDef,
     ListTargetGroupsRequestRequestTypeDef,
     TargetGroupSummaryTypeDef,
     TargetSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    PathMatchTypeOutputTypeDef,
     PathMatchTypeTypeDef,
     PutAuthPolicyRequestRequestTypeDef,
-    PutAuthPolicyResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccessLogSubscriptionRequestRequestTypeDef,
-    UpdateAccessLogSubscriptionResponseTypeDef,
     UpdateServiceNetworkRequestRequestTypeDef,
-    UpdateServiceNetworkResponseTypeDef,
     UpdateServiceNetworkVpcAssociationRequestRequestTypeDef,
-    UpdateServiceNetworkVpcAssociationResponseTypeDef,
     UpdateServiceRequestRequestTypeDef,
-    UpdateServiceResponseTypeDef,
+    CreateAccessLogSubscriptionResponseTypeDef,
+    CreateServiceNetworkResponseTypeDef,
+    CreateServiceNetworkVpcAssociationResponseTypeDef,
+    DeleteServiceNetworkServiceAssociationResponseTypeDef,
+    DeleteServiceNetworkVpcAssociationResponseTypeDef,
+    DeleteServiceResponseTypeDef,
+    DeleteTargetGroupResponseTypeDef,
+    GetAccessLogSubscriptionResponseTypeDef,
+    GetAuthPolicyResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    GetServiceNetworkResponseTypeDef,
+    GetServiceNetworkVpcAssociationResponseTypeDef,
     ListAccessLogSubscriptionsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutAuthPolicyResponseTypeDef,
+    UpdateAccessLogSubscriptionResponseTypeDef,
+    UpdateServiceNetworkResponseTypeDef,
+    UpdateServiceNetworkVpcAssociationResponseTypeDef,
+    UpdateServiceResponseTypeDef,
     CreateServiceNetworkServiceAssociationResponseTypeDef,
     CreateServiceResponseTypeDef,
     GetServiceNetworkServiceAssociationResponseTypeDef,
     GetServiceResponseTypeDef,
     ServiceNetworkServiceAssociationSummaryTypeDef,
     ServiceSummaryTypeDef,
     DeregisterTargetsRequestRequestTypeDef,
-    ListTargetsRequestListTargetsPaginateTypeDef,
     ListTargetsRequestRequestTypeDef,
     RegisterTargetsRequestRequestTypeDef,
     DeregisterTargetsResponseTypeDef,
     RegisterTargetsResponseTypeDef,
+    ForwardActionOutputTypeDef,
     ForwardActionTypeDef,
+    HeaderMatchOutputTypeDef,
     HeaderMatchTypeDef,
+    HealthCheckConfigOutputTypeDef,
     HealthCheckConfigTypeDef,
+    ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+    ListListenersRequestListListenersPaginateTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
+    ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef,
+    ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef,
+    ListServiceNetworksRequestListServiceNetworksPaginateTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
+    ListTargetGroupsRequestListTargetGroupsPaginateTypeDef,
+    ListTargetsRequestListTargetsPaginateTypeDef,
     ListListenersResponseTypeDef,
     ListRulesResponseTypeDef,
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServiceNetworksResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
+    PathMatchOutputTypeDef,
     PathMatchTypeDef,
     ListServiceNetworkServiceAssociationsResponseTypeDef,
     ListServicesResponseTypeDef,
+    RuleActionOutputTypeDef,
     RuleActionTypeDef,
+    TargetGroupConfigOutputTypeDef,
     TargetGroupConfigTypeDef,
     UpdateTargetGroupRequestRequestTypeDef,
+    HttpMatchOutputTypeDef,
     HttpMatchTypeDef,
-    CreateListenerRequestRequestTypeDef,
     CreateListenerResponseTypeDef,
     GetListenerResponseTypeDef,
-    UpdateListenerRequestRequestTypeDef,
     UpdateListenerResponseTypeDef,
-    CreateTargetGroupRequestRequestTypeDef,
+    CreateListenerRequestRequestTypeDef,
+    UpdateListenerRequestRequestTypeDef,
     CreateTargetGroupResponseTypeDef,
     GetTargetGroupResponseTypeDef,
     UpdateTargetGroupResponseTypeDef,
+    CreateTargetGroupRequestRequestTypeDef,
+    RuleMatchOutputTypeDef,
     RuleMatchTypeDef,
-    CreateRuleRequestRequestTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     RuleUpdateSuccessTypeDef,
+    UpdateRuleResponseTypeDef,
+    CreateRuleRequestRequestTypeDef,
     RuleUpdateTypeDef,
     UpdateRuleRequestRequestTypeDef,
-    UpdateRuleResponseTypeDef,
     BatchUpdateRuleResponseTypeDef,
     BatchUpdateRuleRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AccessLogSubscriptionSummaryTypeDef:
     return {...}
```

### Comparing `mypy-boto3-vpc-lattice-1.28.0/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt` & `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.0/setup.py` & `mypy-boto3-vpc-lattice-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-vpc-lattice",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_vpc_lattice"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.VPCLattice 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.VPCLattice 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

