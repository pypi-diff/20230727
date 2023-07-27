# Comparing `tmp/mypy-boto3-pricing-1.28.0.tar.gz` & `tmp/mypy-boto3-pricing-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pricing-1.28.0.tar", last modified: Thu Jul  6 21:00:21 2023, max compression
+gzip compressed data, was "mypy-boto3-pricing-1.28.12.tar", last modified: Thu Jul 27 11:49:24 2023, max compression
```

## Comparing `mypy-boto3-pricing-1.28.0.tar` & `mypy-boto3-pricing-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:21.734399 mypy-boto3-pricing-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:49:44.000000 mypy-boto3-pricing-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-07-06 21:00:21.734399 mypy-boto3-pricing-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12274 2023-07-06 20:49:44.000000 mypy-boto3-pricing-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:21.714399 mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-06 20:49:44.000000 mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-06 20:49:44.000000 mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 20:49:44.000000 mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-07-06 20:49:44.000000 mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-06 20:49:44.000000 mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-07-06 20:49:44.000000 mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-07-06 20:49:44.000000 mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-06 20:49:44.000000 mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-07-06 20:49:44.000000 mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:49:44.000000 mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-07-06 20:49:44.000000 mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-06 20:49:44.000000 mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:49:44.000000 mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:21.734399 mypy-boto3-pricing-1.28.0/mypy_boto3_pricing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-07-06 21:00:21.000000 mypy-boto3-pricing-1.28.0/mypy_boto3_pricing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-06 21:00:21.000000 mypy-boto3-pricing-1.28.0/mypy_boto3_pricing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:21.000000 mypy-boto3-pricing-1.28.0/mypy_boto3_pricing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:21.000000 mypy-boto3-pricing-1.28.0/mypy_boto3_pricing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:21.000000 mypy-boto3-pricing-1.28.0/mypy_boto3_pricing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 21:00:21.000000 mypy-boto3-pricing-1.28.0/mypy_boto3_pricing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:21.734399 mypy-boto3-pricing-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-06 20:49:44.000000 mypy-boto3-pricing-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.917162 mypy-boto3-pricing-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:42.000000 mypy-boto3-pricing-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13746 2023-07-27 11:49:24.917162 mypy-boto3-pricing-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-07-27 11:41:42.000000 mypy-boto3-pricing-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.917162 mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-27 11:41:42.000000 mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-27 11:41:42.000000 mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 11:41:42.000000 mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-07-27 11:41:42.000000 mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-27 11:41:42.000000 mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-07-27 11:41:42.000000 mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-07-27 11:41:42.000000 mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-07-27 11:41:42.000000 mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-27 11:41:42.000000 mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:42.000000 mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-27 11:41:43.000000 mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-07-27 11:41:42.000000 mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:42.000000 mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.917162 mypy-boto3-pricing-1.28.12/mypy_boto3_pricing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13746 2023-07-27 11:49:24.000000 mypy-boto3-pricing-1.28.12/mypy_boto3_pricing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-27 11:49:24.000000 mypy-boto3-pricing-1.28.12/mypy_boto3_pricing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-pricing-1.28.12/mypy_boto3_pricing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-pricing-1.28.12/mypy_boto3_pricing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:24.000000 mypy-boto3-pricing-1.28.12/mypy_boto3_pricing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 11:49:24.000000 mypy-boto3-pricing-1.28.12/mypy_boto3_pricing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:24.917162 mypy-boto3-pricing-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 11:41:42.000000 mypy-boto3-pricing-1.28.12/setup.py
```

### Comparing `mypy-boto3-pricing-1.28.0/LICENSE` & `mypy-boto3-pricing-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.28.0/PKG-INFO` & `mypy-boto3-pricing-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pricing
-Version: 1.28.0
-Summary: Type annotations for boto3.Pricing 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Pricing 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-pricing"></a>
 
 # mypy-boto3-pricing
 
 [![PyPI - mypy-boto3-pricing](https://img.shields.io/pypi/v/mypy-boto3-pricing.svg?color=blue)](https://pypi.org/project/mypy-boto3-pricing)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pricing.svg?color=blue)](https://pypi.org/project/mypy-boto3-pricing)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pricing?color=blue)](https://pypistats.org/packages/mypy-boto3-pricing)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pricing)](https://pepy.tech/project/mypy-boto3-pricing)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pricing 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
+[boto3.Pricing 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
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
 [mypy-boto3-pricing docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,29 +333,29 @@
 
 `mypy_boto3_pricing.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pricing.type_defs import (
     AttributeValueTypeDef,
-    DescribeServicesRequestDescribeServicesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeServicesRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ServiceTypeDef,
     FilterTypeDef,
-    GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
     GetAttributeValuesRequestRequestTypeDef,
     GetPriceListFileUrlRequestRequestTypeDef,
-    GetPriceListFileUrlResponseTypeDef,
-    GetProductsResponseTypeDef,
-    ListPriceListsRequestListPriceListsPaginateTypeDef,
     ListPriceListsRequestRequestTypeDef,
     PriceListTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    DescribeServicesRequestDescribeServicesPaginateTypeDef,
+    GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
+    ListPriceListsRequestListPriceListsPaginateTypeDef,
     GetAttributeValuesResponseTypeDef,
+    GetPriceListFileUrlResponseTypeDef,
+    GetProductsResponseTypeDef,
     DescribeServicesResponseTypeDef,
     GetProductsRequestGetProductsPaginateTypeDef,
     GetProductsRequestRequestTypeDef,
     ListPriceListsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-pricing-1.28.0/README.md` & `mypy-boto3-pricing-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-pricing"></a>
 
 # mypy-boto3-pricing
 
 [![PyPI - mypy-boto3-pricing](https://img.shields.io/pypi/v/mypy-boto3-pricing.svg?color=blue)](https://pypi.org/project/mypy-boto3-pricing)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pricing.svg?color=blue)](https://pypi.org/project/mypy-boto3-pricing)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pricing?color=blue)](https://pypistats.org/packages/mypy-boto3-pricing)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pricing)](https://pepy.tech/project/mypy-boto3-pricing)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pricing 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
+[boto3.Pricing 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
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
 [mypy-boto3-pricing docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,29 +301,29 @@
 
 `mypy_boto3_pricing.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pricing.type_defs import (
     AttributeValueTypeDef,
-    DescribeServicesRequestDescribeServicesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeServicesRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ServiceTypeDef,
     FilterTypeDef,
-    GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
     GetAttributeValuesRequestRequestTypeDef,
     GetPriceListFileUrlRequestRequestTypeDef,
-    GetPriceListFileUrlResponseTypeDef,
-    GetProductsResponseTypeDef,
-    ListPriceListsRequestListPriceListsPaginateTypeDef,
     ListPriceListsRequestRequestTypeDef,
     PriceListTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    DescribeServicesRequestDescribeServicesPaginateTypeDef,
+    GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
+    ListPriceListsRequestListPriceListsPaginateTypeDef,
     GetAttributeValuesResponseTypeDef,
+    GetPriceListFileUrlResponseTypeDef,
+    GetProductsResponseTypeDef,
     DescribeServicesResponseTypeDef,
     GetProductsRequestGetProductsPaginateTypeDef,
     GetProductsRequestRequestTypeDef,
     ListPriceListsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/__init__.py` & `mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/__init__.pyi` & `mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/__main__.py` & `mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Pricing 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Pricing 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing\nOther"
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

### Comparing `mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/client.py` & `mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/client.pyi` & `mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/literals.py` & `mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,29 +14,27 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DescribeServicesPaginatorName",
     "FilterTypeType",
     "GetAttributeValuesPaginatorName",
     "GetProductsPaginatorName",
     "ListPriceListsPaginatorName",
     "PricingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DescribeServicesPaginatorName = Literal["describe_services"]
 FilterTypeType = Literal["TERM_MATCH"]
 GetAttributeValuesPaginatorName = Literal["get_attribute_values"]
 GetProductsPaginatorName = Literal["get_products"]
 ListPriceListsPaginatorName = Literal["list_price_lists"]
 PricingServiceName = Literal["pricing"]
 ServiceName = Literal[
@@ -154,14 +152,15 @@
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
@@ -240,26 +239,28 @@
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

### Comparing `mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/literals.pyi` & `mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,29 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DescribeServicesPaginatorName",
     "FilterTypeType",
     "GetAttributeValuesPaginatorName",
     "GetProductsPaginatorName",
     "ListPriceListsPaginatorName",
     "PricingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 DescribeServicesPaginatorName = Literal["describe_services"]
 FilterTypeType = Literal["TERM_MATCH"]
 GetAttributeValuesPaginatorName = Literal["get_attribute_values"]
 GetProductsPaginatorName = Literal["get_products"]
 ListPriceListsPaginatorName = Literal["list_price_lists"]
 PricingServiceName = Literal["pricing"]
 ServiceName = Literal[
@@ -152,14 +154,15 @@
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
@@ -238,26 +241,28 @@
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

### Comparing `mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/paginator.py` & `mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str = ...,
         FormatVersion: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.DescribeServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/paginators/#describeservicespaginator)
         """
 
 
@@ -83,15 +83,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str,
         AttributeName: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetAttributeValuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.GetAttributeValues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/paginators/#getattributevaluespaginator)
         """
 
 
@@ -103,15 +103,15 @@
 
     def paginate(
         self,
         *,
         ServiceCode: str,
         Filters: Sequence[FilterTypeDef] = ...,
         FormatVersion: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetProductsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.GetProducts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/paginators/#getproductspaginator)
         """
 
 
@@ -124,13 +124,13 @@
     def paginate(
         self,
         *,
         ServiceCode: str,
         EffectiveDate: Union[datetime, str],
         CurrencyCode: str,
         RegionCode: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPriceListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.ListPriceLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/paginators/#listpricelistspaginator)
         """
```

### Comparing `mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/paginator.pyi` & `mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str = ...,
         FormatVersion: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.DescribeServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/paginators/#describeservicespaginator)
         """
 
 class GetAttributeValuesPaginator(Paginator):
@@ -79,15 +79,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str,
         AttributeName: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetAttributeValuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.GetAttributeValues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/paginators/#getattributevaluespaginator)
         """
 
 class GetProductsPaginator(Paginator):
@@ -98,15 +98,15 @@
 
     def paginate(
         self,
         *,
         ServiceCode: str,
         Filters: Sequence[FilterTypeDef] = ...,
         FormatVersion: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetProductsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.GetProducts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/paginators/#getproductspaginator)
         """
 
 class ListPriceListsPaginator(Paginator):
@@ -118,13 +118,13 @@
     def paginate(
         self,
         *,
         ServiceCode: str,
         EffectiveDate: Union[datetime, str],
         CurrencyCode: str,
         RegionCode: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPriceListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.ListPriceLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/paginators/#listpricelistspaginator)
         """
```

### Comparing `mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/type_defs.py` & `mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,49 +23,49 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AttributeValueTypeDef",
-    "DescribeServicesRequestDescribeServicesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeServicesRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ServiceTypeDef",
     "FilterTypeDef",
-    "GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
     "GetAttributeValuesRequestRequestTypeDef",
     "GetPriceListFileUrlRequestRequestTypeDef",
-    "GetPriceListFileUrlResponseTypeDef",
-    "GetProductsResponseTypeDef",
-    "ListPriceListsRequestListPriceListsPaginateTypeDef",
     "ListPriceListsRequestRequestTypeDef",
     "PriceListTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "DescribeServicesRequestDescribeServicesPaginateTypeDef",
+    "GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
+    "ListPriceListsRequestListPriceListsPaginateTypeDef",
     "GetAttributeValuesResponseTypeDef",
+    "GetPriceListFileUrlResponseTypeDef",
+    "GetProductsResponseTypeDef",
     "DescribeServicesResponseTypeDef",
     "GetProductsRequestGetProductsPaginateTypeDef",
     "GetProductsRequestRequestTypeDef",
     "ListPriceListsResponseTypeDef",
 )
 
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-DescribeServicesRequestDescribeServicesPaginateTypeDef = TypedDict(
-    "DescribeServicesRequestDescribeServicesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ServiceCode": str,
-        "FormatVersion": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeServicesRequestRequestTypeDef = TypedDict(
     "DescribeServicesRequestRequestTypeDef",
     {
@@ -73,14 +73,25 @@
         "FormatVersion": str,
         "NextToken": str,
         "MaxResults": int,
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
 _RequiredServiceTypeDef = TypedDict(
     "_RequiredServiceTypeDef",
     {
         "ServiceCode": str,
     },
 )
 _OptionalServiceTypeDef = TypedDict(
@@ -101,37 +112,14 @@
     {
         "Type": Literal["TERM_MATCH"],
         "Field": str,
         "Value": str,
     },
 )
 
-_RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef = TypedDict(
-    "_RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "AttributeName": str,
-    },
-)
-_OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef = TypedDict(
-    "_OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef(
-    _RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
-    _OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetAttributeValuesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAttributeValuesRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "AttributeName": str,
     },
 )
@@ -156,57 +144,14 @@
     "GetPriceListFileUrlRequestRequestTypeDef",
     {
         "PriceListArn": str,
         "FileFormat": str,
     },
 )
 
-GetPriceListFileUrlResponseTypeDef = TypedDict(
-    "GetPriceListFileUrlResponseTypeDef",
-    {
-        "Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetProductsResponseTypeDef = TypedDict(
-    "GetProductsResponseTypeDef",
-    {
-        "FormatVersion": str,
-        "PriceList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
-    "_RequiredListPriceListsRequestListPriceListsPaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "EffectiveDate": Union[datetime, str],
-        "CurrencyCode": str,
-    },
-)
-_OptionalListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
-    "_OptionalListPriceListsRequestListPriceListsPaginateTypeDef",
-    {
-        "RegionCode": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPriceListsRequestListPriceListsPaginateTypeDef(
-    _RequiredListPriceListsRequestListPriceListsPaginateTypeDef,
-    _OptionalListPriceListsRequestListPriceListsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPriceListsRequestRequestTypeDef = TypedDict(
     "_RequiredListPriceListsRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "EffectiveDate": Union[datetime, str],
         "CurrencyCode": str,
     },
@@ -235,66 +180,121 @@
         "RegionCode": str,
         "CurrencyCode": str,
         "FileFormats": List[str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeServicesRequestDescribeServicesPaginateTypeDef = TypedDict(
+    "DescribeServicesRequestDescribeServicesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ServiceCode": str,
+        "FormatVersion": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef = TypedDict(
+    "_RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ServiceCode": str,
+        "AttributeName": str,
     },
 )
+_OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef = TypedDict(
+    "_OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef(
+    _RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
+    _OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
+    "_RequiredListPriceListsRequestListPriceListsPaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "EffectiveDate": Union[datetime, str],
+        "CurrencyCode": str,
+    },
+)
+_OptionalListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
+    "_OptionalListPriceListsRequestListPriceListsPaginateTypeDef",
+    {
+        "RegionCode": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPriceListsRequestListPriceListsPaginateTypeDef(
+    _RequiredListPriceListsRequestListPriceListsPaginateTypeDef,
+    _OptionalListPriceListsRequestListPriceListsPaginateTypeDef,
+):
+    pass
+
 
 GetAttributeValuesResponseTypeDef = TypedDict(
     "GetAttributeValuesResponseTypeDef",
     {
         "AttributeValues": List[AttributeValueTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPriceListFileUrlResponseTypeDef = TypedDict(
+    "GetPriceListFileUrlResponseTypeDef",
+    {
+        "Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetProductsResponseTypeDef = TypedDict(
+    "GetProductsResponseTypeDef",
+    {
+        "FormatVersion": str,
+        "PriceList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "Services": List[ServiceTypeDef],
         "FormatVersion": str,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetProductsRequestGetProductsPaginateTypeDef = TypedDict(
     "_RequiredGetProductsRequestGetProductsPaginateTypeDef",
     {
         "ServiceCode": str,
     },
 )
 _OptionalGetProductsRequestGetProductsPaginateTypeDef = TypedDict(
     "_OptionalGetProductsRequestGetProductsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "FormatVersion": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class GetProductsRequestGetProductsPaginateTypeDef(
     _RequiredGetProductsRequestGetProductsPaginateTypeDef,
@@ -328,10 +328,10 @@
 
 
 ListPriceListsResponseTypeDef = TypedDict(
     "ListPriceListsResponseTypeDef",
     {
         "PriceLists": List[PriceListTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-pricing-1.28.0/mypy_boto3_pricing/type_defs.pyi` & `mypy-boto3-pricing-1.28.12/mypy_boto3_pricing/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -22,49 +22,49 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AttributeValueTypeDef",
-    "DescribeServicesRequestDescribeServicesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeServicesRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ServiceTypeDef",
     "FilterTypeDef",
-    "GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
     "GetAttributeValuesRequestRequestTypeDef",
     "GetPriceListFileUrlRequestRequestTypeDef",
-    "GetPriceListFileUrlResponseTypeDef",
-    "GetProductsResponseTypeDef",
-    "ListPriceListsRequestListPriceListsPaginateTypeDef",
     "ListPriceListsRequestRequestTypeDef",
     "PriceListTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "DescribeServicesRequestDescribeServicesPaginateTypeDef",
+    "GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
+    "ListPriceListsRequestListPriceListsPaginateTypeDef",
     "GetAttributeValuesResponseTypeDef",
+    "GetPriceListFileUrlResponseTypeDef",
+    "GetProductsResponseTypeDef",
     "DescribeServicesResponseTypeDef",
     "GetProductsRequestGetProductsPaginateTypeDef",
     "GetProductsRequestRequestTypeDef",
     "ListPriceListsResponseTypeDef",
 )
 
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-DescribeServicesRequestDescribeServicesPaginateTypeDef = TypedDict(
-    "DescribeServicesRequestDescribeServicesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ServiceCode": str,
-        "FormatVersion": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeServicesRequestRequestTypeDef = TypedDict(
     "DescribeServicesRequestRequestTypeDef",
     {
@@ -72,14 +72,25 @@
         "FormatVersion": str,
         "NextToken": str,
         "MaxResults": int,
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
 _RequiredServiceTypeDef = TypedDict(
     "_RequiredServiceTypeDef",
     {
         "ServiceCode": str,
     },
 )
 _OptionalServiceTypeDef = TypedDict(
@@ -98,35 +109,14 @@
     {
         "Type": Literal["TERM_MATCH"],
         "Field": str,
         "Value": str,
     },
 )
 
-_RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef = TypedDict(
-    "_RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "AttributeName": str,
-    },
-)
-_OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef = TypedDict(
-    "_OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef(
-    _RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
-    _OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetAttributeValuesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAttributeValuesRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "AttributeName": str,
     },
 )
@@ -149,55 +139,14 @@
     "GetPriceListFileUrlRequestRequestTypeDef",
     {
         "PriceListArn": str,
         "FileFormat": str,
     },
 )
 
-GetPriceListFileUrlResponseTypeDef = TypedDict(
-    "GetPriceListFileUrlResponseTypeDef",
-    {
-        "Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetProductsResponseTypeDef = TypedDict(
-    "GetProductsResponseTypeDef",
-    {
-        "FormatVersion": str,
-        "PriceList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
-    "_RequiredListPriceListsRequestListPriceListsPaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "EffectiveDate": Union[datetime, str],
-        "CurrencyCode": str,
-    },
-)
-_OptionalListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
-    "_OptionalListPriceListsRequestListPriceListsPaginateTypeDef",
-    {
-        "RegionCode": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPriceListsRequestListPriceListsPaginateTypeDef(
-    _RequiredListPriceListsRequestListPriceListsPaginateTypeDef,
-    _OptionalListPriceListsRequestListPriceListsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPriceListsRequestRequestTypeDef = TypedDict(
     "_RequiredListPriceListsRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "EffectiveDate": Union[datetime, str],
         "CurrencyCode": str,
     },
@@ -224,66 +173,117 @@
         "RegionCode": str,
         "CurrencyCode": str,
         "FileFormats": List[str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeServicesRequestDescribeServicesPaginateTypeDef = TypedDict(
+    "DescribeServicesRequestDescribeServicesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ServiceCode": str,
+        "FormatVersion": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef = TypedDict(
+    "_RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ServiceCode": str,
+        "AttributeName": str,
     },
 )
+_OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef = TypedDict(
+    "_OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef(
+    _RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
+    _OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
+):
+    pass
+
+_RequiredListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
+    "_RequiredListPriceListsRequestListPriceListsPaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "EffectiveDate": Union[datetime, str],
+        "CurrencyCode": str,
+    },
+)
+_OptionalListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
+    "_OptionalListPriceListsRequestListPriceListsPaginateTypeDef",
+    {
+        "RegionCode": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPriceListsRequestListPriceListsPaginateTypeDef(
+    _RequiredListPriceListsRequestListPriceListsPaginateTypeDef,
+    _OptionalListPriceListsRequestListPriceListsPaginateTypeDef,
+):
+    pass
 
 GetAttributeValuesResponseTypeDef = TypedDict(
     "GetAttributeValuesResponseTypeDef",
     {
         "AttributeValues": List[AttributeValueTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPriceListFileUrlResponseTypeDef = TypedDict(
+    "GetPriceListFileUrlResponseTypeDef",
+    {
+        "Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetProductsResponseTypeDef = TypedDict(
+    "GetProductsResponseTypeDef",
+    {
+        "FormatVersion": str,
+        "PriceList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "Services": List[ServiceTypeDef],
         "FormatVersion": str,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetProductsRequestGetProductsPaginateTypeDef = TypedDict(
     "_RequiredGetProductsRequestGetProductsPaginateTypeDef",
     {
         "ServiceCode": str,
     },
 )
 _OptionalGetProductsRequestGetProductsPaginateTypeDef = TypedDict(
     "_OptionalGetProductsRequestGetProductsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "FormatVersion": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class GetProductsRequestGetProductsPaginateTypeDef(
     _RequiredGetProductsRequestGetProductsPaginateTypeDef,
     _OptionalGetProductsRequestGetProductsPaginateTypeDef,
@@ -313,10 +313,10 @@
     pass
 
 ListPriceListsResponseTypeDef = TypedDict(
     "ListPriceListsResponseTypeDef",
     {
         "PriceLists": List[PriceListTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-pricing-1.28.0/mypy_boto3_pricing.egg-info/PKG-INFO` & `mypy-boto3-pricing-1.28.12/mypy_boto3_pricing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pricing
-Version: 1.28.0
-Summary: Type annotations for boto3.Pricing 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Pricing 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-pricing"></a>
 
 # mypy-boto3-pricing
 
 [![PyPI - mypy-boto3-pricing](https://img.shields.io/pypi/v/mypy-boto3-pricing.svg?color=blue)](https://pypi.org/project/mypy-boto3-pricing)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pricing.svg?color=blue)](https://pypi.org/project/mypy-boto3-pricing)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pricing?color=blue)](https://pypistats.org/packages/mypy-boto3-pricing)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pricing)](https://pepy.tech/project/mypy-boto3-pricing)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pricing 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
+[boto3.Pricing 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
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
 [mypy-boto3-pricing docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,29 +333,29 @@
 
 `mypy_boto3_pricing.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pricing.type_defs import (
     AttributeValueTypeDef,
-    DescribeServicesRequestDescribeServicesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeServicesRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ServiceTypeDef,
     FilterTypeDef,
-    GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
     GetAttributeValuesRequestRequestTypeDef,
     GetPriceListFileUrlRequestRequestTypeDef,
-    GetPriceListFileUrlResponseTypeDef,
-    GetProductsResponseTypeDef,
-    ListPriceListsRequestListPriceListsPaginateTypeDef,
     ListPriceListsRequestRequestTypeDef,
     PriceListTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    DescribeServicesRequestDescribeServicesPaginateTypeDef,
+    GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
+    ListPriceListsRequestListPriceListsPaginateTypeDef,
     GetAttributeValuesResponseTypeDef,
+    GetPriceListFileUrlResponseTypeDef,
+    GetProductsResponseTypeDef,
     DescribeServicesResponseTypeDef,
     GetProductsRequestGetProductsPaginateTypeDef,
     GetProductsRequestRequestTypeDef,
     ListPriceListsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-pricing-1.28.0/mypy_boto3_pricing.egg-info/SOURCES.txt` & `mypy-boto3-pricing-1.28.12/mypy_boto3_pricing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.28.0/setup.py` & `mypy-boto3-pricing-1.28.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pricing",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_pricing"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Pricing 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Pricing 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

