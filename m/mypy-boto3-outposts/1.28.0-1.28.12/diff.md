# Comparing `tmp/mypy-boto3-outposts-1.28.0.tar.gz` & `tmp/mypy-boto3-outposts-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-outposts-1.28.0.tar", last modified: Thu Jul  6 21:00:15 2023, max compression
+gzip compressed data, was "mypy-boto3-outposts-1.28.12.tar", last modified: Thu Jul 27 11:49:21 2023, max compression
```

## Comparing `mypy-boto3-outposts-1.28.0.tar` & `mypy-boto3-outposts-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:15.958387 mypy-boto3-outposts-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16340 2023-07-06 21:00:15.946387 mypy-boto3-outposts-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:15.938387 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21419 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21380 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-07-06 20:48:59.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-07-06 20:48:59.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-06 20:48:59.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24615 2023-07-06 20:48:59.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:15.946387 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16340 2023-07-06 21:00:15.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 21:00:15.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:15.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:15.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:15.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:00:15.000000 mypy-boto3-outposts-1.28.0/mypy_boto3_outposts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:15.958387 mypy-boto3-outposts-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:48:58.000000 mypy-boto3-outposts-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.817133 mypy-boto3-outposts-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:08.000000 mypy-boto3-outposts-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-07-27 11:49:21.817133 mypy-boto3-outposts-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14909 2023-07-27 11:41:08.000000 mypy-boto3-outposts-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.805132 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-27 11:41:08.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-27 11:41:08.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:41:08.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21419 2023-07-27 11:41:09.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21380 2023-07-27 11:41:09.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-27 11:41:09.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-07-27 11:41:09.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-07-27 11:41:09.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-07-27 11:41:09.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:08.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25858 2023-07-27 11:41:10.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25833 2023-07-27 11:41:09.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:08.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.817133 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-07-27 11:49:21.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 11:49:21.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:21.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:21.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:21.817133 mypy-boto3-outposts-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:41:08.000000 mypy-boto3-outposts-1.28.12/setup.py
```

### Comparing `mypy-boto3-outposts-1.28.0/LICENSE` & `mypy-boto3-outposts-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.28.0/PKG-INFO` & `mypy-boto3-outposts-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-outposts
-Version: 1.28.0
-Summary: Type annotations for boto3.Outposts 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Outposts 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-outposts"></a>
 
 # mypy-boto3-outposts
 
 [![PyPI - mypy-boto3-outposts](https://img.shields.io/pypi/v/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-outposts?color=blue)](https://pypistats.org/packages/mypy-boto3-outposts)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-outposts)](https://pepy.tech/project/mypy-boto3-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Outposts 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
+[boto3.Outposts 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
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
 [mypy-boto3-outposts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -360,90 +360,92 @@
 ### Typed dictionaries
 
 `mypy_boto3_outposts.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_outposts.type_defs import (
+    AddressOutputTypeDef,
     AddressTypeDef,
     AssetLocationTypeDef,
     ComputeAttributesTypeDef,
     CancelOrderInputRequestTypeDef,
     EC2CapacityTypeDef,
     ConnectionDetailsTypeDef,
     LineItemRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateOutpostInputRequestTypeDef,
     OutpostTypeDef,
     RackPhysicalPropertiesTypeDef,
     DeleteOutpostInputRequestTypeDef,
     DeleteSiteInputRequestTypeDef,
     GetCatalogItemInputRequestTypeDef,
     GetConnectionRequestRequestTypeDef,
     GetOrderInputRequestTypeDef,
     GetOutpostInputRequestTypeDef,
-    GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetOutpostInstanceTypesInputRequestTypeDef,
     InstanceTypeItemTypeDef,
     GetSiteAddressInputRequestTypeDef,
     GetSiteInputRequestTypeDef,
     LineItemAssetInformationTypeDef,
     ShipmentInformationTypeDef,
-    ListAssetsInputListAssetsPaginateTypeDef,
     ListAssetsInputRequestTypeDef,
-    ListCatalogItemsInputListCatalogItemsPaginateTypeDef,
     ListCatalogItemsInputRequestTypeDef,
-    ListOrdersInputListOrdersPaginateTypeDef,
     ListOrdersInputRequestTypeDef,
     OrderSummaryTypeDef,
-    ListOutpostsInputListOutpostsPaginateTypeDef,
     ListOutpostsInputRequestTypeDef,
-    ListSitesInputListSitesPaginateTypeDef,
     ListSitesInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    RackPhysicalPropertiesOutputTypeDef,
     StartConnectionRequestRequestTypeDef,
-    StartConnectionResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateOutpostInputRequestTypeDef,
     UpdateSiteInputRequestTypeDef,
     UpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
-    GetSiteAddressOutputTypeDef,
     UpdateSiteAddressInputRequestTypeDef,
-    UpdateSiteAddressOutputTypeDef,
     AssetInfoTypeDef,
     CatalogItemTypeDef,
-    GetConnectionResponseTypeDef,
     CreateOrderInputRequestTypeDef,
+    GetConnectionResponseTypeDef,
+    GetSiteAddressOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartConnectionResponseTypeDef,
+    UpdateSiteAddressOutputTypeDef,
     CreateOutpostOutputTypeDef,
     GetOutpostOutputTypeDef,
     ListOutpostsOutputTypeDef,
     UpdateOutpostOutputTypeDef,
     CreateSiteInputRequestTypeDef,
-    SiteTypeDef,
+    GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
+    ListAssetsInputListAssetsPaginateTypeDef,
+    ListCatalogItemsInputListCatalogItemsPaginateTypeDef,
+    ListOrdersInputListOrdersPaginateTypeDef,
+    ListOutpostsInputListOutpostsPaginateTypeDef,
+    ListSitesInputListSitesPaginateTypeDef,
     GetOutpostInstanceTypesOutputTypeDef,
     LineItemTypeDef,
     ListOrdersOutputTypeDef,
+    SiteTypeDef,
     ListAssetsOutputTypeDef,
     GetCatalogItemOutputTypeDef,
     ListCatalogItemsOutputTypeDef,
+    OrderTypeDef,
     CreateSiteOutputTypeDef,
     GetSiteOutputTypeDef,
     ListSitesOutputTypeDef,
     UpdateSiteOutputTypeDef,
     UpdateSiteRackPhysicalPropertiesOutputTypeDef,
-    OrderTypeDef,
     CreateOrderOutputTypeDef,
     GetOrderOutputTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_structure() -> AddressOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-outposts-1.28.0/README.md` & `mypy-boto3-outposts-1.28.12/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-outposts"></a>
 
 # mypy-boto3-outposts
 
 [![PyPI - mypy-boto3-outposts](https://img.shields.io/pypi/v/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-outposts?color=blue)](https://pypistats.org/packages/mypy-boto3-outposts)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-outposts)](https://pepy.tech/project/mypy-boto3-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Outposts 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
+[boto3.Outposts 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
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
 [mypy-boto3-outposts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -328,90 +328,92 @@
 ### Typed dictionaries
 
 `mypy_boto3_outposts.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_outposts.type_defs import (
+    AddressOutputTypeDef,
     AddressTypeDef,
     AssetLocationTypeDef,
     ComputeAttributesTypeDef,
     CancelOrderInputRequestTypeDef,
     EC2CapacityTypeDef,
     ConnectionDetailsTypeDef,
     LineItemRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateOutpostInputRequestTypeDef,
     OutpostTypeDef,
     RackPhysicalPropertiesTypeDef,
     DeleteOutpostInputRequestTypeDef,
     DeleteSiteInputRequestTypeDef,
     GetCatalogItemInputRequestTypeDef,
     GetConnectionRequestRequestTypeDef,
     GetOrderInputRequestTypeDef,
     GetOutpostInputRequestTypeDef,
-    GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetOutpostInstanceTypesInputRequestTypeDef,
     InstanceTypeItemTypeDef,
     GetSiteAddressInputRequestTypeDef,
     GetSiteInputRequestTypeDef,
     LineItemAssetInformationTypeDef,
     ShipmentInformationTypeDef,
-    ListAssetsInputListAssetsPaginateTypeDef,
     ListAssetsInputRequestTypeDef,
-    ListCatalogItemsInputListCatalogItemsPaginateTypeDef,
     ListCatalogItemsInputRequestTypeDef,
-    ListOrdersInputListOrdersPaginateTypeDef,
     ListOrdersInputRequestTypeDef,
     OrderSummaryTypeDef,
-    ListOutpostsInputListOutpostsPaginateTypeDef,
     ListOutpostsInputRequestTypeDef,
-    ListSitesInputListSitesPaginateTypeDef,
     ListSitesInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    RackPhysicalPropertiesOutputTypeDef,
     StartConnectionRequestRequestTypeDef,
-    StartConnectionResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateOutpostInputRequestTypeDef,
     UpdateSiteInputRequestTypeDef,
     UpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
-    GetSiteAddressOutputTypeDef,
     UpdateSiteAddressInputRequestTypeDef,
-    UpdateSiteAddressOutputTypeDef,
     AssetInfoTypeDef,
     CatalogItemTypeDef,
-    GetConnectionResponseTypeDef,
     CreateOrderInputRequestTypeDef,
+    GetConnectionResponseTypeDef,
+    GetSiteAddressOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartConnectionResponseTypeDef,
+    UpdateSiteAddressOutputTypeDef,
     CreateOutpostOutputTypeDef,
     GetOutpostOutputTypeDef,
     ListOutpostsOutputTypeDef,
     UpdateOutpostOutputTypeDef,
     CreateSiteInputRequestTypeDef,
-    SiteTypeDef,
+    GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
+    ListAssetsInputListAssetsPaginateTypeDef,
+    ListCatalogItemsInputListCatalogItemsPaginateTypeDef,
+    ListOrdersInputListOrdersPaginateTypeDef,
+    ListOutpostsInputListOutpostsPaginateTypeDef,
+    ListSitesInputListSitesPaginateTypeDef,
     GetOutpostInstanceTypesOutputTypeDef,
     LineItemTypeDef,
     ListOrdersOutputTypeDef,
+    SiteTypeDef,
     ListAssetsOutputTypeDef,
     GetCatalogItemOutputTypeDef,
     ListCatalogItemsOutputTypeDef,
+    OrderTypeDef,
     CreateSiteOutputTypeDef,
     GetSiteOutputTypeDef,
     ListSitesOutputTypeDef,
     UpdateSiteOutputTypeDef,
     UpdateSiteRackPhysicalPropertiesOutputTypeDef,
-    OrderTypeDef,
     CreateOrderOutputTypeDef,
     GetOrderOutputTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_structure() -> AddressOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/__init__.py` & `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/__init__.pyi` & `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/__main__.py` & `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Outposts 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Outposts 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts\nOther"
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

### Comparing `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/client.py` & `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/client.pyi` & `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/literals.py` & `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,14 +250,15 @@
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
@@ -336,26 +337,28 @@
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

### Comparing `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/literals.pyi` & `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -248,14 +248,15 @@
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
@@ -334,26 +335,28 @@
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

### Comparing `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/paginator.py` & `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 class GetOutpostInstanceTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.GetOutpostInstanceTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#getoutpostinstancetypespaginator)
     """
 
     def paginate(
-        self, *, OutpostId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OutpostId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetOutpostInstanceTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.GetOutpostInstanceTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#getoutpostinstancetypespaginator)
         """
 
 
@@ -87,15 +87,15 @@
 
     def paginate(
         self,
         *,
         OutpostIdentifier: str,
         HostIdFilter: Sequence[str] = ...,
         StatusFilter: Sequence[AssetStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listassetspaginator)
         """
 
 
@@ -107,33 +107,30 @@
 
     def paginate(
         self,
         *,
         ItemClassFilter: Sequence[CatalogItemClassType] = ...,
         SupportedStorageFilter: Sequence[SupportedStorageEnumType] = ...,
         EC2FamilyFilter: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCatalogItemsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListCatalogItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listcatalogitemspaginator)
         """
 
 
 class ListOrdersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListOrders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listorderspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        OutpostIdentifierFilter: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OutpostIdentifierFilter: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOrdersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListOrders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listorderspaginator)
         """
 
 
@@ -145,15 +142,15 @@
 
     def paginate(
         self,
         *,
         LifeCycleStatusFilter: Sequence[str] = ...,
         AvailabilityZoneFilter: Sequence[str] = ...,
         AvailabilityZoneIdFilter: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOutpostsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListOutposts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listoutpostspaginator)
         """
 
 
@@ -165,13 +162,13 @@
 
     def paginate(
         self,
         *,
         OperatingAddressCountryCodeFilter: Sequence[str] = ...,
         OperatingAddressStateOrRegionFilter: Sequence[str] = ...,
         OperatingAddressCityFilter: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSitesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListSites.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listsitespaginator)
         """
```

### Comparing `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/paginator.pyi` & `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 class GetOutpostInstanceTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.GetOutpostInstanceTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#getoutpostinstancetypespaginator)
     """
 
     def paginate(
-        self, *, OutpostId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OutpostId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetOutpostInstanceTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.GetOutpostInstanceTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#getoutpostinstancetypespaginator)
         """
 
 class ListAssetsPaginator(Paginator):
@@ -83,15 +83,15 @@
 
     def paginate(
         self,
         *,
         OutpostIdentifier: str,
         HostIdFilter: Sequence[str] = ...,
         StatusFilter: Sequence[AssetStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listassetspaginator)
         """
 
 class ListCatalogItemsPaginator(Paginator):
@@ -102,32 +102,29 @@
 
     def paginate(
         self,
         *,
         ItemClassFilter: Sequence[CatalogItemClassType] = ...,
         SupportedStorageFilter: Sequence[SupportedStorageEnumType] = ...,
         EC2FamilyFilter: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCatalogItemsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListCatalogItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listcatalogitemspaginator)
         """
 
 class ListOrdersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListOrders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listorderspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        OutpostIdentifierFilter: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OutpostIdentifierFilter: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOrdersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListOrders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listorderspaginator)
         """
 
 class ListOutpostsPaginator(Paginator):
@@ -138,15 +135,15 @@
 
     def paginate(
         self,
         *,
         LifeCycleStatusFilter: Sequence[str] = ...,
         AvailabilityZoneFilter: Sequence[str] = ...,
         AvailabilityZoneIdFilter: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOutpostsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListOutposts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listoutpostspaginator)
         """
 
 class ListSitesPaginator(Paginator):
@@ -157,13 +154,13 @@
 
     def paginate(
         self,
         *,
         OperatingAddressCountryCodeFilter: Sequence[str] = ...,
         OperatingAddressStateOrRegionFilter: Sequence[str] = ...,
         OperatingAddressCityFilter: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSitesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Paginator.ListSites.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/paginators/#listsitespaginator)
         """
```

### Comparing `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/type_defs.py` & `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for outposts service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_outposts.type_defs import AddressTypeDef
+    from mypy_boto3_outposts.type_defs import AddressOutputTypeDef
 
-    data: AddressTypeDef = {...}
+    data: AddressOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -47,88 +47,118 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AddressOutputTypeDef",
     "AddressTypeDef",
     "AssetLocationTypeDef",
     "ComputeAttributesTypeDef",
     "CancelOrderInputRequestTypeDef",
     "EC2CapacityTypeDef",
     "ConnectionDetailsTypeDef",
     "LineItemRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateOutpostInputRequestTypeDef",
     "OutpostTypeDef",
     "RackPhysicalPropertiesTypeDef",
     "DeleteOutpostInputRequestTypeDef",
     "DeleteSiteInputRequestTypeDef",
     "GetCatalogItemInputRequestTypeDef",
     "GetConnectionRequestRequestTypeDef",
     "GetOrderInputRequestTypeDef",
     "GetOutpostInputRequestTypeDef",
-    "GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetOutpostInstanceTypesInputRequestTypeDef",
     "InstanceTypeItemTypeDef",
     "GetSiteAddressInputRequestTypeDef",
     "GetSiteInputRequestTypeDef",
     "LineItemAssetInformationTypeDef",
     "ShipmentInformationTypeDef",
-    "ListAssetsInputListAssetsPaginateTypeDef",
     "ListAssetsInputRequestTypeDef",
-    "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
     "ListCatalogItemsInputRequestTypeDef",
-    "ListOrdersInputListOrdersPaginateTypeDef",
     "ListOrdersInputRequestTypeDef",
     "OrderSummaryTypeDef",
-    "ListOutpostsInputListOutpostsPaginateTypeDef",
     "ListOutpostsInputRequestTypeDef",
-    "ListSitesInputListSitesPaginateTypeDef",
     "ListSitesInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "RackPhysicalPropertiesOutputTypeDef",
     "StartConnectionRequestRequestTypeDef",
-    "StartConnectionResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateOutpostInputRequestTypeDef",
     "UpdateSiteInputRequestTypeDef",
     "UpdateSiteRackPhysicalPropertiesInputRequestTypeDef",
-    "GetSiteAddressOutputTypeDef",
     "UpdateSiteAddressInputRequestTypeDef",
-    "UpdateSiteAddressOutputTypeDef",
     "AssetInfoTypeDef",
     "CatalogItemTypeDef",
-    "GetConnectionResponseTypeDef",
     "CreateOrderInputRequestTypeDef",
+    "GetConnectionResponseTypeDef",
+    "GetSiteAddressOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartConnectionResponseTypeDef",
+    "UpdateSiteAddressOutputTypeDef",
     "CreateOutpostOutputTypeDef",
     "GetOutpostOutputTypeDef",
     "ListOutpostsOutputTypeDef",
     "UpdateOutpostOutputTypeDef",
     "CreateSiteInputRequestTypeDef",
-    "SiteTypeDef",
+    "GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
+    "ListAssetsInputListAssetsPaginateTypeDef",
+    "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
+    "ListOrdersInputListOrdersPaginateTypeDef",
+    "ListOutpostsInputListOutpostsPaginateTypeDef",
+    "ListSitesInputListSitesPaginateTypeDef",
     "GetOutpostInstanceTypesOutputTypeDef",
     "LineItemTypeDef",
     "ListOrdersOutputTypeDef",
+    "SiteTypeDef",
     "ListAssetsOutputTypeDef",
     "GetCatalogItemOutputTypeDef",
     "ListCatalogItemsOutputTypeDef",
+    "OrderTypeDef",
     "CreateSiteOutputTypeDef",
     "GetSiteOutputTypeDef",
     "ListSitesOutputTypeDef",
     "UpdateSiteOutputTypeDef",
     "UpdateSiteRackPhysicalPropertiesOutputTypeDef",
-    "OrderTypeDef",
     "CreateOrderOutputTypeDef",
     "GetOrderOutputTypeDef",
 )
 
+_RequiredAddressOutputTypeDef = TypedDict(
+    "_RequiredAddressOutputTypeDef",
+    {
+        "AddressLine1": str,
+        "City": str,
+        "StateOrRegion": str,
+        "PostalCode": str,
+        "CountryCode": str,
+    },
+)
+_OptionalAddressOutputTypeDef = TypedDict(
+    "_OptionalAddressOutputTypeDef",
+    {
+        "ContactName": str,
+        "ContactPhoneNumber": str,
+        "AddressLine2": str,
+        "AddressLine3": str,
+        "DistrictOrCounty": str,
+        "Municipality": str,
+    },
+    total=False,
+)
+
+
+class AddressOutputTypeDef(_RequiredAddressOutputTypeDef, _OptionalAddressOutputTypeDef):
+    pass
+
+
 _RequiredAddressTypeDef = TypedDict(
     "_RequiredAddressTypeDef",
     {
         "AddressLine1": str,
         "City": str,
         "StateOrRegion": str,
         "PostalCode": str,
@@ -205,14 +235,25 @@
     {
         "CatalogItemId": str,
         "Quantity": int,
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
 _RequiredCreateOutpostInputRequestTypeDef = TypedDict(
     "_RequiredCreateOutpostInputRequestTypeDef",
     {
         "Name": str,
         "SiteId": str,
     },
 )
@@ -308,36 +349,24 @@
 GetOutpostInputRequestTypeDef = TypedDict(
     "GetOutpostInputRequestTypeDef",
     {
         "OutpostId": str,
     },
 )
 
-_RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef = TypedDict(
-    "_RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
-    {
-        "OutpostId": str,
-    },
-)
-_OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef = TypedDict(
-    "_OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
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
-class GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef(
-    _RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
-    _OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetOutpostInstanceTypesInputRequestTypeDef = TypedDict(
     "_RequiredGetOutpostInstanceTypesInputRequestTypeDef",
     {
         "OutpostId": str,
     },
 )
 _OptionalGetOutpostInstanceTypesInputRequestTypeDef = TypedDict(
@@ -394,38 +423,14 @@
     {
         "ShipmentTrackingNumber": str,
         "ShipmentCarrier": ShipmentCarrierType,
     },
     total=False,
 )
 
-_RequiredListAssetsInputListAssetsPaginateTypeDef = TypedDict(
-    "_RequiredListAssetsInputListAssetsPaginateTypeDef",
-    {
-        "OutpostIdentifier": str,
-    },
-)
-_OptionalListAssetsInputListAssetsPaginateTypeDef = TypedDict(
-    "_OptionalListAssetsInputListAssetsPaginateTypeDef",
-    {
-        "HostIdFilter": Sequence[str],
-        "StatusFilter": Sequence[AssetStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAssetsInputListAssetsPaginateTypeDef(
-    _RequiredListAssetsInputListAssetsPaginateTypeDef,
-    _OptionalListAssetsInputListAssetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAssetsInputRequestTypeDef = TypedDict(
     "_RequiredListAssetsInputRequestTypeDef",
     {
         "OutpostIdentifier": str,
     },
 )
 _OptionalListAssetsInputRequestTypeDef = TypedDict(
@@ -442,46 +447,26 @@
 
 class ListAssetsInputRequestTypeDef(
     _RequiredListAssetsInputRequestTypeDef, _OptionalListAssetsInputRequestTypeDef
 ):
     pass
 
 
-ListCatalogItemsInputListCatalogItemsPaginateTypeDef = TypedDict(
-    "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
-    {
-        "ItemClassFilter": Sequence[CatalogItemClassType],
-        "SupportedStorageFilter": Sequence[SupportedStorageEnumType],
-        "EC2FamilyFilter": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCatalogItemsInputRequestTypeDef = TypedDict(
     "ListCatalogItemsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ItemClassFilter": Sequence[CatalogItemClassType],
         "SupportedStorageFilter": Sequence[SupportedStorageEnumType],
         "EC2FamilyFilter": Sequence[str],
     },
     total=False,
 )
 
-ListOrdersInputListOrdersPaginateTypeDef = TypedDict(
-    "ListOrdersInputListOrdersPaginateTypeDef",
-    {
-        "OutpostIdentifierFilter": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOrdersInputRequestTypeDef = TypedDict(
     "ListOrdersInputRequestTypeDef",
     {
         "OutpostIdentifierFilter": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -498,48 +483,26 @@
         "LineItemCountsByStatus": Dict[LineItemStatusType, int],
         "OrderSubmissionDate": datetime,
         "OrderFulfilledDate": datetime,
     },
     total=False,
 )
 
-ListOutpostsInputListOutpostsPaginateTypeDef = TypedDict(
-    "ListOutpostsInputListOutpostsPaginateTypeDef",
-    {
-        "LifeCycleStatusFilter": Sequence[str],
-        "AvailabilityZoneFilter": Sequence[str],
-        "AvailabilityZoneIdFilter": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOutpostsInputRequestTypeDef = TypedDict(
     "ListOutpostsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "LifeCycleStatusFilter": Sequence[str],
         "AvailabilityZoneFilter": Sequence[str],
         "AvailabilityZoneIdFilter": Sequence[str],
     },
     total=False,
 )
 
-ListSitesInputListSitesPaginateTypeDef = TypedDict(
-    "ListSitesInputListSitesPaginateTypeDef",
-    {
-        "OperatingAddressCountryCodeFilter": Sequence[str],
-        "OperatingAddressStateOrRegionFilter": Sequence[str],
-        "OperatingAddressCityFilter": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSitesInputRequestTypeDef = TypedDict(
     "ListSitesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "OperatingAddressCountryCodeFilter": Sequence[str],
         "OperatingAddressStateOrRegionFilter": Sequence[str],
@@ -551,62 +514,40 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+RackPhysicalPropertiesOutputTypeDef = TypedDict(
+    "RackPhysicalPropertiesOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PowerDrawKva": PowerDrawKvaType,
+        "PowerPhase": PowerPhaseType,
+        "PowerConnector": PowerConnectorType,
+        "PowerFeedDrop": PowerFeedDropType,
+        "UplinkGbps": UplinkGbpsType,
+        "UplinkCount": UplinkCountType,
+        "FiberOpticCableType": FiberOpticCableTypeType,
+        "OpticalStandard": OpticalStandardType,
+        "MaximumSupportedWeightLbs": MaximumSupportedWeightLbsType,
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
 StartConnectionRequestRequestTypeDef = TypedDict(
     "StartConnectionRequestRequestTypeDef",
     {
         "DeviceSerialNumber": str,
         "AssetId": str,
         "ClientPublicKey": str,
         "NetworkInterfaceDeviceIndex": int,
     },
 )
 
-StartConnectionResponseTypeDef = TypedDict(
-    "StartConnectionResponseTypeDef",
-    {
-        "ConnectionId": str,
-        "UnderlayIpAddress": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -691,42 +632,23 @@
 class UpdateSiteRackPhysicalPropertiesInputRequestTypeDef(
     _RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
     _OptionalUpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
 ):
     pass
 
 
-GetSiteAddressOutputTypeDef = TypedDict(
-    "GetSiteAddressOutputTypeDef",
-    {
-        "SiteId": str,
-        "AddressType": AddressTypeType,
-        "Address": AddressTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSiteAddressInputRequestTypeDef = TypedDict(
     "UpdateSiteAddressInputRequestTypeDef",
     {
         "SiteId": str,
         "AddressType": AddressTypeType,
         "Address": AddressTypeDef,
     },
 )
 
-UpdateSiteAddressOutputTypeDef = TypedDict(
-    "UpdateSiteAddressOutputTypeDef",
-    {
-        "AddressType": AddressTypeType,
-        "Address": AddressTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssetInfoTypeDef = TypedDict(
     "AssetInfoTypeDef",
     {
         "AssetId": str,
         "RackId": str,
         "AssetType": Literal["COMPUTE"],
         "ComputeAttributes": ComputeAttributesTypeDef,
@@ -745,23 +667,14 @@
         "WeightLbs": int,
         "SupportedUplinkGbps": List[int],
         "SupportedStorage": List[SupportedStorageEnumType],
     },
     total=False,
 )
 
-GetConnectionResponseTypeDef = TypedDict(
-    "GetConnectionResponseTypeDef",
-    {
-        "ConnectionId": str,
-        "ConnectionDetails": ConnectionDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateOrderInputRequestTypeDef = TypedDict(
     "_RequiredCreateOrderInputRequestTypeDef",
     {
         "OutpostIdentifier": str,
         "LineItems": Sequence[LineItemRequestTypeDef],
         "PaymentOption": PaymentOptionType,
     },
@@ -777,44 +690,89 @@
 
 class CreateOrderInputRequestTypeDef(
     _RequiredCreateOrderInputRequestTypeDef, _OptionalCreateOrderInputRequestTypeDef
 ):
     pass
 
 
+GetConnectionResponseTypeDef = TypedDict(
+    "GetConnectionResponseTypeDef",
+    {
+        "ConnectionId": str,
+        "ConnectionDetails": ConnectionDetailsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSiteAddressOutputTypeDef = TypedDict(
+    "GetSiteAddressOutputTypeDef",
+    {
+        "SiteId": str,
+        "AddressType": AddressTypeType,
+        "Address": AddressOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartConnectionResponseTypeDef = TypedDict(
+    "StartConnectionResponseTypeDef",
+    {
+        "ConnectionId": str,
+        "UnderlayIpAddress": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSiteAddressOutputTypeDef = TypedDict(
+    "UpdateSiteAddressOutputTypeDef",
+    {
+        "AddressType": AddressTypeType,
+        "Address": AddressOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateOutpostOutputTypeDef = TypedDict(
     "CreateOutpostOutputTypeDef",
     {
         "Outpost": OutpostTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOutpostOutputTypeDef = TypedDict(
     "GetOutpostOutputTypeDef",
     {
         "Outpost": OutpostTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOutpostsOutputTypeDef = TypedDict(
     "ListOutpostsOutputTypeDef",
     {
         "Outposts": List[OutpostTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateOutpostOutputTypeDef = TypedDict(
     "UpdateOutpostOutputTypeDef",
     {
         "Outpost": OutpostTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSiteInputRequestTypeDef = TypedDict(
     "_RequiredCreateSiteInputRequestTypeDef",
     {
         "Name": str,
@@ -836,40 +794,110 @@
 
 class CreateSiteInputRequestTypeDef(
     _RequiredCreateSiteInputRequestTypeDef, _OptionalCreateSiteInputRequestTypeDef
 ):
     pass
 
 
-SiteTypeDef = TypedDict(
-    "SiteTypeDef",
+_RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef = TypedDict(
+    "_RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
     {
-        "SiteId": str,
-        "AccountId": str,
-        "Name": str,
-        "Description": str,
-        "Tags": Dict[str, str],
-        "SiteArn": str,
-        "Notes": str,
-        "OperatingAddressCountryCode": str,
-        "OperatingAddressStateOrRegion": str,
-        "OperatingAddressCity": str,
-        "RackPhysicalProperties": RackPhysicalPropertiesTypeDef,
+        "OutpostId": str,
+    },
+)
+_OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef = TypedDict(
+    "_OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef(
+    _RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
+    _OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAssetsInputListAssetsPaginateTypeDef = TypedDict(
+    "_RequiredListAssetsInputListAssetsPaginateTypeDef",
+    {
+        "OutpostIdentifier": str,
+    },
+)
+_OptionalListAssetsInputListAssetsPaginateTypeDef = TypedDict(
+    "_OptionalListAssetsInputListAssetsPaginateTypeDef",
+    {
+        "HostIdFilter": Sequence[str],
+        "StatusFilter": Sequence[AssetStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAssetsInputListAssetsPaginateTypeDef(
+    _RequiredListAssetsInputListAssetsPaginateTypeDef,
+    _OptionalListAssetsInputListAssetsPaginateTypeDef,
+):
+    pass
+
+
+ListCatalogItemsInputListCatalogItemsPaginateTypeDef = TypedDict(
+    "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
+    {
+        "ItemClassFilter": Sequence[CatalogItemClassType],
+        "SupportedStorageFilter": Sequence[SupportedStorageEnumType],
+        "EC2FamilyFilter": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOrdersInputListOrdersPaginateTypeDef = TypedDict(
+    "ListOrdersInputListOrdersPaginateTypeDef",
+    {
+        "OutpostIdentifierFilter": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOutpostsInputListOutpostsPaginateTypeDef = TypedDict(
+    "ListOutpostsInputListOutpostsPaginateTypeDef",
+    {
+        "LifeCycleStatusFilter": Sequence[str],
+        "AvailabilityZoneFilter": Sequence[str],
+        "AvailabilityZoneIdFilter": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSitesInputListSitesPaginateTypeDef = TypedDict(
+    "ListSitesInputListSitesPaginateTypeDef",
+    {
+        "OperatingAddressCountryCodeFilter": Sequence[str],
+        "OperatingAddressStateOrRegionFilter": Sequence[str],
+        "OperatingAddressCityFilter": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetOutpostInstanceTypesOutputTypeDef = TypedDict(
     "GetOutpostInstanceTypesOutputTypeDef",
     {
         "InstanceTypes": List[InstanceTypeItemTypeDef],
         "NextToken": str,
         "OutpostId": str,
         "OutpostArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LineItemTypeDef = TypedDict(
     "LineItemTypeDef",
     {
         "CatalogItemId": str,
@@ -885,109 +913,127 @@
 )
 
 ListOrdersOutputTypeDef = TypedDict(
     "ListOrdersOutputTypeDef",
     {
         "Orders": List[OrderSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SiteTypeDef = TypedDict(
+    "SiteTypeDef",
+    {
+        "SiteId": str,
+        "AccountId": str,
+        "Name": str,
+        "Description": str,
+        "Tags": Dict[str, str],
+        "SiteArn": str,
+        "Notes": str,
+        "OperatingAddressCountryCode": str,
+        "OperatingAddressStateOrRegion": str,
+        "OperatingAddressCity": str,
+        "RackPhysicalProperties": RackPhysicalPropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
 ListAssetsOutputTypeDef = TypedDict(
     "ListAssetsOutputTypeDef",
     {
         "Assets": List[AssetInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCatalogItemOutputTypeDef = TypedDict(
     "GetCatalogItemOutputTypeDef",
     {
         "CatalogItem": CatalogItemTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCatalogItemsOutputTypeDef = TypedDict(
     "ListCatalogItemsOutputTypeDef",
     {
         "CatalogItems": List[CatalogItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+OrderTypeDef = TypedDict(
+    "OrderTypeDef",
+    {
+        "OutpostId": str,
+        "OrderId": str,
+        "Status": OrderStatusType,
+        "LineItems": List[LineItemTypeDef],
+        "PaymentOption": PaymentOptionType,
+        "OrderSubmissionDate": datetime,
+        "OrderFulfilledDate": datetime,
+        "PaymentTerm": PaymentTermType,
+        "OrderType": OrderTypeType,
     },
+    total=False,
 )
 
 CreateSiteOutputTypeDef = TypedDict(
     "CreateSiteOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSiteOutputTypeDef = TypedDict(
     "GetSiteOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSitesOutputTypeDef = TypedDict(
     "ListSitesOutputTypeDef",
     {
         "Sites": List[SiteTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSiteOutputTypeDef = TypedDict(
     "UpdateSiteOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSiteRackPhysicalPropertiesOutputTypeDef = TypedDict(
     "UpdateSiteRackPhysicalPropertiesOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-OrderTypeDef = TypedDict(
-    "OrderTypeDef",
-    {
-        "OutpostId": str,
-        "OrderId": str,
-        "Status": OrderStatusType,
-        "LineItems": List[LineItemTypeDef],
-        "PaymentOption": PaymentOptionType,
-        "OrderSubmissionDate": datetime,
-        "OrderFulfilledDate": datetime,
-        "PaymentTerm": PaymentTermType,
-        "OrderType": OrderTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 CreateOrderOutputTypeDef = TypedDict(
     "CreateOrderOutputTypeDef",
     {
         "Order": OrderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOrderOutputTypeDef = TypedDict(
     "GetOrderOutputTypeDef",
     {
         "Order": OrderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts/type_defs.pyi` & `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for outposts service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_outposts.type_defs import AddressTypeDef
+    from mypy_boto3_outposts.type_defs import AddressOutputTypeDef
 
-    data: AddressTypeDef = {...}
+    data: AddressOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -46,88 +46,116 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AddressOutputTypeDef",
     "AddressTypeDef",
     "AssetLocationTypeDef",
     "ComputeAttributesTypeDef",
     "CancelOrderInputRequestTypeDef",
     "EC2CapacityTypeDef",
     "ConnectionDetailsTypeDef",
     "LineItemRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateOutpostInputRequestTypeDef",
     "OutpostTypeDef",
     "RackPhysicalPropertiesTypeDef",
     "DeleteOutpostInputRequestTypeDef",
     "DeleteSiteInputRequestTypeDef",
     "GetCatalogItemInputRequestTypeDef",
     "GetConnectionRequestRequestTypeDef",
     "GetOrderInputRequestTypeDef",
     "GetOutpostInputRequestTypeDef",
-    "GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetOutpostInstanceTypesInputRequestTypeDef",
     "InstanceTypeItemTypeDef",
     "GetSiteAddressInputRequestTypeDef",
     "GetSiteInputRequestTypeDef",
     "LineItemAssetInformationTypeDef",
     "ShipmentInformationTypeDef",
-    "ListAssetsInputListAssetsPaginateTypeDef",
     "ListAssetsInputRequestTypeDef",
-    "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
     "ListCatalogItemsInputRequestTypeDef",
-    "ListOrdersInputListOrdersPaginateTypeDef",
     "ListOrdersInputRequestTypeDef",
     "OrderSummaryTypeDef",
-    "ListOutpostsInputListOutpostsPaginateTypeDef",
     "ListOutpostsInputRequestTypeDef",
-    "ListSitesInputListSitesPaginateTypeDef",
     "ListSitesInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "RackPhysicalPropertiesOutputTypeDef",
     "StartConnectionRequestRequestTypeDef",
-    "StartConnectionResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateOutpostInputRequestTypeDef",
     "UpdateSiteInputRequestTypeDef",
     "UpdateSiteRackPhysicalPropertiesInputRequestTypeDef",
-    "GetSiteAddressOutputTypeDef",
     "UpdateSiteAddressInputRequestTypeDef",
-    "UpdateSiteAddressOutputTypeDef",
     "AssetInfoTypeDef",
     "CatalogItemTypeDef",
-    "GetConnectionResponseTypeDef",
     "CreateOrderInputRequestTypeDef",
+    "GetConnectionResponseTypeDef",
+    "GetSiteAddressOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartConnectionResponseTypeDef",
+    "UpdateSiteAddressOutputTypeDef",
     "CreateOutpostOutputTypeDef",
     "GetOutpostOutputTypeDef",
     "ListOutpostsOutputTypeDef",
     "UpdateOutpostOutputTypeDef",
     "CreateSiteInputRequestTypeDef",
-    "SiteTypeDef",
+    "GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
+    "ListAssetsInputListAssetsPaginateTypeDef",
+    "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
+    "ListOrdersInputListOrdersPaginateTypeDef",
+    "ListOutpostsInputListOutpostsPaginateTypeDef",
+    "ListSitesInputListSitesPaginateTypeDef",
     "GetOutpostInstanceTypesOutputTypeDef",
     "LineItemTypeDef",
     "ListOrdersOutputTypeDef",
+    "SiteTypeDef",
     "ListAssetsOutputTypeDef",
     "GetCatalogItemOutputTypeDef",
     "ListCatalogItemsOutputTypeDef",
+    "OrderTypeDef",
     "CreateSiteOutputTypeDef",
     "GetSiteOutputTypeDef",
     "ListSitesOutputTypeDef",
     "UpdateSiteOutputTypeDef",
     "UpdateSiteRackPhysicalPropertiesOutputTypeDef",
-    "OrderTypeDef",
     "CreateOrderOutputTypeDef",
     "GetOrderOutputTypeDef",
 )
 
+_RequiredAddressOutputTypeDef = TypedDict(
+    "_RequiredAddressOutputTypeDef",
+    {
+        "AddressLine1": str,
+        "City": str,
+        "StateOrRegion": str,
+        "PostalCode": str,
+        "CountryCode": str,
+    },
+)
+_OptionalAddressOutputTypeDef = TypedDict(
+    "_OptionalAddressOutputTypeDef",
+    {
+        "ContactName": str,
+        "ContactPhoneNumber": str,
+        "AddressLine2": str,
+        "AddressLine3": str,
+        "DistrictOrCounty": str,
+        "Municipality": str,
+    },
+    total=False,
+)
+
+class AddressOutputTypeDef(_RequiredAddressOutputTypeDef, _OptionalAddressOutputTypeDef):
+    pass
+
 _RequiredAddressTypeDef = TypedDict(
     "_RequiredAddressTypeDef",
     {
         "AddressLine1": str,
         "City": str,
         "StateOrRegion": str,
         "PostalCode": str,
@@ -202,14 +230,25 @@
     {
         "CatalogItemId": str,
         "Quantity": int,
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
 _RequiredCreateOutpostInputRequestTypeDef = TypedDict(
     "_RequiredCreateOutpostInputRequestTypeDef",
     {
         "Name": str,
         "SiteId": str,
     },
 )
@@ -303,34 +342,24 @@
 GetOutpostInputRequestTypeDef = TypedDict(
     "GetOutpostInputRequestTypeDef",
     {
         "OutpostId": str,
     },
 )
 
-_RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef = TypedDict(
-    "_RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
-    {
-        "OutpostId": str,
-    },
-)
-_OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef = TypedDict(
-    "_OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
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
 
-class GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef(
-    _RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
-    _OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetOutpostInstanceTypesInputRequestTypeDef = TypedDict(
     "_RequiredGetOutpostInstanceTypesInputRequestTypeDef",
     {
         "OutpostId": str,
     },
 )
 _OptionalGetOutpostInstanceTypesInputRequestTypeDef = TypedDict(
@@ -385,36 +414,14 @@
     {
         "ShipmentTrackingNumber": str,
         "ShipmentCarrier": ShipmentCarrierType,
     },
     total=False,
 )
 
-_RequiredListAssetsInputListAssetsPaginateTypeDef = TypedDict(
-    "_RequiredListAssetsInputListAssetsPaginateTypeDef",
-    {
-        "OutpostIdentifier": str,
-    },
-)
-_OptionalListAssetsInputListAssetsPaginateTypeDef = TypedDict(
-    "_OptionalListAssetsInputListAssetsPaginateTypeDef",
-    {
-        "HostIdFilter": Sequence[str],
-        "StatusFilter": Sequence[AssetStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAssetsInputListAssetsPaginateTypeDef(
-    _RequiredListAssetsInputListAssetsPaginateTypeDef,
-    _OptionalListAssetsInputListAssetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAssetsInputRequestTypeDef = TypedDict(
     "_RequiredListAssetsInputRequestTypeDef",
     {
         "OutpostIdentifier": str,
     },
 )
 _OptionalListAssetsInputRequestTypeDef = TypedDict(
@@ -429,46 +436,26 @@
 )
 
 class ListAssetsInputRequestTypeDef(
     _RequiredListAssetsInputRequestTypeDef, _OptionalListAssetsInputRequestTypeDef
 ):
     pass
 
-ListCatalogItemsInputListCatalogItemsPaginateTypeDef = TypedDict(
-    "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
-    {
-        "ItemClassFilter": Sequence[CatalogItemClassType],
-        "SupportedStorageFilter": Sequence[SupportedStorageEnumType],
-        "EC2FamilyFilter": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCatalogItemsInputRequestTypeDef = TypedDict(
     "ListCatalogItemsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ItemClassFilter": Sequence[CatalogItemClassType],
         "SupportedStorageFilter": Sequence[SupportedStorageEnumType],
         "EC2FamilyFilter": Sequence[str],
     },
     total=False,
 )
 
-ListOrdersInputListOrdersPaginateTypeDef = TypedDict(
-    "ListOrdersInputListOrdersPaginateTypeDef",
-    {
-        "OutpostIdentifierFilter": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOrdersInputRequestTypeDef = TypedDict(
     "ListOrdersInputRequestTypeDef",
     {
         "OutpostIdentifierFilter": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -485,48 +472,26 @@
         "LineItemCountsByStatus": Dict[LineItemStatusType, int],
         "OrderSubmissionDate": datetime,
         "OrderFulfilledDate": datetime,
     },
     total=False,
 )
 
-ListOutpostsInputListOutpostsPaginateTypeDef = TypedDict(
-    "ListOutpostsInputListOutpostsPaginateTypeDef",
-    {
-        "LifeCycleStatusFilter": Sequence[str],
-        "AvailabilityZoneFilter": Sequence[str],
-        "AvailabilityZoneIdFilter": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOutpostsInputRequestTypeDef = TypedDict(
     "ListOutpostsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "LifeCycleStatusFilter": Sequence[str],
         "AvailabilityZoneFilter": Sequence[str],
         "AvailabilityZoneIdFilter": Sequence[str],
     },
     total=False,
 )
 
-ListSitesInputListSitesPaginateTypeDef = TypedDict(
-    "ListSitesInputListSitesPaginateTypeDef",
-    {
-        "OperatingAddressCountryCodeFilter": Sequence[str],
-        "OperatingAddressStateOrRegionFilter": Sequence[str],
-        "OperatingAddressCityFilter": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSitesInputRequestTypeDef = TypedDict(
     "ListSitesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "OperatingAddressCountryCodeFilter": Sequence[str],
         "OperatingAddressStateOrRegionFilter": Sequence[str],
@@ -538,62 +503,40 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+RackPhysicalPropertiesOutputTypeDef = TypedDict(
+    "RackPhysicalPropertiesOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PowerDrawKva": PowerDrawKvaType,
+        "PowerPhase": PowerPhaseType,
+        "PowerConnector": PowerConnectorType,
+        "PowerFeedDrop": PowerFeedDropType,
+        "UplinkGbps": UplinkGbpsType,
+        "UplinkCount": UplinkCountType,
+        "FiberOpticCableType": FiberOpticCableTypeType,
+        "OpticalStandard": OpticalStandardType,
+        "MaximumSupportedWeightLbs": MaximumSupportedWeightLbsType,
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
 StartConnectionRequestRequestTypeDef = TypedDict(
     "StartConnectionRequestRequestTypeDef",
     {
         "DeviceSerialNumber": str,
         "AssetId": str,
         "ClientPublicKey": str,
         "NetworkInterfaceDeviceIndex": int,
     },
 )
 
-StartConnectionResponseTypeDef = TypedDict(
-    "StartConnectionResponseTypeDef",
-    {
-        "ConnectionId": str,
-        "UnderlayIpAddress": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -672,42 +615,23 @@
 
 class UpdateSiteRackPhysicalPropertiesInputRequestTypeDef(
     _RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
     _OptionalUpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
 ):
     pass
 
-GetSiteAddressOutputTypeDef = TypedDict(
-    "GetSiteAddressOutputTypeDef",
-    {
-        "SiteId": str,
-        "AddressType": AddressTypeType,
-        "Address": AddressTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSiteAddressInputRequestTypeDef = TypedDict(
     "UpdateSiteAddressInputRequestTypeDef",
     {
         "SiteId": str,
         "AddressType": AddressTypeType,
         "Address": AddressTypeDef,
     },
 )
 
-UpdateSiteAddressOutputTypeDef = TypedDict(
-    "UpdateSiteAddressOutputTypeDef",
-    {
-        "AddressType": AddressTypeType,
-        "Address": AddressTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssetInfoTypeDef = TypedDict(
     "AssetInfoTypeDef",
     {
         "AssetId": str,
         "RackId": str,
         "AssetType": Literal["COMPUTE"],
         "ComputeAttributes": ComputeAttributesTypeDef,
@@ -726,23 +650,14 @@
         "WeightLbs": int,
         "SupportedUplinkGbps": List[int],
         "SupportedStorage": List[SupportedStorageEnumType],
     },
     total=False,
 )
 
-GetConnectionResponseTypeDef = TypedDict(
-    "GetConnectionResponseTypeDef",
-    {
-        "ConnectionId": str,
-        "ConnectionDetails": ConnectionDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateOrderInputRequestTypeDef = TypedDict(
     "_RequiredCreateOrderInputRequestTypeDef",
     {
         "OutpostIdentifier": str,
         "LineItems": Sequence[LineItemRequestTypeDef],
         "PaymentOption": PaymentOptionType,
     },
@@ -756,44 +671,89 @@
 )
 
 class CreateOrderInputRequestTypeDef(
     _RequiredCreateOrderInputRequestTypeDef, _OptionalCreateOrderInputRequestTypeDef
 ):
     pass
 
+GetConnectionResponseTypeDef = TypedDict(
+    "GetConnectionResponseTypeDef",
+    {
+        "ConnectionId": str,
+        "ConnectionDetails": ConnectionDetailsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSiteAddressOutputTypeDef = TypedDict(
+    "GetSiteAddressOutputTypeDef",
+    {
+        "SiteId": str,
+        "AddressType": AddressTypeType,
+        "Address": AddressOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartConnectionResponseTypeDef = TypedDict(
+    "StartConnectionResponseTypeDef",
+    {
+        "ConnectionId": str,
+        "UnderlayIpAddress": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSiteAddressOutputTypeDef = TypedDict(
+    "UpdateSiteAddressOutputTypeDef",
+    {
+        "AddressType": AddressTypeType,
+        "Address": AddressOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateOutpostOutputTypeDef = TypedDict(
     "CreateOutpostOutputTypeDef",
     {
         "Outpost": OutpostTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOutpostOutputTypeDef = TypedDict(
     "GetOutpostOutputTypeDef",
     {
         "Outpost": OutpostTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOutpostsOutputTypeDef = TypedDict(
     "ListOutpostsOutputTypeDef",
     {
         "Outposts": List[OutpostTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateOutpostOutputTypeDef = TypedDict(
     "UpdateOutpostOutputTypeDef",
     {
         "Outpost": OutpostTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSiteInputRequestTypeDef = TypedDict(
     "_RequiredCreateSiteInputRequestTypeDef",
     {
         "Name": str,
@@ -813,40 +773,106 @@
 )
 
 class CreateSiteInputRequestTypeDef(
     _RequiredCreateSiteInputRequestTypeDef, _OptionalCreateSiteInputRequestTypeDef
 ):
     pass
 
-SiteTypeDef = TypedDict(
-    "SiteTypeDef",
+_RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef = TypedDict(
+    "_RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
     {
-        "SiteId": str,
-        "AccountId": str,
-        "Name": str,
-        "Description": str,
-        "Tags": Dict[str, str],
-        "SiteArn": str,
-        "Notes": str,
-        "OperatingAddressCountryCode": str,
-        "OperatingAddressStateOrRegion": str,
-        "OperatingAddressCity": str,
-        "RackPhysicalProperties": RackPhysicalPropertiesTypeDef,
+        "OutpostId": str,
+    },
+)
+_OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef = TypedDict(
+    "_OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef(
+    _RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
+    _OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
+):
+    pass
+
+_RequiredListAssetsInputListAssetsPaginateTypeDef = TypedDict(
+    "_RequiredListAssetsInputListAssetsPaginateTypeDef",
+    {
+        "OutpostIdentifier": str,
+    },
+)
+_OptionalListAssetsInputListAssetsPaginateTypeDef = TypedDict(
+    "_OptionalListAssetsInputListAssetsPaginateTypeDef",
+    {
+        "HostIdFilter": Sequence[str],
+        "StatusFilter": Sequence[AssetStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAssetsInputListAssetsPaginateTypeDef(
+    _RequiredListAssetsInputListAssetsPaginateTypeDef,
+    _OptionalListAssetsInputListAssetsPaginateTypeDef,
+):
+    pass
+
+ListCatalogItemsInputListCatalogItemsPaginateTypeDef = TypedDict(
+    "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
+    {
+        "ItemClassFilter": Sequence[CatalogItemClassType],
+        "SupportedStorageFilter": Sequence[SupportedStorageEnumType],
+        "EC2FamilyFilter": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOrdersInputListOrdersPaginateTypeDef = TypedDict(
+    "ListOrdersInputListOrdersPaginateTypeDef",
+    {
+        "OutpostIdentifierFilter": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOutpostsInputListOutpostsPaginateTypeDef = TypedDict(
+    "ListOutpostsInputListOutpostsPaginateTypeDef",
+    {
+        "LifeCycleStatusFilter": Sequence[str],
+        "AvailabilityZoneFilter": Sequence[str],
+        "AvailabilityZoneIdFilter": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSitesInputListSitesPaginateTypeDef = TypedDict(
+    "ListSitesInputListSitesPaginateTypeDef",
+    {
+        "OperatingAddressCountryCodeFilter": Sequence[str],
+        "OperatingAddressStateOrRegionFilter": Sequence[str],
+        "OperatingAddressCityFilter": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetOutpostInstanceTypesOutputTypeDef = TypedDict(
     "GetOutpostInstanceTypesOutputTypeDef",
     {
         "InstanceTypes": List[InstanceTypeItemTypeDef],
         "NextToken": str,
         "OutpostId": str,
         "OutpostArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LineItemTypeDef = TypedDict(
     "LineItemTypeDef",
     {
         "CatalogItemId": str,
@@ -862,109 +888,127 @@
 )
 
 ListOrdersOutputTypeDef = TypedDict(
     "ListOrdersOutputTypeDef",
     {
         "Orders": List[OrderSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SiteTypeDef = TypedDict(
+    "SiteTypeDef",
+    {
+        "SiteId": str,
+        "AccountId": str,
+        "Name": str,
+        "Description": str,
+        "Tags": Dict[str, str],
+        "SiteArn": str,
+        "Notes": str,
+        "OperatingAddressCountryCode": str,
+        "OperatingAddressStateOrRegion": str,
+        "OperatingAddressCity": str,
+        "RackPhysicalProperties": RackPhysicalPropertiesOutputTypeDef,
     },
+    total=False,
 )
 
 ListAssetsOutputTypeDef = TypedDict(
     "ListAssetsOutputTypeDef",
     {
         "Assets": List[AssetInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCatalogItemOutputTypeDef = TypedDict(
     "GetCatalogItemOutputTypeDef",
     {
         "CatalogItem": CatalogItemTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCatalogItemsOutputTypeDef = TypedDict(
     "ListCatalogItemsOutputTypeDef",
     {
         "CatalogItems": List[CatalogItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+OrderTypeDef = TypedDict(
+    "OrderTypeDef",
+    {
+        "OutpostId": str,
+        "OrderId": str,
+        "Status": OrderStatusType,
+        "LineItems": List[LineItemTypeDef],
+        "PaymentOption": PaymentOptionType,
+        "OrderSubmissionDate": datetime,
+        "OrderFulfilledDate": datetime,
+        "PaymentTerm": PaymentTermType,
+        "OrderType": OrderTypeType,
+    },
+    total=False,
+)
+
 CreateSiteOutputTypeDef = TypedDict(
     "CreateSiteOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSiteOutputTypeDef = TypedDict(
     "GetSiteOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSitesOutputTypeDef = TypedDict(
     "ListSitesOutputTypeDef",
     {
         "Sites": List[SiteTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSiteOutputTypeDef = TypedDict(
     "UpdateSiteOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSiteRackPhysicalPropertiesOutputTypeDef = TypedDict(
     "UpdateSiteRackPhysicalPropertiesOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OrderTypeDef = TypedDict(
-    "OrderTypeDef",
-    {
-        "OutpostId": str,
-        "OrderId": str,
-        "Status": OrderStatusType,
-        "LineItems": List[LineItemTypeDef],
-        "PaymentOption": PaymentOptionType,
-        "OrderSubmissionDate": datetime,
-        "OrderFulfilledDate": datetime,
-        "PaymentTerm": PaymentTermType,
-        "OrderType": OrderTypeType,
-    },
-    total=False,
-)
-
 CreateOrderOutputTypeDef = TypedDict(
     "CreateOrderOutputTypeDef",
     {
         "Order": OrderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOrderOutputTypeDef = TypedDict(
     "GetOrderOutputTypeDef",
     {
         "Order": OrderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts.egg-info/PKG-INFO` & `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-outposts
-Version: 1.28.0
-Summary: Type annotations for boto3.Outposts 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Outposts 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-outposts"></a>
 
 # mypy-boto3-outposts
 
 [![PyPI - mypy-boto3-outposts](https://img.shields.io/pypi/v/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-outposts?color=blue)](https://pypistats.org/packages/mypy-boto3-outposts)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-outposts)](https://pepy.tech/project/mypy-boto3-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Outposts 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
+[boto3.Outposts 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
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
 [mypy-boto3-outposts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -360,90 +360,92 @@
 ### Typed dictionaries
 
 `mypy_boto3_outposts.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_outposts.type_defs import (
+    AddressOutputTypeDef,
     AddressTypeDef,
     AssetLocationTypeDef,
     ComputeAttributesTypeDef,
     CancelOrderInputRequestTypeDef,
     EC2CapacityTypeDef,
     ConnectionDetailsTypeDef,
     LineItemRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateOutpostInputRequestTypeDef,
     OutpostTypeDef,
     RackPhysicalPropertiesTypeDef,
     DeleteOutpostInputRequestTypeDef,
     DeleteSiteInputRequestTypeDef,
     GetCatalogItemInputRequestTypeDef,
     GetConnectionRequestRequestTypeDef,
     GetOrderInputRequestTypeDef,
     GetOutpostInputRequestTypeDef,
-    GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetOutpostInstanceTypesInputRequestTypeDef,
     InstanceTypeItemTypeDef,
     GetSiteAddressInputRequestTypeDef,
     GetSiteInputRequestTypeDef,
     LineItemAssetInformationTypeDef,
     ShipmentInformationTypeDef,
-    ListAssetsInputListAssetsPaginateTypeDef,
     ListAssetsInputRequestTypeDef,
-    ListCatalogItemsInputListCatalogItemsPaginateTypeDef,
     ListCatalogItemsInputRequestTypeDef,
-    ListOrdersInputListOrdersPaginateTypeDef,
     ListOrdersInputRequestTypeDef,
     OrderSummaryTypeDef,
-    ListOutpostsInputListOutpostsPaginateTypeDef,
     ListOutpostsInputRequestTypeDef,
-    ListSitesInputListSitesPaginateTypeDef,
     ListSitesInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    RackPhysicalPropertiesOutputTypeDef,
     StartConnectionRequestRequestTypeDef,
-    StartConnectionResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateOutpostInputRequestTypeDef,
     UpdateSiteInputRequestTypeDef,
     UpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
-    GetSiteAddressOutputTypeDef,
     UpdateSiteAddressInputRequestTypeDef,
-    UpdateSiteAddressOutputTypeDef,
     AssetInfoTypeDef,
     CatalogItemTypeDef,
-    GetConnectionResponseTypeDef,
     CreateOrderInputRequestTypeDef,
+    GetConnectionResponseTypeDef,
+    GetSiteAddressOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartConnectionResponseTypeDef,
+    UpdateSiteAddressOutputTypeDef,
     CreateOutpostOutputTypeDef,
     GetOutpostOutputTypeDef,
     ListOutpostsOutputTypeDef,
     UpdateOutpostOutputTypeDef,
     CreateSiteInputRequestTypeDef,
-    SiteTypeDef,
+    GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
+    ListAssetsInputListAssetsPaginateTypeDef,
+    ListCatalogItemsInputListCatalogItemsPaginateTypeDef,
+    ListOrdersInputListOrdersPaginateTypeDef,
+    ListOutpostsInputListOutpostsPaginateTypeDef,
+    ListSitesInputListSitesPaginateTypeDef,
     GetOutpostInstanceTypesOutputTypeDef,
     LineItemTypeDef,
     ListOrdersOutputTypeDef,
+    SiteTypeDef,
     ListAssetsOutputTypeDef,
     GetCatalogItemOutputTypeDef,
     ListCatalogItemsOutputTypeDef,
+    OrderTypeDef,
     CreateSiteOutputTypeDef,
     GetSiteOutputTypeDef,
     ListSitesOutputTypeDef,
     UpdateSiteOutputTypeDef,
     UpdateSiteRackPhysicalPropertiesOutputTypeDef,
-    OrderTypeDef,
     CreateOrderOutputTypeDef,
     GetOrderOutputTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_structure() -> AddressOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-outposts-1.28.0/mypy_boto3_outposts.egg-info/SOURCES.txt` & `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.28.0/setup.py` & `mypy-boto3-outposts-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-outposts",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_outposts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Outposts 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Outposts 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

