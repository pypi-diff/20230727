# Comparing `tmp/mypy-boto3-schemas-1.28.0.tar.gz` & `tmp/mypy-boto3-schemas-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-schemas-1.28.0.tar", last modified: Thu Jul  6 21:00:35 2023, max compression
+gzip compressed data, was "mypy-boto3-schemas-1.28.12.tar", last modified: Thu Jul 27 11:49:36 2023, max compression
```

## Comparing `mypy-boto3-schemas-1.28.0.tar` & `mypy-boto3-schemas-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:35.038426 mypy-boto3-schemas-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:54:58.000000 mypy-boto3-schemas-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-06 21:00:35.030426 mypy-boto3-schemas-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-07-06 20:54:58.000000 mypy-boto3-schemas-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:35.026426 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-06 20:54:58.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-06 20:54:58.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 20:54:58.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23385 2023-07-06 20:54:59.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23341 2023-07-06 20:54:58.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-06 20:54:59.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-07-06 20:54:59.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-06 20:54:59.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-07-06 20:54:59.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:54:58.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26173 2023-07-06 20:55:00.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26134 2023-07-06 20:54:59.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:54:58.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-06 20:54:59.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-06 20:54:59.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:35.030426 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-06 21:00:34.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-06 21:00:34.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:34.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:34.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:34.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 21:00:34.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:35.038426 mypy-boto3-schemas-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-06 20:54:58.000000 mypy-boto3-schemas-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:36.041267 mypy-boto3-schemas-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:03.000000 mypy-boto3-schemas-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16656 2023-07-27 11:49:36.041267 mypy-boto3-schemas-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-07-27 11:46:03.000000 mypy-boto3-schemas-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:36.041267 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-27 11:46:03.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-27 11:46:03.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 11:46:03.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23385 2023-07-27 11:46:05.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23341 2023-07-27 11:46:03.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-07-27 11:46:05.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-07-27 11:46:05.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-07-27 11:46:05.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-27 11:46:05.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:03.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26113 2023-07-27 11:46:06.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26074 2023-07-27 11:46:05.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:03.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-27 11:46:05.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-27 11:46:05.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:36.041267 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16656 2023-07-27 11:49:35.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-27 11:49:35.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:35.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:35.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:35.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 11:49:35.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:36.041267 mypy-boto3-schemas-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 11:46:03.000000 mypy-boto3-schemas-1.28.12/setup.py
```

### Comparing `mypy-boto3-schemas-1.28.0/LICENSE` & `mypy-boto3-schemas-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.0/PKG-INFO` & `mypy-boto3-schemas-1.28.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-schemas
-Version: 1.28.0
-Summary: Type annotations for boto3.Schemas 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Schemas 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-schemas"></a>
 
 # mypy-boto3-schemas
 
 [![PyPI - mypy-boto3-schemas](https://img.shields.io/pypi/v/mypy-boto3-schemas.svg?color=blue)](https://pypi.org/project/mypy-boto3-schemas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-schemas.svg?color=blue)](https://pypi.org/project/mypy-boto3-schemas)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-schemas?color=blue)](https://pypistats.org/packages/mypy-boto3-schemas)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-schemas)](https://pepy.tech/project/mypy-boto3-schemas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Schemas 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
+[boto3.Schemas 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
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
 [mypy-boto3-schemas docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/).
 
 See how it helps to find and fix potential bugs:
 
@@ -360,79 +360,79 @@
 
 `mypy_boto3_schemas.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_schemas.type_defs import (
     CreateDiscovererRequestRequestTypeDef,
-    CreateDiscovererResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateRegistryRequestRequestTypeDef,
-    CreateRegistryResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
-    CreateSchemaResponseTypeDef,
     DeleteDiscovererRequestRequestTypeDef,
     DeleteRegistryRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSchemaRequestRequestTypeDef,
     DeleteSchemaVersionRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCodeBindingRequestRequestTypeDef,
-    DescribeCodeBindingResponseTypeDef,
     DescribeDiscovererRequestRequestTypeDef,
-    DescribeDiscovererResponseTypeDef,
     DescribeRegistryRequestRequestTypeDef,
-    DescribeRegistryResponseTypeDef,
     DescribeSchemaRequestRequestTypeDef,
-    DescribeSchemaResponseTypeDef,
     DiscovererSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportSchemaRequestRequestTypeDef,
-    ExportSchemaResponseTypeDef,
     GetCodeBindingSourceRequestRequestTypeDef,
-    GetCodeBindingSourceResponseTypeDef,
     GetDiscoveredSchemaRequestRequestTypeDef,
-    GetDiscoveredSchemaResponseTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    ListDiscoverersRequestListDiscoverersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDiscoverersRequestRequestTypeDef,
-    ListRegistriesRequestListRegistriesPaginateTypeDef,
     ListRegistriesRequestRequestTypeDef,
     RegistrySummaryTypeDef,
-    ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
     ListSchemaVersionsRequestRequestTypeDef,
     SchemaVersionSummaryTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
     SchemaSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutCodeBindingRequestRequestTypeDef,
-    PutCodeBindingResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    ResponseMetadataTypeDef,
     SearchSchemaVersionSummaryTypeDef,
     SearchSchemasRequestRequestTypeDef,
-    SearchSchemasRequestSearchSchemasPaginateTypeDef,
     StartDiscovererRequestRequestTypeDef,
-    StartDiscovererResponseTypeDef,
     StopDiscovererRequestRequestTypeDef,
-    StopDiscovererResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDiscovererRequestRequestTypeDef,
-    UpdateDiscovererResponseTypeDef,
     UpdateRegistryRequestRequestTypeDef,
-    UpdateRegistryResponseTypeDef,
     UpdateSchemaRequestRequestTypeDef,
+    CreateDiscovererResponseTypeDef,
+    CreateRegistryResponseTypeDef,
+    CreateSchemaResponseTypeDef,
+    DescribeCodeBindingResponseTypeDef,
+    DescribeDiscovererResponseTypeDef,
+    DescribeRegistryResponseTypeDef,
+    DescribeSchemaResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportSchemaResponseTypeDef,
+    GetCodeBindingSourceResponseTypeDef,
+    GetDiscoveredSchemaResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutCodeBindingResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    StartDiscovererResponseTypeDef,
+    StopDiscovererResponseTypeDef,
+    UpdateDiscovererResponseTypeDef,
+    UpdateRegistryResponseTypeDef,
     UpdateSchemaResponseTypeDef,
     DescribeCodeBindingRequestCodeBindingExistsWaitTypeDef,
     ListDiscoverersResponseTypeDef,
+    ListDiscoverersRequestListDiscoverersPaginateTypeDef,
+    ListRegistriesRequestListRegistriesPaginateTypeDef,
+    ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
+    ListSchemasRequestListSchemasPaginateTypeDef,
+    SearchSchemasRequestSearchSchemasPaginateTypeDef,
     ListRegistriesResponseTypeDef,
     ListSchemaVersionsResponseTypeDef,
     ListSchemasResponseTypeDef,
     SearchSchemaSummaryTypeDef,
     SearchSchemasResponseTypeDef,
 )
```

### Comparing `mypy-boto3-schemas-1.28.0/README.md` & `mypy-boto3-schemas-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-schemas"></a>
 
 # mypy-boto3-schemas
 
 [![PyPI - mypy-boto3-schemas](https://img.shields.io/pypi/v/mypy-boto3-schemas.svg?color=blue)](https://pypi.org/project/mypy-boto3-schemas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-schemas.svg?color=blue)](https://pypi.org/project/mypy-boto3-schemas)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-schemas?color=blue)](https://pypistats.org/packages/mypy-boto3-schemas)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-schemas)](https://pepy.tech/project/mypy-boto3-schemas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Schemas 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
+[boto3.Schemas 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
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
 [mypy-boto3-schemas docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/).
 
 See how it helps to find and fix potential bugs:
 
@@ -328,79 +328,79 @@
 
 `mypy_boto3_schemas.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_schemas.type_defs import (
     CreateDiscovererRequestRequestTypeDef,
-    CreateDiscovererResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateRegistryRequestRequestTypeDef,
-    CreateRegistryResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
-    CreateSchemaResponseTypeDef,
     DeleteDiscovererRequestRequestTypeDef,
     DeleteRegistryRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSchemaRequestRequestTypeDef,
     DeleteSchemaVersionRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCodeBindingRequestRequestTypeDef,
-    DescribeCodeBindingResponseTypeDef,
     DescribeDiscovererRequestRequestTypeDef,
-    DescribeDiscovererResponseTypeDef,
     DescribeRegistryRequestRequestTypeDef,
-    DescribeRegistryResponseTypeDef,
     DescribeSchemaRequestRequestTypeDef,
-    DescribeSchemaResponseTypeDef,
     DiscovererSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportSchemaRequestRequestTypeDef,
-    ExportSchemaResponseTypeDef,
     GetCodeBindingSourceRequestRequestTypeDef,
-    GetCodeBindingSourceResponseTypeDef,
     GetDiscoveredSchemaRequestRequestTypeDef,
-    GetDiscoveredSchemaResponseTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    ListDiscoverersRequestListDiscoverersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDiscoverersRequestRequestTypeDef,
-    ListRegistriesRequestListRegistriesPaginateTypeDef,
     ListRegistriesRequestRequestTypeDef,
     RegistrySummaryTypeDef,
-    ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
     ListSchemaVersionsRequestRequestTypeDef,
     SchemaVersionSummaryTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
     SchemaSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutCodeBindingRequestRequestTypeDef,
-    PutCodeBindingResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    ResponseMetadataTypeDef,
     SearchSchemaVersionSummaryTypeDef,
     SearchSchemasRequestRequestTypeDef,
-    SearchSchemasRequestSearchSchemasPaginateTypeDef,
     StartDiscovererRequestRequestTypeDef,
-    StartDiscovererResponseTypeDef,
     StopDiscovererRequestRequestTypeDef,
-    StopDiscovererResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDiscovererRequestRequestTypeDef,
-    UpdateDiscovererResponseTypeDef,
     UpdateRegistryRequestRequestTypeDef,
-    UpdateRegistryResponseTypeDef,
     UpdateSchemaRequestRequestTypeDef,
+    CreateDiscovererResponseTypeDef,
+    CreateRegistryResponseTypeDef,
+    CreateSchemaResponseTypeDef,
+    DescribeCodeBindingResponseTypeDef,
+    DescribeDiscovererResponseTypeDef,
+    DescribeRegistryResponseTypeDef,
+    DescribeSchemaResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportSchemaResponseTypeDef,
+    GetCodeBindingSourceResponseTypeDef,
+    GetDiscoveredSchemaResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutCodeBindingResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    StartDiscovererResponseTypeDef,
+    StopDiscovererResponseTypeDef,
+    UpdateDiscovererResponseTypeDef,
+    UpdateRegistryResponseTypeDef,
     UpdateSchemaResponseTypeDef,
     DescribeCodeBindingRequestCodeBindingExistsWaitTypeDef,
     ListDiscoverersResponseTypeDef,
+    ListDiscoverersRequestListDiscoverersPaginateTypeDef,
+    ListRegistriesRequestListRegistriesPaginateTypeDef,
+    ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
+    ListSchemasRequestListSchemasPaginateTypeDef,
+    SearchSchemasRequestSearchSchemasPaginateTypeDef,
     ListRegistriesResponseTypeDef,
     ListSchemaVersionsResponseTypeDef,
     ListSchemasResponseTypeDef,
     SearchSchemaSummaryTypeDef,
     SearchSchemasResponseTypeDef,
 )
```

### Comparing `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/__init__.py` & `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/__init__.pyi` & `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/__main__.py` & `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Schemas 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Schemas 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas\nOther"
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

### Comparing `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/client.py` & `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/client.pyi` & `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/literals.py` & `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,15 @@
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
@@ -249,26 +250,28 @@
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

### Comparing `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/literals.pyi` & `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,15 @@
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
@@ -247,26 +248,28 @@
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

### Comparing `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/paginator.py` & `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     """
 
     def paginate(
         self,
         *,
         DiscovererIdPrefix: str = ...,
         SourceArnPrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDiscoverersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListDiscoverers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listdiscovererspaginator)
         """
 
 
@@ -85,34 +85,30 @@
     """
 
     def paginate(
         self,
         *,
         RegistryNamePrefix: str = ...,
         Scope: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRegistriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListRegistries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listregistriespaginator)
         """
 
 
 class ListSchemaVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemaVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listschemaversionspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        RegistryName: str,
-        SchemaName: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RegistryName: str, SchemaName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSchemaVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemaVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listschemaversionspaginator)
         """
 
 
@@ -123,28 +119,28 @@
     """
 
     def paginate(
         self,
         *,
         RegistryName: str,
         SchemaNamePrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listschemaspaginator)
         """
 
 
 class SearchSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.SearchSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#searchschemaspaginator)
     """
 
     def paginate(
-        self, *, Keywords: str, RegistryName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Keywords: str, RegistryName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.SearchSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#searchschemaspaginator)
         """
```

### Comparing `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/paginator.pyi` & `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     """
 
     def paginate(
         self,
         *,
         DiscovererIdPrefix: str = ...,
         SourceArnPrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDiscoverersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListDiscoverers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listdiscovererspaginator)
         """
 
 class ListRegistriesPaginator(Paginator):
@@ -81,33 +81,29 @@
     """
 
     def paginate(
         self,
         *,
         RegistryNamePrefix: str = ...,
         Scope: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRegistriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListRegistries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listregistriespaginator)
         """
 
 class ListSchemaVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemaVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listschemaversionspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        RegistryName: str,
-        SchemaName: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RegistryName: str, SchemaName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSchemaVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemaVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listschemaversionspaginator)
         """
 
 class ListSchemasPaginator(Paginator):
@@ -117,27 +113,27 @@
     """
 
     def paginate(
         self,
         *,
         RegistryName: str,
         SchemaNamePrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#listschemaspaginator)
         """
 
 class SearchSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.SearchSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#searchschemaspaginator)
     """
 
     def paginate(
-        self, *, Keywords: str, RegistryName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Keywords: str, RegistryName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.SearchSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/paginators/#searchschemaspaginator)
         """
```

### Comparing `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/type_defs.py` & `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,79 +23,79 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CreateDiscovererRequestRequestTypeDef",
-    "CreateDiscovererResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateRegistryRequestRequestTypeDef",
-    "CreateRegistryResponseTypeDef",
     "CreateSchemaRequestRequestTypeDef",
-    "CreateSchemaResponseTypeDef",
     "DeleteDiscovererRequestRequestTypeDef",
     "DeleteRegistryRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteSchemaRequestRequestTypeDef",
     "DeleteSchemaVersionRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCodeBindingRequestRequestTypeDef",
-    "DescribeCodeBindingResponseTypeDef",
     "DescribeDiscovererRequestRequestTypeDef",
-    "DescribeDiscovererResponseTypeDef",
     "DescribeRegistryRequestRequestTypeDef",
-    "DescribeRegistryResponseTypeDef",
     "DescribeSchemaRequestRequestTypeDef",
-    "DescribeSchemaResponseTypeDef",
     "DiscovererSummaryTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportSchemaRequestRequestTypeDef",
-    "ExportSchemaResponseTypeDef",
     "GetCodeBindingSourceRequestRequestTypeDef",
-    "GetCodeBindingSourceResponseTypeDef",
     "GetDiscoveredSchemaRequestRequestTypeDef",
-    "GetDiscoveredSchemaResponseTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
-    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDiscoverersRequestRequestTypeDef",
-    "ListRegistriesRequestListRegistriesPaginateTypeDef",
     "ListRegistriesRequestRequestTypeDef",
     "RegistrySummaryTypeDef",
-    "ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
     "ListSchemaVersionsRequestRequestTypeDef",
     "SchemaVersionSummaryTypeDef",
-    "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSchemasRequestRequestTypeDef",
     "SchemaSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PutCodeBindingRequestRequestTypeDef",
-    "PutCodeBindingResponseTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "PutResourcePolicyResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchSchemaVersionSummaryTypeDef",
     "SearchSchemasRequestRequestTypeDef",
-    "SearchSchemasRequestSearchSchemasPaginateTypeDef",
     "StartDiscovererRequestRequestTypeDef",
-    "StartDiscovererResponseTypeDef",
     "StopDiscovererRequestRequestTypeDef",
-    "StopDiscovererResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDiscovererRequestRequestTypeDef",
-    "UpdateDiscovererResponseTypeDef",
     "UpdateRegistryRequestRequestTypeDef",
-    "UpdateRegistryResponseTypeDef",
     "UpdateSchemaRequestRequestTypeDef",
+    "CreateDiscovererResponseTypeDef",
+    "CreateRegistryResponseTypeDef",
+    "CreateSchemaResponseTypeDef",
+    "DescribeCodeBindingResponseTypeDef",
+    "DescribeDiscovererResponseTypeDef",
+    "DescribeRegistryResponseTypeDef",
+    "DescribeSchemaResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportSchemaResponseTypeDef",
+    "GetCodeBindingSourceResponseTypeDef",
+    "GetDiscoveredSchemaResponseTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutCodeBindingResponseTypeDef",
+    "PutResourcePolicyResponseTypeDef",
+    "StartDiscovererResponseTypeDef",
+    "StopDiscovererResponseTypeDef",
+    "UpdateDiscovererResponseTypeDef",
+    "UpdateRegistryResponseTypeDef",
     "UpdateSchemaResponseTypeDef",
     "DescribeCodeBindingRequestCodeBindingExistsWaitTypeDef",
     "ListDiscoverersResponseTypeDef",
+    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
+    "ListRegistriesRequestListRegistriesPaginateTypeDef",
+    "ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
+    "ListSchemasRequestListSchemasPaginateTypeDef",
+    "SearchSchemasRequestSearchSchemasPaginateTypeDef",
     "ListRegistriesResponseTypeDef",
     "ListSchemaVersionsResponseTypeDef",
     "ListSchemasResponseTypeDef",
     "SearchSchemaSummaryTypeDef",
     "SearchSchemasResponseTypeDef",
 )
 
@@ -118,25 +118,22 @@
 
 class CreateDiscovererRequestRequestTypeDef(
     _RequiredCreateDiscovererRequestRequestTypeDef, _OptionalCreateDiscovererRequestRequestTypeDef
 ):
     pass
 
 
-CreateDiscovererResponseTypeDef = TypedDict(
-    "CreateDiscovererResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Description": str,
-        "DiscovererArn": str,
-        "DiscovererId": str,
-        "SourceArn": str,
-        "State": DiscovererStateType,
-        "CrossAccount": bool,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateRegistryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRegistryRequestRequestTypeDef",
     {
         "RegistryName": str,
@@ -154,25 +151,14 @@
 
 class CreateRegistryRequestRequestTypeDef(
     _RequiredCreateRegistryRequestRequestTypeDef, _OptionalCreateRegistryRequestRequestTypeDef
 ):
     pass
 
 
-CreateRegistryResponseTypeDef = TypedDict(
-    "CreateRegistryResponseTypeDef",
-    {
-        "Description": str,
-        "RegistryArn": str,
-        "RegistryName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSchemaRequestRequestTypeDef",
     {
         "Content": str,
         "RegistryName": str,
         "SchemaName": str,
         "Type": TypeType,
@@ -190,29 +176,14 @@
 
 class CreateSchemaRequestRequestTypeDef(
     _RequiredCreateSchemaRequestRequestTypeDef, _OptionalCreateSchemaRequestRequestTypeDef
 ):
     pass
 
 
-CreateSchemaResponseTypeDef = TypedDict(
-    "CreateSchemaResponseTypeDef",
-    {
-        "Description": str,
-        "LastModified": datetime,
-        "SchemaArn": str,
-        "SchemaName": str,
-        "SchemaVersion": str,
-        "Tags": Dict[str, str],
-        "Type": str,
-        "VersionCreatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDiscovererRequestRequestTypeDef = TypedDict(
     "DeleteDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
@@ -277,64 +248,28 @@
 class DescribeCodeBindingRequestRequestTypeDef(
     _RequiredDescribeCodeBindingRequestRequestTypeDef,
     _OptionalDescribeCodeBindingRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeCodeBindingResponseTypeDef = TypedDict(
-    "DescribeCodeBindingResponseTypeDef",
-    {
-        "CreationDate": datetime,
-        "LastModified": datetime,
-        "SchemaVersion": str,
-        "Status": CodeGenerationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDiscovererRequestRequestTypeDef = TypedDict(
     "DescribeDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
-DescribeDiscovererResponseTypeDef = TypedDict(
-    "DescribeDiscovererResponseTypeDef",
-    {
-        "Description": str,
-        "DiscovererArn": str,
-        "DiscovererId": str,
-        "SourceArn": str,
-        "State": DiscovererStateType,
-        "CrossAccount": bool,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeRegistryRequestRequestTypeDef = TypedDict(
     "DescribeRegistryRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
 )
 
-DescribeRegistryResponseTypeDef = TypedDict(
-    "DescribeRegistryResponseTypeDef",
-    {
-        "Description": str,
-        "RegistryArn": str,
-        "RegistryName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSchemaRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
     },
 )
@@ -349,50 +284,27 @@
 
 class DescribeSchemaRequestRequestTypeDef(
     _RequiredDescribeSchemaRequestRequestTypeDef, _OptionalDescribeSchemaRequestRequestTypeDef
 ):
     pass
 
 
-DescribeSchemaResponseTypeDef = TypedDict(
-    "DescribeSchemaResponseTypeDef",
-    {
-        "Content": str,
-        "Description": str,
-        "LastModified": datetime,
-        "SchemaArn": str,
-        "SchemaName": str,
-        "SchemaVersion": str,
-        "Tags": Dict[str, str],
-        "Type": str,
-        "VersionCreatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DiscovererSummaryTypeDef = TypedDict(
     "DiscovererSummaryTypeDef",
     {
         "DiscovererArn": str,
         "DiscovererId": str,
         "SourceArn": str,
         "State": DiscovererStateType,
         "CrossAccount": bool,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredExportSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredExportSchemaRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
         "Type": str,
     },
@@ -408,26 +320,14 @@
 
 class ExportSchemaRequestRequestTypeDef(
     _RequiredExportSchemaRequestRequestTypeDef, _OptionalExportSchemaRequestRequestTypeDef
 ):
     pass
 
 
-ExportSchemaResponseTypeDef = TypedDict(
-    "ExportSchemaResponseTypeDef",
-    {
-        "Content": str,
-        "SchemaArn": str,
-        "SchemaName": str,
-        "SchemaVersion": str,
-        "Type": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetCodeBindingSourceRequestRequestTypeDef = TypedDict(
     "_RequiredGetCodeBindingSourceRequestRequestTypeDef",
     {
         "Language": str,
         "RegistryName": str,
         "SchemaName": str,
     },
@@ -444,61 +344,36 @@
 class GetCodeBindingSourceRequestRequestTypeDef(
     _RequiredGetCodeBindingSourceRequestRequestTypeDef,
     _OptionalGetCodeBindingSourceRequestRequestTypeDef,
 ):
     pass
 
 
-GetCodeBindingSourceResponseTypeDef = TypedDict(
-    "GetCodeBindingSourceResponseTypeDef",
-    {
-        "Body": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDiscoveredSchemaRequestRequestTypeDef = TypedDict(
     "GetDiscoveredSchemaRequestRequestTypeDef",
     {
         "Events": Sequence[str],
         "Type": TypeType,
     },
 )
 
-GetDiscoveredSchemaResponseTypeDef = TypedDict(
-    "GetDiscoveredSchemaResponseTypeDef",
-    {
-        "Content": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
     total=False,
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "RevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDiscoverersRequestListDiscoverersPaginateTypeDef = TypedDict(
-    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "DiscovererIdPrefix": str,
-        "SourceArnPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListDiscoverersRequestRequestTypeDef = TypedDict(
     "ListDiscoverersRequestRequestTypeDef",
     {
@@ -506,24 +381,14 @@
         "Limit": int,
         "NextToken": str,
         "SourceArnPrefix": str,
     },
     total=False,
 )
 
-ListRegistriesRequestListRegistriesPaginateTypeDef = TypedDict(
-    "ListRegistriesRequestListRegistriesPaginateTypeDef",
-    {
-        "RegistryNamePrefix": str,
-        "Scope": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRegistriesRequestRequestTypeDef = TypedDict(
     "ListRegistriesRequestRequestTypeDef",
     {
         "Limit": int,
         "NextToken": str,
         "RegistryNamePrefix": str,
         "Scope": str,
@@ -537,37 +402,14 @@
         "RegistryArn": str,
         "RegistryName": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
-    {
-        "RegistryName": str,
-        "SchemaName": str,
-    },
-)
-_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef(
-    _RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
-    _OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSchemaVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemaVersionsRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
     },
 )
@@ -595,37 +437,14 @@
         "SchemaName": str,
         "SchemaVersion": str,
         "Type": TypeType,
     },
     total=False,
 )
 
-_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "RegistryName": str,
-    },
-)
-_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "SchemaNamePrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSchemasRequestListSchemasPaginateTypeDef(
-    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
-    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSchemasRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemasRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
 )
 _OptionalListSchemasRequestRequestTypeDef = TypedDict(
@@ -660,32 +479,14 @@
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
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 _RequiredPutCodeBindingRequestRequestTypeDef = TypedDict(
     "_RequiredPutCodeBindingRequestRequestTypeDef",
     {
         "Language": str,
         "RegistryName": str,
         "SchemaName": str,
     },
@@ -701,25 +502,14 @@
 
 class PutCodeBindingRequestRequestTypeDef(
     _RequiredPutCodeBindingRequestRequestTypeDef, _OptionalPutCodeBindingRequestRequestTypeDef
 ):
     pass
 
 
-PutCodeBindingResponseTypeDef = TypedDict(
-    "PutCodeBindingResponseTypeDef",
-    {
-        "CreationDate": datetime,
-        "LastModified": datetime,
-        "SchemaVersion": str,
-        "Status": CodeGenerationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourcePolicyRequestRequestTypeDef",
     {
         "Policy": str,
     },
 )
 _OptionalPutResourcePolicyRequestRequestTypeDef = TypedDict(
@@ -734,34 +524,14 @@
 
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
 
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "RevisionId": str,
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
 SearchSchemaVersionSummaryTypeDef = TypedDict(
     "SearchSchemaVersionSummaryTypeDef",
     {
         "CreatedDate": datetime,
         "SchemaVersion": str,
         "Type": TypeType,
     },
@@ -787,69 +557,28 @@
 
 class SearchSchemasRequestRequestTypeDef(
     _RequiredSearchSchemasRequestRequestTypeDef, _OptionalSearchSchemasRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
-    "_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef",
-    {
-        "Keywords": str,
-        "RegistryName": str,
-    },
-)
-_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
-    "_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class SearchSchemasRequestSearchSchemasPaginateTypeDef(
-    _RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef,
-    _OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef,
-):
-    pass
-
-
 StartDiscovererRequestRequestTypeDef = TypedDict(
     "StartDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
-StartDiscovererResponseTypeDef = TypedDict(
-    "StartDiscovererResponseTypeDef",
-    {
-        "DiscovererId": str,
-        "State": DiscovererStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopDiscovererRequestRequestTypeDef = TypedDict(
     "StopDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
-StopDiscovererResponseTypeDef = TypedDict(
-    "StopDiscovererResponseTypeDef",
-    {
-        "DiscovererId": str,
-        "State": DiscovererStateType,
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
@@ -880,28 +609,14 @@
 
 class UpdateDiscovererRequestRequestTypeDef(
     _RequiredUpdateDiscovererRequestRequestTypeDef, _OptionalUpdateDiscovererRequestRequestTypeDef
 ):
     pass
 
 
-UpdateDiscovererResponseTypeDef = TypedDict(
-    "UpdateDiscovererResponseTypeDef",
-    {
-        "Description": str,
-        "DiscovererArn": str,
-        "DiscovererId": str,
-        "SourceArn": str,
-        "State": DiscovererStateType,
-        "CrossAccount": bool,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateRegistryRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRegistryRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
 )
 _OptionalUpdateRegistryRequestRequestTypeDef = TypedDict(
@@ -915,25 +630,14 @@
 
 class UpdateRegistryRequestRequestTypeDef(
     _RequiredUpdateRegistryRequestRequestTypeDef, _OptionalUpdateRegistryRequestRequestTypeDef
 ):
     pass
 
 
-UpdateRegistryResponseTypeDef = TypedDict(
-    "UpdateRegistryResponseTypeDef",
-    {
-        "Description": str,
-        "RegistryArn": str,
-        "RegistryName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSchemaRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
     },
 )
@@ -951,26 +655,233 @@
 
 class UpdateSchemaRequestRequestTypeDef(
     _RequiredUpdateSchemaRequestRequestTypeDef, _OptionalUpdateSchemaRequestRequestTypeDef
 ):
     pass
 
 
+CreateDiscovererResponseTypeDef = TypedDict(
+    "CreateDiscovererResponseTypeDef",
+    {
+        "Description": str,
+        "DiscovererArn": str,
+        "DiscovererId": str,
+        "SourceArn": str,
+        "State": DiscovererStateType,
+        "CrossAccount": bool,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRegistryResponseTypeDef = TypedDict(
+    "CreateRegistryResponseTypeDef",
+    {
+        "Description": str,
+        "RegistryArn": str,
+        "RegistryName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSchemaResponseTypeDef = TypedDict(
+    "CreateSchemaResponseTypeDef",
+    {
+        "Description": str,
+        "LastModified": datetime,
+        "SchemaArn": str,
+        "SchemaName": str,
+        "SchemaVersion": str,
+        "Tags": Dict[str, str],
+        "Type": str,
+        "VersionCreatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCodeBindingResponseTypeDef = TypedDict(
+    "DescribeCodeBindingResponseTypeDef",
+    {
+        "CreationDate": datetime,
+        "LastModified": datetime,
+        "SchemaVersion": str,
+        "Status": CodeGenerationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDiscovererResponseTypeDef = TypedDict(
+    "DescribeDiscovererResponseTypeDef",
+    {
+        "Description": str,
+        "DiscovererArn": str,
+        "DiscovererId": str,
+        "SourceArn": str,
+        "State": DiscovererStateType,
+        "CrossAccount": bool,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRegistryResponseTypeDef = TypedDict(
+    "DescribeRegistryResponseTypeDef",
+    {
+        "Description": str,
+        "RegistryArn": str,
+        "RegistryName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeSchemaResponseTypeDef = TypedDict(
+    "DescribeSchemaResponseTypeDef",
+    {
+        "Content": str,
+        "Description": str,
+        "LastModified": datetime,
+        "SchemaArn": str,
+        "SchemaName": str,
+        "SchemaVersion": str,
+        "Tags": Dict[str, str],
+        "Type": str,
+        "VersionCreatedDate": datetime,
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
+ExportSchemaResponseTypeDef = TypedDict(
+    "ExportSchemaResponseTypeDef",
+    {
+        "Content": str,
+        "SchemaArn": str,
+        "SchemaName": str,
+        "SchemaVersion": str,
+        "Type": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCodeBindingSourceResponseTypeDef = TypedDict(
+    "GetCodeBindingSourceResponseTypeDef",
+    {
+        "Body": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDiscoveredSchemaResponseTypeDef = TypedDict(
+    "GetDiscoveredSchemaResponseTypeDef",
+    {
+        "Content": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "RevisionId": str,
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
+PutCodeBindingResponseTypeDef = TypedDict(
+    "PutCodeBindingResponseTypeDef",
+    {
+        "CreationDate": datetime,
+        "LastModified": datetime,
+        "SchemaVersion": str,
+        "Status": CodeGenerationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "RevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDiscovererResponseTypeDef = TypedDict(
+    "StartDiscovererResponseTypeDef",
+    {
+        "DiscovererId": str,
+        "State": DiscovererStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopDiscovererResponseTypeDef = TypedDict(
+    "StopDiscovererResponseTypeDef",
+    {
+        "DiscovererId": str,
+        "State": DiscovererStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDiscovererResponseTypeDef = TypedDict(
+    "UpdateDiscovererResponseTypeDef",
+    {
+        "Description": str,
+        "DiscovererArn": str,
+        "DiscovererId": str,
+        "SourceArn": str,
+        "State": DiscovererStateType,
+        "CrossAccount": bool,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRegistryResponseTypeDef = TypedDict(
+    "UpdateRegistryResponseTypeDef",
+    {
+        "Description": str,
+        "RegistryArn": str,
+        "RegistryName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateSchemaResponseTypeDef = TypedDict(
     "UpdateSchemaResponseTypeDef",
     {
         "Description": str,
         "LastModified": datetime,
         "SchemaArn": str,
         "SchemaName": str,
         "SchemaVersion": str,
         "Tags": Dict[str, str],
         "Type": str,
         "VersionCreatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeCodeBindingRequestCodeBindingExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeCodeBindingRequestCodeBindingExistsWaitTypeDef",
     {
         "Language": str,
@@ -996,42 +907,131 @@
 
 
 ListDiscoverersResponseTypeDef = TypedDict(
     "ListDiscoverersResponseTypeDef",
     {
         "Discoverers": List[DiscovererSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListDiscoverersRequestListDiscoverersPaginateTypeDef = TypedDict(
+    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
+    {
+        "DiscovererIdPrefix": str,
+        "SourceArnPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRegistriesRequestListRegistriesPaginateTypeDef = TypedDict(
+    "ListRegistriesRequestListRegistriesPaginateTypeDef",
+    {
+        "RegistryNamePrefix": str,
+        "Scope": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
+    {
+        "RegistryName": str,
+        "SchemaName": str,
+    },
+)
+_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef(
+    _RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
+    _OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "RegistryName": str,
+    },
+)
+_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "SchemaNamePrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSchemasRequestListSchemasPaginateTypeDef(
+    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
+    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
+):
+    pass
+
+
+_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
+    "_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef",
+    {
+        "Keywords": str,
+        "RegistryName": str,
+    },
+)
+_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
+    "_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class SearchSchemasRequestSearchSchemasPaginateTypeDef(
+    _RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef,
+    _OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef,
+):
+    pass
+
+
 ListRegistriesResponseTypeDef = TypedDict(
     "ListRegistriesResponseTypeDef",
     {
         "NextToken": str,
         "Registries": List[RegistrySummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSchemaVersionsResponseTypeDef = TypedDict(
     "ListSchemaVersionsResponseTypeDef",
     {
         "NextToken": str,
         "SchemaVersions": List[SchemaVersionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSchemasResponseTypeDef = TypedDict(
     "ListSchemasResponseTypeDef",
     {
         "NextToken": str,
         "Schemas": List[SchemaSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchSchemaSummaryTypeDef = TypedDict(
     "SearchSchemaSummaryTypeDef",
     {
         "RegistryName": str,
@@ -1043,10 +1043,10 @@
 )
 
 SearchSchemasResponseTypeDef = TypedDict(
     "SearchSchemasResponseTypeDef",
     {
         "NextToken": str,
         "Schemas": List[SearchSchemaSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/type_defs.pyi` & `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -22,79 +22,79 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CreateDiscovererRequestRequestTypeDef",
-    "CreateDiscovererResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateRegistryRequestRequestTypeDef",
-    "CreateRegistryResponseTypeDef",
     "CreateSchemaRequestRequestTypeDef",
-    "CreateSchemaResponseTypeDef",
     "DeleteDiscovererRequestRequestTypeDef",
     "DeleteRegistryRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteSchemaRequestRequestTypeDef",
     "DeleteSchemaVersionRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCodeBindingRequestRequestTypeDef",
-    "DescribeCodeBindingResponseTypeDef",
     "DescribeDiscovererRequestRequestTypeDef",
-    "DescribeDiscovererResponseTypeDef",
     "DescribeRegistryRequestRequestTypeDef",
-    "DescribeRegistryResponseTypeDef",
     "DescribeSchemaRequestRequestTypeDef",
-    "DescribeSchemaResponseTypeDef",
     "DiscovererSummaryTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportSchemaRequestRequestTypeDef",
-    "ExportSchemaResponseTypeDef",
     "GetCodeBindingSourceRequestRequestTypeDef",
-    "GetCodeBindingSourceResponseTypeDef",
     "GetDiscoveredSchemaRequestRequestTypeDef",
-    "GetDiscoveredSchemaResponseTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
-    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDiscoverersRequestRequestTypeDef",
-    "ListRegistriesRequestListRegistriesPaginateTypeDef",
     "ListRegistriesRequestRequestTypeDef",
     "RegistrySummaryTypeDef",
-    "ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
     "ListSchemaVersionsRequestRequestTypeDef",
     "SchemaVersionSummaryTypeDef",
-    "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSchemasRequestRequestTypeDef",
     "SchemaSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PutCodeBindingRequestRequestTypeDef",
-    "PutCodeBindingResponseTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "PutResourcePolicyResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchSchemaVersionSummaryTypeDef",
     "SearchSchemasRequestRequestTypeDef",
-    "SearchSchemasRequestSearchSchemasPaginateTypeDef",
     "StartDiscovererRequestRequestTypeDef",
-    "StartDiscovererResponseTypeDef",
     "StopDiscovererRequestRequestTypeDef",
-    "StopDiscovererResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDiscovererRequestRequestTypeDef",
-    "UpdateDiscovererResponseTypeDef",
     "UpdateRegistryRequestRequestTypeDef",
-    "UpdateRegistryResponseTypeDef",
     "UpdateSchemaRequestRequestTypeDef",
+    "CreateDiscovererResponseTypeDef",
+    "CreateRegistryResponseTypeDef",
+    "CreateSchemaResponseTypeDef",
+    "DescribeCodeBindingResponseTypeDef",
+    "DescribeDiscovererResponseTypeDef",
+    "DescribeRegistryResponseTypeDef",
+    "DescribeSchemaResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportSchemaResponseTypeDef",
+    "GetCodeBindingSourceResponseTypeDef",
+    "GetDiscoveredSchemaResponseTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutCodeBindingResponseTypeDef",
+    "PutResourcePolicyResponseTypeDef",
+    "StartDiscovererResponseTypeDef",
+    "StopDiscovererResponseTypeDef",
+    "UpdateDiscovererResponseTypeDef",
+    "UpdateRegistryResponseTypeDef",
     "UpdateSchemaResponseTypeDef",
     "DescribeCodeBindingRequestCodeBindingExistsWaitTypeDef",
     "ListDiscoverersResponseTypeDef",
+    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
+    "ListRegistriesRequestListRegistriesPaginateTypeDef",
+    "ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
+    "ListSchemasRequestListSchemasPaginateTypeDef",
+    "SearchSchemasRequestSearchSchemasPaginateTypeDef",
     "ListRegistriesResponseTypeDef",
     "ListSchemaVersionsResponseTypeDef",
     "ListSchemasResponseTypeDef",
     "SearchSchemaSummaryTypeDef",
     "SearchSchemasResponseTypeDef",
 )
 
@@ -115,25 +115,22 @@
 )
 
 class CreateDiscovererRequestRequestTypeDef(
     _RequiredCreateDiscovererRequestRequestTypeDef, _OptionalCreateDiscovererRequestRequestTypeDef
 ):
     pass
 
-CreateDiscovererResponseTypeDef = TypedDict(
-    "CreateDiscovererResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Description": str,
-        "DiscovererArn": str,
-        "DiscovererId": str,
-        "SourceArn": str,
-        "State": DiscovererStateType,
-        "CrossAccount": bool,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateRegistryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRegistryRequestRequestTypeDef",
     {
         "RegistryName": str,
@@ -149,25 +146,14 @@
 )
 
 class CreateRegistryRequestRequestTypeDef(
     _RequiredCreateRegistryRequestRequestTypeDef, _OptionalCreateRegistryRequestRequestTypeDef
 ):
     pass
 
-CreateRegistryResponseTypeDef = TypedDict(
-    "CreateRegistryResponseTypeDef",
-    {
-        "Description": str,
-        "RegistryArn": str,
-        "RegistryName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSchemaRequestRequestTypeDef",
     {
         "Content": str,
         "RegistryName": str,
         "SchemaName": str,
         "Type": TypeType,
@@ -183,29 +169,14 @@
 )
 
 class CreateSchemaRequestRequestTypeDef(
     _RequiredCreateSchemaRequestRequestTypeDef, _OptionalCreateSchemaRequestRequestTypeDef
 ):
     pass
 
-CreateSchemaResponseTypeDef = TypedDict(
-    "CreateSchemaResponseTypeDef",
-    {
-        "Description": str,
-        "LastModified": datetime,
-        "SchemaArn": str,
-        "SchemaName": str,
-        "SchemaVersion": str,
-        "Tags": Dict[str, str],
-        "Type": str,
-        "VersionCreatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDiscovererRequestRequestTypeDef = TypedDict(
     "DeleteDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
@@ -268,64 +239,28 @@
 
 class DescribeCodeBindingRequestRequestTypeDef(
     _RequiredDescribeCodeBindingRequestRequestTypeDef,
     _OptionalDescribeCodeBindingRequestRequestTypeDef,
 ):
     pass
 
-DescribeCodeBindingResponseTypeDef = TypedDict(
-    "DescribeCodeBindingResponseTypeDef",
-    {
-        "CreationDate": datetime,
-        "LastModified": datetime,
-        "SchemaVersion": str,
-        "Status": CodeGenerationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDiscovererRequestRequestTypeDef = TypedDict(
     "DescribeDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
-DescribeDiscovererResponseTypeDef = TypedDict(
-    "DescribeDiscovererResponseTypeDef",
-    {
-        "Description": str,
-        "DiscovererArn": str,
-        "DiscovererId": str,
-        "SourceArn": str,
-        "State": DiscovererStateType,
-        "CrossAccount": bool,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeRegistryRequestRequestTypeDef = TypedDict(
     "DescribeRegistryRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
 )
 
-DescribeRegistryResponseTypeDef = TypedDict(
-    "DescribeRegistryResponseTypeDef",
-    {
-        "Description": str,
-        "RegistryArn": str,
-        "RegistryName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSchemaRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
     },
 )
@@ -338,50 +273,27 @@
 )
 
 class DescribeSchemaRequestRequestTypeDef(
     _RequiredDescribeSchemaRequestRequestTypeDef, _OptionalDescribeSchemaRequestRequestTypeDef
 ):
     pass
 
-DescribeSchemaResponseTypeDef = TypedDict(
-    "DescribeSchemaResponseTypeDef",
-    {
-        "Content": str,
-        "Description": str,
-        "LastModified": datetime,
-        "SchemaArn": str,
-        "SchemaName": str,
-        "SchemaVersion": str,
-        "Tags": Dict[str, str],
-        "Type": str,
-        "VersionCreatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DiscovererSummaryTypeDef = TypedDict(
     "DiscovererSummaryTypeDef",
     {
         "DiscovererArn": str,
         "DiscovererId": str,
         "SourceArn": str,
         "State": DiscovererStateType,
         "CrossAccount": bool,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredExportSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredExportSchemaRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
         "Type": str,
     },
@@ -395,26 +307,14 @@
 )
 
 class ExportSchemaRequestRequestTypeDef(
     _RequiredExportSchemaRequestRequestTypeDef, _OptionalExportSchemaRequestRequestTypeDef
 ):
     pass
 
-ExportSchemaResponseTypeDef = TypedDict(
-    "ExportSchemaResponseTypeDef",
-    {
-        "Content": str,
-        "SchemaArn": str,
-        "SchemaName": str,
-        "SchemaVersion": str,
-        "Type": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetCodeBindingSourceRequestRequestTypeDef = TypedDict(
     "_RequiredGetCodeBindingSourceRequestRequestTypeDef",
     {
         "Language": str,
         "RegistryName": str,
         "SchemaName": str,
     },
@@ -429,61 +329,36 @@
 
 class GetCodeBindingSourceRequestRequestTypeDef(
     _RequiredGetCodeBindingSourceRequestRequestTypeDef,
     _OptionalGetCodeBindingSourceRequestRequestTypeDef,
 ):
     pass
 
-GetCodeBindingSourceResponseTypeDef = TypedDict(
-    "GetCodeBindingSourceResponseTypeDef",
-    {
-        "Body": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDiscoveredSchemaRequestRequestTypeDef = TypedDict(
     "GetDiscoveredSchemaRequestRequestTypeDef",
     {
         "Events": Sequence[str],
         "Type": TypeType,
     },
 )
 
-GetDiscoveredSchemaResponseTypeDef = TypedDict(
-    "GetDiscoveredSchemaResponseTypeDef",
-    {
-        "Content": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
     total=False,
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "RevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDiscoverersRequestListDiscoverersPaginateTypeDef = TypedDict(
-    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "DiscovererIdPrefix": str,
-        "SourceArnPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListDiscoverersRequestRequestTypeDef = TypedDict(
     "ListDiscoverersRequestRequestTypeDef",
     {
@@ -491,24 +366,14 @@
         "Limit": int,
         "NextToken": str,
         "SourceArnPrefix": str,
     },
     total=False,
 )
 
-ListRegistriesRequestListRegistriesPaginateTypeDef = TypedDict(
-    "ListRegistriesRequestListRegistriesPaginateTypeDef",
-    {
-        "RegistryNamePrefix": str,
-        "Scope": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRegistriesRequestRequestTypeDef = TypedDict(
     "ListRegistriesRequestRequestTypeDef",
     {
         "Limit": int,
         "NextToken": str,
         "RegistryNamePrefix": str,
         "Scope": str,
@@ -522,35 +387,14 @@
         "RegistryArn": str,
         "RegistryName": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
-    {
-        "RegistryName": str,
-        "SchemaName": str,
-    },
-)
-_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef(
-    _RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
-    _OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListSchemaVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemaVersionsRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
     },
 )
@@ -576,35 +420,14 @@
         "SchemaName": str,
         "SchemaVersion": str,
         "Type": TypeType,
     },
     total=False,
 )
 
-_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "RegistryName": str,
-    },
-)
-_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "SchemaNamePrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSchemasRequestListSchemasPaginateTypeDef(
-    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
-    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
-):
-    pass
-
 _RequiredListSchemasRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemasRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
 )
 _OptionalListSchemasRequestRequestTypeDef = TypedDict(
@@ -637,32 +460,14 @@
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
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 _RequiredPutCodeBindingRequestRequestTypeDef = TypedDict(
     "_RequiredPutCodeBindingRequestRequestTypeDef",
     {
         "Language": str,
         "RegistryName": str,
         "SchemaName": str,
     },
@@ -676,25 +481,14 @@
 )
 
 class PutCodeBindingRequestRequestTypeDef(
     _RequiredPutCodeBindingRequestRequestTypeDef, _OptionalPutCodeBindingRequestRequestTypeDef
 ):
     pass
 
-PutCodeBindingResponseTypeDef = TypedDict(
-    "PutCodeBindingResponseTypeDef",
-    {
-        "CreationDate": datetime,
-        "LastModified": datetime,
-        "SchemaVersion": str,
-        "Status": CodeGenerationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourcePolicyRequestRequestTypeDef",
     {
         "Policy": str,
     },
 )
 _OptionalPutResourcePolicyRequestRequestTypeDef = TypedDict(
@@ -707,34 +501,14 @@
 )
 
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "RevisionId": str,
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
 SearchSchemaVersionSummaryTypeDef = TypedDict(
     "SearchSchemaVersionSummaryTypeDef",
     {
         "CreatedDate": datetime,
         "SchemaVersion": str,
         "Type": TypeType,
     },
@@ -758,67 +532,28 @@
 )
 
 class SearchSchemasRequestRequestTypeDef(
     _RequiredSearchSchemasRequestRequestTypeDef, _OptionalSearchSchemasRequestRequestTypeDef
 ):
     pass
 
-_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
-    "_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef",
-    {
-        "Keywords": str,
-        "RegistryName": str,
-    },
-)
-_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
-    "_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class SearchSchemasRequestSearchSchemasPaginateTypeDef(
-    _RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef,
-    _OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef,
-):
-    pass
-
 StartDiscovererRequestRequestTypeDef = TypedDict(
     "StartDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
-StartDiscovererResponseTypeDef = TypedDict(
-    "StartDiscovererResponseTypeDef",
-    {
-        "DiscovererId": str,
-        "State": DiscovererStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopDiscovererRequestRequestTypeDef = TypedDict(
     "StopDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
-StopDiscovererResponseTypeDef = TypedDict(
-    "StopDiscovererResponseTypeDef",
-    {
-        "DiscovererId": str,
-        "State": DiscovererStateType,
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
@@ -847,28 +582,14 @@
 )
 
 class UpdateDiscovererRequestRequestTypeDef(
     _RequiredUpdateDiscovererRequestRequestTypeDef, _OptionalUpdateDiscovererRequestRequestTypeDef
 ):
     pass
 
-UpdateDiscovererResponseTypeDef = TypedDict(
-    "UpdateDiscovererResponseTypeDef",
-    {
-        "Description": str,
-        "DiscovererArn": str,
-        "DiscovererId": str,
-        "SourceArn": str,
-        "State": DiscovererStateType,
-        "CrossAccount": bool,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateRegistryRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRegistryRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
 )
 _OptionalUpdateRegistryRequestRequestTypeDef = TypedDict(
@@ -880,25 +601,14 @@
 )
 
 class UpdateRegistryRequestRequestTypeDef(
     _RequiredUpdateRegistryRequestRequestTypeDef, _OptionalUpdateRegistryRequestRequestTypeDef
 ):
     pass
 
-UpdateRegistryResponseTypeDef = TypedDict(
-    "UpdateRegistryResponseTypeDef",
-    {
-        "Description": str,
-        "RegistryArn": str,
-        "RegistryName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSchemaRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
     },
 )
@@ -914,26 +624,233 @@
 )
 
 class UpdateSchemaRequestRequestTypeDef(
     _RequiredUpdateSchemaRequestRequestTypeDef, _OptionalUpdateSchemaRequestRequestTypeDef
 ):
     pass
 
+CreateDiscovererResponseTypeDef = TypedDict(
+    "CreateDiscovererResponseTypeDef",
+    {
+        "Description": str,
+        "DiscovererArn": str,
+        "DiscovererId": str,
+        "SourceArn": str,
+        "State": DiscovererStateType,
+        "CrossAccount": bool,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRegistryResponseTypeDef = TypedDict(
+    "CreateRegistryResponseTypeDef",
+    {
+        "Description": str,
+        "RegistryArn": str,
+        "RegistryName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSchemaResponseTypeDef = TypedDict(
+    "CreateSchemaResponseTypeDef",
+    {
+        "Description": str,
+        "LastModified": datetime,
+        "SchemaArn": str,
+        "SchemaName": str,
+        "SchemaVersion": str,
+        "Tags": Dict[str, str],
+        "Type": str,
+        "VersionCreatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCodeBindingResponseTypeDef = TypedDict(
+    "DescribeCodeBindingResponseTypeDef",
+    {
+        "CreationDate": datetime,
+        "LastModified": datetime,
+        "SchemaVersion": str,
+        "Status": CodeGenerationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDiscovererResponseTypeDef = TypedDict(
+    "DescribeDiscovererResponseTypeDef",
+    {
+        "Description": str,
+        "DiscovererArn": str,
+        "DiscovererId": str,
+        "SourceArn": str,
+        "State": DiscovererStateType,
+        "CrossAccount": bool,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRegistryResponseTypeDef = TypedDict(
+    "DescribeRegistryResponseTypeDef",
+    {
+        "Description": str,
+        "RegistryArn": str,
+        "RegistryName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeSchemaResponseTypeDef = TypedDict(
+    "DescribeSchemaResponseTypeDef",
+    {
+        "Content": str,
+        "Description": str,
+        "LastModified": datetime,
+        "SchemaArn": str,
+        "SchemaName": str,
+        "SchemaVersion": str,
+        "Tags": Dict[str, str],
+        "Type": str,
+        "VersionCreatedDate": datetime,
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
+ExportSchemaResponseTypeDef = TypedDict(
+    "ExportSchemaResponseTypeDef",
+    {
+        "Content": str,
+        "SchemaArn": str,
+        "SchemaName": str,
+        "SchemaVersion": str,
+        "Type": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCodeBindingSourceResponseTypeDef = TypedDict(
+    "GetCodeBindingSourceResponseTypeDef",
+    {
+        "Body": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDiscoveredSchemaResponseTypeDef = TypedDict(
+    "GetDiscoveredSchemaResponseTypeDef",
+    {
+        "Content": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "RevisionId": str,
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
+PutCodeBindingResponseTypeDef = TypedDict(
+    "PutCodeBindingResponseTypeDef",
+    {
+        "CreationDate": datetime,
+        "LastModified": datetime,
+        "SchemaVersion": str,
+        "Status": CodeGenerationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "RevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDiscovererResponseTypeDef = TypedDict(
+    "StartDiscovererResponseTypeDef",
+    {
+        "DiscovererId": str,
+        "State": DiscovererStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopDiscovererResponseTypeDef = TypedDict(
+    "StopDiscovererResponseTypeDef",
+    {
+        "DiscovererId": str,
+        "State": DiscovererStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDiscovererResponseTypeDef = TypedDict(
+    "UpdateDiscovererResponseTypeDef",
+    {
+        "Description": str,
+        "DiscovererArn": str,
+        "DiscovererId": str,
+        "SourceArn": str,
+        "State": DiscovererStateType,
+        "CrossAccount": bool,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRegistryResponseTypeDef = TypedDict(
+    "UpdateRegistryResponseTypeDef",
+    {
+        "Description": str,
+        "RegistryArn": str,
+        "RegistryName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateSchemaResponseTypeDef = TypedDict(
     "UpdateSchemaResponseTypeDef",
     {
         "Description": str,
         "LastModified": datetime,
         "SchemaArn": str,
         "SchemaName": str,
         "SchemaVersion": str,
         "Tags": Dict[str, str],
         "Type": str,
         "VersionCreatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeCodeBindingRequestCodeBindingExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeCodeBindingRequestCodeBindingExistsWaitTypeDef",
     {
         "Language": str,
@@ -957,42 +874,125 @@
     pass
 
 ListDiscoverersResponseTypeDef = TypedDict(
     "ListDiscoverersResponseTypeDef",
     {
         "Discoverers": List[DiscovererSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDiscoverersRequestListDiscoverersPaginateTypeDef = TypedDict(
+    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
+    {
+        "DiscovererIdPrefix": str,
+        "SourceArnPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRegistriesRequestListRegistriesPaginateTypeDef = TypedDict(
+    "ListRegistriesRequestListRegistriesPaginateTypeDef",
+    {
+        "RegistryNamePrefix": str,
+        "Scope": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
+    {
+        "RegistryName": str,
+        "SchemaName": str,
+    },
+)
+_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef(
+    _RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
+    _OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "RegistryName": str,
+    },
+)
+_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "SchemaNamePrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSchemasRequestListSchemasPaginateTypeDef(
+    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
+    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
+):
+    pass
+
+_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
+    "_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef",
+    {
+        "Keywords": str,
+        "RegistryName": str,
     },
 )
+_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
+    "_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class SearchSchemasRequestSearchSchemasPaginateTypeDef(
+    _RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef,
+    _OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef,
+):
+    pass
 
 ListRegistriesResponseTypeDef = TypedDict(
     "ListRegistriesResponseTypeDef",
     {
         "NextToken": str,
         "Registries": List[RegistrySummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSchemaVersionsResponseTypeDef = TypedDict(
     "ListSchemaVersionsResponseTypeDef",
     {
         "NextToken": str,
         "SchemaVersions": List[SchemaVersionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSchemasResponseTypeDef = TypedDict(
     "ListSchemasResponseTypeDef",
     {
         "NextToken": str,
         "Schemas": List[SchemaSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchSchemaSummaryTypeDef = TypedDict(
     "SearchSchemaSummaryTypeDef",
     {
         "RegistryName": str,
@@ -1004,10 +1004,10 @@
 )
 
 SearchSchemasResponseTypeDef = TypedDict(
     "SearchSchemasResponseTypeDef",
     {
         "NextToken": str,
         "Schemas": List[SearchSchemaSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/waiter.py` & `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/waiter.pyi` & `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas.egg-info/PKG-INFO` & `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-schemas
-Version: 1.28.0
-Summary: Type annotations for boto3.Schemas 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Schemas 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-schemas"></a>
 
 # mypy-boto3-schemas
 
 [![PyPI - mypy-boto3-schemas](https://img.shields.io/pypi/v/mypy-boto3-schemas.svg?color=blue)](https://pypi.org/project/mypy-boto3-schemas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-schemas.svg?color=blue)](https://pypi.org/project/mypy-boto3-schemas)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-schemas?color=blue)](https://pypistats.org/packages/mypy-boto3-schemas)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-schemas)](https://pepy.tech/project/mypy-boto3-schemas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Schemas 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
+[boto3.Schemas 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
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
 [mypy-boto3-schemas docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/).
 
 See how it helps to find and fix potential bugs:
 
@@ -360,79 +360,79 @@
 
 `mypy_boto3_schemas.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_schemas.type_defs import (
     CreateDiscovererRequestRequestTypeDef,
-    CreateDiscovererResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateRegistryRequestRequestTypeDef,
-    CreateRegistryResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
-    CreateSchemaResponseTypeDef,
     DeleteDiscovererRequestRequestTypeDef,
     DeleteRegistryRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSchemaRequestRequestTypeDef,
     DeleteSchemaVersionRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCodeBindingRequestRequestTypeDef,
-    DescribeCodeBindingResponseTypeDef,
     DescribeDiscovererRequestRequestTypeDef,
-    DescribeDiscovererResponseTypeDef,
     DescribeRegistryRequestRequestTypeDef,
-    DescribeRegistryResponseTypeDef,
     DescribeSchemaRequestRequestTypeDef,
-    DescribeSchemaResponseTypeDef,
     DiscovererSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportSchemaRequestRequestTypeDef,
-    ExportSchemaResponseTypeDef,
     GetCodeBindingSourceRequestRequestTypeDef,
-    GetCodeBindingSourceResponseTypeDef,
     GetDiscoveredSchemaRequestRequestTypeDef,
-    GetDiscoveredSchemaResponseTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    ListDiscoverersRequestListDiscoverersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDiscoverersRequestRequestTypeDef,
-    ListRegistriesRequestListRegistriesPaginateTypeDef,
     ListRegistriesRequestRequestTypeDef,
     RegistrySummaryTypeDef,
-    ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
     ListSchemaVersionsRequestRequestTypeDef,
     SchemaVersionSummaryTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
     SchemaSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutCodeBindingRequestRequestTypeDef,
-    PutCodeBindingResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    ResponseMetadataTypeDef,
     SearchSchemaVersionSummaryTypeDef,
     SearchSchemasRequestRequestTypeDef,
-    SearchSchemasRequestSearchSchemasPaginateTypeDef,
     StartDiscovererRequestRequestTypeDef,
-    StartDiscovererResponseTypeDef,
     StopDiscovererRequestRequestTypeDef,
-    StopDiscovererResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDiscovererRequestRequestTypeDef,
-    UpdateDiscovererResponseTypeDef,
     UpdateRegistryRequestRequestTypeDef,
-    UpdateRegistryResponseTypeDef,
     UpdateSchemaRequestRequestTypeDef,
+    CreateDiscovererResponseTypeDef,
+    CreateRegistryResponseTypeDef,
+    CreateSchemaResponseTypeDef,
+    DescribeCodeBindingResponseTypeDef,
+    DescribeDiscovererResponseTypeDef,
+    DescribeRegistryResponseTypeDef,
+    DescribeSchemaResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportSchemaResponseTypeDef,
+    GetCodeBindingSourceResponseTypeDef,
+    GetDiscoveredSchemaResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutCodeBindingResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    StartDiscovererResponseTypeDef,
+    StopDiscovererResponseTypeDef,
+    UpdateDiscovererResponseTypeDef,
+    UpdateRegistryResponseTypeDef,
     UpdateSchemaResponseTypeDef,
     DescribeCodeBindingRequestCodeBindingExistsWaitTypeDef,
     ListDiscoverersResponseTypeDef,
+    ListDiscoverersRequestListDiscoverersPaginateTypeDef,
+    ListRegistriesRequestListRegistriesPaginateTypeDef,
+    ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
+    ListSchemasRequestListSchemasPaginateTypeDef,
+    SearchSchemasRequestSearchSchemasPaginateTypeDef,
     ListRegistriesResponseTypeDef,
     ListSchemaVersionsResponseTypeDef,
     ListSchemasResponseTypeDef,
     SearchSchemaSummaryTypeDef,
     SearchSchemasResponseTypeDef,
 )
```

### Comparing `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas.egg-info/SOURCES.txt` & `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.0/setup.py` & `mypy-boto3-schemas-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-schemas",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_schemas"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Schemas 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Schemas 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

