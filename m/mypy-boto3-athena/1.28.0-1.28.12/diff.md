# Comparing `tmp/mypy-boto3-athena-1.28.0.tar.gz` & `tmp/mypy-boto3-athena-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-athena-1.28.0.tar", last modified: Thu Jul  6 20:59:02 2023, max compression
+gzip compressed data, was "mypy-boto3-athena-1.28.12.tar", last modified: Thu Jul 27 05:34:20 2023, max compression
```

## Comparing `mypy-boto3-athena-1.28.0.tar` & `mypy-boto3-athena-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:02.094228 mypy-boto3-athena-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:33:47.000000 mypy-boto3-athena-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-07-06 20:59:02.090227 mypy-boto3-athena-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19434 2023-07-06 20:33:47.000000 mypy-boto3-athena-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:02.086228 mypy-boto3-athena-1.28.0/mypy_boto3_athena/
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-06 20:33:47.000000 mypy-boto3-athena-1.28.0/mypy_boto3_athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-06 20:33:47.000000 mypy-boto3-athena-1.28.0/mypy_boto3_athena/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-06 20:33:47.000000 mypy-boto3-athena-1.28.0/mypy_boto3_athena/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46117 2023-07-06 20:33:49.000000 mypy-boto3-athena-1.28.0/mypy_boto3_athena/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    46035 2023-07-06 20:33:47.000000 mypy-boto3-athena-1.28.0/mypy_boto3_athena/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-07-06 20:33:49.000000 mypy-boto3-athena-1.28.0/mypy_boto3_athena/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-07-06 20:33:49.000000 mypy-boto3-athena-1.28.0/mypy_boto3_athena/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-07-06 20:33:49.000000 mypy-boto3-athena-1.28.0/mypy_boto3_athena/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-07-06 20:33:49.000000 mypy-boto3-athena-1.28.0/mypy_boto3_athena/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:33:47.000000 mypy-boto3-athena-1.28.0/mypy_boto3_athena/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    62804 2023-07-06 20:33:51.000000 mypy-boto3-athena-1.28.0/mypy_boto3_athena/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    62715 2023-07-06 20:33:50.000000 mypy-boto3-athena-1.28.0/mypy_boto3_athena/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:33:47.000000 mypy-boto3-athena-1.28.0/mypy_boto3_athena/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:02.090227 mypy-boto3-athena-1.28.0/mypy_boto3_athena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-07-06 20:59:01.000000 mypy-boto3-athena-1.28.0/mypy_boto3_athena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-06 20:59:01.000000 mypy-boto3-athena-1.28.0/mypy_boto3_athena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:01.000000 mypy-boto3-athena-1.28.0/mypy_boto3_athena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:01.000000 mypy-boto3-athena-1.28.0/mypy_boto3_athena.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:01.000000 mypy-boto3-athena-1.28.0/mypy_boto3_athena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 20:59:01.000000 mypy-boto3-athena-1.28.0/mypy_boto3_athena.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:02.094228 mypy-boto3-athena-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-06 20:33:47.000000 mypy-boto3-athena-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.584572 mypy-boto3-athena-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21381 2023-07-27 05:34:20.584572 mypy-boto3-athena-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19898 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.580572 mypy-boto3-athena-1.28.12/mypy_boto3_athena/
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46117 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46035 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10516 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    67186 2023-07-27 05:17:43.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67091 2023-07-27 05:17:42.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.584572 mypy-boto3-athena-1.28.12/mypy_boto3_athena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21381 2023-07-27 05:34:20.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 05:34:20.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:20.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 05:34:20.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:20.584572 mypy-boto3-athena-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/setup.py
```

### Comparing `mypy-boto3-athena-1.28.0/LICENSE` & `mypy-boto3-athena-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.0/PKG-INFO` & `mypy-boto3-athena-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-athena
-Version: 1.28.0
-Summary: Type annotations for boto3.Athena 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Athena 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-athena"></a>
 
 # mypy-boto3-athena
 
 [![PyPI - mypy-boto3-athena](https://img.shields.io/pypi/v/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-athena?color=blue)](https://pypistats.org/packages/mypy-boto3-athena)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-athena)](https://pepy.tech/project/mypy-boto3-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Athena 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[boto3.Athena 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
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
 [mypy-boto3-athena docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,14 +358,15 @@
 ### Typed dictionaries
 
 `mypy_boto3_athena.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_athena.type_defs import (
+    AclConfigurationOutputTypeDef,
     AclConfigurationTypeDef,
     ApplicationDPUSizesTypeDef,
     AthenaErrorTypeDef,
     BatchGetNamedQueryInputRequestTypeDef,
     NamedQueryTypeDef,
     UnprocessedNamedQueryIdTypeDef,
     BatchGetPreparedStatementInputRequestTypeDef,
@@ -375,38 +376,43 @@
     UnprocessedQueryExecutionIdTypeDef,
     CalculationConfigurationTypeDef,
     CalculationResultTypeDef,
     CalculationStatisticsTypeDef,
     CalculationStatusTypeDef,
     CancelCapacityReservationInputRequestTypeDef,
     CapacityAllocationTypeDef,
+    CapacityAssignmentOutputTypeDef,
     CapacityAssignmentTypeDef,
     ColumnInfoTypeDef,
     ColumnTypeDef,
     TagTypeDef,
     CreateNamedQueryInputRequestTypeDef,
     CreateNamedQueryOutputTypeDef,
     CreateNotebookInputRequestTypeDef,
     CreateNotebookOutputTypeDef,
     CreatePreparedStatementInputRequestTypeDef,
     CreatePresignedNotebookUrlRequestRequestTypeDef,
     CreatePresignedNotebookUrlResponseTypeDef,
+    CustomerContentEncryptionConfigurationOutputTypeDef,
     CustomerContentEncryptionConfigurationTypeDef,
     DataCatalogSummaryTypeDef,
     DataCatalogTypeDef,
     DatabaseTypeDef,
     DatumTypeDef,
     DeleteCapacityReservationInputRequestTypeDef,
     DeleteDataCatalogInputRequestTypeDef,
     DeleteNamedQueryInputRequestTypeDef,
     DeleteNotebookInputRequestTypeDef,
     DeletePreparedStatementInputRequestTypeDef,
     DeleteWorkGroupInputRequestTypeDef,
+    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
+    EngineConfigurationOutputTypeDef,
     EngineConfigurationTypeDef,
+    EngineVersionOutputTypeDef,
     EngineVersionTypeDef,
     ExecutorsSummaryTypeDef,
     ExportNotebookInputRequestTypeDef,
     NotebookMetadataTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeRequestRequestTypeDef,
     GetCalculationExecutionCodeResponseTypeDef,
@@ -451,23 +457,26 @@
     ListQueryExecutionsInputRequestTypeDef,
     ListQueryExecutionsOutputTypeDef,
     ListSessionsRequestRequestTypeDef,
     ListTableMetadataInputListTableMetadataPaginateTypeDef,
     ListTableMetadataInputRequestTypeDef,
     ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    TagOutputTypeDef,
     ListWorkGroupsInputRequestTypeDef,
     PaginatorConfigTypeDef,
+    QueryExecutionContextOutputTypeDef,
     QueryExecutionContextTypeDef,
     ResultReuseInformationTypeDef,
     QueryRuntimeStatisticsRowsTypeDef,
     QueryRuntimeStatisticsTimelineTypeDef,
     QueryStagePlanNodeTypeDef,
     QueryStageTypeDef,
     ResponseMetadataTypeDef,
+    ResultReuseByAgeConfigurationOutputTypeDef,
     ResultReuseByAgeConfigurationTypeDef,
     StartCalculationExecutionResponseTypeDef,
     StartQueryExecutionOutputTypeDef,
     StartSessionResponseTypeDef,
     StopCalculationExecutionRequestRequestTypeDef,
     StopCalculationExecutionResponseTypeDef,
     StopQueryExecutionInputRequestTypeDef,
@@ -493,65 +502,68 @@
     CapacityReservationTypeDef,
     CapacityAssignmentConfigurationTypeDef,
     PutCapacityAssignmentConfigurationInputRequestTypeDef,
     ResultSetMetadataTypeDef,
     TableMetadataTypeDef,
     CreateCapacityReservationInputRequestTypeDef,
     CreateDataCatalogInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ListDataCatalogsOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetDatabaseOutputTypeDef,
     ListDatabasesOutputTypeDef,
     RowTypeDef,
+    ResultConfigurationOutputTypeDef,
+    SessionConfigurationTypeDef,
     ResultConfigurationTypeDef,
     ResultConfigurationUpdatesTypeDef,
-    SessionConfigurationTypeDef,
     StartSessionRequestRequestTypeDef,
     ListEngineVersionsOutputTypeDef,
     WorkGroupSummaryTypeDef,
     ListExecutorsResponseTypeDef,
     ExportNotebookOutputTypeDef,
     GetNotebookMetadataOutputTypeDef,
     ListNotebookMetadataOutputTypeDef,
     ListNotebookMetadataInputRequestTypeDef,
     GetSessionStatusResponseTypeDef,
     SessionSummaryTypeDef,
     ListNotebookSessionsResponseTypeDef,
     ListPreparedStatementsOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     QueryExecutionStatisticsTypeDef,
     QueryRuntimeStatisticsTypeDef,
+    ResultReuseConfigurationOutputTypeDef,
     ResultReuseConfigurationTypeDef,
     ListCalculationExecutionsResponseTypeDef,
     GetCapacityReservationOutputTypeDef,
     ListCapacityReservationsOutputTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
     GetTableMetadataOutputTypeDef,
     ListTableMetadataOutputTypeDef,
     ResultSetTypeDef,
+    WorkGroupConfigurationOutputTypeDef,
+    GetSessionResponseTypeDef,
     WorkGroupConfigurationTypeDef,
     WorkGroupConfigurationUpdatesTypeDef,
-    GetSessionResponseTypeDef,
     ListWorkGroupsOutputTypeDef,
     ListSessionsResponseTypeDef,
     GetQueryRuntimeStatisticsOutputTypeDef,
     QueryExecutionTypeDef,
     StartQueryExecutionInputRequestTypeDef,
     GetQueryResultsOutputTypeDef,
-    CreateWorkGroupInputRequestTypeDef,
     WorkGroupTypeDef,
+    CreateWorkGroupInputRequestTypeDef,
     UpdateWorkGroupInputRequestTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     GetQueryExecutionOutputTypeDef,
     GetWorkGroupOutputTypeDef,
 )
 
 
-def get_structure() -> AclConfigurationTypeDef:
+def get_structure() -> AclConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-athena-1.28.0/README.md` & `mypy-boto3-athena-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-athena"></a>
 
 # mypy-boto3-athena
 
 [![PyPI - mypy-boto3-athena](https://img.shields.io/pypi/v/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-athena?color=blue)](https://pypistats.org/packages/mypy-boto3-athena)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-athena)](https://pepy.tech/project/mypy-boto3-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Athena 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[boto3.Athena 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
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
 [mypy-boto3-athena docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,14 +326,15 @@
 ### Typed dictionaries
 
 `mypy_boto3_athena.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_athena.type_defs import (
+    AclConfigurationOutputTypeDef,
     AclConfigurationTypeDef,
     ApplicationDPUSizesTypeDef,
     AthenaErrorTypeDef,
     BatchGetNamedQueryInputRequestTypeDef,
     NamedQueryTypeDef,
     UnprocessedNamedQueryIdTypeDef,
     BatchGetPreparedStatementInputRequestTypeDef,
@@ -343,38 +344,43 @@
     UnprocessedQueryExecutionIdTypeDef,
     CalculationConfigurationTypeDef,
     CalculationResultTypeDef,
     CalculationStatisticsTypeDef,
     CalculationStatusTypeDef,
     CancelCapacityReservationInputRequestTypeDef,
     CapacityAllocationTypeDef,
+    CapacityAssignmentOutputTypeDef,
     CapacityAssignmentTypeDef,
     ColumnInfoTypeDef,
     ColumnTypeDef,
     TagTypeDef,
     CreateNamedQueryInputRequestTypeDef,
     CreateNamedQueryOutputTypeDef,
     CreateNotebookInputRequestTypeDef,
     CreateNotebookOutputTypeDef,
     CreatePreparedStatementInputRequestTypeDef,
     CreatePresignedNotebookUrlRequestRequestTypeDef,
     CreatePresignedNotebookUrlResponseTypeDef,
+    CustomerContentEncryptionConfigurationOutputTypeDef,
     CustomerContentEncryptionConfigurationTypeDef,
     DataCatalogSummaryTypeDef,
     DataCatalogTypeDef,
     DatabaseTypeDef,
     DatumTypeDef,
     DeleteCapacityReservationInputRequestTypeDef,
     DeleteDataCatalogInputRequestTypeDef,
     DeleteNamedQueryInputRequestTypeDef,
     DeleteNotebookInputRequestTypeDef,
     DeletePreparedStatementInputRequestTypeDef,
     DeleteWorkGroupInputRequestTypeDef,
+    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
+    EngineConfigurationOutputTypeDef,
     EngineConfigurationTypeDef,
+    EngineVersionOutputTypeDef,
     EngineVersionTypeDef,
     ExecutorsSummaryTypeDef,
     ExportNotebookInputRequestTypeDef,
     NotebookMetadataTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeRequestRequestTypeDef,
     GetCalculationExecutionCodeResponseTypeDef,
@@ -419,23 +425,26 @@
     ListQueryExecutionsInputRequestTypeDef,
     ListQueryExecutionsOutputTypeDef,
     ListSessionsRequestRequestTypeDef,
     ListTableMetadataInputListTableMetadataPaginateTypeDef,
     ListTableMetadataInputRequestTypeDef,
     ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    TagOutputTypeDef,
     ListWorkGroupsInputRequestTypeDef,
     PaginatorConfigTypeDef,
+    QueryExecutionContextOutputTypeDef,
     QueryExecutionContextTypeDef,
     ResultReuseInformationTypeDef,
     QueryRuntimeStatisticsRowsTypeDef,
     QueryRuntimeStatisticsTimelineTypeDef,
     QueryStagePlanNodeTypeDef,
     QueryStageTypeDef,
     ResponseMetadataTypeDef,
+    ResultReuseByAgeConfigurationOutputTypeDef,
     ResultReuseByAgeConfigurationTypeDef,
     StartCalculationExecutionResponseTypeDef,
     StartQueryExecutionOutputTypeDef,
     StartSessionResponseTypeDef,
     StopCalculationExecutionRequestRequestTypeDef,
     StopCalculationExecutionResponseTypeDef,
     StopQueryExecutionInputRequestTypeDef,
@@ -461,65 +470,68 @@
     CapacityReservationTypeDef,
     CapacityAssignmentConfigurationTypeDef,
     PutCapacityAssignmentConfigurationInputRequestTypeDef,
     ResultSetMetadataTypeDef,
     TableMetadataTypeDef,
     CreateCapacityReservationInputRequestTypeDef,
     CreateDataCatalogInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ListDataCatalogsOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetDatabaseOutputTypeDef,
     ListDatabasesOutputTypeDef,
     RowTypeDef,
+    ResultConfigurationOutputTypeDef,
+    SessionConfigurationTypeDef,
     ResultConfigurationTypeDef,
     ResultConfigurationUpdatesTypeDef,
-    SessionConfigurationTypeDef,
     StartSessionRequestRequestTypeDef,
     ListEngineVersionsOutputTypeDef,
     WorkGroupSummaryTypeDef,
     ListExecutorsResponseTypeDef,
     ExportNotebookOutputTypeDef,
     GetNotebookMetadataOutputTypeDef,
     ListNotebookMetadataOutputTypeDef,
     ListNotebookMetadataInputRequestTypeDef,
     GetSessionStatusResponseTypeDef,
     SessionSummaryTypeDef,
     ListNotebookSessionsResponseTypeDef,
     ListPreparedStatementsOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     QueryExecutionStatisticsTypeDef,
     QueryRuntimeStatisticsTypeDef,
+    ResultReuseConfigurationOutputTypeDef,
     ResultReuseConfigurationTypeDef,
     ListCalculationExecutionsResponseTypeDef,
     GetCapacityReservationOutputTypeDef,
     ListCapacityReservationsOutputTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
     GetTableMetadataOutputTypeDef,
     ListTableMetadataOutputTypeDef,
     ResultSetTypeDef,
+    WorkGroupConfigurationOutputTypeDef,
+    GetSessionResponseTypeDef,
     WorkGroupConfigurationTypeDef,
     WorkGroupConfigurationUpdatesTypeDef,
-    GetSessionResponseTypeDef,
     ListWorkGroupsOutputTypeDef,
     ListSessionsResponseTypeDef,
     GetQueryRuntimeStatisticsOutputTypeDef,
     QueryExecutionTypeDef,
     StartQueryExecutionInputRequestTypeDef,
     GetQueryResultsOutputTypeDef,
-    CreateWorkGroupInputRequestTypeDef,
     WorkGroupTypeDef,
+    CreateWorkGroupInputRequestTypeDef,
     UpdateWorkGroupInputRequestTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     GetQueryExecutionOutputTypeDef,
     GetWorkGroupOutputTypeDef,
 )
 
 
-def get_structure() -> AclConfigurationTypeDef:
+def get_structure() -> AclConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-athena-1.28.0/mypy_boto3_athena/__init__.py` & `mypy-boto3-athena-1.28.12/mypy_boto3_athena/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.0/mypy_boto3_athena/__init__.pyi` & `mypy-boto3-athena-1.28.12/mypy_boto3_athena/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.0/mypy_boto3_athena/__main__.py` & `mypy-boto3-athena-1.28.12/mypy_boto3_athena/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Athena 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Athena 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena\nOther"
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

### Comparing `mypy-boto3-athena-1.28.0/mypy_boto3_athena/client.py` & `mypy-boto3-athena-1.28.12/mypy_boto3_athena/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.0/mypy_boto3_athena/client.pyi` & `mypy-boto3-athena-1.28.12/mypy_boto3_athena/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.0/mypy_boto3_athena/literals.py` & `mypy-boto3-athena-1.28.12/mypy_boto3_athena/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "CalculationExecutionStateType",
     "CapacityAllocationStatusType",
     "CapacityReservationStatusType",
     "ColumnNullableType",
     "DataCatalogTypeType",
     "EncryptionOptionType",
@@ -44,15 +43,14 @@
     "AthenaServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 CalculationExecutionStateType = Literal[
     "CANCELED", "CANCELING", "COMPLETED", "CREATED", "CREATING", "FAILED", "QUEUED", "RUNNING"
 ]
 CapacityAllocationStatusType = Literal["FAILED", "PENDING", "SUCCEEDED"]
 CapacityReservationStatusType = Literal[
     "ACTIVE", "CANCELLED", "CANCELLING", "FAILED", "PENDING", "UPDATE_PENDING"
 ]
@@ -194,14 +192,15 @@
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
@@ -280,26 +279,28 @@
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

### Comparing `mypy-boto3-athena-1.28.0/mypy_boto3_athena/literals.pyi` & `mypy-boto3-athena-1.28.12/mypy_boto3_athena/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "CalculationExecutionStateType",
     "CapacityAllocationStatusType",
     "CapacityReservationStatusType",
     "ColumnNullableType",
     "DataCatalogTypeType",
     "EncryptionOptionType",
@@ -43,14 +44,15 @@
     "AthenaServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 CalculationExecutionStateType = Literal[
     "CANCELED", "CANCELING", "COMPLETED", "CREATED", "CREATING", "FAILED", "QUEUED", "RUNNING"
 ]
 CapacityAllocationStatusType = Literal["FAILED", "PENDING", "SUCCEEDED"]
 CapacityReservationStatusType = Literal[
     "ACTIVE", "CANCELLED", "CANCELLING", "FAILED", "PENDING", "UPDATE_PENDING"
 ]
@@ -192,14 +194,15 @@
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
@@ -278,26 +281,28 @@
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

### Comparing `mypy-boto3-athena-1.28.0/mypy_boto3_athena/paginator.py` & `mypy-boto3-athena-1.28.12/mypy_boto3_athena/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.0/mypy_boto3_athena/paginator.pyi` & `mypy-boto3-athena-1.28.12/mypy_boto3_athena/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.0/mypy_boto3_athena/type_defs.py` & `mypy-boto3-athena-1.28.12/mypy_boto3_athena/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for athena service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_athena.type_defs import AclConfigurationTypeDef
+    from mypy_boto3_athena.type_defs import AclConfigurationOutputTypeDef
 
-    data: AclConfigurationTypeDef = {...}
+    data: AclConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -37,14 +37,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AclConfigurationOutputTypeDef",
     "AclConfigurationTypeDef",
     "ApplicationDPUSizesTypeDef",
     "AthenaErrorTypeDef",
     "BatchGetNamedQueryInputRequestTypeDef",
     "NamedQueryTypeDef",
     "UnprocessedNamedQueryIdTypeDef",
     "BatchGetPreparedStatementInputRequestTypeDef",
@@ -54,38 +55,43 @@
     "UnprocessedQueryExecutionIdTypeDef",
     "CalculationConfigurationTypeDef",
     "CalculationResultTypeDef",
     "CalculationStatisticsTypeDef",
     "CalculationStatusTypeDef",
     "CancelCapacityReservationInputRequestTypeDef",
     "CapacityAllocationTypeDef",
+    "CapacityAssignmentOutputTypeDef",
     "CapacityAssignmentTypeDef",
     "ColumnInfoTypeDef",
     "ColumnTypeDef",
     "TagTypeDef",
     "CreateNamedQueryInputRequestTypeDef",
     "CreateNamedQueryOutputTypeDef",
     "CreateNotebookInputRequestTypeDef",
     "CreateNotebookOutputTypeDef",
     "CreatePreparedStatementInputRequestTypeDef",
     "CreatePresignedNotebookUrlRequestRequestTypeDef",
     "CreatePresignedNotebookUrlResponseTypeDef",
+    "CustomerContentEncryptionConfigurationOutputTypeDef",
     "CustomerContentEncryptionConfigurationTypeDef",
     "DataCatalogSummaryTypeDef",
     "DataCatalogTypeDef",
     "DatabaseTypeDef",
     "DatumTypeDef",
     "DeleteCapacityReservationInputRequestTypeDef",
     "DeleteDataCatalogInputRequestTypeDef",
     "DeleteNamedQueryInputRequestTypeDef",
     "DeleteNotebookInputRequestTypeDef",
     "DeletePreparedStatementInputRequestTypeDef",
     "DeleteWorkGroupInputRequestTypeDef",
+    "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
+    "EngineConfigurationOutputTypeDef",
     "EngineConfigurationTypeDef",
+    "EngineVersionOutputTypeDef",
     "EngineVersionTypeDef",
     "ExecutorsSummaryTypeDef",
     "ExportNotebookInputRequestTypeDef",
     "NotebookMetadataTypeDef",
     "FilterDefinitionTypeDef",
     "GetCalculationExecutionCodeRequestRequestTypeDef",
     "GetCalculationExecutionCodeResponseTypeDef",
@@ -130,23 +136,26 @@
     "ListQueryExecutionsInputRequestTypeDef",
     "ListQueryExecutionsOutputTypeDef",
     "ListSessionsRequestRequestTypeDef",
     "ListTableMetadataInputListTableMetadataPaginateTypeDef",
     "ListTableMetadataInputRequestTypeDef",
     "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "TagOutputTypeDef",
     "ListWorkGroupsInputRequestTypeDef",
     "PaginatorConfigTypeDef",
+    "QueryExecutionContextOutputTypeDef",
     "QueryExecutionContextTypeDef",
     "ResultReuseInformationTypeDef",
     "QueryRuntimeStatisticsRowsTypeDef",
     "QueryRuntimeStatisticsTimelineTypeDef",
     "QueryStagePlanNodeTypeDef",
     "QueryStageTypeDef",
     "ResponseMetadataTypeDef",
+    "ResultReuseByAgeConfigurationOutputTypeDef",
     "ResultReuseByAgeConfigurationTypeDef",
     "StartCalculationExecutionResponseTypeDef",
     "StartQueryExecutionOutputTypeDef",
     "StartSessionResponseTypeDef",
     "StopCalculationExecutionRequestRequestTypeDef",
     "StopCalculationExecutionResponseTypeDef",
     "StopQueryExecutionInputRequestTypeDef",
@@ -172,63 +181,73 @@
     "CapacityReservationTypeDef",
     "CapacityAssignmentConfigurationTypeDef",
     "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     "ResultSetMetadataTypeDef",
     "TableMetadataTypeDef",
     "CreateCapacityReservationInputRequestTypeDef",
     "CreateDataCatalogInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ListDataCatalogsOutputTypeDef",
     "GetDataCatalogOutputTypeDef",
     "GetDatabaseOutputTypeDef",
     "ListDatabasesOutputTypeDef",
     "RowTypeDef",
+    "ResultConfigurationOutputTypeDef",
+    "SessionConfigurationTypeDef",
     "ResultConfigurationTypeDef",
     "ResultConfigurationUpdatesTypeDef",
-    "SessionConfigurationTypeDef",
     "StartSessionRequestRequestTypeDef",
     "ListEngineVersionsOutputTypeDef",
     "WorkGroupSummaryTypeDef",
     "ListExecutorsResponseTypeDef",
     "ExportNotebookOutputTypeDef",
     "GetNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataInputRequestTypeDef",
     "GetSessionStatusResponseTypeDef",
     "SessionSummaryTypeDef",
     "ListNotebookSessionsResponseTypeDef",
     "ListPreparedStatementsOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "QueryExecutionStatisticsTypeDef",
     "QueryRuntimeStatisticsTypeDef",
+    "ResultReuseConfigurationOutputTypeDef",
     "ResultReuseConfigurationTypeDef",
     "ListCalculationExecutionsResponseTypeDef",
     "GetCapacityReservationOutputTypeDef",
     "ListCapacityReservationsOutputTypeDef",
     "GetCapacityAssignmentConfigurationOutputTypeDef",
     "GetTableMetadataOutputTypeDef",
     "ListTableMetadataOutputTypeDef",
     "ResultSetTypeDef",
+    "WorkGroupConfigurationOutputTypeDef",
+    "GetSessionResponseTypeDef",
     "WorkGroupConfigurationTypeDef",
     "WorkGroupConfigurationUpdatesTypeDef",
-    "GetSessionResponseTypeDef",
     "ListWorkGroupsOutputTypeDef",
     "ListSessionsResponseTypeDef",
     "GetQueryRuntimeStatisticsOutputTypeDef",
     "QueryExecutionTypeDef",
     "StartQueryExecutionInputRequestTypeDef",
     "GetQueryResultsOutputTypeDef",
-    "CreateWorkGroupInputRequestTypeDef",
     "WorkGroupTypeDef",
+    "CreateWorkGroupInputRequestTypeDef",
     "UpdateWorkGroupInputRequestTypeDef",
     "BatchGetQueryExecutionOutputTypeDef",
     "GetQueryExecutionOutputTypeDef",
     "GetWorkGroupOutputTypeDef",
 )
 
+AclConfigurationOutputTypeDef = TypedDict(
+    "AclConfigurationOutputTypeDef",
+    {
+        "S3AclOption": Literal["BUCKET_OWNER_FULL_CONTROL"],
+    },
+)
+
 AclConfigurationTypeDef = TypedDict(
     "AclConfigurationTypeDef",
     {
         "S3AclOption": Literal["BUCKET_OWNER_FULL_CONTROL"],
     },
 )
 
@@ -404,18 +423,26 @@
 
 class CapacityAllocationTypeDef(
     _RequiredCapacityAllocationTypeDef, _OptionalCapacityAllocationTypeDef
 ):
     pass
 
 
+CapacityAssignmentOutputTypeDef = TypedDict(
+    "CapacityAssignmentOutputTypeDef",
+    {
+        "WorkGroupNames": List[str],
+    },
+    total=False,
+)
+
 CapacityAssignmentTypeDef = TypedDict(
     "CapacityAssignmentTypeDef",
     {
-        "WorkGroupNames": List[str],
+        "WorkGroupNames": Sequence[str],
     },
     total=False,
 )
 
 _RequiredColumnInfoTypeDef = TypedDict(
     "_RequiredColumnInfoTypeDef",
     {
@@ -572,14 +599,21 @@
         "NotebookUrl": str,
         "AuthToken": str,
         "AuthTokenExpirationTime": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CustomerContentEncryptionConfigurationOutputTypeDef = TypedDict(
+    "CustomerContentEncryptionConfigurationOutputTypeDef",
+    {
+        "KmsKey": str,
+    },
+)
+
 CustomerContentEncryptionConfigurationTypeDef = TypedDict(
     "CustomerContentEncryptionConfigurationTypeDef",
     {
         "KmsKey": str,
     },
 )
 
@@ -694,14 +728,35 @@
 
 class DeleteWorkGroupInputRequestTypeDef(
     _RequiredDeleteWorkGroupInputRequestTypeDef, _OptionalDeleteWorkGroupInputRequestTypeDef
 ):
     pass
 
 
+_RequiredEncryptionConfigurationOutputTypeDef = TypedDict(
+    "_RequiredEncryptionConfigurationOutputTypeDef",
+    {
+        "EncryptionOption": EncryptionOptionType,
+    },
+)
+_OptionalEncryptionConfigurationOutputTypeDef = TypedDict(
+    "_OptionalEncryptionConfigurationOutputTypeDef",
+    {
+        "KmsKey": str,
+    },
+    total=False,
+)
+
+
+class EncryptionConfigurationOutputTypeDef(
+    _RequiredEncryptionConfigurationOutputTypeDef, _OptionalEncryptionConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredEncryptionConfigurationTypeDef = TypedDict(
     "_RequiredEncryptionConfigurationTypeDef",
     {
         "EncryptionOption": EncryptionOptionType,
     },
 )
 _OptionalEncryptionConfigurationTypeDef = TypedDict(
@@ -715,38 +770,71 @@
 
 class EncryptionConfigurationTypeDef(
     _RequiredEncryptionConfigurationTypeDef, _OptionalEncryptionConfigurationTypeDef
 ):
     pass
 
 
+_RequiredEngineConfigurationOutputTypeDef = TypedDict(
+    "_RequiredEngineConfigurationOutputTypeDef",
+    {
+        "MaxConcurrentDpus": int,
+    },
+)
+_OptionalEngineConfigurationOutputTypeDef = TypedDict(
+    "_OptionalEngineConfigurationOutputTypeDef",
+    {
+        "CoordinatorDpuSize": int,
+        "DefaultExecutorDpuSize": int,
+        "AdditionalConfigs": Dict[str, str],
+        "SparkProperties": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class EngineConfigurationOutputTypeDef(
+    _RequiredEngineConfigurationOutputTypeDef, _OptionalEngineConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredEngineConfigurationTypeDef = TypedDict(
     "_RequiredEngineConfigurationTypeDef",
     {
         "MaxConcurrentDpus": int,
     },
 )
 _OptionalEngineConfigurationTypeDef = TypedDict(
     "_OptionalEngineConfigurationTypeDef",
     {
         "CoordinatorDpuSize": int,
         "DefaultExecutorDpuSize": int,
-        "AdditionalConfigs": Dict[str, str],
-        "SparkProperties": Dict[str, str],
+        "AdditionalConfigs": Mapping[str, str],
+        "SparkProperties": Mapping[str, str],
     },
     total=False,
 )
 
 
 class EngineConfigurationTypeDef(
     _RequiredEngineConfigurationTypeDef, _OptionalEngineConfigurationTypeDef
 ):
     pass
 
 
+EngineVersionOutputTypeDef = TypedDict(
+    "EngineVersionOutputTypeDef",
+    {
+        "SelectedEngineVersion": str,
+        "EffectiveEngineVersion": str,
+    },
+    total=False,
+)
+
 EngineVersionTypeDef = TypedDict(
     "EngineVersionTypeDef",
     {
         "SelectedEngineVersion": str,
         "EffectiveEngineVersion": str,
     },
     total=False,
@@ -1390,14 +1478,23 @@
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 ListWorkGroupsInputRequestTypeDef = TypedDict(
     "ListWorkGroupsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1409,14 +1506,23 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+QueryExecutionContextOutputTypeDef = TypedDict(
+    "QueryExecutionContextOutputTypeDef",
+    {
+        "Database": str,
+        "Catalog": str,
+    },
+    total=False,
+)
+
 QueryExecutionContextTypeDef = TypedDict(
     "QueryExecutionContextTypeDef",
     {
         "Database": str,
         "Catalog": str,
     },
     total=False,
@@ -1486,14 +1592,36 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+_RequiredResultReuseByAgeConfigurationOutputTypeDef = TypedDict(
+    "_RequiredResultReuseByAgeConfigurationOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalResultReuseByAgeConfigurationOutputTypeDef = TypedDict(
+    "_OptionalResultReuseByAgeConfigurationOutputTypeDef",
+    {
+        "MaxAgeInMinutes": int,
+    },
+    total=False,
+)
+
+
+class ResultReuseByAgeConfigurationOutputTypeDef(
+    _RequiredResultReuseByAgeConfigurationOutputTypeDef,
+    _OptionalResultReuseByAgeConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredResultReuseByAgeConfigurationTypeDef = TypedDict(
     "_RequiredResultReuseByAgeConfigurationTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalResultReuseByAgeConfigurationTypeDef = TypedDict(
@@ -1846,15 +1974,15 @@
     pass
 
 
 CapacityAssignmentConfigurationTypeDef = TypedDict(
     "CapacityAssignmentConfigurationTypeDef",
     {
         "CapacityReservationName": str,
-        "CapacityAssignments": List[CapacityAssignmentTypeDef],
+        "CapacityAssignments": List[CapacityAssignmentOutputTypeDef],
     },
     total=False,
 )
 
 PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
     "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     {
@@ -1938,23 +2066,14 @@
 
 class CreateDataCatalogInputRequestTypeDef(
     _RequiredCreateDataCatalogInputRequestTypeDef, _OptionalCreateDataCatalogInputRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1997,14 +2116,36 @@
     "RowTypeDef",
     {
         "Data": List[DatumTypeDef],
     },
     total=False,
 )
 
+ResultConfigurationOutputTypeDef = TypedDict(
+    "ResultConfigurationOutputTypeDef",
+    {
+        "OutputLocation": str,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "ExpectedBucketOwner": str,
+        "AclConfiguration": AclConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+SessionConfigurationTypeDef = TypedDict(
+    "SessionConfigurationTypeDef",
+    {
+        "ExecutionRole": str,
+        "WorkingDirectory": str,
+        "IdleTimeoutSeconds": int,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ResultConfigurationTypeDef = TypedDict(
     "ResultConfigurationTypeDef",
     {
         "OutputLocation": str,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "ExpectedBucketOwner": str,
         "AclConfiguration": AclConfigurationTypeDef,
@@ -2023,25 +2164,14 @@
         "RemoveExpectedBucketOwner": bool,
         "AclConfiguration": AclConfigurationTypeDef,
         "RemoveAclConfiguration": bool,
     },
     total=False,
 )
 
-SessionConfigurationTypeDef = TypedDict(
-    "SessionConfigurationTypeDef",
-    {
-        "ExecutionRole": str,
-        "WorkingDirectory": str,
-        "IdleTimeoutSeconds": int,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredStartSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSessionRequestRequestTypeDef",
     {
         "WorkGroup": str,
         "EngineConfiguration": EngineConfigurationTypeDef,
     },
 )
@@ -2062,28 +2192,28 @@
 ):
     pass
 
 
 ListEngineVersionsOutputTypeDef = TypedDict(
     "ListEngineVersionsOutputTypeDef",
     {
-        "EngineVersions": List[EngineVersionTypeDef],
+        "EngineVersions": List[EngineVersionOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WorkGroupSummaryTypeDef = TypedDict(
     "WorkGroupSummaryTypeDef",
     {
         "Name": str,
         "State": WorkGroupStateType,
         "Description": str,
         "CreationTime": datetime,
-        "EngineVersion": EngineVersionTypeDef,
+        "EngineVersion": EngineVersionOutputTypeDef,
     },
     total=False,
 )
 
 ListExecutorsResponseTypeDef = TypedDict(
     "ListExecutorsResponseTypeDef",
     {
@@ -2154,15 +2284,15 @@
 )
 
 SessionSummaryTypeDef = TypedDict(
     "SessionSummaryTypeDef",
     {
         "SessionId": str,
         "Description": str,
-        "EngineVersion": EngineVersionTypeDef,
+        "EngineVersion": EngineVersionOutputTypeDef,
         "NotebookVersion": str,
         "Status": SessionStatusTypeDef,
     },
     total=False,
 )
 
 ListNotebookSessionsResponseTypeDef = TypedDict(
@@ -2179,14 +2309,23 @@
     {
         "PreparedStatements": List[PreparedStatementSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 QueryExecutionStatisticsTypeDef = TypedDict(
     "QueryExecutionStatisticsTypeDef",
     {
         "EngineExecutionTimeInMillis": int,
         "DataScannedInBytes": int,
         "DataManifestLocation": str,
         "TotalExecutionTimeInMillis": int,
@@ -2204,14 +2343,22 @@
         "Timeline": QueryRuntimeStatisticsTimelineTypeDef,
         "Rows": QueryRuntimeStatisticsRowsTypeDef,
         "OutputStage": "QueryStageTypeDef",
     },
     total=False,
 )
 
+ResultReuseConfigurationOutputTypeDef = TypedDict(
+    "ResultReuseConfigurationOutputTypeDef",
+    {
+        "ResultReuseByAgeConfiguration": ResultReuseByAgeConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ResultReuseConfigurationTypeDef = TypedDict(
     "ResultReuseConfigurationTypeDef",
     {
         "ResultReuseByAgeConfiguration": ResultReuseByAgeConfigurationTypeDef,
     },
     total=False,
 )
@@ -2272,14 +2419,49 @@
     {
         "Rows": List[RowTypeDef],
         "ResultSetMetadata": ResultSetMetadataTypeDef,
     },
     total=False,
 )
 
+WorkGroupConfigurationOutputTypeDef = TypedDict(
+    "WorkGroupConfigurationOutputTypeDef",
+    {
+        "ResultConfiguration": ResultConfigurationOutputTypeDef,
+        "EnforceWorkGroupConfiguration": bool,
+        "PublishCloudWatchMetricsEnabled": bool,
+        "BytesScannedCutoffPerQuery": int,
+        "RequesterPaysEnabled": bool,
+        "EngineVersion": EngineVersionOutputTypeDef,
+        "AdditionalConfiguration": str,
+        "ExecutionRole": str,
+        "CustomerContentEncryptionConfiguration": (
+            CustomerContentEncryptionConfigurationOutputTypeDef
+        ),
+        "EnableMinimumEncryptionConfiguration": bool,
+    },
+    total=False,
+)
+
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "Description": str,
+        "WorkGroup": str,
+        "EngineVersion": str,
+        "EngineConfiguration": EngineConfigurationOutputTypeDef,
+        "NotebookVersion": str,
+        "SessionConfiguration": SessionConfigurationTypeDef,
+        "Status": SessionStatusTypeDef,
+        "Statistics": SessionStatisticsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 WorkGroupConfigurationTypeDef = TypedDict(
     "WorkGroupConfigurationTypeDef",
     {
         "ResultConfiguration": ResultConfigurationTypeDef,
         "EnforceWorkGroupConfiguration": bool,
         "PublishCloudWatchMetricsEnabled": bool,
         "BytesScannedCutoffPerQuery": int,
@@ -2308,30 +2490,14 @@
         "ExecutionRole": str,
         "CustomerContentEncryptionConfiguration": CustomerContentEncryptionConfigurationTypeDef,
         "EnableMinimumEncryptionConfiguration": bool,
     },
     total=False,
 )
 
-GetSessionResponseTypeDef = TypedDict(
-    "GetSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "Description": str,
-        "WorkGroup": str,
-        "EngineVersion": str,
-        "EngineConfiguration": EngineConfigurationTypeDef,
-        "NotebookVersion": str,
-        "SessionConfiguration": SessionConfigurationTypeDef,
-        "Status": SessionStatusTypeDef,
-        "Statistics": SessionStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListWorkGroupsOutputTypeDef = TypedDict(
     "ListWorkGroupsOutputTypeDef",
     {
         "WorkGroups": List[WorkGroupSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2356,21 +2522,21 @@
 
 QueryExecutionTypeDef = TypedDict(
     "QueryExecutionTypeDef",
     {
         "QueryExecutionId": str,
         "Query": str,
         "StatementType": StatementTypeType,
-        "ResultConfiguration": ResultConfigurationTypeDef,
-        "ResultReuseConfiguration": ResultReuseConfigurationTypeDef,
-        "QueryExecutionContext": QueryExecutionContextTypeDef,
+        "ResultConfiguration": ResultConfigurationOutputTypeDef,
+        "ResultReuseConfiguration": ResultReuseConfigurationOutputTypeDef,
+        "QueryExecutionContext": QueryExecutionContextOutputTypeDef,
         "Status": QueryExecutionStatusTypeDef,
         "Statistics": QueryExecutionStatisticsTypeDef,
         "WorkGroup": str,
-        "EngineVersion": EngineVersionTypeDef,
+        "EngineVersion": EngineVersionOutputTypeDef,
         "ExecutionParameters": List[str],
         "SubstatementType": str,
     },
     total=False,
 )
 
 _RequiredStartQueryExecutionInputRequestTypeDef = TypedDict(
@@ -2405,56 +2571,56 @@
         "UpdateCount": int,
         "ResultSet": ResultSetTypeDef,
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateWorkGroupInputRequestTypeDef = TypedDict(
-    "_RequiredCreateWorkGroupInputRequestTypeDef",
+_RequiredWorkGroupTypeDef = TypedDict(
+    "_RequiredWorkGroupTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalCreateWorkGroupInputRequestTypeDef = TypedDict(
-    "_OptionalCreateWorkGroupInputRequestTypeDef",
+_OptionalWorkGroupTypeDef = TypedDict(
+    "_OptionalWorkGroupTypeDef",
     {
-        "Configuration": WorkGroupConfigurationTypeDef,
+        "State": WorkGroupStateType,
+        "Configuration": WorkGroupConfigurationOutputTypeDef,
         "Description": str,
-        "Tags": Sequence[TagTypeDef],
+        "CreationTime": datetime,
     },
     total=False,
 )
 
 
-class CreateWorkGroupInputRequestTypeDef(
-    _RequiredCreateWorkGroupInputRequestTypeDef, _OptionalCreateWorkGroupInputRequestTypeDef
-):
+class WorkGroupTypeDef(_RequiredWorkGroupTypeDef, _OptionalWorkGroupTypeDef):
     pass
 
 
-_RequiredWorkGroupTypeDef = TypedDict(
-    "_RequiredWorkGroupTypeDef",
+_RequiredCreateWorkGroupInputRequestTypeDef = TypedDict(
+    "_RequiredCreateWorkGroupInputRequestTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalWorkGroupTypeDef = TypedDict(
-    "_OptionalWorkGroupTypeDef",
+_OptionalCreateWorkGroupInputRequestTypeDef = TypedDict(
+    "_OptionalCreateWorkGroupInputRequestTypeDef",
     {
-        "State": WorkGroupStateType,
         "Configuration": WorkGroupConfigurationTypeDef,
         "Description": str,
-        "CreationTime": datetime,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
-class WorkGroupTypeDef(_RequiredWorkGroupTypeDef, _OptionalWorkGroupTypeDef):
+class CreateWorkGroupInputRequestTypeDef(
+    _RequiredCreateWorkGroupInputRequestTypeDef, _OptionalCreateWorkGroupInputRequestTypeDef
+):
     pass
 
 
 _RequiredUpdateWorkGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkGroupInputRequestTypeDef",
     {
         "WorkGroup": str,
```

### Comparing `mypy-boto3-athena-1.28.0/mypy_boto3_athena/type_defs.pyi` & `mypy-boto3-athena-1.28.12/mypy_boto3_athena/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for athena service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_athena.type_defs import AclConfigurationTypeDef
+    from mypy_boto3_athena.type_defs import AclConfigurationOutputTypeDef
 
-    data: AclConfigurationTypeDef = {...}
+    data: AclConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -36,14 +36,15 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AclConfigurationOutputTypeDef",
     "AclConfigurationTypeDef",
     "ApplicationDPUSizesTypeDef",
     "AthenaErrorTypeDef",
     "BatchGetNamedQueryInputRequestTypeDef",
     "NamedQueryTypeDef",
     "UnprocessedNamedQueryIdTypeDef",
     "BatchGetPreparedStatementInputRequestTypeDef",
@@ -53,38 +54,43 @@
     "UnprocessedQueryExecutionIdTypeDef",
     "CalculationConfigurationTypeDef",
     "CalculationResultTypeDef",
     "CalculationStatisticsTypeDef",
     "CalculationStatusTypeDef",
     "CancelCapacityReservationInputRequestTypeDef",
     "CapacityAllocationTypeDef",
+    "CapacityAssignmentOutputTypeDef",
     "CapacityAssignmentTypeDef",
     "ColumnInfoTypeDef",
     "ColumnTypeDef",
     "TagTypeDef",
     "CreateNamedQueryInputRequestTypeDef",
     "CreateNamedQueryOutputTypeDef",
     "CreateNotebookInputRequestTypeDef",
     "CreateNotebookOutputTypeDef",
     "CreatePreparedStatementInputRequestTypeDef",
     "CreatePresignedNotebookUrlRequestRequestTypeDef",
     "CreatePresignedNotebookUrlResponseTypeDef",
+    "CustomerContentEncryptionConfigurationOutputTypeDef",
     "CustomerContentEncryptionConfigurationTypeDef",
     "DataCatalogSummaryTypeDef",
     "DataCatalogTypeDef",
     "DatabaseTypeDef",
     "DatumTypeDef",
     "DeleteCapacityReservationInputRequestTypeDef",
     "DeleteDataCatalogInputRequestTypeDef",
     "DeleteNamedQueryInputRequestTypeDef",
     "DeleteNotebookInputRequestTypeDef",
     "DeletePreparedStatementInputRequestTypeDef",
     "DeleteWorkGroupInputRequestTypeDef",
+    "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
+    "EngineConfigurationOutputTypeDef",
     "EngineConfigurationTypeDef",
+    "EngineVersionOutputTypeDef",
     "EngineVersionTypeDef",
     "ExecutorsSummaryTypeDef",
     "ExportNotebookInputRequestTypeDef",
     "NotebookMetadataTypeDef",
     "FilterDefinitionTypeDef",
     "GetCalculationExecutionCodeRequestRequestTypeDef",
     "GetCalculationExecutionCodeResponseTypeDef",
@@ -129,23 +135,26 @@
     "ListQueryExecutionsInputRequestTypeDef",
     "ListQueryExecutionsOutputTypeDef",
     "ListSessionsRequestRequestTypeDef",
     "ListTableMetadataInputListTableMetadataPaginateTypeDef",
     "ListTableMetadataInputRequestTypeDef",
     "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "TagOutputTypeDef",
     "ListWorkGroupsInputRequestTypeDef",
     "PaginatorConfigTypeDef",
+    "QueryExecutionContextOutputTypeDef",
     "QueryExecutionContextTypeDef",
     "ResultReuseInformationTypeDef",
     "QueryRuntimeStatisticsRowsTypeDef",
     "QueryRuntimeStatisticsTimelineTypeDef",
     "QueryStagePlanNodeTypeDef",
     "QueryStageTypeDef",
     "ResponseMetadataTypeDef",
+    "ResultReuseByAgeConfigurationOutputTypeDef",
     "ResultReuseByAgeConfigurationTypeDef",
     "StartCalculationExecutionResponseTypeDef",
     "StartQueryExecutionOutputTypeDef",
     "StartSessionResponseTypeDef",
     "StopCalculationExecutionRequestRequestTypeDef",
     "StopCalculationExecutionResponseTypeDef",
     "StopQueryExecutionInputRequestTypeDef",
@@ -171,63 +180,73 @@
     "CapacityReservationTypeDef",
     "CapacityAssignmentConfigurationTypeDef",
     "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     "ResultSetMetadataTypeDef",
     "TableMetadataTypeDef",
     "CreateCapacityReservationInputRequestTypeDef",
     "CreateDataCatalogInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ListDataCatalogsOutputTypeDef",
     "GetDataCatalogOutputTypeDef",
     "GetDatabaseOutputTypeDef",
     "ListDatabasesOutputTypeDef",
     "RowTypeDef",
+    "ResultConfigurationOutputTypeDef",
+    "SessionConfigurationTypeDef",
     "ResultConfigurationTypeDef",
     "ResultConfigurationUpdatesTypeDef",
-    "SessionConfigurationTypeDef",
     "StartSessionRequestRequestTypeDef",
     "ListEngineVersionsOutputTypeDef",
     "WorkGroupSummaryTypeDef",
     "ListExecutorsResponseTypeDef",
     "ExportNotebookOutputTypeDef",
     "GetNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataInputRequestTypeDef",
     "GetSessionStatusResponseTypeDef",
     "SessionSummaryTypeDef",
     "ListNotebookSessionsResponseTypeDef",
     "ListPreparedStatementsOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "QueryExecutionStatisticsTypeDef",
     "QueryRuntimeStatisticsTypeDef",
+    "ResultReuseConfigurationOutputTypeDef",
     "ResultReuseConfigurationTypeDef",
     "ListCalculationExecutionsResponseTypeDef",
     "GetCapacityReservationOutputTypeDef",
     "ListCapacityReservationsOutputTypeDef",
     "GetCapacityAssignmentConfigurationOutputTypeDef",
     "GetTableMetadataOutputTypeDef",
     "ListTableMetadataOutputTypeDef",
     "ResultSetTypeDef",
+    "WorkGroupConfigurationOutputTypeDef",
+    "GetSessionResponseTypeDef",
     "WorkGroupConfigurationTypeDef",
     "WorkGroupConfigurationUpdatesTypeDef",
-    "GetSessionResponseTypeDef",
     "ListWorkGroupsOutputTypeDef",
     "ListSessionsResponseTypeDef",
     "GetQueryRuntimeStatisticsOutputTypeDef",
     "QueryExecutionTypeDef",
     "StartQueryExecutionInputRequestTypeDef",
     "GetQueryResultsOutputTypeDef",
-    "CreateWorkGroupInputRequestTypeDef",
     "WorkGroupTypeDef",
+    "CreateWorkGroupInputRequestTypeDef",
     "UpdateWorkGroupInputRequestTypeDef",
     "BatchGetQueryExecutionOutputTypeDef",
     "GetQueryExecutionOutputTypeDef",
     "GetWorkGroupOutputTypeDef",
 )
 
+AclConfigurationOutputTypeDef = TypedDict(
+    "AclConfigurationOutputTypeDef",
+    {
+        "S3AclOption": Literal["BUCKET_OWNER_FULL_CONTROL"],
+    },
+)
+
 AclConfigurationTypeDef = TypedDict(
     "AclConfigurationTypeDef",
     {
         "S3AclOption": Literal["BUCKET_OWNER_FULL_CONTROL"],
     },
 )
 
@@ -399,18 +418,26 @@
 )
 
 class CapacityAllocationTypeDef(
     _RequiredCapacityAllocationTypeDef, _OptionalCapacityAllocationTypeDef
 ):
     pass
 
+CapacityAssignmentOutputTypeDef = TypedDict(
+    "CapacityAssignmentOutputTypeDef",
+    {
+        "WorkGroupNames": List[str],
+    },
+    total=False,
+)
+
 CapacityAssignmentTypeDef = TypedDict(
     "CapacityAssignmentTypeDef",
     {
-        "WorkGroupNames": List[str],
+        "WorkGroupNames": Sequence[str],
     },
     total=False,
 )
 
 _RequiredColumnInfoTypeDef = TypedDict(
     "_RequiredColumnInfoTypeDef",
     {
@@ -557,14 +584,21 @@
         "NotebookUrl": str,
         "AuthToken": str,
         "AuthTokenExpirationTime": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CustomerContentEncryptionConfigurationOutputTypeDef = TypedDict(
+    "CustomerContentEncryptionConfigurationOutputTypeDef",
+    {
+        "KmsKey": str,
+    },
+)
+
 CustomerContentEncryptionConfigurationTypeDef = TypedDict(
     "CustomerContentEncryptionConfigurationTypeDef",
     {
         "KmsKey": str,
     },
 )
 
@@ -673,14 +707,33 @@
 )
 
 class DeleteWorkGroupInputRequestTypeDef(
     _RequiredDeleteWorkGroupInputRequestTypeDef, _OptionalDeleteWorkGroupInputRequestTypeDef
 ):
     pass
 
+_RequiredEncryptionConfigurationOutputTypeDef = TypedDict(
+    "_RequiredEncryptionConfigurationOutputTypeDef",
+    {
+        "EncryptionOption": EncryptionOptionType,
+    },
+)
+_OptionalEncryptionConfigurationOutputTypeDef = TypedDict(
+    "_OptionalEncryptionConfigurationOutputTypeDef",
+    {
+        "KmsKey": str,
+    },
+    total=False,
+)
+
+class EncryptionConfigurationOutputTypeDef(
+    _RequiredEncryptionConfigurationOutputTypeDef, _OptionalEncryptionConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredEncryptionConfigurationTypeDef = TypedDict(
     "_RequiredEncryptionConfigurationTypeDef",
     {
         "EncryptionOption": EncryptionOptionType,
     },
 )
 _OptionalEncryptionConfigurationTypeDef = TypedDict(
@@ -692,36 +745,67 @@
 )
 
 class EncryptionConfigurationTypeDef(
     _RequiredEncryptionConfigurationTypeDef, _OptionalEncryptionConfigurationTypeDef
 ):
     pass
 
+_RequiredEngineConfigurationOutputTypeDef = TypedDict(
+    "_RequiredEngineConfigurationOutputTypeDef",
+    {
+        "MaxConcurrentDpus": int,
+    },
+)
+_OptionalEngineConfigurationOutputTypeDef = TypedDict(
+    "_OptionalEngineConfigurationOutputTypeDef",
+    {
+        "CoordinatorDpuSize": int,
+        "DefaultExecutorDpuSize": int,
+        "AdditionalConfigs": Dict[str, str],
+        "SparkProperties": Dict[str, str],
+    },
+    total=False,
+)
+
+class EngineConfigurationOutputTypeDef(
+    _RequiredEngineConfigurationOutputTypeDef, _OptionalEngineConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredEngineConfigurationTypeDef = TypedDict(
     "_RequiredEngineConfigurationTypeDef",
     {
         "MaxConcurrentDpus": int,
     },
 )
 _OptionalEngineConfigurationTypeDef = TypedDict(
     "_OptionalEngineConfigurationTypeDef",
     {
         "CoordinatorDpuSize": int,
         "DefaultExecutorDpuSize": int,
-        "AdditionalConfigs": Dict[str, str],
-        "SparkProperties": Dict[str, str],
+        "AdditionalConfigs": Mapping[str, str],
+        "SparkProperties": Mapping[str, str],
     },
     total=False,
 )
 
 class EngineConfigurationTypeDef(
     _RequiredEngineConfigurationTypeDef, _OptionalEngineConfigurationTypeDef
 ):
     pass
 
+EngineVersionOutputTypeDef = TypedDict(
+    "EngineVersionOutputTypeDef",
+    {
+        "SelectedEngineVersion": str,
+        "EffectiveEngineVersion": str,
+    },
+    total=False,
+)
+
 EngineVersionTypeDef = TypedDict(
     "EngineVersionTypeDef",
     {
         "SelectedEngineVersion": str,
         "EffectiveEngineVersion": str,
     },
     total=False,
@@ -1335,14 +1419,23 @@
 )
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 ListWorkGroupsInputRequestTypeDef = TypedDict(
     "ListWorkGroupsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1354,14 +1447,23 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+QueryExecutionContextOutputTypeDef = TypedDict(
+    "QueryExecutionContextOutputTypeDef",
+    {
+        "Database": str,
+        "Catalog": str,
+    },
+    total=False,
+)
+
 QueryExecutionContextTypeDef = TypedDict(
     "QueryExecutionContextTypeDef",
     {
         "Database": str,
         "Catalog": str,
     },
     total=False,
@@ -1431,14 +1533,34 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+_RequiredResultReuseByAgeConfigurationOutputTypeDef = TypedDict(
+    "_RequiredResultReuseByAgeConfigurationOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalResultReuseByAgeConfigurationOutputTypeDef = TypedDict(
+    "_OptionalResultReuseByAgeConfigurationOutputTypeDef",
+    {
+        "MaxAgeInMinutes": int,
+    },
+    total=False,
+)
+
+class ResultReuseByAgeConfigurationOutputTypeDef(
+    _RequiredResultReuseByAgeConfigurationOutputTypeDef,
+    _OptionalResultReuseByAgeConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredResultReuseByAgeConfigurationTypeDef = TypedDict(
     "_RequiredResultReuseByAgeConfigurationTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalResultReuseByAgeConfigurationTypeDef = TypedDict(
@@ -1775,15 +1897,15 @@
 ):
     pass
 
 CapacityAssignmentConfigurationTypeDef = TypedDict(
     "CapacityAssignmentConfigurationTypeDef",
     {
         "CapacityReservationName": str,
-        "CapacityAssignments": List[CapacityAssignmentTypeDef],
+        "CapacityAssignments": List[CapacityAssignmentOutputTypeDef],
     },
     total=False,
 )
 
 PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
     "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     {
@@ -1861,23 +1983,14 @@
 )
 
 class CreateDataCatalogInputRequestTypeDef(
     _RequiredCreateDataCatalogInputRequestTypeDef, _OptionalCreateDataCatalogInputRequestTypeDef
 ):
     pass
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1920,14 +2033,36 @@
     "RowTypeDef",
     {
         "Data": List[DatumTypeDef],
     },
     total=False,
 )
 
+ResultConfigurationOutputTypeDef = TypedDict(
+    "ResultConfigurationOutputTypeDef",
+    {
+        "OutputLocation": str,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "ExpectedBucketOwner": str,
+        "AclConfiguration": AclConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+SessionConfigurationTypeDef = TypedDict(
+    "SessionConfigurationTypeDef",
+    {
+        "ExecutionRole": str,
+        "WorkingDirectory": str,
+        "IdleTimeoutSeconds": int,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ResultConfigurationTypeDef = TypedDict(
     "ResultConfigurationTypeDef",
     {
         "OutputLocation": str,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "ExpectedBucketOwner": str,
         "AclConfiguration": AclConfigurationTypeDef,
@@ -1946,25 +2081,14 @@
         "RemoveExpectedBucketOwner": bool,
         "AclConfiguration": AclConfigurationTypeDef,
         "RemoveAclConfiguration": bool,
     },
     total=False,
 )
 
-SessionConfigurationTypeDef = TypedDict(
-    "SessionConfigurationTypeDef",
-    {
-        "ExecutionRole": str,
-        "WorkingDirectory": str,
-        "IdleTimeoutSeconds": int,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredStartSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSessionRequestRequestTypeDef",
     {
         "WorkGroup": str,
         "EngineConfiguration": EngineConfigurationTypeDef,
     },
 )
@@ -1983,28 +2107,28 @@
     _RequiredStartSessionRequestRequestTypeDef, _OptionalStartSessionRequestRequestTypeDef
 ):
     pass
 
 ListEngineVersionsOutputTypeDef = TypedDict(
     "ListEngineVersionsOutputTypeDef",
     {
-        "EngineVersions": List[EngineVersionTypeDef],
+        "EngineVersions": List[EngineVersionOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WorkGroupSummaryTypeDef = TypedDict(
     "WorkGroupSummaryTypeDef",
     {
         "Name": str,
         "State": WorkGroupStateType,
         "Description": str,
         "CreationTime": datetime,
-        "EngineVersion": EngineVersionTypeDef,
+        "EngineVersion": EngineVersionOutputTypeDef,
     },
     total=False,
 )
 
 ListExecutorsResponseTypeDef = TypedDict(
     "ListExecutorsResponseTypeDef",
     {
@@ -2073,15 +2197,15 @@
 )
 
 SessionSummaryTypeDef = TypedDict(
     "SessionSummaryTypeDef",
     {
         "SessionId": str,
         "Description": str,
-        "EngineVersion": EngineVersionTypeDef,
+        "EngineVersion": EngineVersionOutputTypeDef,
         "NotebookVersion": str,
         "Status": SessionStatusTypeDef,
     },
     total=False,
 )
 
 ListNotebookSessionsResponseTypeDef = TypedDict(
@@ -2098,14 +2222,23 @@
     {
         "PreparedStatements": List[PreparedStatementSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 QueryExecutionStatisticsTypeDef = TypedDict(
     "QueryExecutionStatisticsTypeDef",
     {
         "EngineExecutionTimeInMillis": int,
         "DataScannedInBytes": int,
         "DataManifestLocation": str,
         "TotalExecutionTimeInMillis": int,
@@ -2123,14 +2256,22 @@
         "Timeline": QueryRuntimeStatisticsTimelineTypeDef,
         "Rows": QueryRuntimeStatisticsRowsTypeDef,
         "OutputStage": "QueryStageTypeDef",
     },
     total=False,
 )
 
+ResultReuseConfigurationOutputTypeDef = TypedDict(
+    "ResultReuseConfigurationOutputTypeDef",
+    {
+        "ResultReuseByAgeConfiguration": ResultReuseByAgeConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ResultReuseConfigurationTypeDef = TypedDict(
     "ResultReuseConfigurationTypeDef",
     {
         "ResultReuseByAgeConfiguration": ResultReuseByAgeConfigurationTypeDef,
     },
     total=False,
 )
@@ -2191,14 +2332,49 @@
     {
         "Rows": List[RowTypeDef],
         "ResultSetMetadata": ResultSetMetadataTypeDef,
     },
     total=False,
 )
 
+WorkGroupConfigurationOutputTypeDef = TypedDict(
+    "WorkGroupConfigurationOutputTypeDef",
+    {
+        "ResultConfiguration": ResultConfigurationOutputTypeDef,
+        "EnforceWorkGroupConfiguration": bool,
+        "PublishCloudWatchMetricsEnabled": bool,
+        "BytesScannedCutoffPerQuery": int,
+        "RequesterPaysEnabled": bool,
+        "EngineVersion": EngineVersionOutputTypeDef,
+        "AdditionalConfiguration": str,
+        "ExecutionRole": str,
+        "CustomerContentEncryptionConfiguration": (
+            CustomerContentEncryptionConfigurationOutputTypeDef
+        ),
+        "EnableMinimumEncryptionConfiguration": bool,
+    },
+    total=False,
+)
+
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "Description": str,
+        "WorkGroup": str,
+        "EngineVersion": str,
+        "EngineConfiguration": EngineConfigurationOutputTypeDef,
+        "NotebookVersion": str,
+        "SessionConfiguration": SessionConfigurationTypeDef,
+        "Status": SessionStatusTypeDef,
+        "Statistics": SessionStatisticsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 WorkGroupConfigurationTypeDef = TypedDict(
     "WorkGroupConfigurationTypeDef",
     {
         "ResultConfiguration": ResultConfigurationTypeDef,
         "EnforceWorkGroupConfiguration": bool,
         "PublishCloudWatchMetricsEnabled": bool,
         "BytesScannedCutoffPerQuery": int,
@@ -2227,30 +2403,14 @@
         "ExecutionRole": str,
         "CustomerContentEncryptionConfiguration": CustomerContentEncryptionConfigurationTypeDef,
         "EnableMinimumEncryptionConfiguration": bool,
     },
     total=False,
 )
 
-GetSessionResponseTypeDef = TypedDict(
-    "GetSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "Description": str,
-        "WorkGroup": str,
-        "EngineVersion": str,
-        "EngineConfiguration": EngineConfigurationTypeDef,
-        "NotebookVersion": str,
-        "SessionConfiguration": SessionConfigurationTypeDef,
-        "Status": SessionStatusTypeDef,
-        "Statistics": SessionStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListWorkGroupsOutputTypeDef = TypedDict(
     "ListWorkGroupsOutputTypeDef",
     {
         "WorkGroups": List[WorkGroupSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2275,21 +2435,21 @@
 
 QueryExecutionTypeDef = TypedDict(
     "QueryExecutionTypeDef",
     {
         "QueryExecutionId": str,
         "Query": str,
         "StatementType": StatementTypeType,
-        "ResultConfiguration": ResultConfigurationTypeDef,
-        "ResultReuseConfiguration": ResultReuseConfigurationTypeDef,
-        "QueryExecutionContext": QueryExecutionContextTypeDef,
+        "ResultConfiguration": ResultConfigurationOutputTypeDef,
+        "ResultReuseConfiguration": ResultReuseConfigurationOutputTypeDef,
+        "QueryExecutionContext": QueryExecutionContextOutputTypeDef,
         "Status": QueryExecutionStatusTypeDef,
         "Statistics": QueryExecutionStatisticsTypeDef,
         "WorkGroup": str,
-        "EngineVersion": EngineVersionTypeDef,
+        "EngineVersion": EngineVersionOutputTypeDef,
         "ExecutionParameters": List[str],
         "SubstatementType": str,
     },
     total=False,
 )
 
 _RequiredStartQueryExecutionInputRequestTypeDef = TypedDict(
@@ -2322,53 +2482,53 @@
         "UpdateCount": int,
         "ResultSet": ResultSetTypeDef,
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateWorkGroupInputRequestTypeDef = TypedDict(
-    "_RequiredCreateWorkGroupInputRequestTypeDef",
+_RequiredWorkGroupTypeDef = TypedDict(
+    "_RequiredWorkGroupTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalCreateWorkGroupInputRequestTypeDef = TypedDict(
-    "_OptionalCreateWorkGroupInputRequestTypeDef",
+_OptionalWorkGroupTypeDef = TypedDict(
+    "_OptionalWorkGroupTypeDef",
     {
-        "Configuration": WorkGroupConfigurationTypeDef,
+        "State": WorkGroupStateType,
+        "Configuration": WorkGroupConfigurationOutputTypeDef,
         "Description": str,
-        "Tags": Sequence[TagTypeDef],
+        "CreationTime": datetime,
     },
     total=False,
 )
 
-class CreateWorkGroupInputRequestTypeDef(
-    _RequiredCreateWorkGroupInputRequestTypeDef, _OptionalCreateWorkGroupInputRequestTypeDef
-):
+class WorkGroupTypeDef(_RequiredWorkGroupTypeDef, _OptionalWorkGroupTypeDef):
     pass
 
-_RequiredWorkGroupTypeDef = TypedDict(
-    "_RequiredWorkGroupTypeDef",
+_RequiredCreateWorkGroupInputRequestTypeDef = TypedDict(
+    "_RequiredCreateWorkGroupInputRequestTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalWorkGroupTypeDef = TypedDict(
-    "_OptionalWorkGroupTypeDef",
+_OptionalCreateWorkGroupInputRequestTypeDef = TypedDict(
+    "_OptionalCreateWorkGroupInputRequestTypeDef",
     {
-        "State": WorkGroupStateType,
         "Configuration": WorkGroupConfigurationTypeDef,
         "Description": str,
-        "CreationTime": datetime,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-class WorkGroupTypeDef(_RequiredWorkGroupTypeDef, _OptionalWorkGroupTypeDef):
+class CreateWorkGroupInputRequestTypeDef(
+    _RequiredCreateWorkGroupInputRequestTypeDef, _OptionalCreateWorkGroupInputRequestTypeDef
+):
     pass
 
 _RequiredUpdateWorkGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkGroupInputRequestTypeDef",
     {
         "WorkGroup": str,
     },
```

### Comparing `mypy-boto3-athena-1.28.0/mypy_boto3_athena.egg-info/PKG-INFO` & `mypy-boto3-athena-1.28.12/mypy_boto3_athena.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-athena
-Version: 1.28.0
-Summary: Type annotations for boto3.Athena 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Athena 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-athena"></a>
 
 # mypy-boto3-athena
 
 [![PyPI - mypy-boto3-athena](https://img.shields.io/pypi/v/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-athena?color=blue)](https://pypistats.org/packages/mypy-boto3-athena)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-athena)](https://pepy.tech/project/mypy-boto3-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Athena 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[boto3.Athena 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
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
 [mypy-boto3-athena docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,14 +358,15 @@
 ### Typed dictionaries
 
 `mypy_boto3_athena.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_athena.type_defs import (
+    AclConfigurationOutputTypeDef,
     AclConfigurationTypeDef,
     ApplicationDPUSizesTypeDef,
     AthenaErrorTypeDef,
     BatchGetNamedQueryInputRequestTypeDef,
     NamedQueryTypeDef,
     UnprocessedNamedQueryIdTypeDef,
     BatchGetPreparedStatementInputRequestTypeDef,
@@ -375,38 +376,43 @@
     UnprocessedQueryExecutionIdTypeDef,
     CalculationConfigurationTypeDef,
     CalculationResultTypeDef,
     CalculationStatisticsTypeDef,
     CalculationStatusTypeDef,
     CancelCapacityReservationInputRequestTypeDef,
     CapacityAllocationTypeDef,
+    CapacityAssignmentOutputTypeDef,
     CapacityAssignmentTypeDef,
     ColumnInfoTypeDef,
     ColumnTypeDef,
     TagTypeDef,
     CreateNamedQueryInputRequestTypeDef,
     CreateNamedQueryOutputTypeDef,
     CreateNotebookInputRequestTypeDef,
     CreateNotebookOutputTypeDef,
     CreatePreparedStatementInputRequestTypeDef,
     CreatePresignedNotebookUrlRequestRequestTypeDef,
     CreatePresignedNotebookUrlResponseTypeDef,
+    CustomerContentEncryptionConfigurationOutputTypeDef,
     CustomerContentEncryptionConfigurationTypeDef,
     DataCatalogSummaryTypeDef,
     DataCatalogTypeDef,
     DatabaseTypeDef,
     DatumTypeDef,
     DeleteCapacityReservationInputRequestTypeDef,
     DeleteDataCatalogInputRequestTypeDef,
     DeleteNamedQueryInputRequestTypeDef,
     DeleteNotebookInputRequestTypeDef,
     DeletePreparedStatementInputRequestTypeDef,
     DeleteWorkGroupInputRequestTypeDef,
+    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
+    EngineConfigurationOutputTypeDef,
     EngineConfigurationTypeDef,
+    EngineVersionOutputTypeDef,
     EngineVersionTypeDef,
     ExecutorsSummaryTypeDef,
     ExportNotebookInputRequestTypeDef,
     NotebookMetadataTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeRequestRequestTypeDef,
     GetCalculationExecutionCodeResponseTypeDef,
@@ -451,23 +457,26 @@
     ListQueryExecutionsInputRequestTypeDef,
     ListQueryExecutionsOutputTypeDef,
     ListSessionsRequestRequestTypeDef,
     ListTableMetadataInputListTableMetadataPaginateTypeDef,
     ListTableMetadataInputRequestTypeDef,
     ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    TagOutputTypeDef,
     ListWorkGroupsInputRequestTypeDef,
     PaginatorConfigTypeDef,
+    QueryExecutionContextOutputTypeDef,
     QueryExecutionContextTypeDef,
     ResultReuseInformationTypeDef,
     QueryRuntimeStatisticsRowsTypeDef,
     QueryRuntimeStatisticsTimelineTypeDef,
     QueryStagePlanNodeTypeDef,
     QueryStageTypeDef,
     ResponseMetadataTypeDef,
+    ResultReuseByAgeConfigurationOutputTypeDef,
     ResultReuseByAgeConfigurationTypeDef,
     StartCalculationExecutionResponseTypeDef,
     StartQueryExecutionOutputTypeDef,
     StartSessionResponseTypeDef,
     StopCalculationExecutionRequestRequestTypeDef,
     StopCalculationExecutionResponseTypeDef,
     StopQueryExecutionInputRequestTypeDef,
@@ -493,65 +502,68 @@
     CapacityReservationTypeDef,
     CapacityAssignmentConfigurationTypeDef,
     PutCapacityAssignmentConfigurationInputRequestTypeDef,
     ResultSetMetadataTypeDef,
     TableMetadataTypeDef,
     CreateCapacityReservationInputRequestTypeDef,
     CreateDataCatalogInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ListDataCatalogsOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetDatabaseOutputTypeDef,
     ListDatabasesOutputTypeDef,
     RowTypeDef,
+    ResultConfigurationOutputTypeDef,
+    SessionConfigurationTypeDef,
     ResultConfigurationTypeDef,
     ResultConfigurationUpdatesTypeDef,
-    SessionConfigurationTypeDef,
     StartSessionRequestRequestTypeDef,
     ListEngineVersionsOutputTypeDef,
     WorkGroupSummaryTypeDef,
     ListExecutorsResponseTypeDef,
     ExportNotebookOutputTypeDef,
     GetNotebookMetadataOutputTypeDef,
     ListNotebookMetadataOutputTypeDef,
     ListNotebookMetadataInputRequestTypeDef,
     GetSessionStatusResponseTypeDef,
     SessionSummaryTypeDef,
     ListNotebookSessionsResponseTypeDef,
     ListPreparedStatementsOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     QueryExecutionStatisticsTypeDef,
     QueryRuntimeStatisticsTypeDef,
+    ResultReuseConfigurationOutputTypeDef,
     ResultReuseConfigurationTypeDef,
     ListCalculationExecutionsResponseTypeDef,
     GetCapacityReservationOutputTypeDef,
     ListCapacityReservationsOutputTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
     GetTableMetadataOutputTypeDef,
     ListTableMetadataOutputTypeDef,
     ResultSetTypeDef,
+    WorkGroupConfigurationOutputTypeDef,
+    GetSessionResponseTypeDef,
     WorkGroupConfigurationTypeDef,
     WorkGroupConfigurationUpdatesTypeDef,
-    GetSessionResponseTypeDef,
     ListWorkGroupsOutputTypeDef,
     ListSessionsResponseTypeDef,
     GetQueryRuntimeStatisticsOutputTypeDef,
     QueryExecutionTypeDef,
     StartQueryExecutionInputRequestTypeDef,
     GetQueryResultsOutputTypeDef,
-    CreateWorkGroupInputRequestTypeDef,
     WorkGroupTypeDef,
+    CreateWorkGroupInputRequestTypeDef,
     UpdateWorkGroupInputRequestTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     GetQueryExecutionOutputTypeDef,
     GetWorkGroupOutputTypeDef,
 )
 
 
-def get_structure() -> AclConfigurationTypeDef:
+def get_structure() -> AclConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-athena-1.28.0/mypy_boto3_athena.egg-info/SOURCES.txt` & `mypy-boto3-athena-1.28.12/mypy_boto3_athena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.0/setup.py` & `mypy-boto3-athena-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-athena",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_athena"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Athena 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Athena 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

