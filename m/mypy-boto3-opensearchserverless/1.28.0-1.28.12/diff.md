# Comparing `tmp/mypy-boto3-opensearchserverless-1.28.0.tar.gz` & `tmp/mypy-boto3-opensearchserverless-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-opensearchserverless-1.28.0.tar", last modified: Thu Jul  6 21:00:14 2023, max compression
+gzip compressed data, was "mypy-boto3-opensearchserverless-1.28.12.tar", last modified: Thu Jul 27 05:44:17 2023, max compression
```

## Comparing `mypy-boto3-opensearchserverless-1.28.0.tar` & `mypy-boto3-opensearchserverless-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:14.850385 mypy-boto3-opensearchserverless-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:48:41.000000 mypy-boto3-opensearchserverless-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15877 2023-07-06 21:00:14.838385 mypy-boto3-opensearchserverless-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-07-06 20:48:41.000000 mypy-boto3-opensearchserverless-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:14.838385 mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-06 20:48:41.000000 mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-06 20:48:41.000000 mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-06 20:48:41.000000 mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23936 2023-07-06 20:48:41.000000 mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23898 2023-07-06 20:48:41.000000 mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-06 20:48:41.000000 mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-07-06 20:48:41.000000 mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:48:41.000000 mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29403 2023-07-06 20:48:42.000000 mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29364 2023-07-06 20:48:41.000000 mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:48:41.000000 mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:14.838385 mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15877 2023-07-06 21:00:14.000000 mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-06 21:00:14.000000 mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:14.000000 mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:14.000000 mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:14.000000 mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 21:00:14.000000 mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:14.850385 mypy-boto3-opensearchserverless-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-06 20:48:40.000000 mypy-boto3-opensearchserverless-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:17.383381 mypy-boto3-opensearchserverless-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15955 2023-07-27 05:44:17.383381 mypy-boto3-opensearchserverless-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14409 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:17.383381 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23936 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23898 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    30270 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30229 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:17.383381 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15955 2023-07-27 05:44:17.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-27 05:44:17.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:44:17.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:44:17.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:44:17.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 05:44:17.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:44:17.383381 mypy-boto3-opensearchserverless-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-27 05:44:02.000000 mypy-boto3-opensearchserverless-1.28.12/setup.py
```

### Comparing `mypy-boto3-opensearchserverless-1.28.0/LICENSE` & `mypy-boto3-opensearchserverless-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearchserverless-1.28.0/PKG-INFO` & `mypy-boto3-opensearchserverless-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opensearchserverless
-Version: 1.28.0
-Summary: Type annotations for boto3.OpenSearchServiceServerless 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.OpenSearchServiceServerless 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-opensearchserverless"></a>
 
 # mypy-boto3-opensearchserverless
 
 [![PyPI - mypy-boto3-opensearchserverless](https://img.shields.io/pypi/v/mypy-boto3-opensearchserverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearchserverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearchserverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearchserverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opensearchserverless?color=blue)](https://pypistats.org/packages/mypy-boto3-opensearchserverless)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opensearchserverless)](https://pepy.tech/project/mypy-boto3-opensearchserverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchServiceServerless 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
+[boto3.OpenSearchServiceServerless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
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
 [mypy-boto3-opensearchserverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,21 +306,23 @@
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opensearchserverless.type_defs import (
     AccessPolicyDetailTypeDef,
     AccessPolicyStatsTypeDef,
     AccessPolicySummaryTypeDef,
-    CapacityLimitsTypeDef,
+    CapacityLimitsOutputTypeDef,
     BatchGetCollectionRequestRequestTypeDef,
     CollectionDetailTypeDef,
     CollectionErrorDetailTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetVpcEndpointRequestRequestTypeDef,
     VpcEndpointDetailTypeDef,
     VpcEndpointErrorDetailTypeDef,
+    CapacityLimitsTypeDef,
     CollectionFiltersTypeDef,
     CollectionSummaryTypeDef,
     CreateAccessPolicyRequestRequestTypeDef,
     CreateCollectionDetailTypeDef,
     TagTypeDef,
     SamlConfigOptionsTypeDef,
     CreateSecurityPolicyRequestRequestTypeDef,
@@ -341,52 +343,53 @@
     GetSecurityPolicyRequestRequestTypeDef,
     ListAccessPoliciesRequestRequestTypeDef,
     ListSecurityConfigsRequestRequestTypeDef,
     SecurityConfigSummaryTypeDef,
     ListSecurityPoliciesRequestRequestTypeDef,
     SecurityPolicySummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     VpcEndpointFiltersTypeDef,
     VpcEndpointSummaryTypeDef,
-    ResponseMetadataTypeDef,
+    SamlConfigOptionsOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccessPolicyRequestRequestTypeDef,
     UpdateCollectionDetailTypeDef,
     UpdateCollectionRequestRequestTypeDef,
     UpdateSecurityPolicyRequestRequestTypeDef,
     UpdateVpcEndpointDetailTypeDef,
     UpdateVpcEndpointRequestRequestTypeDef,
+    AccountSettingsDetailTypeDef,
+    BatchGetCollectionResponseTypeDef,
     CreateAccessPolicyResponseTypeDef,
     GetAccessPolicyResponseTypeDef,
-    UpdateAccessPolicyResponseTypeDef,
     ListAccessPoliciesResponseTypeDef,
-    AccountSettingsDetailTypeDef,
-    UpdateAccountSettingsRequestRequestTypeDef,
-    BatchGetCollectionResponseTypeDef,
+    UpdateAccessPolicyResponseTypeDef,
     BatchGetVpcEndpointResponseTypeDef,
+    UpdateAccountSettingsRequestRequestTypeDef,
     ListCollectionsRequestRequestTypeDef,
     ListCollectionsResponseTypeDef,
     CreateCollectionResponseTypeDef,
     CreateCollectionRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSecurityConfigRequestRequestTypeDef,
-    SecurityConfigDetailTypeDef,
     UpdateSecurityConfigRequestRequestTypeDef,
     CreateSecurityPolicyResponseTypeDef,
     GetSecurityPolicyResponseTypeDef,
     UpdateSecurityPolicyResponseTypeDef,
     CreateVpcEndpointResponseTypeDef,
     DeleteCollectionResponseTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     GetPoliciesStatsResponseTypeDef,
     ListSecurityConfigsResponseTypeDef,
     ListSecurityPoliciesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
     ListVpcEndpointsResponseTypeDef,
+    SecurityConfigDetailTypeDef,
     UpdateCollectionResponseTypeDef,
     UpdateVpcEndpointResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     UpdateAccountSettingsResponseTypeDef,
     CreateSecurityConfigResponseTypeDef,
     GetSecurityConfigResponseTypeDef,
     UpdateSecurityConfigResponseTypeDef,
```

### Comparing `mypy-boto3-opensearchserverless-1.28.0/README.md` & `mypy-boto3-opensearchserverless-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-opensearchserverless"></a>
 
 # mypy-boto3-opensearchserverless
 
 [![PyPI - mypy-boto3-opensearchserverless](https://img.shields.io/pypi/v/mypy-boto3-opensearchserverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearchserverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearchserverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearchserverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opensearchserverless?color=blue)](https://pypistats.org/packages/mypy-boto3-opensearchserverless)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opensearchserverless)](https://pepy.tech/project/mypy-boto3-opensearchserverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchServiceServerless 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
+[boto3.OpenSearchServiceServerless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
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
 [mypy-boto3-opensearchserverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -274,21 +274,23 @@
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opensearchserverless.type_defs import (
     AccessPolicyDetailTypeDef,
     AccessPolicyStatsTypeDef,
     AccessPolicySummaryTypeDef,
-    CapacityLimitsTypeDef,
+    CapacityLimitsOutputTypeDef,
     BatchGetCollectionRequestRequestTypeDef,
     CollectionDetailTypeDef,
     CollectionErrorDetailTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetVpcEndpointRequestRequestTypeDef,
     VpcEndpointDetailTypeDef,
     VpcEndpointErrorDetailTypeDef,
+    CapacityLimitsTypeDef,
     CollectionFiltersTypeDef,
     CollectionSummaryTypeDef,
     CreateAccessPolicyRequestRequestTypeDef,
     CreateCollectionDetailTypeDef,
     TagTypeDef,
     SamlConfigOptionsTypeDef,
     CreateSecurityPolicyRequestRequestTypeDef,
@@ -309,52 +311,53 @@
     GetSecurityPolicyRequestRequestTypeDef,
     ListAccessPoliciesRequestRequestTypeDef,
     ListSecurityConfigsRequestRequestTypeDef,
     SecurityConfigSummaryTypeDef,
     ListSecurityPoliciesRequestRequestTypeDef,
     SecurityPolicySummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     VpcEndpointFiltersTypeDef,
     VpcEndpointSummaryTypeDef,
-    ResponseMetadataTypeDef,
+    SamlConfigOptionsOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccessPolicyRequestRequestTypeDef,
     UpdateCollectionDetailTypeDef,
     UpdateCollectionRequestRequestTypeDef,
     UpdateSecurityPolicyRequestRequestTypeDef,
     UpdateVpcEndpointDetailTypeDef,
     UpdateVpcEndpointRequestRequestTypeDef,
+    AccountSettingsDetailTypeDef,
+    BatchGetCollectionResponseTypeDef,
     CreateAccessPolicyResponseTypeDef,
     GetAccessPolicyResponseTypeDef,
-    UpdateAccessPolicyResponseTypeDef,
     ListAccessPoliciesResponseTypeDef,
-    AccountSettingsDetailTypeDef,
-    UpdateAccountSettingsRequestRequestTypeDef,
-    BatchGetCollectionResponseTypeDef,
+    UpdateAccessPolicyResponseTypeDef,
     BatchGetVpcEndpointResponseTypeDef,
+    UpdateAccountSettingsRequestRequestTypeDef,
     ListCollectionsRequestRequestTypeDef,
     ListCollectionsResponseTypeDef,
     CreateCollectionResponseTypeDef,
     CreateCollectionRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSecurityConfigRequestRequestTypeDef,
-    SecurityConfigDetailTypeDef,
     UpdateSecurityConfigRequestRequestTypeDef,
     CreateSecurityPolicyResponseTypeDef,
     GetSecurityPolicyResponseTypeDef,
     UpdateSecurityPolicyResponseTypeDef,
     CreateVpcEndpointResponseTypeDef,
     DeleteCollectionResponseTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     GetPoliciesStatsResponseTypeDef,
     ListSecurityConfigsResponseTypeDef,
     ListSecurityPoliciesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
     ListVpcEndpointsResponseTypeDef,
+    SecurityConfigDetailTypeDef,
     UpdateCollectionResponseTypeDef,
     UpdateVpcEndpointResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     UpdateAccountSettingsResponseTypeDef,
     CreateSecurityConfigResponseTypeDef,
     GetSecurityConfigResponseTypeDef,
     UpdateSecurityConfigResponseTypeDef,
```

### Comparing `mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless/__init__.py` & `mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless/__main__.py` & `mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpenSearchServiceServerless 1.28.0\nVersion:        "
-        " 1.28.0\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.OpenSearchServiceServerless 1.28.12\nVersion:        "
+        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless\nOther"
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

### Comparing `mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless/client.py` & `mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless/client.pyi` & `mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless/literals.py` & `mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "ResourceServiceName",
     "RegionName",
 )
 
 
 AccessPolicyTypeType = Literal["data"]
 CollectionStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED"]
-CollectionTypeType = Literal["SEARCH", "TIMESERIES"]
+CollectionTypeType = Literal["SEARCH", "TIMESERIES", "VECTORSEARCH"]
 SecurityConfigTypeType = Literal["saml"]
 SecurityPolicyTypeType = Literal["encryption", "network"]
 VpcEndpointStatusType = Literal["ACTIVE", "DELETING", "FAILED", "PENDING"]
 OpenSearchServiceServerlessServiceName = Literal["opensearchserverless"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -155,14 +155,15 @@
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
@@ -241,26 +242,28 @@
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

### Comparing `mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless/literals.pyi` & `mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 AccessPolicyTypeType = Literal["data"]
 CollectionStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED"]
-CollectionTypeType = Literal["SEARCH", "TIMESERIES"]
+CollectionTypeType = Literal["SEARCH", "TIMESERIES", "VECTORSEARCH"]
 SecurityConfigTypeType = Literal["saml"]
 SecurityPolicyTypeType = Literal["encryption", "network"]
 VpcEndpointStatusType = Literal["ACTIVE", "DELETING", "FAILED", "PENDING"]
 OpenSearchServiceServerlessServiceName = Literal["opensearchserverless"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -153,14 +153,15 @@
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
@@ -239,26 +240,28 @@
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

### Comparing `mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless/type_defs.py` & `mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,21 +31,23 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccessPolicyDetailTypeDef",
     "AccessPolicyStatsTypeDef",
     "AccessPolicySummaryTypeDef",
-    "CapacityLimitsTypeDef",
+    "CapacityLimitsOutputTypeDef",
     "BatchGetCollectionRequestRequestTypeDef",
     "CollectionDetailTypeDef",
     "CollectionErrorDetailTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetVpcEndpointRequestRequestTypeDef",
     "VpcEndpointDetailTypeDef",
     "VpcEndpointErrorDetailTypeDef",
+    "CapacityLimitsTypeDef",
     "CollectionFiltersTypeDef",
     "CollectionSummaryTypeDef",
     "CreateAccessPolicyRequestRequestTypeDef",
     "CreateCollectionDetailTypeDef",
     "TagTypeDef",
     "SamlConfigOptionsTypeDef",
     "CreateSecurityPolicyRequestRequestTypeDef",
@@ -66,52 +68,53 @@
     "GetSecurityPolicyRequestRequestTypeDef",
     "ListAccessPoliciesRequestRequestTypeDef",
     "ListSecurityConfigsRequestRequestTypeDef",
     "SecurityConfigSummaryTypeDef",
     "ListSecurityPoliciesRequestRequestTypeDef",
     "SecurityPolicySummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "VpcEndpointFiltersTypeDef",
     "VpcEndpointSummaryTypeDef",
-    "ResponseMetadataTypeDef",
+    "SamlConfigOptionsOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccessPolicyRequestRequestTypeDef",
     "UpdateCollectionDetailTypeDef",
     "UpdateCollectionRequestRequestTypeDef",
     "UpdateSecurityPolicyRequestRequestTypeDef",
     "UpdateVpcEndpointDetailTypeDef",
     "UpdateVpcEndpointRequestRequestTypeDef",
+    "AccountSettingsDetailTypeDef",
+    "BatchGetCollectionResponseTypeDef",
     "CreateAccessPolicyResponseTypeDef",
     "GetAccessPolicyResponseTypeDef",
-    "UpdateAccessPolicyResponseTypeDef",
     "ListAccessPoliciesResponseTypeDef",
-    "AccountSettingsDetailTypeDef",
-    "UpdateAccountSettingsRequestRequestTypeDef",
-    "BatchGetCollectionResponseTypeDef",
+    "UpdateAccessPolicyResponseTypeDef",
     "BatchGetVpcEndpointResponseTypeDef",
+    "UpdateAccountSettingsRequestRequestTypeDef",
     "ListCollectionsRequestRequestTypeDef",
     "ListCollectionsResponseTypeDef",
     "CreateCollectionResponseTypeDef",
     "CreateCollectionRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSecurityConfigRequestRequestTypeDef",
-    "SecurityConfigDetailTypeDef",
     "UpdateSecurityConfigRequestRequestTypeDef",
     "CreateSecurityPolicyResponseTypeDef",
     "GetSecurityPolicyResponseTypeDef",
     "UpdateSecurityPolicyResponseTypeDef",
     "CreateVpcEndpointResponseTypeDef",
     "DeleteCollectionResponseTypeDef",
     "DeleteVpcEndpointResponseTypeDef",
     "GetPoliciesStatsResponseTypeDef",
     "ListSecurityConfigsResponseTypeDef",
     "ListSecurityPoliciesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListVpcEndpointsRequestRequestTypeDef",
     "ListVpcEndpointsResponseTypeDef",
+    "SecurityConfigDetailTypeDef",
     "UpdateCollectionResponseTypeDef",
     "UpdateVpcEndpointResponseTypeDef",
     "GetAccountSettingsResponseTypeDef",
     "UpdateAccountSettingsResponseTypeDef",
     "CreateSecurityConfigResponseTypeDef",
     "GetSecurityConfigResponseTypeDef",
     "UpdateSecurityConfigResponseTypeDef",
@@ -148,16 +151,16 @@
         "name": str,
         "policyVersion": str,
         "type": Literal["data"],
     },
     total=False,
 )
 
-CapacityLimitsTypeDef = TypedDict(
-    "CapacityLimitsTypeDef",
+CapacityLimitsOutputTypeDef = TypedDict(
+    "CapacityLimitsOutputTypeDef",
     {
         "maxIndexingCapacityInOCU": int,
         "maxSearchCapacityInOCU": int,
     },
     total=False,
 )
 
@@ -195,14 +198,25 @@
         "errorMessage": str,
         "id": str,
         "name": str,
     },
     total=False,
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
 BatchGetVpcEndpointRequestRequestTypeDef = TypedDict(
     "BatchGetVpcEndpointRequestRequestTypeDef",
     {
         "ids": Sequence[str],
     },
 )
 
@@ -226,14 +240,23 @@
         "errorCode": str,
         "errorMessage": str,
         "id": str,
     },
     total=False,
 )
 
+CapacityLimitsTypeDef = TypedDict(
+    "CapacityLimitsTypeDef",
+    {
+        "maxIndexingCapacityInOCU": int,
+        "maxSearchCapacityInOCU": int,
+    },
+    total=False,
+)
+
 CollectionFiltersTypeDef = TypedDict(
     "CollectionFiltersTypeDef",
     {
         "name": str,
         "status": CollectionStatusType,
     },
     total=False,
@@ -665,14 +688,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 VpcEndpointFiltersTypeDef = TypedDict(
     "VpcEndpointFiltersTypeDef",
     {
         "status": VpcEndpointStatusType,
     },
     total=False,
 )
@@ -683,25 +714,37 @@
         "id": str,
         "name": str,
         "status": VpcEndpointStatusType,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredSamlConfigOptionsOutputTypeDef = TypedDict(
+    "_RequiredSamlConfigOptionsOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "metadata": str,
+    },
+)
+_OptionalSamlConfigOptionsOutputTypeDef = TypedDict(
+    "_OptionalSamlConfigOptionsOutputTypeDef",
+    {
+        "groupAttribute": str,
+        "sessionTimeout": int,
+        "userAttribute": str,
     },
+    total=False,
 )
 
+
+class SamlConfigOptionsOutputTypeDef(
+    _RequiredSamlConfigOptionsOutputTypeDef, _OptionalSamlConfigOptionsOutputTypeDef
+):
+    pass
+
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -829,81 +872,81 @@
 
 class UpdateVpcEndpointRequestRequestTypeDef(
     _RequiredUpdateVpcEndpointRequestRequestTypeDef, _OptionalUpdateVpcEndpointRequestRequestTypeDef
 ):
     pass
 
 
-CreateAccessPolicyResponseTypeDef = TypedDict(
-    "CreateAccessPolicyResponseTypeDef",
+AccountSettingsDetailTypeDef = TypedDict(
+    "AccountSettingsDetailTypeDef",
     {
-        "accessPolicyDetail": AccessPolicyDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "capacityLimits": CapacityLimitsOutputTypeDef,
     },
+    total=False,
 )
 
-GetAccessPolicyResponseTypeDef = TypedDict(
-    "GetAccessPolicyResponseTypeDef",
+BatchGetCollectionResponseTypeDef = TypedDict(
+    "BatchGetCollectionResponseTypeDef",
+    {
+        "collectionDetails": List[CollectionDetailTypeDef],
+        "collectionErrorDetails": List[CollectionErrorDetailTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAccessPolicyResponseTypeDef = TypedDict(
+    "CreateAccessPolicyResponseTypeDef",
     {
         "accessPolicyDetail": AccessPolicyDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateAccessPolicyResponseTypeDef = TypedDict(
-    "UpdateAccessPolicyResponseTypeDef",
+GetAccessPolicyResponseTypeDef = TypedDict(
+    "GetAccessPolicyResponseTypeDef",
     {
         "accessPolicyDetail": AccessPolicyDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccessPoliciesResponseTypeDef = TypedDict(
     "ListAccessPoliciesResponseTypeDef",
     {
         "accessPolicySummaries": List[AccessPolicySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AccountSettingsDetailTypeDef = TypedDict(
-    "AccountSettingsDetailTypeDef",
-    {
-        "capacityLimits": CapacityLimitsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateAccountSettingsRequestRequestTypeDef",
-    {
-        "capacityLimits": CapacityLimitsTypeDef,
-    },
-    total=False,
-)
-
-BatchGetCollectionResponseTypeDef = TypedDict(
-    "BatchGetCollectionResponseTypeDef",
+UpdateAccessPolicyResponseTypeDef = TypedDict(
+    "UpdateAccessPolicyResponseTypeDef",
     {
-        "collectionDetails": List[CollectionDetailTypeDef],
-        "collectionErrorDetails": List[CollectionErrorDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "accessPolicyDetail": AccessPolicyDetailTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetVpcEndpointResponseTypeDef = TypedDict(
     "BatchGetVpcEndpointResponseTypeDef",
     {
         "vpcEndpointDetails": List[VpcEndpointDetailTypeDef],
         "vpcEndpointErrorDetails": List[VpcEndpointErrorDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateAccountSettingsRequestRequestTypeDef",
+    {
+        "capacityLimits": CapacityLimitsTypeDef,
+    },
+    total=False,
+)
+
 ListCollectionsRequestRequestTypeDef = TypedDict(
     "ListCollectionsRequestRequestTypeDef",
     {
         "collectionFilters": CollectionFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
@@ -911,23 +954,23 @@
 )
 
 ListCollectionsResponseTypeDef = TypedDict(
     "ListCollectionsResponseTypeDef",
     {
         "collectionSummaries": List[CollectionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCollectionResponseTypeDef = TypedDict(
     "CreateCollectionResponseTypeDef",
     {
         "createCollectionDetail": CreateCollectionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCollectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCollectionRequestRequestTypeDef",
     {
         "name": str,
@@ -947,22 +990,14 @@
 
 class CreateCollectionRequestRequestTypeDef(
     _RequiredCreateCollectionRequestRequestTypeDef, _OptionalCreateCollectionRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -988,28 +1023,14 @@
 class CreateSecurityConfigRequestRequestTypeDef(
     _RequiredCreateSecurityConfigRequestRequestTypeDef,
     _OptionalCreateSecurityConfigRequestRequestTypeDef,
 ):
     pass
 
 
-SecurityConfigDetailTypeDef = TypedDict(
-    "SecurityConfigDetailTypeDef",
-    {
-        "configVersion": str,
-        "createdDate": int,
-        "description": str,
-        "id": str,
-        "lastModifiedDate": int,
-        "samlOptions": SamlConfigOptionsTypeDef,
-        "type": Literal["saml"],
-    },
-    total=False,
-)
-
 _RequiredUpdateSecurityConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSecurityConfigRequestRequestTypeDef",
     {
         "configVersion": str,
         "id": str,
     },
 )
@@ -1031,84 +1052,92 @@
     pass
 
 
 CreateSecurityPolicyResponseTypeDef = TypedDict(
     "CreateSecurityPolicyResponseTypeDef",
     {
         "securityPolicyDetail": SecurityPolicyDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSecurityPolicyResponseTypeDef = TypedDict(
     "GetSecurityPolicyResponseTypeDef",
     {
         "securityPolicyDetail": SecurityPolicyDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSecurityPolicyResponseTypeDef = TypedDict(
     "UpdateSecurityPolicyResponseTypeDef",
     {
         "securityPolicyDetail": SecurityPolicyDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVpcEndpointResponseTypeDef = TypedDict(
     "CreateVpcEndpointResponseTypeDef",
     {
         "createVpcEndpointDetail": CreateVpcEndpointDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCollectionResponseTypeDef = TypedDict(
     "DeleteCollectionResponseTypeDef",
     {
         "deleteCollectionDetail": DeleteCollectionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVpcEndpointResponseTypeDef = TypedDict(
     "DeleteVpcEndpointResponseTypeDef",
     {
         "deleteVpcEndpointDetail": DeleteVpcEndpointDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPoliciesStatsResponseTypeDef = TypedDict(
     "GetPoliciesStatsResponseTypeDef",
     {
         "AccessPolicyStats": AccessPolicyStatsTypeDef,
         "SecurityConfigStats": SecurityConfigStatsTypeDef,
         "SecurityPolicyStats": SecurityPolicyStatsTypeDef,
         "TotalPolicyCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSecurityConfigsResponseTypeDef = TypedDict(
     "ListSecurityConfigsResponseTypeDef",
     {
         "nextToken": str,
         "securityConfigSummaries": List[SecurityConfigSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSecurityPoliciesResponseTypeDef = TypedDict(
     "ListSecurityPoliciesResponseTypeDef",
     {
         "nextToken": str,
         "securityPolicySummaries": List[SecurityPolicySummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVpcEndpointsRequestRequestTypeDef = TypedDict(
     "ListVpcEndpointsRequestRequestTypeDef",
     {
         "maxResults": int,
@@ -1119,66 +1148,80 @@
 )
 
 ListVpcEndpointsResponseTypeDef = TypedDict(
     "ListVpcEndpointsResponseTypeDef",
     {
         "nextToken": str,
         "vpcEndpointSummaries": List[VpcEndpointSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SecurityConfigDetailTypeDef = TypedDict(
+    "SecurityConfigDetailTypeDef",
+    {
+        "configVersion": str,
+        "createdDate": int,
+        "description": str,
+        "id": str,
+        "lastModifiedDate": int,
+        "samlOptions": SamlConfigOptionsOutputTypeDef,
+        "type": Literal["saml"],
+    },
+    total=False,
+)
+
 UpdateCollectionResponseTypeDef = TypedDict(
     "UpdateCollectionResponseTypeDef",
     {
         "updateCollectionDetail": UpdateCollectionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVpcEndpointResponseTypeDef = TypedDict(
     "UpdateVpcEndpointResponseTypeDef",
     {
         "UpdateVpcEndpointDetail": UpdateVpcEndpointDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountSettingsResponseTypeDef = TypedDict(
     "GetAccountSettingsResponseTypeDef",
     {
         "accountSettingsDetail": AccountSettingsDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAccountSettingsResponseTypeDef = TypedDict(
     "UpdateAccountSettingsResponseTypeDef",
     {
         "accountSettingsDetail": AccountSettingsDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSecurityConfigResponseTypeDef = TypedDict(
     "CreateSecurityConfigResponseTypeDef",
     {
         "securityConfigDetail": SecurityConfigDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSecurityConfigResponseTypeDef = TypedDict(
     "GetSecurityConfigResponseTypeDef",
     {
         "securityConfigDetail": SecurityConfigDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSecurityConfigResponseTypeDef = TypedDict(
     "UpdateSecurityConfigResponseTypeDef",
     {
         "securityConfigDetail": SecurityConfigDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless/type_defs.pyi` & `mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -30,21 +30,23 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessPolicyDetailTypeDef",
     "AccessPolicyStatsTypeDef",
     "AccessPolicySummaryTypeDef",
-    "CapacityLimitsTypeDef",
+    "CapacityLimitsOutputTypeDef",
     "BatchGetCollectionRequestRequestTypeDef",
     "CollectionDetailTypeDef",
     "CollectionErrorDetailTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetVpcEndpointRequestRequestTypeDef",
     "VpcEndpointDetailTypeDef",
     "VpcEndpointErrorDetailTypeDef",
+    "CapacityLimitsTypeDef",
     "CollectionFiltersTypeDef",
     "CollectionSummaryTypeDef",
     "CreateAccessPolicyRequestRequestTypeDef",
     "CreateCollectionDetailTypeDef",
     "TagTypeDef",
     "SamlConfigOptionsTypeDef",
     "CreateSecurityPolicyRequestRequestTypeDef",
@@ -65,52 +67,53 @@
     "GetSecurityPolicyRequestRequestTypeDef",
     "ListAccessPoliciesRequestRequestTypeDef",
     "ListSecurityConfigsRequestRequestTypeDef",
     "SecurityConfigSummaryTypeDef",
     "ListSecurityPoliciesRequestRequestTypeDef",
     "SecurityPolicySummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "VpcEndpointFiltersTypeDef",
     "VpcEndpointSummaryTypeDef",
-    "ResponseMetadataTypeDef",
+    "SamlConfigOptionsOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccessPolicyRequestRequestTypeDef",
     "UpdateCollectionDetailTypeDef",
     "UpdateCollectionRequestRequestTypeDef",
     "UpdateSecurityPolicyRequestRequestTypeDef",
     "UpdateVpcEndpointDetailTypeDef",
     "UpdateVpcEndpointRequestRequestTypeDef",
+    "AccountSettingsDetailTypeDef",
+    "BatchGetCollectionResponseTypeDef",
     "CreateAccessPolicyResponseTypeDef",
     "GetAccessPolicyResponseTypeDef",
-    "UpdateAccessPolicyResponseTypeDef",
     "ListAccessPoliciesResponseTypeDef",
-    "AccountSettingsDetailTypeDef",
-    "UpdateAccountSettingsRequestRequestTypeDef",
-    "BatchGetCollectionResponseTypeDef",
+    "UpdateAccessPolicyResponseTypeDef",
     "BatchGetVpcEndpointResponseTypeDef",
+    "UpdateAccountSettingsRequestRequestTypeDef",
     "ListCollectionsRequestRequestTypeDef",
     "ListCollectionsResponseTypeDef",
     "CreateCollectionResponseTypeDef",
     "CreateCollectionRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSecurityConfigRequestRequestTypeDef",
-    "SecurityConfigDetailTypeDef",
     "UpdateSecurityConfigRequestRequestTypeDef",
     "CreateSecurityPolicyResponseTypeDef",
     "GetSecurityPolicyResponseTypeDef",
     "UpdateSecurityPolicyResponseTypeDef",
     "CreateVpcEndpointResponseTypeDef",
     "DeleteCollectionResponseTypeDef",
     "DeleteVpcEndpointResponseTypeDef",
     "GetPoliciesStatsResponseTypeDef",
     "ListSecurityConfigsResponseTypeDef",
     "ListSecurityPoliciesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListVpcEndpointsRequestRequestTypeDef",
     "ListVpcEndpointsResponseTypeDef",
+    "SecurityConfigDetailTypeDef",
     "UpdateCollectionResponseTypeDef",
     "UpdateVpcEndpointResponseTypeDef",
     "GetAccountSettingsResponseTypeDef",
     "UpdateAccountSettingsResponseTypeDef",
     "CreateSecurityConfigResponseTypeDef",
     "GetSecurityConfigResponseTypeDef",
     "UpdateSecurityConfigResponseTypeDef",
@@ -147,16 +150,16 @@
         "name": str,
         "policyVersion": str,
         "type": Literal["data"],
     },
     total=False,
 )
 
-CapacityLimitsTypeDef = TypedDict(
-    "CapacityLimitsTypeDef",
+CapacityLimitsOutputTypeDef = TypedDict(
+    "CapacityLimitsOutputTypeDef",
     {
         "maxIndexingCapacityInOCU": int,
         "maxSearchCapacityInOCU": int,
     },
     total=False,
 )
 
@@ -194,14 +197,25 @@
         "errorMessage": str,
         "id": str,
         "name": str,
     },
     total=False,
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
 BatchGetVpcEndpointRequestRequestTypeDef = TypedDict(
     "BatchGetVpcEndpointRequestRequestTypeDef",
     {
         "ids": Sequence[str],
     },
 )
 
@@ -225,14 +239,23 @@
         "errorCode": str,
         "errorMessage": str,
         "id": str,
     },
     total=False,
 )
 
+CapacityLimitsTypeDef = TypedDict(
+    "CapacityLimitsTypeDef",
+    {
+        "maxIndexingCapacityInOCU": int,
+        "maxSearchCapacityInOCU": int,
+    },
+    total=False,
+)
+
 CollectionFiltersTypeDef = TypedDict(
     "CollectionFiltersTypeDef",
     {
         "name": str,
         "status": CollectionStatusType,
     },
     total=False,
@@ -640,14 +663,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 VpcEndpointFiltersTypeDef = TypedDict(
     "VpcEndpointFiltersTypeDef",
     {
         "status": VpcEndpointStatusType,
     },
     total=False,
 )
@@ -658,25 +689,35 @@
         "id": str,
         "name": str,
         "status": VpcEndpointStatusType,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredSamlConfigOptionsOutputTypeDef = TypedDict(
+    "_RequiredSamlConfigOptionsOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "metadata": str,
+    },
+)
+_OptionalSamlConfigOptionsOutputTypeDef = TypedDict(
+    "_OptionalSamlConfigOptionsOutputTypeDef",
+    {
+        "groupAttribute": str,
+        "sessionTimeout": int,
+        "userAttribute": str,
     },
+    total=False,
 )
 
+class SamlConfigOptionsOutputTypeDef(
+    _RequiredSamlConfigOptionsOutputTypeDef, _OptionalSamlConfigOptionsOutputTypeDef
+):
+    pass
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -796,81 +837,81 @@
 )
 
 class UpdateVpcEndpointRequestRequestTypeDef(
     _RequiredUpdateVpcEndpointRequestRequestTypeDef, _OptionalUpdateVpcEndpointRequestRequestTypeDef
 ):
     pass
 
-CreateAccessPolicyResponseTypeDef = TypedDict(
-    "CreateAccessPolicyResponseTypeDef",
+AccountSettingsDetailTypeDef = TypedDict(
+    "AccountSettingsDetailTypeDef",
     {
-        "accessPolicyDetail": AccessPolicyDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "capacityLimits": CapacityLimitsOutputTypeDef,
     },
+    total=False,
 )
 
-GetAccessPolicyResponseTypeDef = TypedDict(
-    "GetAccessPolicyResponseTypeDef",
+BatchGetCollectionResponseTypeDef = TypedDict(
+    "BatchGetCollectionResponseTypeDef",
+    {
+        "collectionDetails": List[CollectionDetailTypeDef],
+        "collectionErrorDetails": List[CollectionErrorDetailTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAccessPolicyResponseTypeDef = TypedDict(
+    "CreateAccessPolicyResponseTypeDef",
     {
         "accessPolicyDetail": AccessPolicyDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateAccessPolicyResponseTypeDef = TypedDict(
-    "UpdateAccessPolicyResponseTypeDef",
+GetAccessPolicyResponseTypeDef = TypedDict(
+    "GetAccessPolicyResponseTypeDef",
     {
         "accessPolicyDetail": AccessPolicyDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccessPoliciesResponseTypeDef = TypedDict(
     "ListAccessPoliciesResponseTypeDef",
     {
         "accessPolicySummaries": List[AccessPolicySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AccountSettingsDetailTypeDef = TypedDict(
-    "AccountSettingsDetailTypeDef",
-    {
-        "capacityLimits": CapacityLimitsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateAccountSettingsRequestRequestTypeDef",
-    {
-        "capacityLimits": CapacityLimitsTypeDef,
-    },
-    total=False,
-)
-
-BatchGetCollectionResponseTypeDef = TypedDict(
-    "BatchGetCollectionResponseTypeDef",
+UpdateAccessPolicyResponseTypeDef = TypedDict(
+    "UpdateAccessPolicyResponseTypeDef",
     {
-        "collectionDetails": List[CollectionDetailTypeDef],
-        "collectionErrorDetails": List[CollectionErrorDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "accessPolicyDetail": AccessPolicyDetailTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetVpcEndpointResponseTypeDef = TypedDict(
     "BatchGetVpcEndpointResponseTypeDef",
     {
         "vpcEndpointDetails": List[VpcEndpointDetailTypeDef],
         "vpcEndpointErrorDetails": List[VpcEndpointErrorDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateAccountSettingsRequestRequestTypeDef",
+    {
+        "capacityLimits": CapacityLimitsTypeDef,
+    },
+    total=False,
+)
+
 ListCollectionsRequestRequestTypeDef = TypedDict(
     "ListCollectionsRequestRequestTypeDef",
     {
         "collectionFilters": CollectionFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
@@ -878,23 +919,23 @@
 )
 
 ListCollectionsResponseTypeDef = TypedDict(
     "ListCollectionsResponseTypeDef",
     {
         "collectionSummaries": List[CollectionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCollectionResponseTypeDef = TypedDict(
     "CreateCollectionResponseTypeDef",
     {
         "createCollectionDetail": CreateCollectionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCollectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCollectionRequestRequestTypeDef",
     {
         "name": str,
@@ -912,22 +953,14 @@
 )
 
 class CreateCollectionRequestRequestTypeDef(
     _RequiredCreateCollectionRequestRequestTypeDef, _OptionalCreateCollectionRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -951,28 +984,14 @@
 
 class CreateSecurityConfigRequestRequestTypeDef(
     _RequiredCreateSecurityConfigRequestRequestTypeDef,
     _OptionalCreateSecurityConfigRequestRequestTypeDef,
 ):
     pass
 
-SecurityConfigDetailTypeDef = TypedDict(
-    "SecurityConfigDetailTypeDef",
-    {
-        "configVersion": str,
-        "createdDate": int,
-        "description": str,
-        "id": str,
-        "lastModifiedDate": int,
-        "samlOptions": SamlConfigOptionsTypeDef,
-        "type": Literal["saml"],
-    },
-    total=False,
-)
-
 _RequiredUpdateSecurityConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSecurityConfigRequestRequestTypeDef",
     {
         "configVersion": str,
         "id": str,
     },
 )
@@ -992,84 +1011,92 @@
 ):
     pass
 
 CreateSecurityPolicyResponseTypeDef = TypedDict(
     "CreateSecurityPolicyResponseTypeDef",
     {
         "securityPolicyDetail": SecurityPolicyDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSecurityPolicyResponseTypeDef = TypedDict(
     "GetSecurityPolicyResponseTypeDef",
     {
         "securityPolicyDetail": SecurityPolicyDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSecurityPolicyResponseTypeDef = TypedDict(
     "UpdateSecurityPolicyResponseTypeDef",
     {
         "securityPolicyDetail": SecurityPolicyDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVpcEndpointResponseTypeDef = TypedDict(
     "CreateVpcEndpointResponseTypeDef",
     {
         "createVpcEndpointDetail": CreateVpcEndpointDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCollectionResponseTypeDef = TypedDict(
     "DeleteCollectionResponseTypeDef",
     {
         "deleteCollectionDetail": DeleteCollectionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVpcEndpointResponseTypeDef = TypedDict(
     "DeleteVpcEndpointResponseTypeDef",
     {
         "deleteVpcEndpointDetail": DeleteVpcEndpointDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPoliciesStatsResponseTypeDef = TypedDict(
     "GetPoliciesStatsResponseTypeDef",
     {
         "AccessPolicyStats": AccessPolicyStatsTypeDef,
         "SecurityConfigStats": SecurityConfigStatsTypeDef,
         "SecurityPolicyStats": SecurityPolicyStatsTypeDef,
         "TotalPolicyCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSecurityConfigsResponseTypeDef = TypedDict(
     "ListSecurityConfigsResponseTypeDef",
     {
         "nextToken": str,
         "securityConfigSummaries": List[SecurityConfigSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSecurityPoliciesResponseTypeDef = TypedDict(
     "ListSecurityPoliciesResponseTypeDef",
     {
         "nextToken": str,
         "securityPolicySummaries": List[SecurityPolicySummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVpcEndpointsRequestRequestTypeDef = TypedDict(
     "ListVpcEndpointsRequestRequestTypeDef",
     {
         "maxResults": int,
@@ -1080,66 +1107,80 @@
 )
 
 ListVpcEndpointsResponseTypeDef = TypedDict(
     "ListVpcEndpointsResponseTypeDef",
     {
         "nextToken": str,
         "vpcEndpointSummaries": List[VpcEndpointSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SecurityConfigDetailTypeDef = TypedDict(
+    "SecurityConfigDetailTypeDef",
+    {
+        "configVersion": str,
+        "createdDate": int,
+        "description": str,
+        "id": str,
+        "lastModifiedDate": int,
+        "samlOptions": SamlConfigOptionsOutputTypeDef,
+        "type": Literal["saml"],
+    },
+    total=False,
+)
+
 UpdateCollectionResponseTypeDef = TypedDict(
     "UpdateCollectionResponseTypeDef",
     {
         "updateCollectionDetail": UpdateCollectionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVpcEndpointResponseTypeDef = TypedDict(
     "UpdateVpcEndpointResponseTypeDef",
     {
         "UpdateVpcEndpointDetail": UpdateVpcEndpointDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountSettingsResponseTypeDef = TypedDict(
     "GetAccountSettingsResponseTypeDef",
     {
         "accountSettingsDetail": AccountSettingsDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAccountSettingsResponseTypeDef = TypedDict(
     "UpdateAccountSettingsResponseTypeDef",
     {
         "accountSettingsDetail": AccountSettingsDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSecurityConfigResponseTypeDef = TypedDict(
     "CreateSecurityConfigResponseTypeDef",
     {
         "securityConfigDetail": SecurityConfigDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSecurityConfigResponseTypeDef = TypedDict(
     "GetSecurityConfigResponseTypeDef",
     {
         "securityConfigDetail": SecurityConfigDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSecurityConfigResponseTypeDef = TypedDict(
     "UpdateSecurityConfigResponseTypeDef",
     {
         "securityConfigDetail": SecurityConfigDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless.egg-info/PKG-INFO` & `mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opensearchserverless
-Version: 1.28.0
-Summary: Type annotations for boto3.OpenSearchServiceServerless 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.OpenSearchServiceServerless 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-opensearchserverless"></a>
 
 # mypy-boto3-opensearchserverless
 
 [![PyPI - mypy-boto3-opensearchserverless](https://img.shields.io/pypi/v/mypy-boto3-opensearchserverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearchserverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearchserverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearchserverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opensearchserverless?color=blue)](https://pypistats.org/packages/mypy-boto3-opensearchserverless)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opensearchserverless)](https://pepy.tech/project/mypy-boto3-opensearchserverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchServiceServerless 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
+[boto3.OpenSearchServiceServerless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
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
 [mypy-boto3-opensearchserverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,21 +306,23 @@
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opensearchserverless.type_defs import (
     AccessPolicyDetailTypeDef,
     AccessPolicyStatsTypeDef,
     AccessPolicySummaryTypeDef,
-    CapacityLimitsTypeDef,
+    CapacityLimitsOutputTypeDef,
     BatchGetCollectionRequestRequestTypeDef,
     CollectionDetailTypeDef,
     CollectionErrorDetailTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetVpcEndpointRequestRequestTypeDef,
     VpcEndpointDetailTypeDef,
     VpcEndpointErrorDetailTypeDef,
+    CapacityLimitsTypeDef,
     CollectionFiltersTypeDef,
     CollectionSummaryTypeDef,
     CreateAccessPolicyRequestRequestTypeDef,
     CreateCollectionDetailTypeDef,
     TagTypeDef,
     SamlConfigOptionsTypeDef,
     CreateSecurityPolicyRequestRequestTypeDef,
@@ -341,52 +343,53 @@
     GetSecurityPolicyRequestRequestTypeDef,
     ListAccessPoliciesRequestRequestTypeDef,
     ListSecurityConfigsRequestRequestTypeDef,
     SecurityConfigSummaryTypeDef,
     ListSecurityPoliciesRequestRequestTypeDef,
     SecurityPolicySummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     VpcEndpointFiltersTypeDef,
     VpcEndpointSummaryTypeDef,
-    ResponseMetadataTypeDef,
+    SamlConfigOptionsOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccessPolicyRequestRequestTypeDef,
     UpdateCollectionDetailTypeDef,
     UpdateCollectionRequestRequestTypeDef,
     UpdateSecurityPolicyRequestRequestTypeDef,
     UpdateVpcEndpointDetailTypeDef,
     UpdateVpcEndpointRequestRequestTypeDef,
+    AccountSettingsDetailTypeDef,
+    BatchGetCollectionResponseTypeDef,
     CreateAccessPolicyResponseTypeDef,
     GetAccessPolicyResponseTypeDef,
-    UpdateAccessPolicyResponseTypeDef,
     ListAccessPoliciesResponseTypeDef,
-    AccountSettingsDetailTypeDef,
-    UpdateAccountSettingsRequestRequestTypeDef,
-    BatchGetCollectionResponseTypeDef,
+    UpdateAccessPolicyResponseTypeDef,
     BatchGetVpcEndpointResponseTypeDef,
+    UpdateAccountSettingsRequestRequestTypeDef,
     ListCollectionsRequestRequestTypeDef,
     ListCollectionsResponseTypeDef,
     CreateCollectionResponseTypeDef,
     CreateCollectionRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSecurityConfigRequestRequestTypeDef,
-    SecurityConfigDetailTypeDef,
     UpdateSecurityConfigRequestRequestTypeDef,
     CreateSecurityPolicyResponseTypeDef,
     GetSecurityPolicyResponseTypeDef,
     UpdateSecurityPolicyResponseTypeDef,
     CreateVpcEndpointResponseTypeDef,
     DeleteCollectionResponseTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     GetPoliciesStatsResponseTypeDef,
     ListSecurityConfigsResponseTypeDef,
     ListSecurityPoliciesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
     ListVpcEndpointsResponseTypeDef,
+    SecurityConfigDetailTypeDef,
     UpdateCollectionResponseTypeDef,
     UpdateVpcEndpointResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     UpdateAccountSettingsResponseTypeDef,
     CreateSecurityConfigResponseTypeDef,
     GetSecurityConfigResponseTypeDef,
     UpdateSecurityConfigResponseTypeDef,
```

### Comparing `mypy-boto3-opensearchserverless-1.28.0/mypy_boto3_opensearchserverless.egg-info/SOURCES.txt` & `mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearchserverless-1.28.0/setup.py` & `mypy-boto3-opensearchserverless-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-opensearchserverless",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_opensearchserverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.OpenSearchServiceServerless 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.OpenSearchServiceServerless 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

