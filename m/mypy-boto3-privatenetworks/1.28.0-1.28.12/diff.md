# Comparing `tmp/mypy-boto3-privatenetworks-1.28.0.tar.gz` & `tmp/mypy-boto3-privatenetworks-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-privatenetworks-1.28.0.tar", last modified: Thu Jul  6 21:00:21 2023, max compression
+gzip compressed data, was "mypy-boto3-privatenetworks-1.28.12.tar", last modified: Thu Jul 27 11:49:24 2023, max compression
```

## Comparing `mypy-boto3-privatenetworks-1.28.0.tar` & `mypy-boto3-privatenetworks-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:21.982399 mypy-boto3-privatenetworks-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:49:45.000000 mypy-boto3-privatenetworks-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-07-06 21:00:21.974399 mypy-boto3-privatenetworks-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-07-06 20:49:45.000000 mypy-boto3-privatenetworks-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:21.970399 mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-06 20:49:45.000000 mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-06 20:49:45.000000 mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:49:45.000000 mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21342 2023-07-06 20:49:45.000000 mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-07-06 20:49:45.000000 mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-07-06 20:49:46.000000 mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-07-06 20:49:46.000000 mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-07-06 20:49:45.000000 mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-06 20:49:45.000000 mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:49:45.000000 mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29010 2023-07-06 20:49:47.000000 mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28957 2023-07-06 20:49:46.000000 mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:49:45.000000 mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:21.974399 mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-07-06 21:00:21.000000 mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-06 21:00:21.000000 mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:21.000000 mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:21.000000 mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:21.000000 mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 21:00:21.000000 mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:21.982399 mypy-boto3-privatenetworks-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-06 20:49:45.000000 mypy-boto3-privatenetworks-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.957163 mypy-boto3-privatenetworks-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-07-27 11:49:24.957163 mypy-boto3-privatenetworks-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.957163 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21342 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-07-27 11:41:44.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31478 2023-07-27 11:41:45.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31419 2023-07-27 11:41:44.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.957163 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-07-27 11:49:24.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-27 11:49:24.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:24.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 11:49:24.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:24.957163 mypy-boto3-privatenetworks-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/setup.py
```

### Comparing `mypy-boto3-privatenetworks-1.28.0/LICENSE` & `mypy-boto3-privatenetworks-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.0/PKG-INFO` & `mypy-boto3-privatenetworks-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-privatenetworks
-Version: 1.28.0
-Summary: Type annotations for boto3.Private5G 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Private5G 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-privatenetworks"></a>
 
 # mypy-boto3-privatenetworks
 
 [![PyPI - mypy-boto3-privatenetworks](https://img.shields.io/pypi/v/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-privatenetworks?color=blue)](https://pypistats.org/packages/mypy-boto3-privatenetworks)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-privatenetworks)](https://pepy.tech/project/mypy-boto3-privatenetworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Private5G 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
+[boto3.Private5G 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
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
 [mypy-boto3-privatenetworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,76 +354,82 @@
 
 `mypy_boto3_privatenetworks.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_privatenetworks.type_defs import (
     AcknowledgeOrderReceiptRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ActivateDeviceIdentifierRequestRequestTypeDef,
     DeviceIdentifierTypeDef,
     AddressTypeDef,
     CommitmentConfigurationTypeDef,
+    AddressOutputTypeDef,
+    CommitmentConfigurationOutputTypeDef,
     PositionTypeDef,
     CreateNetworkRequestRequestTypeDef,
     NetworkTypeDef,
     DeactivateDeviceIdentifierRequestRequestTypeDef,
     DeleteNetworkRequestRequestTypeDef,
     DeleteNetworkSiteRequestRequestTypeDef,
     GetDeviceIdentifierRequestRequestTypeDef,
     GetNetworkRequestRequestTypeDef,
     GetNetworkResourceRequestRequestTypeDef,
     GetNetworkSiteRequestRequestTypeDef,
     GetOrderRequestRequestTypeDef,
-    ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDeviceIdentifiersRequestRequestTypeDef,
-    ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
     ListNetworkResourcesRequestRequestTypeDef,
-    ListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
     ListNetworkSitesRequestRequestTypeDef,
-    ListNetworksRequestListNetworksPaginateTypeDef,
     ListNetworksRequestRequestTypeDef,
-    ListOrdersRequestListOrdersPaginateTypeDef,
     ListOrdersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    NameValuePairOutputTypeDef,
     NameValuePairTypeDef,
+    PositionOutputTypeDef,
     TrackingInformationTypeDef,
-    PaginatorConfigTypeDef,
-    PingResponseTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateNetworkSiteRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PingResponseTypeDef,
     ActivateDeviceIdentifierResponseTypeDef,
     DeactivateDeviceIdentifierResponseTypeDef,
     GetDeviceIdentifierResponseTypeDef,
     ListDeviceIdentifiersResponseTypeDef,
-    ReturnInformationTypeDef,
     ActivateNetworkSiteRequestRequestTypeDef,
+    StartNetworkResourceUpdateRequestRequestTypeDef,
+    ReturnInformationTypeDef,
     CommitmentInformationTypeDef,
     OrderedResourceDefinitionTypeDef,
-    StartNetworkResourceUpdateRequestRequestTypeDef,
     ConfigureAccessPointRequestRequestTypeDef,
     CreateNetworkResponseTypeDef,
     DeleteNetworkResponseTypeDef,
     GetNetworkResponseTypeDef,
     ListNetworksResponseTypeDef,
+    ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
+    ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
+    ListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
+    ListNetworksRequestListNetworksPaginateTypeDef,
+    ListOrdersRequestListOrdersPaginateTypeDef,
+    NetworkResourceDefinitionOutputTypeDef,
     NetworkResourceDefinitionTypeDef,
     NetworkResourceTypeDef,
     OrderTypeDef,
+    SitePlanOutputTypeDef,
     SitePlanTypeDef,
     ConfigureAccessPointResponseTypeDef,
     GetNetworkResourceResponseTypeDef,
     ListNetworkResourcesResponseTypeDef,
     StartNetworkResourceUpdateResponseTypeDef,
     AcknowledgeOrderReceiptResponseTypeDef,
     GetOrderResponseTypeDef,
     ListOrdersResponseTypeDef,
-    CreateNetworkSiteRequestRequestTypeDef,
     NetworkSiteTypeDef,
+    CreateNetworkSiteRequestRequestTypeDef,
     UpdateNetworkSitePlanRequestRequestTypeDef,
     ActivateNetworkSiteResponseTypeDef,
     CreateNetworkSiteResponseTypeDef,
     DeleteNetworkSiteResponseTypeDef,
     GetNetworkSiteResponseTypeDef,
     ListNetworkSitesResponseTypeDef,
     UpdateNetworkSiteResponseTypeDef,
```

### Comparing `mypy-boto3-privatenetworks-1.28.0/README.md` & `mypy-boto3-privatenetworks-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-privatenetworks"></a>
 
 # mypy-boto3-privatenetworks
 
 [![PyPI - mypy-boto3-privatenetworks](https://img.shields.io/pypi/v/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-privatenetworks?color=blue)](https://pypistats.org/packages/mypy-boto3-privatenetworks)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-privatenetworks)](https://pepy.tech/project/mypy-boto3-privatenetworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Private5G 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
+[boto3.Private5G 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
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
 [mypy-boto3-privatenetworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,76 +322,82 @@
 
 `mypy_boto3_privatenetworks.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_privatenetworks.type_defs import (
     AcknowledgeOrderReceiptRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ActivateDeviceIdentifierRequestRequestTypeDef,
     DeviceIdentifierTypeDef,
     AddressTypeDef,
     CommitmentConfigurationTypeDef,
+    AddressOutputTypeDef,
+    CommitmentConfigurationOutputTypeDef,
     PositionTypeDef,
     CreateNetworkRequestRequestTypeDef,
     NetworkTypeDef,
     DeactivateDeviceIdentifierRequestRequestTypeDef,
     DeleteNetworkRequestRequestTypeDef,
     DeleteNetworkSiteRequestRequestTypeDef,
     GetDeviceIdentifierRequestRequestTypeDef,
     GetNetworkRequestRequestTypeDef,
     GetNetworkResourceRequestRequestTypeDef,
     GetNetworkSiteRequestRequestTypeDef,
     GetOrderRequestRequestTypeDef,
-    ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDeviceIdentifiersRequestRequestTypeDef,
-    ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
     ListNetworkResourcesRequestRequestTypeDef,
-    ListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
     ListNetworkSitesRequestRequestTypeDef,
-    ListNetworksRequestListNetworksPaginateTypeDef,
     ListNetworksRequestRequestTypeDef,
-    ListOrdersRequestListOrdersPaginateTypeDef,
     ListOrdersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    NameValuePairOutputTypeDef,
     NameValuePairTypeDef,
+    PositionOutputTypeDef,
     TrackingInformationTypeDef,
-    PaginatorConfigTypeDef,
-    PingResponseTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateNetworkSiteRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PingResponseTypeDef,
     ActivateDeviceIdentifierResponseTypeDef,
     DeactivateDeviceIdentifierResponseTypeDef,
     GetDeviceIdentifierResponseTypeDef,
     ListDeviceIdentifiersResponseTypeDef,
-    ReturnInformationTypeDef,
     ActivateNetworkSiteRequestRequestTypeDef,
+    StartNetworkResourceUpdateRequestRequestTypeDef,
+    ReturnInformationTypeDef,
     CommitmentInformationTypeDef,
     OrderedResourceDefinitionTypeDef,
-    StartNetworkResourceUpdateRequestRequestTypeDef,
     ConfigureAccessPointRequestRequestTypeDef,
     CreateNetworkResponseTypeDef,
     DeleteNetworkResponseTypeDef,
     GetNetworkResponseTypeDef,
     ListNetworksResponseTypeDef,
+    ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
+    ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
+    ListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
+    ListNetworksRequestListNetworksPaginateTypeDef,
+    ListOrdersRequestListOrdersPaginateTypeDef,
+    NetworkResourceDefinitionOutputTypeDef,
     NetworkResourceDefinitionTypeDef,
     NetworkResourceTypeDef,
     OrderTypeDef,
+    SitePlanOutputTypeDef,
     SitePlanTypeDef,
     ConfigureAccessPointResponseTypeDef,
     GetNetworkResourceResponseTypeDef,
     ListNetworkResourcesResponseTypeDef,
     StartNetworkResourceUpdateResponseTypeDef,
     AcknowledgeOrderReceiptResponseTypeDef,
     GetOrderResponseTypeDef,
     ListOrdersResponseTypeDef,
-    CreateNetworkSiteRequestRequestTypeDef,
     NetworkSiteTypeDef,
+    CreateNetworkSiteRequestRequestTypeDef,
     UpdateNetworkSitePlanRequestRequestTypeDef,
     ActivateNetworkSiteResponseTypeDef,
     CreateNetworkSiteResponseTypeDef,
     DeleteNetworkSiteResponseTypeDef,
     GetNetworkSiteResponseTypeDef,
     ListNetworkSitesResponseTypeDef,
     UpdateNetworkSiteResponseTypeDef,
```

### Comparing `mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/__init__.py` & `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/__init__.pyi` & `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/__main__.py` & `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Private5G 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Private5G 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G\nOther"
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

### Comparing `mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/client.py` & `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/client.pyi` & `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/literals.py` & `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,14 +197,15 @@
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
@@ -283,26 +284,28 @@
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

### Comparing `mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/literals.pyi` & `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -195,14 +195,15 @@
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
@@ -281,26 +282,28 @@
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

### Comparing `mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/paginator.py` & `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[DeviceIdentifierFilterKeysType, Sequence[str]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeviceIdentifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListDeviceIdentifiers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listdeviceidentifierspaginator)
         """
 
 
@@ -97,15 +97,15 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[NetworkResourceFilterKeysType, Sequence[str]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNetworkResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListNetworkResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listnetworkresourcespaginator)
         """
 
 
@@ -116,15 +116,15 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNetworkSitesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListNetworkSites.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listnetworksitespaginator)
         """
 
 
@@ -134,15 +134,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listnetworkspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListNetworks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listnetworkspaginator)
         """
 
 
@@ -153,13 +153,13 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[OrderFilterKeysType, Sequence[str]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOrdersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListOrders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listorderspaginator)
         """
```

### Comparing `mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/paginator.pyi` & `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[DeviceIdentifierFilterKeysType, Sequence[str]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeviceIdentifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListDeviceIdentifiers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listdeviceidentifierspaginator)
         """
 
 class ListNetworkResourcesPaginator(Paginator):
@@ -92,15 +92,15 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[NetworkResourceFilterKeysType, Sequence[str]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNetworkResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListNetworkResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listnetworkresourcespaginator)
         """
 
 class ListNetworkSitesPaginator(Paginator):
@@ -110,15 +110,15 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNetworkSitesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListNetworkSites.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listnetworksitespaginator)
         """
 
 class ListNetworksPaginator(Paginator):
@@ -127,15 +127,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listnetworkspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListNetworks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listnetworkspaginator)
         """
 
 class ListOrdersPaginator(Paginator):
@@ -145,13 +145,13 @@
     """
 
     def paginate(
         self,
         *,
         networkArn: str,
         filters: Mapping[OrderFilterKeysType, Sequence[str]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOrdersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Paginator.ListOrders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/paginators/#listorderspaginator)
         """
```

### Comparing `mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/type_defs.py` & `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,76 +39,82 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AcknowledgeOrderReceiptRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ActivateDeviceIdentifierRequestRequestTypeDef",
     "DeviceIdentifierTypeDef",
     "AddressTypeDef",
     "CommitmentConfigurationTypeDef",
+    "AddressOutputTypeDef",
+    "CommitmentConfigurationOutputTypeDef",
     "PositionTypeDef",
     "CreateNetworkRequestRequestTypeDef",
     "NetworkTypeDef",
     "DeactivateDeviceIdentifierRequestRequestTypeDef",
     "DeleteNetworkRequestRequestTypeDef",
     "DeleteNetworkSiteRequestRequestTypeDef",
     "GetDeviceIdentifierRequestRequestTypeDef",
     "GetNetworkRequestRequestTypeDef",
     "GetNetworkResourceRequestRequestTypeDef",
     "GetNetworkSiteRequestRequestTypeDef",
     "GetOrderRequestRequestTypeDef",
-    "ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDeviceIdentifiersRequestRequestTypeDef",
-    "ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
     "ListNetworkResourcesRequestRequestTypeDef",
-    "ListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
     "ListNetworkSitesRequestRequestTypeDef",
-    "ListNetworksRequestListNetworksPaginateTypeDef",
     "ListNetworksRequestRequestTypeDef",
-    "ListOrdersRequestListOrdersPaginateTypeDef",
     "ListOrdersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "NameValuePairOutputTypeDef",
     "NameValuePairTypeDef",
+    "PositionOutputTypeDef",
     "TrackingInformationTypeDef",
-    "PaginatorConfigTypeDef",
-    "PingResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateNetworkSiteRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PingResponseTypeDef",
     "ActivateDeviceIdentifierResponseTypeDef",
     "DeactivateDeviceIdentifierResponseTypeDef",
     "GetDeviceIdentifierResponseTypeDef",
     "ListDeviceIdentifiersResponseTypeDef",
-    "ReturnInformationTypeDef",
     "ActivateNetworkSiteRequestRequestTypeDef",
+    "StartNetworkResourceUpdateRequestRequestTypeDef",
+    "ReturnInformationTypeDef",
     "CommitmentInformationTypeDef",
     "OrderedResourceDefinitionTypeDef",
-    "StartNetworkResourceUpdateRequestRequestTypeDef",
     "ConfigureAccessPointRequestRequestTypeDef",
     "CreateNetworkResponseTypeDef",
     "DeleteNetworkResponseTypeDef",
     "GetNetworkResponseTypeDef",
     "ListNetworksResponseTypeDef",
+    "ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
+    "ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
+    "ListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
+    "ListNetworksRequestListNetworksPaginateTypeDef",
+    "ListOrdersRequestListOrdersPaginateTypeDef",
+    "NetworkResourceDefinitionOutputTypeDef",
     "NetworkResourceDefinitionTypeDef",
     "NetworkResourceTypeDef",
     "OrderTypeDef",
+    "SitePlanOutputTypeDef",
     "SitePlanTypeDef",
     "ConfigureAccessPointResponseTypeDef",
     "GetNetworkResourceResponseTypeDef",
     "ListNetworkResourcesResponseTypeDef",
     "StartNetworkResourceUpdateResponseTypeDef",
     "AcknowledgeOrderReceiptResponseTypeDef",
     "GetOrderResponseTypeDef",
     "ListOrdersResponseTypeDef",
-    "CreateNetworkSiteRequestRequestTypeDef",
     "NetworkSiteTypeDef",
+    "CreateNetworkSiteRequestRequestTypeDef",
     "UpdateNetworkSitePlanRequestRequestTypeDef",
     "ActivateNetworkSiteResponseTypeDef",
     "CreateNetworkSiteResponseTypeDef",
     "DeleteNetworkSiteResponseTypeDef",
     "GetNetworkSiteResponseTypeDef",
     "ListNetworkSitesResponseTypeDef",
     "UpdateNetworkSiteResponseTypeDef",
@@ -117,14 +123,25 @@
 AcknowledgeOrderReceiptRequestRequestTypeDef = TypedDict(
     "AcknowledgeOrderReceiptRequestRequestTypeDef",
     {
         "orderArn": str,
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
 _RequiredActivateDeviceIdentifierRequestRequestTypeDef = TypedDict(
     "_RequiredActivateDeviceIdentifierRequestRequestTypeDef",
     {
         "deviceIdentifierArn": str,
     },
 )
 _OptionalActivateDeviceIdentifierRequestRequestTypeDef = TypedDict(
@@ -191,14 +208,50 @@
     "CommitmentConfigurationTypeDef",
     {
         "automaticRenewal": bool,
         "commitmentLength": CommitmentLengthType,
     },
 )
 
+_RequiredAddressOutputTypeDef = TypedDict(
+    "_RequiredAddressOutputTypeDef",
+    {
+        "city": str,
+        "country": str,
+        "name": str,
+        "postalCode": str,
+        "stateOrProvince": str,
+        "street1": str,
+    },
+)
+_OptionalAddressOutputTypeDef = TypedDict(
+    "_OptionalAddressOutputTypeDef",
+    {
+        "company": str,
+        "emailAddress": str,
+        "phoneNumber": str,
+        "street2": str,
+        "street3": str,
+    },
+    total=False,
+)
+
+
+class AddressOutputTypeDef(_RequiredAddressOutputTypeDef, _OptionalAddressOutputTypeDef):
+    pass
+
+
+CommitmentConfigurationOutputTypeDef = TypedDict(
+    "CommitmentConfigurationOutputTypeDef",
+    {
+        "automaticRenewal": bool,
+        "commitmentLength": CommitmentLengthType,
+    },
+)
+
 PositionTypeDef = TypedDict(
     "PositionTypeDef",
     {
         "elevation": float,
         "elevationReference": ElevationReferenceType,
         "elevationUnit": Literal["FEET"],
         "latitude": float,
@@ -348,37 +401,24 @@
 GetOrderRequestRequestTypeDef = TypedDict(
     "GetOrderRequestRequestTypeDef",
     {
         "orderArn": str,
     },
 )
 
-_RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef = TypedDict(
-    "_RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
-    {
-        "networkArn": str,
-    },
-)
-_OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef = TypedDict(
-    "_OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "filters": Mapping[DeviceIdentifierFilterKeysType, Sequence[str]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef(
-    _RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
-    _OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDeviceIdentifiersRequestRequestTypeDef = TypedDict(
     "_RequiredListDeviceIdentifiersRequestRequestTypeDef",
     {
         "networkArn": str,
     },
 )
 _OptionalListDeviceIdentifiersRequestRequestTypeDef = TypedDict(
@@ -395,37 +435,14 @@
 class ListDeviceIdentifiersRequestRequestTypeDef(
     _RequiredListDeviceIdentifiersRequestRequestTypeDef,
     _OptionalListDeviceIdentifiersRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
-    {
-        "networkArn": str,
-    },
-)
-_OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
-    {
-        "filters": Mapping[NetworkResourceFilterKeysType, Sequence[str]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef(
-    _RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
-    _OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListNetworkResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListNetworkResourcesRequestRequestTypeDef",
     {
         "networkArn": str,
     },
 )
 _OptionalListNetworkResourcesRequestRequestTypeDef = TypedDict(
@@ -442,37 +459,14 @@
 class ListNetworkResourcesRequestRequestTypeDef(
     _RequiredListNetworkResourcesRequestRequestTypeDef,
     _OptionalListNetworkResourcesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef = TypedDict(
-    "_RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
-    {
-        "networkArn": str,
-    },
-)
-_OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef = TypedDict(
-    "_OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
-    {
-        "filters": Mapping[Literal["STATUS"], Sequence[str]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListNetworkSitesRequestListNetworkSitesPaginateTypeDef(
-    _RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
-    _OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListNetworkSitesRequestRequestTypeDef = TypedDict(
     "_RequiredListNetworkSitesRequestRequestTypeDef",
     {
         "networkArn": str,
     },
 )
 _OptionalListNetworkSitesRequestRequestTypeDef = TypedDict(
@@ -488,56 +482,24 @@
 
 class ListNetworkSitesRequestRequestTypeDef(
     _RequiredListNetworkSitesRequestRequestTypeDef, _OptionalListNetworkSitesRequestRequestTypeDef
 ):
     pass
 
 
-ListNetworksRequestListNetworksPaginateTypeDef = TypedDict(
-    "ListNetworksRequestListNetworksPaginateTypeDef",
-    {
-        "filters": Mapping[Literal["STATUS"], Sequence[str]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListNetworksRequestRequestTypeDef = TypedDict(
     "ListNetworksRequestRequestTypeDef",
     {
         "filters": Mapping[Literal["STATUS"], Sequence[str]],
         "maxResults": int,
         "startToken": str,
     },
     total=False,
 )
 
-_RequiredListOrdersRequestListOrdersPaginateTypeDef = TypedDict(
-    "_RequiredListOrdersRequestListOrdersPaginateTypeDef",
-    {
-        "networkArn": str,
-    },
-)
-_OptionalListOrdersRequestListOrdersPaginateTypeDef = TypedDict(
-    "_OptionalListOrdersRequestListOrdersPaginateTypeDef",
-    {
-        "filters": Mapping[OrderFilterKeysType, Sequence[str]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListOrdersRequestListOrdersPaginateTypeDef(
-    _RequiredListOrdersRequestListOrdersPaginateTypeDef,
-    _OptionalListOrdersRequestListOrdersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListOrdersRequestRequestTypeDef = TypedDict(
     "_RequiredListOrdersRequestRequestTypeDef",
     {
         "networkArn": str,
     },
 )
 _OptionalListOrdersRequestRequestTypeDef = TypedDict(
@@ -560,21 +522,34 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_RequiredNameValuePairOutputTypeDef = TypedDict(
+    "_RequiredNameValuePairOutputTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
     },
 )
+_OptionalNameValuePairOutputTypeDef = TypedDict(
+    "_OptionalNameValuePairOutputTypeDef",
+    {
+        "value": str,
+    },
+    total=False,
+)
+
+
+class NameValuePairOutputTypeDef(
+    _RequiredNameValuePairOutputTypeDef, _OptionalNameValuePairOutputTypeDef
+):
+    pass
+
 
 _RequiredNameValuePairTypeDef = TypedDict(
     "_RequiredNameValuePairTypeDef",
     {
         "name": str,
     },
 )
@@ -587,51 +562,34 @@
 )
 
 
 class NameValuePairTypeDef(_RequiredNameValuePairTypeDef, _OptionalNameValuePairTypeDef):
     pass
 
 
-TrackingInformationTypeDef = TypedDict(
-    "TrackingInformationTypeDef",
+PositionOutputTypeDef = TypedDict(
+    "PositionOutputTypeDef",
     {
-        "trackingNumber": str,
+        "elevation": float,
+        "elevationReference": ElevationReferenceType,
+        "elevationUnit": Literal["FEET"],
+        "latitude": float,
+        "longitude": float,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+TrackingInformationTypeDef = TypedDict(
+    "TrackingInformationTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "trackingNumber": str,
     },
     total=False,
 )
 
-PingResponseTypeDef = TypedDict(
-    "PingResponseTypeDef",
-    {
-        "status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
@@ -662,58 +620,63 @@
 
 class UpdateNetworkSiteRequestRequestTypeDef(
     _RequiredUpdateNetworkSiteRequestRequestTypeDef, _OptionalUpdateNetworkSiteRequestRequestTypeDef
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PingResponseTypeDef = TypedDict(
+    "PingResponseTypeDef",
+    {
+        "status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ActivateDeviceIdentifierResponseTypeDef = TypedDict(
     "ActivateDeviceIdentifierResponseTypeDef",
     {
         "deviceIdentifier": DeviceIdentifierTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeactivateDeviceIdentifierResponseTypeDef = TypedDict(
     "DeactivateDeviceIdentifierResponseTypeDef",
     {
         "deviceIdentifier": DeviceIdentifierTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeviceIdentifierResponseTypeDef = TypedDict(
     "GetDeviceIdentifierResponseTypeDef",
     {
         "deviceIdentifier": DeviceIdentifierTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeviceIdentifiersResponseTypeDef = TypedDict(
     "ListDeviceIdentifiersResponseTypeDef",
     {
         "deviceIdentifiers": List[DeviceIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ReturnInformationTypeDef = TypedDict(
-    "ReturnInformationTypeDef",
-    {
-        "replacementOrderArn": str,
-        "returnReason": str,
-        "shippingAddress": AddressTypeDef,
-        "shippingLabel": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredActivateNetworkSiteRequestRequestTypeDef = TypedDict(
     "_RequiredActivateNetworkSiteRequestRequestTypeDef",
     {
         "networkSiteArn": str,
         "shippingAddress": AddressTypeDef,
@@ -732,18 +695,54 @@
 class ActivateNetworkSiteRequestRequestTypeDef(
     _RequiredActivateNetworkSiteRequestRequestTypeDef,
     _OptionalActivateNetworkSiteRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
+    "_RequiredStartNetworkResourceUpdateRequestRequestTypeDef",
+    {
+        "networkResourceArn": str,
+        "updateType": UpdateTypeType,
+    },
+)
+_OptionalStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
+    "_OptionalStartNetworkResourceUpdateRequestRequestTypeDef",
+    {
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
+        "returnReason": str,
+        "shippingAddress": AddressTypeDef,
+    },
+    total=False,
+)
+
+
+class StartNetworkResourceUpdateRequestRequestTypeDef(
+    _RequiredStartNetworkResourceUpdateRequestRequestTypeDef,
+    _OptionalStartNetworkResourceUpdateRequestRequestTypeDef,
+):
+    pass
+
+
+ReturnInformationTypeDef = TypedDict(
+    "ReturnInformationTypeDef",
+    {
+        "replacementOrderArn": str,
+        "returnReason": str,
+        "shippingAddress": AddressOutputTypeDef,
+        "shippingLabel": str,
+    },
+    total=False,
+)
+
 _RequiredCommitmentInformationTypeDef = TypedDict(
     "_RequiredCommitmentInformationTypeDef",
     {
-        "commitmentConfiguration": CommitmentConfigurationTypeDef,
+        "commitmentConfiguration": CommitmentConfigurationOutputTypeDef,
     },
 )
 _OptionalCommitmentInformationTypeDef = TypedDict(
     "_OptionalCommitmentInformationTypeDef",
     {
         "expiresOn": datetime,
         "startAt": datetime,
@@ -764,51 +763,26 @@
         "count": int,
         "type": NetworkResourceDefinitionTypeType,
     },
 )
 _OptionalOrderedResourceDefinitionTypeDef = TypedDict(
     "_OptionalOrderedResourceDefinitionTypeDef",
     {
-        "commitmentConfiguration": CommitmentConfigurationTypeDef,
+        "commitmentConfiguration": CommitmentConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 
 class OrderedResourceDefinitionTypeDef(
     _RequiredOrderedResourceDefinitionTypeDef, _OptionalOrderedResourceDefinitionTypeDef
 ):
     pass
 
 
-_RequiredStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
-    "_RequiredStartNetworkResourceUpdateRequestRequestTypeDef",
-    {
-        "networkResourceArn": str,
-        "updateType": UpdateTypeType,
-    },
-)
-_OptionalStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
-    "_OptionalStartNetworkResourceUpdateRequestRequestTypeDef",
-    {
-        "commitmentConfiguration": CommitmentConfigurationTypeDef,
-        "returnReason": str,
-        "shippingAddress": AddressTypeDef,
-    },
-    total=False,
-)
-
-
-class StartNetworkResourceUpdateRequestRequestTypeDef(
-    _RequiredStartNetworkResourceUpdateRequestRequestTypeDef,
-    _OptionalStartNetworkResourceUpdateRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredConfigureAccessPointRequestRequestTypeDef = TypedDict(
     "_RequiredConfigureAccessPointRequestRequestTypeDef",
     {
         "accessPointArn": str,
     },
 )
 _OptionalConfigureAccessPointRequestRequestTypeDef = TypedDict(
@@ -832,80 +806,203 @@
 
 
 CreateNetworkResponseTypeDef = TypedDict(
     "CreateNetworkResponseTypeDef",
     {
         "network": NetworkTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteNetworkResponseTypeDef = TypedDict(
     "DeleteNetworkResponseTypeDef",
     {
         "network": NetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNetworkResponseTypeDef = TypedDict(
     "GetNetworkResponseTypeDef",
     {
         "network": NetworkTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNetworksResponseTypeDef = TypedDict(
     "ListNetworksResponseTypeDef",
     {
         "networks": List[NetworkTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef = TypedDict(
+    "_RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
+    {
+        "networkArn": str,
+    },
+)
+_OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef = TypedDict(
+    "_OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
+    {
+        "filters": Mapping[DeviceIdentifierFilterKeysType, Sequence[str]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef(
+    _RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
+    _OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
+    {
+        "networkArn": str,
     },
 )
+_OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
+    {
+        "filters": Mapping[NetworkResourceFilterKeysType, Sequence[str]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef(
+    _RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
+    _OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef = TypedDict(
+    "_RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
+    {
+        "networkArn": str,
+    },
+)
+_OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef = TypedDict(
+    "_OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
+    {
+        "filters": Mapping[Literal["STATUS"], Sequence[str]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListNetworkSitesRequestListNetworkSitesPaginateTypeDef(
+    _RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
+    _OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
+):
+    pass
+
+
+ListNetworksRequestListNetworksPaginateTypeDef = TypedDict(
+    "ListNetworksRequestListNetworksPaginateTypeDef",
+    {
+        "filters": Mapping[Literal["STATUS"], Sequence[str]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListOrdersRequestListOrdersPaginateTypeDef = TypedDict(
+    "_RequiredListOrdersRequestListOrdersPaginateTypeDef",
+    {
+        "networkArn": str,
+    },
+)
+_OptionalListOrdersRequestListOrdersPaginateTypeDef = TypedDict(
+    "_OptionalListOrdersRequestListOrdersPaginateTypeDef",
+    {
+        "filters": Mapping[OrderFilterKeysType, Sequence[str]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListOrdersRequestListOrdersPaginateTypeDef(
+    _RequiredListOrdersRequestListOrdersPaginateTypeDef,
+    _OptionalListOrdersRequestListOrdersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredNetworkResourceDefinitionOutputTypeDef = TypedDict(
+    "_RequiredNetworkResourceDefinitionOutputTypeDef",
+    {
+        "count": int,
+        "type": NetworkResourceDefinitionTypeType,
+    },
+)
+_OptionalNetworkResourceDefinitionOutputTypeDef = TypedDict(
+    "_OptionalNetworkResourceDefinitionOutputTypeDef",
+    {
+        "options": List[NameValuePairOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class NetworkResourceDefinitionOutputTypeDef(
+    _RequiredNetworkResourceDefinitionOutputTypeDef, _OptionalNetworkResourceDefinitionOutputTypeDef
+):
+    pass
+
 
 _RequiredNetworkResourceDefinitionTypeDef = TypedDict(
     "_RequiredNetworkResourceDefinitionTypeDef",
     {
         "count": int,
         "type": NetworkResourceDefinitionTypeType,
     },
 )
 _OptionalNetworkResourceDefinitionTypeDef = TypedDict(
     "_OptionalNetworkResourceDefinitionTypeDef",
     {
-        "options": List[NameValuePairTypeDef],
+        "options": Sequence[NameValuePairTypeDef],
     },
     total=False,
 )
 
 
 class NetworkResourceDefinitionTypeDef(
     _RequiredNetworkResourceDefinitionTypeDef, _OptionalNetworkResourceDefinitionTypeDef
 ):
     pass
 
 
 NetworkResourceTypeDef = TypedDict(
     "NetworkResourceTypeDef",
     {
-        "attributes": List[NameValuePairTypeDef],
+        "attributes": List[NameValuePairOutputTypeDef],
         "commitmentInformation": CommitmentInformationTypeDef,
         "createdAt": datetime,
         "description": str,
         "health": HealthStatusType,
         "model": str,
         "networkArn": str,
         "networkResourceArn": str,
         "networkSiteArn": str,
         "orderArn": str,
-        "position": PositionTypeDef,
+        "position": PositionOutputTypeDef,
         "returnInformation": ReturnInformationTypeDef,
         "serialNumber": str,
         "status": NetworkResourceStatusType,
         "statusReason": str,
         "type": Literal["RADIO_UNIT"],
         "vendor": str,
     },
@@ -917,141 +1014,150 @@
     {
         "acknowledgmentStatus": AcknowledgmentStatusType,
         "createdAt": datetime,
         "networkArn": str,
         "networkSiteArn": str,
         "orderArn": str,
         "orderedResources": List[OrderedResourceDefinitionTypeDef],
-        "shippingAddress": AddressTypeDef,
+        "shippingAddress": AddressOutputTypeDef,
         "trackingInformation": List[TrackingInformationTypeDef],
     },
     total=False,
 )
 
+SitePlanOutputTypeDef = TypedDict(
+    "SitePlanOutputTypeDef",
+    {
+        "options": List[NameValuePairOutputTypeDef],
+        "resourceDefinitions": List[NetworkResourceDefinitionOutputTypeDef],
+    },
+    total=False,
+)
+
 SitePlanTypeDef = TypedDict(
     "SitePlanTypeDef",
     {
-        "options": List[NameValuePairTypeDef],
-        "resourceDefinitions": List[NetworkResourceDefinitionTypeDef],
+        "options": Sequence[NameValuePairTypeDef],
+        "resourceDefinitions": Sequence[NetworkResourceDefinitionTypeDef],
     },
     total=False,
 )
 
 ConfigureAccessPointResponseTypeDef = TypedDict(
     "ConfigureAccessPointResponseTypeDef",
     {
         "accessPoint": NetworkResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNetworkResourceResponseTypeDef = TypedDict(
     "GetNetworkResourceResponseTypeDef",
     {
         "networkResource": NetworkResourceTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNetworkResourcesResponseTypeDef = TypedDict(
     "ListNetworkResourcesResponseTypeDef",
     {
         "networkResources": List[NetworkResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartNetworkResourceUpdateResponseTypeDef = TypedDict(
     "StartNetworkResourceUpdateResponseTypeDef",
     {
         "networkResource": NetworkResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AcknowledgeOrderReceiptResponseTypeDef = TypedDict(
     "AcknowledgeOrderReceiptResponseTypeDef",
     {
         "order": OrderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOrderResponseTypeDef = TypedDict(
     "GetOrderResponseTypeDef",
     {
         "order": OrderTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOrdersResponseTypeDef = TypedDict(
     "ListOrdersResponseTypeDef",
     {
         "nextToken": str,
         "orders": List[OrderTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateNetworkSiteRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateNetworkSiteRequestRequestTypeDef",
+_RequiredNetworkSiteTypeDef = TypedDict(
+    "_RequiredNetworkSiteTypeDef",
     {
         "networkArn": str,
+        "networkSiteArn": str,
         "networkSiteName": str,
+        "status": NetworkSiteStatusType,
     },
 )
-_OptionalCreateNetworkSiteRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateNetworkSiteRequestRequestTypeDef",
+_OptionalNetworkSiteTypeDef = TypedDict(
+    "_OptionalNetworkSiteTypeDef",
     {
         "availabilityZone": str,
         "availabilityZoneId": str,
-        "clientToken": str,
+        "createdAt": datetime,
+        "currentPlan": SitePlanOutputTypeDef,
         "description": str,
-        "pendingPlan": SitePlanTypeDef,
-        "tags": Mapping[str, str],
+        "pendingPlan": SitePlanOutputTypeDef,
+        "statusReason": str,
     },
     total=False,
 )
 
 
-class CreateNetworkSiteRequestRequestTypeDef(
-    _RequiredCreateNetworkSiteRequestRequestTypeDef, _OptionalCreateNetworkSiteRequestRequestTypeDef
-):
+class NetworkSiteTypeDef(_RequiredNetworkSiteTypeDef, _OptionalNetworkSiteTypeDef):
     pass
 
 
-_RequiredNetworkSiteTypeDef = TypedDict(
-    "_RequiredNetworkSiteTypeDef",
+_RequiredCreateNetworkSiteRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateNetworkSiteRequestRequestTypeDef",
     {
         "networkArn": str,
-        "networkSiteArn": str,
         "networkSiteName": str,
-        "status": NetworkSiteStatusType,
     },
 )
-_OptionalNetworkSiteTypeDef = TypedDict(
-    "_OptionalNetworkSiteTypeDef",
+_OptionalCreateNetworkSiteRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateNetworkSiteRequestRequestTypeDef",
     {
         "availabilityZone": str,
         "availabilityZoneId": str,
-        "createdAt": datetime,
-        "currentPlan": SitePlanTypeDef,
+        "clientToken": str,
         "description": str,
         "pendingPlan": SitePlanTypeDef,
-        "statusReason": str,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class NetworkSiteTypeDef(_RequiredNetworkSiteTypeDef, _OptionalNetworkSiteTypeDef):
+class CreateNetworkSiteRequestRequestTypeDef(
+    _RequiredCreateNetworkSiteRequestRequestTypeDef, _OptionalCreateNetworkSiteRequestRequestTypeDef
+):
     pass
 
 
 _RequiredUpdateNetworkSitePlanRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNetworkSitePlanRequestRequestTypeDef",
     {
         "networkSiteArn": str,
@@ -1074,54 +1180,54 @@
     pass
 
 
 ActivateNetworkSiteResponseTypeDef = TypedDict(
     "ActivateNetworkSiteResponseTypeDef",
     {
         "networkSite": NetworkSiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateNetworkSiteResponseTypeDef = TypedDict(
     "CreateNetworkSiteResponseTypeDef",
     {
         "networkSite": NetworkSiteTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteNetworkSiteResponseTypeDef = TypedDict(
     "DeleteNetworkSiteResponseTypeDef",
     {
         "networkSite": NetworkSiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNetworkSiteResponseTypeDef = TypedDict(
     "GetNetworkSiteResponseTypeDef",
     {
         "networkSite": NetworkSiteTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNetworkSitesResponseTypeDef = TypedDict(
     "ListNetworkSitesResponseTypeDef",
     {
         "networkSites": List[NetworkSiteTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNetworkSiteResponseTypeDef = TypedDict(
     "UpdateNetworkSiteResponseTypeDef",
     {
         "networkSite": NetworkSiteTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks/type_defs.pyi` & `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -38,76 +38,82 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcknowledgeOrderReceiptRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ActivateDeviceIdentifierRequestRequestTypeDef",
     "DeviceIdentifierTypeDef",
     "AddressTypeDef",
     "CommitmentConfigurationTypeDef",
+    "AddressOutputTypeDef",
+    "CommitmentConfigurationOutputTypeDef",
     "PositionTypeDef",
     "CreateNetworkRequestRequestTypeDef",
     "NetworkTypeDef",
     "DeactivateDeviceIdentifierRequestRequestTypeDef",
     "DeleteNetworkRequestRequestTypeDef",
     "DeleteNetworkSiteRequestRequestTypeDef",
     "GetDeviceIdentifierRequestRequestTypeDef",
     "GetNetworkRequestRequestTypeDef",
     "GetNetworkResourceRequestRequestTypeDef",
     "GetNetworkSiteRequestRequestTypeDef",
     "GetOrderRequestRequestTypeDef",
-    "ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDeviceIdentifiersRequestRequestTypeDef",
-    "ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
     "ListNetworkResourcesRequestRequestTypeDef",
-    "ListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
     "ListNetworkSitesRequestRequestTypeDef",
-    "ListNetworksRequestListNetworksPaginateTypeDef",
     "ListNetworksRequestRequestTypeDef",
-    "ListOrdersRequestListOrdersPaginateTypeDef",
     "ListOrdersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "NameValuePairOutputTypeDef",
     "NameValuePairTypeDef",
+    "PositionOutputTypeDef",
     "TrackingInformationTypeDef",
-    "PaginatorConfigTypeDef",
-    "PingResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateNetworkSiteRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PingResponseTypeDef",
     "ActivateDeviceIdentifierResponseTypeDef",
     "DeactivateDeviceIdentifierResponseTypeDef",
     "GetDeviceIdentifierResponseTypeDef",
     "ListDeviceIdentifiersResponseTypeDef",
-    "ReturnInformationTypeDef",
     "ActivateNetworkSiteRequestRequestTypeDef",
+    "StartNetworkResourceUpdateRequestRequestTypeDef",
+    "ReturnInformationTypeDef",
     "CommitmentInformationTypeDef",
     "OrderedResourceDefinitionTypeDef",
-    "StartNetworkResourceUpdateRequestRequestTypeDef",
     "ConfigureAccessPointRequestRequestTypeDef",
     "CreateNetworkResponseTypeDef",
     "DeleteNetworkResponseTypeDef",
     "GetNetworkResponseTypeDef",
     "ListNetworksResponseTypeDef",
+    "ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
+    "ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
+    "ListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
+    "ListNetworksRequestListNetworksPaginateTypeDef",
+    "ListOrdersRequestListOrdersPaginateTypeDef",
+    "NetworkResourceDefinitionOutputTypeDef",
     "NetworkResourceDefinitionTypeDef",
     "NetworkResourceTypeDef",
     "OrderTypeDef",
+    "SitePlanOutputTypeDef",
     "SitePlanTypeDef",
     "ConfigureAccessPointResponseTypeDef",
     "GetNetworkResourceResponseTypeDef",
     "ListNetworkResourcesResponseTypeDef",
     "StartNetworkResourceUpdateResponseTypeDef",
     "AcknowledgeOrderReceiptResponseTypeDef",
     "GetOrderResponseTypeDef",
     "ListOrdersResponseTypeDef",
-    "CreateNetworkSiteRequestRequestTypeDef",
     "NetworkSiteTypeDef",
+    "CreateNetworkSiteRequestRequestTypeDef",
     "UpdateNetworkSitePlanRequestRequestTypeDef",
     "ActivateNetworkSiteResponseTypeDef",
     "CreateNetworkSiteResponseTypeDef",
     "DeleteNetworkSiteResponseTypeDef",
     "GetNetworkSiteResponseTypeDef",
     "ListNetworkSitesResponseTypeDef",
     "UpdateNetworkSiteResponseTypeDef",
@@ -116,14 +122,25 @@
 AcknowledgeOrderReceiptRequestRequestTypeDef = TypedDict(
     "AcknowledgeOrderReceiptRequestRequestTypeDef",
     {
         "orderArn": str,
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
 _RequiredActivateDeviceIdentifierRequestRequestTypeDef = TypedDict(
     "_RequiredActivateDeviceIdentifierRequestRequestTypeDef",
     {
         "deviceIdentifierArn": str,
     },
 )
 _OptionalActivateDeviceIdentifierRequestRequestTypeDef = TypedDict(
@@ -186,14 +203,48 @@
     "CommitmentConfigurationTypeDef",
     {
         "automaticRenewal": bool,
         "commitmentLength": CommitmentLengthType,
     },
 )
 
+_RequiredAddressOutputTypeDef = TypedDict(
+    "_RequiredAddressOutputTypeDef",
+    {
+        "city": str,
+        "country": str,
+        "name": str,
+        "postalCode": str,
+        "stateOrProvince": str,
+        "street1": str,
+    },
+)
+_OptionalAddressOutputTypeDef = TypedDict(
+    "_OptionalAddressOutputTypeDef",
+    {
+        "company": str,
+        "emailAddress": str,
+        "phoneNumber": str,
+        "street2": str,
+        "street3": str,
+    },
+    total=False,
+)
+
+class AddressOutputTypeDef(_RequiredAddressOutputTypeDef, _OptionalAddressOutputTypeDef):
+    pass
+
+CommitmentConfigurationOutputTypeDef = TypedDict(
+    "CommitmentConfigurationOutputTypeDef",
+    {
+        "automaticRenewal": bool,
+        "commitmentLength": CommitmentLengthType,
+    },
+)
+
 PositionTypeDef = TypedDict(
     "PositionTypeDef",
     {
         "elevation": float,
         "elevationReference": ElevationReferenceType,
         "elevationUnit": Literal["FEET"],
         "latitude": float,
@@ -333,35 +384,24 @@
 GetOrderRequestRequestTypeDef = TypedDict(
     "GetOrderRequestRequestTypeDef",
     {
         "orderArn": str,
     },
 )
 
-_RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef = TypedDict(
-    "_RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
-    {
-        "networkArn": str,
-    },
-)
-_OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef = TypedDict(
-    "_OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "filters": Mapping[DeviceIdentifierFilterKeysType, Sequence[str]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef(
-    _RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
-    _OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
-):
-    pass
-
 _RequiredListDeviceIdentifiersRequestRequestTypeDef = TypedDict(
     "_RequiredListDeviceIdentifiersRequestRequestTypeDef",
     {
         "networkArn": str,
     },
 )
 _OptionalListDeviceIdentifiersRequestRequestTypeDef = TypedDict(
@@ -376,35 +416,14 @@
 
 class ListDeviceIdentifiersRequestRequestTypeDef(
     _RequiredListDeviceIdentifiersRequestRequestTypeDef,
     _OptionalListDeviceIdentifiersRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
-    {
-        "networkArn": str,
-    },
-)
-_OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
-    {
-        "filters": Mapping[NetworkResourceFilterKeysType, Sequence[str]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef(
-    _RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
-    _OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredListNetworkResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListNetworkResourcesRequestRequestTypeDef",
     {
         "networkArn": str,
     },
 )
 _OptionalListNetworkResourcesRequestRequestTypeDef = TypedDict(
@@ -419,35 +438,14 @@
 
 class ListNetworkResourcesRequestRequestTypeDef(
     _RequiredListNetworkResourcesRequestRequestTypeDef,
     _OptionalListNetworkResourcesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef = TypedDict(
-    "_RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
-    {
-        "networkArn": str,
-    },
-)
-_OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef = TypedDict(
-    "_OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
-    {
-        "filters": Mapping[Literal["STATUS"], Sequence[str]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListNetworkSitesRequestListNetworkSitesPaginateTypeDef(
-    _RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
-    _OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
-):
-    pass
-
 _RequiredListNetworkSitesRequestRequestTypeDef = TypedDict(
     "_RequiredListNetworkSitesRequestRequestTypeDef",
     {
         "networkArn": str,
     },
 )
 _OptionalListNetworkSitesRequestRequestTypeDef = TypedDict(
@@ -461,54 +459,24 @@
 )
 
 class ListNetworkSitesRequestRequestTypeDef(
     _RequiredListNetworkSitesRequestRequestTypeDef, _OptionalListNetworkSitesRequestRequestTypeDef
 ):
     pass
 
-ListNetworksRequestListNetworksPaginateTypeDef = TypedDict(
-    "ListNetworksRequestListNetworksPaginateTypeDef",
-    {
-        "filters": Mapping[Literal["STATUS"], Sequence[str]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListNetworksRequestRequestTypeDef = TypedDict(
     "ListNetworksRequestRequestTypeDef",
     {
         "filters": Mapping[Literal["STATUS"], Sequence[str]],
         "maxResults": int,
         "startToken": str,
     },
     total=False,
 )
 
-_RequiredListOrdersRequestListOrdersPaginateTypeDef = TypedDict(
-    "_RequiredListOrdersRequestListOrdersPaginateTypeDef",
-    {
-        "networkArn": str,
-    },
-)
-_OptionalListOrdersRequestListOrdersPaginateTypeDef = TypedDict(
-    "_OptionalListOrdersRequestListOrdersPaginateTypeDef",
-    {
-        "filters": Mapping[OrderFilterKeysType, Sequence[str]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListOrdersRequestListOrdersPaginateTypeDef(
-    _RequiredListOrdersRequestListOrdersPaginateTypeDef,
-    _OptionalListOrdersRequestListOrdersPaginateTypeDef,
-):
-    pass
-
 _RequiredListOrdersRequestRequestTypeDef = TypedDict(
     "_RequiredListOrdersRequestRequestTypeDef",
     {
         "networkArn": str,
     },
 )
 _OptionalListOrdersRequestRequestTypeDef = TypedDict(
@@ -529,22 +497,33 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_RequiredNameValuePairOutputTypeDef = TypedDict(
+    "_RequiredNameValuePairOutputTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+    },
+)
+_OptionalNameValuePairOutputTypeDef = TypedDict(
+    "_OptionalNameValuePairOutputTypeDef",
+    {
+        "value": str,
     },
+    total=False,
 )
 
+class NameValuePairOutputTypeDef(
+    _RequiredNameValuePairOutputTypeDef, _OptionalNameValuePairOutputTypeDef
+):
+    pass
+
 _RequiredNameValuePairTypeDef = TypedDict(
     "_RequiredNameValuePairTypeDef",
     {
         "name": str,
     },
 )
 _OptionalNameValuePairTypeDef = TypedDict(
@@ -554,51 +533,34 @@
     },
     total=False,
 )
 
 class NameValuePairTypeDef(_RequiredNameValuePairTypeDef, _OptionalNameValuePairTypeDef):
     pass
 
-TrackingInformationTypeDef = TypedDict(
-    "TrackingInformationTypeDef",
+PositionOutputTypeDef = TypedDict(
+    "PositionOutputTypeDef",
     {
-        "trackingNumber": str,
+        "elevation": float,
+        "elevationReference": ElevationReferenceType,
+        "elevationUnit": Literal["FEET"],
+        "latitude": float,
+        "longitude": float,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+TrackingInformationTypeDef = TypedDict(
+    "TrackingInformationTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "trackingNumber": str,
     },
     total=False,
 )
 
-PingResponseTypeDef = TypedDict(
-    "PingResponseTypeDef",
-    {
-        "status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
@@ -627,58 +589,63 @@
 )
 
 class UpdateNetworkSiteRequestRequestTypeDef(
     _RequiredUpdateNetworkSiteRequestRequestTypeDef, _OptionalUpdateNetworkSiteRequestRequestTypeDef
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PingResponseTypeDef = TypedDict(
+    "PingResponseTypeDef",
+    {
+        "status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ActivateDeviceIdentifierResponseTypeDef = TypedDict(
     "ActivateDeviceIdentifierResponseTypeDef",
     {
         "deviceIdentifier": DeviceIdentifierTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeactivateDeviceIdentifierResponseTypeDef = TypedDict(
     "DeactivateDeviceIdentifierResponseTypeDef",
     {
         "deviceIdentifier": DeviceIdentifierTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeviceIdentifierResponseTypeDef = TypedDict(
     "GetDeviceIdentifierResponseTypeDef",
     {
         "deviceIdentifier": DeviceIdentifierTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeviceIdentifiersResponseTypeDef = TypedDict(
     "ListDeviceIdentifiersResponseTypeDef",
     {
         "deviceIdentifiers": List[DeviceIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ReturnInformationTypeDef = TypedDict(
-    "ReturnInformationTypeDef",
-    {
-        "replacementOrderArn": str,
-        "returnReason": str,
-        "shippingAddress": AddressTypeDef,
-        "shippingLabel": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredActivateNetworkSiteRequestRequestTypeDef = TypedDict(
     "_RequiredActivateNetworkSiteRequestRequestTypeDef",
     {
         "networkSiteArn": str,
         "shippingAddress": AddressTypeDef,
@@ -695,18 +662,52 @@
 
 class ActivateNetworkSiteRequestRequestTypeDef(
     _RequiredActivateNetworkSiteRequestRequestTypeDef,
     _OptionalActivateNetworkSiteRequestRequestTypeDef,
 ):
     pass
 
+_RequiredStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
+    "_RequiredStartNetworkResourceUpdateRequestRequestTypeDef",
+    {
+        "networkResourceArn": str,
+        "updateType": UpdateTypeType,
+    },
+)
+_OptionalStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
+    "_OptionalStartNetworkResourceUpdateRequestRequestTypeDef",
+    {
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
+        "returnReason": str,
+        "shippingAddress": AddressTypeDef,
+    },
+    total=False,
+)
+
+class StartNetworkResourceUpdateRequestRequestTypeDef(
+    _RequiredStartNetworkResourceUpdateRequestRequestTypeDef,
+    _OptionalStartNetworkResourceUpdateRequestRequestTypeDef,
+):
+    pass
+
+ReturnInformationTypeDef = TypedDict(
+    "ReturnInformationTypeDef",
+    {
+        "replacementOrderArn": str,
+        "returnReason": str,
+        "shippingAddress": AddressOutputTypeDef,
+        "shippingLabel": str,
+    },
+    total=False,
+)
+
 _RequiredCommitmentInformationTypeDef = TypedDict(
     "_RequiredCommitmentInformationTypeDef",
     {
-        "commitmentConfiguration": CommitmentConfigurationTypeDef,
+        "commitmentConfiguration": CommitmentConfigurationOutputTypeDef,
     },
 )
 _OptionalCommitmentInformationTypeDef = TypedDict(
     "_OptionalCommitmentInformationTypeDef",
     {
         "expiresOn": datetime,
         "startAt": datetime,
@@ -725,47 +726,24 @@
         "count": int,
         "type": NetworkResourceDefinitionTypeType,
     },
 )
 _OptionalOrderedResourceDefinitionTypeDef = TypedDict(
     "_OptionalOrderedResourceDefinitionTypeDef",
     {
-        "commitmentConfiguration": CommitmentConfigurationTypeDef,
+        "commitmentConfiguration": CommitmentConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 class OrderedResourceDefinitionTypeDef(
     _RequiredOrderedResourceDefinitionTypeDef, _OptionalOrderedResourceDefinitionTypeDef
 ):
     pass
 
-_RequiredStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
-    "_RequiredStartNetworkResourceUpdateRequestRequestTypeDef",
-    {
-        "networkResourceArn": str,
-        "updateType": UpdateTypeType,
-    },
-)
-_OptionalStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
-    "_OptionalStartNetworkResourceUpdateRequestRequestTypeDef",
-    {
-        "commitmentConfiguration": CommitmentConfigurationTypeDef,
-        "returnReason": str,
-        "shippingAddress": AddressTypeDef,
-    },
-    total=False,
-)
-
-class StartNetworkResourceUpdateRequestRequestTypeDef(
-    _RequiredStartNetworkResourceUpdateRequestRequestTypeDef,
-    _OptionalStartNetworkResourceUpdateRequestRequestTypeDef,
-):
-    pass
-
 _RequiredConfigureAccessPointRequestRequestTypeDef = TypedDict(
     "_RequiredConfigureAccessPointRequestRequestTypeDef",
     {
         "accessPointArn": str,
     },
 )
 _OptionalConfigureAccessPointRequestRequestTypeDef = TypedDict(
@@ -787,78 +765,191 @@
     pass
 
 CreateNetworkResponseTypeDef = TypedDict(
     "CreateNetworkResponseTypeDef",
     {
         "network": NetworkTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteNetworkResponseTypeDef = TypedDict(
     "DeleteNetworkResponseTypeDef",
     {
         "network": NetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNetworkResponseTypeDef = TypedDict(
     "GetNetworkResponseTypeDef",
     {
         "network": NetworkTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNetworksResponseTypeDef = TypedDict(
     "ListNetworksResponseTypeDef",
     {
         "networks": List[NetworkTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef = TypedDict(
+    "_RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
+    {
+        "networkArn": str,
+    },
+)
+_OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef = TypedDict(
+    "_OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
+    {
+        "filters": Mapping[DeviceIdentifierFilterKeysType, Sequence[str]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef(
+    _RequiredListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
+    _OptionalListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
+):
+    pass
+
+_RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
+    {
+        "networkArn": str,
+    },
+)
+_OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
+    {
+        "filters": Mapping[NetworkResourceFilterKeysType, Sequence[str]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef(
+    _RequiredListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
+    _OptionalListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
+):
+    pass
+
+_RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef = TypedDict(
+    "_RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
+    {
+        "networkArn": str,
+    },
+)
+_OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef = TypedDict(
+    "_OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
+    {
+        "filters": Mapping[Literal["STATUS"], Sequence[str]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListNetworkSitesRequestListNetworkSitesPaginateTypeDef(
+    _RequiredListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
+    _OptionalListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
+):
+    pass
+
+ListNetworksRequestListNetworksPaginateTypeDef = TypedDict(
+    "ListNetworksRequestListNetworksPaginateTypeDef",
+    {
+        "filters": Mapping[Literal["STATUS"], Sequence[str]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListOrdersRequestListOrdersPaginateTypeDef = TypedDict(
+    "_RequiredListOrdersRequestListOrdersPaginateTypeDef",
+    {
+        "networkArn": str,
+    },
+)
+_OptionalListOrdersRequestListOrdersPaginateTypeDef = TypedDict(
+    "_OptionalListOrdersRequestListOrdersPaginateTypeDef",
+    {
+        "filters": Mapping[OrderFilterKeysType, Sequence[str]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListOrdersRequestListOrdersPaginateTypeDef(
+    _RequiredListOrdersRequestListOrdersPaginateTypeDef,
+    _OptionalListOrdersRequestListOrdersPaginateTypeDef,
+):
+    pass
+
+_RequiredNetworkResourceDefinitionOutputTypeDef = TypedDict(
+    "_RequiredNetworkResourceDefinitionOutputTypeDef",
+    {
+        "count": int,
+        "type": NetworkResourceDefinitionTypeType,
     },
 )
+_OptionalNetworkResourceDefinitionOutputTypeDef = TypedDict(
+    "_OptionalNetworkResourceDefinitionOutputTypeDef",
+    {
+        "options": List[NameValuePairOutputTypeDef],
+    },
+    total=False,
+)
+
+class NetworkResourceDefinitionOutputTypeDef(
+    _RequiredNetworkResourceDefinitionOutputTypeDef, _OptionalNetworkResourceDefinitionOutputTypeDef
+):
+    pass
 
 _RequiredNetworkResourceDefinitionTypeDef = TypedDict(
     "_RequiredNetworkResourceDefinitionTypeDef",
     {
         "count": int,
         "type": NetworkResourceDefinitionTypeType,
     },
 )
 _OptionalNetworkResourceDefinitionTypeDef = TypedDict(
     "_OptionalNetworkResourceDefinitionTypeDef",
     {
-        "options": List[NameValuePairTypeDef],
+        "options": Sequence[NameValuePairTypeDef],
     },
     total=False,
 )
 
 class NetworkResourceDefinitionTypeDef(
     _RequiredNetworkResourceDefinitionTypeDef, _OptionalNetworkResourceDefinitionTypeDef
 ):
     pass
 
 NetworkResourceTypeDef = TypedDict(
     "NetworkResourceTypeDef",
     {
-        "attributes": List[NameValuePairTypeDef],
+        "attributes": List[NameValuePairOutputTypeDef],
         "commitmentInformation": CommitmentInformationTypeDef,
         "createdAt": datetime,
         "description": str,
         "health": HealthStatusType,
         "model": str,
         "networkArn": str,
         "networkResourceArn": str,
         "networkSiteArn": str,
         "orderArn": str,
-        "position": PositionTypeDef,
+        "position": PositionOutputTypeDef,
         "returnInformation": ReturnInformationTypeDef,
         "serialNumber": str,
         "status": NetworkResourceStatusType,
         "statusReason": str,
         "type": Literal["RADIO_UNIT"],
         "vendor": str,
     },
@@ -870,138 +961,147 @@
     {
         "acknowledgmentStatus": AcknowledgmentStatusType,
         "createdAt": datetime,
         "networkArn": str,
         "networkSiteArn": str,
         "orderArn": str,
         "orderedResources": List[OrderedResourceDefinitionTypeDef],
-        "shippingAddress": AddressTypeDef,
+        "shippingAddress": AddressOutputTypeDef,
         "trackingInformation": List[TrackingInformationTypeDef],
     },
     total=False,
 )
 
+SitePlanOutputTypeDef = TypedDict(
+    "SitePlanOutputTypeDef",
+    {
+        "options": List[NameValuePairOutputTypeDef],
+        "resourceDefinitions": List[NetworkResourceDefinitionOutputTypeDef],
+    },
+    total=False,
+)
+
 SitePlanTypeDef = TypedDict(
     "SitePlanTypeDef",
     {
-        "options": List[NameValuePairTypeDef],
-        "resourceDefinitions": List[NetworkResourceDefinitionTypeDef],
+        "options": Sequence[NameValuePairTypeDef],
+        "resourceDefinitions": Sequence[NetworkResourceDefinitionTypeDef],
     },
     total=False,
 )
 
 ConfigureAccessPointResponseTypeDef = TypedDict(
     "ConfigureAccessPointResponseTypeDef",
     {
         "accessPoint": NetworkResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNetworkResourceResponseTypeDef = TypedDict(
     "GetNetworkResourceResponseTypeDef",
     {
         "networkResource": NetworkResourceTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNetworkResourcesResponseTypeDef = TypedDict(
     "ListNetworkResourcesResponseTypeDef",
     {
         "networkResources": List[NetworkResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartNetworkResourceUpdateResponseTypeDef = TypedDict(
     "StartNetworkResourceUpdateResponseTypeDef",
     {
         "networkResource": NetworkResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AcknowledgeOrderReceiptResponseTypeDef = TypedDict(
     "AcknowledgeOrderReceiptResponseTypeDef",
     {
         "order": OrderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOrderResponseTypeDef = TypedDict(
     "GetOrderResponseTypeDef",
     {
         "order": OrderTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOrdersResponseTypeDef = TypedDict(
     "ListOrdersResponseTypeDef",
     {
         "nextToken": str,
         "orders": List[OrderTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateNetworkSiteRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateNetworkSiteRequestRequestTypeDef",
+_RequiredNetworkSiteTypeDef = TypedDict(
+    "_RequiredNetworkSiteTypeDef",
     {
         "networkArn": str,
+        "networkSiteArn": str,
         "networkSiteName": str,
+        "status": NetworkSiteStatusType,
     },
 )
-_OptionalCreateNetworkSiteRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateNetworkSiteRequestRequestTypeDef",
+_OptionalNetworkSiteTypeDef = TypedDict(
+    "_OptionalNetworkSiteTypeDef",
     {
         "availabilityZone": str,
         "availabilityZoneId": str,
-        "clientToken": str,
+        "createdAt": datetime,
+        "currentPlan": SitePlanOutputTypeDef,
         "description": str,
-        "pendingPlan": SitePlanTypeDef,
-        "tags": Mapping[str, str],
+        "pendingPlan": SitePlanOutputTypeDef,
+        "statusReason": str,
     },
     total=False,
 )
 
-class CreateNetworkSiteRequestRequestTypeDef(
-    _RequiredCreateNetworkSiteRequestRequestTypeDef, _OptionalCreateNetworkSiteRequestRequestTypeDef
-):
+class NetworkSiteTypeDef(_RequiredNetworkSiteTypeDef, _OptionalNetworkSiteTypeDef):
     pass
 
-_RequiredNetworkSiteTypeDef = TypedDict(
-    "_RequiredNetworkSiteTypeDef",
+_RequiredCreateNetworkSiteRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateNetworkSiteRequestRequestTypeDef",
     {
         "networkArn": str,
-        "networkSiteArn": str,
         "networkSiteName": str,
-        "status": NetworkSiteStatusType,
     },
 )
-_OptionalNetworkSiteTypeDef = TypedDict(
-    "_OptionalNetworkSiteTypeDef",
+_OptionalCreateNetworkSiteRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateNetworkSiteRequestRequestTypeDef",
     {
         "availabilityZone": str,
         "availabilityZoneId": str,
-        "createdAt": datetime,
-        "currentPlan": SitePlanTypeDef,
+        "clientToken": str,
         "description": str,
         "pendingPlan": SitePlanTypeDef,
-        "statusReason": str,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class NetworkSiteTypeDef(_RequiredNetworkSiteTypeDef, _OptionalNetworkSiteTypeDef):
+class CreateNetworkSiteRequestRequestTypeDef(
+    _RequiredCreateNetworkSiteRequestRequestTypeDef, _OptionalCreateNetworkSiteRequestRequestTypeDef
+):
     pass
 
 _RequiredUpdateNetworkSitePlanRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNetworkSitePlanRequestRequestTypeDef",
     {
         "networkSiteArn": str,
         "pendingPlan": SitePlanTypeDef,
@@ -1021,54 +1121,54 @@
 ):
     pass
 
 ActivateNetworkSiteResponseTypeDef = TypedDict(
     "ActivateNetworkSiteResponseTypeDef",
     {
         "networkSite": NetworkSiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateNetworkSiteResponseTypeDef = TypedDict(
     "CreateNetworkSiteResponseTypeDef",
     {
         "networkSite": NetworkSiteTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteNetworkSiteResponseTypeDef = TypedDict(
     "DeleteNetworkSiteResponseTypeDef",
     {
         "networkSite": NetworkSiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNetworkSiteResponseTypeDef = TypedDict(
     "GetNetworkSiteResponseTypeDef",
     {
         "networkSite": NetworkSiteTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNetworkSitesResponseTypeDef = TypedDict(
     "ListNetworkSitesResponseTypeDef",
     {
         "networkSites": List[NetworkSiteTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNetworkSiteResponseTypeDef = TypedDict(
     "UpdateNetworkSiteResponseTypeDef",
     {
         "networkSite": NetworkSiteTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks.egg-info/PKG-INFO` & `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-privatenetworks
-Version: 1.28.0
-Summary: Type annotations for boto3.Private5G 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Private5G 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-privatenetworks"></a>
 
 # mypy-boto3-privatenetworks
 
 [![PyPI - mypy-boto3-privatenetworks](https://img.shields.io/pypi/v/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-privatenetworks?color=blue)](https://pypistats.org/packages/mypy-boto3-privatenetworks)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-privatenetworks)](https://pepy.tech/project/mypy-boto3-privatenetworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Private5G 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
+[boto3.Private5G 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
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
 [mypy-boto3-privatenetworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,76 +354,82 @@
 
 `mypy_boto3_privatenetworks.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_privatenetworks.type_defs import (
     AcknowledgeOrderReceiptRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ActivateDeviceIdentifierRequestRequestTypeDef,
     DeviceIdentifierTypeDef,
     AddressTypeDef,
     CommitmentConfigurationTypeDef,
+    AddressOutputTypeDef,
+    CommitmentConfigurationOutputTypeDef,
     PositionTypeDef,
     CreateNetworkRequestRequestTypeDef,
     NetworkTypeDef,
     DeactivateDeviceIdentifierRequestRequestTypeDef,
     DeleteNetworkRequestRequestTypeDef,
     DeleteNetworkSiteRequestRequestTypeDef,
     GetDeviceIdentifierRequestRequestTypeDef,
     GetNetworkRequestRequestTypeDef,
     GetNetworkResourceRequestRequestTypeDef,
     GetNetworkSiteRequestRequestTypeDef,
     GetOrderRequestRequestTypeDef,
-    ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDeviceIdentifiersRequestRequestTypeDef,
-    ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
     ListNetworkResourcesRequestRequestTypeDef,
-    ListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
     ListNetworkSitesRequestRequestTypeDef,
-    ListNetworksRequestListNetworksPaginateTypeDef,
     ListNetworksRequestRequestTypeDef,
-    ListOrdersRequestListOrdersPaginateTypeDef,
     ListOrdersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    NameValuePairOutputTypeDef,
     NameValuePairTypeDef,
+    PositionOutputTypeDef,
     TrackingInformationTypeDef,
-    PaginatorConfigTypeDef,
-    PingResponseTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateNetworkSiteRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PingResponseTypeDef,
     ActivateDeviceIdentifierResponseTypeDef,
     DeactivateDeviceIdentifierResponseTypeDef,
     GetDeviceIdentifierResponseTypeDef,
     ListDeviceIdentifiersResponseTypeDef,
-    ReturnInformationTypeDef,
     ActivateNetworkSiteRequestRequestTypeDef,
+    StartNetworkResourceUpdateRequestRequestTypeDef,
+    ReturnInformationTypeDef,
     CommitmentInformationTypeDef,
     OrderedResourceDefinitionTypeDef,
-    StartNetworkResourceUpdateRequestRequestTypeDef,
     ConfigureAccessPointRequestRequestTypeDef,
     CreateNetworkResponseTypeDef,
     DeleteNetworkResponseTypeDef,
     GetNetworkResponseTypeDef,
     ListNetworksResponseTypeDef,
+    ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
+    ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
+    ListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
+    ListNetworksRequestListNetworksPaginateTypeDef,
+    ListOrdersRequestListOrdersPaginateTypeDef,
+    NetworkResourceDefinitionOutputTypeDef,
     NetworkResourceDefinitionTypeDef,
     NetworkResourceTypeDef,
     OrderTypeDef,
+    SitePlanOutputTypeDef,
     SitePlanTypeDef,
     ConfigureAccessPointResponseTypeDef,
     GetNetworkResourceResponseTypeDef,
     ListNetworkResourcesResponseTypeDef,
     StartNetworkResourceUpdateResponseTypeDef,
     AcknowledgeOrderReceiptResponseTypeDef,
     GetOrderResponseTypeDef,
     ListOrdersResponseTypeDef,
-    CreateNetworkSiteRequestRequestTypeDef,
     NetworkSiteTypeDef,
+    CreateNetworkSiteRequestRequestTypeDef,
     UpdateNetworkSitePlanRequestRequestTypeDef,
     ActivateNetworkSiteResponseTypeDef,
     CreateNetworkSiteResponseTypeDef,
     DeleteNetworkSiteResponseTypeDef,
     GetNetworkSiteResponseTypeDef,
     ListNetworkSitesResponseTypeDef,
     UpdateNetworkSiteResponseTypeDef,
```

### Comparing `mypy-boto3-privatenetworks-1.28.0/mypy_boto3_privatenetworks.egg-info/SOURCES.txt` & `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.0/setup.py` & `mypy-boto3-privatenetworks-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-privatenetworks",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_privatenetworks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Private5G 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Private5G 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

