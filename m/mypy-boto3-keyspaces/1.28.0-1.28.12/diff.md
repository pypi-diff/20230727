# Comparing `tmp/mypy-boto3-keyspaces-1.28.0.tar.gz` & `tmp/mypy-boto3-keyspaces-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-keyspaces-1.28.0.tar", last modified: Thu Jul  6 20:59:54 2023, max compression
+gzip compressed data, was "mypy-boto3-keyspaces-1.28.12.tar", last modified: Thu Jul 27 05:34:53 2023, max compression
```

## Comparing `mypy-boto3-keyspaces-1.28.0.tar` & `mypy-boto3-keyspaces-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:54.170343 mypy-boto3-keyspaces-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:44:40.000000 mypy-boto3-keyspaces-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14654 2023-07-06 20:59:54.170343 mypy-boto3-keyspaces-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13161 2023-07-06 20:44:40.000000 mypy-boto3-keyspaces-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:54.170343 mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-06 20:44:40.000000 mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-06 20:44:40.000000 mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 20:44:40.000000 mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13482 2023-07-06 20:44:41.000000 mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13459 2023-07-06 20:44:40.000000 mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-07-06 20:44:41.000000 mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-07-06 20:44:41.000000 mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-06 20:44:41.000000 mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-06 20:44:41.000000 mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:44:40.000000 mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-07-06 20:44:41.000000 mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16586 2023-07-06 20:44:41.000000 mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:44:40.000000 mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:54.170343 mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14654 2023-07-06 20:59:53.000000 mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-06 20:59:53.000000 mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:53.000000 mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:53.000000 mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:53.000000 mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 20:59:53.000000 mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:54.170343 mypy-boto3-keyspaces-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 20:44:40.000000 mypy-boto3-keyspaces-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.204469 mypy-boto3-keyspaces-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14963 2023-07-27 05:34:53.204469 mypy-boto3-keyspaces-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13468 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.200469 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13482 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13459 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19084 2023-07-27 05:24:38.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19050 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.204469 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14963 2023-07-27 05:34:53.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 05:34:53.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:53.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:53.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:53.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:53.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:53.204469 mypy-boto3-keyspaces-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/setup.py
```

### Comparing `mypy-boto3-keyspaces-1.28.0/LICENSE` & `mypy-boto3-keyspaces-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.0/PKG-INFO` & `mypy-boto3-keyspaces-1.28.12/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-keyspaces
-Version: 1.28.0
-Summary: Type annotations for boto3.Keyspaces 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Keyspaces 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-keyspaces"></a>
 
 # mypy-boto3-keyspaces
 
 [![PyPI - mypy-boto3-keyspaces](https://img.shields.io/pypi/v/mypy-boto3-keyspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-keyspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-keyspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-keyspaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-keyspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-keyspaces)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-keyspaces)](https://pepy.tech/project/mypy-boto3-keyspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Keyspaces 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
+[boto3.Keyspaces 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
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
 [mypy-boto3-keyspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,56 +338,66 @@
 `mypy_boto3_keyspaces.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_keyspaces.type_defs import (
     CapacitySpecificationSummaryTypeDef,
     CapacitySpecificationTypeDef,
+    ClientSideTimestampsOutputTypeDef,
     ClientSideTimestampsTypeDef,
+    ClusteringKeyOutputTypeDef,
     ClusteringKeyTypeDef,
+    ColumnDefinitionOutputTypeDef,
     ColumnDefinitionTypeDef,
+    CommentOutputTypeDef,
     CommentTypeDef,
     ReplicationSpecificationTypeDef,
     TagTypeDef,
     CreateKeyspaceResponseTypeDef,
     EncryptionSpecificationTypeDef,
     PointInTimeRecoveryTypeDef,
     TimeToLiveTypeDef,
     CreateTableResponseTypeDef,
     DeleteKeyspaceRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
+    EncryptionSpecificationOutputTypeDef,
     GetKeyspaceRequestRequestTypeDef,
     GetKeyspaceResponseTypeDef,
     GetTableRequestRequestTypeDef,
     PointInTimeRecoverySummaryTypeDef,
+    TimeToLiveOutputTypeDef,
     KeyspaceSummaryTypeDef,
     ListKeyspacesRequestListKeyspacesPaginateTypeDef,
     ListKeyspacesRequestRequestTypeDef,
     ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableSummaryTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
+    PartitionKeyOutputTypeDef,
     PartitionKeyTypeDef,
     ResponseMetadataTypeDef,
     RestoreTableResponseTypeDef,
+    StaticColumnOutputTypeDef,
     StaticColumnTypeDef,
     UpdateTableResponseTypeDef,
     CreateKeyspaceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     RestoreTableRequestRequestTypeDef,
     UpdateTableRequestRequestTypeDef,
     ListKeyspacesResponseTypeDef,
     ListTablesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
-    CreateTableRequestRequestTypeDef,
     GetTableResponseTypeDef,
+    CreateTableRequestRequestTypeDef,
 )
 
 
 def get_structure() -> CapacitySpecificationSummaryTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-keyspaces-1.28.0/README.md` & `mypy-boto3-keyspaces-1.28.12/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-keyspaces"></a>
 
 # mypy-boto3-keyspaces
 
 [![PyPI - mypy-boto3-keyspaces](https://img.shields.io/pypi/v/mypy-boto3-keyspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-keyspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-keyspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-keyspaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-keyspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-keyspaces)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-keyspaces)](https://pepy.tech/project/mypy-boto3-keyspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Keyspaces 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
+[boto3.Keyspaces 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
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
 [mypy-boto3-keyspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,56 +306,66 @@
 `mypy_boto3_keyspaces.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_keyspaces.type_defs import (
     CapacitySpecificationSummaryTypeDef,
     CapacitySpecificationTypeDef,
+    ClientSideTimestampsOutputTypeDef,
     ClientSideTimestampsTypeDef,
+    ClusteringKeyOutputTypeDef,
     ClusteringKeyTypeDef,
+    ColumnDefinitionOutputTypeDef,
     ColumnDefinitionTypeDef,
+    CommentOutputTypeDef,
     CommentTypeDef,
     ReplicationSpecificationTypeDef,
     TagTypeDef,
     CreateKeyspaceResponseTypeDef,
     EncryptionSpecificationTypeDef,
     PointInTimeRecoveryTypeDef,
     TimeToLiveTypeDef,
     CreateTableResponseTypeDef,
     DeleteKeyspaceRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
+    EncryptionSpecificationOutputTypeDef,
     GetKeyspaceRequestRequestTypeDef,
     GetKeyspaceResponseTypeDef,
     GetTableRequestRequestTypeDef,
     PointInTimeRecoverySummaryTypeDef,
+    TimeToLiveOutputTypeDef,
     KeyspaceSummaryTypeDef,
     ListKeyspacesRequestListKeyspacesPaginateTypeDef,
     ListKeyspacesRequestRequestTypeDef,
     ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableSummaryTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
+    PartitionKeyOutputTypeDef,
     PartitionKeyTypeDef,
     ResponseMetadataTypeDef,
     RestoreTableResponseTypeDef,
+    StaticColumnOutputTypeDef,
     StaticColumnTypeDef,
     UpdateTableResponseTypeDef,
     CreateKeyspaceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     RestoreTableRequestRequestTypeDef,
     UpdateTableRequestRequestTypeDef,
     ListKeyspacesResponseTypeDef,
     ListTablesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
-    CreateTableRequestRequestTypeDef,
     GetTableResponseTypeDef,
+    CreateTableRequestRequestTypeDef,
 )
 
 
 def get_structure() -> CapacitySpecificationSummaryTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/__init__.py` & `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/__init__.pyi` & `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/__main__.py` & `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Keyspaces 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Keyspaces 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces\nOther"
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

### Comparing `mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/client.py` & `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/client.pyi` & `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/literals.py` & `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,15 @@
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
@@ -260,26 +261,28 @@
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

### Comparing `mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/literals.pyi` & `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -172,14 +172,15 @@
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
@@ -258,26 +259,28 @@
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

### Comparing `mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/paginator.py` & `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/paginator.pyi` & `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/type_defs.py` & `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,56 +33,66 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CapacitySpecificationSummaryTypeDef",
     "CapacitySpecificationTypeDef",
+    "ClientSideTimestampsOutputTypeDef",
     "ClientSideTimestampsTypeDef",
+    "ClusteringKeyOutputTypeDef",
     "ClusteringKeyTypeDef",
+    "ColumnDefinitionOutputTypeDef",
     "ColumnDefinitionTypeDef",
+    "CommentOutputTypeDef",
     "CommentTypeDef",
     "ReplicationSpecificationTypeDef",
     "TagTypeDef",
     "CreateKeyspaceResponseTypeDef",
     "EncryptionSpecificationTypeDef",
     "PointInTimeRecoveryTypeDef",
     "TimeToLiveTypeDef",
     "CreateTableResponseTypeDef",
     "DeleteKeyspaceRequestRequestTypeDef",
     "DeleteTableRequestRequestTypeDef",
+    "EncryptionSpecificationOutputTypeDef",
     "GetKeyspaceRequestRequestTypeDef",
     "GetKeyspaceResponseTypeDef",
     "GetTableRequestRequestTypeDef",
     "PointInTimeRecoverySummaryTypeDef",
+    "TimeToLiveOutputTypeDef",
     "KeyspaceSummaryTypeDef",
     "ListKeyspacesRequestListKeyspacesPaginateTypeDef",
     "ListKeyspacesRequestRequestTypeDef",
     "ListTablesRequestListTablesPaginateTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableSummaryTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "PaginatorConfigTypeDef",
+    "PartitionKeyOutputTypeDef",
     "PartitionKeyTypeDef",
     "ResponseMetadataTypeDef",
     "RestoreTableResponseTypeDef",
+    "StaticColumnOutputTypeDef",
     "StaticColumnTypeDef",
     "UpdateTableResponseTypeDef",
     "CreateKeyspaceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "RestoreTableRequestRequestTypeDef",
     "UpdateTableRequestRequestTypeDef",
     "ListKeyspacesResponseTypeDef",
     "ListTablesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
-    "CreateTableRequestRequestTypeDef",
     "GetTableResponseTypeDef",
+    "CreateTableRequestRequestTypeDef",
 )
 
 _RequiredCapacitySpecificationSummaryTypeDef = TypedDict(
     "_RequiredCapacitySpecificationSummaryTypeDef",
     {
         "throughputMode": ThroughputModeType,
     },
@@ -122,37 +132,67 @@
 
 class CapacitySpecificationTypeDef(
     _RequiredCapacitySpecificationTypeDef, _OptionalCapacitySpecificationTypeDef
 ):
     pass
 
 
+ClientSideTimestampsOutputTypeDef = TypedDict(
+    "ClientSideTimestampsOutputTypeDef",
+    {
+        "status": Literal["ENABLED"],
+    },
+)
+
 ClientSideTimestampsTypeDef = TypedDict(
     "ClientSideTimestampsTypeDef",
     {
         "status": Literal["ENABLED"],
     },
 )
 
+ClusteringKeyOutputTypeDef = TypedDict(
+    "ClusteringKeyOutputTypeDef",
+    {
+        "name": str,
+        "orderBy": SortOrderType,
+    },
+)
+
 ClusteringKeyTypeDef = TypedDict(
     "ClusteringKeyTypeDef",
     {
         "name": str,
         "orderBy": SortOrderType,
     },
 )
 
+ColumnDefinitionOutputTypeDef = TypedDict(
+    "ColumnDefinitionOutputTypeDef",
+    {
+        "name": str,
+        "type": str,
+    },
+)
+
 ColumnDefinitionTypeDef = TypedDict(
     "ColumnDefinitionTypeDef",
     {
         "name": str,
         "type": str,
     },
 )
 
+CommentOutputTypeDef = TypedDict(
+    "CommentOutputTypeDef",
+    {
+        "message": str,
+    },
+)
+
 CommentTypeDef = TypedDict(
     "CommentTypeDef",
     {
         "message": str,
     },
 )
 
@@ -247,14 +287,35 @@
     "DeleteTableRequestRequestTypeDef",
     {
         "keyspaceName": str,
         "tableName": str,
     },
 )
 
+_RequiredEncryptionSpecificationOutputTypeDef = TypedDict(
+    "_RequiredEncryptionSpecificationOutputTypeDef",
+    {
+        "type": EncryptionTypeType,
+    },
+)
+_OptionalEncryptionSpecificationOutputTypeDef = TypedDict(
+    "_OptionalEncryptionSpecificationOutputTypeDef",
+    {
+        "kmsKeyIdentifier": str,
+    },
+    total=False,
+)
+
+
+class EncryptionSpecificationOutputTypeDef(
+    _RequiredEncryptionSpecificationOutputTypeDef, _OptionalEncryptionSpecificationOutputTypeDef
+):
+    pass
+
+
 GetKeyspaceRequestRequestTypeDef = TypedDict(
     "GetKeyspaceRequestRequestTypeDef",
     {
         "keyspaceName": str,
     },
 )
 
@@ -294,14 +355,21 @@
 
 class PointInTimeRecoverySummaryTypeDef(
     _RequiredPointInTimeRecoverySummaryTypeDef, _OptionalPointInTimeRecoverySummaryTypeDef
 ):
     pass
 
 
+TimeToLiveOutputTypeDef = TypedDict(
+    "TimeToLiveOutputTypeDef",
+    {
+        "status": Literal["ENABLED"],
+    },
+)
+
 _RequiredKeyspaceSummaryTypeDef = TypedDict(
     "_RequiredKeyspaceSummaryTypeDef",
     {
         "keyspaceName": str,
         "resourceArn": str,
         "replicationStrategy": rsType,
     },
@@ -430,24 +498,39 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
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
     total=False,
 )
 
+PartitionKeyOutputTypeDef = TypedDict(
+    "PartitionKeyOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+
 PartitionKeyTypeDef = TypedDict(
     "PartitionKeyTypeDef",
     {
         "name": str,
     },
 )
 
@@ -466,14 +549,21 @@
     "RestoreTableResponseTypeDef",
     {
         "restoredTableARN": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+StaticColumnOutputTypeDef = TypedDict(
+    "StaticColumnOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+
 StaticColumnTypeDef = TypedDict(
     "StaticColumnTypeDef",
     {
         "name": str,
     },
 )
 
@@ -503,23 +593,14 @@
 
 class CreateKeyspaceRequestRequestTypeDef(
     _RequiredCreateKeyspaceRequestRequestTypeDef, _OptionalCreateKeyspaceRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "nextToken": str,
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
@@ -602,14 +683,46 @@
     {
         "nextToken": str,
         "tables": List[TableSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "nextToken": str,
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredSchemaDefinitionOutputTypeDef = TypedDict(
+    "_RequiredSchemaDefinitionOutputTypeDef",
+    {
+        "allColumns": List[ColumnDefinitionOutputTypeDef],
+        "partitionKeys": List[PartitionKeyOutputTypeDef],
+    },
+)
+_OptionalSchemaDefinitionOutputTypeDef = TypedDict(
+    "_OptionalSchemaDefinitionOutputTypeDef",
+    {
+        "clusteringKeys": List[ClusteringKeyOutputTypeDef],
+        "staticColumns": List[StaticColumnOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class SchemaDefinitionOutputTypeDef(
+    _RequiredSchemaDefinitionOutputTypeDef, _OptionalSchemaDefinitionOutputTypeDef
+):
+    pass
+
+
 _RequiredSchemaDefinitionTypeDef = TypedDict(
     "_RequiredSchemaDefinitionTypeDef",
     {
         "allColumns": Sequence[ColumnDefinitionTypeDef],
         "partitionKeys": Sequence[PartitionKeyTypeDef],
     },
 )
@@ -623,14 +736,34 @@
 )
 
 
 class SchemaDefinitionTypeDef(_RequiredSchemaDefinitionTypeDef, _OptionalSchemaDefinitionTypeDef):
     pass
 
 
+GetTableResponseTypeDef = TypedDict(
+    "GetTableResponseTypeDef",
+    {
+        "keyspaceName": str,
+        "tableName": str,
+        "resourceArn": str,
+        "creationTimestamp": datetime,
+        "status": TableStatusType,
+        "schemaDefinition": SchemaDefinitionOutputTypeDef,
+        "capacitySpecification": CapacitySpecificationSummaryTypeDef,
+        "encryptionSpecification": EncryptionSpecificationOutputTypeDef,
+        "pointInTimeRecovery": PointInTimeRecoverySummaryTypeDef,
+        "ttl": TimeToLiveOutputTypeDef,
+        "defaultTimeToLive": int,
+        "comment": CommentOutputTypeDef,
+        "clientSideTimestamps": ClientSideTimestampsOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateTableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTableRequestRequestTypeDef",
     {
         "keyspaceName": str,
         "tableName": str,
         "schemaDefinition": SchemaDefinitionTypeDef,
     },
@@ -651,28 +784,7 @@
 )
 
 
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
 ):
     pass
-
-
-GetTableResponseTypeDef = TypedDict(
-    "GetTableResponseTypeDef",
-    {
-        "keyspaceName": str,
-        "tableName": str,
-        "resourceArn": str,
-        "creationTimestamp": datetime,
-        "status": TableStatusType,
-        "schemaDefinition": SchemaDefinitionTypeDef,
-        "capacitySpecification": CapacitySpecificationSummaryTypeDef,
-        "encryptionSpecification": EncryptionSpecificationTypeDef,
-        "pointInTimeRecovery": PointInTimeRecoverySummaryTypeDef,
-        "ttl": TimeToLiveTypeDef,
-        "defaultTimeToLive": int,
-        "comment": CommentTypeDef,
-        "clientSideTimestamps": ClientSideTimestampsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces/type_defs.pyi` & `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -32,56 +32,66 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CapacitySpecificationSummaryTypeDef",
     "CapacitySpecificationTypeDef",
+    "ClientSideTimestampsOutputTypeDef",
     "ClientSideTimestampsTypeDef",
+    "ClusteringKeyOutputTypeDef",
     "ClusteringKeyTypeDef",
+    "ColumnDefinitionOutputTypeDef",
     "ColumnDefinitionTypeDef",
+    "CommentOutputTypeDef",
     "CommentTypeDef",
     "ReplicationSpecificationTypeDef",
     "TagTypeDef",
     "CreateKeyspaceResponseTypeDef",
     "EncryptionSpecificationTypeDef",
     "PointInTimeRecoveryTypeDef",
     "TimeToLiveTypeDef",
     "CreateTableResponseTypeDef",
     "DeleteKeyspaceRequestRequestTypeDef",
     "DeleteTableRequestRequestTypeDef",
+    "EncryptionSpecificationOutputTypeDef",
     "GetKeyspaceRequestRequestTypeDef",
     "GetKeyspaceResponseTypeDef",
     "GetTableRequestRequestTypeDef",
     "PointInTimeRecoverySummaryTypeDef",
+    "TimeToLiveOutputTypeDef",
     "KeyspaceSummaryTypeDef",
     "ListKeyspacesRequestListKeyspacesPaginateTypeDef",
     "ListKeyspacesRequestRequestTypeDef",
     "ListTablesRequestListTablesPaginateTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableSummaryTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "PaginatorConfigTypeDef",
+    "PartitionKeyOutputTypeDef",
     "PartitionKeyTypeDef",
     "ResponseMetadataTypeDef",
     "RestoreTableResponseTypeDef",
+    "StaticColumnOutputTypeDef",
     "StaticColumnTypeDef",
     "UpdateTableResponseTypeDef",
     "CreateKeyspaceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "RestoreTableRequestRequestTypeDef",
     "UpdateTableRequestRequestTypeDef",
     "ListKeyspacesResponseTypeDef",
     "ListTablesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
-    "CreateTableRequestRequestTypeDef",
     "GetTableResponseTypeDef",
+    "CreateTableRequestRequestTypeDef",
 )
 
 _RequiredCapacitySpecificationSummaryTypeDef = TypedDict(
     "_RequiredCapacitySpecificationSummaryTypeDef",
     {
         "throughputMode": ThroughputModeType,
     },
@@ -117,37 +127,67 @@
 )
 
 class CapacitySpecificationTypeDef(
     _RequiredCapacitySpecificationTypeDef, _OptionalCapacitySpecificationTypeDef
 ):
     pass
 
+ClientSideTimestampsOutputTypeDef = TypedDict(
+    "ClientSideTimestampsOutputTypeDef",
+    {
+        "status": Literal["ENABLED"],
+    },
+)
+
 ClientSideTimestampsTypeDef = TypedDict(
     "ClientSideTimestampsTypeDef",
     {
         "status": Literal["ENABLED"],
     },
 )
 
+ClusteringKeyOutputTypeDef = TypedDict(
+    "ClusteringKeyOutputTypeDef",
+    {
+        "name": str,
+        "orderBy": SortOrderType,
+    },
+)
+
 ClusteringKeyTypeDef = TypedDict(
     "ClusteringKeyTypeDef",
     {
         "name": str,
         "orderBy": SortOrderType,
     },
 )
 
+ColumnDefinitionOutputTypeDef = TypedDict(
+    "ColumnDefinitionOutputTypeDef",
+    {
+        "name": str,
+        "type": str,
+    },
+)
+
 ColumnDefinitionTypeDef = TypedDict(
     "ColumnDefinitionTypeDef",
     {
         "name": str,
         "type": str,
     },
 )
 
+CommentOutputTypeDef = TypedDict(
+    "CommentOutputTypeDef",
+    {
+        "message": str,
+    },
+)
+
 CommentTypeDef = TypedDict(
     "CommentTypeDef",
     {
         "message": str,
     },
 )
 
@@ -238,14 +278,33 @@
     "DeleteTableRequestRequestTypeDef",
     {
         "keyspaceName": str,
         "tableName": str,
     },
 )
 
+_RequiredEncryptionSpecificationOutputTypeDef = TypedDict(
+    "_RequiredEncryptionSpecificationOutputTypeDef",
+    {
+        "type": EncryptionTypeType,
+    },
+)
+_OptionalEncryptionSpecificationOutputTypeDef = TypedDict(
+    "_OptionalEncryptionSpecificationOutputTypeDef",
+    {
+        "kmsKeyIdentifier": str,
+    },
+    total=False,
+)
+
+class EncryptionSpecificationOutputTypeDef(
+    _RequiredEncryptionSpecificationOutputTypeDef, _OptionalEncryptionSpecificationOutputTypeDef
+):
+    pass
+
 GetKeyspaceRequestRequestTypeDef = TypedDict(
     "GetKeyspaceRequestRequestTypeDef",
     {
         "keyspaceName": str,
     },
 )
 
@@ -283,14 +342,21 @@
 )
 
 class PointInTimeRecoverySummaryTypeDef(
     _RequiredPointInTimeRecoverySummaryTypeDef, _OptionalPointInTimeRecoverySummaryTypeDef
 ):
     pass
 
+TimeToLiveOutputTypeDef = TypedDict(
+    "TimeToLiveOutputTypeDef",
+    {
+        "status": Literal["ENABLED"],
+    },
+)
+
 _RequiredKeyspaceSummaryTypeDef = TypedDict(
     "_RequiredKeyspaceSummaryTypeDef",
     {
         "keyspaceName": str,
         "resourceArn": str,
         "replicationStrategy": rsType,
     },
@@ -409,24 +475,39 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
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
     total=False,
 )
 
+PartitionKeyOutputTypeDef = TypedDict(
+    "PartitionKeyOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+
 PartitionKeyTypeDef = TypedDict(
     "PartitionKeyTypeDef",
     {
         "name": str,
     },
 )
 
@@ -445,14 +526,21 @@
     "RestoreTableResponseTypeDef",
     {
         "restoredTableARN": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+StaticColumnOutputTypeDef = TypedDict(
+    "StaticColumnOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+
 StaticColumnTypeDef = TypedDict(
     "StaticColumnTypeDef",
     {
         "name": str,
     },
 )
 
@@ -480,23 +568,14 @@
 )
 
 class CreateKeyspaceRequestRequestTypeDef(
     _RequiredCreateKeyspaceRequestRequestTypeDef, _OptionalCreateKeyspaceRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "nextToken": str,
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
@@ -575,14 +654,44 @@
     {
         "nextToken": str,
         "tables": List[TableSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "nextToken": str,
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredSchemaDefinitionOutputTypeDef = TypedDict(
+    "_RequiredSchemaDefinitionOutputTypeDef",
+    {
+        "allColumns": List[ColumnDefinitionOutputTypeDef],
+        "partitionKeys": List[PartitionKeyOutputTypeDef],
+    },
+)
+_OptionalSchemaDefinitionOutputTypeDef = TypedDict(
+    "_OptionalSchemaDefinitionOutputTypeDef",
+    {
+        "clusteringKeys": List[ClusteringKeyOutputTypeDef],
+        "staticColumns": List[StaticColumnOutputTypeDef],
+    },
+    total=False,
+)
+
+class SchemaDefinitionOutputTypeDef(
+    _RequiredSchemaDefinitionOutputTypeDef, _OptionalSchemaDefinitionOutputTypeDef
+):
+    pass
+
 _RequiredSchemaDefinitionTypeDef = TypedDict(
     "_RequiredSchemaDefinitionTypeDef",
     {
         "allColumns": Sequence[ColumnDefinitionTypeDef],
         "partitionKeys": Sequence[PartitionKeyTypeDef],
     },
 )
@@ -594,14 +703,34 @@
     },
     total=False,
 )
 
 class SchemaDefinitionTypeDef(_RequiredSchemaDefinitionTypeDef, _OptionalSchemaDefinitionTypeDef):
     pass
 
+GetTableResponseTypeDef = TypedDict(
+    "GetTableResponseTypeDef",
+    {
+        "keyspaceName": str,
+        "tableName": str,
+        "resourceArn": str,
+        "creationTimestamp": datetime,
+        "status": TableStatusType,
+        "schemaDefinition": SchemaDefinitionOutputTypeDef,
+        "capacitySpecification": CapacitySpecificationSummaryTypeDef,
+        "encryptionSpecification": EncryptionSpecificationOutputTypeDef,
+        "pointInTimeRecovery": PointInTimeRecoverySummaryTypeDef,
+        "ttl": TimeToLiveOutputTypeDef,
+        "defaultTimeToLive": int,
+        "comment": CommentOutputTypeDef,
+        "clientSideTimestamps": ClientSideTimestampsOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateTableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTableRequestRequestTypeDef",
     {
         "keyspaceName": str,
         "tableName": str,
         "schemaDefinition": SchemaDefinitionTypeDef,
     },
@@ -621,27 +750,7 @@
     total=False,
 )
 
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
 ):
     pass
-
-GetTableResponseTypeDef = TypedDict(
-    "GetTableResponseTypeDef",
-    {
-        "keyspaceName": str,
-        "tableName": str,
-        "resourceArn": str,
-        "creationTimestamp": datetime,
-        "status": TableStatusType,
-        "schemaDefinition": SchemaDefinitionTypeDef,
-        "capacitySpecification": CapacitySpecificationSummaryTypeDef,
-        "encryptionSpecification": EncryptionSpecificationTypeDef,
-        "pointInTimeRecovery": PointInTimeRecoverySummaryTypeDef,
-        "ttl": TimeToLiveTypeDef,
-        "defaultTimeToLive": int,
-        "comment": CommentTypeDef,
-        "clientSideTimestamps": ClientSideTimestampsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces.egg-info/PKG-INFO` & `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-keyspaces
-Version: 1.28.0
-Summary: Type annotations for boto3.Keyspaces 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Keyspaces 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-keyspaces"></a>
 
 # mypy-boto3-keyspaces
 
 [![PyPI - mypy-boto3-keyspaces](https://img.shields.io/pypi/v/mypy-boto3-keyspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-keyspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-keyspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-keyspaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-keyspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-keyspaces)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-keyspaces)](https://pepy.tech/project/mypy-boto3-keyspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Keyspaces 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
+[boto3.Keyspaces 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
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
 [mypy-boto3-keyspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,56 +338,66 @@
 `mypy_boto3_keyspaces.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_keyspaces.type_defs import (
     CapacitySpecificationSummaryTypeDef,
     CapacitySpecificationTypeDef,
+    ClientSideTimestampsOutputTypeDef,
     ClientSideTimestampsTypeDef,
+    ClusteringKeyOutputTypeDef,
     ClusteringKeyTypeDef,
+    ColumnDefinitionOutputTypeDef,
     ColumnDefinitionTypeDef,
+    CommentOutputTypeDef,
     CommentTypeDef,
     ReplicationSpecificationTypeDef,
     TagTypeDef,
     CreateKeyspaceResponseTypeDef,
     EncryptionSpecificationTypeDef,
     PointInTimeRecoveryTypeDef,
     TimeToLiveTypeDef,
     CreateTableResponseTypeDef,
     DeleteKeyspaceRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
+    EncryptionSpecificationOutputTypeDef,
     GetKeyspaceRequestRequestTypeDef,
     GetKeyspaceResponseTypeDef,
     GetTableRequestRequestTypeDef,
     PointInTimeRecoverySummaryTypeDef,
+    TimeToLiveOutputTypeDef,
     KeyspaceSummaryTypeDef,
     ListKeyspacesRequestListKeyspacesPaginateTypeDef,
     ListKeyspacesRequestRequestTypeDef,
     ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableSummaryTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
+    PartitionKeyOutputTypeDef,
     PartitionKeyTypeDef,
     ResponseMetadataTypeDef,
     RestoreTableResponseTypeDef,
+    StaticColumnOutputTypeDef,
     StaticColumnTypeDef,
     UpdateTableResponseTypeDef,
     CreateKeyspaceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     RestoreTableRequestRequestTypeDef,
     UpdateTableRequestRequestTypeDef,
     ListKeyspacesResponseTypeDef,
     ListTablesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
-    CreateTableRequestRequestTypeDef,
     GetTableResponseTypeDef,
+    CreateTableRequestRequestTypeDef,
 )
 
 
 def get_structure() -> CapacitySpecificationSummaryTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-keyspaces-1.28.0/mypy_boto3_keyspaces.egg-info/SOURCES.txt` & `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.0/setup.py` & `mypy-boto3-keyspaces-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-keyspaces",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_keyspaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Keyspaces 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Keyspaces 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

