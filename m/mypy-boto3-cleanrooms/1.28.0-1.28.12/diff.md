# Comparing `tmp/mypy-boto3-cleanrooms-1.28.0.tar.gz` & `tmp/mypy-boto3-cleanrooms-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cleanrooms-1.28.0.tar", last modified: Thu Jul  6 20:59:08 2023, max compression
+gzip compressed data, was "mypy-boto3-cleanrooms-1.28.12.tar", last modified: Thu Jul 27 05:34:24 2023, max compression
```

## Comparing `mypy-boto3-cleanrooms-1.28.0.tar` & `mypy-boto3-cleanrooms-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:08.862242 mypy-boto3-cleanrooms-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:34:53.000000 mypy-boto3-cleanrooms-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18937 2023-07-06 20:59:08.858242 mypy-boto3-cleanrooms-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17433 2023-07-06 20:34:53.000000 mypy-boto3-cleanrooms-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:08.858242 mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-06 20:34:53.000000 mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-06 20:34:53.000000 mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-06 20:34:53.000000 mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29888 2023-07-06 20:34:54.000000 mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29837 2023-07-06 20:34:53.000000 mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-07-06 20:34:54.000000 mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-07-06 20:34:54.000000 mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-07-06 20:34:54.000000 mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-07-06 20:34:54.000000 mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:53.000000 mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-07-06 20:34:55.000000 mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41640 2023-07-06 20:34:55.000000 mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:34:53.000000 mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:08.858242 mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18937 2023-07-06 20:59:08.000000 mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-06 20:59:08.000000 mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:08.000000 mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:08.000000 mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:08.000000 mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 20:59:08.000000 mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:08.862242 mypy-boto3-cleanrooms-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-06 20:34:53.000000 mypy-boto3-cleanrooms-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.864563 mypy-boto3-cleanrooms-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19502 2023-07-27 05:34:24.864563 mypy-boto3-cleanrooms-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17996 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.864563 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29888 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29837 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46253 2023-07-27 05:18:25.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46192 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.864563 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19502 2023-07-27 05:34:24.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:24.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:24.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:24.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:24.864563 mypy-boto3-cleanrooms-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/setup.py
```

### Comparing `mypy-boto3-cleanrooms-1.28.0/LICENSE` & `mypy-boto3-cleanrooms-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.0/PKG-INFO` & `mypy-boto3-cleanrooms-1.28.12/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cleanrooms
-Version: 1.28.0
-Summary: Type annotations for boto3.CleanRoomsService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CleanRoomsService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cleanrooms"></a>
 
 # mypy-boto3-cleanrooms
 
 [![PyPI - mypy-boto3-cleanrooms](https://img.shields.io/pypi/v/mypy-boto3-cleanrooms.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanrooms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cleanrooms.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanrooms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cleanrooms?color=blue)](https://pypistats.org/packages/mypy-boto3-cleanrooms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cleanrooms)](https://pepy.tech/project/mypy-boto3-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CleanRoomsService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
+[boto3.CleanRoomsService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
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
 [mypy-boto3-cleanrooms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -366,25 +366,29 @@
 ### Typed dictionaries
 
 `mypy_boto3_cleanrooms.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cleanrooms.type_defs import (
+    AggregateColumnOutputTypeDef,
     AggregateColumnTypeDef,
+    AggregationConstraintOutputTypeDef,
     AggregationConstraintTypeDef,
+    AnalysisRuleListOutputTypeDef,
     AnalysisRuleListTypeDef,
     BatchGetSchemaErrorTypeDef,
     BatchGetSchemaInputRequestTypeDef,
     CollaborationSummaryTypeDef,
-    DataEncryptionMetadataTypeDef,
+    DataEncryptionMetadataOutputTypeDef,
     ColumnTypeDef,
     ConfiguredTableAssociationSummaryTypeDef,
     ConfiguredTableAssociationTypeDef,
     ConfiguredTableSummaryTypeDef,
+    DataEncryptionMetadataTypeDef,
     MemberSpecificationTypeDef,
     CreateConfiguredTableAssociationInputRequestTypeDef,
     CreateMembershipInputRequestTypeDef,
     MembershipTypeDef,
     DeleteCollaborationInputRequestTypeDef,
     DeleteConfiguredTableAnalysisRuleInputRequestTypeDef,
     DeleteConfiguredTableAssociationInputRequestTypeDef,
@@ -395,14 +399,15 @@
     GetConfiguredTableAnalysisRuleInputRequestTypeDef,
     GetConfiguredTableAssociationInputRequestTypeDef,
     GetConfiguredTableInputRequestTypeDef,
     GetMembershipInputRequestTypeDef,
     GetProtectedQueryInputRequestTypeDef,
     GetSchemaAnalysisRuleInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
+    GlueTableReferenceOutputTypeDef,
     GlueTableReferenceTypeDef,
     ListCollaborationsInputListCollaborationsPaginateTypeDef,
     ListCollaborationsInputRequestTypeDef,
     ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
     ListConfiguredTableAssociationsInputRequestTypeDef,
     ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef,
     ListConfiguredTablesInputRequestTypeDef,
@@ -418,58 +423,66 @@
     ListSchemasInputListSchemasPaginateTypeDef,
     ListSchemasInputRequestTypeDef,
     SchemaSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     PaginatorConfigTypeDef,
     ProtectedQueryErrorTypeDef,
+    ProtectedQueryS3OutputConfigurationOutputTypeDef,
     ProtectedQueryS3OutputConfigurationTypeDef,
     ProtectedQueryS3OutputTypeDef,
+    ProtectedQuerySQLParametersOutputTypeDef,
     ProtectedQuerySQLParametersTypeDef,
     ProtectedQueryStatisticsTypeDef,
     ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateCollaborationInputRequestTypeDef,
     UpdateConfiguredTableAssociationInputRequestTypeDef,
     UpdateConfiguredTableInputRequestTypeDef,
     UpdateMembershipInputRequestTypeDef,
     UpdateProtectedQueryInputRequestTypeDef,
+    AnalysisRuleAggregationOutputTypeDef,
     AnalysisRuleAggregationTypeDef,
     ListCollaborationsOutputTypeDef,
     CollaborationTypeDef,
     SchemaTypeDef,
     ListConfiguredTableAssociationsOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     GetConfiguredTableAssociationOutputTypeDef,
     UpdateConfiguredTableAssociationOutputTypeDef,
     ListConfiguredTablesOutputTypeDef,
     CreateCollaborationInputRequestTypeDef,
     CreateMembershipOutputTypeDef,
     GetMembershipOutputTypeDef,
     UpdateMembershipOutputTypeDef,
+    TableReferenceOutputTypeDef,
     TableReferenceTypeDef,
     ListMembersOutputTypeDef,
     ListMembershipsOutputTypeDef,
     ListProtectedQueriesOutputTypeDef,
     ListSchemasOutputTypeDef,
+    ProtectedQueryOutputConfigurationOutputTypeDef,
     ProtectedQueryOutputConfigurationTypeDef,
     ProtectedQueryOutputTypeDef,
     AnalysisRulePolicyV1TypeDef,
+    ConfiguredTableAnalysisRulePolicyV1OutputTypeDef,
     ConfiguredTableAnalysisRulePolicyV1TypeDef,
     CreateCollaborationOutputTypeDef,
     GetCollaborationOutputTypeDef,
     UpdateCollaborationOutputTypeDef,
     BatchGetSchemaOutputTypeDef,
     GetSchemaOutputTypeDef,
     ConfiguredTableTypeDef,
     CreateConfiguredTableInputRequestTypeDef,
+    ProtectedQueryResultConfigurationOutputTypeDef,
     ProtectedQueryResultConfigurationTypeDef,
     ProtectedQueryResultTypeDef,
     AnalysisRulePolicyTypeDef,
+    ConfiguredTableAnalysisRulePolicyOutputTypeDef,
     ConfiguredTableAnalysisRulePolicyTypeDef,
     CreateConfiguredTableOutputTypeDef,
     GetConfiguredTableOutputTypeDef,
     UpdateConfiguredTableOutputTypeDef,
     StartProtectedQueryInputRequestTypeDef,
     ProtectedQueryTypeDef,
     AnalysisRuleTypeDef,
@@ -482,15 +495,15 @@
     GetSchemaAnalysisRuleOutputTypeDef,
     CreateConfiguredTableAnalysisRuleOutputTypeDef,
     GetConfiguredTableAnalysisRuleOutputTypeDef,
     UpdateConfiguredTableAnalysisRuleOutputTypeDef,
 )
 
 
-def get_structure() -> AggregateColumnTypeDef:
+def get_structure() -> AggregateColumnOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cleanrooms-1.28.0/README.md` & `mypy-boto3-cleanrooms-1.28.12/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cleanrooms"></a>
 
 # mypy-boto3-cleanrooms
 
 [![PyPI - mypy-boto3-cleanrooms](https://img.shields.io/pypi/v/mypy-boto3-cleanrooms.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanrooms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cleanrooms.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanrooms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cleanrooms?color=blue)](https://pypistats.org/packages/mypy-boto3-cleanrooms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cleanrooms)](https://pepy.tech/project/mypy-boto3-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CleanRoomsService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
+[boto3.CleanRoomsService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
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
 [mypy-boto3-cleanrooms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,25 +334,29 @@
 ### Typed dictionaries
 
 `mypy_boto3_cleanrooms.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cleanrooms.type_defs import (
+    AggregateColumnOutputTypeDef,
     AggregateColumnTypeDef,
+    AggregationConstraintOutputTypeDef,
     AggregationConstraintTypeDef,
+    AnalysisRuleListOutputTypeDef,
     AnalysisRuleListTypeDef,
     BatchGetSchemaErrorTypeDef,
     BatchGetSchemaInputRequestTypeDef,
     CollaborationSummaryTypeDef,
-    DataEncryptionMetadataTypeDef,
+    DataEncryptionMetadataOutputTypeDef,
     ColumnTypeDef,
     ConfiguredTableAssociationSummaryTypeDef,
     ConfiguredTableAssociationTypeDef,
     ConfiguredTableSummaryTypeDef,
+    DataEncryptionMetadataTypeDef,
     MemberSpecificationTypeDef,
     CreateConfiguredTableAssociationInputRequestTypeDef,
     CreateMembershipInputRequestTypeDef,
     MembershipTypeDef,
     DeleteCollaborationInputRequestTypeDef,
     DeleteConfiguredTableAnalysisRuleInputRequestTypeDef,
     DeleteConfiguredTableAssociationInputRequestTypeDef,
@@ -363,14 +367,15 @@
     GetConfiguredTableAnalysisRuleInputRequestTypeDef,
     GetConfiguredTableAssociationInputRequestTypeDef,
     GetConfiguredTableInputRequestTypeDef,
     GetMembershipInputRequestTypeDef,
     GetProtectedQueryInputRequestTypeDef,
     GetSchemaAnalysisRuleInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
+    GlueTableReferenceOutputTypeDef,
     GlueTableReferenceTypeDef,
     ListCollaborationsInputListCollaborationsPaginateTypeDef,
     ListCollaborationsInputRequestTypeDef,
     ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
     ListConfiguredTableAssociationsInputRequestTypeDef,
     ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef,
     ListConfiguredTablesInputRequestTypeDef,
@@ -386,58 +391,66 @@
     ListSchemasInputListSchemasPaginateTypeDef,
     ListSchemasInputRequestTypeDef,
     SchemaSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     PaginatorConfigTypeDef,
     ProtectedQueryErrorTypeDef,
+    ProtectedQueryS3OutputConfigurationOutputTypeDef,
     ProtectedQueryS3OutputConfigurationTypeDef,
     ProtectedQueryS3OutputTypeDef,
+    ProtectedQuerySQLParametersOutputTypeDef,
     ProtectedQuerySQLParametersTypeDef,
     ProtectedQueryStatisticsTypeDef,
     ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateCollaborationInputRequestTypeDef,
     UpdateConfiguredTableAssociationInputRequestTypeDef,
     UpdateConfiguredTableInputRequestTypeDef,
     UpdateMembershipInputRequestTypeDef,
     UpdateProtectedQueryInputRequestTypeDef,
+    AnalysisRuleAggregationOutputTypeDef,
     AnalysisRuleAggregationTypeDef,
     ListCollaborationsOutputTypeDef,
     CollaborationTypeDef,
     SchemaTypeDef,
     ListConfiguredTableAssociationsOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     GetConfiguredTableAssociationOutputTypeDef,
     UpdateConfiguredTableAssociationOutputTypeDef,
     ListConfiguredTablesOutputTypeDef,
     CreateCollaborationInputRequestTypeDef,
     CreateMembershipOutputTypeDef,
     GetMembershipOutputTypeDef,
     UpdateMembershipOutputTypeDef,
+    TableReferenceOutputTypeDef,
     TableReferenceTypeDef,
     ListMembersOutputTypeDef,
     ListMembershipsOutputTypeDef,
     ListProtectedQueriesOutputTypeDef,
     ListSchemasOutputTypeDef,
+    ProtectedQueryOutputConfigurationOutputTypeDef,
     ProtectedQueryOutputConfigurationTypeDef,
     ProtectedQueryOutputTypeDef,
     AnalysisRulePolicyV1TypeDef,
+    ConfiguredTableAnalysisRulePolicyV1OutputTypeDef,
     ConfiguredTableAnalysisRulePolicyV1TypeDef,
     CreateCollaborationOutputTypeDef,
     GetCollaborationOutputTypeDef,
     UpdateCollaborationOutputTypeDef,
     BatchGetSchemaOutputTypeDef,
     GetSchemaOutputTypeDef,
     ConfiguredTableTypeDef,
     CreateConfiguredTableInputRequestTypeDef,
+    ProtectedQueryResultConfigurationOutputTypeDef,
     ProtectedQueryResultConfigurationTypeDef,
     ProtectedQueryResultTypeDef,
     AnalysisRulePolicyTypeDef,
+    ConfiguredTableAnalysisRulePolicyOutputTypeDef,
     ConfiguredTableAnalysisRulePolicyTypeDef,
     CreateConfiguredTableOutputTypeDef,
     GetConfiguredTableOutputTypeDef,
     UpdateConfiguredTableOutputTypeDef,
     StartProtectedQueryInputRequestTypeDef,
     ProtectedQueryTypeDef,
     AnalysisRuleTypeDef,
@@ -450,15 +463,15 @@
     GetSchemaAnalysisRuleOutputTypeDef,
     CreateConfiguredTableAnalysisRuleOutputTypeDef,
     GetConfiguredTableAnalysisRuleOutputTypeDef,
     UpdateConfiguredTableAnalysisRuleOutputTypeDef,
 )
 
 
-def get_structure() -> AggregateColumnTypeDef:
+def get_structure() -> AggregateColumnOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/__init__.py` & `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/__init__.pyi` & `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/__main__.py` & `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CleanRoomsService 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.CleanRoomsService 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService\nOther"
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

### Comparing `mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/client.py` & `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/client.pyi` & `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/literals.py` & `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AggregateFunctionNameType",
     "AggregationTypeType",
     "AnalysisMethodType",
     "AnalysisRuleTypeType",
     "CollaborationQueryLogStatusType",
     "ConfiguredTableAnalysisRuleTypeType",
@@ -49,15 +48,14 @@
     "CleanRoomsServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AggregateFunctionNameType = Literal["AVG", "COUNT", "COUNT_DISTINCT", "SUM", "SUM_DISTINCT"]
 AggregationTypeType = Literal["COUNT_DISTINCT"]
 AnalysisMethodType = Literal["DIRECT_QUERY"]
 AnalysisRuleTypeType = Literal["AGGREGATION", "LIST"]
 CollaborationQueryLogStatusType = Literal["DISABLED", "ENABLED"]
 ConfiguredTableAnalysisRuleTypeType = Literal["AGGREGATION", "LIST"]
 FilterableMemberStatusType = Literal["ACTIVE", "INVITED"]
@@ -212,14 +210,15 @@
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
@@ -298,26 +297,28 @@
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

### Comparing `mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/literals.pyi` & `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AggregateFunctionNameType",
     "AggregationTypeType",
     "AnalysisMethodType",
     "AnalysisRuleTypeType",
     "CollaborationQueryLogStatusType",
     "ConfiguredTableAnalysisRuleTypeType",
@@ -48,14 +49,15 @@
     "CleanRoomsServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AggregateFunctionNameType = Literal["AVG", "COUNT", "COUNT_DISTINCT", "SUM", "SUM_DISTINCT"]
 AggregationTypeType = Literal["COUNT_DISTINCT"]
 AnalysisMethodType = Literal["DIRECT_QUERY"]
 AnalysisRuleTypeType = Literal["AGGREGATION", "LIST"]
 CollaborationQueryLogStatusType = Literal["DISABLED", "ENABLED"]
 ConfiguredTableAnalysisRuleTypeType = Literal["AGGREGATION", "LIST"]
 FilterableMemberStatusType = Literal["ACTIVE", "INVITED"]
@@ -210,14 +212,15 @@
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
@@ -296,26 +299,28 @@
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

### Comparing `mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/paginator.py` & `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/paginator.pyi` & `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/type_defs.py` & `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for cleanrooms service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_cleanrooms.type_defs import AggregateColumnTypeDef
+    from mypy_boto3_cleanrooms.type_defs import AggregateColumnOutputTypeDef
 
-    data: AggregateColumnTypeDef = {...}
+    data: AggregateColumnOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -38,25 +38,29 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AggregateColumnOutputTypeDef",
     "AggregateColumnTypeDef",
+    "AggregationConstraintOutputTypeDef",
     "AggregationConstraintTypeDef",
+    "AnalysisRuleListOutputTypeDef",
     "AnalysisRuleListTypeDef",
     "BatchGetSchemaErrorTypeDef",
     "BatchGetSchemaInputRequestTypeDef",
     "CollaborationSummaryTypeDef",
-    "DataEncryptionMetadataTypeDef",
+    "DataEncryptionMetadataOutputTypeDef",
     "ColumnTypeDef",
     "ConfiguredTableAssociationSummaryTypeDef",
     "ConfiguredTableAssociationTypeDef",
     "ConfiguredTableSummaryTypeDef",
+    "DataEncryptionMetadataTypeDef",
     "MemberSpecificationTypeDef",
     "CreateConfiguredTableAssociationInputRequestTypeDef",
     "CreateMembershipInputRequestTypeDef",
     "MembershipTypeDef",
     "DeleteCollaborationInputRequestTypeDef",
     "DeleteConfiguredTableAnalysisRuleInputRequestTypeDef",
     "DeleteConfiguredTableAssociationInputRequestTypeDef",
@@ -67,14 +71,15 @@
     "GetConfiguredTableAnalysisRuleInputRequestTypeDef",
     "GetConfiguredTableAssociationInputRequestTypeDef",
     "GetConfiguredTableInputRequestTypeDef",
     "GetMembershipInputRequestTypeDef",
     "GetProtectedQueryInputRequestTypeDef",
     "GetSchemaAnalysisRuleInputRequestTypeDef",
     "GetSchemaInputRequestTypeDef",
+    "GlueTableReferenceOutputTypeDef",
     "GlueTableReferenceTypeDef",
     "ListCollaborationsInputListCollaborationsPaginateTypeDef",
     "ListCollaborationsInputRequestTypeDef",
     "ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
     "ListConfiguredTableAssociationsInputRequestTypeDef",
     "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
     "ListConfiguredTablesInputRequestTypeDef",
@@ -90,58 +95,66 @@
     "ListSchemasInputListSchemasPaginateTypeDef",
     "ListSchemasInputRequestTypeDef",
     "SchemaSummaryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ProtectedQueryErrorTypeDef",
+    "ProtectedQueryS3OutputConfigurationOutputTypeDef",
     "ProtectedQueryS3OutputConfigurationTypeDef",
     "ProtectedQueryS3OutputTypeDef",
+    "ProtectedQuerySQLParametersOutputTypeDef",
     "ProtectedQuerySQLParametersTypeDef",
     "ProtectedQueryStatisticsTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateCollaborationInputRequestTypeDef",
     "UpdateConfiguredTableAssociationInputRequestTypeDef",
     "UpdateConfiguredTableInputRequestTypeDef",
     "UpdateMembershipInputRequestTypeDef",
     "UpdateProtectedQueryInputRequestTypeDef",
+    "AnalysisRuleAggregationOutputTypeDef",
     "AnalysisRuleAggregationTypeDef",
     "ListCollaborationsOutputTypeDef",
     "CollaborationTypeDef",
     "SchemaTypeDef",
     "ListConfiguredTableAssociationsOutputTypeDef",
     "CreateConfiguredTableAssociationOutputTypeDef",
     "GetConfiguredTableAssociationOutputTypeDef",
     "UpdateConfiguredTableAssociationOutputTypeDef",
     "ListConfiguredTablesOutputTypeDef",
     "CreateCollaborationInputRequestTypeDef",
     "CreateMembershipOutputTypeDef",
     "GetMembershipOutputTypeDef",
     "UpdateMembershipOutputTypeDef",
+    "TableReferenceOutputTypeDef",
     "TableReferenceTypeDef",
     "ListMembersOutputTypeDef",
     "ListMembershipsOutputTypeDef",
     "ListProtectedQueriesOutputTypeDef",
     "ListSchemasOutputTypeDef",
+    "ProtectedQueryOutputConfigurationOutputTypeDef",
     "ProtectedQueryOutputConfigurationTypeDef",
     "ProtectedQueryOutputTypeDef",
     "AnalysisRulePolicyV1TypeDef",
+    "ConfiguredTableAnalysisRulePolicyV1OutputTypeDef",
     "ConfiguredTableAnalysisRulePolicyV1TypeDef",
     "CreateCollaborationOutputTypeDef",
     "GetCollaborationOutputTypeDef",
     "UpdateCollaborationOutputTypeDef",
     "BatchGetSchemaOutputTypeDef",
     "GetSchemaOutputTypeDef",
     "ConfiguredTableTypeDef",
     "CreateConfiguredTableInputRequestTypeDef",
+    "ProtectedQueryResultConfigurationOutputTypeDef",
     "ProtectedQueryResultConfigurationTypeDef",
     "ProtectedQueryResultTypeDef",
     "AnalysisRulePolicyTypeDef",
+    "ConfiguredTableAnalysisRulePolicyOutputTypeDef",
     "ConfiguredTableAnalysisRulePolicyTypeDef",
     "CreateConfiguredTableOutputTypeDef",
     "GetConfiguredTableOutputTypeDef",
     "UpdateConfiguredTableOutputTypeDef",
     "StartProtectedQueryInputRequestTypeDef",
     "ProtectedQueryTypeDef",
     "AnalysisRuleTypeDef",
@@ -153,31 +166,70 @@
     "UpdateProtectedQueryOutputTypeDef",
     "GetSchemaAnalysisRuleOutputTypeDef",
     "CreateConfiguredTableAnalysisRuleOutputTypeDef",
     "GetConfiguredTableAnalysisRuleOutputTypeDef",
     "UpdateConfiguredTableAnalysisRuleOutputTypeDef",
 )
 
+AggregateColumnOutputTypeDef = TypedDict(
+    "AggregateColumnOutputTypeDef",
+    {
+        "columnNames": List[str],
+        "function": AggregateFunctionNameType,
+    },
+)
+
 AggregateColumnTypeDef = TypedDict(
     "AggregateColumnTypeDef",
     {
         "columnNames": Sequence[str],
         "function": AggregateFunctionNameType,
     },
 )
 
+AggregationConstraintOutputTypeDef = TypedDict(
+    "AggregationConstraintOutputTypeDef",
+    {
+        "columnName": str,
+        "minimum": int,
+        "type": Literal["COUNT_DISTINCT"],
+    },
+)
+
 AggregationConstraintTypeDef = TypedDict(
     "AggregationConstraintTypeDef",
     {
         "columnName": str,
         "minimum": int,
         "type": Literal["COUNT_DISTINCT"],
     },
 )
 
+_RequiredAnalysisRuleListOutputTypeDef = TypedDict(
+    "_RequiredAnalysisRuleListOutputTypeDef",
+    {
+        "joinColumns": List[str],
+        "listColumns": List[str],
+    },
+)
+_OptionalAnalysisRuleListOutputTypeDef = TypedDict(
+    "_OptionalAnalysisRuleListOutputTypeDef",
+    {
+        "allowedJoinOperators": List[JoinOperatorType],
+    },
+    total=False,
+)
+
+
+class AnalysisRuleListOutputTypeDef(
+    _RequiredAnalysisRuleListOutputTypeDef, _OptionalAnalysisRuleListOutputTypeDef
+):
+    pass
+
+
 _RequiredAnalysisRuleListTypeDef = TypedDict(
     "_RequiredAnalysisRuleListTypeDef",
     {
         "joinColumns": Sequence[str],
         "listColumns": Sequence[str],
     },
 )
@@ -236,16 +288,16 @@
 
 class CollaborationSummaryTypeDef(
     _RequiredCollaborationSummaryTypeDef, _OptionalCollaborationSummaryTypeDef
 ):
     pass
 
 
-DataEncryptionMetadataTypeDef = TypedDict(
-    "DataEncryptionMetadataTypeDef",
+DataEncryptionMetadataOutputTypeDef = TypedDict(
+    "DataEncryptionMetadataOutputTypeDef",
     {
         "allowCleartext": bool,
         "allowDuplicates": bool,
         "allowJoinsOnColumnsWithDifferentNames": bool,
         "preserveNulls": bool,
     },
 )
@@ -311,14 +363,24 @@
         "createTime": datetime,
         "updateTime": datetime,
         "analysisRuleTypes": List[ConfiguredTableAnalysisRuleTypeType],
         "analysisMethod": Literal["DIRECT_QUERY"],
     },
 )
 
+DataEncryptionMetadataTypeDef = TypedDict(
+    "DataEncryptionMetadataTypeDef",
+    {
+        "allowCleartext": bool,
+        "allowDuplicates": bool,
+        "allowJoinsOnColumnsWithDifferentNames": bool,
+        "preserveNulls": bool,
+    },
+)
+
 MemberSpecificationTypeDef = TypedDict(
     "MemberSpecificationTypeDef",
     {
         "accountId": str,
         "memberAbilities": Sequence[MemberAbilityType],
         "displayName": str,
     },
@@ -493,14 +555,22 @@
     "GetSchemaInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
         "name": str,
     },
 )
 
+GlueTableReferenceOutputTypeDef = TypedDict(
+    "GlueTableReferenceOutputTypeDef",
+    {
+        "tableName": str,
+        "databaseName": str,
+    },
+)
+
 GlueTableReferenceTypeDef = TypedDict(
     "GlueTableReferenceTypeDef",
     {
         "tableName": str,
         "databaseName": str,
     },
 )
@@ -850,14 +920,37 @@
     "ProtectedQueryErrorTypeDef",
     {
         "message": str,
         "code": str,
     },
 )
 
+_RequiredProtectedQueryS3OutputConfigurationOutputTypeDef = TypedDict(
+    "_RequiredProtectedQueryS3OutputConfigurationOutputTypeDef",
+    {
+        "resultFormat": ResultFormatType,
+        "bucket": str,
+    },
+)
+_OptionalProtectedQueryS3OutputConfigurationOutputTypeDef = TypedDict(
+    "_OptionalProtectedQueryS3OutputConfigurationOutputTypeDef",
+    {
+        "keyPrefix": str,
+    },
+    total=False,
+)
+
+
+class ProtectedQueryS3OutputConfigurationOutputTypeDef(
+    _RequiredProtectedQueryS3OutputConfigurationOutputTypeDef,
+    _OptionalProtectedQueryS3OutputConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredProtectedQueryS3OutputConfigurationTypeDef = TypedDict(
     "_RequiredProtectedQueryS3OutputConfigurationTypeDef",
     {
         "resultFormat": ResultFormatType,
         "bucket": str,
     },
 )
@@ -880,14 +973,22 @@
 ProtectedQueryS3OutputTypeDef = TypedDict(
     "ProtectedQueryS3OutputTypeDef",
     {
         "location": str,
     },
 )
 
+ProtectedQuerySQLParametersOutputTypeDef = TypedDict(
+    "ProtectedQuerySQLParametersOutputTypeDef",
+    {
+        "queryString": str,
+    },
+    total=False,
+)
+
 ProtectedQuerySQLParametersTypeDef = TypedDict(
     "ProtectedQuerySQLParametersTypeDef",
     {
         "queryString": str,
     },
     total=False,
 )
@@ -1022,14 +1123,40 @@
     {
         "membershipIdentifier": str,
         "protectedQueryIdentifier": str,
         "targetStatus": Literal["CANCELLED"],
     },
 )
 
+_RequiredAnalysisRuleAggregationOutputTypeDef = TypedDict(
+    "_RequiredAnalysisRuleAggregationOutputTypeDef",
+    {
+        "aggregateColumns": List[AggregateColumnOutputTypeDef],
+        "joinColumns": List[str],
+        "dimensionColumns": List[str],
+        "scalarFunctions": List[ScalarFunctionsType],
+        "outputConstraints": List[AggregationConstraintOutputTypeDef],
+    },
+)
+_OptionalAnalysisRuleAggregationOutputTypeDef = TypedDict(
+    "_OptionalAnalysisRuleAggregationOutputTypeDef",
+    {
+        "joinRequired": Literal["QUERY_RUNNER"],
+        "allowedJoinOperators": List[JoinOperatorType],
+    },
+    total=False,
+)
+
+
+class AnalysisRuleAggregationOutputTypeDef(
+    _RequiredAnalysisRuleAggregationOutputTypeDef, _OptionalAnalysisRuleAggregationOutputTypeDef
+):
+    pass
+
+
 _RequiredAnalysisRuleAggregationTypeDef = TypedDict(
     "_RequiredAnalysisRuleAggregationTypeDef",
     {
         "aggregateColumns": Sequence[AggregateColumnTypeDef],
         "joinColumns": Sequence[str],
         "dimensionColumns": Sequence[str],
         "scalarFunctions": Sequence[ScalarFunctionsType],
@@ -1077,15 +1204,15 @@
 )
 _OptionalCollaborationTypeDef = TypedDict(
     "_OptionalCollaborationTypeDef",
     {
         "description": str,
         "membershipId": str,
         "membershipArn": str,
-        "dataEncryptionMetadata": DataEncryptionMetadataTypeDef,
+        "dataEncryptionMetadata": DataEncryptionMetadataOutputTypeDef,
     },
     total=False,
 )
 
 
 class CollaborationTypeDef(_RequiredCollaborationTypeDef, _OptionalCollaborationTypeDef):
     pass
@@ -1209,14 +1336,22 @@
     "UpdateMembershipOutputTypeDef",
     {
         "membership": MembershipTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TableReferenceOutputTypeDef = TypedDict(
+    "TableReferenceOutputTypeDef",
+    {
+        "glue": GlueTableReferenceOutputTypeDef,
+    },
+    total=False,
+)
+
 TableReferenceTypeDef = TypedDict(
     "TableReferenceTypeDef",
     {
         "glue": GlueTableReferenceTypeDef,
     },
     total=False,
 )
@@ -1253,14 +1388,22 @@
     {
         "schemaSummaries": List[SchemaSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ProtectedQueryOutputConfigurationOutputTypeDef = TypedDict(
+    "ProtectedQueryOutputConfigurationOutputTypeDef",
+    {
+        "s3": ProtectedQueryS3OutputConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ProtectedQueryOutputConfigurationTypeDef = TypedDict(
     "ProtectedQueryOutputConfigurationTypeDef",
     {
         "s3": ProtectedQueryS3OutputConfigurationTypeDef,
     },
     total=False,
 )
@@ -1272,16 +1415,25 @@
     },
     total=False,
 )
 
 AnalysisRulePolicyV1TypeDef = TypedDict(
     "AnalysisRulePolicyV1TypeDef",
     {
-        "list": AnalysisRuleListTypeDef,
-        "aggregation": AnalysisRuleAggregationTypeDef,
+        "list": AnalysisRuleListOutputTypeDef,
+        "aggregation": AnalysisRuleAggregationOutputTypeDef,
+    },
+    total=False,
+)
+
+ConfiguredTableAnalysisRulePolicyV1OutputTypeDef = TypedDict(
+    "ConfiguredTableAnalysisRulePolicyV1OutputTypeDef",
+    {
+        "list": AnalysisRuleListOutputTypeDef,
+        "aggregation": AnalysisRuleAggregationOutputTypeDef,
     },
     total=False,
 )
 
 ConfiguredTableAnalysisRulePolicyV1TypeDef = TypedDict(
     "ConfiguredTableAnalysisRulePolicyV1TypeDef",
     {
@@ -1334,15 +1486,15 @@
 
 _RequiredConfiguredTableTypeDef = TypedDict(
     "_RequiredConfiguredTableTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
-        "tableReference": TableReferenceTypeDef,
+        "tableReference": TableReferenceOutputTypeDef,
         "createTime": datetime,
         "updateTime": datetime,
         "analysisRuleTypes": List[ConfiguredTableAnalysisRuleTypeType],
         "analysisMethod": Literal["DIRECT_QUERY"],
         "allowedColumns": List[str],
     },
 )
@@ -1381,14 +1533,21 @@
 class CreateConfiguredTableInputRequestTypeDef(
     _RequiredCreateConfiguredTableInputRequestTypeDef,
     _OptionalCreateConfiguredTableInputRequestTypeDef,
 ):
     pass
 
 
+ProtectedQueryResultConfigurationOutputTypeDef = TypedDict(
+    "ProtectedQueryResultConfigurationOutputTypeDef",
+    {
+        "outputConfiguration": ProtectedQueryOutputConfigurationOutputTypeDef,
+    },
+)
+
 ProtectedQueryResultConfigurationTypeDef = TypedDict(
     "ProtectedQueryResultConfigurationTypeDef",
     {
         "outputConfiguration": ProtectedQueryOutputConfigurationTypeDef,
     },
 )
 
@@ -1403,14 +1562,22 @@
     "AnalysisRulePolicyTypeDef",
     {
         "v1": AnalysisRulePolicyV1TypeDef,
     },
     total=False,
 )
 
+ConfiguredTableAnalysisRulePolicyOutputTypeDef = TypedDict(
+    "ConfiguredTableAnalysisRulePolicyOutputTypeDef",
+    {
+        "v1": ConfiguredTableAnalysisRulePolicyV1OutputTypeDef,
+    },
+    total=False,
+)
+
 ConfiguredTableAnalysisRulePolicyTypeDef = TypedDict(
     "ConfiguredTableAnalysisRulePolicyTypeDef",
     {
         "v1": ConfiguredTableAnalysisRulePolicyV1TypeDef,
     },
     total=False,
 )
@@ -1452,17 +1619,17 @@
 _RequiredProtectedQueryTypeDef = TypedDict(
     "_RequiredProtectedQueryTypeDef",
     {
         "id": str,
         "membershipId": str,
         "membershipArn": str,
         "createTime": datetime,
-        "sqlParameters": ProtectedQuerySQLParametersTypeDef,
+        "sqlParameters": ProtectedQuerySQLParametersOutputTypeDef,
         "status": ProtectedQueryStatusType,
-        "resultConfiguration": ProtectedQueryResultConfigurationTypeDef,
+        "resultConfiguration": ProtectedQueryResultConfigurationOutputTypeDef,
     },
 )
 _OptionalProtectedQueryTypeDef = TypedDict(
     "_OptionalProtectedQueryTypeDef",
     {
         "statistics": ProtectedQueryStatisticsTypeDef,
         "result": ProtectedQueryResultTypeDef,
@@ -1489,15 +1656,15 @@
 )
 
 ConfiguredTableAnalysisRuleTypeDef = TypedDict(
     "ConfiguredTableAnalysisRuleTypeDef",
     {
         "configuredTableId": str,
         "configuredTableArn": str,
-        "policy": ConfiguredTableAnalysisRulePolicyTypeDef,
+        "policy": ConfiguredTableAnalysisRulePolicyOutputTypeDef,
         "type": ConfiguredTableAnalysisRuleTypeType,
         "createTime": datetime,
         "updateTime": datetime,
     },
 )
 
 CreateConfiguredTableAnalysisRuleInputRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms/type_defs.pyi` & `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for cleanrooms service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_cleanrooms.type_defs import AggregateColumnTypeDef
+    from mypy_boto3_cleanrooms.type_defs import AggregateColumnOutputTypeDef
 
-    data: AggregateColumnTypeDef = {...}
+    data: AggregateColumnOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -37,25 +37,29 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AggregateColumnOutputTypeDef",
     "AggregateColumnTypeDef",
+    "AggregationConstraintOutputTypeDef",
     "AggregationConstraintTypeDef",
+    "AnalysisRuleListOutputTypeDef",
     "AnalysisRuleListTypeDef",
     "BatchGetSchemaErrorTypeDef",
     "BatchGetSchemaInputRequestTypeDef",
     "CollaborationSummaryTypeDef",
-    "DataEncryptionMetadataTypeDef",
+    "DataEncryptionMetadataOutputTypeDef",
     "ColumnTypeDef",
     "ConfiguredTableAssociationSummaryTypeDef",
     "ConfiguredTableAssociationTypeDef",
     "ConfiguredTableSummaryTypeDef",
+    "DataEncryptionMetadataTypeDef",
     "MemberSpecificationTypeDef",
     "CreateConfiguredTableAssociationInputRequestTypeDef",
     "CreateMembershipInputRequestTypeDef",
     "MembershipTypeDef",
     "DeleteCollaborationInputRequestTypeDef",
     "DeleteConfiguredTableAnalysisRuleInputRequestTypeDef",
     "DeleteConfiguredTableAssociationInputRequestTypeDef",
@@ -66,14 +70,15 @@
     "GetConfiguredTableAnalysisRuleInputRequestTypeDef",
     "GetConfiguredTableAssociationInputRequestTypeDef",
     "GetConfiguredTableInputRequestTypeDef",
     "GetMembershipInputRequestTypeDef",
     "GetProtectedQueryInputRequestTypeDef",
     "GetSchemaAnalysisRuleInputRequestTypeDef",
     "GetSchemaInputRequestTypeDef",
+    "GlueTableReferenceOutputTypeDef",
     "GlueTableReferenceTypeDef",
     "ListCollaborationsInputListCollaborationsPaginateTypeDef",
     "ListCollaborationsInputRequestTypeDef",
     "ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
     "ListConfiguredTableAssociationsInputRequestTypeDef",
     "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
     "ListConfiguredTablesInputRequestTypeDef",
@@ -89,58 +94,66 @@
     "ListSchemasInputListSchemasPaginateTypeDef",
     "ListSchemasInputRequestTypeDef",
     "SchemaSummaryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ProtectedQueryErrorTypeDef",
+    "ProtectedQueryS3OutputConfigurationOutputTypeDef",
     "ProtectedQueryS3OutputConfigurationTypeDef",
     "ProtectedQueryS3OutputTypeDef",
+    "ProtectedQuerySQLParametersOutputTypeDef",
     "ProtectedQuerySQLParametersTypeDef",
     "ProtectedQueryStatisticsTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateCollaborationInputRequestTypeDef",
     "UpdateConfiguredTableAssociationInputRequestTypeDef",
     "UpdateConfiguredTableInputRequestTypeDef",
     "UpdateMembershipInputRequestTypeDef",
     "UpdateProtectedQueryInputRequestTypeDef",
+    "AnalysisRuleAggregationOutputTypeDef",
     "AnalysisRuleAggregationTypeDef",
     "ListCollaborationsOutputTypeDef",
     "CollaborationTypeDef",
     "SchemaTypeDef",
     "ListConfiguredTableAssociationsOutputTypeDef",
     "CreateConfiguredTableAssociationOutputTypeDef",
     "GetConfiguredTableAssociationOutputTypeDef",
     "UpdateConfiguredTableAssociationOutputTypeDef",
     "ListConfiguredTablesOutputTypeDef",
     "CreateCollaborationInputRequestTypeDef",
     "CreateMembershipOutputTypeDef",
     "GetMembershipOutputTypeDef",
     "UpdateMembershipOutputTypeDef",
+    "TableReferenceOutputTypeDef",
     "TableReferenceTypeDef",
     "ListMembersOutputTypeDef",
     "ListMembershipsOutputTypeDef",
     "ListProtectedQueriesOutputTypeDef",
     "ListSchemasOutputTypeDef",
+    "ProtectedQueryOutputConfigurationOutputTypeDef",
     "ProtectedQueryOutputConfigurationTypeDef",
     "ProtectedQueryOutputTypeDef",
     "AnalysisRulePolicyV1TypeDef",
+    "ConfiguredTableAnalysisRulePolicyV1OutputTypeDef",
     "ConfiguredTableAnalysisRulePolicyV1TypeDef",
     "CreateCollaborationOutputTypeDef",
     "GetCollaborationOutputTypeDef",
     "UpdateCollaborationOutputTypeDef",
     "BatchGetSchemaOutputTypeDef",
     "GetSchemaOutputTypeDef",
     "ConfiguredTableTypeDef",
     "CreateConfiguredTableInputRequestTypeDef",
+    "ProtectedQueryResultConfigurationOutputTypeDef",
     "ProtectedQueryResultConfigurationTypeDef",
     "ProtectedQueryResultTypeDef",
     "AnalysisRulePolicyTypeDef",
+    "ConfiguredTableAnalysisRulePolicyOutputTypeDef",
     "ConfiguredTableAnalysisRulePolicyTypeDef",
     "CreateConfiguredTableOutputTypeDef",
     "GetConfiguredTableOutputTypeDef",
     "UpdateConfiguredTableOutputTypeDef",
     "StartProtectedQueryInputRequestTypeDef",
     "ProtectedQueryTypeDef",
     "AnalysisRuleTypeDef",
@@ -152,31 +165,68 @@
     "UpdateProtectedQueryOutputTypeDef",
     "GetSchemaAnalysisRuleOutputTypeDef",
     "CreateConfiguredTableAnalysisRuleOutputTypeDef",
     "GetConfiguredTableAnalysisRuleOutputTypeDef",
     "UpdateConfiguredTableAnalysisRuleOutputTypeDef",
 )
 
+AggregateColumnOutputTypeDef = TypedDict(
+    "AggregateColumnOutputTypeDef",
+    {
+        "columnNames": List[str],
+        "function": AggregateFunctionNameType,
+    },
+)
+
 AggregateColumnTypeDef = TypedDict(
     "AggregateColumnTypeDef",
     {
         "columnNames": Sequence[str],
         "function": AggregateFunctionNameType,
     },
 )
 
+AggregationConstraintOutputTypeDef = TypedDict(
+    "AggregationConstraintOutputTypeDef",
+    {
+        "columnName": str,
+        "minimum": int,
+        "type": Literal["COUNT_DISTINCT"],
+    },
+)
+
 AggregationConstraintTypeDef = TypedDict(
     "AggregationConstraintTypeDef",
     {
         "columnName": str,
         "minimum": int,
         "type": Literal["COUNT_DISTINCT"],
     },
 )
 
+_RequiredAnalysisRuleListOutputTypeDef = TypedDict(
+    "_RequiredAnalysisRuleListOutputTypeDef",
+    {
+        "joinColumns": List[str],
+        "listColumns": List[str],
+    },
+)
+_OptionalAnalysisRuleListOutputTypeDef = TypedDict(
+    "_OptionalAnalysisRuleListOutputTypeDef",
+    {
+        "allowedJoinOperators": List[JoinOperatorType],
+    },
+    total=False,
+)
+
+class AnalysisRuleListOutputTypeDef(
+    _RequiredAnalysisRuleListOutputTypeDef, _OptionalAnalysisRuleListOutputTypeDef
+):
+    pass
+
 _RequiredAnalysisRuleListTypeDef = TypedDict(
     "_RequiredAnalysisRuleListTypeDef",
     {
         "joinColumns": Sequence[str],
         "listColumns": Sequence[str],
     },
 )
@@ -231,16 +281,16 @@
 )
 
 class CollaborationSummaryTypeDef(
     _RequiredCollaborationSummaryTypeDef, _OptionalCollaborationSummaryTypeDef
 ):
     pass
 
-DataEncryptionMetadataTypeDef = TypedDict(
-    "DataEncryptionMetadataTypeDef",
+DataEncryptionMetadataOutputTypeDef = TypedDict(
+    "DataEncryptionMetadataOutputTypeDef",
     {
         "allowCleartext": bool,
         "allowDuplicates": bool,
         "allowJoinsOnColumnsWithDifferentNames": bool,
         "preserveNulls": bool,
     },
 )
@@ -304,14 +354,24 @@
         "createTime": datetime,
         "updateTime": datetime,
         "analysisRuleTypes": List[ConfiguredTableAnalysisRuleTypeType],
         "analysisMethod": Literal["DIRECT_QUERY"],
     },
 )
 
+DataEncryptionMetadataTypeDef = TypedDict(
+    "DataEncryptionMetadataTypeDef",
+    {
+        "allowCleartext": bool,
+        "allowDuplicates": bool,
+        "allowJoinsOnColumnsWithDifferentNames": bool,
+        "preserveNulls": bool,
+    },
+)
+
 MemberSpecificationTypeDef = TypedDict(
     "MemberSpecificationTypeDef",
     {
         "accountId": str,
         "memberAbilities": Sequence[MemberAbilityType],
         "displayName": str,
     },
@@ -482,14 +542,22 @@
     "GetSchemaInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
         "name": str,
     },
 )
 
+GlueTableReferenceOutputTypeDef = TypedDict(
+    "GlueTableReferenceOutputTypeDef",
+    {
+        "tableName": str,
+        "databaseName": str,
+    },
+)
+
 GlueTableReferenceTypeDef = TypedDict(
     "GlueTableReferenceTypeDef",
     {
         "tableName": str,
         "databaseName": str,
     },
 )
@@ -819,14 +887,35 @@
     "ProtectedQueryErrorTypeDef",
     {
         "message": str,
         "code": str,
     },
 )
 
+_RequiredProtectedQueryS3OutputConfigurationOutputTypeDef = TypedDict(
+    "_RequiredProtectedQueryS3OutputConfigurationOutputTypeDef",
+    {
+        "resultFormat": ResultFormatType,
+        "bucket": str,
+    },
+)
+_OptionalProtectedQueryS3OutputConfigurationOutputTypeDef = TypedDict(
+    "_OptionalProtectedQueryS3OutputConfigurationOutputTypeDef",
+    {
+        "keyPrefix": str,
+    },
+    total=False,
+)
+
+class ProtectedQueryS3OutputConfigurationOutputTypeDef(
+    _RequiredProtectedQueryS3OutputConfigurationOutputTypeDef,
+    _OptionalProtectedQueryS3OutputConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredProtectedQueryS3OutputConfigurationTypeDef = TypedDict(
     "_RequiredProtectedQueryS3OutputConfigurationTypeDef",
     {
         "resultFormat": ResultFormatType,
         "bucket": str,
     },
 )
@@ -847,14 +936,22 @@
 ProtectedQueryS3OutputTypeDef = TypedDict(
     "ProtectedQueryS3OutputTypeDef",
     {
         "location": str,
     },
 )
 
+ProtectedQuerySQLParametersOutputTypeDef = TypedDict(
+    "ProtectedQuerySQLParametersOutputTypeDef",
+    {
+        "queryString": str,
+    },
+    total=False,
+)
+
 ProtectedQuerySQLParametersTypeDef = TypedDict(
     "ProtectedQuerySQLParametersTypeDef",
     {
         "queryString": str,
     },
     total=False,
 )
@@ -981,14 +1078,38 @@
     {
         "membershipIdentifier": str,
         "protectedQueryIdentifier": str,
         "targetStatus": Literal["CANCELLED"],
     },
 )
 
+_RequiredAnalysisRuleAggregationOutputTypeDef = TypedDict(
+    "_RequiredAnalysisRuleAggregationOutputTypeDef",
+    {
+        "aggregateColumns": List[AggregateColumnOutputTypeDef],
+        "joinColumns": List[str],
+        "dimensionColumns": List[str],
+        "scalarFunctions": List[ScalarFunctionsType],
+        "outputConstraints": List[AggregationConstraintOutputTypeDef],
+    },
+)
+_OptionalAnalysisRuleAggregationOutputTypeDef = TypedDict(
+    "_OptionalAnalysisRuleAggregationOutputTypeDef",
+    {
+        "joinRequired": Literal["QUERY_RUNNER"],
+        "allowedJoinOperators": List[JoinOperatorType],
+    },
+    total=False,
+)
+
+class AnalysisRuleAggregationOutputTypeDef(
+    _RequiredAnalysisRuleAggregationOutputTypeDef, _OptionalAnalysisRuleAggregationOutputTypeDef
+):
+    pass
+
 _RequiredAnalysisRuleAggregationTypeDef = TypedDict(
     "_RequiredAnalysisRuleAggregationTypeDef",
     {
         "aggregateColumns": Sequence[AggregateColumnTypeDef],
         "joinColumns": Sequence[str],
         "dimensionColumns": Sequence[str],
         "scalarFunctions": Sequence[ScalarFunctionsType],
@@ -1034,15 +1155,15 @@
 )
 _OptionalCollaborationTypeDef = TypedDict(
     "_OptionalCollaborationTypeDef",
     {
         "description": str,
         "membershipId": str,
         "membershipArn": str,
-        "dataEncryptionMetadata": DataEncryptionMetadataTypeDef,
+        "dataEncryptionMetadata": DataEncryptionMetadataOutputTypeDef,
     },
     total=False,
 )
 
 class CollaborationTypeDef(_RequiredCollaborationTypeDef, _OptionalCollaborationTypeDef):
     pass
 
@@ -1160,14 +1281,22 @@
     "UpdateMembershipOutputTypeDef",
     {
         "membership": MembershipTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TableReferenceOutputTypeDef = TypedDict(
+    "TableReferenceOutputTypeDef",
+    {
+        "glue": GlueTableReferenceOutputTypeDef,
+    },
+    total=False,
+)
+
 TableReferenceTypeDef = TypedDict(
     "TableReferenceTypeDef",
     {
         "glue": GlueTableReferenceTypeDef,
     },
     total=False,
 )
@@ -1204,14 +1333,22 @@
     {
         "schemaSummaries": List[SchemaSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ProtectedQueryOutputConfigurationOutputTypeDef = TypedDict(
+    "ProtectedQueryOutputConfigurationOutputTypeDef",
+    {
+        "s3": ProtectedQueryS3OutputConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ProtectedQueryOutputConfigurationTypeDef = TypedDict(
     "ProtectedQueryOutputConfigurationTypeDef",
     {
         "s3": ProtectedQueryS3OutputConfigurationTypeDef,
     },
     total=False,
 )
@@ -1223,16 +1360,25 @@
     },
     total=False,
 )
 
 AnalysisRulePolicyV1TypeDef = TypedDict(
     "AnalysisRulePolicyV1TypeDef",
     {
-        "list": AnalysisRuleListTypeDef,
-        "aggregation": AnalysisRuleAggregationTypeDef,
+        "list": AnalysisRuleListOutputTypeDef,
+        "aggregation": AnalysisRuleAggregationOutputTypeDef,
+    },
+    total=False,
+)
+
+ConfiguredTableAnalysisRulePolicyV1OutputTypeDef = TypedDict(
+    "ConfiguredTableAnalysisRulePolicyV1OutputTypeDef",
+    {
+        "list": AnalysisRuleListOutputTypeDef,
+        "aggregation": AnalysisRuleAggregationOutputTypeDef,
     },
     total=False,
 )
 
 ConfiguredTableAnalysisRulePolicyV1TypeDef = TypedDict(
     "ConfiguredTableAnalysisRulePolicyV1TypeDef",
     {
@@ -1285,15 +1431,15 @@
 
 _RequiredConfiguredTableTypeDef = TypedDict(
     "_RequiredConfiguredTableTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
-        "tableReference": TableReferenceTypeDef,
+        "tableReference": TableReferenceOutputTypeDef,
         "createTime": datetime,
         "updateTime": datetime,
         "analysisRuleTypes": List[ConfiguredTableAnalysisRuleTypeType],
         "analysisMethod": Literal["DIRECT_QUERY"],
         "allowedColumns": List[str],
     },
 )
@@ -1328,14 +1474,21 @@
 
 class CreateConfiguredTableInputRequestTypeDef(
     _RequiredCreateConfiguredTableInputRequestTypeDef,
     _OptionalCreateConfiguredTableInputRequestTypeDef,
 ):
     pass
 
+ProtectedQueryResultConfigurationOutputTypeDef = TypedDict(
+    "ProtectedQueryResultConfigurationOutputTypeDef",
+    {
+        "outputConfiguration": ProtectedQueryOutputConfigurationOutputTypeDef,
+    },
+)
+
 ProtectedQueryResultConfigurationTypeDef = TypedDict(
     "ProtectedQueryResultConfigurationTypeDef",
     {
         "outputConfiguration": ProtectedQueryOutputConfigurationTypeDef,
     },
 )
 
@@ -1350,14 +1503,22 @@
     "AnalysisRulePolicyTypeDef",
     {
         "v1": AnalysisRulePolicyV1TypeDef,
     },
     total=False,
 )
 
+ConfiguredTableAnalysisRulePolicyOutputTypeDef = TypedDict(
+    "ConfiguredTableAnalysisRulePolicyOutputTypeDef",
+    {
+        "v1": ConfiguredTableAnalysisRulePolicyV1OutputTypeDef,
+    },
+    total=False,
+)
+
 ConfiguredTableAnalysisRulePolicyTypeDef = TypedDict(
     "ConfiguredTableAnalysisRulePolicyTypeDef",
     {
         "v1": ConfiguredTableAnalysisRulePolicyV1TypeDef,
     },
     total=False,
 )
@@ -1399,17 +1560,17 @@
 _RequiredProtectedQueryTypeDef = TypedDict(
     "_RequiredProtectedQueryTypeDef",
     {
         "id": str,
         "membershipId": str,
         "membershipArn": str,
         "createTime": datetime,
-        "sqlParameters": ProtectedQuerySQLParametersTypeDef,
+        "sqlParameters": ProtectedQuerySQLParametersOutputTypeDef,
         "status": ProtectedQueryStatusType,
-        "resultConfiguration": ProtectedQueryResultConfigurationTypeDef,
+        "resultConfiguration": ProtectedQueryResultConfigurationOutputTypeDef,
     },
 )
 _OptionalProtectedQueryTypeDef = TypedDict(
     "_OptionalProtectedQueryTypeDef",
     {
         "statistics": ProtectedQueryStatisticsTypeDef,
         "result": ProtectedQueryResultTypeDef,
@@ -1434,15 +1595,15 @@
 )
 
 ConfiguredTableAnalysisRuleTypeDef = TypedDict(
     "ConfiguredTableAnalysisRuleTypeDef",
     {
         "configuredTableId": str,
         "configuredTableArn": str,
-        "policy": ConfiguredTableAnalysisRulePolicyTypeDef,
+        "policy": ConfiguredTableAnalysisRulePolicyOutputTypeDef,
         "type": ConfiguredTableAnalysisRuleTypeType,
         "createTime": datetime,
         "updateTime": datetime,
     },
 )
 
 CreateConfiguredTableAnalysisRuleInputRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms.egg-info/PKG-INFO` & `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cleanrooms
-Version: 1.28.0
-Summary: Type annotations for boto3.CleanRoomsService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CleanRoomsService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cleanrooms"></a>
 
 # mypy-boto3-cleanrooms
 
 [![PyPI - mypy-boto3-cleanrooms](https://img.shields.io/pypi/v/mypy-boto3-cleanrooms.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanrooms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cleanrooms.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanrooms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cleanrooms?color=blue)](https://pypistats.org/packages/mypy-boto3-cleanrooms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cleanrooms)](https://pepy.tech/project/mypy-boto3-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CleanRoomsService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
+[boto3.CleanRoomsService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
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
 [mypy-boto3-cleanrooms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -366,25 +366,29 @@
 ### Typed dictionaries
 
 `mypy_boto3_cleanrooms.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cleanrooms.type_defs import (
+    AggregateColumnOutputTypeDef,
     AggregateColumnTypeDef,
+    AggregationConstraintOutputTypeDef,
     AggregationConstraintTypeDef,
+    AnalysisRuleListOutputTypeDef,
     AnalysisRuleListTypeDef,
     BatchGetSchemaErrorTypeDef,
     BatchGetSchemaInputRequestTypeDef,
     CollaborationSummaryTypeDef,
-    DataEncryptionMetadataTypeDef,
+    DataEncryptionMetadataOutputTypeDef,
     ColumnTypeDef,
     ConfiguredTableAssociationSummaryTypeDef,
     ConfiguredTableAssociationTypeDef,
     ConfiguredTableSummaryTypeDef,
+    DataEncryptionMetadataTypeDef,
     MemberSpecificationTypeDef,
     CreateConfiguredTableAssociationInputRequestTypeDef,
     CreateMembershipInputRequestTypeDef,
     MembershipTypeDef,
     DeleteCollaborationInputRequestTypeDef,
     DeleteConfiguredTableAnalysisRuleInputRequestTypeDef,
     DeleteConfiguredTableAssociationInputRequestTypeDef,
@@ -395,14 +399,15 @@
     GetConfiguredTableAnalysisRuleInputRequestTypeDef,
     GetConfiguredTableAssociationInputRequestTypeDef,
     GetConfiguredTableInputRequestTypeDef,
     GetMembershipInputRequestTypeDef,
     GetProtectedQueryInputRequestTypeDef,
     GetSchemaAnalysisRuleInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
+    GlueTableReferenceOutputTypeDef,
     GlueTableReferenceTypeDef,
     ListCollaborationsInputListCollaborationsPaginateTypeDef,
     ListCollaborationsInputRequestTypeDef,
     ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
     ListConfiguredTableAssociationsInputRequestTypeDef,
     ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef,
     ListConfiguredTablesInputRequestTypeDef,
@@ -418,58 +423,66 @@
     ListSchemasInputListSchemasPaginateTypeDef,
     ListSchemasInputRequestTypeDef,
     SchemaSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     PaginatorConfigTypeDef,
     ProtectedQueryErrorTypeDef,
+    ProtectedQueryS3OutputConfigurationOutputTypeDef,
     ProtectedQueryS3OutputConfigurationTypeDef,
     ProtectedQueryS3OutputTypeDef,
+    ProtectedQuerySQLParametersOutputTypeDef,
     ProtectedQuerySQLParametersTypeDef,
     ProtectedQueryStatisticsTypeDef,
     ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateCollaborationInputRequestTypeDef,
     UpdateConfiguredTableAssociationInputRequestTypeDef,
     UpdateConfiguredTableInputRequestTypeDef,
     UpdateMembershipInputRequestTypeDef,
     UpdateProtectedQueryInputRequestTypeDef,
+    AnalysisRuleAggregationOutputTypeDef,
     AnalysisRuleAggregationTypeDef,
     ListCollaborationsOutputTypeDef,
     CollaborationTypeDef,
     SchemaTypeDef,
     ListConfiguredTableAssociationsOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     GetConfiguredTableAssociationOutputTypeDef,
     UpdateConfiguredTableAssociationOutputTypeDef,
     ListConfiguredTablesOutputTypeDef,
     CreateCollaborationInputRequestTypeDef,
     CreateMembershipOutputTypeDef,
     GetMembershipOutputTypeDef,
     UpdateMembershipOutputTypeDef,
+    TableReferenceOutputTypeDef,
     TableReferenceTypeDef,
     ListMembersOutputTypeDef,
     ListMembershipsOutputTypeDef,
     ListProtectedQueriesOutputTypeDef,
     ListSchemasOutputTypeDef,
+    ProtectedQueryOutputConfigurationOutputTypeDef,
     ProtectedQueryOutputConfigurationTypeDef,
     ProtectedQueryOutputTypeDef,
     AnalysisRulePolicyV1TypeDef,
+    ConfiguredTableAnalysisRulePolicyV1OutputTypeDef,
     ConfiguredTableAnalysisRulePolicyV1TypeDef,
     CreateCollaborationOutputTypeDef,
     GetCollaborationOutputTypeDef,
     UpdateCollaborationOutputTypeDef,
     BatchGetSchemaOutputTypeDef,
     GetSchemaOutputTypeDef,
     ConfiguredTableTypeDef,
     CreateConfiguredTableInputRequestTypeDef,
+    ProtectedQueryResultConfigurationOutputTypeDef,
     ProtectedQueryResultConfigurationTypeDef,
     ProtectedQueryResultTypeDef,
     AnalysisRulePolicyTypeDef,
+    ConfiguredTableAnalysisRulePolicyOutputTypeDef,
     ConfiguredTableAnalysisRulePolicyTypeDef,
     CreateConfiguredTableOutputTypeDef,
     GetConfiguredTableOutputTypeDef,
     UpdateConfiguredTableOutputTypeDef,
     StartProtectedQueryInputRequestTypeDef,
     ProtectedQueryTypeDef,
     AnalysisRuleTypeDef,
@@ -482,15 +495,15 @@
     GetSchemaAnalysisRuleOutputTypeDef,
     CreateConfiguredTableAnalysisRuleOutputTypeDef,
     GetConfiguredTableAnalysisRuleOutputTypeDef,
     UpdateConfiguredTableAnalysisRuleOutputTypeDef,
 )
 
 
-def get_structure() -> AggregateColumnTypeDef:
+def get_structure() -> AggregateColumnOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cleanrooms-1.28.0/mypy_boto3_cleanrooms.egg-info/SOURCES.txt` & `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.0/setup.py` & `mypy-boto3-cleanrooms-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cleanrooms",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_cleanrooms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CleanRoomsService 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.CleanRoomsService 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

