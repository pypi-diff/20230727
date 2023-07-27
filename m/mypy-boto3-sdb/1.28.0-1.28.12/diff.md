# Comparing `tmp/mypy-boto3-sdb-1.28.0.tar.gz` & `tmp/mypy-boto3-sdb-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sdb-1.28.0.tar", last modified: Thu Jul  6 21:00:35 2023, max compression
+gzip compressed data, was "mypy-boto3-sdb-1.28.12.tar", last modified: Thu Jul 27 11:49:36 2023, max compression
```

## Comparing `mypy-boto3-sdb-1.28.0.tar` & `mypy-boto3-sdb-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:35.338426 mypy-boto3-sdb-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:55:00.000000 mypy-boto3-sdb-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-06 21:00:35.330426 mypy-boto3-sdb-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-07-06 20:55:00.000000 mypy-boto3-sdb-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:35.318426 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-06 20:55:00.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-06 20:55:00.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-06 20:55:00.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10495 2023-07-06 20:55:01.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-07-06 20:55:00.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-07-06 20:55:01.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-07-06 20:55:01.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-06 20:55:01.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-06 20:55:01.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:55:00.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-07-06 20:55:01.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-07-06 20:55:01.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:55:00.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:35.330426 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-06 21:00:35.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 21:00:35.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:35.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:35.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:35.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 21:00:35.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:35.338426 mypy-boto3-sdb-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-06 20:55:00.000000 mypy-boto3-sdb-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:36.157268 mypy-boto3-sdb-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:06.000000 mypy-boto3-sdb-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13262 2023-07-27 11:49:36.157268 mypy-boto3-sdb-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-07-27 11:46:06.000000 mypy-boto3-sdb-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:36.153268 mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-27 11:46:06.000000 mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-27 11:46:06.000000 mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-27 11:46:06.000000 mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10495 2023-07-27 11:46:06.000000 mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-07-27 11:46:06.000000 mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-07-27 11:46:06.000000 mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-07-27 11:46:06.000000 mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-27 11:46:06.000000 mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-27 11:46:06.000000 mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:06.000000 mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-07-27 11:46:06.000000 mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-07-27 11:46:06.000000 mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:06.000000 mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:36.157268 mypy-boto3-sdb-1.28.12/mypy_boto3_sdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13262 2023-07-27 11:49:35.000000 mypy-boto3-sdb-1.28.12/mypy_boto3_sdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 11:49:35.000000 mypy-boto3-sdb-1.28.12/mypy_boto3_sdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:35.000000 mypy-boto3-sdb-1.28.12/mypy_boto3_sdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:35.000000 mypy-boto3-sdb-1.28.12/mypy_boto3_sdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:35.000000 mypy-boto3-sdb-1.28.12/mypy_boto3_sdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:35.000000 mypy-boto3-sdb-1.28.12/mypy_boto3_sdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:36.157268 mypy-boto3-sdb-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-27 11:46:06.000000 mypy-boto3-sdb-1.28.12/setup.py
```

### Comparing `mypy-boto3-sdb-1.28.0/LICENSE` & `mypy-boto3-sdb-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.28.0/PKG-INFO` & `mypy-boto3-sdb-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sdb
-Version: 1.28.0
-Summary: Type annotations for boto3.SimpleDB 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SimpleDB 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sdb"></a>
 
 # mypy-boto3-sdb
 
 [![PyPI - mypy-boto3-sdb](https://img.shields.io/pypi/v/mypy-boto3-sdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-sdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-sdb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sdb?color=blue)](https://pypistats.org/packages/mypy-boto3-sdb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sdb)](https://pepy.tech/project/mypy-boto3-sdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SimpleDB 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
+[boto3.SimpleDB 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
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
 [mypy-boto3-sdb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -319,43 +319,44 @@
 ### Typed dictionaries
 
 `mypy_boto3_sdb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sdb.type_defs import (
+    AttributeOutputTypeDef,
     AttributeTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateConditionTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainMetadataRequestRequestTypeDef,
-    DomainMetadataResultTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetAttributesRequestRequestTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
-    ListDomainsRequestRequestTypeDef,
-    ListDomainsResultTypeDef,
     PaginatorConfigTypeDef,
+    ListDomainsRequestRequestTypeDef,
     ReplaceableAttributeTypeDef,
-    ResponseMetadataTypeDef,
     SelectRequestRequestTypeDef,
-    SelectRequestSelectPaginateTypeDef,
-    DeletableItemTypeDef,
-    GetAttributesResultTypeDef,
     ItemTypeDef,
+    DeletableItemTypeDef,
     DeleteAttributesRequestRequestTypeDef,
+    DomainMetadataResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAttributesResultTypeDef,
+    ListDomainsResultTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
+    SelectRequestSelectPaginateTypeDef,
     PutAttributesRequestRequestTypeDef,
     ReplaceableItemTypeDef,
-    BatchDeleteAttributesRequestRequestTypeDef,
     SelectResultTypeDef,
+    BatchDeleteAttributesRequestRequestTypeDef,
     BatchPutAttributesRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AttributeTypeDef:
+def get_structure() -> AttributeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sdb-1.28.0/README.md` & `mypy-boto3-sdb-1.28.12/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sdb"></a>
 
 # mypy-boto3-sdb
 
 [![PyPI - mypy-boto3-sdb](https://img.shields.io/pypi/v/mypy-boto3-sdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-sdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-sdb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sdb?color=blue)](https://pypistats.org/packages/mypy-boto3-sdb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sdb)](https://pepy.tech/project/mypy-boto3-sdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SimpleDB 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
+[boto3.SimpleDB 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
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
 [mypy-boto3-sdb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -287,43 +287,44 @@
 ### Typed dictionaries
 
 `mypy_boto3_sdb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sdb.type_defs import (
+    AttributeOutputTypeDef,
     AttributeTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateConditionTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainMetadataRequestRequestTypeDef,
-    DomainMetadataResultTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetAttributesRequestRequestTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
-    ListDomainsRequestRequestTypeDef,
-    ListDomainsResultTypeDef,
     PaginatorConfigTypeDef,
+    ListDomainsRequestRequestTypeDef,
     ReplaceableAttributeTypeDef,
-    ResponseMetadataTypeDef,
     SelectRequestRequestTypeDef,
-    SelectRequestSelectPaginateTypeDef,
-    DeletableItemTypeDef,
-    GetAttributesResultTypeDef,
     ItemTypeDef,
+    DeletableItemTypeDef,
     DeleteAttributesRequestRequestTypeDef,
+    DomainMetadataResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAttributesResultTypeDef,
+    ListDomainsResultTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
+    SelectRequestSelectPaginateTypeDef,
     PutAttributesRequestRequestTypeDef,
     ReplaceableItemTypeDef,
-    BatchDeleteAttributesRequestRequestTypeDef,
     SelectResultTypeDef,
+    BatchDeleteAttributesRequestRequestTypeDef,
     BatchPutAttributesRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AttributeTypeDef:
+def get_structure() -> AttributeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/__init__.py` & `mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/__init__.pyi` & `mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/__main__.py` & `mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SimpleDB 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.SimpleDB 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB\nOther"
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

### Comparing `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/client.py` & `mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/client.pyi` & `mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/literals.py` & `mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,14 +148,15 @@
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
@@ -234,26 +235,28 @@
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

### Comparing `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/literals.pyi` & `mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,15 @@
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
@@ -232,26 +233,28 @@
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

### Comparing `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/paginator.py` & `mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 class ListDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.ListDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/paginators/#listdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDomainsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/paginators/#listdomainspaginator)
         """
 
 
@@ -62,13 +62,13 @@
     """
 
     def paginate(
         self,
         *,
         SelectExpression: str,
         ConsistentRead: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SelectResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.Select.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/paginators/#selectpaginator)
         """
```

### Comparing `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/paginator.pyi` & `mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 class ListDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.ListDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/paginators/#listdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDomainsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/paginators/#listdomainspaginator)
         """
 
 class SelectPaginator(Paginator):
@@ -58,13 +58,13 @@
     """
 
     def paginate(
         self,
         *,
         SelectExpression: str,
         ConsistentRead: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SelectResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.Select.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/paginators/#selectpaginator)
         """
```

### Comparing `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/type_defs.py` & `mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -2,56 +2,75 @@
 Type annotations for sdb service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_sdb.type_defs import AttributeTypeDef
+    from mypy_boto3_sdb.type_defs import AttributeOutputTypeDef
 
-    data: AttributeTypeDef = {...}
+    data: AttributeOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "AttributeOutputTypeDef",
     "AttributeTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateConditionTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DomainMetadataRequestRequestTypeDef",
-    "DomainMetadataResultTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "GetAttributesRequestRequestTypeDef",
-    "ListDomainsRequestListDomainsPaginateTypeDef",
-    "ListDomainsRequestRequestTypeDef",
-    "ListDomainsResultTypeDef",
     "PaginatorConfigTypeDef",
+    "ListDomainsRequestRequestTypeDef",
     "ReplaceableAttributeTypeDef",
-    "ResponseMetadataTypeDef",
     "SelectRequestRequestTypeDef",
-    "SelectRequestSelectPaginateTypeDef",
-    "DeletableItemTypeDef",
-    "GetAttributesResultTypeDef",
     "ItemTypeDef",
+    "DeletableItemTypeDef",
     "DeleteAttributesRequestRequestTypeDef",
+    "DomainMetadataResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAttributesResultTypeDef",
+    "ListDomainsResultTypeDef",
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    "SelectRequestSelectPaginateTypeDef",
     "PutAttributesRequestRequestTypeDef",
     "ReplaceableItemTypeDef",
-    "BatchDeleteAttributesRequestRequestTypeDef",
     "SelectResultTypeDef",
+    "BatchDeleteAttributesRequestRequestTypeDef",
     "BatchPutAttributesRequestRequestTypeDef",
 )
 
+_RequiredAttributeOutputTypeDef = TypedDict(
+    "_RequiredAttributeOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
+_OptionalAttributeOutputTypeDef = TypedDict(
+    "_OptionalAttributeOutputTypeDef",
+    {
+        "AlternateNameEncoding": str,
+        "AlternateValueEncoding": str,
+    },
+    total=False,
+)
+
+class AttributeOutputTypeDef(_RequiredAttributeOutputTypeDef, _OptionalAttributeOutputTypeDef):
+    pass
+
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -60,19 +79,17 @@
     {
         "AlternateNameEncoding": str,
         "AlternateValueEncoding": str,
     },
     total=False,
 )
 
-
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
-
 CreateDomainRequestRequestTypeDef = TypedDict(
     "CreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
@@ -96,32 +113,22 @@
 DomainMetadataRequestRequestTypeDef = TypedDict(
     "DomainMetadataRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-DomainMetadataResultTypeDef = TypedDict(
-    "DomainMetadataResultTypeDef",
-    {
-        "ItemCount": int,
-        "ItemNamesSizeBytes": int,
-        "AttributeNameCount": int,
-        "AttributeNamesSizeBytes": int,
-        "AttributeValueCount": int,
-        "AttributeValuesSizeBytes": int,
-        "Timestamp": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredGetAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAttributesRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -133,57 +140,38 @@
     {
         "AttributeNames": Sequence[str],
         "ConsistentRead": bool,
     },
     total=False,
 )
 
-
 class GetAttributesRequestRequestTypeDef(
     _RequiredGetAttributesRequestRequestTypeDef, _OptionalGetAttributesRequestRequestTypeDef
 ):
     pass
 
-
-ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
-    "ListDomainsRequestListDomainsPaginateTypeDef",
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
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "MaxNumberOfDomains": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListDomainsResultTypeDef = TypedDict(
-    "ListDomainsResultTypeDef",
-    {
-        "DomainNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 _RequiredReplaceableAttributeTypeDef = TypedDict(
     "_RequiredReplaceableAttributeTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -191,32 +179,19 @@
     "_OptionalReplaceableAttributeTypeDef",
     {
         "Replace": bool,
     },
     total=False,
 )
 
-
 class ReplaceableAttributeTypeDef(
     _RequiredReplaceableAttributeTypeDef, _OptionalReplaceableAttributeTypeDef
 ):
     pass
 
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
 _RequiredSelectRequestRequestTypeDef = TypedDict(
     "_RequiredSelectRequestRequestTypeDef",
     {
         "SelectExpression": str,
     },
 )
 _OptionalSelectRequestRequestTypeDef = TypedDict(
@@ -224,113 +199,141 @@
     {
         "NextToken": str,
         "ConsistentRead": bool,
     },
     total=False,
 )
 
-
 class SelectRequestRequestTypeDef(
     _RequiredSelectRequestRequestTypeDef, _OptionalSelectRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredSelectRequestSelectPaginateTypeDef = TypedDict(
-    "_RequiredSelectRequestSelectPaginateTypeDef",
+_RequiredItemTypeDef = TypedDict(
+    "_RequiredItemTypeDef",
     {
-        "SelectExpression": str,
+        "Name": str,
+        "Attributes": List[AttributeOutputTypeDef],
     },
 )
-_OptionalSelectRequestSelectPaginateTypeDef = TypedDict(
-    "_OptionalSelectRequestSelectPaginateTypeDef",
+_OptionalItemTypeDef = TypedDict(
+    "_OptionalItemTypeDef",
     {
-        "ConsistentRead": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "AlternateNameEncoding": str,
     },
     total=False,
 )
 
-
-class SelectRequestSelectPaginateTypeDef(
-    _RequiredSelectRequestSelectPaginateTypeDef, _OptionalSelectRequestSelectPaginateTypeDef
-):
+class ItemTypeDef(_RequiredItemTypeDef, _OptionalItemTypeDef):
     pass
 
-
 _RequiredDeletableItemTypeDef = TypedDict(
     "_RequiredDeletableItemTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDeletableItemTypeDef = TypedDict(
     "_OptionalDeletableItemTypeDef",
     {
         "Attributes": Sequence[AttributeTypeDef],
     },
     total=False,
 )
 
-
 class DeletableItemTypeDef(_RequiredDeletableItemTypeDef, _OptionalDeletableItemTypeDef):
     pass
 
+_RequiredDeleteAttributesRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteAttributesRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "ItemName": str,
+    },
+)
+_OptionalDeleteAttributesRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteAttributesRequestRequestTypeDef",
+    {
+        "Attributes": Sequence[AttributeTypeDef],
+        "Expected": UpdateConditionTypeDef,
+    },
+    total=False,
+)
+
+class DeleteAttributesRequestRequestTypeDef(
+    _RequiredDeleteAttributesRequestRequestTypeDef, _OptionalDeleteAttributesRequestRequestTypeDef
+):
+    pass
+
+DomainMetadataResultTypeDef = TypedDict(
+    "DomainMetadataResultTypeDef",
+    {
+        "ItemCount": int,
+        "ItemNamesSizeBytes": int,
+        "AttributeNameCount": int,
+        "AttributeNamesSizeBytes": int,
+        "AttributeValueCount": int,
+        "AttributeValuesSizeBytes": int,
+        "Timestamp": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 GetAttributesResultTypeDef = TypedDict(
     "GetAttributesResultTypeDef",
     {
-        "Attributes": List[AttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Attributes": List[AttributeOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredItemTypeDef = TypedDict(
-    "_RequiredItemTypeDef",
+ListDomainsResultTypeDef = TypedDict(
+    "ListDomainsResultTypeDef",
     {
-        "Name": str,
-        "Attributes": List[AttributeTypeDef],
+        "DomainNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalItemTypeDef = TypedDict(
-    "_OptionalItemTypeDef",
+
+ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
+    "ListDomainsRequestListDomainsPaginateTypeDef",
     {
-        "AlternateNameEncoding": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class ItemTypeDef(_RequiredItemTypeDef, _OptionalItemTypeDef):
-    pass
-
-
-_RequiredDeleteAttributesRequestRequestTypeDef = TypedDict(
-    "_RequiredDeleteAttributesRequestRequestTypeDef",
+_RequiredSelectRequestSelectPaginateTypeDef = TypedDict(
+    "_RequiredSelectRequestSelectPaginateTypeDef",
     {
-        "DomainName": str,
-        "ItemName": str,
+        "SelectExpression": str,
     },
 )
-_OptionalDeleteAttributesRequestRequestTypeDef = TypedDict(
-    "_OptionalDeleteAttributesRequestRequestTypeDef",
+_OptionalSelectRequestSelectPaginateTypeDef = TypedDict(
+    "_OptionalSelectRequestSelectPaginateTypeDef",
     {
-        "Attributes": Sequence[AttributeTypeDef],
-        "Expected": UpdateConditionTypeDef,
+        "ConsistentRead": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class DeleteAttributesRequestRequestTypeDef(
-    _RequiredDeleteAttributesRequestRequestTypeDef, _OptionalDeleteAttributesRequestRequestTypeDef
+class SelectRequestSelectPaginateTypeDef(
+    _RequiredSelectRequestSelectPaginateTypeDef, _OptionalSelectRequestSelectPaginateTypeDef
 ):
     pass
 
-
 _RequiredPutAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutAttributesRequestRequestTypeDef",
     {
         "DomainName": str,
         "ItemName": str,
         "Attributes": Sequence[ReplaceableAttributeTypeDef],
     },
@@ -339,43 +342,41 @@
     "_OptionalPutAttributesRequestRequestTypeDef",
     {
         "Expected": UpdateConditionTypeDef,
     },
     total=False,
 )
 
-
 class PutAttributesRequestRequestTypeDef(
     _RequiredPutAttributesRequestRequestTypeDef, _OptionalPutAttributesRequestRequestTypeDef
 ):
     pass
 
-
 ReplaceableItemTypeDef = TypedDict(
     "ReplaceableItemTypeDef",
     {
         "Name": str,
         "Attributes": Sequence[ReplaceableAttributeTypeDef],
     },
 )
 
-BatchDeleteAttributesRequestRequestTypeDef = TypedDict(
-    "BatchDeleteAttributesRequestRequestTypeDef",
-    {
-        "DomainName": str,
-        "Items": Sequence[DeletableItemTypeDef],
-    },
-)
-
 SelectResultTypeDef = TypedDict(
     "SelectResultTypeDef",
     {
         "Items": List[ItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchDeleteAttributesRequestRequestTypeDef = TypedDict(
+    "BatchDeleteAttributesRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "Items": Sequence[DeletableItemTypeDef],
     },
 )
 
 BatchPutAttributesRequestRequestTypeDef = TypedDict(
     "BatchPutAttributesRequestRequestTypeDef",
     {
         "DomainName": str,
```

### Comparing `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/type_defs.pyi` & `mypy-boto3-sdb-1.28.12/mypy_boto3_sdb/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,55 +2,78 @@
 Type annotations for sdb service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_sdb.type_defs import AttributeTypeDef
+    from mypy_boto3_sdb.type_defs import AttributeOutputTypeDef
 
-    data: AttributeTypeDef = {...}
+    data: AttributeOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "AttributeOutputTypeDef",
     "AttributeTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateConditionTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DomainMetadataRequestRequestTypeDef",
-    "DomainMetadataResultTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "GetAttributesRequestRequestTypeDef",
-    "ListDomainsRequestListDomainsPaginateTypeDef",
-    "ListDomainsRequestRequestTypeDef",
-    "ListDomainsResultTypeDef",
     "PaginatorConfigTypeDef",
+    "ListDomainsRequestRequestTypeDef",
     "ReplaceableAttributeTypeDef",
-    "ResponseMetadataTypeDef",
     "SelectRequestRequestTypeDef",
-    "SelectRequestSelectPaginateTypeDef",
-    "DeletableItemTypeDef",
-    "GetAttributesResultTypeDef",
     "ItemTypeDef",
+    "DeletableItemTypeDef",
     "DeleteAttributesRequestRequestTypeDef",
+    "DomainMetadataResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAttributesResultTypeDef",
+    "ListDomainsResultTypeDef",
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    "SelectRequestSelectPaginateTypeDef",
     "PutAttributesRequestRequestTypeDef",
     "ReplaceableItemTypeDef",
-    "BatchDeleteAttributesRequestRequestTypeDef",
     "SelectResultTypeDef",
+    "BatchDeleteAttributesRequestRequestTypeDef",
     "BatchPutAttributesRequestRequestTypeDef",
 )
 
+_RequiredAttributeOutputTypeDef = TypedDict(
+    "_RequiredAttributeOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
+_OptionalAttributeOutputTypeDef = TypedDict(
+    "_OptionalAttributeOutputTypeDef",
+    {
+        "AlternateNameEncoding": str,
+        "AlternateValueEncoding": str,
+    },
+    total=False,
+)
+
+
+class AttributeOutputTypeDef(_RequiredAttributeOutputTypeDef, _OptionalAttributeOutputTypeDef):
+    pass
+
+
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -59,17 +82,19 @@
     {
         "AlternateNameEncoding": str,
         "AlternateValueEncoding": str,
     },
     total=False,
 )
 
+
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
+
 CreateDomainRequestRequestTypeDef = TypedDict(
     "CreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
@@ -93,32 +118,22 @@
 DomainMetadataRequestRequestTypeDef = TypedDict(
     "DomainMetadataRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-DomainMetadataResultTypeDef = TypedDict(
-    "DomainMetadataResultTypeDef",
-    {
-        "ItemCount": int,
-        "ItemNamesSizeBytes": int,
-        "AttributeNameCount": int,
-        "AttributeNamesSizeBytes": int,
-        "AttributeValueCount": int,
-        "AttributeValuesSizeBytes": int,
-        "Timestamp": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredGetAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAttributesRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -130,55 +145,40 @@
     {
         "AttributeNames": Sequence[str],
         "ConsistentRead": bool,
     },
     total=False,
 )
 
+
 class GetAttributesRequestRequestTypeDef(
     _RequiredGetAttributesRequestRequestTypeDef, _OptionalGetAttributesRequestRequestTypeDef
 ):
     pass
 
-ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
-    "ListDomainsRequestListDomainsPaginateTypeDef",
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
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "MaxNumberOfDomains": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListDomainsResultTypeDef = TypedDict(
-    "ListDomainsResultTypeDef",
-    {
-        "DomainNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 _RequiredReplaceableAttributeTypeDef = TypedDict(
     "_RequiredReplaceableAttributeTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -186,29 +186,20 @@
     "_OptionalReplaceableAttributeTypeDef",
     {
         "Replace": bool,
     },
     total=False,
 )
 
+
 class ReplaceableAttributeTypeDef(
     _RequiredReplaceableAttributeTypeDef, _OptionalReplaceableAttributeTypeDef
 ):
     pass
 
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
 
 _RequiredSelectRequestRequestTypeDef = TypedDict(
     "_RequiredSelectRequestRequestTypeDef",
     {
         "SelectExpression": str,
     },
 )
@@ -217,103 +208,151 @@
     {
         "NextToken": str,
         "ConsistentRead": bool,
     },
     total=False,
 )
 
+
 class SelectRequestRequestTypeDef(
     _RequiredSelectRequestRequestTypeDef, _OptionalSelectRequestRequestTypeDef
 ):
     pass
 
-_RequiredSelectRequestSelectPaginateTypeDef = TypedDict(
-    "_RequiredSelectRequestSelectPaginateTypeDef",
+
+_RequiredItemTypeDef = TypedDict(
+    "_RequiredItemTypeDef",
     {
-        "SelectExpression": str,
+        "Name": str,
+        "Attributes": List[AttributeOutputTypeDef],
     },
 )
-_OptionalSelectRequestSelectPaginateTypeDef = TypedDict(
-    "_OptionalSelectRequestSelectPaginateTypeDef",
+_OptionalItemTypeDef = TypedDict(
+    "_OptionalItemTypeDef",
     {
-        "ConsistentRead": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "AlternateNameEncoding": str,
     },
     total=False,
 )
 
-class SelectRequestSelectPaginateTypeDef(
-    _RequiredSelectRequestSelectPaginateTypeDef, _OptionalSelectRequestSelectPaginateTypeDef
-):
+
+class ItemTypeDef(_RequiredItemTypeDef, _OptionalItemTypeDef):
     pass
 
+
 _RequiredDeletableItemTypeDef = TypedDict(
     "_RequiredDeletableItemTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDeletableItemTypeDef = TypedDict(
     "_OptionalDeletableItemTypeDef",
     {
         "Attributes": Sequence[AttributeTypeDef],
     },
     total=False,
 )
 
+
 class DeletableItemTypeDef(_RequiredDeletableItemTypeDef, _OptionalDeletableItemTypeDef):
     pass
 
+
+_RequiredDeleteAttributesRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteAttributesRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "ItemName": str,
+    },
+)
+_OptionalDeleteAttributesRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteAttributesRequestRequestTypeDef",
+    {
+        "Attributes": Sequence[AttributeTypeDef],
+        "Expected": UpdateConditionTypeDef,
+    },
+    total=False,
+)
+
+
+class DeleteAttributesRequestRequestTypeDef(
+    _RequiredDeleteAttributesRequestRequestTypeDef, _OptionalDeleteAttributesRequestRequestTypeDef
+):
+    pass
+
+
+DomainMetadataResultTypeDef = TypedDict(
+    "DomainMetadataResultTypeDef",
+    {
+        "ItemCount": int,
+        "ItemNamesSizeBytes": int,
+        "AttributeNameCount": int,
+        "AttributeNamesSizeBytes": int,
+        "AttributeValueCount": int,
+        "AttributeValuesSizeBytes": int,
+        "Timestamp": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetAttributesResultTypeDef = TypedDict(
     "GetAttributesResultTypeDef",
     {
-        "Attributes": List[AttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Attributes": List[AttributeOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredItemTypeDef = TypedDict(
-    "_RequiredItemTypeDef",
+ListDomainsResultTypeDef = TypedDict(
+    "ListDomainsResultTypeDef",
     {
-        "Name": str,
-        "Attributes": List[AttributeTypeDef],
+        "DomainNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalItemTypeDef = TypedDict(
-    "_OptionalItemTypeDef",
+
+ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
+    "ListDomainsRequestListDomainsPaginateTypeDef",
     {
-        "AlternateNameEncoding": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ItemTypeDef(_RequiredItemTypeDef, _OptionalItemTypeDef):
-    pass
-
-_RequiredDeleteAttributesRequestRequestTypeDef = TypedDict(
-    "_RequiredDeleteAttributesRequestRequestTypeDef",
+_RequiredSelectRequestSelectPaginateTypeDef = TypedDict(
+    "_RequiredSelectRequestSelectPaginateTypeDef",
     {
-        "DomainName": str,
-        "ItemName": str,
+        "SelectExpression": str,
     },
 )
-_OptionalDeleteAttributesRequestRequestTypeDef = TypedDict(
-    "_OptionalDeleteAttributesRequestRequestTypeDef",
+_OptionalSelectRequestSelectPaginateTypeDef = TypedDict(
+    "_OptionalSelectRequestSelectPaginateTypeDef",
     {
-        "Attributes": Sequence[AttributeTypeDef],
-        "Expected": UpdateConditionTypeDef,
+        "ConsistentRead": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class DeleteAttributesRequestRequestTypeDef(
-    _RequiredDeleteAttributesRequestRequestTypeDef, _OptionalDeleteAttributesRequestRequestTypeDef
+
+class SelectRequestSelectPaginateTypeDef(
+    _RequiredSelectRequestSelectPaginateTypeDef, _OptionalSelectRequestSelectPaginateTypeDef
 ):
     pass
 
+
 _RequiredPutAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutAttributesRequestRequestTypeDef",
     {
         "DomainName": str,
         "ItemName": str,
         "Attributes": Sequence[ReplaceableAttributeTypeDef],
     },
@@ -322,41 +361,43 @@
     "_OptionalPutAttributesRequestRequestTypeDef",
     {
         "Expected": UpdateConditionTypeDef,
     },
     total=False,
 )
 
+
 class PutAttributesRequestRequestTypeDef(
     _RequiredPutAttributesRequestRequestTypeDef, _OptionalPutAttributesRequestRequestTypeDef
 ):
     pass
 
+
 ReplaceableItemTypeDef = TypedDict(
     "ReplaceableItemTypeDef",
     {
         "Name": str,
         "Attributes": Sequence[ReplaceableAttributeTypeDef],
     },
 )
 
-BatchDeleteAttributesRequestRequestTypeDef = TypedDict(
-    "BatchDeleteAttributesRequestRequestTypeDef",
-    {
-        "DomainName": str,
-        "Items": Sequence[DeletableItemTypeDef],
-    },
-)
-
 SelectResultTypeDef = TypedDict(
     "SelectResultTypeDef",
     {
         "Items": List[ItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchDeleteAttributesRequestRequestTypeDef = TypedDict(
+    "BatchDeleteAttributesRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "Items": Sequence[DeletableItemTypeDef],
     },
 )
 
 BatchPutAttributesRequestRequestTypeDef = TypedDict(
     "BatchPutAttributesRequestRequestTypeDef",
     {
         "DomainName": str,
```

### Comparing `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb.egg-info/PKG-INFO` & `mypy-boto3-sdb-1.28.12/mypy_boto3_sdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sdb
-Version: 1.28.0
-Summary: Type annotations for boto3.SimpleDB 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SimpleDB 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sdb"></a>
 
 # mypy-boto3-sdb
 
 [![PyPI - mypy-boto3-sdb](https://img.shields.io/pypi/v/mypy-boto3-sdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-sdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-sdb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sdb?color=blue)](https://pypistats.org/packages/mypy-boto3-sdb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sdb)](https://pepy.tech/project/mypy-boto3-sdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SimpleDB 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
+[boto3.SimpleDB 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
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
 [mypy-boto3-sdb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -319,43 +319,44 @@
 ### Typed dictionaries
 
 `mypy_boto3_sdb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sdb.type_defs import (
+    AttributeOutputTypeDef,
     AttributeTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateConditionTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainMetadataRequestRequestTypeDef,
-    DomainMetadataResultTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetAttributesRequestRequestTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
-    ListDomainsRequestRequestTypeDef,
-    ListDomainsResultTypeDef,
     PaginatorConfigTypeDef,
+    ListDomainsRequestRequestTypeDef,
     ReplaceableAttributeTypeDef,
-    ResponseMetadataTypeDef,
     SelectRequestRequestTypeDef,
-    SelectRequestSelectPaginateTypeDef,
-    DeletableItemTypeDef,
-    GetAttributesResultTypeDef,
     ItemTypeDef,
+    DeletableItemTypeDef,
     DeleteAttributesRequestRequestTypeDef,
+    DomainMetadataResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAttributesResultTypeDef,
+    ListDomainsResultTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
+    SelectRequestSelectPaginateTypeDef,
     PutAttributesRequestRequestTypeDef,
     ReplaceableItemTypeDef,
-    BatchDeleteAttributesRequestRequestTypeDef,
     SelectResultTypeDef,
+    BatchDeleteAttributesRequestRequestTypeDef,
     BatchPutAttributesRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AttributeTypeDef:
+def get_structure() -> AttributeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb.egg-info/SOURCES.txt` & `mypy-boto3-sdb-1.28.12/mypy_boto3_sdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.28.0/setup.py` & `mypy-boto3-sdb-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sdb",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_sdb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SimpleDB 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.SimpleDB 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

