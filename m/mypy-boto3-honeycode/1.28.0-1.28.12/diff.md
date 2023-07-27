# Comparing `tmp/mypy-boto3-honeycode-1.28.0.tar.gz` & `tmp/mypy-boto3-honeycode-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-honeycode-1.28.0.tar", last modified: Thu Jul  6 20:59:42 2023, max compression
+gzip compressed data, was "mypy-boto3-honeycode-1.28.12.tar", last modified: Thu Jul 27 05:34:46 2023, max compression
```

## Comparing `mypy-boto3-honeycode-1.28.0.tar` & `mypy-boto3-honeycode-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:42.066317 mypy-boto3-honeycode-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:42:37.000000 mypy-boto3-honeycode-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-07-06 20:59:42.066317 mypy-boto3-honeycode-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-07-06 20:42:37.000000 mypy-boto3-honeycode-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:42.066317 mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-06 20:42:37.000000 mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-06 20:42:37.000000 mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 20:42:37.000000 mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15516 2023-07-06 20:42:37.000000 mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-07-06 20:42:37.000000 mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-06 20:42:38.000000 mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-07-06 20:42:37.000000 mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-07-06 20:42:37.000000 mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-06 20:42:37.000000 mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:42:37.000000 mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20834 2023-07-06 20:42:38.000000 mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20799 2023-07-06 20:42:38.000000 mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:42:37.000000 mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:42.066317 mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-07-06 20:59:41.000000 mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-06 20:59:41.000000 mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:41.000000 mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:41.000000 mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:41.000000 mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 20:59:41.000000 mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:42.066317 mypy-boto3-honeycode-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 20:42:37.000000 mypy-boto3-honeycode-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:46.304494 mypy-boto3-honeycode-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-27 05:34:46.304494 mypy-boto3-honeycode-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13986 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:46.304494 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15516 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-07-27 05:23:19.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9241 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22615 2023-07-27 05:23:19.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22578 2023-07-27 05:23:19.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:46.304494 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-27 05:34:46.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 05:34:46.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:46.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:46.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:46.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:46.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:46.304494 mypy-boto3-honeycode-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/setup.py
```

### Comparing `mypy-boto3-honeycode-1.28.0/LICENSE` & `mypy-boto3-honeycode-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.0/PKG-INFO` & `mypy-boto3-honeycode-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-honeycode
-Version: 1.28.0
-Summary: Type annotations for boto3.Honeycode 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Honeycode 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-honeycode"></a>
 
 # mypy-boto3-honeycode
 
 [![PyPI - mypy-boto3-honeycode](https://img.shields.io/pypi/v/mypy-boto3-honeycode.svg?color=blue)](https://pypi.org/project/mypy-boto3-honeycode)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-honeycode.svg?color=blue)](https://pypi.org/project/mypy-boto3-honeycode)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-honeycode?color=blue)](https://pypistats.org/packages/mypy-boto3-honeycode)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-honeycode)](https://pepy.tech/project/mypy-boto3-honeycode)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Honeycode 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
+[boto3.Honeycode 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
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
 [mypy-boto3-honeycode docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/).
 
 See how it helps to find and fix potential bugs:
 
@@ -342,19 +342,22 @@
     FailedBatchItemTypeDef,
     BatchDeleteTableRowsRequestRequestTypeDef,
     UpsertRowsResultTypeDef,
     CellInputTypeDef,
     CellTypeDef,
     ColumnMetadataTypeDef,
     DataItemTypeDef,
+    DelimitedTextImportOptionsOutputTypeDef,
     DelimitedTextImportOptionsTypeDef,
     DescribeTableDataImportJobRequestRequestTypeDef,
+    SourceDataColumnPropertiesOutputTypeDef,
     SourceDataColumnPropertiesTypeDef,
     FilterTypeDef,
     VariableValueTypeDef,
+    ImportDataSourceConfigOutputTypeDef,
     ImportDataSourceConfigTypeDef,
     ImportJobSubmitterTypeDef,
     InvokeScreenAutomationResultTypeDef,
     ListTableColumnsRequestListTableColumnsPaginateTypeDef,
     ListTableColumnsRequestRequestTypeDef,
     TableColumnTypeDef,
     ListTableRowsRequestListTableRowsPaginateTypeDef,
@@ -373,33 +376,36 @@
     BatchDeleteTableRowsResultTypeDef,
     BatchUpdateTableRowsResultTypeDef,
     BatchUpsertTableRowsResultTypeDef,
     CreateRowDataTypeDef,
     UpdateRowDataTypeDef,
     TableRowTypeDef,
     ResultRowTypeDef,
+    DestinationOptionsOutputTypeDef,
     DestinationOptionsTypeDef,
     QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     QueryTableRowsRequestRequestTypeDef,
     UpsertRowDataTypeDef,
     GetScreenDataRequestRequestTypeDef,
     InvokeScreenAutomationRequestRequestTypeDef,
+    ImportDataSourceOutputTypeDef,
     ImportDataSourceTypeDef,
     ListTableColumnsResultTypeDef,
     ListTablesResultTypeDef,
     BatchCreateTableRowsRequestRequestTypeDef,
     BatchUpdateTableRowsRequestRequestTypeDef,
     ListTableRowsResultTypeDef,
     QueryTableRowsResultTypeDef,
     ResultSetTypeDef,
+    ImportOptionsOutputTypeDef,
     ImportOptionsTypeDef,
     BatchUpsertTableRowsRequestRequestTypeDef,
     GetScreenDataResultTypeDef,
-    StartTableDataImportJobRequestRequestTypeDef,
     TableDataImportJobMetadataTypeDef,
+    StartTableDataImportJobRequestRequestTypeDef,
     DescribeTableDataImportJobResultTypeDef,
 )
 
 
 def get_structure() -> FailedBatchItemTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-honeycode-1.28.0/README.md` & `mypy-boto3-honeycode-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-honeycode"></a>
 
 # mypy-boto3-honeycode
 
 [![PyPI - mypy-boto3-honeycode](https://img.shields.io/pypi/v/mypy-boto3-honeycode.svg?color=blue)](https://pypi.org/project/mypy-boto3-honeycode)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-honeycode.svg?color=blue)](https://pypi.org/project/mypy-boto3-honeycode)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-honeycode?color=blue)](https://pypistats.org/packages/mypy-boto3-honeycode)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-honeycode)](https://pepy.tech/project/mypy-boto3-honeycode)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Honeycode 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
+[boto3.Honeycode 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
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
 [mypy-boto3-honeycode docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/).
 
 See how it helps to find and fix potential bugs:
 
@@ -310,19 +310,22 @@
     FailedBatchItemTypeDef,
     BatchDeleteTableRowsRequestRequestTypeDef,
     UpsertRowsResultTypeDef,
     CellInputTypeDef,
     CellTypeDef,
     ColumnMetadataTypeDef,
     DataItemTypeDef,
+    DelimitedTextImportOptionsOutputTypeDef,
     DelimitedTextImportOptionsTypeDef,
     DescribeTableDataImportJobRequestRequestTypeDef,
+    SourceDataColumnPropertiesOutputTypeDef,
     SourceDataColumnPropertiesTypeDef,
     FilterTypeDef,
     VariableValueTypeDef,
+    ImportDataSourceConfigOutputTypeDef,
     ImportDataSourceConfigTypeDef,
     ImportJobSubmitterTypeDef,
     InvokeScreenAutomationResultTypeDef,
     ListTableColumnsRequestListTableColumnsPaginateTypeDef,
     ListTableColumnsRequestRequestTypeDef,
     TableColumnTypeDef,
     ListTableRowsRequestListTableRowsPaginateTypeDef,
@@ -341,33 +344,36 @@
     BatchDeleteTableRowsResultTypeDef,
     BatchUpdateTableRowsResultTypeDef,
     BatchUpsertTableRowsResultTypeDef,
     CreateRowDataTypeDef,
     UpdateRowDataTypeDef,
     TableRowTypeDef,
     ResultRowTypeDef,
+    DestinationOptionsOutputTypeDef,
     DestinationOptionsTypeDef,
     QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     QueryTableRowsRequestRequestTypeDef,
     UpsertRowDataTypeDef,
     GetScreenDataRequestRequestTypeDef,
     InvokeScreenAutomationRequestRequestTypeDef,
+    ImportDataSourceOutputTypeDef,
     ImportDataSourceTypeDef,
     ListTableColumnsResultTypeDef,
     ListTablesResultTypeDef,
     BatchCreateTableRowsRequestRequestTypeDef,
     BatchUpdateTableRowsRequestRequestTypeDef,
     ListTableRowsResultTypeDef,
     QueryTableRowsResultTypeDef,
     ResultSetTypeDef,
+    ImportOptionsOutputTypeDef,
     ImportOptionsTypeDef,
     BatchUpsertTableRowsRequestRequestTypeDef,
     GetScreenDataResultTypeDef,
-    StartTableDataImportJobRequestRequestTypeDef,
     TableDataImportJobMetadataTypeDef,
+    StartTableDataImportJobRequestRequestTypeDef,
     DescribeTableDataImportJobResultTypeDef,
 )
 
 
 def get_structure() -> FailedBatchItemTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/__init__.py` & `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/__init__.pyi` & `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/__main__.py` & `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Honeycode 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Honeycode 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode\nOther"
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

### Comparing `mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/client.py` & `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/client.pyi` & `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/literals.py` & `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,15 @@
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
@@ -280,26 +281,28 @@
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

### Comparing `mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/literals.pyi` & `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,15 @@
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
@@ -278,26 +279,28 @@
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

### Comparing `mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/paginator.py` & `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/paginator.pyi` & `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/type_defs.py` & `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,19 +37,22 @@
     "FailedBatchItemTypeDef",
     "BatchDeleteTableRowsRequestRequestTypeDef",
     "UpsertRowsResultTypeDef",
     "CellInputTypeDef",
     "CellTypeDef",
     "ColumnMetadataTypeDef",
     "DataItemTypeDef",
+    "DelimitedTextImportOptionsOutputTypeDef",
     "DelimitedTextImportOptionsTypeDef",
     "DescribeTableDataImportJobRequestRequestTypeDef",
+    "SourceDataColumnPropertiesOutputTypeDef",
     "SourceDataColumnPropertiesTypeDef",
     "FilterTypeDef",
     "VariableValueTypeDef",
+    "ImportDataSourceConfigOutputTypeDef",
     "ImportDataSourceConfigTypeDef",
     "ImportJobSubmitterTypeDef",
     "InvokeScreenAutomationResultTypeDef",
     "ListTableColumnsRequestListTableColumnsPaginateTypeDef",
     "ListTableColumnsRequestRequestTypeDef",
     "TableColumnTypeDef",
     "ListTableRowsRequestListTableRowsPaginateTypeDef",
@@ -68,33 +71,36 @@
     "BatchDeleteTableRowsResultTypeDef",
     "BatchUpdateTableRowsResultTypeDef",
     "BatchUpsertTableRowsResultTypeDef",
     "CreateRowDataTypeDef",
     "UpdateRowDataTypeDef",
     "TableRowTypeDef",
     "ResultRowTypeDef",
+    "DestinationOptionsOutputTypeDef",
     "DestinationOptionsTypeDef",
     "QueryTableRowsRequestQueryTableRowsPaginateTypeDef",
     "QueryTableRowsRequestRequestTypeDef",
     "UpsertRowDataTypeDef",
     "GetScreenDataRequestRequestTypeDef",
     "InvokeScreenAutomationRequestRequestTypeDef",
+    "ImportDataSourceOutputTypeDef",
     "ImportDataSourceTypeDef",
     "ListTableColumnsResultTypeDef",
     "ListTablesResultTypeDef",
     "BatchCreateTableRowsRequestRequestTypeDef",
     "BatchUpdateTableRowsRequestRequestTypeDef",
     "ListTableRowsResultTypeDef",
     "QueryTableRowsResultTypeDef",
     "ResultSetTypeDef",
+    "ImportOptionsOutputTypeDef",
     "ImportOptionsTypeDef",
     "BatchUpsertTableRowsRequestRequestTypeDef",
     "GetScreenDataResultTypeDef",
-    "StartTableDataImportJobRequestRequestTypeDef",
     "TableDataImportJobMetadataTypeDef",
+    "StartTableDataImportJobRequestRequestTypeDef",
     "DescribeTableDataImportJobResultTypeDef",
 )
 
 FailedBatchItemTypeDef = TypedDict(
     "FailedBatchItemTypeDef",
     {
         "id": str,
@@ -169,14 +175,38 @@
         "overrideFormat": FormatType,
         "rawValue": str,
         "formattedValue": str,
     },
     total=False,
 )
 
+_RequiredDelimitedTextImportOptionsOutputTypeDef = TypedDict(
+    "_RequiredDelimitedTextImportOptionsOutputTypeDef",
+    {
+        "delimiter": str,
+    },
+)
+_OptionalDelimitedTextImportOptionsOutputTypeDef = TypedDict(
+    "_OptionalDelimitedTextImportOptionsOutputTypeDef",
+    {
+        "hasHeaderRow": bool,
+        "ignoreEmptyRows": bool,
+        "dataCharacterEncoding": ImportDataCharacterEncodingType,
+    },
+    total=False,
+)
+
+
+class DelimitedTextImportOptionsOutputTypeDef(
+    _RequiredDelimitedTextImportOptionsOutputTypeDef,
+    _OptionalDelimitedTextImportOptionsOutputTypeDef,
+):
+    pass
+
+
 _RequiredDelimitedTextImportOptionsTypeDef = TypedDict(
     "_RequiredDelimitedTextImportOptionsTypeDef",
     {
         "delimiter": str,
     },
 )
 _OptionalDelimitedTextImportOptionsTypeDef = TypedDict(
@@ -201,14 +231,22 @@
     {
         "workbookId": str,
         "tableId": str,
         "jobId": str,
     },
 )
 
+SourceDataColumnPropertiesOutputTypeDef = TypedDict(
+    "SourceDataColumnPropertiesOutputTypeDef",
+    {
+        "columnIndex": int,
+    },
+    total=False,
+)
+
 SourceDataColumnPropertiesTypeDef = TypedDict(
     "SourceDataColumnPropertiesTypeDef",
     {
         "columnIndex": int,
     },
     total=False,
 )
@@ -235,14 +273,22 @@
 VariableValueTypeDef = TypedDict(
     "VariableValueTypeDef",
     {
         "rawValue": str,
     },
 )
 
+ImportDataSourceConfigOutputTypeDef = TypedDict(
+    "ImportDataSourceConfigOutputTypeDef",
+    {
+        "dataSourceUrl": str,
+    },
+    total=False,
+)
+
 ImportDataSourceConfigTypeDef = TypedDict(
     "ImportDataSourceConfigTypeDef",
     {
         "dataSourceUrl": str,
     },
     total=False,
 )
@@ -558,18 +604,26 @@
 )
 
 
 class ResultRowTypeDef(_RequiredResultRowTypeDef, _OptionalResultRowTypeDef):
     pass
 
 
+DestinationOptionsOutputTypeDef = TypedDict(
+    "DestinationOptionsOutputTypeDef",
+    {
+        "columnMap": Dict[str, SourceDataColumnPropertiesOutputTypeDef],
+    },
+    total=False,
+)
+
 DestinationOptionsTypeDef = TypedDict(
     "DestinationOptionsTypeDef",
     {
-        "columnMap": Dict[str, SourceDataColumnPropertiesTypeDef],
+        "columnMap": Mapping[str, SourceDataColumnPropertiesTypeDef],
     },
     total=False,
 )
 
 _RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
     "_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
     {
@@ -675,14 +729,21 @@
 class InvokeScreenAutomationRequestRequestTypeDef(
     _RequiredInvokeScreenAutomationRequestRequestTypeDef,
     _OptionalInvokeScreenAutomationRequestRequestTypeDef,
 ):
     pass
 
 
+ImportDataSourceOutputTypeDef = TypedDict(
+    "ImportDataSourceOutputTypeDef",
+    {
+        "dataSourceConfig": ImportDataSourceConfigOutputTypeDef,
+    },
+)
+
 ImportDataSourceTypeDef = TypedDict(
     "ImportDataSourceTypeDef",
     {
         "dataSourceConfig": ImportDataSourceConfigTypeDef,
     },
 )
 
@@ -781,14 +842,23 @@
     "ResultSetTypeDef",
     {
         "headers": List[ColumnMetadataTypeDef],
         "rows": List[ResultRowTypeDef],
     },
 )
 
+ImportOptionsOutputTypeDef = TypedDict(
+    "ImportOptionsOutputTypeDef",
+    {
+        "destinationOptions": DestinationOptionsOutputTypeDef,
+        "delimitedTextOptions": DelimitedTextImportOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 ImportOptionsTypeDef = TypedDict(
     "ImportOptionsTypeDef",
     {
         "destinationOptions": DestinationOptionsTypeDef,
         "delimitedTextOptions": DelimitedTextImportOptionsTypeDef,
     },
     total=False,
@@ -824,36 +894,36 @@
         "results": Dict[str, ResultSetTypeDef],
         "workbookCursor": int,
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TableDataImportJobMetadataTypeDef = TypedDict(
+    "TableDataImportJobMetadataTypeDef",
+    {
+        "submitter": ImportJobSubmitterTypeDef,
+        "submitTime": datetime,
+        "importOptions": ImportOptionsOutputTypeDef,
+        "dataSource": ImportDataSourceOutputTypeDef,
+    },
+)
+
 StartTableDataImportJobRequestRequestTypeDef = TypedDict(
     "StartTableDataImportJobRequestRequestTypeDef",
     {
         "workbookId": str,
         "dataSource": ImportDataSourceTypeDef,
         "dataFormat": Literal["DELIMITED_TEXT"],
         "destinationTableId": str,
         "importOptions": ImportOptionsTypeDef,
         "clientRequestToken": str,
     },
 )
 
-TableDataImportJobMetadataTypeDef = TypedDict(
-    "TableDataImportJobMetadataTypeDef",
-    {
-        "submitter": ImportJobSubmitterTypeDef,
-        "submitTime": datetime,
-        "importOptions": ImportOptionsTypeDef,
-        "dataSource": ImportDataSourceTypeDef,
-    },
-)
-
 DescribeTableDataImportJobResultTypeDef = TypedDict(
     "DescribeTableDataImportJobResultTypeDef",
     {
         "jobStatus": TableDataImportJobStatusType,
         "message": str,
         "jobMetadata": TableDataImportJobMetadataTypeDef,
         "errorCode": ErrorCodeType,
```

### Comparing `mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode/type_defs.pyi` & `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -36,19 +36,22 @@
     "FailedBatchItemTypeDef",
     "BatchDeleteTableRowsRequestRequestTypeDef",
     "UpsertRowsResultTypeDef",
     "CellInputTypeDef",
     "CellTypeDef",
     "ColumnMetadataTypeDef",
     "DataItemTypeDef",
+    "DelimitedTextImportOptionsOutputTypeDef",
     "DelimitedTextImportOptionsTypeDef",
     "DescribeTableDataImportJobRequestRequestTypeDef",
+    "SourceDataColumnPropertiesOutputTypeDef",
     "SourceDataColumnPropertiesTypeDef",
     "FilterTypeDef",
     "VariableValueTypeDef",
+    "ImportDataSourceConfigOutputTypeDef",
     "ImportDataSourceConfigTypeDef",
     "ImportJobSubmitterTypeDef",
     "InvokeScreenAutomationResultTypeDef",
     "ListTableColumnsRequestListTableColumnsPaginateTypeDef",
     "ListTableColumnsRequestRequestTypeDef",
     "TableColumnTypeDef",
     "ListTableRowsRequestListTableRowsPaginateTypeDef",
@@ -67,33 +70,36 @@
     "BatchDeleteTableRowsResultTypeDef",
     "BatchUpdateTableRowsResultTypeDef",
     "BatchUpsertTableRowsResultTypeDef",
     "CreateRowDataTypeDef",
     "UpdateRowDataTypeDef",
     "TableRowTypeDef",
     "ResultRowTypeDef",
+    "DestinationOptionsOutputTypeDef",
     "DestinationOptionsTypeDef",
     "QueryTableRowsRequestQueryTableRowsPaginateTypeDef",
     "QueryTableRowsRequestRequestTypeDef",
     "UpsertRowDataTypeDef",
     "GetScreenDataRequestRequestTypeDef",
     "InvokeScreenAutomationRequestRequestTypeDef",
+    "ImportDataSourceOutputTypeDef",
     "ImportDataSourceTypeDef",
     "ListTableColumnsResultTypeDef",
     "ListTablesResultTypeDef",
     "BatchCreateTableRowsRequestRequestTypeDef",
     "BatchUpdateTableRowsRequestRequestTypeDef",
     "ListTableRowsResultTypeDef",
     "QueryTableRowsResultTypeDef",
     "ResultSetTypeDef",
+    "ImportOptionsOutputTypeDef",
     "ImportOptionsTypeDef",
     "BatchUpsertTableRowsRequestRequestTypeDef",
     "GetScreenDataResultTypeDef",
-    "StartTableDataImportJobRequestRequestTypeDef",
     "TableDataImportJobMetadataTypeDef",
+    "StartTableDataImportJobRequestRequestTypeDef",
     "DescribeTableDataImportJobResultTypeDef",
 )
 
 FailedBatchItemTypeDef = TypedDict(
     "FailedBatchItemTypeDef",
     {
         "id": str,
@@ -166,14 +172,36 @@
         "overrideFormat": FormatType,
         "rawValue": str,
         "formattedValue": str,
     },
     total=False,
 )
 
+_RequiredDelimitedTextImportOptionsOutputTypeDef = TypedDict(
+    "_RequiredDelimitedTextImportOptionsOutputTypeDef",
+    {
+        "delimiter": str,
+    },
+)
+_OptionalDelimitedTextImportOptionsOutputTypeDef = TypedDict(
+    "_OptionalDelimitedTextImportOptionsOutputTypeDef",
+    {
+        "hasHeaderRow": bool,
+        "ignoreEmptyRows": bool,
+        "dataCharacterEncoding": ImportDataCharacterEncodingType,
+    },
+    total=False,
+)
+
+class DelimitedTextImportOptionsOutputTypeDef(
+    _RequiredDelimitedTextImportOptionsOutputTypeDef,
+    _OptionalDelimitedTextImportOptionsOutputTypeDef,
+):
+    pass
+
 _RequiredDelimitedTextImportOptionsTypeDef = TypedDict(
     "_RequiredDelimitedTextImportOptionsTypeDef",
     {
         "delimiter": str,
     },
 )
 _OptionalDelimitedTextImportOptionsTypeDef = TypedDict(
@@ -196,14 +224,22 @@
     {
         "workbookId": str,
         "tableId": str,
         "jobId": str,
     },
 )
 
+SourceDataColumnPropertiesOutputTypeDef = TypedDict(
+    "SourceDataColumnPropertiesOutputTypeDef",
+    {
+        "columnIndex": int,
+    },
+    total=False,
+)
+
 SourceDataColumnPropertiesTypeDef = TypedDict(
     "SourceDataColumnPropertiesTypeDef",
     {
         "columnIndex": int,
     },
     total=False,
 )
@@ -228,14 +264,22 @@
 VariableValueTypeDef = TypedDict(
     "VariableValueTypeDef",
     {
         "rawValue": str,
     },
 )
 
+ImportDataSourceConfigOutputTypeDef = TypedDict(
+    "ImportDataSourceConfigOutputTypeDef",
+    {
+        "dataSourceUrl": str,
+    },
+    total=False,
+)
+
 ImportDataSourceConfigTypeDef = TypedDict(
     "ImportDataSourceConfigTypeDef",
     {
         "dataSourceUrl": str,
     },
     total=False,
 )
@@ -537,18 +581,26 @@
     },
     total=False,
 )
 
 class ResultRowTypeDef(_RequiredResultRowTypeDef, _OptionalResultRowTypeDef):
     pass
 
+DestinationOptionsOutputTypeDef = TypedDict(
+    "DestinationOptionsOutputTypeDef",
+    {
+        "columnMap": Dict[str, SourceDataColumnPropertiesOutputTypeDef],
+    },
+    total=False,
+)
+
 DestinationOptionsTypeDef = TypedDict(
     "DestinationOptionsTypeDef",
     {
-        "columnMap": Dict[str, SourceDataColumnPropertiesTypeDef],
+        "columnMap": Mapping[str, SourceDataColumnPropertiesTypeDef],
     },
     total=False,
 )
 
 _RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
     "_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
     {
@@ -646,14 +698,21 @@
 
 class InvokeScreenAutomationRequestRequestTypeDef(
     _RequiredInvokeScreenAutomationRequestRequestTypeDef,
     _OptionalInvokeScreenAutomationRequestRequestTypeDef,
 ):
     pass
 
+ImportDataSourceOutputTypeDef = TypedDict(
+    "ImportDataSourceOutputTypeDef",
+    {
+        "dataSourceConfig": ImportDataSourceConfigOutputTypeDef,
+    },
+)
+
 ImportDataSourceTypeDef = TypedDict(
     "ImportDataSourceTypeDef",
     {
         "dataSourceConfig": ImportDataSourceConfigTypeDef,
     },
 )
 
@@ -748,14 +807,23 @@
     "ResultSetTypeDef",
     {
         "headers": List[ColumnMetadataTypeDef],
         "rows": List[ResultRowTypeDef],
     },
 )
 
+ImportOptionsOutputTypeDef = TypedDict(
+    "ImportOptionsOutputTypeDef",
+    {
+        "destinationOptions": DestinationOptionsOutputTypeDef,
+        "delimitedTextOptions": DelimitedTextImportOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 ImportOptionsTypeDef = TypedDict(
     "ImportOptionsTypeDef",
     {
         "destinationOptions": DestinationOptionsTypeDef,
         "delimitedTextOptions": DelimitedTextImportOptionsTypeDef,
     },
     total=False,
@@ -789,36 +857,36 @@
         "results": Dict[str, ResultSetTypeDef],
         "workbookCursor": int,
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TableDataImportJobMetadataTypeDef = TypedDict(
+    "TableDataImportJobMetadataTypeDef",
+    {
+        "submitter": ImportJobSubmitterTypeDef,
+        "submitTime": datetime,
+        "importOptions": ImportOptionsOutputTypeDef,
+        "dataSource": ImportDataSourceOutputTypeDef,
+    },
+)
+
 StartTableDataImportJobRequestRequestTypeDef = TypedDict(
     "StartTableDataImportJobRequestRequestTypeDef",
     {
         "workbookId": str,
         "dataSource": ImportDataSourceTypeDef,
         "dataFormat": Literal["DELIMITED_TEXT"],
         "destinationTableId": str,
         "importOptions": ImportOptionsTypeDef,
         "clientRequestToken": str,
     },
 )
 
-TableDataImportJobMetadataTypeDef = TypedDict(
-    "TableDataImportJobMetadataTypeDef",
-    {
-        "submitter": ImportJobSubmitterTypeDef,
-        "submitTime": datetime,
-        "importOptions": ImportOptionsTypeDef,
-        "dataSource": ImportDataSourceTypeDef,
-    },
-)
-
 DescribeTableDataImportJobResultTypeDef = TypedDict(
     "DescribeTableDataImportJobResultTypeDef",
     {
         "jobStatus": TableDataImportJobStatusType,
         "message": str,
         "jobMetadata": TableDataImportJobMetadataTypeDef,
         "errorCode": ErrorCodeType,
```

### Comparing `mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode.egg-info/PKG-INFO` & `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-honeycode
-Version: 1.28.0
-Summary: Type annotations for boto3.Honeycode 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Honeycode 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-honeycode"></a>
 
 # mypy-boto3-honeycode
 
 [![PyPI - mypy-boto3-honeycode](https://img.shields.io/pypi/v/mypy-boto3-honeycode.svg?color=blue)](https://pypi.org/project/mypy-boto3-honeycode)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-honeycode.svg?color=blue)](https://pypi.org/project/mypy-boto3-honeycode)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-honeycode?color=blue)](https://pypistats.org/packages/mypy-boto3-honeycode)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-honeycode)](https://pepy.tech/project/mypy-boto3-honeycode)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Honeycode 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
+[boto3.Honeycode 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
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
 [mypy-boto3-honeycode docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/).
 
 See how it helps to find and fix potential bugs:
 
@@ -342,19 +342,22 @@
     FailedBatchItemTypeDef,
     BatchDeleteTableRowsRequestRequestTypeDef,
     UpsertRowsResultTypeDef,
     CellInputTypeDef,
     CellTypeDef,
     ColumnMetadataTypeDef,
     DataItemTypeDef,
+    DelimitedTextImportOptionsOutputTypeDef,
     DelimitedTextImportOptionsTypeDef,
     DescribeTableDataImportJobRequestRequestTypeDef,
+    SourceDataColumnPropertiesOutputTypeDef,
     SourceDataColumnPropertiesTypeDef,
     FilterTypeDef,
     VariableValueTypeDef,
+    ImportDataSourceConfigOutputTypeDef,
     ImportDataSourceConfigTypeDef,
     ImportJobSubmitterTypeDef,
     InvokeScreenAutomationResultTypeDef,
     ListTableColumnsRequestListTableColumnsPaginateTypeDef,
     ListTableColumnsRequestRequestTypeDef,
     TableColumnTypeDef,
     ListTableRowsRequestListTableRowsPaginateTypeDef,
@@ -373,33 +376,36 @@
     BatchDeleteTableRowsResultTypeDef,
     BatchUpdateTableRowsResultTypeDef,
     BatchUpsertTableRowsResultTypeDef,
     CreateRowDataTypeDef,
     UpdateRowDataTypeDef,
     TableRowTypeDef,
     ResultRowTypeDef,
+    DestinationOptionsOutputTypeDef,
     DestinationOptionsTypeDef,
     QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     QueryTableRowsRequestRequestTypeDef,
     UpsertRowDataTypeDef,
     GetScreenDataRequestRequestTypeDef,
     InvokeScreenAutomationRequestRequestTypeDef,
+    ImportDataSourceOutputTypeDef,
     ImportDataSourceTypeDef,
     ListTableColumnsResultTypeDef,
     ListTablesResultTypeDef,
     BatchCreateTableRowsRequestRequestTypeDef,
     BatchUpdateTableRowsRequestRequestTypeDef,
     ListTableRowsResultTypeDef,
     QueryTableRowsResultTypeDef,
     ResultSetTypeDef,
+    ImportOptionsOutputTypeDef,
     ImportOptionsTypeDef,
     BatchUpsertTableRowsRequestRequestTypeDef,
     GetScreenDataResultTypeDef,
-    StartTableDataImportJobRequestRequestTypeDef,
     TableDataImportJobMetadataTypeDef,
+    StartTableDataImportJobRequestRequestTypeDef,
     DescribeTableDataImportJobResultTypeDef,
 )
 
 
 def get_structure() -> FailedBatchItemTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-honeycode-1.28.0/mypy_boto3_honeycode.egg-info/SOURCES.txt` & `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.0/setup.py` & `mypy-boto3-honeycode-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-honeycode",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_honeycode"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Honeycode 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Honeycode 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

