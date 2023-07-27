# Comparing `tmp/mypy-boto3-resource-explorer-2-1.28.0.tar.gz` & `tmp/mypy-boto3-resource-explorer-2-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-resource-explorer-2-1.28.0.tar", last modified: Thu Jul  6 21:00:26 2023, max compression
+gzip compressed data, was "mypy-boto3-resource-explorer-2-1.28.12.tar", last modified: Thu Jul 27 11:49:30 2023, max compression
```

## Comparing `mypy-boto3-resource-explorer-2-1.28.0.tar` & `mypy-boto3-resource-explorer-2-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:26.346408 mypy-boto3-resource-explorer-2-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:53:14.000000 mypy-boto3-resource-explorer-2-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-06 21:00:26.342408 mypy-boto3-resource-explorer-2-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-07-06 20:53:14.000000 mypy-boto3-resource-explorer-2-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:26.330408 mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-06 20:53:14.000000 mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-06 20:53:14.000000 mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-06 20:53:14.000000 mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17102 2023-07-06 20:53:14.000000 mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-07-06 20:53:14.000000 mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-06 20:53:14.000000 mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-07-06 20:53:14.000000 mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-06 20:53:14.000000 mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-06 20:53:14.000000 mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:53:14.000000 mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-07-06 20:53:15.000000 mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-07-06 20:53:14.000000 mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:53:14.000000 mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:26.342408 mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-06 21:00:26.000000 mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 21:00:26.000000 mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:26.000000 mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:26.000000 mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:26.000000 mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 21:00:26.000000 mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:26.346408 mypy-boto3-resource-explorer-2-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-06 20:53:14.000000 mypy-boto3-resource-explorer-2-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.317213 mypy-boto3-resource-explorer-2-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-07-27 11:49:30.317213 mypy-boto3-resource-explorer-2-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.313213 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17102 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-07-27 11:44:39.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13357 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.317213 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-07-27 11:49:30.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-27 11:49:30.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:30.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 11:49:30.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:30.317213 mypy-boto3-resource-explorer-2-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/setup.py
```

### Comparing `mypy-boto3-resource-explorer-2-1.28.0/LICENSE` & `mypy-boto3-resource-explorer-2-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-explorer-2-1.28.0/PKG-INFO` & `mypy-boto3-resource-explorer-2-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resource-explorer-2
-Version: 1.28.0
-Summary: Type annotations for boto3.ResourceExplorer 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ResourceExplorer 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-resource-explorer-2"></a>
 
 # mypy-boto3-resource-explorer-2
 
 [![PyPI - mypy-boto3-resource-explorer-2](https://img.shields.io/pypi/v/mypy-boto3-resource-explorer-2.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-explorer-2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-explorer-2.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-explorer-2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resource-explorer-2?color=blue)](https://pypistats.org/packages/mypy-boto3-resource-explorer-2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resource-explorer-2)](https://pepy.tech/project/mypy-boto3-resource-explorer-2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceExplorer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
+[boto3.ResourceExplorer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
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
 [mypy-boto3-resource-explorer-2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,61 +336,63 @@
 
 `mypy_boto3_resource_explorer_2.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resource_explorer_2.type_defs import (
     AssociateDefaultViewInputRequestTypeDef,
-    AssociateDefaultViewOutputTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetViewErrorTypeDef,
     BatchGetViewInputRequestTypeDef,
     CreateIndexInputRequestTypeDef,
-    CreateIndexOutputTypeDef,
     IncludedPropertyTypeDef,
     SearchFilterTypeDef,
     DeleteIndexInputRequestTypeDef,
-    DeleteIndexOutputTypeDef,
     DeleteViewInputRequestTypeDef,
-    DeleteViewOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDefaultViewOutputTypeDef,
-    GetIndexOutputTypeDef,
     GetViewInputRequestTypeDef,
+    IncludedPropertyOutputTypeDef,
     IndexTypeDef,
-    ListIndexesInputListIndexesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListIndexesInputRequestTypeDef,
-    ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
     ListSupportedResourceTypesInputRequestTypeDef,
     SupportedResourceTypeTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListViewsInputListViewsPaginateTypeDef,
     ListViewsInputRequestTypeDef,
-    ListViewsOutputTypeDef,
-    PaginatorConfigTypeDef,
     ResourceCountTypeDef,
     ResourcePropertyTypeDef,
-    ResponseMetadataTypeDef,
+    SearchFilterOutputTypeDef,
     SearchInputRequestTypeDef,
-    SearchInputSearchPaginateTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateIndexTypeInputRequestTypeDef,
+    AssociateDefaultViewOutputTypeDef,
+    CreateIndexOutputTypeDef,
+    DeleteIndexOutputTypeDef,
+    DeleteViewOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDefaultViewOutputTypeDef,
+    GetIndexOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    ListViewsOutputTypeDef,
     UpdateIndexTypeOutputTypeDef,
     CreateViewInputRequestTypeDef,
     UpdateViewInputRequestTypeDef,
-    ViewTypeDef,
     ListIndexesOutputTypeDef,
+    ListIndexesInputListIndexesPaginateTypeDef,
+    ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
+    ListViewsInputListViewsPaginateTypeDef,
+    SearchInputSearchPaginateTypeDef,
     ListSupportedResourceTypesOutputTypeDef,
     ResourceTypeDef,
+    ViewTypeDef,
+    SearchOutputTypeDef,
     BatchGetViewOutputTypeDef,
     CreateViewOutputTypeDef,
     GetViewOutputTypeDef,
     UpdateViewOutputTypeDef,
-    SearchOutputTypeDef,
 )
 
 
 def get_structure() -> AssociateDefaultViewInputRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-resource-explorer-2-1.28.0/README.md` & `mypy-boto3-resource-explorer-2-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-resource-explorer-2"></a>
 
 # mypy-boto3-resource-explorer-2
 
 [![PyPI - mypy-boto3-resource-explorer-2](https://img.shields.io/pypi/v/mypy-boto3-resource-explorer-2.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-explorer-2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-explorer-2.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-explorer-2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resource-explorer-2?color=blue)](https://pypistats.org/packages/mypy-boto3-resource-explorer-2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resource-explorer-2)](https://pepy.tech/project/mypy-boto3-resource-explorer-2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceExplorer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
+[boto3.ResourceExplorer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
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
 [mypy-boto3-resource-explorer-2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,61 +304,63 @@
 
 `mypy_boto3_resource_explorer_2.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resource_explorer_2.type_defs import (
     AssociateDefaultViewInputRequestTypeDef,
-    AssociateDefaultViewOutputTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetViewErrorTypeDef,
     BatchGetViewInputRequestTypeDef,
     CreateIndexInputRequestTypeDef,
-    CreateIndexOutputTypeDef,
     IncludedPropertyTypeDef,
     SearchFilterTypeDef,
     DeleteIndexInputRequestTypeDef,
-    DeleteIndexOutputTypeDef,
     DeleteViewInputRequestTypeDef,
-    DeleteViewOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDefaultViewOutputTypeDef,
-    GetIndexOutputTypeDef,
     GetViewInputRequestTypeDef,
+    IncludedPropertyOutputTypeDef,
     IndexTypeDef,
-    ListIndexesInputListIndexesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListIndexesInputRequestTypeDef,
-    ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
     ListSupportedResourceTypesInputRequestTypeDef,
     SupportedResourceTypeTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListViewsInputListViewsPaginateTypeDef,
     ListViewsInputRequestTypeDef,
-    ListViewsOutputTypeDef,
-    PaginatorConfigTypeDef,
     ResourceCountTypeDef,
     ResourcePropertyTypeDef,
-    ResponseMetadataTypeDef,
+    SearchFilterOutputTypeDef,
     SearchInputRequestTypeDef,
-    SearchInputSearchPaginateTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateIndexTypeInputRequestTypeDef,
+    AssociateDefaultViewOutputTypeDef,
+    CreateIndexOutputTypeDef,
+    DeleteIndexOutputTypeDef,
+    DeleteViewOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDefaultViewOutputTypeDef,
+    GetIndexOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    ListViewsOutputTypeDef,
     UpdateIndexTypeOutputTypeDef,
     CreateViewInputRequestTypeDef,
     UpdateViewInputRequestTypeDef,
-    ViewTypeDef,
     ListIndexesOutputTypeDef,
+    ListIndexesInputListIndexesPaginateTypeDef,
+    ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
+    ListViewsInputListViewsPaginateTypeDef,
+    SearchInputSearchPaginateTypeDef,
     ListSupportedResourceTypesOutputTypeDef,
     ResourceTypeDef,
+    ViewTypeDef,
+    SearchOutputTypeDef,
     BatchGetViewOutputTypeDef,
     CreateViewOutputTypeDef,
     GetViewOutputTypeDef,
     UpdateViewOutputTypeDef,
-    SearchOutputTypeDef,
 )
 
 
 def get_structure() -> AssociateDefaultViewInputRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/__init__.py` & `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/__init__.pyi` & `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/__main__.py` & `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ResourceExplorer 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ResourceExplorer 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer\nOther"
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

### Comparing `mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/client.py` & `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/client.pyi` & `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/literals.py` & `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/literals.py`

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

### Comparing `mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/literals.pyi` & `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/literals.pyi`

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

### Comparing `mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/paginator.py` & `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,45 +63,45 @@
     """
 
     def paginate(
         self,
         *,
         Regions: Sequence[str] = ...,
         Type: IndexTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIndexesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListIndexes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listindexespaginator)
         """
 
 
 class ListSupportedResourceTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListSupportedResourceTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listsupportedresourcetypespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSupportedResourceTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListSupportedResourceTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listsupportedresourcetypespaginator)
         """
 
 
 class ListViewsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListViews)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listviewspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListViewsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListViews.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listviewspaginator)
         """
 
 
@@ -112,13 +112,13 @@
     """
 
     def paginate(
         self,
         *,
         QueryString: str,
         ViewArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.Search.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#searchpaginator)
         """
```

### Comparing `mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/paginator.pyi` & `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -60,43 +60,43 @@
     """
 
     def paginate(
         self,
         *,
         Regions: Sequence[str] = ...,
         Type: IndexTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIndexesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListIndexes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listindexespaginator)
         """
 
 class ListSupportedResourceTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListSupportedResourceTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listsupportedresourcetypespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSupportedResourceTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListSupportedResourceTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listsupportedresourcetypespaginator)
         """
 
 class ListViewsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListViews)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listviewspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListViewsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListViews.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#listviewspaginator)
         """
 
 class SearchPaginator(Paginator):
@@ -106,13 +106,13 @@
     """
 
     def paginate(
         self,
         *,
         QueryString: str,
         ViewArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.Search.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/paginators/#searchpaginator)
         """
```

### Comparing `mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/type_defs.py` & `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,75 +21,80 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateDefaultViewInputRequestTypeDef",
-    "AssociateDefaultViewOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetViewErrorTypeDef",
     "BatchGetViewInputRequestTypeDef",
     "CreateIndexInputRequestTypeDef",
-    "CreateIndexOutputTypeDef",
     "IncludedPropertyTypeDef",
     "SearchFilterTypeDef",
     "DeleteIndexInputRequestTypeDef",
-    "DeleteIndexOutputTypeDef",
     "DeleteViewInputRequestTypeDef",
-    "DeleteViewOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetDefaultViewOutputTypeDef",
-    "GetIndexOutputTypeDef",
     "GetViewInputRequestTypeDef",
+    "IncludedPropertyOutputTypeDef",
     "IndexTypeDef",
-    "ListIndexesInputListIndexesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListIndexesInputRequestTypeDef",
-    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
     "ListSupportedResourceTypesInputRequestTypeDef",
     "SupportedResourceTypeTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "ListViewsInputListViewsPaginateTypeDef",
     "ListViewsInputRequestTypeDef",
-    "ListViewsOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "ResourceCountTypeDef",
     "ResourcePropertyTypeDef",
-    "ResponseMetadataTypeDef",
+    "SearchFilterOutputTypeDef",
     "SearchInputRequestTypeDef",
-    "SearchInputSearchPaginateTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateIndexTypeInputRequestTypeDef",
+    "AssociateDefaultViewOutputTypeDef",
+    "CreateIndexOutputTypeDef",
+    "DeleteIndexOutputTypeDef",
+    "DeleteViewOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetDefaultViewOutputTypeDef",
+    "GetIndexOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "ListViewsOutputTypeDef",
     "UpdateIndexTypeOutputTypeDef",
     "CreateViewInputRequestTypeDef",
     "UpdateViewInputRequestTypeDef",
-    "ViewTypeDef",
     "ListIndexesOutputTypeDef",
+    "ListIndexesInputListIndexesPaginateTypeDef",
+    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
+    "ListViewsInputListViewsPaginateTypeDef",
+    "SearchInputSearchPaginateTypeDef",
     "ListSupportedResourceTypesOutputTypeDef",
     "ResourceTypeDef",
+    "ViewTypeDef",
+    "SearchOutputTypeDef",
     "BatchGetViewOutputTypeDef",
     "CreateViewOutputTypeDef",
     "GetViewOutputTypeDef",
     "UpdateViewOutputTypeDef",
-    "SearchOutputTypeDef",
 )
 
 AssociateDefaultViewInputRequestTypeDef = TypedDict(
     "AssociateDefaultViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
 )
 
-AssociateDefaultViewOutputTypeDef = TypedDict(
-    "AssociateDefaultViewOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ViewArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 BatchGetViewErrorTypeDef = TypedDict(
     "BatchGetViewErrorTypeDef",
     {
         "ErrorMessage": str,
@@ -110,24 +115,14 @@
     {
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-CreateIndexOutputTypeDef = TypedDict(
-    "CreateIndexOutputTypeDef",
-    {
-        "Arn": str,
-        "CreatedAt": datetime,
-        "State": IndexStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IncludedPropertyTypeDef = TypedDict(
     "IncludedPropertyTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -141,92 +136,51 @@
 DeleteIndexInputRequestTypeDef = TypedDict(
     "DeleteIndexInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DeleteIndexOutputTypeDef = TypedDict(
-    "DeleteIndexOutputTypeDef",
-    {
-        "Arn": str,
-        "LastUpdatedAt": datetime,
-        "State": IndexStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteViewInputRequestTypeDef = TypedDict(
     "DeleteViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
 )
 
-DeleteViewOutputTypeDef = TypedDict(
-    "DeleteViewOutputTypeDef",
-    {
-        "ViewArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDefaultViewOutputTypeDef = TypedDict(
-    "GetDefaultViewOutputTypeDef",
+GetViewInputRequestTypeDef = TypedDict(
+    "GetViewInputRequestTypeDef",
     {
         "ViewArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetIndexOutputTypeDef = TypedDict(
-    "GetIndexOutputTypeDef",
+IncludedPropertyOutputTypeDef = TypedDict(
+    "IncludedPropertyOutputTypeDef",
     {
-        "Arn": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "ReplicatingFrom": List[str],
-        "ReplicatingTo": List[str],
-        "State": IndexStateType,
-        "Tags": Dict[str, str],
-        "Type": IndexTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetViewInputRequestTypeDef = TypedDict(
-    "GetViewInputRequestTypeDef",
-    {
-        "ViewArn": str,
+        "Name": str,
     },
 )
 
 IndexTypeDef = TypedDict(
     "IndexTypeDef",
     {
         "Arn": str,
         "Region": str,
         "Type": IndexTypeType,
     },
     total=False,
 )
 
-ListIndexesInputListIndexesPaginateTypeDef = TypedDict(
-    "ListIndexesInputListIndexesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Regions": Sequence[str],
-        "Type": IndexTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListIndexesInputRequestTypeDef = TypedDict(
     "ListIndexesInputRequestTypeDef",
     {
@@ -234,22 +188,14 @@
         "NextToken": str,
         "Regions": Sequence[str],
         "Type": IndexTypeType,
     },
     total=False,
 )
 
-ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef = TypedDict(
-    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSupportedResourceTypesInputRequestTypeDef = TypedDict(
     "ListSupportedResourceTypesInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -267,58 +213,23 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListViewsInputListViewsPaginateTypeDef = TypedDict(
-    "ListViewsInputListViewsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListViewsInputRequestTypeDef = TypedDict(
     "ListViewsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListViewsOutputTypeDef = TypedDict(
-    "ListViewsOutputTypeDef",
-    {
-        "NextToken": str,
-        "Views": List[str],
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
 ResourceCountTypeDef = TypedDict(
     "ResourceCountTypeDef",
     {
         "Complete": bool,
         "TotalResources": int,
     },
     total=False,
@@ -330,22 +241,18 @@
         "Data": Dict[str, Any],
         "LastReportedAt": datetime,
         "Name": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+SearchFilterOutputTypeDef = TypedDict(
+    "SearchFilterOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "FilterString": str,
     },
 )
 
 _RequiredSearchInputRequestTypeDef = TypedDict(
     "_RequiredSearchInputRequestTypeDef",
     {
         "QueryString": str,
@@ -364,36 +271,14 @@
 
 class SearchInputRequestTypeDef(
     _RequiredSearchInputRequestTypeDef, _OptionalSearchInputRequestTypeDef
 ):
     pass
 
 
-_RequiredSearchInputSearchPaginateTypeDef = TypedDict(
-    "_RequiredSearchInputSearchPaginateTypeDef",
-    {
-        "QueryString": str,
-    },
-)
-_OptionalSearchInputSearchPaginateTypeDef = TypedDict(
-    "_OptionalSearchInputSearchPaginateTypeDef",
-    {
-        "ViewArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class SearchInputSearchPaginateTypeDef(
-    _RequiredSearchInputSearchPaginateTypeDef, _OptionalSearchInputSearchPaginateTypeDef
-):
-    pass
-
-
 _RequiredTagResourceInputRequestTypeDef = TypedDict(
     "_RequiredTagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalTagResourceInputRequestTypeDef = TypedDict(
@@ -423,22 +308,105 @@
     "UpdateIndexTypeInputRequestTypeDef",
     {
         "Arn": str,
         "Type": IndexTypeType,
     },
 )
 
+AssociateDefaultViewOutputTypeDef = TypedDict(
+    "AssociateDefaultViewOutputTypeDef",
+    {
+        "ViewArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIndexOutputTypeDef = TypedDict(
+    "CreateIndexOutputTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "State": IndexStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteIndexOutputTypeDef = TypedDict(
+    "DeleteIndexOutputTypeDef",
+    {
+        "Arn": str,
+        "LastUpdatedAt": datetime,
+        "State": IndexStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteViewOutputTypeDef = TypedDict(
+    "DeleteViewOutputTypeDef",
+    {
+        "ViewArn": str,
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
+GetDefaultViewOutputTypeDef = TypedDict(
+    "GetDefaultViewOutputTypeDef",
+    {
+        "ViewArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIndexOutputTypeDef = TypedDict(
+    "GetIndexOutputTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "ReplicatingFrom": List[str],
+        "ReplicatingTo": List[str],
+        "State": IndexStateType,
+        "Tags": Dict[str, str],
+        "Type": IndexTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListViewsOutputTypeDef = TypedDict(
+    "ListViewsOutputTypeDef",
+    {
+        "NextToken": str,
+        "Views": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateIndexTypeOutputTypeDef = TypedDict(
     "UpdateIndexTypeOutputTypeDef",
     {
         "Arn": str,
         "LastUpdatedAt": datetime,
         "State": IndexStateType,
         "Type": IndexTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateViewInputRequestTypeDef = TypedDict(
     "_RequiredCreateViewInputRequestTypeDef",
     {
         "ViewName": str,
@@ -480,42 +448,77 @@
 
 class UpdateViewInputRequestTypeDef(
     _RequiredUpdateViewInputRequestTypeDef, _OptionalUpdateViewInputRequestTypeDef
 ):
     pass
 
 
-ViewTypeDef = TypedDict(
-    "ViewTypeDef",
+ListIndexesOutputTypeDef = TypedDict(
+    "ListIndexesOutputTypeDef",
     {
-        "Filters": SearchFilterTypeDef,
-        "IncludedProperties": List[IncludedPropertyTypeDef],
-        "LastUpdatedAt": datetime,
-        "Owner": str,
-        "Scope": str,
-        "ViewArn": str,
+        "Indexes": List[IndexTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIndexesInputListIndexesPaginateTypeDef = TypedDict(
+    "ListIndexesInputListIndexesPaginateTypeDef",
+    {
+        "Regions": Sequence[str],
+        "Type": IndexTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListIndexesOutputTypeDef = TypedDict(
-    "ListIndexesOutputTypeDef",
+ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef = TypedDict(
+    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
     {
-        "Indexes": List[IndexTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+ListViewsInputListViewsPaginateTypeDef = TypedDict(
+    "ListViewsInputListViewsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredSearchInputSearchPaginateTypeDef = TypedDict(
+    "_RequiredSearchInputSearchPaginateTypeDef",
+    {
+        "QueryString": str,
+    },
+)
+_OptionalSearchInputSearchPaginateTypeDef = TypedDict(
+    "_OptionalSearchInputSearchPaginateTypeDef",
+    {
+        "ViewArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class SearchInputSearchPaginateTypeDef(
+    _RequiredSearchInputSearchPaginateTypeDef, _OptionalSearchInputSearchPaginateTypeDef
+):
+    pass
+
+
 ListSupportedResourceTypesOutputTypeDef = TypedDict(
     "ListSupportedResourceTypesOutputTypeDef",
     {
         "NextToken": str,
         "ResourceTypes": List[SupportedResourceTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Arn": str,
@@ -525,51 +528,64 @@
         "Region": str,
         "ResourceType": str,
         "Service": str,
     },
     total=False,
 )
 
+ViewTypeDef = TypedDict(
+    "ViewTypeDef",
+    {
+        "Filters": SearchFilterOutputTypeDef,
+        "IncludedProperties": List[IncludedPropertyOutputTypeDef],
+        "LastUpdatedAt": datetime,
+        "Owner": str,
+        "Scope": str,
+        "ViewArn": str,
+    },
+    total=False,
+)
+
+SearchOutputTypeDef = TypedDict(
+    "SearchOutputTypeDef",
+    {
+        "Count": ResourceCountTypeDef,
+        "NextToken": str,
+        "Resources": List[ResourceTypeDef],
+        "ViewArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BatchGetViewOutputTypeDef = TypedDict(
     "BatchGetViewOutputTypeDef",
     {
         "Errors": List[BatchGetViewErrorTypeDef],
         "Views": List[ViewTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateViewOutputTypeDef = TypedDict(
     "CreateViewOutputTypeDef",
     {
         "View": ViewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetViewOutputTypeDef = TypedDict(
     "GetViewOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "View": ViewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateViewOutputTypeDef = TypedDict(
     "UpdateViewOutputTypeDef",
     {
         "View": ViewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SearchOutputTypeDef = TypedDict(
-    "SearchOutputTypeDef",
-    {
-        "Count": ResourceCountTypeDef,
-        "NextToken": str,
-        "Resources": List[ResourceTypeDef],
-        "ViewArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2/type_defs.pyi` & `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -20,75 +20,80 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateDefaultViewInputRequestTypeDef",
-    "AssociateDefaultViewOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetViewErrorTypeDef",
     "BatchGetViewInputRequestTypeDef",
     "CreateIndexInputRequestTypeDef",
-    "CreateIndexOutputTypeDef",
     "IncludedPropertyTypeDef",
     "SearchFilterTypeDef",
     "DeleteIndexInputRequestTypeDef",
-    "DeleteIndexOutputTypeDef",
     "DeleteViewInputRequestTypeDef",
-    "DeleteViewOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetDefaultViewOutputTypeDef",
-    "GetIndexOutputTypeDef",
     "GetViewInputRequestTypeDef",
+    "IncludedPropertyOutputTypeDef",
     "IndexTypeDef",
-    "ListIndexesInputListIndexesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListIndexesInputRequestTypeDef",
-    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
     "ListSupportedResourceTypesInputRequestTypeDef",
     "SupportedResourceTypeTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "ListViewsInputListViewsPaginateTypeDef",
     "ListViewsInputRequestTypeDef",
-    "ListViewsOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "ResourceCountTypeDef",
     "ResourcePropertyTypeDef",
-    "ResponseMetadataTypeDef",
+    "SearchFilterOutputTypeDef",
     "SearchInputRequestTypeDef",
-    "SearchInputSearchPaginateTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateIndexTypeInputRequestTypeDef",
+    "AssociateDefaultViewOutputTypeDef",
+    "CreateIndexOutputTypeDef",
+    "DeleteIndexOutputTypeDef",
+    "DeleteViewOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetDefaultViewOutputTypeDef",
+    "GetIndexOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "ListViewsOutputTypeDef",
     "UpdateIndexTypeOutputTypeDef",
     "CreateViewInputRequestTypeDef",
     "UpdateViewInputRequestTypeDef",
-    "ViewTypeDef",
     "ListIndexesOutputTypeDef",
+    "ListIndexesInputListIndexesPaginateTypeDef",
+    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
+    "ListViewsInputListViewsPaginateTypeDef",
+    "SearchInputSearchPaginateTypeDef",
     "ListSupportedResourceTypesOutputTypeDef",
     "ResourceTypeDef",
+    "ViewTypeDef",
+    "SearchOutputTypeDef",
     "BatchGetViewOutputTypeDef",
     "CreateViewOutputTypeDef",
     "GetViewOutputTypeDef",
     "UpdateViewOutputTypeDef",
-    "SearchOutputTypeDef",
 )
 
 AssociateDefaultViewInputRequestTypeDef = TypedDict(
     "AssociateDefaultViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
 )
 
-AssociateDefaultViewOutputTypeDef = TypedDict(
-    "AssociateDefaultViewOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ViewArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 BatchGetViewErrorTypeDef = TypedDict(
     "BatchGetViewErrorTypeDef",
     {
         "ErrorMessage": str,
@@ -109,24 +114,14 @@
     {
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-CreateIndexOutputTypeDef = TypedDict(
-    "CreateIndexOutputTypeDef",
-    {
-        "Arn": str,
-        "CreatedAt": datetime,
-        "State": IndexStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IncludedPropertyTypeDef = TypedDict(
     "IncludedPropertyTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -140,92 +135,51 @@
 DeleteIndexInputRequestTypeDef = TypedDict(
     "DeleteIndexInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DeleteIndexOutputTypeDef = TypedDict(
-    "DeleteIndexOutputTypeDef",
-    {
-        "Arn": str,
-        "LastUpdatedAt": datetime,
-        "State": IndexStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteViewInputRequestTypeDef = TypedDict(
     "DeleteViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
 )
 
-DeleteViewOutputTypeDef = TypedDict(
-    "DeleteViewOutputTypeDef",
-    {
-        "ViewArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDefaultViewOutputTypeDef = TypedDict(
-    "GetDefaultViewOutputTypeDef",
+GetViewInputRequestTypeDef = TypedDict(
+    "GetViewInputRequestTypeDef",
     {
         "ViewArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetIndexOutputTypeDef = TypedDict(
-    "GetIndexOutputTypeDef",
+IncludedPropertyOutputTypeDef = TypedDict(
+    "IncludedPropertyOutputTypeDef",
     {
-        "Arn": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "ReplicatingFrom": List[str],
-        "ReplicatingTo": List[str],
-        "State": IndexStateType,
-        "Tags": Dict[str, str],
-        "Type": IndexTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetViewInputRequestTypeDef = TypedDict(
-    "GetViewInputRequestTypeDef",
-    {
-        "ViewArn": str,
+        "Name": str,
     },
 )
 
 IndexTypeDef = TypedDict(
     "IndexTypeDef",
     {
         "Arn": str,
         "Region": str,
         "Type": IndexTypeType,
     },
     total=False,
 )
 
-ListIndexesInputListIndexesPaginateTypeDef = TypedDict(
-    "ListIndexesInputListIndexesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Regions": Sequence[str],
-        "Type": IndexTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListIndexesInputRequestTypeDef = TypedDict(
     "ListIndexesInputRequestTypeDef",
     {
@@ -233,22 +187,14 @@
         "NextToken": str,
         "Regions": Sequence[str],
         "Type": IndexTypeType,
     },
     total=False,
 )
 
-ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef = TypedDict(
-    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSupportedResourceTypesInputRequestTypeDef = TypedDict(
     "ListSupportedResourceTypesInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -266,58 +212,23 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListViewsInputListViewsPaginateTypeDef = TypedDict(
-    "ListViewsInputListViewsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListViewsInputRequestTypeDef = TypedDict(
     "ListViewsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListViewsOutputTypeDef = TypedDict(
-    "ListViewsOutputTypeDef",
-    {
-        "NextToken": str,
-        "Views": List[str],
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
 ResourceCountTypeDef = TypedDict(
     "ResourceCountTypeDef",
     {
         "Complete": bool,
         "TotalResources": int,
     },
     total=False,
@@ -329,22 +240,18 @@
         "Data": Dict[str, Any],
         "LastReportedAt": datetime,
         "Name": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+SearchFilterOutputTypeDef = TypedDict(
+    "SearchFilterOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "FilterString": str,
     },
 )
 
 _RequiredSearchInputRequestTypeDef = TypedDict(
     "_RequiredSearchInputRequestTypeDef",
     {
         "QueryString": str,
@@ -361,34 +268,14 @@
 )
 
 class SearchInputRequestTypeDef(
     _RequiredSearchInputRequestTypeDef, _OptionalSearchInputRequestTypeDef
 ):
     pass
 
-_RequiredSearchInputSearchPaginateTypeDef = TypedDict(
-    "_RequiredSearchInputSearchPaginateTypeDef",
-    {
-        "QueryString": str,
-    },
-)
-_OptionalSearchInputSearchPaginateTypeDef = TypedDict(
-    "_OptionalSearchInputSearchPaginateTypeDef",
-    {
-        "ViewArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class SearchInputSearchPaginateTypeDef(
-    _RequiredSearchInputSearchPaginateTypeDef, _OptionalSearchInputSearchPaginateTypeDef
-):
-    pass
-
 _RequiredTagResourceInputRequestTypeDef = TypedDict(
     "_RequiredTagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalTagResourceInputRequestTypeDef = TypedDict(
@@ -416,22 +303,105 @@
     "UpdateIndexTypeInputRequestTypeDef",
     {
         "Arn": str,
         "Type": IndexTypeType,
     },
 )
 
+AssociateDefaultViewOutputTypeDef = TypedDict(
+    "AssociateDefaultViewOutputTypeDef",
+    {
+        "ViewArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIndexOutputTypeDef = TypedDict(
+    "CreateIndexOutputTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "State": IndexStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteIndexOutputTypeDef = TypedDict(
+    "DeleteIndexOutputTypeDef",
+    {
+        "Arn": str,
+        "LastUpdatedAt": datetime,
+        "State": IndexStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteViewOutputTypeDef = TypedDict(
+    "DeleteViewOutputTypeDef",
+    {
+        "ViewArn": str,
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
+GetDefaultViewOutputTypeDef = TypedDict(
+    "GetDefaultViewOutputTypeDef",
+    {
+        "ViewArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIndexOutputTypeDef = TypedDict(
+    "GetIndexOutputTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "ReplicatingFrom": List[str],
+        "ReplicatingTo": List[str],
+        "State": IndexStateType,
+        "Tags": Dict[str, str],
+        "Type": IndexTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListViewsOutputTypeDef = TypedDict(
+    "ListViewsOutputTypeDef",
+    {
+        "NextToken": str,
+        "Views": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateIndexTypeOutputTypeDef = TypedDict(
     "UpdateIndexTypeOutputTypeDef",
     {
         "Arn": str,
         "LastUpdatedAt": datetime,
         "State": IndexStateType,
         "Type": IndexTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateViewInputRequestTypeDef = TypedDict(
     "_RequiredCreateViewInputRequestTypeDef",
     {
         "ViewName": str,
@@ -469,42 +439,75 @@
 )
 
 class UpdateViewInputRequestTypeDef(
     _RequiredUpdateViewInputRequestTypeDef, _OptionalUpdateViewInputRequestTypeDef
 ):
     pass
 
-ViewTypeDef = TypedDict(
-    "ViewTypeDef",
+ListIndexesOutputTypeDef = TypedDict(
+    "ListIndexesOutputTypeDef",
     {
-        "Filters": SearchFilterTypeDef,
-        "IncludedProperties": List[IncludedPropertyTypeDef],
-        "LastUpdatedAt": datetime,
-        "Owner": str,
-        "Scope": str,
-        "ViewArn": str,
+        "Indexes": List[IndexTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIndexesInputListIndexesPaginateTypeDef = TypedDict(
+    "ListIndexesInputListIndexesPaginateTypeDef",
+    {
+        "Regions": Sequence[str],
+        "Type": IndexTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListIndexesOutputTypeDef = TypedDict(
-    "ListIndexesOutputTypeDef",
+ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef = TypedDict(
+    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
     {
-        "Indexes": List[IndexTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListViewsInputListViewsPaginateTypeDef = TypedDict(
+    "ListViewsInputListViewsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredSearchInputSearchPaginateTypeDef = TypedDict(
+    "_RequiredSearchInputSearchPaginateTypeDef",
+    {
+        "QueryString": str,
+    },
+)
+_OptionalSearchInputSearchPaginateTypeDef = TypedDict(
+    "_OptionalSearchInputSearchPaginateTypeDef",
+    {
+        "ViewArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+class SearchInputSearchPaginateTypeDef(
+    _RequiredSearchInputSearchPaginateTypeDef, _OptionalSearchInputSearchPaginateTypeDef
+):
+    pass
+
 ListSupportedResourceTypesOutputTypeDef = TypedDict(
     "ListSupportedResourceTypesOutputTypeDef",
     {
         "NextToken": str,
         "ResourceTypes": List[SupportedResourceTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Arn": str,
@@ -514,51 +517,64 @@
         "Region": str,
         "ResourceType": str,
         "Service": str,
     },
     total=False,
 )
 
+ViewTypeDef = TypedDict(
+    "ViewTypeDef",
+    {
+        "Filters": SearchFilterOutputTypeDef,
+        "IncludedProperties": List[IncludedPropertyOutputTypeDef],
+        "LastUpdatedAt": datetime,
+        "Owner": str,
+        "Scope": str,
+        "ViewArn": str,
+    },
+    total=False,
+)
+
+SearchOutputTypeDef = TypedDict(
+    "SearchOutputTypeDef",
+    {
+        "Count": ResourceCountTypeDef,
+        "NextToken": str,
+        "Resources": List[ResourceTypeDef],
+        "ViewArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BatchGetViewOutputTypeDef = TypedDict(
     "BatchGetViewOutputTypeDef",
     {
         "Errors": List[BatchGetViewErrorTypeDef],
         "Views": List[ViewTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateViewOutputTypeDef = TypedDict(
     "CreateViewOutputTypeDef",
     {
         "View": ViewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetViewOutputTypeDef = TypedDict(
     "GetViewOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "View": ViewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateViewOutputTypeDef = TypedDict(
     "UpdateViewOutputTypeDef",
     {
         "View": ViewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SearchOutputTypeDef = TypedDict(
-    "SearchOutputTypeDef",
-    {
-        "Count": ResourceCountTypeDef,
-        "NextToken": str,
-        "Resources": List[ResourceTypeDef],
-        "ViewArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2.egg-info/PKG-INFO` & `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resource-explorer-2
-Version: 1.28.0
-Summary: Type annotations for boto3.ResourceExplorer 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ResourceExplorer 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-resource-explorer-2"></a>
 
 # mypy-boto3-resource-explorer-2
 
 [![PyPI - mypy-boto3-resource-explorer-2](https://img.shields.io/pypi/v/mypy-boto3-resource-explorer-2.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-explorer-2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-explorer-2.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-explorer-2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resource-explorer-2?color=blue)](https://pypistats.org/packages/mypy-boto3-resource-explorer-2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resource-explorer-2)](https://pepy.tech/project/mypy-boto3-resource-explorer-2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceExplorer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
+[boto3.ResourceExplorer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
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
 [mypy-boto3-resource-explorer-2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,61 +336,63 @@
 
 `mypy_boto3_resource_explorer_2.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resource_explorer_2.type_defs import (
     AssociateDefaultViewInputRequestTypeDef,
-    AssociateDefaultViewOutputTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetViewErrorTypeDef,
     BatchGetViewInputRequestTypeDef,
     CreateIndexInputRequestTypeDef,
-    CreateIndexOutputTypeDef,
     IncludedPropertyTypeDef,
     SearchFilterTypeDef,
     DeleteIndexInputRequestTypeDef,
-    DeleteIndexOutputTypeDef,
     DeleteViewInputRequestTypeDef,
-    DeleteViewOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDefaultViewOutputTypeDef,
-    GetIndexOutputTypeDef,
     GetViewInputRequestTypeDef,
+    IncludedPropertyOutputTypeDef,
     IndexTypeDef,
-    ListIndexesInputListIndexesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListIndexesInputRequestTypeDef,
-    ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
     ListSupportedResourceTypesInputRequestTypeDef,
     SupportedResourceTypeTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListViewsInputListViewsPaginateTypeDef,
     ListViewsInputRequestTypeDef,
-    ListViewsOutputTypeDef,
-    PaginatorConfigTypeDef,
     ResourceCountTypeDef,
     ResourcePropertyTypeDef,
-    ResponseMetadataTypeDef,
+    SearchFilterOutputTypeDef,
     SearchInputRequestTypeDef,
-    SearchInputSearchPaginateTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateIndexTypeInputRequestTypeDef,
+    AssociateDefaultViewOutputTypeDef,
+    CreateIndexOutputTypeDef,
+    DeleteIndexOutputTypeDef,
+    DeleteViewOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDefaultViewOutputTypeDef,
+    GetIndexOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    ListViewsOutputTypeDef,
     UpdateIndexTypeOutputTypeDef,
     CreateViewInputRequestTypeDef,
     UpdateViewInputRequestTypeDef,
-    ViewTypeDef,
     ListIndexesOutputTypeDef,
+    ListIndexesInputListIndexesPaginateTypeDef,
+    ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
+    ListViewsInputListViewsPaginateTypeDef,
+    SearchInputSearchPaginateTypeDef,
     ListSupportedResourceTypesOutputTypeDef,
     ResourceTypeDef,
+    ViewTypeDef,
+    SearchOutputTypeDef,
     BatchGetViewOutputTypeDef,
     CreateViewOutputTypeDef,
     GetViewOutputTypeDef,
     UpdateViewOutputTypeDef,
-    SearchOutputTypeDef,
 )
 
 
 def get_structure() -> AssociateDefaultViewInputRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-resource-explorer-2-1.28.0/mypy_boto3_resource_explorer_2.egg-info/SOURCES.txt` & `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-explorer-2-1.28.0/setup.py` & `mypy-boto3-resource-explorer-2-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-resource-explorer-2",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_resource_explorer_2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ResourceExplorer 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ResourceExplorer 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

