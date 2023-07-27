# Comparing `tmp/mypy-boto3-managedblockchain-1.28.0.tar.gz` & `tmp/mypy-boto3-managedblockchain-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-managedblockchain-1.28.0.tar", last modified: Thu Jul  6 21:00:04 2023, max compression
+gzip compressed data, was "mypy-boto3-managedblockchain-1.28.12.tar", last modified: Thu Jul 27 05:34:59 2023, max compression
```

## Comparing `mypy-boto3-managedblockchain-1.28.0.tar` & `mypy-boto3-managedblockchain-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:04.266363 mypy-boto3-managedblockchain-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:46:32.000000 mypy-boto3-managedblockchain-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-07-06 21:00:04.262364 mypy-boto3-managedblockchain-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14629 2023-07-06 20:46:32.000000 mypy-boto3-managedblockchain-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:04.258364 mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-06 20:46:32.000000 mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-06 20:46:32.000000 mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-06 20:46:32.000000 mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20594 2023-07-06 20:46:32.000000 mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20559 2023-07-06 20:46:32.000000 mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-07-06 20:46:32.000000 mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-06 20:46:32.000000 mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-06 20:46:32.000000 mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-06 20:46:32.000000 mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:46:32.000000 mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26462 2023-07-06 20:46:33.000000 mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-07-06 20:46:33.000000 mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:46:32.000000 mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:04.262364 mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-07-06 21:00:04.000000 mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-06 21:00:04.000000 mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:04.000000 mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:04.000000 mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:04.000000 mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 21:00:04.000000 mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:04.266363 mypy-boto3-managedblockchain-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-06 20:46:32.000000 mypy-boto3-managedblockchain-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.648446 mypy-boto3-managedblockchain-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16593 2023-07-27 05:34:59.648446 mypy-boto3-managedblockchain-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15066 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.648446 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20594 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20559 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29044 2023-07-27 05:25:51.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29016 2023-07-27 05:25:51.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.648446 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16593 2023-07-27 05:34:59.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-27 05:34:59.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:59.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:59.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:59.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:59.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:59.648446 mypy-boto3-managedblockchain-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/setup.py
```

### Comparing `mypy-boto3-managedblockchain-1.28.0/LICENSE` & `mypy-boto3-managedblockchain-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.0/PKG-INFO` & `mypy-boto3-managedblockchain-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-managedblockchain
-Version: 1.28.0
-Summary: Type annotations for boto3.ManagedBlockchain 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ManagedBlockchain 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-managedblockchain"></a>
 
 # mypy-boto3-managedblockchain
 
 [![PyPI - mypy-boto3-managedblockchain](https://img.shields.io/pypi/v/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-managedblockchain?color=blue)](https://pypistats.org/packages/mypy-boto3-managedblockchain)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-managedblockchain)](https://pepy.tech/project/mypy-boto3-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchain 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[boto3.ManagedBlockchain 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
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
 [mypy-boto3-managedblockchain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,14 +334,15 @@
 `mypy_boto3_managedblockchain.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_managedblockchain.type_defs import (
     AccessorSummaryTypeDef,
     AccessorTypeDef,
+    ApprovalThresholdPolicyOutputTypeDef,
     ApprovalThresholdPolicyTypeDef,
     CreateAccessorInputRequestTypeDef,
     CreateAccessorOutputTypeDef,
     CreateMemberOutputTypeDef,
     CreateNetworkOutputTypeDef,
     CreateNodeOutputTypeDef,
     CreateProposalOutputTypeDef,
@@ -350,14 +351,15 @@
     DeleteNodeInputRequestTypeDef,
     GetAccessorInputRequestTypeDef,
     GetMemberInputRequestTypeDef,
     GetNetworkInputRequestTypeDef,
     GetNodeInputRequestTypeDef,
     GetProposalInputRequestTypeDef,
     NetworkSummaryTypeDef,
+    InviteActionOutputTypeDef,
     InviteActionTypeDef,
     ListAccessorsInputListAccessorsPaginateTypeDef,
     ListAccessorsInputRequestTypeDef,
     ListInvitationsInputRequestTypeDef,
     ListMembersInputRequestTypeDef,
     MemberSummaryTypeDef,
     ListNetworksInputRequestTypeDef,
@@ -365,66 +367,75 @@
     NodeSummaryTypeDef,
     ListProposalVotesInputRequestTypeDef,
     VoteSummaryTypeDef,
     ListProposalsInputRequestTypeDef,
     ProposalSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
+    LogConfigurationOutputTypeDef,
     LogConfigurationTypeDef,
     MemberFabricAttributesTypeDef,
     MemberFabricConfigurationTypeDef,
     NetworkEthereumAttributesTypeDef,
     NetworkFabricAttributesTypeDef,
     NetworkFabricConfigurationTypeDef,
     NodeEthereumAttributesTypeDef,
     NodeFabricAttributesTypeDef,
     PaginatorConfigTypeDef,
+    RemoveActionOutputTypeDef,
     RemoveActionTypeDef,
     RejectInvitationInputRequestTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     VoteOnProposalInputRequestTypeDef,
     ListAccessorsOutputTypeDef,
     GetAccessorOutputTypeDef,
+    VotingPolicyOutputTypeDef,
     VotingPolicyTypeDef,
     InvitationTypeDef,
     ListNetworksOutputTypeDef,
     ListMembersOutputTypeDef,
     ListNodesOutputTypeDef,
     ListProposalVotesOutputTypeDef,
     ListProposalsOutputTypeDef,
+    LogConfigurationsOutputTypeDef,
     LogConfigurationsTypeDef,
     MemberFrameworkAttributesTypeDef,
     MemberFrameworkConfigurationTypeDef,
     NetworkFrameworkAttributesTypeDef,
     NetworkFrameworkConfigurationTypeDef,
     NodeFrameworkAttributesTypeDef,
+    ProposalActionsOutputTypeDef,
     ProposalActionsTypeDef,
     ListInvitationsOutputTypeDef,
+    MemberFabricLogPublishingConfigurationOutputTypeDef,
+    NodeFabricLogPublishingConfigurationOutputTypeDef,
     MemberFabricLogPublishingConfigurationTypeDef,
     NodeFabricLogPublishingConfigurationTypeDef,
     NetworkTypeDef,
-    CreateProposalInputRequestTypeDef,
     ProposalTypeDef,
+    CreateProposalInputRequestTypeDef,
+    MemberLogPublishingConfigurationOutputTypeDef,
+    NodeLogPublishingConfigurationOutputTypeDef,
     MemberLogPublishingConfigurationTypeDef,
     NodeLogPublishingConfigurationTypeDef,
     GetNetworkOutputTypeDef,
     GetProposalOutputTypeDef,
-    MemberConfigurationTypeDef,
     MemberTypeDef,
+    NodeTypeDef,
+    MemberConfigurationTypeDef,
     UpdateMemberInputRequestTypeDef,
     NodeConfigurationTypeDef,
-    NodeTypeDef,
     UpdateNodeInputRequestTypeDef,
+    GetMemberOutputTypeDef,
+    GetNodeOutputTypeDef,
     CreateMemberInputRequestTypeDef,
     CreateNetworkInputRequestTypeDef,
-    GetMemberOutputTypeDef,
     CreateNodeInputRequestTypeDef,
-    GetNodeOutputTypeDef,
 )
 
 
 def get_structure() -> AccessorSummaryTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-managedblockchain-1.28.0/README.md` & `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-managedblockchain
+Version: 1.28.12
+Summary: Type annotations for boto3.ManagedBlockchain 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 managedblockchain type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-managedblockchain"></a>
 
 # mypy-boto3-managedblockchain
 
 [![PyPI - mypy-boto3-managedblockchain](https://img.shields.io/pypi/v/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-managedblockchain?color=blue)](https://pypistats.org/packages/mypy-boto3-managedblockchain)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-managedblockchain)](https://pepy.tech/project/mypy-boto3-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchain 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[boto3.ManagedBlockchain 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
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
 [mypy-boto3-managedblockchain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,14 +334,15 @@
 `mypy_boto3_managedblockchain.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_managedblockchain.type_defs import (
     AccessorSummaryTypeDef,
     AccessorTypeDef,
+    ApprovalThresholdPolicyOutputTypeDef,
     ApprovalThresholdPolicyTypeDef,
     CreateAccessorInputRequestTypeDef,
     CreateAccessorOutputTypeDef,
     CreateMemberOutputTypeDef,
     CreateNetworkOutputTypeDef,
     CreateNodeOutputTypeDef,
     CreateProposalOutputTypeDef,
@@ -318,14 +351,15 @@
     DeleteNodeInputRequestTypeDef,
     GetAccessorInputRequestTypeDef,
     GetMemberInputRequestTypeDef,
     GetNetworkInputRequestTypeDef,
     GetNodeInputRequestTypeDef,
     GetProposalInputRequestTypeDef,
     NetworkSummaryTypeDef,
+    InviteActionOutputTypeDef,
     InviteActionTypeDef,
     ListAccessorsInputListAccessorsPaginateTypeDef,
     ListAccessorsInputRequestTypeDef,
     ListInvitationsInputRequestTypeDef,
     ListMembersInputRequestTypeDef,
     MemberSummaryTypeDef,
     ListNetworksInputRequestTypeDef,
@@ -333,66 +367,75 @@
     NodeSummaryTypeDef,
     ListProposalVotesInputRequestTypeDef,
     VoteSummaryTypeDef,
     ListProposalsInputRequestTypeDef,
     ProposalSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
+    LogConfigurationOutputTypeDef,
     LogConfigurationTypeDef,
     MemberFabricAttributesTypeDef,
     MemberFabricConfigurationTypeDef,
     NetworkEthereumAttributesTypeDef,
     NetworkFabricAttributesTypeDef,
     NetworkFabricConfigurationTypeDef,
     NodeEthereumAttributesTypeDef,
     NodeFabricAttributesTypeDef,
     PaginatorConfigTypeDef,
+    RemoveActionOutputTypeDef,
     RemoveActionTypeDef,
     RejectInvitationInputRequestTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     VoteOnProposalInputRequestTypeDef,
     ListAccessorsOutputTypeDef,
     GetAccessorOutputTypeDef,
+    VotingPolicyOutputTypeDef,
     VotingPolicyTypeDef,
     InvitationTypeDef,
     ListNetworksOutputTypeDef,
     ListMembersOutputTypeDef,
     ListNodesOutputTypeDef,
     ListProposalVotesOutputTypeDef,
     ListProposalsOutputTypeDef,
+    LogConfigurationsOutputTypeDef,
     LogConfigurationsTypeDef,
     MemberFrameworkAttributesTypeDef,
     MemberFrameworkConfigurationTypeDef,
     NetworkFrameworkAttributesTypeDef,
     NetworkFrameworkConfigurationTypeDef,
     NodeFrameworkAttributesTypeDef,
+    ProposalActionsOutputTypeDef,
     ProposalActionsTypeDef,
     ListInvitationsOutputTypeDef,
+    MemberFabricLogPublishingConfigurationOutputTypeDef,
+    NodeFabricLogPublishingConfigurationOutputTypeDef,
     MemberFabricLogPublishingConfigurationTypeDef,
     NodeFabricLogPublishingConfigurationTypeDef,
     NetworkTypeDef,
-    CreateProposalInputRequestTypeDef,
     ProposalTypeDef,
+    CreateProposalInputRequestTypeDef,
+    MemberLogPublishingConfigurationOutputTypeDef,
+    NodeLogPublishingConfigurationOutputTypeDef,
     MemberLogPublishingConfigurationTypeDef,
     NodeLogPublishingConfigurationTypeDef,
     GetNetworkOutputTypeDef,
     GetProposalOutputTypeDef,
-    MemberConfigurationTypeDef,
     MemberTypeDef,
+    NodeTypeDef,
+    MemberConfigurationTypeDef,
     UpdateMemberInputRequestTypeDef,
     NodeConfigurationTypeDef,
-    NodeTypeDef,
     UpdateNodeInputRequestTypeDef,
+    GetMemberOutputTypeDef,
+    GetNodeOutputTypeDef,
     CreateMemberInputRequestTypeDef,
     CreateNetworkInputRequestTypeDef,
-    GetMemberOutputTypeDef,
     CreateNodeInputRequestTypeDef,
-    GetNodeOutputTypeDef,
 )
 
 
 def get_structure() -> AccessorSummaryTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/__init__.py` & `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/__init__.pyi` & `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/__main__.py` & `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ManagedBlockchain 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ManagedBlockchain 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain\nOther"
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

### Comparing `mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/client.py` & `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/client.pyi` & `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/literals.py` & `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/literals.py`

 * *Files 1% similar despite different names*

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

### Comparing `mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/literals.pyi` & `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,15 @@
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
@@ -272,26 +273,28 @@
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

### Comparing `mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/paginator.py` & `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/paginator.pyi` & `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/type_defs.py` & `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -34,18 +34,18 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessorSummaryTypeDef",
     "AccessorTypeDef",
+    "ApprovalThresholdPolicyOutputTypeDef",
     "ApprovalThresholdPolicyTypeDef",
     "CreateAccessorInputRequestTypeDef",
     "CreateAccessorOutputTypeDef",
     "CreateMemberOutputTypeDef",
     "CreateNetworkOutputTypeDef",
     "CreateNodeOutputTypeDef",
     "CreateProposalOutputTypeDef",
@@ -54,14 +54,15 @@
     "DeleteNodeInputRequestTypeDef",
     "GetAccessorInputRequestTypeDef",
     "GetMemberInputRequestTypeDef",
     "GetNetworkInputRequestTypeDef",
     "GetNodeInputRequestTypeDef",
     "GetProposalInputRequestTypeDef",
     "NetworkSummaryTypeDef",
+    "InviteActionOutputTypeDef",
     "InviteActionTypeDef",
     "ListAccessorsInputListAccessorsPaginateTypeDef",
     "ListAccessorsInputRequestTypeDef",
     "ListInvitationsInputRequestTypeDef",
     "ListMembersInputRequestTypeDef",
     "MemberSummaryTypeDef",
     "ListNetworksInputRequestTypeDef",
@@ -69,66 +70,75 @@
     "NodeSummaryTypeDef",
     "ListProposalVotesInputRequestTypeDef",
     "VoteSummaryTypeDef",
     "ListProposalsInputRequestTypeDef",
     "ProposalSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "LogConfigurationOutputTypeDef",
     "LogConfigurationTypeDef",
     "MemberFabricAttributesTypeDef",
     "MemberFabricConfigurationTypeDef",
     "NetworkEthereumAttributesTypeDef",
     "NetworkFabricAttributesTypeDef",
     "NetworkFabricConfigurationTypeDef",
     "NodeEthereumAttributesTypeDef",
     "NodeFabricAttributesTypeDef",
     "PaginatorConfigTypeDef",
+    "RemoveActionOutputTypeDef",
     "RemoveActionTypeDef",
     "RejectInvitationInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "VoteOnProposalInputRequestTypeDef",
     "ListAccessorsOutputTypeDef",
     "GetAccessorOutputTypeDef",
+    "VotingPolicyOutputTypeDef",
     "VotingPolicyTypeDef",
     "InvitationTypeDef",
     "ListNetworksOutputTypeDef",
     "ListMembersOutputTypeDef",
     "ListNodesOutputTypeDef",
     "ListProposalVotesOutputTypeDef",
     "ListProposalsOutputTypeDef",
+    "LogConfigurationsOutputTypeDef",
     "LogConfigurationsTypeDef",
     "MemberFrameworkAttributesTypeDef",
     "MemberFrameworkConfigurationTypeDef",
     "NetworkFrameworkAttributesTypeDef",
     "NetworkFrameworkConfigurationTypeDef",
     "NodeFrameworkAttributesTypeDef",
+    "ProposalActionsOutputTypeDef",
     "ProposalActionsTypeDef",
     "ListInvitationsOutputTypeDef",
+    "MemberFabricLogPublishingConfigurationOutputTypeDef",
+    "NodeFabricLogPublishingConfigurationOutputTypeDef",
     "MemberFabricLogPublishingConfigurationTypeDef",
     "NodeFabricLogPublishingConfigurationTypeDef",
     "NetworkTypeDef",
-    "CreateProposalInputRequestTypeDef",
     "ProposalTypeDef",
+    "CreateProposalInputRequestTypeDef",
+    "MemberLogPublishingConfigurationOutputTypeDef",
+    "NodeLogPublishingConfigurationOutputTypeDef",
     "MemberLogPublishingConfigurationTypeDef",
     "NodeLogPublishingConfigurationTypeDef",
     "GetNetworkOutputTypeDef",
     "GetProposalOutputTypeDef",
-    "MemberConfigurationTypeDef",
     "MemberTypeDef",
+    "NodeTypeDef",
+    "MemberConfigurationTypeDef",
     "UpdateMemberInputRequestTypeDef",
     "NodeConfigurationTypeDef",
-    "NodeTypeDef",
     "UpdateNodeInputRequestTypeDef",
+    "GetMemberOutputTypeDef",
+    "GetNodeOutputTypeDef",
     "CreateMemberInputRequestTypeDef",
     "CreateNetworkInputRequestTypeDef",
-    "GetMemberOutputTypeDef",
     "CreateNodeInputRequestTypeDef",
-    "GetNodeOutputTypeDef",
 )
 
 AccessorSummaryTypeDef = TypedDict(
     "AccessorSummaryTypeDef",
     {
         "Id": str,
         "Type": Literal["BILLING_TOKEN"],
@@ -149,14 +159,24 @@
         "CreationDate": datetime,
         "Arn": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+ApprovalThresholdPolicyOutputTypeDef = TypedDict(
+    "ApprovalThresholdPolicyOutputTypeDef",
+    {
+        "ThresholdPercentage": int,
+        "ProposalDurationInHours": int,
+        "ThresholdComparator": ThresholdComparatorType,
+    },
+    total=False,
+)
+
 ApprovalThresholdPolicyTypeDef = TypedDict(
     "ApprovalThresholdPolicyTypeDef",
     {
         "ThresholdPercentage": int,
         "ProposalDurationInHours": int,
         "ThresholdComparator": ThresholdComparatorType,
     },
@@ -174,21 +194,19 @@
     "_OptionalCreateAccessorInputRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateAccessorInputRequestTypeDef(
     _RequiredCreateAccessorInputRequestTypeDef, _OptionalCreateAccessorInputRequestTypeDef
 ):
     pass
 
-
 CreateAccessorOutputTypeDef = TypedDict(
     "CreateAccessorOutputTypeDef",
     {
         "AccessorId": str,
         "BillingToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -253,21 +271,19 @@
     "_OptionalDeleteNodeInputRequestTypeDef",
     {
         "MemberId": str,
     },
     total=False,
 )
 
-
 class DeleteNodeInputRequestTypeDef(
     _RequiredDeleteNodeInputRequestTypeDef, _OptionalDeleteNodeInputRequestTypeDef
 ):
     pass
 
-
 GetAccessorInputRequestTypeDef = TypedDict(
     "GetAccessorInputRequestTypeDef",
     {
         "AccessorId": str,
     },
 )
 
@@ -297,21 +313,19 @@
     "_OptionalGetNodeInputRequestTypeDef",
     {
         "MemberId": str,
     },
     total=False,
 )
 
-
 class GetNodeInputRequestTypeDef(
     _RequiredGetNodeInputRequestTypeDef, _OptionalGetNodeInputRequestTypeDef
 ):
     pass
 
-
 GetProposalInputRequestTypeDef = TypedDict(
     "GetProposalInputRequestTypeDef",
     {
         "NetworkId": str,
         "ProposalId": str,
     },
 )
@@ -327,14 +341,21 @@
         "Status": NetworkStatusType,
         "CreationDate": datetime,
         "Arn": str,
     },
     total=False,
 )
 
+InviteActionOutputTypeDef = TypedDict(
+    "InviteActionOutputTypeDef",
+    {
+        "Principal": str,
+    },
+)
+
 InviteActionTypeDef = TypedDict(
     "InviteActionTypeDef",
     {
         "Principal": str,
     },
 )
 
@@ -378,21 +399,19 @@
         "IsOwned": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListMembersInputRequestTypeDef(
     _RequiredListMembersInputRequestTypeDef, _OptionalListMembersInputRequestTypeDef
 ):
     pass
 
-
 MemberSummaryTypeDef = TypedDict(
     "MemberSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
         "Status": MemberStatusType,
@@ -428,21 +447,19 @@
         "Status": NodeStatusType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListNodesInputRequestTypeDef(
     _RequiredListNodesInputRequestTypeDef, _OptionalListNodesInputRequestTypeDef
 ):
     pass
 
-
 NodeSummaryTypeDef = TypedDict(
     "NodeSummaryTypeDef",
     {
         "Id": str,
         "Status": NodeStatusType,
         "CreationDate": datetime,
         "AvailabilityZone": str,
@@ -464,21 +481,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListProposalVotesInputRequestTypeDef(
     _RequiredListProposalVotesInputRequestTypeDef, _OptionalListProposalVotesInputRequestTypeDef
 ):
     pass
 
-
 VoteSummaryTypeDef = TypedDict(
     "VoteSummaryTypeDef",
     {
         "Vote": VoteValueType,
         "MemberName": str,
         "MemberId": str,
     },
@@ -496,21 +511,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListProposalsInputRequestTypeDef(
     _RequiredListProposalsInputRequestTypeDef, _OptionalListProposalsInputRequestTypeDef
 ):
     pass
 
-
 ProposalSummaryTypeDef = TypedDict(
     "ProposalSummaryTypeDef",
     {
         "ProposalId": str,
         "Description": str,
         "ProposedByMemberId": str,
         "ProposedByMemberName": str,
@@ -533,14 +546,22 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LogConfigurationOutputTypeDef = TypedDict(
+    "LogConfigurationOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 LogConfigurationTypeDef = TypedDict(
     "LogConfigurationTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -610,14 +631,21 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+RemoveActionOutputTypeDef = TypedDict(
+    "RemoveActionOutputTypeDef",
+    {
+        "MemberId": str,
+    },
+)
+
 RemoveActionTypeDef = TypedDict(
     "RemoveActionTypeDef",
     {
         "MemberId": str,
     },
 )
 
@@ -678,14 +706,22 @@
     "GetAccessorOutputTypeDef",
     {
         "Accessor": AccessorTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+VotingPolicyOutputTypeDef = TypedDict(
+    "VotingPolicyOutputTypeDef",
+    {
+        "ApprovalThresholdPolicy": ApprovalThresholdPolicyOutputTypeDef,
+    },
+    total=False,
+)
+
 VotingPolicyTypeDef = TypedDict(
     "VotingPolicyTypeDef",
     {
         "ApprovalThresholdPolicy": ApprovalThresholdPolicyTypeDef,
     },
     total=False,
 )
@@ -744,14 +780,22 @@
     {
         "Proposals": List[ProposalSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LogConfigurationsOutputTypeDef = TypedDict(
+    "LogConfigurationsOutputTypeDef",
+    {
+        "Cloudwatch": LogConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 LogConfigurationsTypeDef = TypedDict(
     "LogConfigurationsTypeDef",
     {
         "Cloudwatch": LogConfigurationTypeDef,
     },
     total=False,
 )
@@ -794,14 +838,23 @@
     {
         "Fabric": NodeFabricAttributesTypeDef,
         "Ethereum": NodeEthereumAttributesTypeDef,
     },
     total=False,
 )
 
+ProposalActionsOutputTypeDef = TypedDict(
+    "ProposalActionsOutputTypeDef",
+    {
+        "Invitations": List[InviteActionOutputTypeDef],
+        "Removals": List[RemoveActionOutputTypeDef],
+    },
+    total=False,
+)
+
 ProposalActionsTypeDef = TypedDict(
     "ProposalActionsTypeDef",
     {
         "Invitations": Sequence[InviteActionTypeDef],
         "Removals": Sequence[RemoveActionTypeDef],
     },
     total=False,
@@ -812,14 +865,31 @@
     {
         "Invitations": List[InvitationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+MemberFabricLogPublishingConfigurationOutputTypeDef = TypedDict(
+    "MemberFabricLogPublishingConfigurationOutputTypeDef",
+    {
+        "CaLogs": LogConfigurationsOutputTypeDef,
+    },
+    total=False,
+)
+
+NodeFabricLogPublishingConfigurationOutputTypeDef = TypedDict(
+    "NodeFabricLogPublishingConfigurationOutputTypeDef",
+    {
+        "ChaincodeLogs": LogConfigurationsOutputTypeDef,
+        "PeerLogs": LogConfigurationsOutputTypeDef,
+    },
+    total=False,
+)
+
 MemberFabricLogPublishingConfigurationTypeDef = TypedDict(
     "MemberFabricLogPublishingConfigurationTypeDef",
     {
         "CaLogs": LogConfigurationsTypeDef,
     },
     total=False,
 )
@@ -839,23 +909,44 @@
         "Id": str,
         "Name": str,
         "Description": str,
         "Framework": FrameworkType,
         "FrameworkVersion": str,
         "FrameworkAttributes": NetworkFrameworkAttributesTypeDef,
         "VpcEndpointServiceName": str,
-        "VotingPolicy": VotingPolicyTypeDef,
+        "VotingPolicy": VotingPolicyOutputTypeDef,
         "Status": NetworkStatusType,
         "CreationDate": datetime,
         "Tags": Dict[str, str],
         "Arn": str,
     },
     total=False,
 )
 
+ProposalTypeDef = TypedDict(
+    "ProposalTypeDef",
+    {
+        "ProposalId": str,
+        "NetworkId": str,
+        "Description": str,
+        "Actions": ProposalActionsOutputTypeDef,
+        "ProposedByMemberId": str,
+        "ProposedByMemberName": str,
+        "Status": ProposalStatusType,
+        "CreationDate": datetime,
+        "ExpirationDate": datetime,
+        "YesVoteCount": int,
+        "NoVoteCount": int,
+        "OutstandingVoteCount": int,
+        "Tags": Dict[str, str],
+        "Arn": str,
+    },
+    total=False,
+)
+
 _RequiredCreateProposalInputRequestTypeDef = TypedDict(
     "_RequiredCreateProposalInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "NetworkId": str,
         "MemberId": str,
         "Actions": ProposalActionsTypeDef,
@@ -866,38 +957,31 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateProposalInputRequestTypeDef(
     _RequiredCreateProposalInputRequestTypeDef, _OptionalCreateProposalInputRequestTypeDef
 ):
     pass
 
+MemberLogPublishingConfigurationOutputTypeDef = TypedDict(
+    "MemberLogPublishingConfigurationOutputTypeDef",
+    {
+        "Fabric": MemberFabricLogPublishingConfigurationOutputTypeDef,
+    },
+    total=False,
+)
 
-ProposalTypeDef = TypedDict(
-    "ProposalTypeDef",
+NodeLogPublishingConfigurationOutputTypeDef = TypedDict(
+    "NodeLogPublishingConfigurationOutputTypeDef",
     {
-        "ProposalId": str,
-        "NetworkId": str,
-        "Description": str,
-        "Actions": ProposalActionsTypeDef,
-        "ProposedByMemberId": str,
-        "ProposedByMemberName": str,
-        "Status": ProposalStatusType,
-        "CreationDate": datetime,
-        "ExpirationDate": datetime,
-        "YesVoteCount": int,
-        "NoVoteCount": int,
-        "OutstandingVoteCount": int,
-        "Tags": Dict[str, str],
-        "Arn": str,
+        "Fabric": NodeFabricLogPublishingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 MemberLogPublishingConfigurationTypeDef = TypedDict(
     "MemberLogPublishingConfigurationTypeDef",
     {
@@ -926,14 +1010,52 @@
     "GetProposalOutputTypeDef",
     {
         "Proposal": ProposalTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+MemberTypeDef = TypedDict(
+    "MemberTypeDef",
+    {
+        "NetworkId": str,
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "FrameworkAttributes": MemberFrameworkAttributesTypeDef,
+        "LogPublishingConfiguration": MemberLogPublishingConfigurationOutputTypeDef,
+        "Status": MemberStatusType,
+        "CreationDate": datetime,
+        "Tags": Dict[str, str],
+        "Arn": str,
+        "KmsKeyArn": str,
+    },
+    total=False,
+)
+
+NodeTypeDef = TypedDict(
+    "NodeTypeDef",
+    {
+        "NetworkId": str,
+        "MemberId": str,
+        "Id": str,
+        "InstanceType": str,
+        "AvailabilityZone": str,
+        "FrameworkAttributes": NodeFrameworkAttributesTypeDef,
+        "LogPublishingConfiguration": NodeLogPublishingConfigurationOutputTypeDef,
+        "StateDB": StateDBTypeType,
+        "Status": NodeStatusType,
+        "CreationDate": datetime,
+        "Tags": Dict[str, str],
+        "Arn": str,
+        "KmsKeyArn": str,
+    },
+    total=False,
+)
+
 _RequiredMemberConfigurationTypeDef = TypedDict(
     "_RequiredMemberConfigurationTypeDef",
     {
         "Name": str,
         "FrameworkConfiguration": MemberFrameworkConfigurationTypeDef,
     },
 )
@@ -944,39 +1066,19 @@
         "LogPublishingConfiguration": MemberLogPublishingConfigurationTypeDef,
         "Tags": Mapping[str, str],
         "KmsKeyArn": str,
     },
     total=False,
 )
 
-
 class MemberConfigurationTypeDef(
     _RequiredMemberConfigurationTypeDef, _OptionalMemberConfigurationTypeDef
 ):
     pass
 
-
-MemberTypeDef = TypedDict(
-    "MemberTypeDef",
-    {
-        "NetworkId": str,
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "FrameworkAttributes": MemberFrameworkAttributesTypeDef,
-        "LogPublishingConfiguration": MemberLogPublishingConfigurationTypeDef,
-        "Status": MemberStatusType,
-        "CreationDate": datetime,
-        "Tags": Dict[str, str],
-        "Arn": str,
-        "KmsKeyArn": str,
-    },
-    total=False,
-)
-
 _RequiredUpdateMemberInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMemberInputRequestTypeDef",
     {
         "NetworkId": str,
         "MemberId": str,
     },
 )
@@ -984,21 +1086,19 @@
     "_OptionalUpdateMemberInputRequestTypeDef",
     {
         "LogPublishingConfiguration": MemberLogPublishingConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateMemberInputRequestTypeDef(
     _RequiredUpdateMemberInputRequestTypeDef, _OptionalUpdateMemberInputRequestTypeDef
 ):
     pass
 
-
 _RequiredNodeConfigurationTypeDef = TypedDict(
     "_RequiredNodeConfigurationTypeDef",
     {
         "InstanceType": str,
     },
 )
 _OptionalNodeConfigurationTypeDef = TypedDict(
@@ -1007,41 +1107,19 @@
         "AvailabilityZone": str,
         "LogPublishingConfiguration": NodeLogPublishingConfigurationTypeDef,
         "StateDB": StateDBTypeType,
     },
     total=False,
 )
 
-
 class NodeConfigurationTypeDef(
     _RequiredNodeConfigurationTypeDef, _OptionalNodeConfigurationTypeDef
 ):
     pass
 
-
-NodeTypeDef = TypedDict(
-    "NodeTypeDef",
-    {
-        "NetworkId": str,
-        "MemberId": str,
-        "Id": str,
-        "InstanceType": str,
-        "AvailabilityZone": str,
-        "FrameworkAttributes": NodeFrameworkAttributesTypeDef,
-        "LogPublishingConfiguration": NodeLogPublishingConfigurationTypeDef,
-        "StateDB": StateDBTypeType,
-        "Status": NodeStatusType,
-        "CreationDate": datetime,
-        "Tags": Dict[str, str],
-        "Arn": str,
-        "KmsKeyArn": str,
-    },
-    total=False,
-)
-
 _RequiredUpdateNodeInputRequestTypeDef = TypedDict(
     "_RequiredUpdateNodeInputRequestTypeDef",
     {
         "NetworkId": str,
         "NodeId": str,
     },
 )
@@ -1050,20 +1128,34 @@
     {
         "MemberId": str,
         "LogPublishingConfiguration": NodeLogPublishingConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateNodeInputRequestTypeDef(
     _RequiredUpdateNodeInputRequestTypeDef, _OptionalUpdateNodeInputRequestTypeDef
 ):
     pass
 
+GetMemberOutputTypeDef = TypedDict(
+    "GetMemberOutputTypeDef",
+    {
+        "Member": MemberTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetNodeOutputTypeDef = TypedDict(
+    "GetNodeOutputTypeDef",
+    {
+        "Node": NodeTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 CreateMemberInputRequestTypeDef = TypedDict(
     "CreateMemberInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "InvitationId": str,
         "NetworkId": str,
@@ -1088,29 +1180,19 @@
         "Description": str,
         "FrameworkConfiguration": NetworkFrameworkConfigurationTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateNetworkInputRequestTypeDef(
     _RequiredCreateNetworkInputRequestTypeDef, _OptionalCreateNetworkInputRequestTypeDef
 ):
     pass
 
-
-GetMemberOutputTypeDef = TypedDict(
-    "GetMemberOutputTypeDef",
-    {
-        "Member": MemberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateNodeInputRequestTypeDef = TypedDict(
     "_RequiredCreateNodeInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "NetworkId": str,
         "NodeConfiguration": NodeConfigurationTypeDef,
     },
@@ -1120,21 +1202,11 @@
     {
         "MemberId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateNodeInputRequestTypeDef(
     _RequiredCreateNodeInputRequestTypeDef, _OptionalCreateNodeInputRequestTypeDef
 ):
     pass
-
-
-GetNodeOutputTypeDef = TypedDict(
-    "GetNodeOutputTypeDef",
-    {
-        "Node": NodeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain/type_defs.pyi` & `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,17 +34,19 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccessorSummaryTypeDef",
     "AccessorTypeDef",
+    "ApprovalThresholdPolicyOutputTypeDef",
     "ApprovalThresholdPolicyTypeDef",
     "CreateAccessorInputRequestTypeDef",
     "CreateAccessorOutputTypeDef",
     "CreateMemberOutputTypeDef",
     "CreateNetworkOutputTypeDef",
     "CreateNodeOutputTypeDef",
     "CreateProposalOutputTypeDef",
@@ -53,14 +55,15 @@
     "DeleteNodeInputRequestTypeDef",
     "GetAccessorInputRequestTypeDef",
     "GetMemberInputRequestTypeDef",
     "GetNetworkInputRequestTypeDef",
     "GetNodeInputRequestTypeDef",
     "GetProposalInputRequestTypeDef",
     "NetworkSummaryTypeDef",
+    "InviteActionOutputTypeDef",
     "InviteActionTypeDef",
     "ListAccessorsInputListAccessorsPaginateTypeDef",
     "ListAccessorsInputRequestTypeDef",
     "ListInvitationsInputRequestTypeDef",
     "ListMembersInputRequestTypeDef",
     "MemberSummaryTypeDef",
     "ListNetworksInputRequestTypeDef",
@@ -68,66 +71,75 @@
     "NodeSummaryTypeDef",
     "ListProposalVotesInputRequestTypeDef",
     "VoteSummaryTypeDef",
     "ListProposalsInputRequestTypeDef",
     "ProposalSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "LogConfigurationOutputTypeDef",
     "LogConfigurationTypeDef",
     "MemberFabricAttributesTypeDef",
     "MemberFabricConfigurationTypeDef",
     "NetworkEthereumAttributesTypeDef",
     "NetworkFabricAttributesTypeDef",
     "NetworkFabricConfigurationTypeDef",
     "NodeEthereumAttributesTypeDef",
     "NodeFabricAttributesTypeDef",
     "PaginatorConfigTypeDef",
+    "RemoveActionOutputTypeDef",
     "RemoveActionTypeDef",
     "RejectInvitationInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "VoteOnProposalInputRequestTypeDef",
     "ListAccessorsOutputTypeDef",
     "GetAccessorOutputTypeDef",
+    "VotingPolicyOutputTypeDef",
     "VotingPolicyTypeDef",
     "InvitationTypeDef",
     "ListNetworksOutputTypeDef",
     "ListMembersOutputTypeDef",
     "ListNodesOutputTypeDef",
     "ListProposalVotesOutputTypeDef",
     "ListProposalsOutputTypeDef",
+    "LogConfigurationsOutputTypeDef",
     "LogConfigurationsTypeDef",
     "MemberFrameworkAttributesTypeDef",
     "MemberFrameworkConfigurationTypeDef",
     "NetworkFrameworkAttributesTypeDef",
     "NetworkFrameworkConfigurationTypeDef",
     "NodeFrameworkAttributesTypeDef",
+    "ProposalActionsOutputTypeDef",
     "ProposalActionsTypeDef",
     "ListInvitationsOutputTypeDef",
+    "MemberFabricLogPublishingConfigurationOutputTypeDef",
+    "NodeFabricLogPublishingConfigurationOutputTypeDef",
     "MemberFabricLogPublishingConfigurationTypeDef",
     "NodeFabricLogPublishingConfigurationTypeDef",
     "NetworkTypeDef",
-    "CreateProposalInputRequestTypeDef",
     "ProposalTypeDef",
+    "CreateProposalInputRequestTypeDef",
+    "MemberLogPublishingConfigurationOutputTypeDef",
+    "NodeLogPublishingConfigurationOutputTypeDef",
     "MemberLogPublishingConfigurationTypeDef",
     "NodeLogPublishingConfigurationTypeDef",
     "GetNetworkOutputTypeDef",
     "GetProposalOutputTypeDef",
-    "MemberConfigurationTypeDef",
     "MemberTypeDef",
+    "NodeTypeDef",
+    "MemberConfigurationTypeDef",
     "UpdateMemberInputRequestTypeDef",
     "NodeConfigurationTypeDef",
-    "NodeTypeDef",
     "UpdateNodeInputRequestTypeDef",
+    "GetMemberOutputTypeDef",
+    "GetNodeOutputTypeDef",
     "CreateMemberInputRequestTypeDef",
     "CreateNetworkInputRequestTypeDef",
-    "GetMemberOutputTypeDef",
     "CreateNodeInputRequestTypeDef",
-    "GetNodeOutputTypeDef",
 )
 
 AccessorSummaryTypeDef = TypedDict(
     "AccessorSummaryTypeDef",
     {
         "Id": str,
         "Type": Literal["BILLING_TOKEN"],
@@ -148,14 +160,24 @@
         "CreationDate": datetime,
         "Arn": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+ApprovalThresholdPolicyOutputTypeDef = TypedDict(
+    "ApprovalThresholdPolicyOutputTypeDef",
+    {
+        "ThresholdPercentage": int,
+        "ProposalDurationInHours": int,
+        "ThresholdComparator": ThresholdComparatorType,
+    },
+    total=False,
+)
+
 ApprovalThresholdPolicyTypeDef = TypedDict(
     "ApprovalThresholdPolicyTypeDef",
     {
         "ThresholdPercentage": int,
         "ProposalDurationInHours": int,
         "ThresholdComparator": ThresholdComparatorType,
     },
@@ -173,19 +195,21 @@
     "_OptionalCreateAccessorInputRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateAccessorInputRequestTypeDef(
     _RequiredCreateAccessorInputRequestTypeDef, _OptionalCreateAccessorInputRequestTypeDef
 ):
     pass
 
+
 CreateAccessorOutputTypeDef = TypedDict(
     "CreateAccessorOutputTypeDef",
     {
         "AccessorId": str,
         "BillingToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -250,19 +274,21 @@
     "_OptionalDeleteNodeInputRequestTypeDef",
     {
         "MemberId": str,
     },
     total=False,
 )
 
+
 class DeleteNodeInputRequestTypeDef(
     _RequiredDeleteNodeInputRequestTypeDef, _OptionalDeleteNodeInputRequestTypeDef
 ):
     pass
 
+
 GetAccessorInputRequestTypeDef = TypedDict(
     "GetAccessorInputRequestTypeDef",
     {
         "AccessorId": str,
     },
 )
 
@@ -292,19 +318,21 @@
     "_OptionalGetNodeInputRequestTypeDef",
     {
         "MemberId": str,
     },
     total=False,
 )
 
+
 class GetNodeInputRequestTypeDef(
     _RequiredGetNodeInputRequestTypeDef, _OptionalGetNodeInputRequestTypeDef
 ):
     pass
 
+
 GetProposalInputRequestTypeDef = TypedDict(
     "GetProposalInputRequestTypeDef",
     {
         "NetworkId": str,
         "ProposalId": str,
     },
 )
@@ -320,14 +348,21 @@
         "Status": NetworkStatusType,
         "CreationDate": datetime,
         "Arn": str,
     },
     total=False,
 )
 
+InviteActionOutputTypeDef = TypedDict(
+    "InviteActionOutputTypeDef",
+    {
+        "Principal": str,
+    },
+)
+
 InviteActionTypeDef = TypedDict(
     "InviteActionTypeDef",
     {
         "Principal": str,
     },
 )
 
@@ -371,19 +406,21 @@
         "IsOwned": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListMembersInputRequestTypeDef(
     _RequiredListMembersInputRequestTypeDef, _OptionalListMembersInputRequestTypeDef
 ):
     pass
 
+
 MemberSummaryTypeDef = TypedDict(
     "MemberSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
         "Status": MemberStatusType,
@@ -419,19 +456,21 @@
         "Status": NodeStatusType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListNodesInputRequestTypeDef(
     _RequiredListNodesInputRequestTypeDef, _OptionalListNodesInputRequestTypeDef
 ):
     pass
 
+
 NodeSummaryTypeDef = TypedDict(
     "NodeSummaryTypeDef",
     {
         "Id": str,
         "Status": NodeStatusType,
         "CreationDate": datetime,
         "AvailabilityZone": str,
@@ -453,19 +492,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListProposalVotesInputRequestTypeDef(
     _RequiredListProposalVotesInputRequestTypeDef, _OptionalListProposalVotesInputRequestTypeDef
 ):
     pass
 
+
 VoteSummaryTypeDef = TypedDict(
     "VoteSummaryTypeDef",
     {
         "Vote": VoteValueType,
         "MemberName": str,
         "MemberId": str,
     },
@@ -483,19 +524,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListProposalsInputRequestTypeDef(
     _RequiredListProposalsInputRequestTypeDef, _OptionalListProposalsInputRequestTypeDef
 ):
     pass
 
+
 ProposalSummaryTypeDef = TypedDict(
     "ProposalSummaryTypeDef",
     {
         "ProposalId": str,
         "Description": str,
         "ProposedByMemberId": str,
         "ProposedByMemberName": str,
@@ -518,14 +561,22 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LogConfigurationOutputTypeDef = TypedDict(
+    "LogConfigurationOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 LogConfigurationTypeDef = TypedDict(
     "LogConfigurationTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -595,14 +646,21 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+RemoveActionOutputTypeDef = TypedDict(
+    "RemoveActionOutputTypeDef",
+    {
+        "MemberId": str,
+    },
+)
+
 RemoveActionTypeDef = TypedDict(
     "RemoveActionTypeDef",
     {
         "MemberId": str,
     },
 )
 
@@ -663,14 +721,22 @@
     "GetAccessorOutputTypeDef",
     {
         "Accessor": AccessorTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+VotingPolicyOutputTypeDef = TypedDict(
+    "VotingPolicyOutputTypeDef",
+    {
+        "ApprovalThresholdPolicy": ApprovalThresholdPolicyOutputTypeDef,
+    },
+    total=False,
+)
+
 VotingPolicyTypeDef = TypedDict(
     "VotingPolicyTypeDef",
     {
         "ApprovalThresholdPolicy": ApprovalThresholdPolicyTypeDef,
     },
     total=False,
 )
@@ -729,14 +795,22 @@
     {
         "Proposals": List[ProposalSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LogConfigurationsOutputTypeDef = TypedDict(
+    "LogConfigurationsOutputTypeDef",
+    {
+        "Cloudwatch": LogConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 LogConfigurationsTypeDef = TypedDict(
     "LogConfigurationsTypeDef",
     {
         "Cloudwatch": LogConfigurationTypeDef,
     },
     total=False,
 )
@@ -779,14 +853,23 @@
     {
         "Fabric": NodeFabricAttributesTypeDef,
         "Ethereum": NodeEthereumAttributesTypeDef,
     },
     total=False,
 )
 
+ProposalActionsOutputTypeDef = TypedDict(
+    "ProposalActionsOutputTypeDef",
+    {
+        "Invitations": List[InviteActionOutputTypeDef],
+        "Removals": List[RemoveActionOutputTypeDef],
+    },
+    total=False,
+)
+
 ProposalActionsTypeDef = TypedDict(
     "ProposalActionsTypeDef",
     {
         "Invitations": Sequence[InviteActionTypeDef],
         "Removals": Sequence[RemoveActionTypeDef],
     },
     total=False,
@@ -797,14 +880,31 @@
     {
         "Invitations": List[InvitationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+MemberFabricLogPublishingConfigurationOutputTypeDef = TypedDict(
+    "MemberFabricLogPublishingConfigurationOutputTypeDef",
+    {
+        "CaLogs": LogConfigurationsOutputTypeDef,
+    },
+    total=False,
+)
+
+NodeFabricLogPublishingConfigurationOutputTypeDef = TypedDict(
+    "NodeFabricLogPublishingConfigurationOutputTypeDef",
+    {
+        "ChaincodeLogs": LogConfigurationsOutputTypeDef,
+        "PeerLogs": LogConfigurationsOutputTypeDef,
+    },
+    total=False,
+)
+
 MemberFabricLogPublishingConfigurationTypeDef = TypedDict(
     "MemberFabricLogPublishingConfigurationTypeDef",
     {
         "CaLogs": LogConfigurationsTypeDef,
     },
     total=False,
 )
@@ -824,23 +924,44 @@
         "Id": str,
         "Name": str,
         "Description": str,
         "Framework": FrameworkType,
         "FrameworkVersion": str,
         "FrameworkAttributes": NetworkFrameworkAttributesTypeDef,
         "VpcEndpointServiceName": str,
-        "VotingPolicy": VotingPolicyTypeDef,
+        "VotingPolicy": VotingPolicyOutputTypeDef,
         "Status": NetworkStatusType,
         "CreationDate": datetime,
         "Tags": Dict[str, str],
         "Arn": str,
     },
     total=False,
 )
 
+ProposalTypeDef = TypedDict(
+    "ProposalTypeDef",
+    {
+        "ProposalId": str,
+        "NetworkId": str,
+        "Description": str,
+        "Actions": ProposalActionsOutputTypeDef,
+        "ProposedByMemberId": str,
+        "ProposedByMemberName": str,
+        "Status": ProposalStatusType,
+        "CreationDate": datetime,
+        "ExpirationDate": datetime,
+        "YesVoteCount": int,
+        "NoVoteCount": int,
+        "OutstandingVoteCount": int,
+        "Tags": Dict[str, str],
+        "Arn": str,
+    },
+    total=False,
+)
+
 _RequiredCreateProposalInputRequestTypeDef = TypedDict(
     "_RequiredCreateProposalInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "NetworkId": str,
         "MemberId": str,
         "Actions": ProposalActionsTypeDef,
@@ -851,36 +972,33 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateProposalInputRequestTypeDef(
     _RequiredCreateProposalInputRequestTypeDef, _OptionalCreateProposalInputRequestTypeDef
 ):
     pass
 
-ProposalTypeDef = TypedDict(
-    "ProposalTypeDef",
+
+MemberLogPublishingConfigurationOutputTypeDef = TypedDict(
+    "MemberLogPublishingConfigurationOutputTypeDef",
     {
-        "ProposalId": str,
-        "NetworkId": str,
-        "Description": str,
-        "Actions": ProposalActionsTypeDef,
-        "ProposedByMemberId": str,
-        "ProposedByMemberName": str,
-        "Status": ProposalStatusType,
-        "CreationDate": datetime,
-        "ExpirationDate": datetime,
-        "YesVoteCount": int,
-        "NoVoteCount": int,
-        "OutstandingVoteCount": int,
-        "Tags": Dict[str, str],
-        "Arn": str,
+        "Fabric": MemberFabricLogPublishingConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+NodeLogPublishingConfigurationOutputTypeDef = TypedDict(
+    "NodeLogPublishingConfigurationOutputTypeDef",
+    {
+        "Fabric": NodeFabricLogPublishingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 MemberLogPublishingConfigurationTypeDef = TypedDict(
     "MemberLogPublishingConfigurationTypeDef",
     {
@@ -909,14 +1027,52 @@
     "GetProposalOutputTypeDef",
     {
         "Proposal": ProposalTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+MemberTypeDef = TypedDict(
+    "MemberTypeDef",
+    {
+        "NetworkId": str,
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "FrameworkAttributes": MemberFrameworkAttributesTypeDef,
+        "LogPublishingConfiguration": MemberLogPublishingConfigurationOutputTypeDef,
+        "Status": MemberStatusType,
+        "CreationDate": datetime,
+        "Tags": Dict[str, str],
+        "Arn": str,
+        "KmsKeyArn": str,
+    },
+    total=False,
+)
+
+NodeTypeDef = TypedDict(
+    "NodeTypeDef",
+    {
+        "NetworkId": str,
+        "MemberId": str,
+        "Id": str,
+        "InstanceType": str,
+        "AvailabilityZone": str,
+        "FrameworkAttributes": NodeFrameworkAttributesTypeDef,
+        "LogPublishingConfiguration": NodeLogPublishingConfigurationOutputTypeDef,
+        "StateDB": StateDBTypeType,
+        "Status": NodeStatusType,
+        "CreationDate": datetime,
+        "Tags": Dict[str, str],
+        "Arn": str,
+        "KmsKeyArn": str,
+    },
+    total=False,
+)
+
 _RequiredMemberConfigurationTypeDef = TypedDict(
     "_RequiredMemberConfigurationTypeDef",
     {
         "Name": str,
         "FrameworkConfiguration": MemberFrameworkConfigurationTypeDef,
     },
 )
@@ -927,36 +1083,20 @@
         "LogPublishingConfiguration": MemberLogPublishingConfigurationTypeDef,
         "Tags": Mapping[str, str],
         "KmsKeyArn": str,
     },
     total=False,
 )
 
+
 class MemberConfigurationTypeDef(
     _RequiredMemberConfigurationTypeDef, _OptionalMemberConfigurationTypeDef
 ):
     pass
 
-MemberTypeDef = TypedDict(
-    "MemberTypeDef",
-    {
-        "NetworkId": str,
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "FrameworkAttributes": MemberFrameworkAttributesTypeDef,
-        "LogPublishingConfiguration": MemberLogPublishingConfigurationTypeDef,
-        "Status": MemberStatusType,
-        "CreationDate": datetime,
-        "Tags": Dict[str, str],
-        "Arn": str,
-        "KmsKeyArn": str,
-    },
-    total=False,
-)
 
 _RequiredUpdateMemberInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMemberInputRequestTypeDef",
     {
         "NetworkId": str,
         "MemberId": str,
     },
@@ -965,19 +1105,21 @@
     "_OptionalUpdateMemberInputRequestTypeDef",
     {
         "LogPublishingConfiguration": MemberLogPublishingConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateMemberInputRequestTypeDef(
     _RequiredUpdateMemberInputRequestTypeDef, _OptionalUpdateMemberInputRequestTypeDef
 ):
     pass
 
+
 _RequiredNodeConfigurationTypeDef = TypedDict(
     "_RequiredNodeConfigurationTypeDef",
     {
         "InstanceType": str,
     },
 )
 _OptionalNodeConfigurationTypeDef = TypedDict(
@@ -986,38 +1128,20 @@
         "AvailabilityZone": str,
         "LogPublishingConfiguration": NodeLogPublishingConfigurationTypeDef,
         "StateDB": StateDBTypeType,
     },
     total=False,
 )
 
+
 class NodeConfigurationTypeDef(
     _RequiredNodeConfigurationTypeDef, _OptionalNodeConfigurationTypeDef
 ):
     pass
 
-NodeTypeDef = TypedDict(
-    "NodeTypeDef",
-    {
-        "NetworkId": str,
-        "MemberId": str,
-        "Id": str,
-        "InstanceType": str,
-        "AvailabilityZone": str,
-        "FrameworkAttributes": NodeFrameworkAttributesTypeDef,
-        "LogPublishingConfiguration": NodeLogPublishingConfigurationTypeDef,
-        "StateDB": StateDBTypeType,
-        "Status": NodeStatusType,
-        "CreationDate": datetime,
-        "Tags": Dict[str, str],
-        "Arn": str,
-        "KmsKeyArn": str,
-    },
-    total=False,
-)
 
 _RequiredUpdateNodeInputRequestTypeDef = TypedDict(
     "_RequiredUpdateNodeInputRequestTypeDef",
     {
         "NetworkId": str,
         "NodeId": str,
     },
@@ -1027,19 +1151,37 @@
     {
         "MemberId": str,
         "LogPublishingConfiguration": NodeLogPublishingConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateNodeInputRequestTypeDef(
     _RequiredUpdateNodeInputRequestTypeDef, _OptionalUpdateNodeInputRequestTypeDef
 ):
     pass
 
+
+GetMemberOutputTypeDef = TypedDict(
+    "GetMemberOutputTypeDef",
+    {
+        "Member": MemberTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetNodeOutputTypeDef = TypedDict(
+    "GetNodeOutputTypeDef",
+    {
+        "Node": NodeTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateMemberInputRequestTypeDef = TypedDict(
     "CreateMemberInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "InvitationId": str,
         "NetworkId": str,
         "MemberConfiguration": MemberConfigurationTypeDef,
@@ -1063,26 +1205,20 @@
         "Description": str,
         "FrameworkConfiguration": NetworkFrameworkConfigurationTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateNetworkInputRequestTypeDef(
     _RequiredCreateNetworkInputRequestTypeDef, _OptionalCreateNetworkInputRequestTypeDef
 ):
     pass
 
-GetMemberOutputTypeDef = TypedDict(
-    "GetMemberOutputTypeDef",
-    {
-        "Member": MemberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreateNodeInputRequestTypeDef = TypedDict(
     "_RequiredCreateNodeInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "NetworkId": str,
         "NodeConfiguration": NodeConfigurationTypeDef,
@@ -1093,19 +1229,12 @@
     {
         "MemberId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateNodeInputRequestTypeDef(
     _RequiredCreateNodeInputRequestTypeDef, _OptionalCreateNodeInputRequestTypeDef
 ):
     pass
-
-GetNodeOutputTypeDef = TypedDict(
-    "GetNodeOutputTypeDef",
-    {
-        "Node": NodeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain.egg-info/PKG-INFO` & `mypy-boto3-managedblockchain-1.28.12/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-managedblockchain
-Version: 1.28.0
-Summary: Type annotations for boto3.ManagedBlockchain 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 managedblockchain type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-managedblockchain"></a>
 
 # mypy-boto3-managedblockchain
 
 [![PyPI - mypy-boto3-managedblockchain](https://img.shields.io/pypi/v/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-managedblockchain?color=blue)](https://pypistats.org/packages/mypy-boto3-managedblockchain)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-managedblockchain)](https://pepy.tech/project/mypy-boto3-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchain 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[boto3.ManagedBlockchain 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
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
 [mypy-boto3-managedblockchain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,14 +302,15 @@
 `mypy_boto3_managedblockchain.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_managedblockchain.type_defs import (
     AccessorSummaryTypeDef,
     AccessorTypeDef,
+    ApprovalThresholdPolicyOutputTypeDef,
     ApprovalThresholdPolicyTypeDef,
     CreateAccessorInputRequestTypeDef,
     CreateAccessorOutputTypeDef,
     CreateMemberOutputTypeDef,
     CreateNetworkOutputTypeDef,
     CreateNodeOutputTypeDef,
     CreateProposalOutputTypeDef,
@@ -350,14 +319,15 @@
     DeleteNodeInputRequestTypeDef,
     GetAccessorInputRequestTypeDef,
     GetMemberInputRequestTypeDef,
     GetNetworkInputRequestTypeDef,
     GetNodeInputRequestTypeDef,
     GetProposalInputRequestTypeDef,
     NetworkSummaryTypeDef,
+    InviteActionOutputTypeDef,
     InviteActionTypeDef,
     ListAccessorsInputListAccessorsPaginateTypeDef,
     ListAccessorsInputRequestTypeDef,
     ListInvitationsInputRequestTypeDef,
     ListMembersInputRequestTypeDef,
     MemberSummaryTypeDef,
     ListNetworksInputRequestTypeDef,
@@ -365,66 +335,75 @@
     NodeSummaryTypeDef,
     ListProposalVotesInputRequestTypeDef,
     VoteSummaryTypeDef,
     ListProposalsInputRequestTypeDef,
     ProposalSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
+    LogConfigurationOutputTypeDef,
     LogConfigurationTypeDef,
     MemberFabricAttributesTypeDef,
     MemberFabricConfigurationTypeDef,
     NetworkEthereumAttributesTypeDef,
     NetworkFabricAttributesTypeDef,
     NetworkFabricConfigurationTypeDef,
     NodeEthereumAttributesTypeDef,
     NodeFabricAttributesTypeDef,
     PaginatorConfigTypeDef,
+    RemoveActionOutputTypeDef,
     RemoveActionTypeDef,
     RejectInvitationInputRequestTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     VoteOnProposalInputRequestTypeDef,
     ListAccessorsOutputTypeDef,
     GetAccessorOutputTypeDef,
+    VotingPolicyOutputTypeDef,
     VotingPolicyTypeDef,
     InvitationTypeDef,
     ListNetworksOutputTypeDef,
     ListMembersOutputTypeDef,
     ListNodesOutputTypeDef,
     ListProposalVotesOutputTypeDef,
     ListProposalsOutputTypeDef,
+    LogConfigurationsOutputTypeDef,
     LogConfigurationsTypeDef,
     MemberFrameworkAttributesTypeDef,
     MemberFrameworkConfigurationTypeDef,
     NetworkFrameworkAttributesTypeDef,
     NetworkFrameworkConfigurationTypeDef,
     NodeFrameworkAttributesTypeDef,
+    ProposalActionsOutputTypeDef,
     ProposalActionsTypeDef,
     ListInvitationsOutputTypeDef,
+    MemberFabricLogPublishingConfigurationOutputTypeDef,
+    NodeFabricLogPublishingConfigurationOutputTypeDef,
     MemberFabricLogPublishingConfigurationTypeDef,
     NodeFabricLogPublishingConfigurationTypeDef,
     NetworkTypeDef,
-    CreateProposalInputRequestTypeDef,
     ProposalTypeDef,
+    CreateProposalInputRequestTypeDef,
+    MemberLogPublishingConfigurationOutputTypeDef,
+    NodeLogPublishingConfigurationOutputTypeDef,
     MemberLogPublishingConfigurationTypeDef,
     NodeLogPublishingConfigurationTypeDef,
     GetNetworkOutputTypeDef,
     GetProposalOutputTypeDef,
-    MemberConfigurationTypeDef,
     MemberTypeDef,
+    NodeTypeDef,
+    MemberConfigurationTypeDef,
     UpdateMemberInputRequestTypeDef,
     NodeConfigurationTypeDef,
-    NodeTypeDef,
     UpdateNodeInputRequestTypeDef,
+    GetMemberOutputTypeDef,
+    GetNodeOutputTypeDef,
     CreateMemberInputRequestTypeDef,
     CreateNetworkInputRequestTypeDef,
-    GetMemberOutputTypeDef,
     CreateNodeInputRequestTypeDef,
-    GetNodeOutputTypeDef,
 )
 
 
 def get_structure() -> AccessorSummaryTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-managedblockchain-1.28.0/mypy_boto3_managedblockchain.egg-info/SOURCES.txt` & `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.0/setup.py` & `mypy-boto3-managedblockchain-1.28.12/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-managedblockchain",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_managedblockchain"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ManagedBlockchain 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ManagedBlockchain 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

