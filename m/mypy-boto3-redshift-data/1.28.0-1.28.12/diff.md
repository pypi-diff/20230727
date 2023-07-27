# Comparing `tmp/mypy-boto3-redshift-data-1.28.0.tar.gz` & `tmp/mypy-boto3-redshift-data-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-redshift-data-1.28.0.tar", last modified: Thu Jul  6 21:00:25 2023, max compression
+gzip compressed data, was "mypy-boto3-redshift-data-1.28.12.tar", last modified: Thu Jul 27 11:49:27 2023, max compression
```

## Comparing `mypy-boto3-redshift-data-1.28.0.tar` & `mypy-boto3-redshift-data-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:25.078405 mypy-boto3-redshift-data-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:52:58.000000 mypy-boto3-redshift-data-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15032 2023-07-06 21:00:25.070405 mypy-boto3-redshift-data-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-07-06 20:52:58.000000 mypy-boto3-redshift-data-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:25.062405 mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-06 20:52:58.000000 mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-06 20:52:58.000000 mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-06 20:52:58.000000 mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-07-06 20:52:58.000000 mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-07-06 20:52:58.000000 mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-06 20:52:58.000000 mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-07-06 20:52:58.000000 mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-07-06 20:52:58.000000 mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-07-06 20:52:58.000000 mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:52:58.000000 mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16716 2023-07-06 20:52:59.000000 mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16687 2023-07-06 20:52:58.000000 mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:52:58.000000 mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:25.070405 mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15032 2023-07-06 21:00:24.000000 mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-06 21:00:24.000000 mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:24.000000 mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:24.000000 mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:24.000000 mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 21:00:24.000000 mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:25.078405 mypy-boto3-redshift-data-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-06 20:52:57.000000 mypy-boto3-redshift-data-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.701189 mypy-boto3-redshift-data-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15050 2023-07-27 11:49:27.697189 mypy-boto3-redshift-data-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.697189 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16860 2023-07-27 11:44:25.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16831 2023-07-27 11:44:25.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.697189 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15050 2023-07-27 11:49:27.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 11:49:27.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:27.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 11:49:27.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:27.701189 mypy-boto3-redshift-data-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/setup.py
```

### Comparing `mypy-boto3-redshift-data-1.28.0/LICENSE` & `mypy-boto3-redshift-data-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.28.0/PKG-INFO` & `mypy-boto3-redshift-data-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift-data
-Version: 1.28.0
-Summary: Type annotations for boto3.RedshiftDataAPIService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.RedshiftDataAPIService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-redshift-data"></a>
 
 # mypy-boto3-redshift-data
 
 [![PyPI - mypy-boto3-redshift-data](https://img.shields.io/pypi/v/mypy-boto3-redshift-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift-data?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift-data)](https://pepy.tech/project/mypy-boto3-redshift-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftDataAPIService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
+[boto3.RedshiftDataAPIService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
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
 [mypy-boto3-redshift-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -341,44 +341,45 @@
 
 `mypy_boto3_redshift_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_redshift_data.type_defs import (
     BatchExecuteStatementInputRequestTypeDef,
-    BatchExecuteStatementOutputTypeDef,
+    ResponseMetadataTypeDef,
     CancelStatementRequestRequestTypeDef,
-    CancelStatementResponseTypeDef,
     ColumnMetadataTypeDef,
     DescribeStatementRequestRequestTypeDef,
-    SqlParameterTypeDef,
+    SqlParameterOutputTypeDef,
     SubStatementDataTypeDef,
-    DescribeTableRequestDescribeTablePaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeTableRequestRequestTypeDef,
-    ExecuteStatementOutputTypeDef,
+    SqlParameterTypeDef,
     FieldTypeDef,
-    GetStatementResultRequestGetStatementResultPaginateTypeDef,
     GetStatementResultRequestRequestTypeDef,
-    ListDatabasesRequestListDatabasesPaginateTypeDef,
     ListDatabasesRequestRequestTypeDef,
-    ListDatabasesResponseTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
-    ListSchemasResponseTypeDef,
-    ListStatementsRequestListStatementsPaginateTypeDef,
     ListStatementsRequestRequestTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableMemberTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    BatchExecuteStatementOutputTypeDef,
+    CancelStatementResponseTypeDef,
+    ExecuteStatementOutputTypeDef,
+    ListDatabasesResponseTypeDef,
+    ListSchemasResponseTypeDef,
     DescribeTableResponseTypeDef,
-    ExecuteStatementInputRequestTypeDef,
     StatementDataTypeDef,
     DescribeStatementResponseTypeDef,
+    DescribeTableRequestDescribeTablePaginateTypeDef,
+    GetStatementResultRequestGetStatementResultPaginateTypeDef,
+    ListDatabasesRequestListDatabasesPaginateTypeDef,
+    ListSchemasRequestListSchemasPaginateTypeDef,
+    ListStatementsRequestListStatementsPaginateTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
+    ExecuteStatementInputRequestTypeDef,
     GetStatementResultResponseTypeDef,
     ListTablesResponseTypeDef,
     ListStatementsResponseTypeDef,
 )
 
 
 def get_structure() -> BatchExecuteStatementInputRequestTypeDef:
```

### Comparing `mypy-boto3-redshift-data-1.28.0/README.md` & `mypy-boto3-redshift-data-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-redshift-data"></a>
 
 # mypy-boto3-redshift-data
 
 [![PyPI - mypy-boto3-redshift-data](https://img.shields.io/pypi/v/mypy-boto3-redshift-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift-data?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift-data)](https://pepy.tech/project/mypy-boto3-redshift-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftDataAPIService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
+[boto3.RedshiftDataAPIService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
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
 [mypy-boto3-redshift-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -309,44 +309,45 @@
 
 `mypy_boto3_redshift_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_redshift_data.type_defs import (
     BatchExecuteStatementInputRequestTypeDef,
-    BatchExecuteStatementOutputTypeDef,
+    ResponseMetadataTypeDef,
     CancelStatementRequestRequestTypeDef,
-    CancelStatementResponseTypeDef,
     ColumnMetadataTypeDef,
     DescribeStatementRequestRequestTypeDef,
-    SqlParameterTypeDef,
+    SqlParameterOutputTypeDef,
     SubStatementDataTypeDef,
-    DescribeTableRequestDescribeTablePaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeTableRequestRequestTypeDef,
-    ExecuteStatementOutputTypeDef,
+    SqlParameterTypeDef,
     FieldTypeDef,
-    GetStatementResultRequestGetStatementResultPaginateTypeDef,
     GetStatementResultRequestRequestTypeDef,
-    ListDatabasesRequestListDatabasesPaginateTypeDef,
     ListDatabasesRequestRequestTypeDef,
-    ListDatabasesResponseTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
-    ListSchemasResponseTypeDef,
-    ListStatementsRequestListStatementsPaginateTypeDef,
     ListStatementsRequestRequestTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableMemberTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    BatchExecuteStatementOutputTypeDef,
+    CancelStatementResponseTypeDef,
+    ExecuteStatementOutputTypeDef,
+    ListDatabasesResponseTypeDef,
+    ListSchemasResponseTypeDef,
     DescribeTableResponseTypeDef,
-    ExecuteStatementInputRequestTypeDef,
     StatementDataTypeDef,
     DescribeStatementResponseTypeDef,
+    DescribeTableRequestDescribeTablePaginateTypeDef,
+    GetStatementResultRequestGetStatementResultPaginateTypeDef,
+    ListDatabasesRequestListDatabasesPaginateTypeDef,
+    ListSchemasRequestListSchemasPaginateTypeDef,
+    ListStatementsRequestListStatementsPaginateTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
+    ExecuteStatementInputRequestTypeDef,
     GetStatementResultResponseTypeDef,
     ListTablesResponseTypeDef,
     ListStatementsResponseTypeDef,
 )
 
 
 def get_structure() -> BatchExecuteStatementInputRequestTypeDef:
```

### Comparing `mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/__init__.py` & `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/__init__.pyi` & `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/__main__.py` & `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RedshiftDataAPIService 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.RedshiftDataAPIService 1.28.12\nVersion:        "
+        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService\nOther"
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

### Comparing `mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/client.py` & `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/client.pyi` & `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/literals.py` & `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/literals.py`

 * *Files 1% similar despite different names*

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

### Comparing `mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/literals.pyi` & `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,15 @@
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
@@ -245,26 +246,28 @@
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

### Comparing `mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/paginator.py` & `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -49,25 +49,22 @@
     "GetStatementResultPaginator",
     "ListDatabasesPaginator",
     "ListSchemasPaginator",
     "ListStatementsPaginator",
     "ListTablesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeTablePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.DescribeTable)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#describetablepaginator)
     """
 
     def paginate(
@@ -77,59 +74,56 @@
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         Schema: str = ...,
         SecretArn: str = ...,
         Table: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeTableResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.DescribeTable.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#describetablepaginator)
         """
 
-
 class GetStatementResultPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.GetStatementResult)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#getstatementresultpaginator)
     """
 
     def paginate(
-        self, *, Id: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Id: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetStatementResultResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.GetStatementResult.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#getstatementresultpaginator)
         """
 
-
 class ListDatabasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListDatabases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#listdatabasespaginator)
     """
 
     def paginate(
         self,
         *,
         Database: str,
         ClusterIdentifier: str = ...,
         DbUser: str = ...,
         SecretArn: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatabasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListDatabases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#listdatabasespaginator)
         """
 
-
 class ListSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#listschemaspaginator)
     """
 
     def paginate(
@@ -138,42 +132,40 @@
         Database: str,
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         SchemaPattern: str = ...,
         SecretArn: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#listschemaspaginator)
         """
 
-
 class ListStatementsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListStatements)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#liststatementspaginator)
     """
 
     def paginate(
         self,
         *,
         RoleLevel: bool = ...,
         StatementName: str = ...,
         Status: StatusStringType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStatementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListStatements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#liststatementspaginator)
         """
 
-
 class ListTablesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListTables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#listtablespaginator)
     """
 
     def paginate(
@@ -183,13 +175,13 @@
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         SchemaPattern: str = ...,
         SecretArn: str = ...,
         TablePattern: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTablesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#listtablespaginator)
         """
```

### Comparing `mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/paginator.pyi` & `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,22 +49,25 @@
     "GetStatementResultPaginator",
     "ListDatabasesPaginator",
     "ListSchemasPaginator",
     "ListStatementsPaginator",
     "ListTablesPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeTablePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.DescribeTable)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#describetablepaginator)
     """
 
     def paginate(
@@ -74,56 +77,59 @@
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         Schema: str = ...,
         SecretArn: str = ...,
         Table: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeTableResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.DescribeTable.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#describetablepaginator)
         """
 
+
 class GetStatementResultPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.GetStatementResult)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#getstatementresultpaginator)
     """
 
     def paginate(
-        self, *, Id: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Id: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetStatementResultResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.GetStatementResult.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#getstatementresultpaginator)
         """
 
+
 class ListDatabasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListDatabases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#listdatabasespaginator)
     """
 
     def paginate(
         self,
         *,
         Database: str,
         ClusterIdentifier: str = ...,
         DbUser: str = ...,
         SecretArn: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatabasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListDatabases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#listdatabasespaginator)
         """
 
+
 class ListSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#listschemaspaginator)
     """
 
     def paginate(
@@ -132,40 +138,42 @@
         Database: str,
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         SchemaPattern: str = ...,
         SecretArn: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#listschemaspaginator)
         """
 
+
 class ListStatementsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListStatements)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#liststatementspaginator)
     """
 
     def paginate(
         self,
         *,
         RoleLevel: bool = ...,
         StatementName: str = ...,
         Status: StatusStringType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStatementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListStatements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#liststatementspaginator)
         """
 
+
 class ListTablesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListTables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#listtablespaginator)
     """
 
     def paginate(
@@ -175,13 +183,13 @@
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         SchemaPattern: str = ...,
         SecretArn: str = ...,
         TablePattern: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTablesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/paginators/#listtablespaginator)
         """
```

### Comparing `mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/type_defs.py` & `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -18,47 +18,47 @@
 from .literals import StatementStatusStringType, StatusStringType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BatchExecuteStatementInputRequestTypeDef",
-    "BatchExecuteStatementOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CancelStatementRequestRequestTypeDef",
-    "CancelStatementResponseTypeDef",
     "ColumnMetadataTypeDef",
     "DescribeStatementRequestRequestTypeDef",
-    "SqlParameterTypeDef",
+    "SqlParameterOutputTypeDef",
     "SubStatementDataTypeDef",
-    "DescribeTableRequestDescribeTablePaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeTableRequestRequestTypeDef",
-    "ExecuteStatementOutputTypeDef",
+    "SqlParameterTypeDef",
     "FieldTypeDef",
-    "GetStatementResultRequestGetStatementResultPaginateTypeDef",
     "GetStatementResultRequestRequestTypeDef",
-    "ListDatabasesRequestListDatabasesPaginateTypeDef",
     "ListDatabasesRequestRequestTypeDef",
-    "ListDatabasesResponseTypeDef",
-    "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSchemasRequestRequestTypeDef",
-    "ListSchemasResponseTypeDef",
-    "ListStatementsRequestListStatementsPaginateTypeDef",
     "ListStatementsRequestRequestTypeDef",
-    "ListTablesRequestListTablesPaginateTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableMemberTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "BatchExecuteStatementOutputTypeDef",
+    "CancelStatementResponseTypeDef",
+    "ExecuteStatementOutputTypeDef",
+    "ListDatabasesResponseTypeDef",
+    "ListSchemasResponseTypeDef",
     "DescribeTableResponseTypeDef",
-    "ExecuteStatementInputRequestTypeDef",
     "StatementDataTypeDef",
     "DescribeStatementResponseTypeDef",
+    "DescribeTableRequestDescribeTablePaginateTypeDef",
+    "GetStatementResultRequestGetStatementResultPaginateTypeDef",
+    "ListDatabasesRequestListDatabasesPaginateTypeDef",
+    "ListSchemasRequestListSchemasPaginateTypeDef",
+    "ListStatementsRequestListStatementsPaginateTypeDef",
+    "ListTablesRequestListTablesPaginateTypeDef",
+    "ExecuteStatementInputRequestTypeDef",
     "GetStatementResultResponseTypeDef",
     "ListTablesResponseTypeDef",
     "ListStatementsResponseTypeDef",
 )
 
 _RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementInputRequestTypeDef",
@@ -77,51 +77,38 @@
         "StatementName": str,
         "WithEvent": bool,
         "WorkgroupName": str,
     },
     total=False,
 )
 
-
 class BatchExecuteStatementInputRequestTypeDef(
     _RequiredBatchExecuteStatementInputRequestTypeDef,
     _OptionalBatchExecuteStatementInputRequestTypeDef,
 ):
     pass
 
-
-BatchExecuteStatementOutputTypeDef = TypedDict(
-    "BatchExecuteStatementOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ClusterIdentifier": str,
-        "CreatedAt": datetime,
-        "Database": str,
-        "DbUser": str,
-        "Id": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CancelStatementRequestRequestTypeDef = TypedDict(
     "CancelStatementRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-CancelStatementResponseTypeDef = TypedDict(
-    "CancelStatementResponseTypeDef",
-    {
-        "Status": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ColumnMetadataTypeDef = TypedDict(
     "ColumnMetadataTypeDef",
     {
         "columnDefault": str,
         "isCaseSensitive": bool,
         "isCurrency": bool,
         "isSigned": bool,
@@ -141,16 +128,16 @@
 DescribeStatementRequestRequestTypeDef = TypedDict(
     "DescribeStatementRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-SqlParameterTypeDef = TypedDict(
-    "SqlParameterTypeDef",
+SqlParameterOutputTypeDef = TypedDict(
+    "SqlParameterOutputTypeDef",
     {
         "name": str,
         "value": str,
     },
 )
 
 _RequiredSubStatementDataTypeDef = TypedDict(
@@ -172,48 +159,27 @@
         "ResultSize": int,
         "Status": StatementStatusStringType,
         "UpdatedAt": datetime,
     },
     total=False,
 )
 
-
 class SubStatementDataTypeDef(_RequiredSubStatementDataTypeDef, _OptionalSubStatementDataTypeDef):
     pass
 
-
-_RequiredDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
-    "_RequiredDescribeTableRequestDescribeTablePaginateTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
-    "_OptionalDescribeTableRequestDescribeTablePaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ClusterIdentifier": str,
-        "ConnectedDatabase": str,
-        "DbUser": str,
-        "Schema": str,
-        "SecretArn": str,
-        "Table": str,
-        "WorkgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class DescribeTableRequestDescribeTablePaginateTypeDef(
-    _RequiredDescribeTableRequestDescribeTablePaginateTypeDef,
-    _OptionalDescribeTableRequestDescribeTablePaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeTableRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTableRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
 _OptionalDescribeTableRequestRequestTypeDef = TypedDict(
@@ -228,32 +194,24 @@
         "SecretArn": str,
         "Table": str,
         "WorkgroupName": str,
     },
     total=False,
 )
 
-
 class DescribeTableRequestRequestTypeDef(
     _RequiredDescribeTableRequestRequestTypeDef, _OptionalDescribeTableRequestRequestTypeDef
 ):
     pass
 
-
-ExecuteStatementOutputTypeDef = TypedDict(
-    "ExecuteStatementOutputTypeDef",
+SqlParameterTypeDef = TypedDict(
+    "SqlParameterTypeDef",
     {
-        "ClusterIdentifier": str,
-        "CreatedAt": datetime,
-        "Database": str,
-        "DbUser": str,
-        "Id": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "value": str,
     },
 )
 
 FieldTypeDef = TypedDict(
     "FieldTypeDef",
     {
         "blobValue": bytes,
@@ -262,306 +220,383 @@
         "isNull": bool,
         "longValue": int,
         "stringValue": str,
     },
     total=False,
 )
 
-_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
-    "_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
-    "_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetStatementResultRequestGetStatementResultPaginateTypeDef(
-    _RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef,
-    _OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetStatementResultRequestRequestTypeDef = TypedDict(
     "_RequiredGetStatementResultRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalGetStatementResultRequestRequestTypeDef = TypedDict(
     "_OptionalGetStatementResultRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetStatementResultRequestRequestTypeDef(
     _RequiredGetStatementResultRequestRequestTypeDef,
     _OptionalGetStatementResultRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
-    "_RequiredListDatabasesRequestListDatabasesPaginateTypeDef",
+_RequiredListDatabasesRequestRequestTypeDef = TypedDict(
+    "_RequiredListDatabasesRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
-_OptionalListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
-    "_OptionalListDatabasesRequestListDatabasesPaginateTypeDef",
+_OptionalListDatabasesRequestRequestTypeDef = TypedDict(
+    "_OptionalListDatabasesRequestRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "DbUser": str,
+        "MaxResults": int,
+        "NextToken": str,
         "SecretArn": str,
         "WorkgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
-class ListDatabasesRequestListDatabasesPaginateTypeDef(
-    _RequiredListDatabasesRequestListDatabasesPaginateTypeDef,
-    _OptionalListDatabasesRequestListDatabasesPaginateTypeDef,
+class ListDatabasesRequestRequestTypeDef(
+    _RequiredListDatabasesRequestRequestTypeDef, _OptionalListDatabasesRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredListDatabasesRequestRequestTypeDef = TypedDict(
-    "_RequiredListDatabasesRequestRequestTypeDef",
+_RequiredListSchemasRequestRequestTypeDef = TypedDict(
+    "_RequiredListSchemasRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
-_OptionalListDatabasesRequestRequestTypeDef = TypedDict(
-    "_OptionalListDatabasesRequestRequestTypeDef",
+_OptionalListSchemasRequestRequestTypeDef = TypedDict(
+    "_OptionalListSchemasRequestRequestTypeDef",
     {
         "ClusterIdentifier": str,
+        "ConnectedDatabase": str,
         "DbUser": str,
         "MaxResults": int,
         "NextToken": str,
+        "SchemaPattern": str,
         "SecretArn": str,
         "WorkgroupName": str,
     },
     total=False,
 )
 
-
-class ListDatabasesRequestRequestTypeDef(
-    _RequiredListDatabasesRequestRequestTypeDef, _OptionalListDatabasesRequestRequestTypeDef
+class ListSchemasRequestRequestTypeDef(
+    _RequiredListSchemasRequestRequestTypeDef, _OptionalListSchemasRequestRequestTypeDef
 ):
     pass
 
-
-ListDatabasesResponseTypeDef = TypedDict(
-    "ListDatabasesResponseTypeDef",
+ListStatementsRequestRequestTypeDef = TypedDict(
+    "ListStatementsRequestRequestTypeDef",
     {
-        "Databases": List[str],
+        "MaxResults": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RoleLevel": bool,
+        "StatementName": str,
+        "Status": StatusStringType,
     },
+    total=False,
 )
 
-_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
+_RequiredListTablesRequestRequestTypeDef = TypedDict(
+    "_RequiredListTablesRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
-_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
+_OptionalListTablesRequestRequestTypeDef = TypedDict(
+    "_OptionalListTablesRequestRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "ConnectedDatabase": str,
         "DbUser": str,
+        "MaxResults": int,
+        "NextToken": str,
         "SchemaPattern": str,
         "SecretArn": str,
+        "TablePattern": str,
         "WorkgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
-class ListSchemasRequestListSchemasPaginateTypeDef(
-    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
-    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
+class ListTablesRequestRequestTypeDef(
+    _RequiredListTablesRequestRequestTypeDef, _OptionalListTablesRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredListSchemasRequestRequestTypeDef = TypedDict(
-    "_RequiredListSchemasRequestRequestTypeDef",
+TableMemberTypeDef = TypedDict(
+    "TableMemberTypeDef",
     {
-        "Database": str,
+        "name": str,
+        "schema": str,
+        "type": str,
     },
+    total=False,
 )
-_OptionalListSchemasRequestRequestTypeDef = TypedDict(
-    "_OptionalListSchemasRequestRequestTypeDef",
+
+BatchExecuteStatementOutputTypeDef = TypedDict(
+    "BatchExecuteStatementOutputTypeDef",
     {
         "ClusterIdentifier": str,
-        "ConnectedDatabase": str,
+        "CreatedAt": datetime,
+        "Database": str,
         "DbUser": str,
-        "MaxResults": int,
-        "NextToken": str,
-        "SchemaPattern": str,
+        "Id": str,
         "SecretArn": str,
         "WorkgroupName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+CancelStatementResponseTypeDef = TypedDict(
+    "CancelStatementResponseTypeDef",
+    {
+        "Status": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ListSchemasRequestRequestTypeDef(
-    _RequiredListSchemasRequestRequestTypeDef, _OptionalListSchemasRequestRequestTypeDef
-):
-    pass
+ExecuteStatementOutputTypeDef = TypedDict(
+    "ExecuteStatementOutputTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "CreatedAt": datetime,
+        "Database": str,
+        "DbUser": str,
+        "Id": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+ListDatabasesResponseTypeDef = TypedDict(
+    "ListDatabasesResponseTypeDef",
+    {
+        "Databases": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ListSchemasResponseTypeDef = TypedDict(
     "ListSchemasResponseTypeDef",
     {
         "NextToken": str,
         "Schemas": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListStatementsRequestListStatementsPaginateTypeDef = TypedDict(
-    "ListStatementsRequestListStatementsPaginateTypeDef",
+DescribeTableResponseTypeDef = TypedDict(
+    "DescribeTableResponseTypeDef",
     {
-        "RoleLevel": bool,
+        "ColumnList": List[ColumnMetadataTypeDef],
+        "NextToken": str,
+        "TableName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredStatementDataTypeDef = TypedDict(
+    "_RequiredStatementDataTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalStatementDataTypeDef = TypedDict(
+    "_OptionalStatementDataTypeDef",
+    {
+        "CreatedAt": datetime,
+        "IsBatchStatement": bool,
+        "QueryParameters": List[SqlParameterOutputTypeDef],
+        "QueryString": str,
+        "QueryStrings": List[str],
+        "SecretArn": str,
         "StatementName": str,
         "Status": StatusStringType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "UpdatedAt": datetime,
     },
     total=False,
 )
 
-ListStatementsRequestRequestTypeDef = TypedDict(
-    "ListStatementsRequestRequestTypeDef",
+class StatementDataTypeDef(_RequiredStatementDataTypeDef, _OptionalStatementDataTypeDef):
+    pass
+
+DescribeStatementResponseTypeDef = TypedDict(
+    "DescribeStatementResponseTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
-        "RoleLevel": bool,
-        "StatementName": str,
+        "ClusterIdentifier": str,
+        "CreatedAt": datetime,
+        "Database": str,
+        "DbUser": str,
+        "Duration": int,
+        "Error": str,
+        "HasResultSet": bool,
+        "Id": str,
+        "QueryParameters": List[SqlParameterOutputTypeDef],
+        "QueryString": str,
+        "RedshiftPid": int,
+        "RedshiftQueryId": int,
+        "ResultRows": int,
+        "ResultSize": int,
+        "SecretArn": str,
         "Status": StatusStringType,
+        "SubStatements": List[SubStatementDataTypeDef],
+        "UpdatedAt": datetime,
+        "WorkgroupName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_RequiredListTablesRequestListTablesPaginateTypeDef",
+_RequiredDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
+    "_RequiredDescribeTableRequestDescribeTablePaginateTypeDef",
     {
         "Database": str,
     },
 )
-_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_OptionalListTablesRequestListTablesPaginateTypeDef",
+_OptionalDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
+    "_OptionalDescribeTableRequestDescribeTablePaginateTypeDef",
     {
         "ClusterIdentifier": str,
         "ConnectedDatabase": str,
         "DbUser": str,
-        "SchemaPattern": str,
+        "Schema": str,
         "SecretArn": str,
-        "TablePattern": str,
+        "Table": str,
         "WorkgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class ListTablesRequestListTablesPaginateTypeDef(
-    _RequiredListTablesRequestListTablesPaginateTypeDef,
-    _OptionalListTablesRequestListTablesPaginateTypeDef,
+class DescribeTableRequestDescribeTablePaginateTypeDef(
+    _RequiredDescribeTableRequestDescribeTablePaginateTypeDef,
+    _OptionalDescribeTableRequestDescribeTablePaginateTypeDef,
 ):
     pass
 
+_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
+    "_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
+    "_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetStatementResultRequestGetStatementResultPaginateTypeDef(
+    _RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef,
+    _OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef,
+):
+    pass
 
-_RequiredListTablesRequestRequestTypeDef = TypedDict(
-    "_RequiredListTablesRequestRequestTypeDef",
+_RequiredListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
+    "_RequiredListDatabasesRequestListDatabasesPaginateTypeDef",
     {
         "Database": str,
     },
 )
-_OptionalListTablesRequestRequestTypeDef = TypedDict(
-    "_OptionalListTablesRequestRequestTypeDef",
+_OptionalListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
+    "_OptionalListDatabasesRequestListDatabasesPaginateTypeDef",
     {
         "ClusterIdentifier": str,
-        "ConnectedDatabase": str,
         "DbUser": str,
-        "MaxResults": int,
-        "NextToken": str,
-        "SchemaPattern": str,
         "SecretArn": str,
-        "TablePattern": str,
         "WorkgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class ListTablesRequestRequestTypeDef(
-    _RequiredListTablesRequestRequestTypeDef, _OptionalListTablesRequestRequestTypeDef
+class ListDatabasesRequestListDatabasesPaginateTypeDef(
+    _RequiredListDatabasesRequestListDatabasesPaginateTypeDef,
+    _OptionalListDatabasesRequestListDatabasesPaginateTypeDef,
 ):
     pass
 
-
-TableMemberTypeDef = TypedDict(
-    "TableMemberTypeDef",
+_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
     {
-        "name": str,
-        "schema": str,
-        "type": str,
+        "Database": str,
+    },
+)
+_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ConnectedDatabase": str,
+        "DbUser": str,
+        "SchemaPattern": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+class ListSchemasRequestListSchemasPaginateTypeDef(
+    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
+    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
+):
+    pass
+
+ListStatementsRequestListStatementsPaginateTypeDef = TypedDict(
+    "ListStatementsRequestListStatementsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "RoleLevel": bool,
+        "StatementName": str,
+        "Status": StatusStringType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_RequiredListTablesRequestListTablesPaginateTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Database": str,
     },
 )
-
-DescribeTableResponseTypeDef = TypedDict(
-    "DescribeTableResponseTypeDef",
+_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_OptionalListTablesRequestListTablesPaginateTypeDef",
     {
-        "ColumnList": List[ColumnMetadataTypeDef],
-        "NextToken": str,
-        "TableName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ClusterIdentifier": str,
+        "ConnectedDatabase": str,
+        "DbUser": str,
+        "SchemaPattern": str,
+        "SecretArn": str,
+        "TablePattern": str,
+        "WorkgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+class ListTablesRequestListTablesPaginateTypeDef(
+    _RequiredListTablesRequestListTablesPaginateTypeDef,
+    _OptionalListTablesRequestListTablesPaginateTypeDef,
+):
+    pass
+
 _RequiredExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredExecuteStatementInputRequestTypeDef",
     {
         "Database": str,
         "Sql": str,
     },
 )
@@ -576,95 +611,40 @@
         "StatementName": str,
         "WithEvent": bool,
         "WorkgroupName": str,
     },
     total=False,
 )
 
-
 class ExecuteStatementInputRequestTypeDef(
     _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
 ):
     pass
 
-
-_RequiredStatementDataTypeDef = TypedDict(
-    "_RequiredStatementDataTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalStatementDataTypeDef = TypedDict(
-    "_OptionalStatementDataTypeDef",
-    {
-        "CreatedAt": datetime,
-        "IsBatchStatement": bool,
-        "QueryParameters": List[SqlParameterTypeDef],
-        "QueryString": str,
-        "QueryStrings": List[str],
-        "SecretArn": str,
-        "StatementName": str,
-        "Status": StatusStringType,
-        "UpdatedAt": datetime,
-    },
-    total=False,
-)
-
-
-class StatementDataTypeDef(_RequiredStatementDataTypeDef, _OptionalStatementDataTypeDef):
-    pass
-
-
-DescribeStatementResponseTypeDef = TypedDict(
-    "DescribeStatementResponseTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "CreatedAt": datetime,
-        "Database": str,
-        "DbUser": str,
-        "Duration": int,
-        "Error": str,
-        "HasResultSet": bool,
-        "Id": str,
-        "QueryParameters": List[SqlParameterTypeDef],
-        "QueryString": str,
-        "RedshiftPid": int,
-        "RedshiftQueryId": int,
-        "ResultRows": int,
-        "ResultSize": int,
-        "SecretArn": str,
-        "Status": StatusStringType,
-        "SubStatements": List[SubStatementDataTypeDef],
-        "UpdatedAt": datetime,
-        "WorkgroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetStatementResultResponseTypeDef = TypedDict(
     "GetStatementResultResponseTypeDef",
     {
         "ColumnMetadata": List[ColumnMetadataTypeDef],
         "NextToken": str,
         "Records": List[List[FieldTypeDef]],
         "TotalNumRows": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTablesResponseTypeDef = TypedDict(
     "ListTablesResponseTypeDef",
     {
         "NextToken": str,
         "Tables": List[TableMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStatementsResponseTypeDef = TypedDict(
     "ListStatementsResponseTypeDef",
     {
         "NextToken": str,
         "Statements": List[StatementDataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data/type_defs.pyi` & `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,46 +18,48 @@
 from .literals import StatementStatusStringType, StatusStringType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "BatchExecuteStatementInputRequestTypeDef",
-    "BatchExecuteStatementOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CancelStatementRequestRequestTypeDef",
-    "CancelStatementResponseTypeDef",
     "ColumnMetadataTypeDef",
     "DescribeStatementRequestRequestTypeDef",
-    "SqlParameterTypeDef",
+    "SqlParameterOutputTypeDef",
     "SubStatementDataTypeDef",
-    "DescribeTableRequestDescribeTablePaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeTableRequestRequestTypeDef",
-    "ExecuteStatementOutputTypeDef",
+    "SqlParameterTypeDef",
     "FieldTypeDef",
-    "GetStatementResultRequestGetStatementResultPaginateTypeDef",
     "GetStatementResultRequestRequestTypeDef",
-    "ListDatabasesRequestListDatabasesPaginateTypeDef",
     "ListDatabasesRequestRequestTypeDef",
-    "ListDatabasesResponseTypeDef",
-    "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSchemasRequestRequestTypeDef",
-    "ListSchemasResponseTypeDef",
-    "ListStatementsRequestListStatementsPaginateTypeDef",
     "ListStatementsRequestRequestTypeDef",
-    "ListTablesRequestListTablesPaginateTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableMemberTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "BatchExecuteStatementOutputTypeDef",
+    "CancelStatementResponseTypeDef",
+    "ExecuteStatementOutputTypeDef",
+    "ListDatabasesResponseTypeDef",
+    "ListSchemasResponseTypeDef",
     "DescribeTableResponseTypeDef",
-    "ExecuteStatementInputRequestTypeDef",
     "StatementDataTypeDef",
     "DescribeStatementResponseTypeDef",
+    "DescribeTableRequestDescribeTablePaginateTypeDef",
+    "GetStatementResultRequestGetStatementResultPaginateTypeDef",
+    "ListDatabasesRequestListDatabasesPaginateTypeDef",
+    "ListSchemasRequestListSchemasPaginateTypeDef",
+    "ListStatementsRequestListStatementsPaginateTypeDef",
+    "ListTablesRequestListTablesPaginateTypeDef",
+    "ExecuteStatementInputRequestTypeDef",
     "GetStatementResultResponseTypeDef",
     "ListTablesResponseTypeDef",
     "ListStatementsResponseTypeDef",
 )
 
 _RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementInputRequestTypeDef",
@@ -76,49 +78,40 @@
         "StatementName": str,
         "WithEvent": bool,
         "WorkgroupName": str,
     },
     total=False,
 )
 
+
 class BatchExecuteStatementInputRequestTypeDef(
     _RequiredBatchExecuteStatementInputRequestTypeDef,
     _OptionalBatchExecuteStatementInputRequestTypeDef,
 ):
     pass
 
-BatchExecuteStatementOutputTypeDef = TypedDict(
-    "BatchExecuteStatementOutputTypeDef",
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ClusterIdentifier": str,
-        "CreatedAt": datetime,
-        "Database": str,
-        "DbUser": str,
-        "Id": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CancelStatementRequestRequestTypeDef = TypedDict(
     "CancelStatementRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-CancelStatementResponseTypeDef = TypedDict(
-    "CancelStatementResponseTypeDef",
-    {
-        "Status": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ColumnMetadataTypeDef = TypedDict(
     "ColumnMetadataTypeDef",
     {
         "columnDefault": str,
         "isCaseSensitive": bool,
         "isCurrency": bool,
         "isSigned": bool,
@@ -138,16 +131,16 @@
 DescribeStatementRequestRequestTypeDef = TypedDict(
     "DescribeStatementRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-SqlParameterTypeDef = TypedDict(
-    "SqlParameterTypeDef",
+SqlParameterOutputTypeDef = TypedDict(
+    "SqlParameterOutputTypeDef",
     {
         "name": str,
         "value": str,
     },
 )
 
 _RequiredSubStatementDataTypeDef = TypedDict(
@@ -169,44 +162,29 @@
         "ResultSize": int,
         "Status": StatementStatusStringType,
         "UpdatedAt": datetime,
     },
     total=False,
 )
 
+
 class SubStatementDataTypeDef(_RequiredSubStatementDataTypeDef, _OptionalSubStatementDataTypeDef):
     pass
 
-_RequiredDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
-    "_RequiredDescribeTableRequestDescribeTablePaginateTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
-    "_OptionalDescribeTableRequestDescribeTablePaginateTypeDef",
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ClusterIdentifier": str,
-        "ConnectedDatabase": str,
-        "DbUser": str,
-        "Schema": str,
-        "SecretArn": str,
-        "Table": str,
-        "WorkgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class DescribeTableRequestDescribeTablePaginateTypeDef(
-    _RequiredDescribeTableRequestDescribeTablePaginateTypeDef,
-    _OptionalDescribeTableRequestDescribeTablePaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeTableRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTableRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
 _OptionalDescribeTableRequestRequestTypeDef = TypedDict(
@@ -221,30 +199,26 @@
         "SecretArn": str,
         "Table": str,
         "WorkgroupName": str,
     },
     total=False,
 )
 
+
 class DescribeTableRequestRequestTypeDef(
     _RequiredDescribeTableRequestRequestTypeDef, _OptionalDescribeTableRequestRequestTypeDef
 ):
     pass
 
-ExecuteStatementOutputTypeDef = TypedDict(
-    "ExecuteStatementOutputTypeDef",
+
+SqlParameterTypeDef = TypedDict(
+    "SqlParameterTypeDef",
     {
-        "ClusterIdentifier": str,
-        "CreatedAt": datetime,
-        "Database": str,
-        "DbUser": str,
-        "Id": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "value": str,
     },
 )
 
 FieldTypeDef = TypedDict(
     "FieldTypeDef",
     {
         "blobValue": bytes,
@@ -253,77 +227,35 @@
         "isNull": bool,
         "longValue": int,
         "stringValue": str,
     },
     total=False,
 )
 
-_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
-    "_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
-    "_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetStatementResultRequestGetStatementResultPaginateTypeDef(
-    _RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef,
-    _OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef,
-):
-    pass
-
 _RequiredGetStatementResultRequestRequestTypeDef = TypedDict(
     "_RequiredGetStatementResultRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalGetStatementResultRequestRequestTypeDef = TypedDict(
     "_OptionalGetStatementResultRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetStatementResultRequestRequestTypeDef(
     _RequiredGetStatementResultRequestRequestTypeDef,
     _OptionalGetStatementResultRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
-    "_RequiredListDatabasesRequestListDatabasesPaginateTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
-    "_OptionalListDatabasesRequestListDatabasesPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "DbUser": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDatabasesRequestListDatabasesPaginateTypeDef(
-    _RequiredListDatabasesRequestListDatabasesPaginateTypeDef,
-    _OptionalListDatabasesRequestListDatabasesPaginateTypeDef,
-):
-    pass
 
 _RequiredListDatabasesRequestRequestTypeDef = TypedDict(
     "_RequiredListDatabasesRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
@@ -336,53 +268,20 @@
         "NextToken": str,
         "SecretArn": str,
         "WorkgroupName": str,
     },
     total=False,
 )
 
+
 class ListDatabasesRequestRequestTypeDef(
     _RequiredListDatabasesRequestRequestTypeDef, _OptionalListDatabasesRequestRequestTypeDef
 ):
     pass
 
-ListDatabasesResponseTypeDef = TypedDict(
-    "ListDatabasesResponseTypeDef",
-    {
-        "Databases": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ConnectedDatabase": str,
-        "DbUser": str,
-        "SchemaPattern": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
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
 
 _RequiredListSchemasRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemasRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
@@ -397,78 +296,33 @@
         "SchemaPattern": str,
         "SecretArn": str,
         "WorkgroupName": str,
     },
     total=False,
 )
 
+
 class ListSchemasRequestRequestTypeDef(
     _RequiredListSchemasRequestRequestTypeDef, _OptionalListSchemasRequestRequestTypeDef
 ):
     pass
 
-ListSchemasResponseTypeDef = TypedDict(
-    "ListSchemasResponseTypeDef",
-    {
-        "NextToken": str,
-        "Schemas": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListStatementsRequestListStatementsPaginateTypeDef = TypedDict(
-    "ListStatementsRequestListStatementsPaginateTypeDef",
-    {
-        "RoleLevel": bool,
-        "StatementName": str,
-        "Status": StatusStringType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListStatementsRequestRequestTypeDef = TypedDict(
     "ListStatementsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "RoleLevel": bool,
         "StatementName": str,
         "Status": StatusStringType,
     },
     total=False,
 )
 
-_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_RequiredListTablesRequestListTablesPaginateTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_OptionalListTablesRequestListTablesPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ConnectedDatabase": str,
-        "DbUser": str,
-        "SchemaPattern": str,
-        "SecretArn": str,
-        "TablePattern": str,
-        "WorkgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTablesRequestListTablesPaginateTypeDef(
-    _RequiredListTablesRequestListTablesPaginateTypeDef,
-    _OptionalListTablesRequestListTablesPaginateTypeDef,
-):
-    pass
-
 _RequiredListTablesRequestRequestTypeDef = TypedDict(
     "_RequiredListTablesRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
 _OptionalListTablesRequestRequestTypeDef = TypedDict(
@@ -483,159 +337,343 @@
         "SecretArn": str,
         "TablePattern": str,
         "WorkgroupName": str,
     },
     total=False,
 )
 
+
 class ListTablesRequestRequestTypeDef(
     _RequiredListTablesRequestRequestTypeDef, _OptionalListTablesRequestRequestTypeDef
 ):
     pass
 
+
 TableMemberTypeDef = TypedDict(
     "TableMemberTypeDef",
     {
         "name": str,
         "schema": str,
         "type": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+BatchExecuteStatementOutputTypeDef = TypedDict(
+    "BatchExecuteStatementOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ClusterIdentifier": str,
+        "CreatedAt": datetime,
+        "Database": str,
+        "DbUser": str,
+        "Id": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelStatementResponseTypeDef = TypedDict(
+    "CancelStatementResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Status": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeTableResponseTypeDef = TypedDict(
-    "DescribeTableResponseTypeDef",
+ExecuteStatementOutputTypeDef = TypedDict(
+    "ExecuteStatementOutputTypeDef",
     {
-        "ColumnList": List[ColumnMetadataTypeDef],
-        "NextToken": str,
-        "TableName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ClusterIdentifier": str,
+        "CreatedAt": datetime,
+        "Database": str,
+        "DbUser": str,
+        "Id": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredExecuteStatementInputRequestTypeDef = TypedDict(
-    "_RequiredExecuteStatementInputRequestTypeDef",
+ListDatabasesResponseTypeDef = TypedDict(
+    "ListDatabasesResponseTypeDef",
     {
-        "Database": str,
-        "Sql": str,
+        "Databases": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalExecuteStatementInputRequestTypeDef = TypedDict(
-    "_OptionalExecuteStatementInputRequestTypeDef",
+
+ListSchemasResponseTypeDef = TypedDict(
+    "ListSchemasResponseTypeDef",
     {
-        "ClientToken": str,
-        "ClusterIdentifier": str,
-        "DbUser": str,
-        "Parameters": Sequence[SqlParameterTypeDef],
-        "SecretArn": str,
-        "StatementName": str,
-        "WithEvent": bool,
-        "WorkgroupName": str,
+        "NextToken": str,
+        "Schemas": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ExecuteStatementInputRequestTypeDef(
-    _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
-):
-    pass
+DescribeTableResponseTypeDef = TypedDict(
+    "DescribeTableResponseTypeDef",
+    {
+        "ColumnList": List[ColumnMetadataTypeDef],
+        "NextToken": str,
+        "TableName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredStatementDataTypeDef = TypedDict(
     "_RequiredStatementDataTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalStatementDataTypeDef = TypedDict(
     "_OptionalStatementDataTypeDef",
     {
         "CreatedAt": datetime,
         "IsBatchStatement": bool,
-        "QueryParameters": List[SqlParameterTypeDef],
+        "QueryParameters": List[SqlParameterOutputTypeDef],
         "QueryString": str,
         "QueryStrings": List[str],
         "SecretArn": str,
         "StatementName": str,
         "Status": StatusStringType,
         "UpdatedAt": datetime,
     },
     total=False,
 )
 
+
 class StatementDataTypeDef(_RequiredStatementDataTypeDef, _OptionalStatementDataTypeDef):
     pass
 
+
 DescribeStatementResponseTypeDef = TypedDict(
     "DescribeStatementResponseTypeDef",
     {
         "ClusterIdentifier": str,
         "CreatedAt": datetime,
         "Database": str,
         "DbUser": str,
         "Duration": int,
         "Error": str,
         "HasResultSet": bool,
         "Id": str,
-        "QueryParameters": List[SqlParameterTypeDef],
+        "QueryParameters": List[SqlParameterOutputTypeDef],
         "QueryString": str,
         "RedshiftPid": int,
         "RedshiftQueryId": int,
         "ResultRows": int,
         "ResultSize": int,
         "SecretArn": str,
         "Status": StatusStringType,
         "SubStatements": List[SubStatementDataTypeDef],
         "UpdatedAt": datetime,
         "WorkgroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
+    "_RequiredDescribeTableRequestDescribeTablePaginateTypeDef",
+    {
+        "Database": str,
+    },
+)
+_OptionalDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
+    "_OptionalDescribeTableRequestDescribeTablePaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ConnectedDatabase": str,
+        "DbUser": str,
+        "Schema": str,
+        "SecretArn": str,
+        "Table": str,
+        "WorkgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeTableRequestDescribeTablePaginateTypeDef(
+    _RequiredDescribeTableRequestDescribeTablePaginateTypeDef,
+    _OptionalDescribeTableRequestDescribeTablePaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
+    "_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef",
+    {
+        "Id": str,
     },
 )
+_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
+    "_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetStatementResultRequestGetStatementResultPaginateTypeDef(
+    _RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef,
+    _OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
+    "_RequiredListDatabasesRequestListDatabasesPaginateTypeDef",
+    {
+        "Database": str,
+    },
+)
+_OptionalListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
+    "_OptionalListDatabasesRequestListDatabasesPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "DbUser": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDatabasesRequestListDatabasesPaginateTypeDef(
+    _RequiredListDatabasesRequestListDatabasesPaginateTypeDef,
+    _OptionalListDatabasesRequestListDatabasesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "Database": str,
+    },
+)
+_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ConnectedDatabase": str,
+        "DbUser": str,
+        "SchemaPattern": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
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
+ListStatementsRequestListStatementsPaginateTypeDef = TypedDict(
+    "ListStatementsRequestListStatementsPaginateTypeDef",
+    {
+        "RoleLevel": bool,
+        "StatementName": str,
+        "Status": StatusStringType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_RequiredListTablesRequestListTablesPaginateTypeDef",
+    {
+        "Database": str,
+    },
+)
+_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_OptionalListTablesRequestListTablesPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ConnectedDatabase": str,
+        "DbUser": str,
+        "SchemaPattern": str,
+        "SecretArn": str,
+        "TablePattern": str,
+        "WorkgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTablesRequestListTablesPaginateTypeDef(
+    _RequiredListTablesRequestListTablesPaginateTypeDef,
+    _OptionalListTablesRequestListTablesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredExecuteStatementInputRequestTypeDef = TypedDict(
+    "_RequiredExecuteStatementInputRequestTypeDef",
+    {
+        "Database": str,
+        "Sql": str,
+    },
+)
+_OptionalExecuteStatementInputRequestTypeDef = TypedDict(
+    "_OptionalExecuteStatementInputRequestTypeDef",
+    {
+        "ClientToken": str,
+        "ClusterIdentifier": str,
+        "DbUser": str,
+        "Parameters": Sequence[SqlParameterTypeDef],
+        "SecretArn": str,
+        "StatementName": str,
+        "WithEvent": bool,
+        "WorkgroupName": str,
+    },
+    total=False,
+)
+
+
+class ExecuteStatementInputRequestTypeDef(
+    _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
+):
+    pass
+
 
 GetStatementResultResponseTypeDef = TypedDict(
     "GetStatementResultResponseTypeDef",
     {
         "ColumnMetadata": List[ColumnMetadataTypeDef],
         "NextToken": str,
         "Records": List[List[FieldTypeDef]],
         "TotalNumRows": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTablesResponseTypeDef = TypedDict(
     "ListTablesResponseTypeDef",
     {
         "NextToken": str,
         "Tables": List[TableMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStatementsResponseTypeDef = TypedDict(
     "ListStatementsResponseTypeDef",
     {
         "NextToken": str,
         "Statements": List[StatementDataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data.egg-info/PKG-INFO` & `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift-data
-Version: 1.28.0
-Summary: Type annotations for boto3.RedshiftDataAPIService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.RedshiftDataAPIService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-redshift-data"></a>
 
 # mypy-boto3-redshift-data
 
 [![PyPI - mypy-boto3-redshift-data](https://img.shields.io/pypi/v/mypy-boto3-redshift-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift-data?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift-data)](https://pepy.tech/project/mypy-boto3-redshift-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftDataAPIService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
+[boto3.RedshiftDataAPIService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
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
 [mypy-boto3-redshift-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -341,44 +341,45 @@
 
 `mypy_boto3_redshift_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_redshift_data.type_defs import (
     BatchExecuteStatementInputRequestTypeDef,
-    BatchExecuteStatementOutputTypeDef,
+    ResponseMetadataTypeDef,
     CancelStatementRequestRequestTypeDef,
-    CancelStatementResponseTypeDef,
     ColumnMetadataTypeDef,
     DescribeStatementRequestRequestTypeDef,
-    SqlParameterTypeDef,
+    SqlParameterOutputTypeDef,
     SubStatementDataTypeDef,
-    DescribeTableRequestDescribeTablePaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeTableRequestRequestTypeDef,
-    ExecuteStatementOutputTypeDef,
+    SqlParameterTypeDef,
     FieldTypeDef,
-    GetStatementResultRequestGetStatementResultPaginateTypeDef,
     GetStatementResultRequestRequestTypeDef,
-    ListDatabasesRequestListDatabasesPaginateTypeDef,
     ListDatabasesRequestRequestTypeDef,
-    ListDatabasesResponseTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
-    ListSchemasResponseTypeDef,
-    ListStatementsRequestListStatementsPaginateTypeDef,
     ListStatementsRequestRequestTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableMemberTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    BatchExecuteStatementOutputTypeDef,
+    CancelStatementResponseTypeDef,
+    ExecuteStatementOutputTypeDef,
+    ListDatabasesResponseTypeDef,
+    ListSchemasResponseTypeDef,
     DescribeTableResponseTypeDef,
-    ExecuteStatementInputRequestTypeDef,
     StatementDataTypeDef,
     DescribeStatementResponseTypeDef,
+    DescribeTableRequestDescribeTablePaginateTypeDef,
+    GetStatementResultRequestGetStatementResultPaginateTypeDef,
+    ListDatabasesRequestListDatabasesPaginateTypeDef,
+    ListSchemasRequestListSchemasPaginateTypeDef,
+    ListStatementsRequestListStatementsPaginateTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
+    ExecuteStatementInputRequestTypeDef,
     GetStatementResultResponseTypeDef,
     ListTablesResponseTypeDef,
     ListStatementsResponseTypeDef,
 )
 
 
 def get_structure() -> BatchExecuteStatementInputRequestTypeDef:
```

### Comparing `mypy-boto3-redshift-data-1.28.0/mypy_boto3_redshift_data.egg-info/SOURCES.txt` & `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.28.0/setup.py` & `mypy-boto3-redshift-data-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-redshift-data",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_redshift_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RedshiftDataAPIService 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.RedshiftDataAPIService 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

