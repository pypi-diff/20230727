# Comparing `tmp/mypy-boto3-marketplace-catalog-1.28.0.tar.gz` & `tmp/mypy-boto3-marketplace-catalog-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-marketplace-catalog-1.28.0.tar", last modified: Thu Jul  6 21:00:04 2023, max compression
+gzip compressed data, was "mypy-boto3-marketplace-catalog-1.28.12.tar", last modified: Thu Jul 27 05:34:59 2023, max compression
```

## Comparing `mypy-boto3-marketplace-catalog-1.28.0.tar` & `mypy-boto3-marketplace-catalog-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:04.602364 mypy-boto3-marketplace-catalog-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:46:34.000000 mypy-boto3-marketplace-catalog-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14539 2023-07-06 21:00:04.602364 mypy-boto3-marketplace-catalog-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13007 2023-07-06 20:46:34.000000 mypy-boto3-marketplace-catalog-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:04.586364 mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-06 20:46:34.000000 mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-06 20:46:34.000000 mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-06 20:46:34.000000 mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-07-06 20:46:34.000000 mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-07-06 20:46:34.000000 mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-07-06 20:46:36.000000 mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-07-06 20:46:36.000000 mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-06 20:46:34.000000 mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-06 20:46:34.000000 mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:46:34.000000 mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-07-06 20:46:37.000000 mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-07-06 20:46:37.000000 mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:46:34.000000 mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:04.602364 mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14539 2023-07-06 21:00:04.000000 mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 21:00:04.000000 mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:04.000000 mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:04.000000 mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:04.000000 mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 21:00:04.000000 mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:04.602364 mypy-boto3-marketplace-catalog-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-06 20:46:34.000000 mypy-boto3-marketplace-catalog-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.924445 mypy-boto3-marketplace-catalog-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-07-27 05:34:59.924445 mypy-boto3-marketplace-catalog-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13039 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.920445 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.924445 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-07-27 05:34:59.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-27 05:34:59.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:59.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:59.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:59.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 05:34:59.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:59.924445 mypy-boto3-marketplace-catalog-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/setup.py
```

### Comparing `mypy-boto3-marketplace-catalog-1.28.0/LICENSE` & `mypy-boto3-marketplace-catalog-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.0/PKG-INFO` & `mypy-boto3-marketplace-catalog-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-marketplace-catalog
-Version: 1.28.0
-Summary: Type annotations for boto3.MarketplaceCatalog 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MarketplaceCatalog 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-marketplace-catalog"></a>
 
 # mypy-boto3-marketplace-catalog
 
 [![PyPI - mypy-boto3-marketplace-catalog](https://img.shields.io/pypi/v/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-marketplace-catalog?color=blue)](https://pypistats.org/packages/mypy-boto3-marketplace-catalog)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-marketplace-catalog)](https://pepy.tech/project/mypy-boto3-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceCatalog 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
+[boto3.MarketplaceCatalog 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
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
 [mypy-boto3-marketplace-catalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,42 +329,44 @@
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_marketplace_catalog.type_defs import (
     CancelChangeSetRequestRequestTypeDef,
     CancelChangeSetResponseTypeDef,
     ChangeSetSummaryListItemTypeDef,
-    EntityTypeDef,
+    EntityOutputTypeDef,
     ErrorDetailTypeDef,
+    EntityTypeDef,
     TagTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DescribeChangeSetRequestRequestTypeDef,
     DescribeEntityRequestRequestTypeDef,
     DescribeEntityResponseTypeDef,
     EntitySummaryTypeDef,
     FilterTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
     GetResourcePolicyResponseTypeDef,
     SortTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     StartChangeSetResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     ListChangeSetsResponseTypeDef,
     ChangeSummaryTypeDef,
     ChangeTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEntitiesResponseTypeDef,
     ListChangeSetsRequestListChangeSetsPaginateTypeDef,
     ListChangeSetsRequestRequestTypeDef,
     ListEntitiesRequestListEntitiesPaginateTypeDef,
     ListEntitiesRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DescribeChangeSetResponseTypeDef,
     StartChangeSetRequestRequestTypeDef,
 )
 
 
 def get_structure() -> CancelChangeSetRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-marketplace-catalog-1.28.0/README.md` & `mypy-boto3-marketplace-catalog-1.28.12/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-marketplace-catalog"></a>
 
 # mypy-boto3-marketplace-catalog
 
 [![PyPI - mypy-boto3-marketplace-catalog](https://img.shields.io/pypi/v/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-marketplace-catalog?color=blue)](https://pypistats.org/packages/mypy-boto3-marketplace-catalog)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-marketplace-catalog)](https://pepy.tech/project/mypy-boto3-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceCatalog 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
+[boto3.MarketplaceCatalog 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
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
 [mypy-boto3-marketplace-catalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,42 +297,44 @@
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_marketplace_catalog.type_defs import (
     CancelChangeSetRequestRequestTypeDef,
     CancelChangeSetResponseTypeDef,
     ChangeSetSummaryListItemTypeDef,
-    EntityTypeDef,
+    EntityOutputTypeDef,
     ErrorDetailTypeDef,
+    EntityTypeDef,
     TagTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DescribeChangeSetRequestRequestTypeDef,
     DescribeEntityRequestRequestTypeDef,
     DescribeEntityResponseTypeDef,
     EntitySummaryTypeDef,
     FilterTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
     GetResourcePolicyResponseTypeDef,
     SortTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     StartChangeSetResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     ListChangeSetsResponseTypeDef,
     ChangeSummaryTypeDef,
     ChangeTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEntitiesResponseTypeDef,
     ListChangeSetsRequestListChangeSetsPaginateTypeDef,
     ListChangeSetsRequestRequestTypeDef,
     ListEntitiesRequestListEntitiesPaginateTypeDef,
     ListEntitiesRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DescribeChangeSetResponseTypeDef,
     StartChangeSetRequestRequestTypeDef,
 )
 
 
 def get_structure() -> CancelChangeSetRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/__init__.py` & `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/__init__.pyi` & `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/__main__.py` & `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MarketplaceCatalog 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.MarketplaceCatalog 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog\nOther"
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

### Comparing `mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/client.py` & `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/client.pyi` & `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/literals.py` & `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,14 +156,15 @@
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
@@ -242,26 +243,28 @@
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

### Comparing `mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/literals.pyi` & `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -154,14 +154,15 @@
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
@@ -240,26 +241,28 @@
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

### Comparing `mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/paginator.py` & `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/paginator.pyi` & `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/type_defs.py` & `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,42 +22,44 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CancelChangeSetRequestRequestTypeDef",
     "CancelChangeSetResponseTypeDef",
     "ChangeSetSummaryListItemTypeDef",
-    "EntityTypeDef",
+    "EntityOutputTypeDef",
     "ErrorDetailTypeDef",
+    "EntityTypeDef",
     "TagTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DescribeChangeSetRequestRequestTypeDef",
     "DescribeEntityRequestRequestTypeDef",
     "DescribeEntityResponseTypeDef",
     "EntitySummaryTypeDef",
     "FilterTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
     "GetResourcePolicyResponseTypeDef",
     "SortTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "StartChangeSetResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ListChangeSetsResponseTypeDef",
     "ChangeSummaryTypeDef",
     "ChangeTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEntitiesResponseTypeDef",
     "ListChangeSetsRequestListChangeSetsPaginateTypeDef",
     "ListChangeSetsRequestRequestTypeDef",
     "ListEntitiesRequestListEntitiesPaginateTypeDef",
     "ListEntitiesRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "DescribeChangeSetResponseTypeDef",
     "StartChangeSetRequestRequestTypeDef",
 )
 
 CancelChangeSetRequestRequestTypeDef = TypedDict(
     "CancelChangeSetRequestRequestTypeDef",
     {
@@ -86,42 +88,61 @@
         "Status": ChangeStatusType,
         "EntityIdList": List[str],
         "FailureCode": FailureCodeType,
     },
     total=False,
 )
 
-_RequiredEntityTypeDef = TypedDict(
-    "_RequiredEntityTypeDef",
+_RequiredEntityOutputTypeDef = TypedDict(
+    "_RequiredEntityOutputTypeDef",
     {
         "Type": str,
     },
 )
-_OptionalEntityTypeDef = TypedDict(
-    "_OptionalEntityTypeDef",
+_OptionalEntityOutputTypeDef = TypedDict(
+    "_OptionalEntityOutputTypeDef",
     {
         "Identifier": str,
     },
     total=False,
 )
 
 
-class EntityTypeDef(_RequiredEntityTypeDef, _OptionalEntityTypeDef):
+class EntityOutputTypeDef(_RequiredEntityOutputTypeDef, _OptionalEntityOutputTypeDef):
     pass
 
 
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+_RequiredEntityTypeDef = TypedDict(
+    "_RequiredEntityTypeDef",
+    {
+        "Type": str,
+    },
+)
+_OptionalEntityTypeDef = TypedDict(
+    "_OptionalEntityTypeDef",
+    {
+        "Identifier": str,
+    },
+    total=False,
+)
+
+
+class EntityTypeDef(_RequiredEntityTypeDef, _OptionalEntityTypeDef):
+    pass
+
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -210,14 +231,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -269,15 +298,15 @@
     },
 )
 
 ChangeSummaryTypeDef = TypedDict(
     "ChangeSummaryTypeDef",
     {
         "ChangeType": str,
-        "Entity": EntityTypeDef,
+        "Entity": EntityOutputTypeDef,
         "Details": str,
         "ErrorDetailList": List[ErrorDetailTypeDef],
         "ChangeName": str,
     },
     total=False,
 )
 
@@ -299,23 +328,14 @@
 )
 
 
 class ChangeTypeDef(_RequiredChangeTypeDef, _OptionalChangeTypeDef):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -425,14 +445,23 @@
 
 class ListEntitiesRequestRequestTypeDef(
     _RequiredListEntitiesRequestRequestTypeDef, _OptionalListEntitiesRequestRequestTypeDef
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeChangeSetResponseTypeDef = TypedDict(
     "DescribeChangeSetResponseTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetArn": str,
         "ChangeSetName": str,
         "StartTime": str,
```

### Comparing `mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog/type_defs.pyi` & `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -21,42 +21,44 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CancelChangeSetRequestRequestTypeDef",
     "CancelChangeSetResponseTypeDef",
     "ChangeSetSummaryListItemTypeDef",
-    "EntityTypeDef",
+    "EntityOutputTypeDef",
     "ErrorDetailTypeDef",
+    "EntityTypeDef",
     "TagTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DescribeChangeSetRequestRequestTypeDef",
     "DescribeEntityRequestRequestTypeDef",
     "DescribeEntityResponseTypeDef",
     "EntitySummaryTypeDef",
     "FilterTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
     "GetResourcePolicyResponseTypeDef",
     "SortTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "StartChangeSetResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ListChangeSetsResponseTypeDef",
     "ChangeSummaryTypeDef",
     "ChangeTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEntitiesResponseTypeDef",
     "ListChangeSetsRequestListChangeSetsPaginateTypeDef",
     "ListChangeSetsRequestRequestTypeDef",
     "ListEntitiesRequestListEntitiesPaginateTypeDef",
     "ListEntitiesRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "DescribeChangeSetResponseTypeDef",
     "StartChangeSetRequestRequestTypeDef",
 )
 
 CancelChangeSetRequestRequestTypeDef = TypedDict(
     "CancelChangeSetRequestRequestTypeDef",
     {
@@ -85,40 +87,57 @@
         "Status": ChangeStatusType,
         "EntityIdList": List[str],
         "FailureCode": FailureCodeType,
     },
     total=False,
 )
 
-_RequiredEntityTypeDef = TypedDict(
-    "_RequiredEntityTypeDef",
+_RequiredEntityOutputTypeDef = TypedDict(
+    "_RequiredEntityOutputTypeDef",
     {
         "Type": str,
     },
 )
-_OptionalEntityTypeDef = TypedDict(
-    "_OptionalEntityTypeDef",
+_OptionalEntityOutputTypeDef = TypedDict(
+    "_OptionalEntityOutputTypeDef",
     {
         "Identifier": str,
     },
     total=False,
 )
 
-class EntityTypeDef(_RequiredEntityTypeDef, _OptionalEntityTypeDef):
+class EntityOutputTypeDef(_RequiredEntityOutputTypeDef, _OptionalEntityOutputTypeDef):
     pass
 
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+_RequiredEntityTypeDef = TypedDict(
+    "_RequiredEntityTypeDef",
+    {
+        "Type": str,
+    },
+)
+_OptionalEntityTypeDef = TypedDict(
+    "_OptionalEntityTypeDef",
+    {
+        "Identifier": str,
+    },
+    total=False,
+)
+
+class EntityTypeDef(_RequiredEntityTypeDef, _OptionalEntityTypeDef):
+    pass
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -207,14 +226,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -266,15 +293,15 @@
     },
 )
 
 ChangeSummaryTypeDef = TypedDict(
     "ChangeSummaryTypeDef",
     {
         "ChangeType": str,
-        "Entity": EntityTypeDef,
+        "Entity": EntityOutputTypeDef,
         "Details": str,
         "ErrorDetailList": List[ErrorDetailTypeDef],
         "ChangeName": str,
     },
     total=False,
 )
 
@@ -294,23 +321,14 @@
     },
     total=False,
 )
 
 class ChangeTypeDef(_RequiredChangeTypeDef, _OptionalChangeTypeDef):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -412,14 +430,23 @@
 )
 
 class ListEntitiesRequestRequestTypeDef(
     _RequiredListEntitiesRequestRequestTypeDef, _OptionalListEntitiesRequestRequestTypeDef
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeChangeSetResponseTypeDef = TypedDict(
     "DescribeChangeSetResponseTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetArn": str,
         "ChangeSetName": str,
         "StartTime": str,
```

### Comparing `mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog.egg-info/PKG-INFO` & `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-marketplace-catalog
-Version: 1.28.0
-Summary: Type annotations for boto3.MarketplaceCatalog 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MarketplaceCatalog 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-marketplace-catalog"></a>
 
 # mypy-boto3-marketplace-catalog
 
 [![PyPI - mypy-boto3-marketplace-catalog](https://img.shields.io/pypi/v/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-marketplace-catalog?color=blue)](https://pypistats.org/packages/mypy-boto3-marketplace-catalog)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-marketplace-catalog)](https://pepy.tech/project/mypy-boto3-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceCatalog 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
+[boto3.MarketplaceCatalog 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
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
 [mypy-boto3-marketplace-catalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,42 +329,44 @@
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_marketplace_catalog.type_defs import (
     CancelChangeSetRequestRequestTypeDef,
     CancelChangeSetResponseTypeDef,
     ChangeSetSummaryListItemTypeDef,
-    EntityTypeDef,
+    EntityOutputTypeDef,
     ErrorDetailTypeDef,
+    EntityTypeDef,
     TagTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DescribeChangeSetRequestRequestTypeDef,
     DescribeEntityRequestRequestTypeDef,
     DescribeEntityResponseTypeDef,
     EntitySummaryTypeDef,
     FilterTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
     GetResourcePolicyResponseTypeDef,
     SortTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     StartChangeSetResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     ListChangeSetsResponseTypeDef,
     ChangeSummaryTypeDef,
     ChangeTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEntitiesResponseTypeDef,
     ListChangeSetsRequestListChangeSetsPaginateTypeDef,
     ListChangeSetsRequestRequestTypeDef,
     ListEntitiesRequestListEntitiesPaginateTypeDef,
     ListEntitiesRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DescribeChangeSetResponseTypeDef,
     StartChangeSetRequestRequestTypeDef,
 )
 
 
 def get_structure() -> CancelChangeSetRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-marketplace-catalog-1.28.0/mypy_boto3_marketplace_catalog.egg-info/SOURCES.txt` & `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.0/setup.py` & `mypy-boto3-marketplace-catalog-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-marketplace-catalog",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_marketplace_catalog"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MarketplaceCatalog 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.MarketplaceCatalog 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

