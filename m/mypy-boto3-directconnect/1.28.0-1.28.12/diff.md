# Comparing `tmp/mypy-boto3-directconnect-1.28.0.tar.gz` & `tmp/mypy-boto3-directconnect-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-directconnect-1.28.0.tar", last modified: Thu Jul  6 20:59:24 2023, max compression
+gzip compressed data, was "mypy-boto3-directconnect-1.28.12.tar", last modified: Thu Jul 27 05:34:34 2023, max compression
```

## Comparing `mypy-boto3-directconnect-1.28.0.tar` & `mypy-boto3-directconnect-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:24.446278 mypy-boto3-directconnect-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:37:50.000000 mypy-boto3-directconnect-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20279 2023-07-06 20:59:24.442278 mypy-boto3-directconnect-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18770 2023-07-06 20:37:50.000000 mypy-boto3-directconnect-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:24.434278 mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-06 20:37:50.000000 mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-06 20:37:50.000000 mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-06 20:37:50.000000 mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47262 2023-07-06 20:37:50.000000 mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47189 2023-07-06 20:37:50.000000 mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-07-06 20:37:51.000000 mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10818 2023-07-06 20:37:50.000000 mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-06 20:37:50.000000 mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-06 20:37:50.000000 mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:37:50.000000 mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55029 2023-07-06 20:37:53.000000 mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    54982 2023-07-06 20:37:53.000000 mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:37:50.000000 mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:24.442278 mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20279 2023-07-06 20:59:24.000000 mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-06 20:59:24.000000 mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:24.000000 mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:24.000000 mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:24.000000 mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 20:59:24.000000 mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:24.446278 mypy-boto3-directconnect-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-06 20:37:50.000000 mypy-boto3-directconnect-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:34.556533 mypy-boto3-directconnect-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20324 2023-07-27 05:34:34.556533 mypy-boto3-directconnect-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:34.544533 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47262 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47189 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    55635 2023-07-27 05:20:15.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55586 2023-07-27 05:20:15.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:34.556533 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20324 2023-07-27 05:34:34.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 05:34:34.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:34.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:34.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:34.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 05:34:34.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:34.556533 mypy-boto3-directconnect-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/setup.py
```

### Comparing `mypy-boto3-directconnect-1.28.0/LICENSE` & `mypy-boto3-directconnect-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.28.0/PKG-INFO` & `mypy-boto3-directconnect-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-directconnect
-Version: 1.28.0
-Summary: Type annotations for boto3.DirectConnect 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.DirectConnect 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-directconnect"></a>
 
 # mypy-boto3-directconnect
 
 [![PyPI - mypy-boto3-directconnect](https://img.shields.io/pypi/v/mypy-boto3-directconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-directconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-directconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-directconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-directconnect?color=blue)](https://pypistats.org/packages/mypy-boto3-directconnect)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-directconnect)](https://pepy.tech/project/mypy-boto3-directconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DirectConnect 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
+[boto3.DirectConnect 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
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
 [mypy-boto3-directconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -369,14 +369,15 @@
     ConfirmCustomerAgreementResponseTypeDef,
     ConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
     ConfirmPrivateVirtualInterfaceResponseTypeDef,
     ConfirmPublicVirtualInterfaceRequestRequestTypeDef,
     ConfirmPublicVirtualInterfaceResponseTypeDef,
     ConfirmTransitVirtualInterfaceRequestRequestTypeDef,
     ConfirmTransitVirtualInterfaceResponseTypeDef,
+    TagOutputTypeDef,
     NewBGPPeerTypeDef,
     CreateDirectConnectGatewayRequestRequestTypeDef,
     DirectConnectGatewayTypeDef,
     CustomerAgreementTypeDef,
     DeleteBGPPeerRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
@@ -404,14 +405,15 @@
     DescribeInterconnectsRequestRequestTypeDef,
     DescribeLagsRequestRequestTypeDef,
     DescribeLoaRequestRequestTypeDef,
     DescribeRouterConfigurationRequestRequestTypeDef,
     RouterTypeTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DescribeVirtualInterfacesRequestRequestTypeDef,
+    RouteFilterPrefixOutputTypeDef,
     DisassociateConnectionFromLagRequestRequestTypeDef,
     DisassociateMacSecKeyRequestRequestTypeDef,
     ListVirtualInterfaceTestHistoryRequestRequestTypeDef,
     VirtualInterfaceTestHistoryTypeDef,
     LoaResponseMetadataTypeDef,
     LocationTypeDef,
     PaginatorConfigTypeDef,
@@ -428,58 +430,58 @@
     CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     CreateDirectConnectGatewayAssociationRequestRequestTypeDef,
     UpdateDirectConnectGatewayAssociationRequestRequestTypeDef,
     AllocateHostedConnectionRequestRequestTypeDef,
     CreateConnectionRequestRequestTypeDef,
     CreateInterconnectRequestRequestTypeDef,
     CreateLagRequestRequestTypeDef,
-    InterconnectResponseMetadataTypeDef,
-    InterconnectTypeDef,
     NewPrivateVirtualInterfaceAllocationTypeDef,
     NewPrivateVirtualInterfaceTypeDef,
     NewPublicVirtualInterfaceAllocationTypeDef,
     NewPublicVirtualInterfaceTypeDef,
     NewTransitVirtualInterfaceAllocationTypeDef,
     NewTransitVirtualInterfaceTypeDef,
-    ResourceTagTypeDef,
     TagResourceRequestRequestTypeDef,
     AssociateMacSecKeyResponseTypeDef,
+    DisassociateMacSecKeyResponseTypeDef,
     ConnectionResponseMetadataTypeDef,
     ConnectionTypeDef,
-    DisassociateMacSecKeyResponseTypeDef,
-    DirectConnectGatewayAssociationProposalTypeDef,
-    DirectConnectGatewayAssociationTypeDef,
-    VirtualInterfaceResponseMetadataTypeDef,
-    VirtualInterfaceTypeDef,
+    InterconnectResponseMetadataTypeDef,
+    InterconnectTypeDef,
+    ResourceTagTypeDef,
     CreateBGPPeerRequestRequestTypeDef,
     CreateDirectConnectGatewayResultTypeDef,
     DeleteDirectConnectGatewayResultTypeDef,
     DescribeDirectConnectGatewaysResultTypeDef,
     UpdateDirectConnectGatewayResponseTypeDef,
     DescribeCustomerMetadataResponseTypeDef,
     DescribeConnectionLoaResponseTypeDef,
     DescribeInterconnectLoaResponseTypeDef,
     DescribeDirectConnectGatewayAttachmentsResultTypeDef,
     DescribeRouterConfigurationResponseTypeDef,
+    DirectConnectGatewayAssociationProposalTypeDef,
+    DirectConnectGatewayAssociationTypeDef,
+    VirtualInterfaceResponseMetadataTypeDef,
+    VirtualInterfaceTypeDef,
     ListVirtualInterfaceTestHistoryResponseTypeDef,
     StartBgpFailoverTestResponseTypeDef,
     StopBgpFailoverTestResponseTypeDef,
     LocationsTypeDef,
     VirtualGatewaysTypeDef,
-    InterconnectsTypeDef,
     AllocatePrivateVirtualInterfaceRequestRequestTypeDef,
     CreatePrivateVirtualInterfaceRequestRequestTypeDef,
     AllocatePublicVirtualInterfaceRequestRequestTypeDef,
     CreatePublicVirtualInterfaceRequestRequestTypeDef,
     AllocateTransitVirtualInterfaceRequestRequestTypeDef,
     CreateTransitVirtualInterfaceRequestRequestTypeDef,
-    DescribeTagsResponseTypeDef,
     ConnectionsTypeDef,
     LagResponseMetadataTypeDef,
     LagTypeDef,
+    InterconnectsTypeDef,
+    DescribeTagsResponseTypeDef,
     CreateDirectConnectGatewayAssociationProposalResultTypeDef,
     DeleteDirectConnectGatewayAssociationProposalResultTypeDef,
     DescribeDirectConnectGatewayAssociationProposalsResultTypeDef,
     AcceptDirectConnectGatewayAssociationProposalResultTypeDef,
     CreateDirectConnectGatewayAssociationResultTypeDef,
     DeleteDirectConnectGatewayAssociationResultTypeDef,
     DescribeDirectConnectGatewayAssociationsResultTypeDef,
```

### Comparing `mypy-boto3-directconnect-1.28.0/README.md` & `mypy-boto3-directconnect-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-directconnect"></a>
 
 # mypy-boto3-directconnect
 
 [![PyPI - mypy-boto3-directconnect](https://img.shields.io/pypi/v/mypy-boto3-directconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-directconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-directconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-directconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-directconnect?color=blue)](https://pypistats.org/packages/mypy-boto3-directconnect)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-directconnect)](https://pepy.tech/project/mypy-boto3-directconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DirectConnect 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
+[boto3.DirectConnect 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
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
 [mypy-boto3-directconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -337,14 +337,15 @@
     ConfirmCustomerAgreementResponseTypeDef,
     ConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
     ConfirmPrivateVirtualInterfaceResponseTypeDef,
     ConfirmPublicVirtualInterfaceRequestRequestTypeDef,
     ConfirmPublicVirtualInterfaceResponseTypeDef,
     ConfirmTransitVirtualInterfaceRequestRequestTypeDef,
     ConfirmTransitVirtualInterfaceResponseTypeDef,
+    TagOutputTypeDef,
     NewBGPPeerTypeDef,
     CreateDirectConnectGatewayRequestRequestTypeDef,
     DirectConnectGatewayTypeDef,
     CustomerAgreementTypeDef,
     DeleteBGPPeerRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
@@ -372,14 +373,15 @@
     DescribeInterconnectsRequestRequestTypeDef,
     DescribeLagsRequestRequestTypeDef,
     DescribeLoaRequestRequestTypeDef,
     DescribeRouterConfigurationRequestRequestTypeDef,
     RouterTypeTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DescribeVirtualInterfacesRequestRequestTypeDef,
+    RouteFilterPrefixOutputTypeDef,
     DisassociateConnectionFromLagRequestRequestTypeDef,
     DisassociateMacSecKeyRequestRequestTypeDef,
     ListVirtualInterfaceTestHistoryRequestRequestTypeDef,
     VirtualInterfaceTestHistoryTypeDef,
     LoaResponseMetadataTypeDef,
     LocationTypeDef,
     PaginatorConfigTypeDef,
@@ -396,58 +398,58 @@
     CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     CreateDirectConnectGatewayAssociationRequestRequestTypeDef,
     UpdateDirectConnectGatewayAssociationRequestRequestTypeDef,
     AllocateHostedConnectionRequestRequestTypeDef,
     CreateConnectionRequestRequestTypeDef,
     CreateInterconnectRequestRequestTypeDef,
     CreateLagRequestRequestTypeDef,
-    InterconnectResponseMetadataTypeDef,
-    InterconnectTypeDef,
     NewPrivateVirtualInterfaceAllocationTypeDef,
     NewPrivateVirtualInterfaceTypeDef,
     NewPublicVirtualInterfaceAllocationTypeDef,
     NewPublicVirtualInterfaceTypeDef,
     NewTransitVirtualInterfaceAllocationTypeDef,
     NewTransitVirtualInterfaceTypeDef,
-    ResourceTagTypeDef,
     TagResourceRequestRequestTypeDef,
     AssociateMacSecKeyResponseTypeDef,
+    DisassociateMacSecKeyResponseTypeDef,
     ConnectionResponseMetadataTypeDef,
     ConnectionTypeDef,
-    DisassociateMacSecKeyResponseTypeDef,
-    DirectConnectGatewayAssociationProposalTypeDef,
-    DirectConnectGatewayAssociationTypeDef,
-    VirtualInterfaceResponseMetadataTypeDef,
-    VirtualInterfaceTypeDef,
+    InterconnectResponseMetadataTypeDef,
+    InterconnectTypeDef,
+    ResourceTagTypeDef,
     CreateBGPPeerRequestRequestTypeDef,
     CreateDirectConnectGatewayResultTypeDef,
     DeleteDirectConnectGatewayResultTypeDef,
     DescribeDirectConnectGatewaysResultTypeDef,
     UpdateDirectConnectGatewayResponseTypeDef,
     DescribeCustomerMetadataResponseTypeDef,
     DescribeConnectionLoaResponseTypeDef,
     DescribeInterconnectLoaResponseTypeDef,
     DescribeDirectConnectGatewayAttachmentsResultTypeDef,
     DescribeRouterConfigurationResponseTypeDef,
+    DirectConnectGatewayAssociationProposalTypeDef,
+    DirectConnectGatewayAssociationTypeDef,
+    VirtualInterfaceResponseMetadataTypeDef,
+    VirtualInterfaceTypeDef,
     ListVirtualInterfaceTestHistoryResponseTypeDef,
     StartBgpFailoverTestResponseTypeDef,
     StopBgpFailoverTestResponseTypeDef,
     LocationsTypeDef,
     VirtualGatewaysTypeDef,
-    InterconnectsTypeDef,
     AllocatePrivateVirtualInterfaceRequestRequestTypeDef,
     CreatePrivateVirtualInterfaceRequestRequestTypeDef,
     AllocatePublicVirtualInterfaceRequestRequestTypeDef,
     CreatePublicVirtualInterfaceRequestRequestTypeDef,
     AllocateTransitVirtualInterfaceRequestRequestTypeDef,
     CreateTransitVirtualInterfaceRequestRequestTypeDef,
-    DescribeTagsResponseTypeDef,
     ConnectionsTypeDef,
     LagResponseMetadataTypeDef,
     LagTypeDef,
+    InterconnectsTypeDef,
+    DescribeTagsResponseTypeDef,
     CreateDirectConnectGatewayAssociationProposalResultTypeDef,
     DeleteDirectConnectGatewayAssociationProposalResultTypeDef,
     DescribeDirectConnectGatewayAssociationProposalsResultTypeDef,
     AcceptDirectConnectGatewayAssociationProposalResultTypeDef,
     CreateDirectConnectGatewayAssociationResultTypeDef,
     DeleteDirectConnectGatewayAssociationResultTypeDef,
     DescribeDirectConnectGatewayAssociationsResultTypeDef,
```

### Comparing `mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/__init__.py` & `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/__init__.pyi` & `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/__main__.py` & `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DirectConnect 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.DirectConnect 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect\nOther"
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

### Comparing `mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/client.py` & `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/client.pyi` & `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/literals.py` & `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,14 +214,15 @@
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
@@ -300,26 +301,28 @@
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

### Comparing `mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/literals.pyi` & `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/literals.pyi`

 * *Files 1% similar despite different names*

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

### Comparing `mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/paginator.py` & `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/paginator.pyi` & `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/type_defs.py` & `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     "ConfirmCustomerAgreementResponseTypeDef",
     "ConfirmPrivateVirtualInterfaceRequestRequestTypeDef",
     "ConfirmPrivateVirtualInterfaceResponseTypeDef",
     "ConfirmPublicVirtualInterfaceRequestRequestTypeDef",
     "ConfirmPublicVirtualInterfaceResponseTypeDef",
     "ConfirmTransitVirtualInterfaceRequestRequestTypeDef",
     "ConfirmTransitVirtualInterfaceResponseTypeDef",
+    "TagOutputTypeDef",
     "NewBGPPeerTypeDef",
     "CreateDirectConnectGatewayRequestRequestTypeDef",
     "DirectConnectGatewayTypeDef",
     "CustomerAgreementTypeDef",
     "DeleteBGPPeerRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
@@ -95,14 +96,15 @@
     "DescribeInterconnectsRequestRequestTypeDef",
     "DescribeLagsRequestRequestTypeDef",
     "DescribeLoaRequestRequestTypeDef",
     "DescribeRouterConfigurationRequestRequestTypeDef",
     "RouterTypeTypeDef",
     "DescribeTagsRequestRequestTypeDef",
     "DescribeVirtualInterfacesRequestRequestTypeDef",
+    "RouteFilterPrefixOutputTypeDef",
     "DisassociateConnectionFromLagRequestRequestTypeDef",
     "DisassociateMacSecKeyRequestRequestTypeDef",
     "ListVirtualInterfaceTestHistoryRequestRequestTypeDef",
     "VirtualInterfaceTestHistoryTypeDef",
     "LoaResponseMetadataTypeDef",
     "LocationTypeDef",
     "PaginatorConfigTypeDef",
@@ -119,58 +121,58 @@
     "CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     "CreateDirectConnectGatewayAssociationRequestRequestTypeDef",
     "UpdateDirectConnectGatewayAssociationRequestRequestTypeDef",
     "AllocateHostedConnectionRequestRequestTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "CreateInterconnectRequestRequestTypeDef",
     "CreateLagRequestRequestTypeDef",
-    "InterconnectResponseMetadataTypeDef",
-    "InterconnectTypeDef",
     "NewPrivateVirtualInterfaceAllocationTypeDef",
     "NewPrivateVirtualInterfaceTypeDef",
     "NewPublicVirtualInterfaceAllocationTypeDef",
     "NewPublicVirtualInterfaceTypeDef",
     "NewTransitVirtualInterfaceAllocationTypeDef",
     "NewTransitVirtualInterfaceTypeDef",
-    "ResourceTagTypeDef",
     "TagResourceRequestRequestTypeDef",
     "AssociateMacSecKeyResponseTypeDef",
+    "DisassociateMacSecKeyResponseTypeDef",
     "ConnectionResponseMetadataTypeDef",
     "ConnectionTypeDef",
-    "DisassociateMacSecKeyResponseTypeDef",
-    "DirectConnectGatewayAssociationProposalTypeDef",
-    "DirectConnectGatewayAssociationTypeDef",
-    "VirtualInterfaceResponseMetadataTypeDef",
-    "VirtualInterfaceTypeDef",
+    "InterconnectResponseMetadataTypeDef",
+    "InterconnectTypeDef",
+    "ResourceTagTypeDef",
     "CreateBGPPeerRequestRequestTypeDef",
     "CreateDirectConnectGatewayResultTypeDef",
     "DeleteDirectConnectGatewayResultTypeDef",
     "DescribeDirectConnectGatewaysResultTypeDef",
     "UpdateDirectConnectGatewayResponseTypeDef",
     "DescribeCustomerMetadataResponseTypeDef",
     "DescribeConnectionLoaResponseTypeDef",
     "DescribeInterconnectLoaResponseTypeDef",
     "DescribeDirectConnectGatewayAttachmentsResultTypeDef",
     "DescribeRouterConfigurationResponseTypeDef",
+    "DirectConnectGatewayAssociationProposalTypeDef",
+    "DirectConnectGatewayAssociationTypeDef",
+    "VirtualInterfaceResponseMetadataTypeDef",
+    "VirtualInterfaceTypeDef",
     "ListVirtualInterfaceTestHistoryResponseTypeDef",
     "StartBgpFailoverTestResponseTypeDef",
     "StopBgpFailoverTestResponseTypeDef",
     "LocationsTypeDef",
     "VirtualGatewaysTypeDef",
-    "InterconnectsTypeDef",
     "AllocatePrivateVirtualInterfaceRequestRequestTypeDef",
     "CreatePrivateVirtualInterfaceRequestRequestTypeDef",
     "AllocatePublicVirtualInterfaceRequestRequestTypeDef",
     "CreatePublicVirtualInterfaceRequestRequestTypeDef",
     "AllocateTransitVirtualInterfaceRequestRequestTypeDef",
     "CreateTransitVirtualInterfaceRequestRequestTypeDef",
-    "DescribeTagsResponseTypeDef",
     "ConnectionsTypeDef",
     "LagResponseMetadataTypeDef",
     "LagTypeDef",
+    "InterconnectsTypeDef",
+    "DescribeTagsResponseTypeDef",
     "CreateDirectConnectGatewayAssociationProposalResultTypeDef",
     "DeleteDirectConnectGatewayAssociationProposalResultTypeDef",
     "DescribeDirectConnectGatewayAssociationProposalsResultTypeDef",
     "AcceptDirectConnectGatewayAssociationProposalResultTypeDef",
     "CreateDirectConnectGatewayAssociationResultTypeDef",
     "DeleteDirectConnectGatewayAssociationResultTypeDef",
     "DescribeDirectConnectGatewayAssociationsResultTypeDef",
@@ -397,14 +399,33 @@
     "ConfirmTransitVirtualInterfaceResponseTypeDef",
     {
         "virtualInterfaceState": VirtualInterfaceStateType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
+    {
+        "key": str,
+    },
+)
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
+    {
+        "value": str,
+    },
+    total=False,
+)
+
+
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
+    pass
+
+
 NewBGPPeerTypeDef = TypedDict(
     "NewBGPPeerTypeDef",
     {
         "asn": int,
         "authKey": str,
         "addressFamily": AddressFamilyType,
         "amazonAddress": str,
@@ -789,14 +810,22 @@
     {
         "connectionId": str,
         "virtualInterfaceId": str,
     },
     total=False,
 )
 
+RouteFilterPrefixOutputTypeDef = TypedDict(
+    "RouteFilterPrefixOutputTypeDef",
+    {
+        "cidr": str,
+    },
+    total=False,
+)
+
 DisassociateConnectionFromLagRequestRequestTypeDef = TypedDict(
     "DisassociateConnectionFromLagRequestRequestTypeDef",
     {
         "connectionId": str,
         "lagId": str,
     },
 )
@@ -1189,58 +1218,14 @@
 
 class CreateLagRequestRequestTypeDef(
     _RequiredCreateLagRequestRequestTypeDef, _OptionalCreateLagRequestRequestTypeDef
 ):
     pass
 
 
-InterconnectResponseMetadataTypeDef = TypedDict(
-    "InterconnectResponseMetadataTypeDef",
-    {
-        "interconnectId": str,
-        "interconnectName": str,
-        "interconnectState": InterconnectStateType,
-        "region": str,
-        "location": str,
-        "bandwidth": str,
-        "loaIssueTime": datetime,
-        "lagId": str,
-        "awsDevice": str,
-        "jumboFrameCapable": bool,
-        "awsDeviceV2": str,
-        "awsLogicalDeviceId": str,
-        "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagTypeDef],
-        "providerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-InterconnectTypeDef = TypedDict(
-    "InterconnectTypeDef",
-    {
-        "interconnectId": str,
-        "interconnectName": str,
-        "interconnectState": InterconnectStateType,
-        "region": str,
-        "location": str,
-        "bandwidth": str,
-        "loaIssueTime": datetime,
-        "lagId": str,
-        "awsDevice": str,
-        "jumboFrameCapable": bool,
-        "awsDeviceV2": str,
-        "awsLogicalDeviceId": str,
-        "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagTypeDef],
-        "providerName": str,
-    },
-    total=False,
-)
-
 _RequiredNewPrivateVirtualInterfaceAllocationTypeDef = TypedDict(
     "_RequiredNewPrivateVirtualInterfaceAllocationTypeDef",
     {
         "virtualInterfaceName": str,
         "vlan": int,
         "asn": int,
     },
@@ -1384,23 +1369,14 @@
         "directConnectGatewayId": str,
         "tags": Sequence[TagTypeDef],
         "enableSiteLink": bool,
     },
     total=False,
 )
 
-ResourceTagTypeDef = TypedDict(
-    "ResourceTagTypeDef",
-    {
-        "resourceArn": str,
-        "tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1410,14 +1386,23 @@
     {
         "connectionId": str,
         "macSecKeys": List[MacSecKeyTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DisassociateMacSecKeyResponseTypeDef = TypedDict(
+    "DisassociateMacSecKeyResponseTypeDef",
+    {
+        "connectionId": str,
+        "macSecKeys": List[MacSecKeyTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ConnectionResponseMetadataTypeDef = TypedDict(
     "ConnectionResponseMetadataTypeDef",
     {
         "ownerAccount": str,
         "connectionId": str,
         "connectionName": str,
         "connectionState": ConnectionStateType,
@@ -1429,15 +1414,15 @@
         "loaIssueTime": datetime,
         "lagId": str,
         "awsDevice": str,
         "jumboFrameCapable": bool,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "portEncryptionStatus": str,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1458,126 +1443,73 @@
         "loaIssueTime": datetime,
         "lagId": str,
         "awsDevice": str,
         "jumboFrameCapable": bool,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "portEncryptionStatus": str,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
     },
     total=False,
 )
 
-DisassociateMacSecKeyResponseTypeDef = TypedDict(
-    "DisassociateMacSecKeyResponseTypeDef",
-    {
-        "connectionId": str,
-        "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DirectConnectGatewayAssociationProposalTypeDef = TypedDict(
-    "DirectConnectGatewayAssociationProposalTypeDef",
-    {
-        "proposalId": str,
-        "directConnectGatewayId": str,
-        "directConnectGatewayOwnerAccount": str,
-        "proposalState": DirectConnectGatewayAssociationProposalStateType,
-        "associatedGateway": AssociatedGatewayTypeDef,
-        "existingAllowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixTypeDef],
-        "requestedAllowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixTypeDef],
-    },
-    total=False,
-)
-
-DirectConnectGatewayAssociationTypeDef = TypedDict(
-    "DirectConnectGatewayAssociationTypeDef",
-    {
-        "directConnectGatewayId": str,
-        "directConnectGatewayOwnerAccount": str,
-        "associationState": DirectConnectGatewayAssociationStateType,
-        "stateChangeError": str,
-        "associatedGateway": AssociatedGatewayTypeDef,
-        "associationId": str,
-        "allowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixTypeDef],
-        "virtualGatewayId": str,
-        "virtualGatewayRegion": str,
-        "virtualGatewayOwnerAccount": str,
-    },
-    total=False,
-)
-
-VirtualInterfaceResponseMetadataTypeDef = TypedDict(
-    "VirtualInterfaceResponseMetadataTypeDef",
+InterconnectResponseMetadataTypeDef = TypedDict(
+    "InterconnectResponseMetadataTypeDef",
     {
-        "ownerAccount": str,
-        "virtualInterfaceId": str,
+        "interconnectId": str,
+        "interconnectName": str,
+        "interconnectState": InterconnectStateType,
+        "region": str,
         "location": str,
-        "connectionId": str,
-        "virtualInterfaceType": str,
-        "virtualInterfaceName": str,
-        "vlan": int,
-        "asn": int,
-        "amazonSideAsn": int,
-        "authKey": str,
-        "amazonAddress": str,
-        "customerAddress": str,
-        "addressFamily": AddressFamilyType,
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "customerRouterConfig": str,
-        "mtu": int,
+        "bandwidth": str,
+        "loaIssueTime": datetime,
+        "lagId": str,
+        "awsDevice": str,
         "jumboFrameCapable": bool,
-        "virtualGatewayId": str,
-        "directConnectGatewayId": str,
-        "routeFilterPrefixes": List[RouteFilterPrefixTypeDef],
-        "bgpPeers": List[BGPPeerTypeDef],
-        "region": str,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
-        "tags": List[TagTypeDef],
-        "siteLinkEnabled": bool,
+        "hasLogicalRedundancy": HasLogicalRedundancyType,
+        "tags": List[TagOutputTypeDef],
+        "providerName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-VirtualInterfaceTypeDef = TypedDict(
-    "VirtualInterfaceTypeDef",
+InterconnectTypeDef = TypedDict(
+    "InterconnectTypeDef",
     {
-        "ownerAccount": str,
-        "virtualInterfaceId": str,
+        "interconnectId": str,
+        "interconnectName": str,
+        "interconnectState": InterconnectStateType,
+        "region": str,
         "location": str,
-        "connectionId": str,
-        "virtualInterfaceType": str,
-        "virtualInterfaceName": str,
-        "vlan": int,
-        "asn": int,
-        "amazonSideAsn": int,
-        "authKey": str,
-        "amazonAddress": str,
-        "customerAddress": str,
-        "addressFamily": AddressFamilyType,
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "customerRouterConfig": str,
-        "mtu": int,
+        "bandwidth": str,
+        "loaIssueTime": datetime,
+        "lagId": str,
+        "awsDevice": str,
         "jumboFrameCapable": bool,
-        "virtualGatewayId": str,
-        "directConnectGatewayId": str,
-        "routeFilterPrefixes": List[RouteFilterPrefixTypeDef],
-        "bgpPeers": List[BGPPeerTypeDef],
-        "region": str,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
-        "tags": List[TagTypeDef],
-        "siteLinkEnabled": bool,
+        "hasLogicalRedundancy": HasLogicalRedundancyType,
+        "tags": List[TagOutputTypeDef],
+        "providerName": str,
+    },
+    total=False,
+)
+
+ResourceTagTypeDef = TypedDict(
+    "ResourceTagTypeDef",
+    {
+        "resourceArn": str,
+        "tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
 CreateBGPPeerRequestRequestTypeDef = TypedDict(
     "CreateBGPPeerRequestRequestTypeDef",
     {
@@ -1661,14 +1593,111 @@
         "router": RouterTypeTypeDef,
         "virtualInterfaceId": str,
         "virtualInterfaceName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DirectConnectGatewayAssociationProposalTypeDef = TypedDict(
+    "DirectConnectGatewayAssociationProposalTypeDef",
+    {
+        "proposalId": str,
+        "directConnectGatewayId": str,
+        "directConnectGatewayOwnerAccount": str,
+        "proposalState": DirectConnectGatewayAssociationProposalStateType,
+        "associatedGateway": AssociatedGatewayTypeDef,
+        "existingAllowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixOutputTypeDef],
+        "requestedAllowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixOutputTypeDef],
+    },
+    total=False,
+)
+
+DirectConnectGatewayAssociationTypeDef = TypedDict(
+    "DirectConnectGatewayAssociationTypeDef",
+    {
+        "directConnectGatewayId": str,
+        "directConnectGatewayOwnerAccount": str,
+        "associationState": DirectConnectGatewayAssociationStateType,
+        "stateChangeError": str,
+        "associatedGateway": AssociatedGatewayTypeDef,
+        "associationId": str,
+        "allowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixOutputTypeDef],
+        "virtualGatewayId": str,
+        "virtualGatewayRegion": str,
+        "virtualGatewayOwnerAccount": str,
+    },
+    total=False,
+)
+
+VirtualInterfaceResponseMetadataTypeDef = TypedDict(
+    "VirtualInterfaceResponseMetadataTypeDef",
+    {
+        "ownerAccount": str,
+        "virtualInterfaceId": str,
+        "location": str,
+        "connectionId": str,
+        "virtualInterfaceType": str,
+        "virtualInterfaceName": str,
+        "vlan": int,
+        "asn": int,
+        "amazonSideAsn": int,
+        "authKey": str,
+        "amazonAddress": str,
+        "customerAddress": str,
+        "addressFamily": AddressFamilyType,
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "customerRouterConfig": str,
+        "mtu": int,
+        "jumboFrameCapable": bool,
+        "virtualGatewayId": str,
+        "directConnectGatewayId": str,
+        "routeFilterPrefixes": List[RouteFilterPrefixOutputTypeDef],
+        "bgpPeers": List[BGPPeerTypeDef],
+        "region": str,
+        "awsDeviceV2": str,
+        "awsLogicalDeviceId": str,
+        "tags": List[TagOutputTypeDef],
+        "siteLinkEnabled": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+VirtualInterfaceTypeDef = TypedDict(
+    "VirtualInterfaceTypeDef",
+    {
+        "ownerAccount": str,
+        "virtualInterfaceId": str,
+        "location": str,
+        "connectionId": str,
+        "virtualInterfaceType": str,
+        "virtualInterfaceName": str,
+        "vlan": int,
+        "asn": int,
+        "amazonSideAsn": int,
+        "authKey": str,
+        "amazonAddress": str,
+        "customerAddress": str,
+        "addressFamily": AddressFamilyType,
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "customerRouterConfig": str,
+        "mtu": int,
+        "jumboFrameCapable": bool,
+        "virtualGatewayId": str,
+        "directConnectGatewayId": str,
+        "routeFilterPrefixes": List[RouteFilterPrefixOutputTypeDef],
+        "bgpPeers": List[BGPPeerTypeDef],
+        "region": str,
+        "awsDeviceV2": str,
+        "awsLogicalDeviceId": str,
+        "tags": List[TagOutputTypeDef],
+        "siteLinkEnabled": bool,
+    },
+    total=False,
+)
+
 ListVirtualInterfaceTestHistoryResponseTypeDef = TypedDict(
     "ListVirtualInterfaceTestHistoryResponseTypeDef",
     {
         "virtualInterfaceTestHistory": List[VirtualInterfaceTestHistoryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1702,22 +1731,14 @@
     "VirtualGatewaysTypeDef",
     {
         "virtualGateways": List[VirtualGatewayTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-InterconnectsTypeDef = TypedDict(
-    "InterconnectsTypeDef",
-    {
-        "interconnects": List[InterconnectTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AllocatePrivateVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "AllocatePrivateVirtualInterfaceRequestRequestTypeDef",
     {
         "connectionId": str,
         "ownerAccount": str,
         "newPrivateVirtualInterfaceAllocation": NewPrivateVirtualInterfaceAllocationTypeDef,
     },
@@ -1761,22 +1782,14 @@
     "CreateTransitVirtualInterfaceRequestRequestTypeDef",
     {
         "connectionId": str,
         "newTransitVirtualInterface": NewTransitVirtualInterfaceTypeDef,
     },
 )
 
-DescribeTagsResponseTypeDef = TypedDict(
-    "DescribeTagsResponseTypeDef",
-    {
-        "resourceTags": List[ResourceTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ConnectionsTypeDef = TypedDict(
     "ConnectionsTypeDef",
     {
         "connections": List[ConnectionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1796,15 +1809,15 @@
         "awsDevice": str,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "connections": List[ConnectionTypeDef],
         "allowsHostedConnections": bool,
         "jumboFrameCapable": bool,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1824,23 +1837,39 @@
         "awsDevice": str,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "connections": List[ConnectionTypeDef],
         "allowsHostedConnections": bool,
         "jumboFrameCapable": bool,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
     },
     total=False,
 )
 
+InterconnectsTypeDef = TypedDict(
+    "InterconnectsTypeDef",
+    {
+        "interconnects": List[InterconnectTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeTagsResponseTypeDef = TypedDict(
+    "DescribeTagsResponseTypeDef",
+    {
+        "resourceTags": List[ResourceTagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateDirectConnectGatewayAssociationProposalResultTypeDef = TypedDict(
     "CreateDirectConnectGatewayAssociationProposalResultTypeDef",
     {
         "directConnectGatewayAssociationProposal": DirectConnectGatewayAssociationProposalTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect/type_defs.pyi` & `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     "ConfirmCustomerAgreementResponseTypeDef",
     "ConfirmPrivateVirtualInterfaceRequestRequestTypeDef",
     "ConfirmPrivateVirtualInterfaceResponseTypeDef",
     "ConfirmPublicVirtualInterfaceRequestRequestTypeDef",
     "ConfirmPublicVirtualInterfaceResponseTypeDef",
     "ConfirmTransitVirtualInterfaceRequestRequestTypeDef",
     "ConfirmTransitVirtualInterfaceResponseTypeDef",
+    "TagOutputTypeDef",
     "NewBGPPeerTypeDef",
     "CreateDirectConnectGatewayRequestRequestTypeDef",
     "DirectConnectGatewayTypeDef",
     "CustomerAgreementTypeDef",
     "DeleteBGPPeerRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
@@ -94,14 +95,15 @@
     "DescribeInterconnectsRequestRequestTypeDef",
     "DescribeLagsRequestRequestTypeDef",
     "DescribeLoaRequestRequestTypeDef",
     "DescribeRouterConfigurationRequestRequestTypeDef",
     "RouterTypeTypeDef",
     "DescribeTagsRequestRequestTypeDef",
     "DescribeVirtualInterfacesRequestRequestTypeDef",
+    "RouteFilterPrefixOutputTypeDef",
     "DisassociateConnectionFromLagRequestRequestTypeDef",
     "DisassociateMacSecKeyRequestRequestTypeDef",
     "ListVirtualInterfaceTestHistoryRequestRequestTypeDef",
     "VirtualInterfaceTestHistoryTypeDef",
     "LoaResponseMetadataTypeDef",
     "LocationTypeDef",
     "PaginatorConfigTypeDef",
@@ -118,58 +120,58 @@
     "CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     "CreateDirectConnectGatewayAssociationRequestRequestTypeDef",
     "UpdateDirectConnectGatewayAssociationRequestRequestTypeDef",
     "AllocateHostedConnectionRequestRequestTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "CreateInterconnectRequestRequestTypeDef",
     "CreateLagRequestRequestTypeDef",
-    "InterconnectResponseMetadataTypeDef",
-    "InterconnectTypeDef",
     "NewPrivateVirtualInterfaceAllocationTypeDef",
     "NewPrivateVirtualInterfaceTypeDef",
     "NewPublicVirtualInterfaceAllocationTypeDef",
     "NewPublicVirtualInterfaceTypeDef",
     "NewTransitVirtualInterfaceAllocationTypeDef",
     "NewTransitVirtualInterfaceTypeDef",
-    "ResourceTagTypeDef",
     "TagResourceRequestRequestTypeDef",
     "AssociateMacSecKeyResponseTypeDef",
+    "DisassociateMacSecKeyResponseTypeDef",
     "ConnectionResponseMetadataTypeDef",
     "ConnectionTypeDef",
-    "DisassociateMacSecKeyResponseTypeDef",
-    "DirectConnectGatewayAssociationProposalTypeDef",
-    "DirectConnectGatewayAssociationTypeDef",
-    "VirtualInterfaceResponseMetadataTypeDef",
-    "VirtualInterfaceTypeDef",
+    "InterconnectResponseMetadataTypeDef",
+    "InterconnectTypeDef",
+    "ResourceTagTypeDef",
     "CreateBGPPeerRequestRequestTypeDef",
     "CreateDirectConnectGatewayResultTypeDef",
     "DeleteDirectConnectGatewayResultTypeDef",
     "DescribeDirectConnectGatewaysResultTypeDef",
     "UpdateDirectConnectGatewayResponseTypeDef",
     "DescribeCustomerMetadataResponseTypeDef",
     "DescribeConnectionLoaResponseTypeDef",
     "DescribeInterconnectLoaResponseTypeDef",
     "DescribeDirectConnectGatewayAttachmentsResultTypeDef",
     "DescribeRouterConfigurationResponseTypeDef",
+    "DirectConnectGatewayAssociationProposalTypeDef",
+    "DirectConnectGatewayAssociationTypeDef",
+    "VirtualInterfaceResponseMetadataTypeDef",
+    "VirtualInterfaceTypeDef",
     "ListVirtualInterfaceTestHistoryResponseTypeDef",
     "StartBgpFailoverTestResponseTypeDef",
     "StopBgpFailoverTestResponseTypeDef",
     "LocationsTypeDef",
     "VirtualGatewaysTypeDef",
-    "InterconnectsTypeDef",
     "AllocatePrivateVirtualInterfaceRequestRequestTypeDef",
     "CreatePrivateVirtualInterfaceRequestRequestTypeDef",
     "AllocatePublicVirtualInterfaceRequestRequestTypeDef",
     "CreatePublicVirtualInterfaceRequestRequestTypeDef",
     "AllocateTransitVirtualInterfaceRequestRequestTypeDef",
     "CreateTransitVirtualInterfaceRequestRequestTypeDef",
-    "DescribeTagsResponseTypeDef",
     "ConnectionsTypeDef",
     "LagResponseMetadataTypeDef",
     "LagTypeDef",
+    "InterconnectsTypeDef",
+    "DescribeTagsResponseTypeDef",
     "CreateDirectConnectGatewayAssociationProposalResultTypeDef",
     "DeleteDirectConnectGatewayAssociationProposalResultTypeDef",
     "DescribeDirectConnectGatewayAssociationProposalsResultTypeDef",
     "AcceptDirectConnectGatewayAssociationProposalResultTypeDef",
     "CreateDirectConnectGatewayAssociationResultTypeDef",
     "DeleteDirectConnectGatewayAssociationResultTypeDef",
     "DescribeDirectConnectGatewayAssociationsResultTypeDef",
@@ -390,14 +392,31 @@
     "ConfirmTransitVirtualInterfaceResponseTypeDef",
     {
         "virtualInterfaceState": VirtualInterfaceStateType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
+    {
+        "key": str,
+    },
+)
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
+    {
+        "value": str,
+    },
+    total=False,
+)
+
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
+    pass
+
 NewBGPPeerTypeDef = TypedDict(
     "NewBGPPeerTypeDef",
     {
         "asn": int,
         "authKey": str,
         "addressFamily": AddressFamilyType,
         "amazonAddress": str,
@@ -772,14 +791,22 @@
     {
         "connectionId": str,
         "virtualInterfaceId": str,
     },
     total=False,
 )
 
+RouteFilterPrefixOutputTypeDef = TypedDict(
+    "RouteFilterPrefixOutputTypeDef",
+    {
+        "cidr": str,
+    },
+    total=False,
+)
+
 DisassociateConnectionFromLagRequestRequestTypeDef = TypedDict(
     "DisassociateConnectionFromLagRequestRequestTypeDef",
     {
         "connectionId": str,
         "lagId": str,
     },
 )
@@ -1150,58 +1177,14 @@
 )
 
 class CreateLagRequestRequestTypeDef(
     _RequiredCreateLagRequestRequestTypeDef, _OptionalCreateLagRequestRequestTypeDef
 ):
     pass
 
-InterconnectResponseMetadataTypeDef = TypedDict(
-    "InterconnectResponseMetadataTypeDef",
-    {
-        "interconnectId": str,
-        "interconnectName": str,
-        "interconnectState": InterconnectStateType,
-        "region": str,
-        "location": str,
-        "bandwidth": str,
-        "loaIssueTime": datetime,
-        "lagId": str,
-        "awsDevice": str,
-        "jumboFrameCapable": bool,
-        "awsDeviceV2": str,
-        "awsLogicalDeviceId": str,
-        "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagTypeDef],
-        "providerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-InterconnectTypeDef = TypedDict(
-    "InterconnectTypeDef",
-    {
-        "interconnectId": str,
-        "interconnectName": str,
-        "interconnectState": InterconnectStateType,
-        "region": str,
-        "location": str,
-        "bandwidth": str,
-        "loaIssueTime": datetime,
-        "lagId": str,
-        "awsDevice": str,
-        "jumboFrameCapable": bool,
-        "awsDeviceV2": str,
-        "awsLogicalDeviceId": str,
-        "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagTypeDef],
-        "providerName": str,
-    },
-    total=False,
-)
-
 _RequiredNewPrivateVirtualInterfaceAllocationTypeDef = TypedDict(
     "_RequiredNewPrivateVirtualInterfaceAllocationTypeDef",
     {
         "virtualInterfaceName": str,
         "vlan": int,
         "asn": int,
     },
@@ -1337,23 +1320,14 @@
         "directConnectGatewayId": str,
         "tags": Sequence[TagTypeDef],
         "enableSiteLink": bool,
     },
     total=False,
 )
 
-ResourceTagTypeDef = TypedDict(
-    "ResourceTagTypeDef",
-    {
-        "resourceArn": str,
-        "tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1363,14 +1337,23 @@
     {
         "connectionId": str,
         "macSecKeys": List[MacSecKeyTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DisassociateMacSecKeyResponseTypeDef = TypedDict(
+    "DisassociateMacSecKeyResponseTypeDef",
+    {
+        "connectionId": str,
+        "macSecKeys": List[MacSecKeyTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ConnectionResponseMetadataTypeDef = TypedDict(
     "ConnectionResponseMetadataTypeDef",
     {
         "ownerAccount": str,
         "connectionId": str,
         "connectionName": str,
         "connectionState": ConnectionStateType,
@@ -1382,15 +1365,15 @@
         "loaIssueTime": datetime,
         "lagId": str,
         "awsDevice": str,
         "jumboFrameCapable": bool,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "portEncryptionStatus": str,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1411,126 +1394,73 @@
         "loaIssueTime": datetime,
         "lagId": str,
         "awsDevice": str,
         "jumboFrameCapable": bool,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "portEncryptionStatus": str,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
     },
     total=False,
 )
 
-DisassociateMacSecKeyResponseTypeDef = TypedDict(
-    "DisassociateMacSecKeyResponseTypeDef",
-    {
-        "connectionId": str,
-        "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DirectConnectGatewayAssociationProposalTypeDef = TypedDict(
-    "DirectConnectGatewayAssociationProposalTypeDef",
-    {
-        "proposalId": str,
-        "directConnectGatewayId": str,
-        "directConnectGatewayOwnerAccount": str,
-        "proposalState": DirectConnectGatewayAssociationProposalStateType,
-        "associatedGateway": AssociatedGatewayTypeDef,
-        "existingAllowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixTypeDef],
-        "requestedAllowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixTypeDef],
-    },
-    total=False,
-)
-
-DirectConnectGatewayAssociationTypeDef = TypedDict(
-    "DirectConnectGatewayAssociationTypeDef",
-    {
-        "directConnectGatewayId": str,
-        "directConnectGatewayOwnerAccount": str,
-        "associationState": DirectConnectGatewayAssociationStateType,
-        "stateChangeError": str,
-        "associatedGateway": AssociatedGatewayTypeDef,
-        "associationId": str,
-        "allowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixTypeDef],
-        "virtualGatewayId": str,
-        "virtualGatewayRegion": str,
-        "virtualGatewayOwnerAccount": str,
-    },
-    total=False,
-)
-
-VirtualInterfaceResponseMetadataTypeDef = TypedDict(
-    "VirtualInterfaceResponseMetadataTypeDef",
+InterconnectResponseMetadataTypeDef = TypedDict(
+    "InterconnectResponseMetadataTypeDef",
     {
-        "ownerAccount": str,
-        "virtualInterfaceId": str,
+        "interconnectId": str,
+        "interconnectName": str,
+        "interconnectState": InterconnectStateType,
+        "region": str,
         "location": str,
-        "connectionId": str,
-        "virtualInterfaceType": str,
-        "virtualInterfaceName": str,
-        "vlan": int,
-        "asn": int,
-        "amazonSideAsn": int,
-        "authKey": str,
-        "amazonAddress": str,
-        "customerAddress": str,
-        "addressFamily": AddressFamilyType,
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "customerRouterConfig": str,
-        "mtu": int,
+        "bandwidth": str,
+        "loaIssueTime": datetime,
+        "lagId": str,
+        "awsDevice": str,
         "jumboFrameCapable": bool,
-        "virtualGatewayId": str,
-        "directConnectGatewayId": str,
-        "routeFilterPrefixes": List[RouteFilterPrefixTypeDef],
-        "bgpPeers": List[BGPPeerTypeDef],
-        "region": str,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
-        "tags": List[TagTypeDef],
-        "siteLinkEnabled": bool,
+        "hasLogicalRedundancy": HasLogicalRedundancyType,
+        "tags": List[TagOutputTypeDef],
+        "providerName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-VirtualInterfaceTypeDef = TypedDict(
-    "VirtualInterfaceTypeDef",
+InterconnectTypeDef = TypedDict(
+    "InterconnectTypeDef",
     {
-        "ownerAccount": str,
-        "virtualInterfaceId": str,
+        "interconnectId": str,
+        "interconnectName": str,
+        "interconnectState": InterconnectStateType,
+        "region": str,
         "location": str,
-        "connectionId": str,
-        "virtualInterfaceType": str,
-        "virtualInterfaceName": str,
-        "vlan": int,
-        "asn": int,
-        "amazonSideAsn": int,
-        "authKey": str,
-        "amazonAddress": str,
-        "customerAddress": str,
-        "addressFamily": AddressFamilyType,
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "customerRouterConfig": str,
-        "mtu": int,
+        "bandwidth": str,
+        "loaIssueTime": datetime,
+        "lagId": str,
+        "awsDevice": str,
         "jumboFrameCapable": bool,
-        "virtualGatewayId": str,
-        "directConnectGatewayId": str,
-        "routeFilterPrefixes": List[RouteFilterPrefixTypeDef],
-        "bgpPeers": List[BGPPeerTypeDef],
-        "region": str,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
-        "tags": List[TagTypeDef],
-        "siteLinkEnabled": bool,
+        "hasLogicalRedundancy": HasLogicalRedundancyType,
+        "tags": List[TagOutputTypeDef],
+        "providerName": str,
+    },
+    total=False,
+)
+
+ResourceTagTypeDef = TypedDict(
+    "ResourceTagTypeDef",
+    {
+        "resourceArn": str,
+        "tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
 CreateBGPPeerRequestRequestTypeDef = TypedDict(
     "CreateBGPPeerRequestRequestTypeDef",
     {
@@ -1614,14 +1544,111 @@
         "router": RouterTypeTypeDef,
         "virtualInterfaceId": str,
         "virtualInterfaceName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DirectConnectGatewayAssociationProposalTypeDef = TypedDict(
+    "DirectConnectGatewayAssociationProposalTypeDef",
+    {
+        "proposalId": str,
+        "directConnectGatewayId": str,
+        "directConnectGatewayOwnerAccount": str,
+        "proposalState": DirectConnectGatewayAssociationProposalStateType,
+        "associatedGateway": AssociatedGatewayTypeDef,
+        "existingAllowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixOutputTypeDef],
+        "requestedAllowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixOutputTypeDef],
+    },
+    total=False,
+)
+
+DirectConnectGatewayAssociationTypeDef = TypedDict(
+    "DirectConnectGatewayAssociationTypeDef",
+    {
+        "directConnectGatewayId": str,
+        "directConnectGatewayOwnerAccount": str,
+        "associationState": DirectConnectGatewayAssociationStateType,
+        "stateChangeError": str,
+        "associatedGateway": AssociatedGatewayTypeDef,
+        "associationId": str,
+        "allowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixOutputTypeDef],
+        "virtualGatewayId": str,
+        "virtualGatewayRegion": str,
+        "virtualGatewayOwnerAccount": str,
+    },
+    total=False,
+)
+
+VirtualInterfaceResponseMetadataTypeDef = TypedDict(
+    "VirtualInterfaceResponseMetadataTypeDef",
+    {
+        "ownerAccount": str,
+        "virtualInterfaceId": str,
+        "location": str,
+        "connectionId": str,
+        "virtualInterfaceType": str,
+        "virtualInterfaceName": str,
+        "vlan": int,
+        "asn": int,
+        "amazonSideAsn": int,
+        "authKey": str,
+        "amazonAddress": str,
+        "customerAddress": str,
+        "addressFamily": AddressFamilyType,
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "customerRouterConfig": str,
+        "mtu": int,
+        "jumboFrameCapable": bool,
+        "virtualGatewayId": str,
+        "directConnectGatewayId": str,
+        "routeFilterPrefixes": List[RouteFilterPrefixOutputTypeDef],
+        "bgpPeers": List[BGPPeerTypeDef],
+        "region": str,
+        "awsDeviceV2": str,
+        "awsLogicalDeviceId": str,
+        "tags": List[TagOutputTypeDef],
+        "siteLinkEnabled": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+VirtualInterfaceTypeDef = TypedDict(
+    "VirtualInterfaceTypeDef",
+    {
+        "ownerAccount": str,
+        "virtualInterfaceId": str,
+        "location": str,
+        "connectionId": str,
+        "virtualInterfaceType": str,
+        "virtualInterfaceName": str,
+        "vlan": int,
+        "asn": int,
+        "amazonSideAsn": int,
+        "authKey": str,
+        "amazonAddress": str,
+        "customerAddress": str,
+        "addressFamily": AddressFamilyType,
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "customerRouterConfig": str,
+        "mtu": int,
+        "jumboFrameCapable": bool,
+        "virtualGatewayId": str,
+        "directConnectGatewayId": str,
+        "routeFilterPrefixes": List[RouteFilterPrefixOutputTypeDef],
+        "bgpPeers": List[BGPPeerTypeDef],
+        "region": str,
+        "awsDeviceV2": str,
+        "awsLogicalDeviceId": str,
+        "tags": List[TagOutputTypeDef],
+        "siteLinkEnabled": bool,
+    },
+    total=False,
+)
+
 ListVirtualInterfaceTestHistoryResponseTypeDef = TypedDict(
     "ListVirtualInterfaceTestHistoryResponseTypeDef",
     {
         "virtualInterfaceTestHistory": List[VirtualInterfaceTestHistoryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1655,22 +1682,14 @@
     "VirtualGatewaysTypeDef",
     {
         "virtualGateways": List[VirtualGatewayTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-InterconnectsTypeDef = TypedDict(
-    "InterconnectsTypeDef",
-    {
-        "interconnects": List[InterconnectTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AllocatePrivateVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "AllocatePrivateVirtualInterfaceRequestRequestTypeDef",
     {
         "connectionId": str,
         "ownerAccount": str,
         "newPrivateVirtualInterfaceAllocation": NewPrivateVirtualInterfaceAllocationTypeDef,
     },
@@ -1714,22 +1733,14 @@
     "CreateTransitVirtualInterfaceRequestRequestTypeDef",
     {
         "connectionId": str,
         "newTransitVirtualInterface": NewTransitVirtualInterfaceTypeDef,
     },
 )
 
-DescribeTagsResponseTypeDef = TypedDict(
-    "DescribeTagsResponseTypeDef",
-    {
-        "resourceTags": List[ResourceTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ConnectionsTypeDef = TypedDict(
     "ConnectionsTypeDef",
     {
         "connections": List[ConnectionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1749,15 +1760,15 @@
         "awsDevice": str,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "connections": List[ConnectionTypeDef],
         "allowsHostedConnections": bool,
         "jumboFrameCapable": bool,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1777,23 +1788,39 @@
         "awsDevice": str,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "connections": List[ConnectionTypeDef],
         "allowsHostedConnections": bool,
         "jumboFrameCapable": bool,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
     },
     total=False,
 )
 
+InterconnectsTypeDef = TypedDict(
+    "InterconnectsTypeDef",
+    {
+        "interconnects": List[InterconnectTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeTagsResponseTypeDef = TypedDict(
+    "DescribeTagsResponseTypeDef",
+    {
+        "resourceTags": List[ResourceTagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateDirectConnectGatewayAssociationProposalResultTypeDef = TypedDict(
     "CreateDirectConnectGatewayAssociationProposalResultTypeDef",
     {
         "directConnectGatewayAssociationProposal": DirectConnectGatewayAssociationProposalTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect.egg-info/PKG-INFO` & `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-directconnect
-Version: 1.28.0
-Summary: Type annotations for boto3.DirectConnect 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.DirectConnect 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-directconnect"></a>
 
 # mypy-boto3-directconnect
 
 [![PyPI - mypy-boto3-directconnect](https://img.shields.io/pypi/v/mypy-boto3-directconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-directconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-directconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-directconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-directconnect?color=blue)](https://pypistats.org/packages/mypy-boto3-directconnect)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-directconnect)](https://pepy.tech/project/mypy-boto3-directconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DirectConnect 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
+[boto3.DirectConnect 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
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
 [mypy-boto3-directconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -369,14 +369,15 @@
     ConfirmCustomerAgreementResponseTypeDef,
     ConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
     ConfirmPrivateVirtualInterfaceResponseTypeDef,
     ConfirmPublicVirtualInterfaceRequestRequestTypeDef,
     ConfirmPublicVirtualInterfaceResponseTypeDef,
     ConfirmTransitVirtualInterfaceRequestRequestTypeDef,
     ConfirmTransitVirtualInterfaceResponseTypeDef,
+    TagOutputTypeDef,
     NewBGPPeerTypeDef,
     CreateDirectConnectGatewayRequestRequestTypeDef,
     DirectConnectGatewayTypeDef,
     CustomerAgreementTypeDef,
     DeleteBGPPeerRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
@@ -404,14 +405,15 @@
     DescribeInterconnectsRequestRequestTypeDef,
     DescribeLagsRequestRequestTypeDef,
     DescribeLoaRequestRequestTypeDef,
     DescribeRouterConfigurationRequestRequestTypeDef,
     RouterTypeTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DescribeVirtualInterfacesRequestRequestTypeDef,
+    RouteFilterPrefixOutputTypeDef,
     DisassociateConnectionFromLagRequestRequestTypeDef,
     DisassociateMacSecKeyRequestRequestTypeDef,
     ListVirtualInterfaceTestHistoryRequestRequestTypeDef,
     VirtualInterfaceTestHistoryTypeDef,
     LoaResponseMetadataTypeDef,
     LocationTypeDef,
     PaginatorConfigTypeDef,
@@ -428,58 +430,58 @@
     CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     CreateDirectConnectGatewayAssociationRequestRequestTypeDef,
     UpdateDirectConnectGatewayAssociationRequestRequestTypeDef,
     AllocateHostedConnectionRequestRequestTypeDef,
     CreateConnectionRequestRequestTypeDef,
     CreateInterconnectRequestRequestTypeDef,
     CreateLagRequestRequestTypeDef,
-    InterconnectResponseMetadataTypeDef,
-    InterconnectTypeDef,
     NewPrivateVirtualInterfaceAllocationTypeDef,
     NewPrivateVirtualInterfaceTypeDef,
     NewPublicVirtualInterfaceAllocationTypeDef,
     NewPublicVirtualInterfaceTypeDef,
     NewTransitVirtualInterfaceAllocationTypeDef,
     NewTransitVirtualInterfaceTypeDef,
-    ResourceTagTypeDef,
     TagResourceRequestRequestTypeDef,
     AssociateMacSecKeyResponseTypeDef,
+    DisassociateMacSecKeyResponseTypeDef,
     ConnectionResponseMetadataTypeDef,
     ConnectionTypeDef,
-    DisassociateMacSecKeyResponseTypeDef,
-    DirectConnectGatewayAssociationProposalTypeDef,
-    DirectConnectGatewayAssociationTypeDef,
-    VirtualInterfaceResponseMetadataTypeDef,
-    VirtualInterfaceTypeDef,
+    InterconnectResponseMetadataTypeDef,
+    InterconnectTypeDef,
+    ResourceTagTypeDef,
     CreateBGPPeerRequestRequestTypeDef,
     CreateDirectConnectGatewayResultTypeDef,
     DeleteDirectConnectGatewayResultTypeDef,
     DescribeDirectConnectGatewaysResultTypeDef,
     UpdateDirectConnectGatewayResponseTypeDef,
     DescribeCustomerMetadataResponseTypeDef,
     DescribeConnectionLoaResponseTypeDef,
     DescribeInterconnectLoaResponseTypeDef,
     DescribeDirectConnectGatewayAttachmentsResultTypeDef,
     DescribeRouterConfigurationResponseTypeDef,
+    DirectConnectGatewayAssociationProposalTypeDef,
+    DirectConnectGatewayAssociationTypeDef,
+    VirtualInterfaceResponseMetadataTypeDef,
+    VirtualInterfaceTypeDef,
     ListVirtualInterfaceTestHistoryResponseTypeDef,
     StartBgpFailoverTestResponseTypeDef,
     StopBgpFailoverTestResponseTypeDef,
     LocationsTypeDef,
     VirtualGatewaysTypeDef,
-    InterconnectsTypeDef,
     AllocatePrivateVirtualInterfaceRequestRequestTypeDef,
     CreatePrivateVirtualInterfaceRequestRequestTypeDef,
     AllocatePublicVirtualInterfaceRequestRequestTypeDef,
     CreatePublicVirtualInterfaceRequestRequestTypeDef,
     AllocateTransitVirtualInterfaceRequestRequestTypeDef,
     CreateTransitVirtualInterfaceRequestRequestTypeDef,
-    DescribeTagsResponseTypeDef,
     ConnectionsTypeDef,
     LagResponseMetadataTypeDef,
     LagTypeDef,
+    InterconnectsTypeDef,
+    DescribeTagsResponseTypeDef,
     CreateDirectConnectGatewayAssociationProposalResultTypeDef,
     DeleteDirectConnectGatewayAssociationProposalResultTypeDef,
     DescribeDirectConnectGatewayAssociationProposalsResultTypeDef,
     AcceptDirectConnectGatewayAssociationProposalResultTypeDef,
     CreateDirectConnectGatewayAssociationResultTypeDef,
     DeleteDirectConnectGatewayAssociationResultTypeDef,
     DescribeDirectConnectGatewayAssociationsResultTypeDef,
```

### Comparing `mypy-boto3-directconnect-1.28.0/mypy_boto3_directconnect.egg-info/SOURCES.txt` & `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.28.0/setup.py` & `mypy-boto3-directconnect-1.28.12/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-directconnect",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_directconnect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DirectConnect 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.DirectConnect 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

