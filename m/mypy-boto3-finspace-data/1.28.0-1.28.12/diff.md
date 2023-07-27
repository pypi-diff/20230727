# Comparing `tmp/mypy-boto3-finspace-data-1.28.0.tar.gz` & `tmp/mypy-boto3-finspace-data-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-finspace-data-1.28.0.tar", last modified: Thu Jul  6 20:59:35 2023, max compression
+gzip compressed data, was "mypy-boto3-finspace-data-1.28.12.tar", last modified: Thu Jul 27 05:34:41 2023, max compression
```

## Comparing `mypy-boto3-finspace-data-1.28.0.tar` & `mypy-boto3-finspace-data-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:35.078302 mypy-boto3-finspace-data-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:41:00.000000 mypy-boto3-finspace-data-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17204 2023-07-06 20:59:35.078302 mypy-boto3-finspace-data-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15696 2023-07-06 20:41:00.000000 mypy-boto3-finspace-data-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:35.070302 mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-06 20:41:00.000000 mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-06 20:41:00.000000 mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-06 20:41:00.000000 mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25240 2023-07-06 20:41:01.000000 mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25197 2023-07-06 20:41:01.000000 mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-07-06 20:41:01.000000 mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-07-06 20:41:01.000000 mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-07-06 20:41:01.000000 mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-06 20:41:01.000000 mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:41:00.000000 mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34527 2023-07-06 20:41:02.000000 mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34474 2023-07-06 20:41:01.000000 mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:41:00.000000 mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:35.078302 mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17204 2023-07-06 20:59:34.000000 mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-06 20:59:34.000000 mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:34.000000 mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:34.000000 mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:34.000000 mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 20:59:34.000000 mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:35.078302 mypy-boto3-finspace-data-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-06 20:41:00.000000 mypy-boto3-finspace-data-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:41.480511 mypy-boto3-finspace-data-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17374 2023-07-27 05:34:41.476511 mypy-boto3-finspace-data-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15864 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:41.472511 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25240 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25197 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36156 2023-07-27 05:22:17.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36101 2023-07-27 05:22:17.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:41.476511 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17374 2023-07-27 05:34:41.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 05:34:41.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:41.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:41.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:41.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 05:34:41.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:41.480511 mypy-boto3-finspace-data-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/setup.py
```

### Comparing `mypy-boto3-finspace-data-1.28.0/LICENSE` & `mypy-boto3-finspace-data-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.0/PKG-INFO` & `mypy-boto3-finspace-data-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-finspace-data
-Version: 1.28.0
-Summary: Type annotations for boto3.FinSpaceData 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.FinSpaceData 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-finspace-data"></a>
 
 # mypy-boto3-finspace-data
 
 [![PyPI - mypy-boto3-finspace-data](https://img.shields.io/pypi/v/mypy-boto3-finspace-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-finspace-data?color=blue)](https://pypistats.org/packages/mypy-boto3-finspace-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-finspace-data)](https://pepy.tech/project/mypy-boto3-finspace-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FinSpaceData 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
+[boto3.FinSpaceData 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
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
 [mypy-boto3-finspace-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,27 +353,30 @@
 
 ```python
 from mypy_boto3_finspace_data.type_defs import (
     AssociateUserToPermissionGroupRequestRequestTypeDef,
     AssociateUserToPermissionGroupResponseTypeDef,
     AwsCredentialsTypeDef,
     ChangesetErrorInfoTypeDef,
+    ColumnDefinitionOutputTypeDef,
     ColumnDefinitionTypeDef,
     CreateChangesetRequestRequestTypeDef,
     CreateChangesetResponseTypeDef,
     DataViewDestinationTypeParamsTypeDef,
     CreateDataViewResponseTypeDef,
     DatasetOwnerInfoTypeDef,
     CreateDatasetResponseTypeDef,
     CreatePermissionGroupRequestRequestTypeDef,
     CreatePermissionGroupResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     CreateUserResponseTypeDef,
     CredentialsTypeDef,
+    DataViewDestinationTypeParamsOutputTypeDef,
     DataViewErrorInfoTypeDef,
+    DatasetOwnerInfoOutputTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteDatasetResponseTypeDef,
     DeletePermissionGroupRequestRequestTypeDef,
     DeletePermissionGroupResponseTypeDef,
     DisableUserRequestRequestTypeDef,
     DisableUserResponseTypeDef,
     DisassociateUserFromPermissionGroupRequestRequestTypeDef,
@@ -417,32 +420,34 @@
     UpdateDatasetResponseTypeDef,
     UpdatePermissionGroupRequestRequestTypeDef,
     UpdatePermissionGroupResponseTypeDef,
     UpdateUserRequestRequestTypeDef,
     UpdateUserResponseTypeDef,
     ChangesetSummaryTypeDef,
     GetChangesetResponseTypeDef,
+    SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
     CreateDataViewRequestRequestTypeDef,
     GetProgrammaticAccessCredentialsResponseTypeDef,
     DataViewSummaryTypeDef,
     GetDataViewResponseTypeDef,
     GetExternalDataViewAccessDetailsResponseTypeDef,
     GetPermissionGroupResponseTypeDef,
     ListPermissionGroupsResponseTypeDef,
     ListPermissionGroupsByUserResponseTypeDef,
     ListUsersByPermissionGroupResponseTypeDef,
     ListUsersResponseTypeDef,
     PermissionGroupParamsTypeDef,
     ListChangesetsResponseTypeDef,
+    SchemaUnionOutputTypeDef,
     SchemaUnionTypeDef,
     ListDataViewsResponseTypeDef,
-    CreateDatasetRequestRequestTypeDef,
     DatasetTypeDef,
     GetDatasetResponseTypeDef,
+    CreateDatasetRequestRequestTypeDef,
     UpdateDatasetRequestRequestTypeDef,
     ListDatasetsResponseTypeDef,
 )
 
 
 def get_structure() -> AssociateUserToPermissionGroupRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-finspace-data-1.28.0/README.md` & `mypy-boto3-finspace-data-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-finspace-data"></a>
 
 # mypy-boto3-finspace-data
 
 [![PyPI - mypy-boto3-finspace-data](https://img.shields.io/pypi/v/mypy-boto3-finspace-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-finspace-data?color=blue)](https://pypistats.org/packages/mypy-boto3-finspace-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-finspace-data)](https://pepy.tech/project/mypy-boto3-finspace-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FinSpaceData 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
+[boto3.FinSpaceData 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
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
 [mypy-boto3-finspace-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,27 +321,30 @@
 
 ```python
 from mypy_boto3_finspace_data.type_defs import (
     AssociateUserToPermissionGroupRequestRequestTypeDef,
     AssociateUserToPermissionGroupResponseTypeDef,
     AwsCredentialsTypeDef,
     ChangesetErrorInfoTypeDef,
+    ColumnDefinitionOutputTypeDef,
     ColumnDefinitionTypeDef,
     CreateChangesetRequestRequestTypeDef,
     CreateChangesetResponseTypeDef,
     DataViewDestinationTypeParamsTypeDef,
     CreateDataViewResponseTypeDef,
     DatasetOwnerInfoTypeDef,
     CreateDatasetResponseTypeDef,
     CreatePermissionGroupRequestRequestTypeDef,
     CreatePermissionGroupResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     CreateUserResponseTypeDef,
     CredentialsTypeDef,
+    DataViewDestinationTypeParamsOutputTypeDef,
     DataViewErrorInfoTypeDef,
+    DatasetOwnerInfoOutputTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteDatasetResponseTypeDef,
     DeletePermissionGroupRequestRequestTypeDef,
     DeletePermissionGroupResponseTypeDef,
     DisableUserRequestRequestTypeDef,
     DisableUserResponseTypeDef,
     DisassociateUserFromPermissionGroupRequestRequestTypeDef,
@@ -385,32 +388,34 @@
     UpdateDatasetResponseTypeDef,
     UpdatePermissionGroupRequestRequestTypeDef,
     UpdatePermissionGroupResponseTypeDef,
     UpdateUserRequestRequestTypeDef,
     UpdateUserResponseTypeDef,
     ChangesetSummaryTypeDef,
     GetChangesetResponseTypeDef,
+    SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
     CreateDataViewRequestRequestTypeDef,
     GetProgrammaticAccessCredentialsResponseTypeDef,
     DataViewSummaryTypeDef,
     GetDataViewResponseTypeDef,
     GetExternalDataViewAccessDetailsResponseTypeDef,
     GetPermissionGroupResponseTypeDef,
     ListPermissionGroupsResponseTypeDef,
     ListPermissionGroupsByUserResponseTypeDef,
     ListUsersByPermissionGroupResponseTypeDef,
     ListUsersResponseTypeDef,
     PermissionGroupParamsTypeDef,
     ListChangesetsResponseTypeDef,
+    SchemaUnionOutputTypeDef,
     SchemaUnionTypeDef,
     ListDataViewsResponseTypeDef,
-    CreateDatasetRequestRequestTypeDef,
     DatasetTypeDef,
     GetDatasetResponseTypeDef,
+    CreateDatasetRequestRequestTypeDef,
     UpdateDatasetRequestRequestTypeDef,
     ListDatasetsResponseTypeDef,
 )
 
 
 def get_structure() -> AssociateUserToPermissionGroupRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/__init__.py` & `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/__init__.pyi` & `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/__main__.py` & `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FinSpaceData 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.FinSpaceData 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData\nOther"
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

### Comparing `mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/client.py` & `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/client.pyi` & `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/literals.py` & `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,14 +223,15 @@
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
@@ -309,26 +310,28 @@
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

### Comparing `mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/literals.pyi` & `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -221,14 +221,15 @@
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
@@ -307,26 +308,28 @@
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

### Comparing `mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/paginator.py` & `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/paginator.pyi` & `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/type_defs.py` & `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,27 +38,30 @@
 
 
 __all__ = (
     "AssociateUserToPermissionGroupRequestRequestTypeDef",
     "AssociateUserToPermissionGroupResponseTypeDef",
     "AwsCredentialsTypeDef",
     "ChangesetErrorInfoTypeDef",
+    "ColumnDefinitionOutputTypeDef",
     "ColumnDefinitionTypeDef",
     "CreateChangesetRequestRequestTypeDef",
     "CreateChangesetResponseTypeDef",
     "DataViewDestinationTypeParamsTypeDef",
     "CreateDataViewResponseTypeDef",
     "DatasetOwnerInfoTypeDef",
     "CreateDatasetResponseTypeDef",
     "CreatePermissionGroupRequestRequestTypeDef",
     "CreatePermissionGroupResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
     "CreateUserResponseTypeDef",
     "CredentialsTypeDef",
+    "DataViewDestinationTypeParamsOutputTypeDef",
     "DataViewErrorInfoTypeDef",
+    "DatasetOwnerInfoOutputTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteDatasetResponseTypeDef",
     "DeletePermissionGroupRequestRequestTypeDef",
     "DeletePermissionGroupResponseTypeDef",
     "DisableUserRequestRequestTypeDef",
     "DisableUserResponseTypeDef",
     "DisassociateUserFromPermissionGroupRequestRequestTypeDef",
@@ -102,32 +105,34 @@
     "UpdateDatasetResponseTypeDef",
     "UpdatePermissionGroupRequestRequestTypeDef",
     "UpdatePermissionGroupResponseTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UpdateUserResponseTypeDef",
     "ChangesetSummaryTypeDef",
     "GetChangesetResponseTypeDef",
+    "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
     "CreateDataViewRequestRequestTypeDef",
     "GetProgrammaticAccessCredentialsResponseTypeDef",
     "DataViewSummaryTypeDef",
     "GetDataViewResponseTypeDef",
     "GetExternalDataViewAccessDetailsResponseTypeDef",
     "GetPermissionGroupResponseTypeDef",
     "ListPermissionGroupsResponseTypeDef",
     "ListPermissionGroupsByUserResponseTypeDef",
     "ListUsersByPermissionGroupResponseTypeDef",
     "ListUsersResponseTypeDef",
     "PermissionGroupParamsTypeDef",
     "ListChangesetsResponseTypeDef",
+    "SchemaUnionOutputTypeDef",
     "SchemaUnionTypeDef",
     "ListDataViewsResponseTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
     "DatasetTypeDef",
     "GetDatasetResponseTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
     "UpdateDatasetRequestRequestTypeDef",
     "ListDatasetsResponseTypeDef",
 )
 
 _RequiredAssociateUserToPermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateUserToPermissionGroupRequestRequestTypeDef",
     {
@@ -175,14 +180,24 @@
     {
         "errorMessage": str,
         "errorCategory": ErrorCategoryType,
     },
     total=False,
 )
 
+ColumnDefinitionOutputTypeDef = TypedDict(
+    "ColumnDefinitionOutputTypeDef",
+    {
+        "dataType": ColumnDataTypeType,
+        "columnName": str,
+        "columnDescription": str,
+    },
+    total=False,
+)
+
 ColumnDefinitionTypeDef = TypedDict(
     "ColumnDefinitionTypeDef",
     {
         "dataType": ColumnDataTypeType,
         "columnName": str,
         "columnDescription": str,
     },
@@ -343,23 +358,56 @@
         "accessKeyId": str,
         "secretAccessKey": str,
         "sessionToken": str,
     },
     total=False,
 )
 
+_RequiredDataViewDestinationTypeParamsOutputTypeDef = TypedDict(
+    "_RequiredDataViewDestinationTypeParamsOutputTypeDef",
+    {
+        "destinationType": str,
+    },
+)
+_OptionalDataViewDestinationTypeParamsOutputTypeDef = TypedDict(
+    "_OptionalDataViewDestinationTypeParamsOutputTypeDef",
+    {
+        "s3DestinationExportFileFormat": ExportFileFormatType,
+        "s3DestinationExportFileFormatOptions": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class DataViewDestinationTypeParamsOutputTypeDef(
+    _RequiredDataViewDestinationTypeParamsOutputTypeDef,
+    _OptionalDataViewDestinationTypeParamsOutputTypeDef,
+):
+    pass
+
+
 DataViewErrorInfoTypeDef = TypedDict(
     "DataViewErrorInfoTypeDef",
     {
         "errorMessage": str,
         "errorCategory": ErrorCategoryType,
     },
     total=False,
 )
 
+DatasetOwnerInfoOutputTypeDef = TypedDict(
+    "DatasetOwnerInfoOutputTypeDef",
+    {
+        "name": str,
+        "phoneNumber": str,
+        "email": str,
+    },
+    total=False,
+)
+
 _RequiredDeleteDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDatasetRequestRequestTypeDef",
     {
         "datasetId": str,
     },
 )
 _OptionalDeleteDatasetRequestRequestTypeDef = TypedDict(
@@ -1090,14 +1138,23 @@
         "activeFromTimestamp": int,
         "updatesChangesetId": str,
         "updatedByChangesetId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+SchemaDefinitionOutputTypeDef = TypedDict(
+    "SchemaDefinitionOutputTypeDef",
+    {
+        "columns": List[ColumnDefinitionOutputTypeDef],
+        "primaryKeyColumns": List[str],
+    },
+    total=False,
+)
+
 SchemaDefinitionTypeDef = TypedDict(
     "SchemaDefinitionTypeDef",
     {
         "columns": Sequence[ColumnDefinitionTypeDef],
         "primaryKeyColumns": Sequence[str],
     },
     total=False,
@@ -1145,15 +1202,15 @@
         "dataViewArn": str,
         "datasetId": str,
         "asOfTimestamp": int,
         "partitionColumns": List[str],
         "sortColumns": List[str],
         "status": DataViewStatusType,
         "errorInfo": DataViewErrorInfoTypeDef,
-        "destinationTypeProperties": DataViewDestinationTypeParamsTypeDef,
+        "destinationTypeProperties": DataViewDestinationTypeParamsOutputTypeDef,
         "autoUpdate": bool,
         "createTime": int,
         "lastModifiedTime": int,
     },
     total=False,
 )
 
@@ -1166,15 +1223,15 @@
         "asOfTimestamp": int,
         "errorInfo": DataViewErrorInfoTypeDef,
         "lastModifiedTime": int,
         "createTime": int,
         "sortColumns": List[str],
         "dataViewId": str,
         "dataViewArn": str,
-        "destinationTypeParams": DataViewDestinationTypeParamsTypeDef,
+        "destinationTypeParams": DataViewDestinationTypeParamsOutputTypeDef,
         "status": DataViewStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetExternalDataViewAccessDetailsResponseTypeDef = TypedDict(
     "GetExternalDataViewAccessDetailsResponseTypeDef",
@@ -1243,14 +1300,22 @@
     {
         "changesets": List[ChangesetSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+SchemaUnionOutputTypeDef = TypedDict(
+    "SchemaUnionOutputTypeDef",
+    {
+        "tabularSchemaConfig": SchemaDefinitionOutputTypeDef,
+    },
+    total=False,
+)
+
 SchemaUnionTypeDef = TypedDict(
     "SchemaUnionTypeDef",
     {
         "tabularSchemaConfig": SchemaDefinitionTypeDef,
     },
     total=False,
 )
@@ -1260,53 +1325,26 @@
     {
         "nextToken": str,
         "dataViews": List[DataViewSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetRequestRequestTypeDef",
-    {
-        "datasetTitle": str,
-        "kind": DatasetKindType,
-        "permissionGroupParams": PermissionGroupParamsTypeDef,
-    },
-)
-_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "datasetDescription": str,
-        "ownerInfo": DatasetOwnerInfoTypeDef,
-        "alias": str,
-        "schemaDefinition": SchemaUnionTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateDatasetRequestRequestTypeDef(
-    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
-):
-    pass
-
-
 DatasetTypeDef = TypedDict(
     "DatasetTypeDef",
     {
         "datasetId": str,
         "datasetArn": str,
         "datasetTitle": str,
         "kind": DatasetKindType,
         "datasetDescription": str,
-        "ownerInfo": DatasetOwnerInfoTypeDef,
+        "ownerInfo": DatasetOwnerInfoOutputTypeDef,
         "createTime": int,
         "lastModifiedTime": int,
-        "schemaDefinition": SchemaUnionTypeDef,
+        "schemaDefinition": SchemaUnionOutputTypeDef,
         "alias": str,
     },
     total=False,
 )
 
 GetDatasetResponseTypeDef = TypedDict(
     "GetDatasetResponseTypeDef",
@@ -1314,21 +1352,48 @@
         "datasetId": str,
         "datasetArn": str,
         "datasetTitle": str,
         "kind": DatasetKindType,
         "datasetDescription": str,
         "createTime": int,
         "lastModifiedTime": int,
-        "schemaDefinition": SchemaUnionTypeDef,
+        "schemaDefinition": SchemaUnionOutputTypeDef,
         "alias": str,
         "status": DatasetStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetRequestRequestTypeDef",
+    {
+        "datasetTitle": str,
+        "kind": DatasetKindType,
+        "permissionGroupParams": PermissionGroupParamsTypeDef,
+    },
+)
+_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "datasetDescription": str,
+        "ownerInfo": DatasetOwnerInfoTypeDef,
+        "alias": str,
+        "schemaDefinition": SchemaUnionTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateDatasetRequestRequestTypeDef(
+    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "datasetId": str,
         "datasetTitle": str,
         "kind": DatasetKindType,
     },
```

### Comparing `mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data/type_defs.pyi` & `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -37,27 +37,30 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateUserToPermissionGroupRequestRequestTypeDef",
     "AssociateUserToPermissionGroupResponseTypeDef",
     "AwsCredentialsTypeDef",
     "ChangesetErrorInfoTypeDef",
+    "ColumnDefinitionOutputTypeDef",
     "ColumnDefinitionTypeDef",
     "CreateChangesetRequestRequestTypeDef",
     "CreateChangesetResponseTypeDef",
     "DataViewDestinationTypeParamsTypeDef",
     "CreateDataViewResponseTypeDef",
     "DatasetOwnerInfoTypeDef",
     "CreateDatasetResponseTypeDef",
     "CreatePermissionGroupRequestRequestTypeDef",
     "CreatePermissionGroupResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
     "CreateUserResponseTypeDef",
     "CredentialsTypeDef",
+    "DataViewDestinationTypeParamsOutputTypeDef",
     "DataViewErrorInfoTypeDef",
+    "DatasetOwnerInfoOutputTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteDatasetResponseTypeDef",
     "DeletePermissionGroupRequestRequestTypeDef",
     "DeletePermissionGroupResponseTypeDef",
     "DisableUserRequestRequestTypeDef",
     "DisableUserResponseTypeDef",
     "DisassociateUserFromPermissionGroupRequestRequestTypeDef",
@@ -101,32 +104,34 @@
     "UpdateDatasetResponseTypeDef",
     "UpdatePermissionGroupRequestRequestTypeDef",
     "UpdatePermissionGroupResponseTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UpdateUserResponseTypeDef",
     "ChangesetSummaryTypeDef",
     "GetChangesetResponseTypeDef",
+    "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
     "CreateDataViewRequestRequestTypeDef",
     "GetProgrammaticAccessCredentialsResponseTypeDef",
     "DataViewSummaryTypeDef",
     "GetDataViewResponseTypeDef",
     "GetExternalDataViewAccessDetailsResponseTypeDef",
     "GetPermissionGroupResponseTypeDef",
     "ListPermissionGroupsResponseTypeDef",
     "ListPermissionGroupsByUserResponseTypeDef",
     "ListUsersByPermissionGroupResponseTypeDef",
     "ListUsersResponseTypeDef",
     "PermissionGroupParamsTypeDef",
     "ListChangesetsResponseTypeDef",
+    "SchemaUnionOutputTypeDef",
     "SchemaUnionTypeDef",
     "ListDataViewsResponseTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
     "DatasetTypeDef",
     "GetDatasetResponseTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
     "UpdateDatasetRequestRequestTypeDef",
     "ListDatasetsResponseTypeDef",
 )
 
 _RequiredAssociateUserToPermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateUserToPermissionGroupRequestRequestTypeDef",
     {
@@ -172,14 +177,24 @@
     {
         "errorMessage": str,
         "errorCategory": ErrorCategoryType,
     },
     total=False,
 )
 
+ColumnDefinitionOutputTypeDef = TypedDict(
+    "ColumnDefinitionOutputTypeDef",
+    {
+        "dataType": ColumnDataTypeType,
+        "columnName": str,
+        "columnDescription": str,
+    },
+    total=False,
+)
+
 ColumnDefinitionTypeDef = TypedDict(
     "ColumnDefinitionTypeDef",
     {
         "dataType": ColumnDataTypeType,
         "columnName": str,
         "columnDescription": str,
     },
@@ -332,23 +347,54 @@
         "accessKeyId": str,
         "secretAccessKey": str,
         "sessionToken": str,
     },
     total=False,
 )
 
+_RequiredDataViewDestinationTypeParamsOutputTypeDef = TypedDict(
+    "_RequiredDataViewDestinationTypeParamsOutputTypeDef",
+    {
+        "destinationType": str,
+    },
+)
+_OptionalDataViewDestinationTypeParamsOutputTypeDef = TypedDict(
+    "_OptionalDataViewDestinationTypeParamsOutputTypeDef",
+    {
+        "s3DestinationExportFileFormat": ExportFileFormatType,
+        "s3DestinationExportFileFormatOptions": Dict[str, str],
+    },
+    total=False,
+)
+
+class DataViewDestinationTypeParamsOutputTypeDef(
+    _RequiredDataViewDestinationTypeParamsOutputTypeDef,
+    _OptionalDataViewDestinationTypeParamsOutputTypeDef,
+):
+    pass
+
 DataViewErrorInfoTypeDef = TypedDict(
     "DataViewErrorInfoTypeDef",
     {
         "errorMessage": str,
         "errorCategory": ErrorCategoryType,
     },
     total=False,
 )
 
+DatasetOwnerInfoOutputTypeDef = TypedDict(
+    "DatasetOwnerInfoOutputTypeDef",
+    {
+        "name": str,
+        "phoneNumber": str,
+        "email": str,
+    },
+    total=False,
+)
+
 _RequiredDeleteDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDatasetRequestRequestTypeDef",
     {
         "datasetId": str,
     },
 )
 _OptionalDeleteDatasetRequestRequestTypeDef = TypedDict(
@@ -1043,14 +1089,23 @@
         "activeFromTimestamp": int,
         "updatesChangesetId": str,
         "updatedByChangesetId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+SchemaDefinitionOutputTypeDef = TypedDict(
+    "SchemaDefinitionOutputTypeDef",
+    {
+        "columns": List[ColumnDefinitionOutputTypeDef],
+        "primaryKeyColumns": List[str],
+    },
+    total=False,
+)
+
 SchemaDefinitionTypeDef = TypedDict(
     "SchemaDefinitionTypeDef",
     {
         "columns": Sequence[ColumnDefinitionTypeDef],
         "primaryKeyColumns": Sequence[str],
     },
     total=False,
@@ -1096,15 +1151,15 @@
         "dataViewArn": str,
         "datasetId": str,
         "asOfTimestamp": int,
         "partitionColumns": List[str],
         "sortColumns": List[str],
         "status": DataViewStatusType,
         "errorInfo": DataViewErrorInfoTypeDef,
-        "destinationTypeProperties": DataViewDestinationTypeParamsTypeDef,
+        "destinationTypeProperties": DataViewDestinationTypeParamsOutputTypeDef,
         "autoUpdate": bool,
         "createTime": int,
         "lastModifiedTime": int,
     },
     total=False,
 )
 
@@ -1117,15 +1172,15 @@
         "asOfTimestamp": int,
         "errorInfo": DataViewErrorInfoTypeDef,
         "lastModifiedTime": int,
         "createTime": int,
         "sortColumns": List[str],
         "dataViewId": str,
         "dataViewArn": str,
-        "destinationTypeParams": DataViewDestinationTypeParamsTypeDef,
+        "destinationTypeParams": DataViewDestinationTypeParamsOutputTypeDef,
         "status": DataViewStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetExternalDataViewAccessDetailsResponseTypeDef = TypedDict(
     "GetExternalDataViewAccessDetailsResponseTypeDef",
@@ -1194,14 +1249,22 @@
     {
         "changesets": List[ChangesetSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+SchemaUnionOutputTypeDef = TypedDict(
+    "SchemaUnionOutputTypeDef",
+    {
+        "tabularSchemaConfig": SchemaDefinitionOutputTypeDef,
+    },
+    total=False,
+)
+
 SchemaUnionTypeDef = TypedDict(
     "SchemaUnionTypeDef",
     {
         "tabularSchemaConfig": SchemaDefinitionTypeDef,
     },
     total=False,
 )
@@ -1211,51 +1274,26 @@
     {
         "nextToken": str,
         "dataViews": List[DataViewSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetRequestRequestTypeDef",
-    {
-        "datasetTitle": str,
-        "kind": DatasetKindType,
-        "permissionGroupParams": PermissionGroupParamsTypeDef,
-    },
-)
-_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "datasetDescription": str,
-        "ownerInfo": DatasetOwnerInfoTypeDef,
-        "alias": str,
-        "schemaDefinition": SchemaUnionTypeDef,
-    },
-    total=False,
-)
-
-class CreateDatasetRequestRequestTypeDef(
-    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
-):
-    pass
-
 DatasetTypeDef = TypedDict(
     "DatasetTypeDef",
     {
         "datasetId": str,
         "datasetArn": str,
         "datasetTitle": str,
         "kind": DatasetKindType,
         "datasetDescription": str,
-        "ownerInfo": DatasetOwnerInfoTypeDef,
+        "ownerInfo": DatasetOwnerInfoOutputTypeDef,
         "createTime": int,
         "lastModifiedTime": int,
-        "schemaDefinition": SchemaUnionTypeDef,
+        "schemaDefinition": SchemaUnionOutputTypeDef,
         "alias": str,
     },
     total=False,
 )
 
 GetDatasetResponseTypeDef = TypedDict(
     "GetDatasetResponseTypeDef",
@@ -1263,21 +1301,46 @@
         "datasetId": str,
         "datasetArn": str,
         "datasetTitle": str,
         "kind": DatasetKindType,
         "datasetDescription": str,
         "createTime": int,
         "lastModifiedTime": int,
-        "schemaDefinition": SchemaUnionTypeDef,
+        "schemaDefinition": SchemaUnionOutputTypeDef,
         "alias": str,
         "status": DatasetStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetRequestRequestTypeDef",
+    {
+        "datasetTitle": str,
+        "kind": DatasetKindType,
+        "permissionGroupParams": PermissionGroupParamsTypeDef,
+    },
+)
+_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "datasetDescription": str,
+        "ownerInfo": DatasetOwnerInfoTypeDef,
+        "alias": str,
+        "schemaDefinition": SchemaUnionTypeDef,
+    },
+    total=False,
+)
+
+class CreateDatasetRequestRequestTypeDef(
+    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
+):
+    pass
+
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "datasetId": str,
         "datasetTitle": str,
         "kind": DatasetKindType,
     },
```

### Comparing `mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data.egg-info/PKG-INFO` & `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-finspace-data
-Version: 1.28.0
-Summary: Type annotations for boto3.FinSpaceData 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.FinSpaceData 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-finspace-data"></a>
 
 # mypy-boto3-finspace-data
 
 [![PyPI - mypy-boto3-finspace-data](https://img.shields.io/pypi/v/mypy-boto3-finspace-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-finspace-data?color=blue)](https://pypistats.org/packages/mypy-boto3-finspace-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-finspace-data)](https://pepy.tech/project/mypy-boto3-finspace-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FinSpaceData 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
+[boto3.FinSpaceData 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
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
 [mypy-boto3-finspace-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,27 +353,30 @@
 
 ```python
 from mypy_boto3_finspace_data.type_defs import (
     AssociateUserToPermissionGroupRequestRequestTypeDef,
     AssociateUserToPermissionGroupResponseTypeDef,
     AwsCredentialsTypeDef,
     ChangesetErrorInfoTypeDef,
+    ColumnDefinitionOutputTypeDef,
     ColumnDefinitionTypeDef,
     CreateChangesetRequestRequestTypeDef,
     CreateChangesetResponseTypeDef,
     DataViewDestinationTypeParamsTypeDef,
     CreateDataViewResponseTypeDef,
     DatasetOwnerInfoTypeDef,
     CreateDatasetResponseTypeDef,
     CreatePermissionGroupRequestRequestTypeDef,
     CreatePermissionGroupResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     CreateUserResponseTypeDef,
     CredentialsTypeDef,
+    DataViewDestinationTypeParamsOutputTypeDef,
     DataViewErrorInfoTypeDef,
+    DatasetOwnerInfoOutputTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteDatasetResponseTypeDef,
     DeletePermissionGroupRequestRequestTypeDef,
     DeletePermissionGroupResponseTypeDef,
     DisableUserRequestRequestTypeDef,
     DisableUserResponseTypeDef,
     DisassociateUserFromPermissionGroupRequestRequestTypeDef,
@@ -417,32 +420,34 @@
     UpdateDatasetResponseTypeDef,
     UpdatePermissionGroupRequestRequestTypeDef,
     UpdatePermissionGroupResponseTypeDef,
     UpdateUserRequestRequestTypeDef,
     UpdateUserResponseTypeDef,
     ChangesetSummaryTypeDef,
     GetChangesetResponseTypeDef,
+    SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
     CreateDataViewRequestRequestTypeDef,
     GetProgrammaticAccessCredentialsResponseTypeDef,
     DataViewSummaryTypeDef,
     GetDataViewResponseTypeDef,
     GetExternalDataViewAccessDetailsResponseTypeDef,
     GetPermissionGroupResponseTypeDef,
     ListPermissionGroupsResponseTypeDef,
     ListPermissionGroupsByUserResponseTypeDef,
     ListUsersByPermissionGroupResponseTypeDef,
     ListUsersResponseTypeDef,
     PermissionGroupParamsTypeDef,
     ListChangesetsResponseTypeDef,
+    SchemaUnionOutputTypeDef,
     SchemaUnionTypeDef,
     ListDataViewsResponseTypeDef,
-    CreateDatasetRequestRequestTypeDef,
     DatasetTypeDef,
     GetDatasetResponseTypeDef,
+    CreateDatasetRequestRequestTypeDef,
     UpdateDatasetRequestRequestTypeDef,
     ListDatasetsResponseTypeDef,
 )
 
 
 def get_structure() -> AssociateUserToPermissionGroupRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-finspace-data-1.28.0/mypy_boto3_finspace_data.egg-info/SOURCES.txt` & `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.0/setup.py` & `mypy-boto3-finspace-data-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-finspace-data",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_finspace_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FinSpaceData 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.FinSpaceData 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

