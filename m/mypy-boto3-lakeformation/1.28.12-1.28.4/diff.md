# Comparing `tmp/mypy-boto3-lakeformation-1.28.12.tar.gz` & `tmp/mypy-boto3-lakeformation-1.28.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lakeformation-1.28.12.tar", last modified: Thu Jul 27 05:34:55 2023, max compression
+gzip compressed data, was "mypy-boto3-lakeformation-1.28.4.tar", last modified: Tue Jul 18 01:01:41 2023, max compression
```

## Comparing `mypy-boto3-lakeformation-1.28.12.tar` & `mypy-boto3-lakeformation-1.28.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.300462 mypy-boto3-lakeformation-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:52.000000 mypy-boto3-lakeformation-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19370 2023-07-27 05:34:55.300462 mypy-boto3-lakeformation-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-07-27 05:24:52.000000 mypy-boto3-lakeformation-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.296462 mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-27 05:24:52.000000 mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-27 05:24:52.000000 mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-27 05:24:52.000000 mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37102 2023-07-27 05:24:53.000000 mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37043 2023-07-27 05:24:52.000000 mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-07-27 05:24:53.000000 mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-07-27 05:24:53.000000 mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-27 05:24:53.000000 mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-07-27 05:24:53.000000 mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:52.000000 mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    56094 2023-07-27 05:24:54.000000 mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55991 2023-07-27 05:24:53.000000 mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:52.000000 mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.300462 mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19370 2023-07-27 05:34:55.000000 mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 05:34:55.000000 mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:55.000000 mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 05:34:55.000000 mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:55.300462 mypy-boto3-lakeformation-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-27 05:24:52.000000 mypy-boto3-lakeformation-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19383 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37102 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37043 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53022 2023-07-18 01:01:31.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52937 2023-07-18 01:01:31.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19383 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-18 01:01:29.000000 mypy-boto3-lakeformation-1.28.4/setup.py
```

### Comparing `mypy-boto3-lakeformation-1.28.12/LICENSE` & `mypy-boto3-lakeformation-1.28.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.12/PKG-INFO` & `mypy-boto3-lakeformation-1.28.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lakeformation
-Version: 1.28.12
-Summary: Type annotations for boto3.LakeFormation 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.4
+Summary: Type annotations for boto3.LakeFormation 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lakeformation"></a>
 
 # mypy-boto3-lakeformation
 
 [![PyPI - mypy-boto3-lakeformation](https://img.shields.io/pypi/v/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lakeformation)](https://pepy.tech/project/mypy-boto3-lakeformation)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lakeformation?color=blue)](https://pypistats.org/packages/mypy-boto3-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LakeFormation 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[boto3.LakeFormation 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lakeformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -352,27 +352,26 @@
 
 `mypy_boto3_lakeformation.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lakeformation.type_defs import (
     LFTagPairTypeDef,
+    ResponseMetadataTypeDef,
     AddObjectInputTypeDef,
     AssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
-    AssumeDecoratedRoleWithSAMLResponseTypeDef,
     AuditContextTypeDef,
     ErrorDetailTypeDef,
     DataLakePrincipalOutputTypeDef,
     DataLakePrincipalTypeDef,
     CancelTransactionRequestRequestTypeDef,
     LFTagPairOutputTypeDef,
     ColumnWildcardOutputTypeDef,
     ColumnWildcardTypeDef,
     CommitTransactionRequestRequestTypeDef,
-    CommitTransactionResponseTypeDef,
     CreateLFTagRequestRequestTypeDef,
     RowFilterOutputTypeDef,
     DataCellsFilterResourceOutputTypeDef,
     DataCellsFilterResourceTypeDef,
     RowFilterTypeDef,
     DataLocationResourceOutputTypeDef,
     DataLocationResourceTypeDef,
@@ -391,50 +390,49 @@
     ExecutionStatisticsTypeDef,
     ExtendTransactionRequestRequestTypeDef,
     FilterConditionTypeDef,
     GetDataCellsFilterRequestRequestTypeDef,
     GetDataLakeSettingsRequestRequestTypeDef,
     GetEffectivePermissionsForPathRequestRequestTypeDef,
     GetLFTagRequestRequestTypeDef,
-    GetLFTagResponseTypeDef,
     GetQueryStateRequestRequestTypeDef,
-    GetQueryStateResponseTypeDef,
     GetQueryStatisticsRequestRequestTypeDef,
     PlanningStatisticsTypeDef,
     GetTableObjectsRequestRequestTypeDef,
     PartitionValueListTypeDef,
-    GetTemporaryGluePartitionCredentialsResponseTypeDef,
-    GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsRequestRequestTypeDef,
-    GetWorkUnitResultsResponseTypeDef,
-    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetWorkUnitsRequestRequestTypeDef,
     WorkUnitRangeTypeDef,
     LFTagKeyResourceOutputTypeDef,
     LFTagKeyResourceTypeDef,
     LFTagOutputTypeDef,
     LFTagTypeDef,
     TableResourceTypeDef,
-    ListLFTagsRequestListLFTagsPaginateTypeDef,
     ListLFTagsRequestRequestTypeDef,
     ListTableStorageOptimizersRequestRequestTypeDef,
     StorageOptimizerTypeDef,
     ListTransactionsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     TableObjectTypeDef,
     QueryPlanningContextTypeDef,
     RegisterResourceRequestRequestTypeDef,
     TableResourceOutputTypeDef,
-    ResponseMetadataTypeDef,
-    StartQueryPlanningResponseTypeDef,
     StartTransactionRequestRequestTypeDef,
-    StartTransactionResponseTypeDef,
     UpdateLFTagRequestRequestTypeDef,
     UpdateResourceRequestRequestTypeDef,
     UpdateTableStorageOptimizerRequestRequestTypeDef,
+    AssumeDecoratedRoleWithSAMLResponseTypeDef,
+    CommitTransactionResponseTypeDef,
+    GetLFTagResponseTypeDef,
+    GetQueryStateResponseTypeDef,
+    GetTemporaryGluePartitionCredentialsResponseTypeDef,
+    GetTemporaryGlueTableCredentialsResponseTypeDef,
+    GetWorkUnitResultsResponseTypeDef,
+    StartQueryPlanningResponseTypeDef,
+    StartTransactionResponseTypeDef,
     UpdateTableStorageOptimizerResponseTypeDef,
     GetTemporaryGlueTableCredentialsRequestRequestTypeDef,
     PrincipalPermissionsOutputTypeDef,
     PrincipalPermissionsTypeDef,
     ColumnLFTagTypeDef,
     LFTagErrorTypeDef,
     ListLFTagsResponseTypeDef,
@@ -448,14 +446,16 @@
     DescribeResourceResponseTypeDef,
     ListResourcesResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     ListTransactionsResponseTypeDef,
     ListResourcesRequestRequestTypeDef,
     GetQueryStatisticsResponseTypeDef,
     GetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
+    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    ListLFTagsRequestListLFTagsPaginateTypeDef,
     GetWorkUnitsResponseTypeDef,
     LFTagPolicyResourceOutputTypeDef,
     LFTagPolicyResourceTypeDef,
     SearchDatabasesByLFTagsRequestRequestTypeDef,
     SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
     SearchTablesByLFTagsRequestRequestTypeDef,
     SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
```

### Comparing `mypy-boto3-lakeformation-1.28.12/README.md` & `mypy-boto3-lakeformation-1.28.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-lakeformation"></a>
 
 # mypy-boto3-lakeformation
 
 [![PyPI - mypy-boto3-lakeformation](https://img.shields.io/pypi/v/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lakeformation)](https://pepy.tech/project/mypy-boto3-lakeformation)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lakeformation?color=blue)](https://pypistats.org/packages/mypy-boto3-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LakeFormation 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[boto3.LakeFormation 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lakeformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,27 +320,26 @@
 
 `mypy_boto3_lakeformation.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lakeformation.type_defs import (
     LFTagPairTypeDef,
+    ResponseMetadataTypeDef,
     AddObjectInputTypeDef,
     AssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
-    AssumeDecoratedRoleWithSAMLResponseTypeDef,
     AuditContextTypeDef,
     ErrorDetailTypeDef,
     DataLakePrincipalOutputTypeDef,
     DataLakePrincipalTypeDef,
     CancelTransactionRequestRequestTypeDef,
     LFTagPairOutputTypeDef,
     ColumnWildcardOutputTypeDef,
     ColumnWildcardTypeDef,
     CommitTransactionRequestRequestTypeDef,
-    CommitTransactionResponseTypeDef,
     CreateLFTagRequestRequestTypeDef,
     RowFilterOutputTypeDef,
     DataCellsFilterResourceOutputTypeDef,
     DataCellsFilterResourceTypeDef,
     RowFilterTypeDef,
     DataLocationResourceOutputTypeDef,
     DataLocationResourceTypeDef,
@@ -359,50 +358,49 @@
     ExecutionStatisticsTypeDef,
     ExtendTransactionRequestRequestTypeDef,
     FilterConditionTypeDef,
     GetDataCellsFilterRequestRequestTypeDef,
     GetDataLakeSettingsRequestRequestTypeDef,
     GetEffectivePermissionsForPathRequestRequestTypeDef,
     GetLFTagRequestRequestTypeDef,
-    GetLFTagResponseTypeDef,
     GetQueryStateRequestRequestTypeDef,
-    GetQueryStateResponseTypeDef,
     GetQueryStatisticsRequestRequestTypeDef,
     PlanningStatisticsTypeDef,
     GetTableObjectsRequestRequestTypeDef,
     PartitionValueListTypeDef,
-    GetTemporaryGluePartitionCredentialsResponseTypeDef,
-    GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsRequestRequestTypeDef,
-    GetWorkUnitResultsResponseTypeDef,
-    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetWorkUnitsRequestRequestTypeDef,
     WorkUnitRangeTypeDef,
     LFTagKeyResourceOutputTypeDef,
     LFTagKeyResourceTypeDef,
     LFTagOutputTypeDef,
     LFTagTypeDef,
     TableResourceTypeDef,
-    ListLFTagsRequestListLFTagsPaginateTypeDef,
     ListLFTagsRequestRequestTypeDef,
     ListTableStorageOptimizersRequestRequestTypeDef,
     StorageOptimizerTypeDef,
     ListTransactionsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     TableObjectTypeDef,
     QueryPlanningContextTypeDef,
     RegisterResourceRequestRequestTypeDef,
     TableResourceOutputTypeDef,
-    ResponseMetadataTypeDef,
-    StartQueryPlanningResponseTypeDef,
     StartTransactionRequestRequestTypeDef,
-    StartTransactionResponseTypeDef,
     UpdateLFTagRequestRequestTypeDef,
     UpdateResourceRequestRequestTypeDef,
     UpdateTableStorageOptimizerRequestRequestTypeDef,
+    AssumeDecoratedRoleWithSAMLResponseTypeDef,
+    CommitTransactionResponseTypeDef,
+    GetLFTagResponseTypeDef,
+    GetQueryStateResponseTypeDef,
+    GetTemporaryGluePartitionCredentialsResponseTypeDef,
+    GetTemporaryGlueTableCredentialsResponseTypeDef,
+    GetWorkUnitResultsResponseTypeDef,
+    StartQueryPlanningResponseTypeDef,
+    StartTransactionResponseTypeDef,
     UpdateTableStorageOptimizerResponseTypeDef,
     GetTemporaryGlueTableCredentialsRequestRequestTypeDef,
     PrincipalPermissionsOutputTypeDef,
     PrincipalPermissionsTypeDef,
     ColumnLFTagTypeDef,
     LFTagErrorTypeDef,
     ListLFTagsResponseTypeDef,
@@ -416,14 +414,16 @@
     DescribeResourceResponseTypeDef,
     ListResourcesResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     ListTransactionsResponseTypeDef,
     ListResourcesRequestRequestTypeDef,
     GetQueryStatisticsResponseTypeDef,
     GetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
+    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    ListLFTagsRequestListLFTagsPaginateTypeDef,
     GetWorkUnitsResponseTypeDef,
     LFTagPolicyResourceOutputTypeDef,
     LFTagPolicyResourceTypeDef,
     SearchDatabasesByLFTagsRequestRequestTypeDef,
     SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
     SearchTablesByLFTagsRequestRequestTypeDef,
     SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
```

### Comparing `mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/__init__.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/__init__.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/__main__.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LakeFormation 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.LakeFormation 1.28.4\nVersion:         1.28.4\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/client.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/client.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/literals.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -292,28 +291,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
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
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/literals.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -290,28 +289,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
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
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/paginator.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -47,103 +47,96 @@
     "GetWorkUnitsPaginator",
     "ListDataCellsFilterPaginator",
     "ListLFTagsPaginator",
     "SearchDatabasesByLFTagsPaginator",
     "SearchTablesByLFTagsPaginator",
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
 class GetWorkUnitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#getworkunitspaginator)
     """
 
     def paginate(
-        self, *, QueryId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QueryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetWorkUnitsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#getworkunitspaginator)
         """
 
-
 class ListDataCellsFilterPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listdatacellsfilterpaginator)
     """
 
     def paginate(
-        self, *, Table: TableResourceTypeDef = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Table: TableResourceTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDataCellsFilterResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listdatacellsfilterpaginator)
         """
 
-
 class ListLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listlftagspaginator)
     """
 
     def paginate(
         self,
         *,
         CatalogId: str = ...,
         ResourceShareType: ResourceShareTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listlftagspaginator)
         """
 
-
 class SearchDatabasesByLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchdatabasesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
         Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchDatabasesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchdatabasesbylftagspaginator)
         """
 
-
 class SearchTablesByLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchtablesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
         Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchTablesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchtablesbylftagspaginator)
         """
```

### Comparing `mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/paginator.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,96 +47,103 @@
     "GetWorkUnitsPaginator",
     "ListDataCellsFilterPaginator",
     "ListLFTagsPaginator",
     "SearchDatabasesByLFTagsPaginator",
     "SearchTablesByLFTagsPaginator",
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
 class GetWorkUnitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#getworkunitspaginator)
     """
 
     def paginate(
-        self, *, QueryId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QueryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetWorkUnitsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#getworkunitspaginator)
         """
 
+
 class ListDataCellsFilterPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listdatacellsfilterpaginator)
     """
 
     def paginate(
-        self, *, Table: TableResourceTypeDef = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Table: TableResourceTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDataCellsFilterResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listdatacellsfilterpaginator)
         """
 
+
 class ListLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listlftagspaginator)
     """
 
     def paginate(
         self,
         *,
         CatalogId: str = ...,
         ResourceShareType: ResourceShareTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listlftagspaginator)
         """
 
+
 class SearchDatabasesByLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchdatabasesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
         Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchDatabasesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchdatabasesbylftagspaginator)
         """
 
+
 class SearchTablesByLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchtablesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
         Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchTablesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchtablesbylftagspaginator)
         """
```

### Comparing `mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/type_defs.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,27 +36,26 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "LFTagPairTypeDef",
+    "ResponseMetadataTypeDef",
     "AddObjectInputTypeDef",
     "AssumeDecoratedRoleWithSAMLRequestRequestTypeDef",
-    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
     "AuditContextTypeDef",
     "ErrorDetailTypeDef",
     "DataLakePrincipalOutputTypeDef",
     "DataLakePrincipalTypeDef",
     "CancelTransactionRequestRequestTypeDef",
     "LFTagPairOutputTypeDef",
     "ColumnWildcardOutputTypeDef",
     "ColumnWildcardTypeDef",
     "CommitTransactionRequestRequestTypeDef",
-    "CommitTransactionResponseTypeDef",
     "CreateLFTagRequestRequestTypeDef",
     "RowFilterOutputTypeDef",
     "DataCellsFilterResourceOutputTypeDef",
     "DataCellsFilterResourceTypeDef",
     "RowFilterTypeDef",
     "DataLocationResourceOutputTypeDef",
     "DataLocationResourceTypeDef",
@@ -75,50 +74,49 @@
     "ExecutionStatisticsTypeDef",
     "ExtendTransactionRequestRequestTypeDef",
     "FilterConditionTypeDef",
     "GetDataCellsFilterRequestRequestTypeDef",
     "GetDataLakeSettingsRequestRequestTypeDef",
     "GetEffectivePermissionsForPathRequestRequestTypeDef",
     "GetLFTagRequestRequestTypeDef",
-    "GetLFTagResponseTypeDef",
     "GetQueryStateRequestRequestTypeDef",
-    "GetQueryStateResponseTypeDef",
     "GetQueryStatisticsRequestRequestTypeDef",
     "PlanningStatisticsTypeDef",
     "GetTableObjectsRequestRequestTypeDef",
     "PartitionValueListTypeDef",
-    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
-    "GetTemporaryGlueTableCredentialsResponseTypeDef",
     "GetWorkUnitResultsRequestRequestTypeDef",
-    "GetWorkUnitResultsResponseTypeDef",
-    "GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetWorkUnitsRequestRequestTypeDef",
     "WorkUnitRangeTypeDef",
     "LFTagKeyResourceOutputTypeDef",
     "LFTagKeyResourceTypeDef",
     "LFTagOutputTypeDef",
     "LFTagTypeDef",
     "TableResourceTypeDef",
-    "ListLFTagsRequestListLFTagsPaginateTypeDef",
     "ListLFTagsRequestRequestTypeDef",
     "ListTableStorageOptimizersRequestRequestTypeDef",
     "StorageOptimizerTypeDef",
     "ListTransactionsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "TableObjectTypeDef",
     "QueryPlanningContextTypeDef",
     "RegisterResourceRequestRequestTypeDef",
     "TableResourceOutputTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartQueryPlanningResponseTypeDef",
     "StartTransactionRequestRequestTypeDef",
-    "StartTransactionResponseTypeDef",
     "UpdateLFTagRequestRequestTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "UpdateTableStorageOptimizerRequestRequestTypeDef",
+    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
+    "CommitTransactionResponseTypeDef",
+    "GetLFTagResponseTypeDef",
+    "GetQueryStateResponseTypeDef",
+    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
+    "GetTemporaryGlueTableCredentialsResponseTypeDef",
+    "GetWorkUnitResultsResponseTypeDef",
+    "StartQueryPlanningResponseTypeDef",
+    "StartTransactionResponseTypeDef",
     "UpdateTableStorageOptimizerResponseTypeDef",
     "GetTemporaryGlueTableCredentialsRequestRequestTypeDef",
     "PrincipalPermissionsOutputTypeDef",
     "PrincipalPermissionsTypeDef",
     "ColumnLFTagTypeDef",
     "LFTagErrorTypeDef",
     "ListLFTagsResponseTypeDef",
@@ -132,14 +130,16 @@
     "DescribeResourceResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "DescribeTransactionResponseTypeDef",
     "ListTransactionsResponseTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "GetQueryStatisticsResponseTypeDef",
     "GetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
+    "GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    "ListLFTagsRequestListLFTagsPaginateTypeDef",
     "GetWorkUnitsResponseTypeDef",
     "LFTagPolicyResourceOutputTypeDef",
     "LFTagPolicyResourceTypeDef",
     "SearchDatabasesByLFTagsRequestRequestTypeDef",
     "SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
     "SearchTablesByLFTagsRequestRequestTypeDef",
     "SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
@@ -200,14 +200,25 @@
 )
 
 
 class LFTagPairTypeDef(_RequiredLFTagPairTypeDef, _OptionalLFTagPairTypeDef):
     pass
 
 
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
 _RequiredAddObjectInputTypeDef = TypedDict(
     "_RequiredAddObjectInputTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
@@ -245,48 +256,35 @@
 class AssumeDecoratedRoleWithSAMLRequestRequestTypeDef(
     _RequiredAssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
     _OptionalAssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
 ):
     pass
 
 
-AssumeDecoratedRoleWithSAMLResponseTypeDef = TypedDict(
-    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AuditContextTypeDef = TypedDict(
     "AuditContextTypeDef",
     {
         "AdditionalAuditContext": str,
     },
     total=False,
 )
 
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 DataLakePrincipalOutputTypeDef = TypedDict(
     "DataLakePrincipalOutputTypeDef",
     {
         "DataLakePrincipalIdentifier": str,
     },
-    total=False,
 )
 
 DataLakePrincipalTypeDef = TypedDict(
     "DataLakePrincipalTypeDef",
     {
         "DataLakePrincipalIdentifier": str,
     },
@@ -296,40 +294,28 @@
 CancelTransactionRequestRequestTypeDef = TypedDict(
     "CancelTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
-_RequiredLFTagPairOutputTypeDef = TypedDict(
-    "_RequiredLFTagPairOutputTypeDef",
+LFTagPairOutputTypeDef = TypedDict(
+    "LFTagPairOutputTypeDef",
     {
+        "CatalogId": str,
         "TagKey": str,
         "TagValues": List[str],
     },
 )
-_OptionalLFTagPairOutputTypeDef = TypedDict(
-    "_OptionalLFTagPairOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class LFTagPairOutputTypeDef(_RequiredLFTagPairOutputTypeDef, _OptionalLFTagPairOutputTypeDef):
-    pass
-
 
 ColumnWildcardOutputTypeDef = TypedDict(
     "ColumnWildcardOutputTypeDef",
     {
         "ExcludedColumnNames": List[str],
     },
-    total=False,
 )
 
 ColumnWildcardTypeDef = TypedDict(
     "ColumnWildcardTypeDef",
     {
         "ExcludedColumnNames": Sequence[str],
     },
@@ -339,22 +325,14 @@
 CommitTransactionRequestRequestTypeDef = TypedDict(
     "CommitTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
-CommitTransactionResponseTypeDef = TypedDict(
-    "CommitTransactionResponseTypeDef",
-    {
-        "TransactionStatus": TransactionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateLFTagRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLFTagRequestRequestTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -375,26 +353,24 @@
 
 RowFilterOutputTypeDef = TypedDict(
     "RowFilterOutputTypeDef",
     {
         "FilterExpression": str,
         "AllRowsWildcard": Dict[str, Any],
     },
-    total=False,
 )
 
 DataCellsFilterResourceOutputTypeDef = TypedDict(
     "DataCellsFilterResourceOutputTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
     },
-    total=False,
 )
 
 DataCellsFilterResourceTypeDef = TypedDict(
     "DataCellsFilterResourceTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
@@ -409,35 +385,22 @@
     {
         "FilterExpression": str,
         "AllRowsWildcard": Mapping[str, Any],
     },
     total=False,
 )
 
-_RequiredDataLocationResourceOutputTypeDef = TypedDict(
-    "_RequiredDataLocationResourceOutputTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalDataLocationResourceOutputTypeDef = TypedDict(
-    "_OptionalDataLocationResourceOutputTypeDef",
+DataLocationResourceOutputTypeDef = TypedDict(
+    "DataLocationResourceOutputTypeDef",
     {
         "CatalogId": str,
+        "ResourceArn": str,
     },
-    total=False,
 )
 
-
-class DataLocationResourceOutputTypeDef(
-    _RequiredDataLocationResourceOutputTypeDef, _OptionalDataLocationResourceOutputTypeDef
-):
-    pass
-
-
 _RequiredDataLocationResourceTypeDef = TypedDict(
     "_RequiredDataLocationResourceTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalDataLocationResourceTypeDef = TypedDict(
@@ -451,35 +414,22 @@
 
 class DataLocationResourceTypeDef(
     _RequiredDataLocationResourceTypeDef, _OptionalDataLocationResourceTypeDef
 ):
     pass
 
 
-_RequiredDatabaseResourceOutputTypeDef = TypedDict(
-    "_RequiredDatabaseResourceOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalDatabaseResourceOutputTypeDef = TypedDict(
-    "_OptionalDatabaseResourceOutputTypeDef",
+DatabaseResourceOutputTypeDef = TypedDict(
+    "DatabaseResourceOutputTypeDef",
     {
         "CatalogId": str,
+        "Name": str,
     },
-    total=False,
 )
 
-
-class DatabaseResourceOutputTypeDef(
-    _RequiredDatabaseResourceOutputTypeDef, _OptionalDatabaseResourceOutputTypeDef
-):
-    pass
-
-
 _RequiredDatabaseResourceTypeDef = TypedDict(
     "_RequiredDatabaseResourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDatabaseResourceTypeDef = TypedDict(
@@ -586,15 +536,14 @@
     "ResourceInfoTypeDef",
     {
         "ResourceArn": str,
         "RoleArn": str,
         "LastModified": datetime,
         "WithFederation": bool,
     },
-    total=False,
 )
 
 DescribeTransactionRequestRequestTypeDef = TypedDict(
     "DescribeTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
@@ -604,33 +553,30 @@
     "TransactionDescriptionTypeDef",
     {
         "TransactionId": str,
         "TransactionStatus": TransactionStatusType,
         "TransactionStartTime": datetime,
         "TransactionEndTime": datetime,
     },
-    total=False,
 )
 
 DetailsMapTypeDef = TypedDict(
     "DetailsMapTypeDef",
     {
         "ResourceShare": List[str],
     },
-    total=False,
 )
 
 ExecutionStatisticsTypeDef = TypedDict(
     "ExecutionStatisticsTypeDef",
     {
         "AverageExecutionTimeMillis": int,
         "DataScannedBytes": int,
         "WorkUnitsExecutedCount": int,
     },
-    total=False,
 )
 
 ExtendTransactionRequestRequestTypeDef = TypedDict(
     "ExtendTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
@@ -706,40 +652,21 @@
 
 class GetLFTagRequestRequestTypeDef(
     _RequiredGetLFTagRequestRequestTypeDef, _OptionalGetLFTagRequestRequestTypeDef
 ):
     pass
 
 
-GetLFTagResponseTypeDef = TypedDict(
-    "GetLFTagResponseTypeDef",
-    {
-        "CatalogId": str,
-        "TagKey": str,
-        "TagValues": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetQueryStateRequestRequestTypeDef = TypedDict(
     "GetQueryStateRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
-GetQueryStateResponseTypeDef = TypedDict(
-    "GetQueryStateResponseTypeDef",
-    {
-        "Error": str,
-        "State": QueryStateStringType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetQueryStatisticsRequestRequestTypeDef = TypedDict(
     "GetQueryStatisticsRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
@@ -747,15 +674,14 @@
     "PlanningStatisticsTypeDef",
     {
         "EstimatedDataToScanBytes": int,
         "PlanningTimeMillis": int,
         "QueueTimeMillis": int,
         "WorkUnitsGeneratedCount": int,
     },
-    total=False,
 )
 
 _RequiredGetTableObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableObjectsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
@@ -784,75 +710,33 @@
 PartitionValueListTypeDef = TypedDict(
     "PartitionValueListTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 
-GetTemporaryGluePartitionCredentialsResponseTypeDef = TypedDict(
-    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetTemporaryGlueTableCredentialsResponseTypeDef = TypedDict(
-    "GetTemporaryGlueTableCredentialsResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkUnitResultsRequestRequestTypeDef = TypedDict(
     "GetWorkUnitResultsRequestRequestTypeDef",
     {
         "QueryId": str,
         "WorkUnitId": int,
         "WorkUnitToken": str,
     },
 )
 
-GetWorkUnitResultsResponseTypeDef = TypedDict(
-    "GetWorkUnitResultsResponseTypeDef",
-    {
-        "ResultStream": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
-    "_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
-    {
-        "QueryId": str,
-    },
-)
-_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
-    "_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
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
-class GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef(
-    _RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
-    _OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetWorkUnitsRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkUnitsRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 _OptionalGetWorkUnitsRequestRequestTypeDef = TypedDict(
@@ -876,35 +760,22 @@
     {
         "WorkUnitIdMax": int,
         "WorkUnitIdMin": int,
         "WorkUnitToken": str,
     },
 )
 
-_RequiredLFTagKeyResourceOutputTypeDef = TypedDict(
-    "_RequiredLFTagKeyResourceOutputTypeDef",
+LFTagKeyResourceOutputTypeDef = TypedDict(
+    "LFTagKeyResourceOutputTypeDef",
     {
+        "CatalogId": str,
         "TagKey": str,
         "TagValues": List[str],
     },
 )
-_OptionalLFTagKeyResourceOutputTypeDef = TypedDict(
-    "_OptionalLFTagKeyResourceOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class LFTagKeyResourceOutputTypeDef(
-    _RequiredLFTagKeyResourceOutputTypeDef, _OptionalLFTagKeyResourceOutputTypeDef
-):
-    pass
-
 
 _RequiredLFTagKeyResourceTypeDef = TypedDict(
     "_RequiredLFTagKeyResourceTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
@@ -955,24 +826,14 @@
 )
 
 
 class TableResourceTypeDef(_RequiredTableResourceTypeDef, _OptionalTableResourceTypeDef):
     pass
 
 
-ListLFTagsRequestListLFTagsPaginateTypeDef = TypedDict(
-    "ListLFTagsRequestListLFTagsPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "ResourceShareType": ResourceShareTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLFTagsRequestRequestTypeDef = TypedDict(
     "ListLFTagsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "ResourceShareType": ResourceShareTypeType,
         "MaxResults": int,
         "NextToken": str,
@@ -1011,46 +872,34 @@
     {
         "StorageOptimizerType": OptimizerTypeType,
         "Config": Dict[str, str],
         "ErrorMessage": str,
         "Warnings": str,
         "LastRunDetails": str,
     },
-    total=False,
 )
 
 ListTransactionsRequestRequestTypeDef = TypedDict(
     "ListTransactionsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "StatusFilter": TransactionStatusFilterType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
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
 TableObjectTypeDef = TypedDict(
     "TableObjectTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
-    total=False,
 )
 
 _RequiredQueryPlanningContextTypeDef = TypedDict(
     "_RequiredQueryPlanningContextTypeDef",
     {
         "DatabaseName": str,
     },
@@ -1092,72 +941,32 @@
 
 class RegisterResourceRequestRequestTypeDef(
     _RequiredRegisterResourceRequestRequestTypeDef, _OptionalRegisterResourceRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredTableResourceOutputTypeDef = TypedDict(
-    "_RequiredTableResourceOutputTypeDef",
-    {
-        "DatabaseName": str,
-    },
-)
-_OptionalTableResourceOutputTypeDef = TypedDict(
-    "_OptionalTableResourceOutputTypeDef",
+TableResourceOutputTypeDef = TypedDict(
+    "TableResourceOutputTypeDef",
     {
         "CatalogId": str,
+        "DatabaseName": str,
         "Name": str,
         "TableWildcard": Dict[str, Any],
     },
-    total=False,
-)
-
-
-class TableResourceOutputTypeDef(
-    _RequiredTableResourceOutputTypeDef, _OptionalTableResourceOutputTypeDef
-):
-    pass
-
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
-StartQueryPlanningResponseTypeDef = TypedDict(
-    "StartQueryPlanningResponseTypeDef",
-    {
-        "QueryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 StartTransactionRequestRequestTypeDef = TypedDict(
     "StartTransactionRequestRequestTypeDef",
     {
         "TransactionType": TransactionTypeType,
     },
     total=False,
 )
 
-StartTransactionResponseTypeDef = TypedDict(
-    "StartTransactionResponseTypeDef",
-    {
-        "TransactionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateLFTagRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLFTagRequestRequestTypeDef",
     {
         "TagKey": str,
     },
 )
 _OptionalUpdateLFTagRequestRequestTypeDef = TypedDict(
@@ -1219,19 +1028,103 @@
 class UpdateTableStorageOptimizerRequestRequestTypeDef(
     _RequiredUpdateTableStorageOptimizerRequestRequestTypeDef,
     _OptionalUpdateTableStorageOptimizerRequestRequestTypeDef,
 ):
     pass
 
 
+AssumeDecoratedRoleWithSAMLResponseTypeDef = TypedDict(
+    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
+    {
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CommitTransactionResponseTypeDef = TypedDict(
+    "CommitTransactionResponseTypeDef",
+    {
+        "TransactionStatus": TransactionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLFTagResponseTypeDef = TypedDict(
+    "GetLFTagResponseTypeDef",
+    {
+        "CatalogId": str,
+        "TagKey": str,
+        "TagValues": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetQueryStateResponseTypeDef = TypedDict(
+    "GetQueryStateResponseTypeDef",
+    {
+        "Error": str,
+        "State": QueryStateStringType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTemporaryGluePartitionCredentialsResponseTypeDef = TypedDict(
+    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
+    {
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTemporaryGlueTableCredentialsResponseTypeDef = TypedDict(
+    "GetTemporaryGlueTableCredentialsResponseTypeDef",
+    {
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkUnitResultsResponseTypeDef = TypedDict(
+    "GetWorkUnitResultsResponseTypeDef",
+    {
+        "ResultStream": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartQueryPlanningResponseTypeDef = TypedDict(
+    "StartQueryPlanningResponseTypeDef",
+    {
+        "QueryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartTransactionResponseTypeDef = TypedDict(
+    "StartTransactionResponseTypeDef",
+    {
+        "TransactionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateTableStorageOptimizerResponseTypeDef = TypedDict(
     "UpdateTableStorageOptimizerResponseTypeDef",
     {
         "Result": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef",
     {
         "TableArn": str,
@@ -1258,15 +1151,14 @@
 
 PrincipalPermissionsOutputTypeDef = TypedDict(
     "PrincipalPermissionsOutputTypeDef",
     {
         "Principal": DataLakePrincipalOutputTypeDef,
         "Permissions": List[PermissionType],
     },
-    total=False,
 )
 
 PrincipalPermissionsTypeDef = TypedDict(
     "PrincipalPermissionsTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
         "Permissions": Sequence[PermissionType],
@@ -1276,59 +1168,44 @@
 
 ColumnLFTagTypeDef = TypedDict(
     "ColumnLFTagTypeDef",
     {
         "Name": str,
         "LFTags": List[LFTagPairOutputTypeDef],
     },
-    total=False,
 )
 
 LFTagErrorTypeDef = TypedDict(
     "LFTagErrorTypeDef",
     {
         "LFTag": LFTagPairOutputTypeDef,
         "Error": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 ListLFTagsResponseTypeDef = TypedDict(
     "ListLFTagsResponseTypeDef",
     {
         "LFTags": List[LFTagPairOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredTableWithColumnsResourceOutputTypeDef = TypedDict(
-    "_RequiredTableWithColumnsResourceOutputTypeDef",
+TableWithColumnsResourceOutputTypeDef = TypedDict(
+    "TableWithColumnsResourceOutputTypeDef",
     {
+        "CatalogId": str,
         "DatabaseName": str,
         "Name": str,
-    },
-)
-_OptionalTableWithColumnsResourceOutputTypeDef = TypedDict(
-    "_OptionalTableWithColumnsResourceOutputTypeDef",
-    {
-        "CatalogId": str,
         "ColumnNames": List[str],
         "ColumnWildcard": ColumnWildcardOutputTypeDef,
     },
-    total=False,
 )
 
-
-class TableWithColumnsResourceOutputTypeDef(
-    _RequiredTableWithColumnsResourceOutputTypeDef, _OptionalTableWithColumnsResourceOutputTypeDef
-):
-    pass
-
-
 _RequiredTableWithColumnsResourceTypeDef = TypedDict(
     "_RequiredTableWithColumnsResourceTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -1345,41 +1222,28 @@
 
 class TableWithColumnsResourceTypeDef(
     _RequiredTableWithColumnsResourceTypeDef, _OptionalTableWithColumnsResourceTypeDef
 ):
     pass
 
 
-_RequiredDataCellsFilterOutputTypeDef = TypedDict(
-    "_RequiredDataCellsFilterOutputTypeDef",
+DataCellsFilterOutputTypeDef = TypedDict(
+    "DataCellsFilterOutputTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
-    },
-)
-_OptionalDataCellsFilterOutputTypeDef = TypedDict(
-    "_OptionalDataCellsFilterOutputTypeDef",
-    {
         "RowFilter": RowFilterOutputTypeDef,
         "ColumnNames": List[str],
         "ColumnWildcard": ColumnWildcardOutputTypeDef,
         "VersionId": str,
     },
-    total=False,
 )
 
-
-class DataCellsFilterOutputTypeDef(
-    _RequiredDataCellsFilterOutputTypeDef, _OptionalDataCellsFilterOutputTypeDef
-):
-    pass
-
-
 _RequiredDataCellsFilterTypeDef = TypedDict(
     "_RequiredDataCellsFilterTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
@@ -1403,15 +1267,14 @@
 
 TaggedDatabaseTypeDef = TypedDict(
     "TaggedDatabaseTypeDef",
     {
         "Database": DatabaseResourceOutputTypeDef,
         "LFTags": List[LFTagPairOutputTypeDef],
     },
-    total=False,
 )
 
 WriteOperationTypeDef = TypedDict(
     "WriteOperationTypeDef",
     {
         "AddObject": AddObjectInputTypeDef,
         "DeleteObject": DeleteObjectInputTypeDef,
@@ -1444,41 +1307,41 @@
     pass
 
 
 DescribeResourceResponseTypeDef = TypedDict(
     "DescribeResourceResponseTypeDef",
     {
         "ResourceInfo": ResourceInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesResponseTypeDef = TypedDict(
     "ListResourcesResponseTypeDef",
     {
         "ResourceInfoList": List[ResourceInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTransactionResponseTypeDef = TypedDict(
     "DescribeTransactionResponseTypeDef",
     {
         "TransactionDescription": TransactionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTransactionsResponseTypeDef = TypedDict(
     "ListTransactionsResponseTypeDef",
     {
         "Transactions": List[TransactionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesRequestRequestTypeDef = TypedDict(
     "ListResourcesRequestRequestTypeDef",
     {
         "FilterConditionList": Sequence[FilterConditionTypeDef],
@@ -1490,15 +1353,15 @@
 
 GetQueryStatisticsResponseTypeDef = TypedDict(
     "GetQueryStatisticsResponseTypeDef",
     {
         "ExecutionStatistics": ExecutionStatisticsTypeDef,
         "PlanningStatistics": PlanningStatisticsTypeDef,
         "QuerySubmissionTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     {
         "TableArn": str,
@@ -1520,45 +1383,64 @@
 class GetTemporaryGluePartitionCredentialsRequestRequestTypeDef(
     _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
     _OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
 ):
     pass
 
 
-GetWorkUnitsResponseTypeDef = TypedDict(
-    "GetWorkUnitsResponseTypeDef",
+_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
+    "_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
     {
-        "NextToken": str,
         "QueryId": str,
-        "WorkUnitRanges": List[WorkUnitRangeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-
-_RequiredLFTagPolicyResourceOutputTypeDef = TypedDict(
-    "_RequiredLFTagPolicyResourceOutputTypeDef",
+_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
+    "_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
     {
-        "ResourceType": ResourceTypeType,
-        "Expression": List[LFTagOutputTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalLFTagPolicyResourceOutputTypeDef = TypedDict(
-    "_OptionalLFTagPolicyResourceOutputTypeDef",
+
+
+class GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef(
+    _RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    _OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+):
+    pass
+
+
+ListLFTagsRequestListLFTagsPaginateTypeDef = TypedDict(
+    "ListLFTagsRequestListLFTagsPaginateTypeDef",
     {
         "CatalogId": str,
+        "ResourceShareType": ResourceShareTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+GetWorkUnitsResponseTypeDef = TypedDict(
+    "GetWorkUnitsResponseTypeDef",
+    {
+        "NextToken": str,
+        "QueryId": str,
+        "WorkUnitRanges": List[WorkUnitRangeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class LFTagPolicyResourceOutputTypeDef(
-    _RequiredLFTagPolicyResourceOutputTypeDef, _OptionalLFTagPolicyResourceOutputTypeDef
-):
-    pass
-
+LFTagPolicyResourceOutputTypeDef = TypedDict(
+    "LFTagPolicyResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "ResourceType": ResourceTypeType,
+        "Expression": List[LFTagOutputTypeDef],
+    },
+)
 
 _RequiredLFTagPolicyResourceTypeDef = TypedDict(
     "_RequiredLFTagPolicyResourceTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "Expression": Sequence[LFTagTypeDef],
     },
@@ -1608,15 +1490,15 @@
         "Expression": Sequence[LFTagTypeDef],
     },
 )
 _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
     "_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
     {
         "CatalogId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef(
     _RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
@@ -1655,15 +1537,15 @@
         "Expression": Sequence[LFTagTypeDef],
     },
 )
 _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
     "_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     {
         "CatalogId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef(
     _RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
@@ -1672,15 +1554,15 @@
     pass
 
 
 ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef = TypedDict(
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     {
         "Table": TableResourceTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListDataCellsFilterRequestRequestTypeDef = TypedDict(
     "ListDataCellsFilterRequestRequestTypeDef",
     {
@@ -1692,25 +1574,24 @@
 )
 
 ListTableStorageOptimizersResponseTypeDef = TypedDict(
     "ListTableStorageOptimizersResponseTypeDef",
     {
         "StorageOptimizerList": List[StorageOptimizerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PartitionObjectsTypeDef = TypedDict(
     "PartitionObjectsTypeDef",
     {
         "PartitionValues": List[str],
         "Objects": List[TableObjectTypeDef],
     },
-    total=False,
 )
 
 StartQueryPlanningRequestRequestTypeDef = TypedDict(
     "StartQueryPlanningRequestRequestTypeDef",
     {
         "QueryPlanningContext": QueryPlanningContextTypeDef,
         "QueryString": str,
@@ -1727,15 +1608,14 @@
         "Parameters": Dict[str, str],
         "TrustedResourceOwners": List[str],
         "AllowExternalDataFiltering": bool,
         "AllowFullTableExternalDataAccess": bool,
         "ExternalDataFilteringAllowList": List[DataLakePrincipalOutputTypeDef],
         "AuthorizedSessionTagValueList": List[str],
     },
-    total=False,
 )
 
 DataLakeSettingsTypeDef = TypedDict(
     "DataLakeSettingsTypeDef",
     {
         "DataLakeAdmins": Sequence[DataLakePrincipalTypeDef],
         "ReadOnlyAdmins": Sequence[DataLakePrincipalTypeDef],
@@ -1753,59 +1633,58 @@
 
 GetResourceLFTagsResponseTypeDef = TypedDict(
     "GetResourceLFTagsResponseTypeDef",
     {
         "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
         "LFTagsOnTable": List[LFTagPairOutputTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TaggedTableTypeDef = TypedDict(
     "TaggedTableTypeDef",
     {
         "Table": TableResourceOutputTypeDef,
         "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
         "LFTagsOnTable": List[LFTagPairOutputTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
     },
-    total=False,
 )
 
 AddLFTagsToResourceResponseTypeDef = TypedDict(
     "AddLFTagsToResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveLFTagsFromResourceResponseTypeDef = TypedDict(
     "RemoveLFTagsFromResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataCellsFilterResponseTypeDef = TypedDict(
     "GetDataCellsFilterResponseTypeDef",
     {
         "DataCellsFilter": DataCellsFilterOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataCellsFilterResponseTypeDef = TypedDict(
     "ListDataCellsFilterResponseTypeDef",
     {
         "DataCellsFilters": List[DataCellsFilterOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDataCellsFilterRequestRequestTypeDef = TypedDict(
     "CreateDataCellsFilterRequestRequestTypeDef",
     {
         "TableData": DataCellsFilterTypeDef,
@@ -1820,15 +1699,15 @@
 )
 
 SearchDatabasesByLFTagsResponseTypeDef = TypedDict(
     "SearchDatabasesByLFTagsResponseTypeDef",
     {
         "NextToken": str,
         "DatabaseList": List[TaggedDatabaseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateTableObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableObjectsRequestRequestTypeDef",
     {
         "DatabaseName": str,
@@ -1861,15 +1740,14 @@
         "Table": TableResourceOutputTypeDef,
         "TableWithColumns": TableWithColumnsResourceOutputTypeDef,
         "DataLocation": DataLocationResourceOutputTypeDef,
         "DataCellsFilter": DataCellsFilterResourceOutputTypeDef,
         "LFTag": LFTagKeyResourceOutputTypeDef,
         "LFTagPolicy": LFTagPolicyResourceOutputTypeDef,
     },
-    total=False,
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Catalog": Mapping[str, Any],
         "Database": DatabaseResourceTypeDef,
@@ -1884,23 +1762,23 @@
 )
 
 GetTableObjectsResponseTypeDef = TypedDict(
     "GetTableObjectsResponseTypeDef",
     {
         "Objects": List[PartitionObjectsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataLakeSettingsResponseTypeDef = TypedDict(
     "GetDataLakeSettingsResponseTypeDef",
     {
         "DataLakeSettings": DataLakeSettingsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutDataLakeSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredPutDataLakeSettingsRequestRequestTypeDef",
     {
         "DataLakeSettings": DataLakeSettingsTypeDef,
@@ -1923,53 +1801,38 @@
 
 
 SearchTablesByLFTagsResponseTypeDef = TypedDict(
     "SearchTablesByLFTagsResponseTypeDef",
     {
         "NextToken": str,
         "TableList": List[TaggedTableTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
-    "_RequiredBatchPermissionsRequestEntryOutputTypeDef",
+BatchPermissionsRequestEntryOutputTypeDef = TypedDict(
+    "BatchPermissionsRequestEntryOutputTypeDef",
     {
         "Id": str,
-    },
-)
-_OptionalBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
-    "_OptionalBatchPermissionsRequestEntryOutputTypeDef",
-    {
         "Principal": DataLakePrincipalOutputTypeDef,
         "Resource": ResourceOutputTypeDef,
         "Permissions": List[PermissionType],
         "PermissionsWithGrantOption": List[PermissionType],
     },
-    total=False,
 )
 
-
-class BatchPermissionsRequestEntryOutputTypeDef(
-    _RequiredBatchPermissionsRequestEntryOutputTypeDef,
-    _OptionalBatchPermissionsRequestEntryOutputTypeDef,
-):
-    pass
-
-
 PrincipalResourcePermissionsTypeDef = TypedDict(
     "PrincipalResourcePermissionsTypeDef",
     {
         "Principal": DataLakePrincipalOutputTypeDef,
         "Resource": ResourceOutputTypeDef,
         "Permissions": List[PermissionType],
         "PermissionsWithGrantOption": List[PermissionType],
         "AdditionalDetails": DetailsMapTypeDef,
     },
-    total=False,
 )
 
 _RequiredAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_RequiredAddLFTagsToResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
         "LFTags": Sequence[LFTagPairTypeDef],
@@ -2124,32 +1987,31 @@
 
 BatchPermissionsFailureEntryTypeDef = TypedDict(
     "BatchPermissionsFailureEntryTypeDef",
     {
         "RequestEntry": BatchPermissionsRequestEntryOutputTypeDef,
         "Error": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 GetEffectivePermissionsForPathResponseTypeDef = TypedDict(
     "GetEffectivePermissionsForPathResponseTypeDef",
     {
         "Permissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPermissionsResponseTypeDef = TypedDict(
     "ListPermissionsResponseTypeDef",
     {
         "PrincipalResourcePermissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGrantPermissionsRequestRequestTypeDef",
     {
         "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
@@ -2193,18 +2055,18 @@
     pass
 
 
 BatchGrantPermissionsResponseTypeDef = TypedDict(
     "BatchGrantPermissionsResponseTypeDef",
     {
         "Failures": List[BatchPermissionsFailureEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchRevokePermissionsResponseTypeDef = TypedDict(
     "BatchRevokePermissionsResponseTypeDef",
     {
         "Failures": List[BatchPermissionsFailureEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation/type_defs.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -35,27 +35,26 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "LFTagPairTypeDef",
+    "ResponseMetadataTypeDef",
     "AddObjectInputTypeDef",
     "AssumeDecoratedRoleWithSAMLRequestRequestTypeDef",
-    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
     "AuditContextTypeDef",
     "ErrorDetailTypeDef",
     "DataLakePrincipalOutputTypeDef",
     "DataLakePrincipalTypeDef",
     "CancelTransactionRequestRequestTypeDef",
     "LFTagPairOutputTypeDef",
     "ColumnWildcardOutputTypeDef",
     "ColumnWildcardTypeDef",
     "CommitTransactionRequestRequestTypeDef",
-    "CommitTransactionResponseTypeDef",
     "CreateLFTagRequestRequestTypeDef",
     "RowFilterOutputTypeDef",
     "DataCellsFilterResourceOutputTypeDef",
     "DataCellsFilterResourceTypeDef",
     "RowFilterTypeDef",
     "DataLocationResourceOutputTypeDef",
     "DataLocationResourceTypeDef",
@@ -74,50 +73,49 @@
     "ExecutionStatisticsTypeDef",
     "ExtendTransactionRequestRequestTypeDef",
     "FilterConditionTypeDef",
     "GetDataCellsFilterRequestRequestTypeDef",
     "GetDataLakeSettingsRequestRequestTypeDef",
     "GetEffectivePermissionsForPathRequestRequestTypeDef",
     "GetLFTagRequestRequestTypeDef",
-    "GetLFTagResponseTypeDef",
     "GetQueryStateRequestRequestTypeDef",
-    "GetQueryStateResponseTypeDef",
     "GetQueryStatisticsRequestRequestTypeDef",
     "PlanningStatisticsTypeDef",
     "GetTableObjectsRequestRequestTypeDef",
     "PartitionValueListTypeDef",
-    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
-    "GetTemporaryGlueTableCredentialsResponseTypeDef",
     "GetWorkUnitResultsRequestRequestTypeDef",
-    "GetWorkUnitResultsResponseTypeDef",
-    "GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetWorkUnitsRequestRequestTypeDef",
     "WorkUnitRangeTypeDef",
     "LFTagKeyResourceOutputTypeDef",
     "LFTagKeyResourceTypeDef",
     "LFTagOutputTypeDef",
     "LFTagTypeDef",
     "TableResourceTypeDef",
-    "ListLFTagsRequestListLFTagsPaginateTypeDef",
     "ListLFTagsRequestRequestTypeDef",
     "ListTableStorageOptimizersRequestRequestTypeDef",
     "StorageOptimizerTypeDef",
     "ListTransactionsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "TableObjectTypeDef",
     "QueryPlanningContextTypeDef",
     "RegisterResourceRequestRequestTypeDef",
     "TableResourceOutputTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartQueryPlanningResponseTypeDef",
     "StartTransactionRequestRequestTypeDef",
-    "StartTransactionResponseTypeDef",
     "UpdateLFTagRequestRequestTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "UpdateTableStorageOptimizerRequestRequestTypeDef",
+    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
+    "CommitTransactionResponseTypeDef",
+    "GetLFTagResponseTypeDef",
+    "GetQueryStateResponseTypeDef",
+    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
+    "GetTemporaryGlueTableCredentialsResponseTypeDef",
+    "GetWorkUnitResultsResponseTypeDef",
+    "StartQueryPlanningResponseTypeDef",
+    "StartTransactionResponseTypeDef",
     "UpdateTableStorageOptimizerResponseTypeDef",
     "GetTemporaryGlueTableCredentialsRequestRequestTypeDef",
     "PrincipalPermissionsOutputTypeDef",
     "PrincipalPermissionsTypeDef",
     "ColumnLFTagTypeDef",
     "LFTagErrorTypeDef",
     "ListLFTagsResponseTypeDef",
@@ -131,14 +129,16 @@
     "DescribeResourceResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "DescribeTransactionResponseTypeDef",
     "ListTransactionsResponseTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "GetQueryStatisticsResponseTypeDef",
     "GetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
+    "GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    "ListLFTagsRequestListLFTagsPaginateTypeDef",
     "GetWorkUnitsResponseTypeDef",
     "LFTagPolicyResourceOutputTypeDef",
     "LFTagPolicyResourceTypeDef",
     "SearchDatabasesByLFTagsRequestRequestTypeDef",
     "SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
     "SearchTablesByLFTagsRequestRequestTypeDef",
     "SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
@@ -197,14 +197,25 @@
     },
     total=False,
 )
 
 class LFTagPairTypeDef(_RequiredLFTagPairTypeDef, _OptionalLFTagPairTypeDef):
     pass
 
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
 _RequiredAddObjectInputTypeDef = TypedDict(
     "_RequiredAddObjectInputTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
@@ -238,48 +249,35 @@
 
 class AssumeDecoratedRoleWithSAMLRequestRequestTypeDef(
     _RequiredAssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
     _OptionalAssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
 ):
     pass
 
-AssumeDecoratedRoleWithSAMLResponseTypeDef = TypedDict(
-    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AuditContextTypeDef = TypedDict(
     "AuditContextTypeDef",
     {
         "AdditionalAuditContext": str,
     },
     total=False,
 )
 
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 DataLakePrincipalOutputTypeDef = TypedDict(
     "DataLakePrincipalOutputTypeDef",
     {
         "DataLakePrincipalIdentifier": str,
     },
-    total=False,
 )
 
 DataLakePrincipalTypeDef = TypedDict(
     "DataLakePrincipalTypeDef",
     {
         "DataLakePrincipalIdentifier": str,
     },
@@ -289,38 +287,28 @@
 CancelTransactionRequestRequestTypeDef = TypedDict(
     "CancelTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
-_RequiredLFTagPairOutputTypeDef = TypedDict(
-    "_RequiredLFTagPairOutputTypeDef",
+LFTagPairOutputTypeDef = TypedDict(
+    "LFTagPairOutputTypeDef",
     {
+        "CatalogId": str,
         "TagKey": str,
         "TagValues": List[str],
     },
 )
-_OptionalLFTagPairOutputTypeDef = TypedDict(
-    "_OptionalLFTagPairOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class LFTagPairOutputTypeDef(_RequiredLFTagPairOutputTypeDef, _OptionalLFTagPairOutputTypeDef):
-    pass
 
 ColumnWildcardOutputTypeDef = TypedDict(
     "ColumnWildcardOutputTypeDef",
     {
         "ExcludedColumnNames": List[str],
     },
-    total=False,
 )
 
 ColumnWildcardTypeDef = TypedDict(
     "ColumnWildcardTypeDef",
     {
         "ExcludedColumnNames": Sequence[str],
     },
@@ -330,22 +318,14 @@
 CommitTransactionRequestRequestTypeDef = TypedDict(
     "CommitTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
-CommitTransactionResponseTypeDef = TypedDict(
-    "CommitTransactionResponseTypeDef",
-    {
-        "TransactionStatus": TransactionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateLFTagRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLFTagRequestRequestTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -364,26 +344,24 @@
 
 RowFilterOutputTypeDef = TypedDict(
     "RowFilterOutputTypeDef",
     {
         "FilterExpression": str,
         "AllRowsWildcard": Dict[str, Any],
     },
-    total=False,
 )
 
 DataCellsFilterResourceOutputTypeDef = TypedDict(
     "DataCellsFilterResourceOutputTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
     },
-    total=False,
 )
 
 DataCellsFilterResourceTypeDef = TypedDict(
     "DataCellsFilterResourceTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
@@ -398,33 +376,22 @@
     {
         "FilterExpression": str,
         "AllRowsWildcard": Mapping[str, Any],
     },
     total=False,
 )
 
-_RequiredDataLocationResourceOutputTypeDef = TypedDict(
-    "_RequiredDataLocationResourceOutputTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalDataLocationResourceOutputTypeDef = TypedDict(
-    "_OptionalDataLocationResourceOutputTypeDef",
+DataLocationResourceOutputTypeDef = TypedDict(
+    "DataLocationResourceOutputTypeDef",
     {
         "CatalogId": str,
+        "ResourceArn": str,
     },
-    total=False,
 )
 
-class DataLocationResourceOutputTypeDef(
-    _RequiredDataLocationResourceOutputTypeDef, _OptionalDataLocationResourceOutputTypeDef
-):
-    pass
-
 _RequiredDataLocationResourceTypeDef = TypedDict(
     "_RequiredDataLocationResourceTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalDataLocationResourceTypeDef = TypedDict(
@@ -436,33 +403,22 @@
 )
 
 class DataLocationResourceTypeDef(
     _RequiredDataLocationResourceTypeDef, _OptionalDataLocationResourceTypeDef
 ):
     pass
 
-_RequiredDatabaseResourceOutputTypeDef = TypedDict(
-    "_RequiredDatabaseResourceOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalDatabaseResourceOutputTypeDef = TypedDict(
-    "_OptionalDatabaseResourceOutputTypeDef",
+DatabaseResourceOutputTypeDef = TypedDict(
+    "DatabaseResourceOutputTypeDef",
     {
         "CatalogId": str,
+        "Name": str,
     },
-    total=False,
 )
 
-class DatabaseResourceOutputTypeDef(
-    _RequiredDatabaseResourceOutputTypeDef, _OptionalDatabaseResourceOutputTypeDef
-):
-    pass
-
 _RequiredDatabaseResourceTypeDef = TypedDict(
     "_RequiredDatabaseResourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDatabaseResourceTypeDef = TypedDict(
@@ -561,15 +517,14 @@
     "ResourceInfoTypeDef",
     {
         "ResourceArn": str,
         "RoleArn": str,
         "LastModified": datetime,
         "WithFederation": bool,
     },
-    total=False,
 )
 
 DescribeTransactionRequestRequestTypeDef = TypedDict(
     "DescribeTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
@@ -579,33 +534,30 @@
     "TransactionDescriptionTypeDef",
     {
         "TransactionId": str,
         "TransactionStatus": TransactionStatusType,
         "TransactionStartTime": datetime,
         "TransactionEndTime": datetime,
     },
-    total=False,
 )
 
 DetailsMapTypeDef = TypedDict(
     "DetailsMapTypeDef",
     {
         "ResourceShare": List[str],
     },
-    total=False,
 )
 
 ExecutionStatisticsTypeDef = TypedDict(
     "ExecutionStatisticsTypeDef",
     {
         "AverageExecutionTimeMillis": int,
         "DataScannedBytes": int,
         "WorkUnitsExecutedCount": int,
     },
-    total=False,
 )
 
 ExtendTransactionRequestRequestTypeDef = TypedDict(
     "ExtendTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
@@ -677,40 +629,21 @@
 )
 
 class GetLFTagRequestRequestTypeDef(
     _RequiredGetLFTagRequestRequestTypeDef, _OptionalGetLFTagRequestRequestTypeDef
 ):
     pass
 
-GetLFTagResponseTypeDef = TypedDict(
-    "GetLFTagResponseTypeDef",
-    {
-        "CatalogId": str,
-        "TagKey": str,
-        "TagValues": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetQueryStateRequestRequestTypeDef = TypedDict(
     "GetQueryStateRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
-GetQueryStateResponseTypeDef = TypedDict(
-    "GetQueryStateResponseTypeDef",
-    {
-        "Error": str,
-        "State": QueryStateStringType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetQueryStatisticsRequestRequestTypeDef = TypedDict(
     "GetQueryStatisticsRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
@@ -718,15 +651,14 @@
     "PlanningStatisticsTypeDef",
     {
         "EstimatedDataToScanBytes": int,
         "PlanningTimeMillis": int,
         "QueueTimeMillis": int,
         "WorkUnitsGeneratedCount": int,
     },
-    total=False,
 )
 
 _RequiredGetTableObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableObjectsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
@@ -753,73 +685,33 @@
 PartitionValueListTypeDef = TypedDict(
     "PartitionValueListTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 
-GetTemporaryGluePartitionCredentialsResponseTypeDef = TypedDict(
-    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetTemporaryGlueTableCredentialsResponseTypeDef = TypedDict(
-    "GetTemporaryGlueTableCredentialsResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkUnitResultsRequestRequestTypeDef = TypedDict(
     "GetWorkUnitResultsRequestRequestTypeDef",
     {
         "QueryId": str,
         "WorkUnitId": int,
         "WorkUnitToken": str,
     },
 )
 
-GetWorkUnitResultsResponseTypeDef = TypedDict(
-    "GetWorkUnitResultsResponseTypeDef",
-    {
-        "ResultStream": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
-    "_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
-    {
-        "QueryId": str,
-    },
-)
-_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
-    "_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
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
 
-class GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef(
-    _RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
-    _OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetWorkUnitsRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkUnitsRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 _OptionalGetWorkUnitsRequestRequestTypeDef = TypedDict(
@@ -841,33 +733,22 @@
     {
         "WorkUnitIdMax": int,
         "WorkUnitIdMin": int,
         "WorkUnitToken": str,
     },
 )
 
-_RequiredLFTagKeyResourceOutputTypeDef = TypedDict(
-    "_RequiredLFTagKeyResourceOutputTypeDef",
+LFTagKeyResourceOutputTypeDef = TypedDict(
+    "LFTagKeyResourceOutputTypeDef",
     {
+        "CatalogId": str,
         "TagKey": str,
         "TagValues": List[str],
     },
 )
-_OptionalLFTagKeyResourceOutputTypeDef = TypedDict(
-    "_OptionalLFTagKeyResourceOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class LFTagKeyResourceOutputTypeDef(
-    _RequiredLFTagKeyResourceOutputTypeDef, _OptionalLFTagKeyResourceOutputTypeDef
-):
-    pass
 
 _RequiredLFTagKeyResourceTypeDef = TypedDict(
     "_RequiredLFTagKeyResourceTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
@@ -914,24 +795,14 @@
     },
     total=False,
 )
 
 class TableResourceTypeDef(_RequiredTableResourceTypeDef, _OptionalTableResourceTypeDef):
     pass
 
-ListLFTagsRequestListLFTagsPaginateTypeDef = TypedDict(
-    "ListLFTagsRequestListLFTagsPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "ResourceShareType": ResourceShareTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLFTagsRequestRequestTypeDef = TypedDict(
     "ListLFTagsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "ResourceShareType": ResourceShareTypeType,
         "MaxResults": int,
         "NextToken": str,
@@ -968,46 +839,34 @@
     {
         "StorageOptimizerType": OptimizerTypeType,
         "Config": Dict[str, str],
         "ErrorMessage": str,
         "Warnings": str,
         "LastRunDetails": str,
     },
-    total=False,
 )
 
 ListTransactionsRequestRequestTypeDef = TypedDict(
     "ListTransactionsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "StatusFilter": TransactionStatusFilterType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
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
 TableObjectTypeDef = TypedDict(
     "TableObjectTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
-    total=False,
 )
 
 _RequiredQueryPlanningContextTypeDef = TypedDict(
     "_RequiredQueryPlanningContextTypeDef",
     {
         "DatabaseName": str,
     },
@@ -1045,70 +904,32 @@
 )
 
 class RegisterResourceRequestRequestTypeDef(
     _RequiredRegisterResourceRequestRequestTypeDef, _OptionalRegisterResourceRequestRequestTypeDef
 ):
     pass
 
-_RequiredTableResourceOutputTypeDef = TypedDict(
-    "_RequiredTableResourceOutputTypeDef",
-    {
-        "DatabaseName": str,
-    },
-)
-_OptionalTableResourceOutputTypeDef = TypedDict(
-    "_OptionalTableResourceOutputTypeDef",
+TableResourceOutputTypeDef = TypedDict(
+    "TableResourceOutputTypeDef",
     {
         "CatalogId": str,
+        "DatabaseName": str,
         "Name": str,
         "TableWildcard": Dict[str, Any],
     },
-    total=False,
-)
-
-class TableResourceOutputTypeDef(
-    _RequiredTableResourceOutputTypeDef, _OptionalTableResourceOutputTypeDef
-):
-    pass
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
-StartQueryPlanningResponseTypeDef = TypedDict(
-    "StartQueryPlanningResponseTypeDef",
-    {
-        "QueryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 StartTransactionRequestRequestTypeDef = TypedDict(
     "StartTransactionRequestRequestTypeDef",
     {
         "TransactionType": TransactionTypeType,
     },
     total=False,
 )
 
-StartTransactionResponseTypeDef = TypedDict(
-    "StartTransactionResponseTypeDef",
-    {
-        "TransactionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateLFTagRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLFTagRequestRequestTypeDef",
     {
         "TagKey": str,
     },
 )
 _OptionalUpdateLFTagRequestRequestTypeDef = TypedDict(
@@ -1164,19 +985,103 @@
 
 class UpdateTableStorageOptimizerRequestRequestTypeDef(
     _RequiredUpdateTableStorageOptimizerRequestRequestTypeDef,
     _OptionalUpdateTableStorageOptimizerRequestRequestTypeDef,
 ):
     pass
 
+AssumeDecoratedRoleWithSAMLResponseTypeDef = TypedDict(
+    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
+    {
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CommitTransactionResponseTypeDef = TypedDict(
+    "CommitTransactionResponseTypeDef",
+    {
+        "TransactionStatus": TransactionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLFTagResponseTypeDef = TypedDict(
+    "GetLFTagResponseTypeDef",
+    {
+        "CatalogId": str,
+        "TagKey": str,
+        "TagValues": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetQueryStateResponseTypeDef = TypedDict(
+    "GetQueryStateResponseTypeDef",
+    {
+        "Error": str,
+        "State": QueryStateStringType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTemporaryGluePartitionCredentialsResponseTypeDef = TypedDict(
+    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
+    {
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTemporaryGlueTableCredentialsResponseTypeDef = TypedDict(
+    "GetTemporaryGlueTableCredentialsResponseTypeDef",
+    {
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkUnitResultsResponseTypeDef = TypedDict(
+    "GetWorkUnitResultsResponseTypeDef",
+    {
+        "ResultStream": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartQueryPlanningResponseTypeDef = TypedDict(
+    "StartQueryPlanningResponseTypeDef",
+    {
+        "QueryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartTransactionResponseTypeDef = TypedDict(
+    "StartTransactionResponseTypeDef",
+    {
+        "TransactionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateTableStorageOptimizerResponseTypeDef = TypedDict(
     "UpdateTableStorageOptimizerResponseTypeDef",
     {
         "Result": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef",
     {
         "TableArn": str,
@@ -1201,15 +1106,14 @@
 
 PrincipalPermissionsOutputTypeDef = TypedDict(
     "PrincipalPermissionsOutputTypeDef",
     {
         "Principal": DataLakePrincipalOutputTypeDef,
         "Permissions": List[PermissionType],
     },
-    total=False,
 )
 
 PrincipalPermissionsTypeDef = TypedDict(
     "PrincipalPermissionsTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
         "Permissions": Sequence[PermissionType],
@@ -1219,57 +1123,44 @@
 
 ColumnLFTagTypeDef = TypedDict(
     "ColumnLFTagTypeDef",
     {
         "Name": str,
         "LFTags": List[LFTagPairOutputTypeDef],
     },
-    total=False,
 )
 
 LFTagErrorTypeDef = TypedDict(
     "LFTagErrorTypeDef",
     {
         "LFTag": LFTagPairOutputTypeDef,
         "Error": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 ListLFTagsResponseTypeDef = TypedDict(
     "ListLFTagsResponseTypeDef",
     {
         "LFTags": List[LFTagPairOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredTableWithColumnsResourceOutputTypeDef = TypedDict(
-    "_RequiredTableWithColumnsResourceOutputTypeDef",
+TableWithColumnsResourceOutputTypeDef = TypedDict(
+    "TableWithColumnsResourceOutputTypeDef",
     {
+        "CatalogId": str,
         "DatabaseName": str,
         "Name": str,
-    },
-)
-_OptionalTableWithColumnsResourceOutputTypeDef = TypedDict(
-    "_OptionalTableWithColumnsResourceOutputTypeDef",
-    {
-        "CatalogId": str,
         "ColumnNames": List[str],
         "ColumnWildcard": ColumnWildcardOutputTypeDef,
     },
-    total=False,
 )
 
-class TableWithColumnsResourceOutputTypeDef(
-    _RequiredTableWithColumnsResourceOutputTypeDef, _OptionalTableWithColumnsResourceOutputTypeDef
-):
-    pass
-
 _RequiredTableWithColumnsResourceTypeDef = TypedDict(
     "_RequiredTableWithColumnsResourceTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -1284,39 +1175,28 @@
 )
 
 class TableWithColumnsResourceTypeDef(
     _RequiredTableWithColumnsResourceTypeDef, _OptionalTableWithColumnsResourceTypeDef
 ):
     pass
 
-_RequiredDataCellsFilterOutputTypeDef = TypedDict(
-    "_RequiredDataCellsFilterOutputTypeDef",
+DataCellsFilterOutputTypeDef = TypedDict(
+    "DataCellsFilterOutputTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
-    },
-)
-_OptionalDataCellsFilterOutputTypeDef = TypedDict(
-    "_OptionalDataCellsFilterOutputTypeDef",
-    {
         "RowFilter": RowFilterOutputTypeDef,
         "ColumnNames": List[str],
         "ColumnWildcard": ColumnWildcardOutputTypeDef,
         "VersionId": str,
     },
-    total=False,
 )
 
-class DataCellsFilterOutputTypeDef(
-    _RequiredDataCellsFilterOutputTypeDef, _OptionalDataCellsFilterOutputTypeDef
-):
-    pass
-
 _RequiredDataCellsFilterTypeDef = TypedDict(
     "_RequiredDataCellsFilterTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
@@ -1338,15 +1218,14 @@
 
 TaggedDatabaseTypeDef = TypedDict(
     "TaggedDatabaseTypeDef",
     {
         "Database": DatabaseResourceOutputTypeDef,
         "LFTags": List[LFTagPairOutputTypeDef],
     },
-    total=False,
 )
 
 WriteOperationTypeDef = TypedDict(
     "WriteOperationTypeDef",
     {
         "AddObject": AddObjectInputTypeDef,
         "DeleteObject": DeleteObjectInputTypeDef,
@@ -1377,41 +1256,41 @@
 ):
     pass
 
 DescribeResourceResponseTypeDef = TypedDict(
     "DescribeResourceResponseTypeDef",
     {
         "ResourceInfo": ResourceInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesResponseTypeDef = TypedDict(
     "ListResourcesResponseTypeDef",
     {
         "ResourceInfoList": List[ResourceInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTransactionResponseTypeDef = TypedDict(
     "DescribeTransactionResponseTypeDef",
     {
         "TransactionDescription": TransactionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTransactionsResponseTypeDef = TypedDict(
     "ListTransactionsResponseTypeDef",
     {
         "Transactions": List[TransactionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesRequestRequestTypeDef = TypedDict(
     "ListResourcesRequestRequestTypeDef",
     {
         "FilterConditionList": Sequence[FilterConditionTypeDef],
@@ -1423,15 +1302,15 @@
 
 GetQueryStatisticsResponseTypeDef = TypedDict(
     "GetQueryStatisticsResponseTypeDef",
     {
         "ExecutionStatistics": ExecutionStatisticsTypeDef,
         "PlanningStatistics": PlanningStatisticsTypeDef,
         "QuerySubmissionTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     {
         "TableArn": str,
@@ -1451,43 +1330,62 @@
 
 class GetTemporaryGluePartitionCredentialsRequestRequestTypeDef(
     _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
     _OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
+    "_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    {
+        "QueryId": str,
+    },
+)
+_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
+    "_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef(
+    _RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    _OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+):
+    pass
+
+ListLFTagsRequestListLFTagsPaginateTypeDef = TypedDict(
+    "ListLFTagsRequestListLFTagsPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "ResourceShareType": ResourceShareTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 GetWorkUnitsResponseTypeDef = TypedDict(
     "GetWorkUnitsResponseTypeDef",
     {
         "NextToken": str,
         "QueryId": str,
         "WorkUnitRanges": List[WorkUnitRangeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredLFTagPolicyResourceOutputTypeDef = TypedDict(
-    "_RequiredLFTagPolicyResourceOutputTypeDef",
+LFTagPolicyResourceOutputTypeDef = TypedDict(
+    "LFTagPolicyResourceOutputTypeDef",
     {
+        "CatalogId": str,
         "ResourceType": ResourceTypeType,
         "Expression": List[LFTagOutputTypeDef],
     },
 )
-_OptionalLFTagPolicyResourceOutputTypeDef = TypedDict(
-    "_OptionalLFTagPolicyResourceOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class LFTagPolicyResourceOutputTypeDef(
-    _RequiredLFTagPolicyResourceOutputTypeDef, _OptionalLFTagPolicyResourceOutputTypeDef
-):
-    pass
 
 _RequiredLFTagPolicyResourceTypeDef = TypedDict(
     "_RequiredLFTagPolicyResourceTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "Expression": Sequence[LFTagTypeDef],
     },
@@ -1533,15 +1431,15 @@
         "Expression": Sequence[LFTagTypeDef],
     },
 )
 _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
     "_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
     {
         "CatalogId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef(
     _RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
     _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
@@ -1576,30 +1474,30 @@
         "Expression": Sequence[LFTagTypeDef],
     },
 )
 _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
     "_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     {
         "CatalogId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef(
     _RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
     _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
 ):
     pass
 
 ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef = TypedDict(
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     {
         "Table": TableResourceTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListDataCellsFilterRequestRequestTypeDef = TypedDict(
     "ListDataCellsFilterRequestRequestTypeDef",
     {
@@ -1611,25 +1509,24 @@
 )
 
 ListTableStorageOptimizersResponseTypeDef = TypedDict(
     "ListTableStorageOptimizersResponseTypeDef",
     {
         "StorageOptimizerList": List[StorageOptimizerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PartitionObjectsTypeDef = TypedDict(
     "PartitionObjectsTypeDef",
     {
         "PartitionValues": List[str],
         "Objects": List[TableObjectTypeDef],
     },
-    total=False,
 )
 
 StartQueryPlanningRequestRequestTypeDef = TypedDict(
     "StartQueryPlanningRequestRequestTypeDef",
     {
         "QueryPlanningContext": QueryPlanningContextTypeDef,
         "QueryString": str,
@@ -1646,15 +1543,14 @@
         "Parameters": Dict[str, str],
         "TrustedResourceOwners": List[str],
         "AllowExternalDataFiltering": bool,
         "AllowFullTableExternalDataAccess": bool,
         "ExternalDataFilteringAllowList": List[DataLakePrincipalOutputTypeDef],
         "AuthorizedSessionTagValueList": List[str],
     },
-    total=False,
 )
 
 DataLakeSettingsTypeDef = TypedDict(
     "DataLakeSettingsTypeDef",
     {
         "DataLakeAdmins": Sequence[DataLakePrincipalTypeDef],
         "ReadOnlyAdmins": Sequence[DataLakePrincipalTypeDef],
@@ -1672,59 +1568,58 @@
 
 GetResourceLFTagsResponseTypeDef = TypedDict(
     "GetResourceLFTagsResponseTypeDef",
     {
         "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
         "LFTagsOnTable": List[LFTagPairOutputTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TaggedTableTypeDef = TypedDict(
     "TaggedTableTypeDef",
     {
         "Table": TableResourceOutputTypeDef,
         "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
         "LFTagsOnTable": List[LFTagPairOutputTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
     },
-    total=False,
 )
 
 AddLFTagsToResourceResponseTypeDef = TypedDict(
     "AddLFTagsToResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveLFTagsFromResourceResponseTypeDef = TypedDict(
     "RemoveLFTagsFromResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataCellsFilterResponseTypeDef = TypedDict(
     "GetDataCellsFilterResponseTypeDef",
     {
         "DataCellsFilter": DataCellsFilterOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataCellsFilterResponseTypeDef = TypedDict(
     "ListDataCellsFilterResponseTypeDef",
     {
         "DataCellsFilters": List[DataCellsFilterOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDataCellsFilterRequestRequestTypeDef = TypedDict(
     "CreateDataCellsFilterRequestRequestTypeDef",
     {
         "TableData": DataCellsFilterTypeDef,
@@ -1739,15 +1634,15 @@
 )
 
 SearchDatabasesByLFTagsResponseTypeDef = TypedDict(
     "SearchDatabasesByLFTagsResponseTypeDef",
     {
         "NextToken": str,
         "DatabaseList": List[TaggedDatabaseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateTableObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableObjectsRequestRequestTypeDef",
     {
         "DatabaseName": str,
@@ -1778,15 +1673,14 @@
         "Table": TableResourceOutputTypeDef,
         "TableWithColumns": TableWithColumnsResourceOutputTypeDef,
         "DataLocation": DataLocationResourceOutputTypeDef,
         "DataCellsFilter": DataCellsFilterResourceOutputTypeDef,
         "LFTag": LFTagKeyResourceOutputTypeDef,
         "LFTagPolicy": LFTagPolicyResourceOutputTypeDef,
     },
-    total=False,
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Catalog": Mapping[str, Any],
         "Database": DatabaseResourceTypeDef,
@@ -1801,23 +1695,23 @@
 )
 
 GetTableObjectsResponseTypeDef = TypedDict(
     "GetTableObjectsResponseTypeDef",
     {
         "Objects": List[PartitionObjectsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataLakeSettingsResponseTypeDef = TypedDict(
     "GetDataLakeSettingsResponseTypeDef",
     {
         "DataLakeSettings": DataLakeSettingsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutDataLakeSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredPutDataLakeSettingsRequestRequestTypeDef",
     {
         "DataLakeSettings": DataLakeSettingsTypeDef,
@@ -1838,51 +1732,38 @@
     pass
 
 SearchTablesByLFTagsResponseTypeDef = TypedDict(
     "SearchTablesByLFTagsResponseTypeDef",
     {
         "NextToken": str,
         "TableList": List[TaggedTableTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
-    "_RequiredBatchPermissionsRequestEntryOutputTypeDef",
+BatchPermissionsRequestEntryOutputTypeDef = TypedDict(
+    "BatchPermissionsRequestEntryOutputTypeDef",
     {
         "Id": str,
-    },
-)
-_OptionalBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
-    "_OptionalBatchPermissionsRequestEntryOutputTypeDef",
-    {
         "Principal": DataLakePrincipalOutputTypeDef,
         "Resource": ResourceOutputTypeDef,
         "Permissions": List[PermissionType],
         "PermissionsWithGrantOption": List[PermissionType],
     },
-    total=False,
 )
 
-class BatchPermissionsRequestEntryOutputTypeDef(
-    _RequiredBatchPermissionsRequestEntryOutputTypeDef,
-    _OptionalBatchPermissionsRequestEntryOutputTypeDef,
-):
-    pass
-
 PrincipalResourcePermissionsTypeDef = TypedDict(
     "PrincipalResourcePermissionsTypeDef",
     {
         "Principal": DataLakePrincipalOutputTypeDef,
         "Resource": ResourceOutputTypeDef,
         "Permissions": List[PermissionType],
         "PermissionsWithGrantOption": List[PermissionType],
         "AdditionalDetails": DetailsMapTypeDef,
     },
-    total=False,
 )
 
 _RequiredAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_RequiredAddLFTagsToResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
         "LFTags": Sequence[LFTagPairTypeDef],
@@ -2025,32 +1906,31 @@
 
 BatchPermissionsFailureEntryTypeDef = TypedDict(
     "BatchPermissionsFailureEntryTypeDef",
     {
         "RequestEntry": BatchPermissionsRequestEntryOutputTypeDef,
         "Error": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 GetEffectivePermissionsForPathResponseTypeDef = TypedDict(
     "GetEffectivePermissionsForPathResponseTypeDef",
     {
         "Permissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPermissionsResponseTypeDef = TypedDict(
     "ListPermissionsResponseTypeDef",
     {
         "PrincipalResourcePermissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGrantPermissionsRequestRequestTypeDef",
     {
         "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
@@ -2090,18 +1970,18 @@
 ):
     pass
 
 BatchGrantPermissionsResponseTypeDef = TypedDict(
     "BatchGrantPermissionsResponseTypeDef",
     {
         "Failures": List[BatchPermissionsFailureEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchRevokePermissionsResponseTypeDef = TypedDict(
     "BatchRevokePermissionsResponseTypeDef",
     {
         "Failures": List[BatchPermissionsFailureEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation.egg-info/PKG-INFO` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lakeformation
-Version: 1.28.12
-Summary: Type annotations for boto3.LakeFormation 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.4
+Summary: Type annotations for boto3.LakeFormation 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lakeformation"></a>
 
 # mypy-boto3-lakeformation
 
 [![PyPI - mypy-boto3-lakeformation](https://img.shields.io/pypi/v/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lakeformation)](https://pepy.tech/project/mypy-boto3-lakeformation)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lakeformation?color=blue)](https://pypistats.org/packages/mypy-boto3-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LakeFormation 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[boto3.LakeFormation 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lakeformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -352,27 +352,26 @@
 
 `mypy_boto3_lakeformation.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lakeformation.type_defs import (
     LFTagPairTypeDef,
+    ResponseMetadataTypeDef,
     AddObjectInputTypeDef,
     AssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
-    AssumeDecoratedRoleWithSAMLResponseTypeDef,
     AuditContextTypeDef,
     ErrorDetailTypeDef,
     DataLakePrincipalOutputTypeDef,
     DataLakePrincipalTypeDef,
     CancelTransactionRequestRequestTypeDef,
     LFTagPairOutputTypeDef,
     ColumnWildcardOutputTypeDef,
     ColumnWildcardTypeDef,
     CommitTransactionRequestRequestTypeDef,
-    CommitTransactionResponseTypeDef,
     CreateLFTagRequestRequestTypeDef,
     RowFilterOutputTypeDef,
     DataCellsFilterResourceOutputTypeDef,
     DataCellsFilterResourceTypeDef,
     RowFilterTypeDef,
     DataLocationResourceOutputTypeDef,
     DataLocationResourceTypeDef,
@@ -391,50 +390,49 @@
     ExecutionStatisticsTypeDef,
     ExtendTransactionRequestRequestTypeDef,
     FilterConditionTypeDef,
     GetDataCellsFilterRequestRequestTypeDef,
     GetDataLakeSettingsRequestRequestTypeDef,
     GetEffectivePermissionsForPathRequestRequestTypeDef,
     GetLFTagRequestRequestTypeDef,
-    GetLFTagResponseTypeDef,
     GetQueryStateRequestRequestTypeDef,
-    GetQueryStateResponseTypeDef,
     GetQueryStatisticsRequestRequestTypeDef,
     PlanningStatisticsTypeDef,
     GetTableObjectsRequestRequestTypeDef,
     PartitionValueListTypeDef,
-    GetTemporaryGluePartitionCredentialsResponseTypeDef,
-    GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsRequestRequestTypeDef,
-    GetWorkUnitResultsResponseTypeDef,
-    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetWorkUnitsRequestRequestTypeDef,
     WorkUnitRangeTypeDef,
     LFTagKeyResourceOutputTypeDef,
     LFTagKeyResourceTypeDef,
     LFTagOutputTypeDef,
     LFTagTypeDef,
     TableResourceTypeDef,
-    ListLFTagsRequestListLFTagsPaginateTypeDef,
     ListLFTagsRequestRequestTypeDef,
     ListTableStorageOptimizersRequestRequestTypeDef,
     StorageOptimizerTypeDef,
     ListTransactionsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     TableObjectTypeDef,
     QueryPlanningContextTypeDef,
     RegisterResourceRequestRequestTypeDef,
     TableResourceOutputTypeDef,
-    ResponseMetadataTypeDef,
-    StartQueryPlanningResponseTypeDef,
     StartTransactionRequestRequestTypeDef,
-    StartTransactionResponseTypeDef,
     UpdateLFTagRequestRequestTypeDef,
     UpdateResourceRequestRequestTypeDef,
     UpdateTableStorageOptimizerRequestRequestTypeDef,
+    AssumeDecoratedRoleWithSAMLResponseTypeDef,
+    CommitTransactionResponseTypeDef,
+    GetLFTagResponseTypeDef,
+    GetQueryStateResponseTypeDef,
+    GetTemporaryGluePartitionCredentialsResponseTypeDef,
+    GetTemporaryGlueTableCredentialsResponseTypeDef,
+    GetWorkUnitResultsResponseTypeDef,
+    StartQueryPlanningResponseTypeDef,
+    StartTransactionResponseTypeDef,
     UpdateTableStorageOptimizerResponseTypeDef,
     GetTemporaryGlueTableCredentialsRequestRequestTypeDef,
     PrincipalPermissionsOutputTypeDef,
     PrincipalPermissionsTypeDef,
     ColumnLFTagTypeDef,
     LFTagErrorTypeDef,
     ListLFTagsResponseTypeDef,
@@ -448,14 +446,16 @@
     DescribeResourceResponseTypeDef,
     ListResourcesResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     ListTransactionsResponseTypeDef,
     ListResourcesRequestRequestTypeDef,
     GetQueryStatisticsResponseTypeDef,
     GetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
+    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    ListLFTagsRequestListLFTagsPaginateTypeDef,
     GetWorkUnitsResponseTypeDef,
     LFTagPolicyResourceOutputTypeDef,
     LFTagPolicyResourceTypeDef,
     SearchDatabasesByLFTagsRequestRequestTypeDef,
     SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
     SearchTablesByLFTagsRequestRequestTypeDef,
     SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
```

### Comparing `mypy-boto3-lakeformation-1.28.12/mypy_boto3_lakeformation.egg-info/SOURCES.txt` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.12/setup.py` & `mypy-boto3-lakeformation-1.28.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lakeformation",
-    version="1.28.12",
+    version="1.28.4",
     packages=["mypy_boto3_lakeformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LakeFormation 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.LakeFormation 1.28.4 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

