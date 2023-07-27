# Comparing `tmp/mypy-boto3-ssm-sap-1.28.0.tar.gz` & `tmp/mypy-boto3-ssm-sap-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ssm-sap-1.28.0.tar", last modified: Thu Jul  6 21:00:42 2023, max compression
+gzip compressed data, was "mypy-boto3-ssm-sap-1.28.12.tar", last modified: Thu Jul 27 11:49:43 2023, max compression
```

## Comparing `mypy-boto3-ssm-sap-1.28.0.tar` & `mypy-boto3-ssm-sap-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:42.958442 mypy-boto3-ssm-sap-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:56:40.000000 mypy-boto3-ssm-sap-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-07-06 21:00:42.954442 mypy-boto3-ssm-sap-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-07-06 20:56:40.000000 mypy-boto3-ssm-sap-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:42.950442 mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-06 20:56:40.000000 mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-06 20:56:40.000000 mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-06 20:56:40.000000 mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15057 2023-07-06 20:56:40.000000 mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-07-06 20:56:40.000000 mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-07-06 20:56:40.000000 mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-07-06 20:56:40.000000 mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-06 20:56:40.000000 mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-07-06 20:56:40.000000 mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:56:40.000000 mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15308 2023-07-06 20:56:41.000000 mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15295 2023-07-06 20:56:41.000000 mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:56:40.000000 mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:42.954442 mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-07-06 21:00:42.000000 mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-06 21:00:42.000000 mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:42.000000 mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:42.000000 mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:42.000000 mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 21:00:42.000000 mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:42.958442 mypy-boto3-ssm-sap-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-06 20:56:40.000000 mypy-boto3-ssm-sap-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:43.725340 mypy-boto3-ssm-sap-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15275 2023-07-27 11:49:43.725340 mypy-boto3-ssm-sap-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:43.705340 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-07-27 11:47:33.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17286 2023-07-27 11:47:35.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-07-27 11:47:33.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:43.725340 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15275 2023-07-27 11:49:43.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-27 11:49:43.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:43.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:43.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:43.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 11:49:43.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:43.725340 mypy-boto3-ssm-sap-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/setup.py
```

### Comparing `mypy-boto3-ssm-sap-1.28.0/LICENSE` & `mypy-boto3-ssm-sap-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-sap-1.28.0/PKG-INFO` & `mypy-boto3-ssm-sap-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-sap
-Version: 1.28.0
-Summary: Type annotations for boto3.SsmSap 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SsmSap 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ssm-sap"></a>
 
 # mypy-boto3-ssm-sap
 
 [![PyPI - mypy-boto3-ssm-sap](https://img.shields.io/pypi/v/mypy-boto3-ssm-sap.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-sap)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-sap.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-sap)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm-sap?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm-sap)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-sap)](https://pepy.tech/project/mypy-boto3-ssm-sap)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SsmSap 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
+[boto3.SsmSap 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
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
 [mypy-boto3-ssm-sap docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,101 +304,112 @@
 ### Literals
 
 `mypy_boto3_ssm_sap.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_ssm_sap.literals import (
+    ApplicationDiscoveryStatusType,
     ApplicationStatusType,
     ApplicationTypeType,
+    BackintModeType,
+    ClusterStatusType,
     ComponentStatusType,
     ComponentTypeType,
     CredentialTypeType,
     DatabaseStatusType,
     DatabaseTypeType,
     FilterOperatorType,
     HostRoleType,
     ListApplicationsPaginatorName,
     ListComponentsPaginatorName,
     ListDatabasesPaginatorName,
     ListOperationsPaginatorName,
+    OperationModeType,
     OperationStatusType,
     PermissionActionTypeType,
+    ReplicationModeType,
     SsmSapServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: ApplicationStatusType) -> bool:
+def check_value(value: ApplicationDiscoveryStatusType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_ssm_sap.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ssm_sap.type_defs import (
+    ApplicationCredentialOutputTypeDef,
     ApplicationCredentialTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationTypeDef,
+    AssociatedHostTypeDef,
+    BackintConfigTypeDef,
     ComponentSummaryTypeDef,
     HostTypeDef,
+    ResilienceTypeDef,
     DatabaseSummaryTypeDef,
     DeleteResourcePermissionInputRequestTypeDef,
-    DeleteResourcePermissionOutputTypeDef,
+    ResponseMetadataTypeDef,
     DeregisterApplicationInputRequestTypeDef,
     FilterTypeDef,
     GetApplicationInputRequestTypeDef,
     GetComponentInputRequestTypeDef,
     GetDatabaseInputRequestTypeDef,
     GetOperationInputRequestTypeDef,
     OperationTypeDef,
     GetResourcePermissionInputRequestTypeDef,
-    GetResourcePermissionOutputTypeDef,
-    ListApplicationsInputListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsInputRequestTypeDef,
-    ListComponentsInputListComponentsPaginateTypeDef,
     ListComponentsInputRequestTypeDef,
-    ListDatabasesInputListDatabasesPaginateTypeDef,
     ListDatabasesInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePermissionInputRequestTypeDef,
-    PutResourcePermissionOutputTypeDef,
-    ResponseMetadataTypeDef,
+    StartApplicationRefreshInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateApplicationSettingsOutputTypeDef,
     DatabaseTypeDef,
     RegisterApplicationInputRequestTypeDef,
     UpdateApplicationSettingsInputRequestTypeDef,
-    ListApplicationsOutputTypeDef,
+    ComponentTypeDef,
+    DeleteResourcePermissionOutputTypeDef,
     GetApplicationOutputTypeDef,
-    RegisterApplicationOutputTypeDef,
+    GetResourcePermissionOutputTypeDef,
+    ListApplicationsOutputTypeDef,
     ListComponentsOutputTypeDef,
-    ComponentTypeDef,
     ListDatabasesOutputTypeDef,
-    ListOperationsInputListOperationsPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutResourcePermissionOutputTypeDef,
+    RegisterApplicationOutputTypeDef,
+    StartApplicationRefreshOutputTypeDef,
+    UpdateApplicationSettingsOutputTypeDef,
     ListOperationsInputRequestTypeDef,
     GetOperationOutputTypeDef,
     ListOperationsOutputTypeDef,
+    ListApplicationsInputListApplicationsPaginateTypeDef,
+    ListComponentsInputListComponentsPaginateTypeDef,
+    ListDatabasesInputListDatabasesPaginateTypeDef,
+    ListOperationsInputListOperationsPaginateTypeDef,
     GetDatabaseOutputTypeDef,
     GetComponentOutputTypeDef,
 )
 
 
-def get_structure() -> ApplicationCredentialTypeDef:
+def get_structure() -> ApplicationCredentialOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ssm-sap-1.28.0/README.md` & `mypy-boto3-ssm-sap-1.28.12/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ssm-sap"></a>
 
 # mypy-boto3-ssm-sap
 
 [![PyPI - mypy-boto3-ssm-sap](https://img.shields.io/pypi/v/mypy-boto3-ssm-sap.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-sap)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-sap.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-sap)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm-sap?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm-sap)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-sap)](https://pepy.tech/project/mypy-boto3-ssm-sap)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SsmSap 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
+[boto3.SsmSap 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
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
 [mypy-boto3-ssm-sap docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/).
 
 See how it helps to find and fix potential bugs:
 
@@ -272,101 +272,112 @@
 ### Literals
 
 `mypy_boto3_ssm_sap.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_ssm_sap.literals import (
+    ApplicationDiscoveryStatusType,
     ApplicationStatusType,
     ApplicationTypeType,
+    BackintModeType,
+    ClusterStatusType,
     ComponentStatusType,
     ComponentTypeType,
     CredentialTypeType,
     DatabaseStatusType,
     DatabaseTypeType,
     FilterOperatorType,
     HostRoleType,
     ListApplicationsPaginatorName,
     ListComponentsPaginatorName,
     ListDatabasesPaginatorName,
     ListOperationsPaginatorName,
+    OperationModeType,
     OperationStatusType,
     PermissionActionTypeType,
+    ReplicationModeType,
     SsmSapServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: ApplicationStatusType) -> bool:
+def check_value(value: ApplicationDiscoveryStatusType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_ssm_sap.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ssm_sap.type_defs import (
+    ApplicationCredentialOutputTypeDef,
     ApplicationCredentialTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationTypeDef,
+    AssociatedHostTypeDef,
+    BackintConfigTypeDef,
     ComponentSummaryTypeDef,
     HostTypeDef,
+    ResilienceTypeDef,
     DatabaseSummaryTypeDef,
     DeleteResourcePermissionInputRequestTypeDef,
-    DeleteResourcePermissionOutputTypeDef,
+    ResponseMetadataTypeDef,
     DeregisterApplicationInputRequestTypeDef,
     FilterTypeDef,
     GetApplicationInputRequestTypeDef,
     GetComponentInputRequestTypeDef,
     GetDatabaseInputRequestTypeDef,
     GetOperationInputRequestTypeDef,
     OperationTypeDef,
     GetResourcePermissionInputRequestTypeDef,
-    GetResourcePermissionOutputTypeDef,
-    ListApplicationsInputListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsInputRequestTypeDef,
-    ListComponentsInputListComponentsPaginateTypeDef,
     ListComponentsInputRequestTypeDef,
-    ListDatabasesInputListDatabasesPaginateTypeDef,
     ListDatabasesInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePermissionInputRequestTypeDef,
-    PutResourcePermissionOutputTypeDef,
-    ResponseMetadataTypeDef,
+    StartApplicationRefreshInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateApplicationSettingsOutputTypeDef,
     DatabaseTypeDef,
     RegisterApplicationInputRequestTypeDef,
     UpdateApplicationSettingsInputRequestTypeDef,
-    ListApplicationsOutputTypeDef,
+    ComponentTypeDef,
+    DeleteResourcePermissionOutputTypeDef,
     GetApplicationOutputTypeDef,
-    RegisterApplicationOutputTypeDef,
+    GetResourcePermissionOutputTypeDef,
+    ListApplicationsOutputTypeDef,
     ListComponentsOutputTypeDef,
-    ComponentTypeDef,
     ListDatabasesOutputTypeDef,
-    ListOperationsInputListOperationsPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutResourcePermissionOutputTypeDef,
+    RegisterApplicationOutputTypeDef,
+    StartApplicationRefreshOutputTypeDef,
+    UpdateApplicationSettingsOutputTypeDef,
     ListOperationsInputRequestTypeDef,
     GetOperationOutputTypeDef,
     ListOperationsOutputTypeDef,
+    ListApplicationsInputListApplicationsPaginateTypeDef,
+    ListComponentsInputListComponentsPaginateTypeDef,
+    ListDatabasesInputListDatabasesPaginateTypeDef,
+    ListOperationsInputListOperationsPaginateTypeDef,
     GetDatabaseOutputTypeDef,
     GetComponentOutputTypeDef,
 )
 
 
-def get_structure() -> ApplicationCredentialTypeDef:
+def get_structure() -> ApplicationCredentialOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/__init__.py` & `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/__init__.pyi` & `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/__main__.py` & `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SsmSap 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.SsmSap 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap\nOther"
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

### Comparing `mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/client.py` & `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,28 +22,30 @@
     ListApplicationsPaginator,
     ListComponentsPaginator,
     ListDatabasesPaginator,
     ListOperationsPaginator,
 )
 from .type_defs import (
     ApplicationCredentialTypeDef,
+    BackintConfigTypeDef,
     DeleteResourcePermissionOutputTypeDef,
     FilterTypeDef,
     GetApplicationOutputTypeDef,
     GetComponentOutputTypeDef,
     GetDatabaseOutputTypeDef,
     GetOperationOutputTypeDef,
     GetResourcePermissionOutputTypeDef,
     ListApplicationsOutputTypeDef,
     ListComponentsOutputTypeDef,
     ListDatabasesOutputTypeDef,
     ListOperationsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutResourcePermissionOutputTypeDef,
     RegisterApplicationOutputTypeDef,
+    StartApplicationRefreshOutputTypeDef,
     UpdateApplicationSettingsOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -274,14 +276,24 @@
         """
         Register an SAP application with AWS Systems Manager for SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.register_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#register_application)
         """
 
+    def start_application_refresh(
+        self, *, ApplicationId: str
+    ) -> StartApplicationRefreshOutputTypeDef:
+        """
+        Refreshes a registered application.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.start_application_refresh)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#start_application_refresh)
+        """
+
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Creates tag for a resource by specifying the ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#tag_resource)
         """
@@ -295,15 +307,16 @@
         """
 
     def update_application_settings(
         self,
         *,
         ApplicationId: str,
         CredentialsToAddOrUpdate: Sequence[ApplicationCredentialTypeDef] = ...,
-        CredentialsToRemove: Sequence[ApplicationCredentialTypeDef] = ...
+        CredentialsToRemove: Sequence[ApplicationCredentialTypeDef] = ...,
+        Backint: BackintConfigTypeDef = ...
     ) -> UpdateApplicationSettingsOutputTypeDef:
         """
         Updates the settings of an application registered with AWS Systems Manager for
         SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.update_application_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#update_application_settings)
```

### Comparing `mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/client.pyi` & `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -22,28 +22,30 @@
     ListApplicationsPaginator,
     ListComponentsPaginator,
     ListDatabasesPaginator,
     ListOperationsPaginator,
 )
 from .type_defs import (
     ApplicationCredentialTypeDef,
+    BackintConfigTypeDef,
     DeleteResourcePermissionOutputTypeDef,
     FilterTypeDef,
     GetApplicationOutputTypeDef,
     GetComponentOutputTypeDef,
     GetDatabaseOutputTypeDef,
     GetOperationOutputTypeDef,
     GetResourcePermissionOutputTypeDef,
     ListApplicationsOutputTypeDef,
     ListComponentsOutputTypeDef,
     ListDatabasesOutputTypeDef,
     ListOperationsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutResourcePermissionOutputTypeDef,
     RegisterApplicationOutputTypeDef,
+    StartApplicationRefreshOutputTypeDef,
     UpdateApplicationSettingsOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -252,14 +254,23 @@
     ) -> RegisterApplicationOutputTypeDef:
         """
         Register an SAP application with AWS Systems Manager for SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.register_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#register_application)
         """
+    def start_application_refresh(
+        self, *, ApplicationId: str
+    ) -> StartApplicationRefreshOutputTypeDef:
+        """
+        Refreshes a registered application.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.start_application_refresh)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#start_application_refresh)
+        """
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Creates tag for a resource by specifying the ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#tag_resource)
         """
@@ -271,15 +282,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#untag_resource)
         """
     def update_application_settings(
         self,
         *,
         ApplicationId: str,
         CredentialsToAddOrUpdate: Sequence[ApplicationCredentialTypeDef] = ...,
-        CredentialsToRemove: Sequence[ApplicationCredentialTypeDef] = ...
+        CredentialsToRemove: Sequence[ApplicationCredentialTypeDef] = ...,
+        Backint: BackintConfigTypeDef = ...
     ) -> UpdateApplicationSettingsOutputTypeDef:
         """
         Updates the settings of an application registered with AWS Systems Manager for
         SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.update_application_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/client/#update_application_settings)
```

### Comparing `mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/literals.py` & `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,68 +2,84 @@
 Type annotations for ssm-sap service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_ssm_sap.literals import ApplicationStatusType
+    from mypy_boto3_ssm_sap.literals import ApplicationDiscoveryStatusType
 
-    data: ApplicationStatusType = "ACTIVATED"
+    data: ApplicationDiscoveryStatusType = "DELETING"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
+    "ApplicationDiscoveryStatusType",
     "ApplicationStatusType",
     "ApplicationTypeType",
+    "BackintModeType",
+    "ClusterStatusType",
     "ComponentStatusType",
     "ComponentTypeType",
     "CredentialTypeType",
     "DatabaseStatusType",
     "DatabaseTypeType",
     "FilterOperatorType",
     "HostRoleType",
     "ListApplicationsPaginatorName",
     "ListComponentsPaginatorName",
     "ListDatabasesPaginatorName",
     "ListOperationsPaginatorName",
+    "OperationModeType",
     "OperationStatusType",
     "PermissionActionTypeType",
+    "ReplicationModeType",
     "SsmSapServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 
+ApplicationDiscoveryStatusType = Literal[
+    "DELETING", "REFRESH_FAILED", "REGISTERING", "REGISTRATION_FAILED", "SUCCESS"
+]
 ApplicationStatusType = Literal[
     "ACTIVATED", "DELETING", "FAILED", "REGISTERING", "STARTING", "STOPPED", "STOPPING", "UNKNOWN"
 ]
 ApplicationTypeType = Literal["HANA"]
-ComponentStatusType = Literal["ACTIVATED"]
-ComponentTypeType = Literal["HANA"]
+BackintModeType = Literal["AWSBackup"]
+ClusterStatusType = Literal["MAINTENANCE", "NONE", "OFFLINE", "ONLINE", "STANDBY"]
+ComponentStatusType = Literal[
+    "ACTIVATED", "RUNNING", "RUNNING_WITH_ERROR", "STARTING", "STOPPED", "STOPPING", "UNDEFINED"
+]
+ComponentTypeType = Literal["HANA", "HANA_NODE"]
 CredentialTypeType = Literal["ADMIN"]
-DatabaseStatusType = Literal["RUNNING", "STARTING", "STOPPED", "UNKNOWN", "WARNING"]
+DatabaseStatusType = Literal["ERROR", "RUNNING", "STARTING", "STOPPED", "UNKNOWN", "WARNING"]
 DatabaseTypeType = Literal["SYSTEM", "TENANT"]
 FilterOperatorType = Literal["Equals", "GreaterThanOrEquals", "LessThanOrEquals"]
 HostRoleType = Literal["LEADER", "STANDBY", "UNKNOWN", "WORKER"]
 ListApplicationsPaginatorName = Literal["list_applications"]
 ListComponentsPaginatorName = Literal["list_components"]
 ListDatabasesPaginatorName = Literal["list_databases"]
 ListOperationsPaginatorName = Literal["list_operations"]
+OperationModeType = Literal[
+    "DELTA_DATASHIPPING", "LOGREPLAY", "LOGREPLAY_READACCESS", "NONE", "PRIMARY"
+]
 OperationStatusType = Literal["ERROR", "INPROGRESS", "SUCCESS"]
 PermissionActionTypeType = Literal["RESTORE"]
+ReplicationModeType = Literal["ASYNC", "NONE", "PRIMARY", "SYNC", "SYNCMEM"]
 SsmSapServiceName = Literal["ssm-sap"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -176,14 +192,15 @@
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
@@ -262,26 +279,28 @@
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

### Comparing `mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/literals.pyi` & `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -2,66 +2,82 @@
 Type annotations for ssm-sap service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_ssm_sap.literals import ApplicationStatusType
+    from mypy_boto3_ssm_sap.literals import ApplicationDiscoveryStatusType
 
-    data: ApplicationStatusType = "ACTIVATED"
+    data: ApplicationDiscoveryStatusType = "DELETING"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "ApplicationDiscoveryStatusType",
     "ApplicationStatusType",
     "ApplicationTypeType",
+    "BackintModeType",
+    "ClusterStatusType",
     "ComponentStatusType",
     "ComponentTypeType",
     "CredentialTypeType",
     "DatabaseStatusType",
     "DatabaseTypeType",
     "FilterOperatorType",
     "HostRoleType",
     "ListApplicationsPaginatorName",
     "ListComponentsPaginatorName",
     "ListDatabasesPaginatorName",
     "ListOperationsPaginatorName",
+    "OperationModeType",
     "OperationStatusType",
     "PermissionActionTypeType",
+    "ReplicationModeType",
     "SsmSapServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+ApplicationDiscoveryStatusType = Literal[
+    "DELETING", "REFRESH_FAILED", "REGISTERING", "REGISTRATION_FAILED", "SUCCESS"
+]
 ApplicationStatusType = Literal[
     "ACTIVATED", "DELETING", "FAILED", "REGISTERING", "STARTING", "STOPPED", "STOPPING", "UNKNOWN"
 ]
 ApplicationTypeType = Literal["HANA"]
-ComponentStatusType = Literal["ACTIVATED"]
-ComponentTypeType = Literal["HANA"]
+BackintModeType = Literal["AWSBackup"]
+ClusterStatusType = Literal["MAINTENANCE", "NONE", "OFFLINE", "ONLINE", "STANDBY"]
+ComponentStatusType = Literal[
+    "ACTIVATED", "RUNNING", "RUNNING_WITH_ERROR", "STARTING", "STOPPED", "STOPPING", "UNDEFINED"
+]
+ComponentTypeType = Literal["HANA", "HANA_NODE"]
 CredentialTypeType = Literal["ADMIN"]
-DatabaseStatusType = Literal["RUNNING", "STARTING", "STOPPED", "UNKNOWN", "WARNING"]
+DatabaseStatusType = Literal["ERROR", "RUNNING", "STARTING", "STOPPED", "UNKNOWN", "WARNING"]
 DatabaseTypeType = Literal["SYSTEM", "TENANT"]
 FilterOperatorType = Literal["Equals", "GreaterThanOrEquals", "LessThanOrEquals"]
 HostRoleType = Literal["LEADER", "STANDBY", "UNKNOWN", "WORKER"]
 ListApplicationsPaginatorName = Literal["list_applications"]
 ListComponentsPaginatorName = Literal["list_components"]
 ListDatabasesPaginatorName = Literal["list_databases"]
 ListOperationsPaginatorName = Literal["list_operations"]
+OperationModeType = Literal[
+    "DELTA_DATASHIPPING", "LOGREPLAY", "LOGREPLAY_READACCESS", "NONE", "PRIMARY"
+]
 OperationStatusType = Literal["ERROR", "INPROGRESS", "SUCCESS"]
 PermissionActionTypeType = Literal["RESTORE"]
+ReplicationModeType = Literal["ASYNC", "NONE", "PRIMARY", "SYNC", "SYNCMEM"]
 SsmSapServiceName = Literal["ssm-sap"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -174,14 +190,15 @@
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
@@ -260,26 +277,28 @@
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

### Comparing `mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/paginator.py` & `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,30 +59,30 @@
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listapplicationspaginator)
         """
 
 
 class ListComponentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListComponents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listcomponentspaginator)
     """
 
     def paginate(
-        self, *, ApplicationId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApplicationId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListComponentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listcomponentspaginator)
         """
 
 
@@ -93,15 +93,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str = ...,
         ComponentId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatabasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListDatabases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listdatabasespaginator)
         """
 
 
@@ -112,13 +112,13 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listoperationspaginator)
         """
```

### Comparing `mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/paginator.pyi` & `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -56,29 +56,29 @@
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listapplicationspaginator)
         """
 
 class ListComponentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListComponents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listcomponentspaginator)
     """
 
     def paginate(
-        self, *, ApplicationId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApplicationId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListComponentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listcomponentspaginator)
         """
 
 class ListDatabasesPaginator(Paginator):
@@ -88,15 +88,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str = ...,
         ComponentId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatabasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListDatabases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listdatabasespaginator)
         """
 
 class ListOperationsPaginator(Paginator):
@@ -106,13 +106,13 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/paginators/#listoperationspaginator)
         """
```

### Comparing `mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/type_defs.py` & `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,92 +2,113 @@
 Type annotations for ssm-sap service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_ssm_sap.type_defs import ApplicationCredentialTypeDef
+    from mypy_boto3_ssm_sap.type_defs import ApplicationCredentialOutputTypeDef
 
-    data: ApplicationCredentialTypeDef = {...}
+    data: ApplicationCredentialOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
+    ApplicationDiscoveryStatusType,
     ApplicationStatusType,
+    ClusterStatusType,
+    ComponentStatusType,
+    ComponentTypeType,
     DatabaseStatusType,
     DatabaseTypeType,
     FilterOperatorType,
     HostRoleType,
+    OperationModeType,
     OperationStatusType,
+    ReplicationModeType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "ApplicationCredentialOutputTypeDef",
     "ApplicationCredentialTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationTypeDef",
+    "AssociatedHostTypeDef",
+    "BackintConfigTypeDef",
     "ComponentSummaryTypeDef",
     "HostTypeDef",
+    "ResilienceTypeDef",
     "DatabaseSummaryTypeDef",
     "DeleteResourcePermissionInputRequestTypeDef",
-    "DeleteResourcePermissionOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DeregisterApplicationInputRequestTypeDef",
     "FilterTypeDef",
     "GetApplicationInputRequestTypeDef",
     "GetComponentInputRequestTypeDef",
     "GetDatabaseInputRequestTypeDef",
     "GetOperationInputRequestTypeDef",
     "OperationTypeDef",
     "GetResourcePermissionInputRequestTypeDef",
-    "GetResourcePermissionOutputTypeDef",
-    "ListApplicationsInputListApplicationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationsInputRequestTypeDef",
-    "ListComponentsInputListComponentsPaginateTypeDef",
     "ListComponentsInputRequestTypeDef",
-    "ListDatabasesInputListDatabasesPaginateTypeDef",
     "ListDatabasesInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PutResourcePermissionInputRequestTypeDef",
-    "PutResourcePermissionOutputTypeDef",
-    "ResponseMetadataTypeDef",
+    "StartApplicationRefreshInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateApplicationSettingsOutputTypeDef",
     "DatabaseTypeDef",
     "RegisterApplicationInputRequestTypeDef",
     "UpdateApplicationSettingsInputRequestTypeDef",
-    "ListApplicationsOutputTypeDef",
+    "ComponentTypeDef",
+    "DeleteResourcePermissionOutputTypeDef",
     "GetApplicationOutputTypeDef",
-    "RegisterApplicationOutputTypeDef",
+    "GetResourcePermissionOutputTypeDef",
+    "ListApplicationsOutputTypeDef",
     "ListComponentsOutputTypeDef",
-    "ComponentTypeDef",
     "ListDatabasesOutputTypeDef",
-    "ListOperationsInputListOperationsPaginateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutResourcePermissionOutputTypeDef",
+    "RegisterApplicationOutputTypeDef",
+    "StartApplicationRefreshOutputTypeDef",
+    "UpdateApplicationSettingsOutputTypeDef",
     "ListOperationsInputRequestTypeDef",
     "GetOperationOutputTypeDef",
     "ListOperationsOutputTypeDef",
+    "ListApplicationsInputListApplicationsPaginateTypeDef",
+    "ListComponentsInputListComponentsPaginateTypeDef",
+    "ListDatabasesInputListDatabasesPaginateTypeDef",
+    "ListOperationsInputListOperationsPaginateTypeDef",
     "GetDatabaseOutputTypeDef",
     "GetComponentOutputTypeDef",
 )
 
+ApplicationCredentialOutputTypeDef = TypedDict(
+    "ApplicationCredentialOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "CredentialType": Literal["ADMIN"],
+        "SecretId": str,
+    },
+)
+
 ApplicationCredentialTypeDef = TypedDict(
     "ApplicationCredentialTypeDef",
     {
         "DatabaseName": str,
         "CredentialType": Literal["ADMIN"],
         "SecretId": str,
     },
@@ -108,39 +129,72 @@
     "ApplicationTypeDef",
     {
         "Id": str,
         "Type": Literal["HANA"],
         "Arn": str,
         "AppRegistryArn": str,
         "Status": ApplicationStatusType,
+        "DiscoveryStatus": ApplicationDiscoveryStatusType,
         "Components": List[str],
         "LastUpdated": datetime,
         "StatusMessage": str,
     },
     total=False,
 )
 
+AssociatedHostTypeDef = TypedDict(
+    "AssociatedHostTypeDef",
+    {
+        "Hostname": str,
+        "Ec2InstanceId": str,
+        "OsVersion": str,
+    },
+    total=False,
+)
+
+BackintConfigTypeDef = TypedDict(
+    "BackintConfigTypeDef",
+    {
+        "BackintMode": Literal["AWSBackup"],
+        "EnsureNoBackupInProcess": bool,
+    },
+)
+
 ComponentSummaryTypeDef = TypedDict(
     "ComponentSummaryTypeDef",
     {
         "ApplicationId": str,
         "ComponentId": str,
-        "ComponentType": Literal["HANA"],
+        "ComponentType": ComponentTypeType,
         "Tags": Dict[str, str],
+        "Arn": str,
     },
     total=False,
 )
 
 HostTypeDef = TypedDict(
     "HostTypeDef",
     {
         "HostName": str,
-        "HostRole": HostRoleType,
         "HostIp": str,
+        "EC2InstanceId": str,
         "InstanceId": str,
+        "HostRole": HostRoleType,
+        "OsVersion": str,
+    },
+    total=False,
+)
+
+ResilienceTypeDef = TypedDict(
+    "ResilienceTypeDef",
+    {
+        "HsrTier": str,
+        "HsrReplicationMode": ReplicationModeType,
+        "HsrOperationMode": OperationModeType,
+        "ClusterStatus": ClusterStatusType,
     },
     total=False,
 )
 
 DatabaseSummaryTypeDef = TypedDict(
     "DatabaseSummaryTypeDef",
     {
@@ -173,19 +227,22 @@
 class DeleteResourcePermissionInputRequestTypeDef(
     _RequiredDeleteResourcePermissionInputRequestTypeDef,
     _OptionalDeleteResourcePermissionInputRequestTypeDef,
 ):
     pass
 
 
-DeleteResourcePermissionOutputTypeDef = TypedDict(
-    "DeleteResourcePermissionOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeregisterApplicationInputRequestTypeDef = TypedDict(
     "DeregisterApplicationInputRequestTypeDef",
     {
         "ApplicationId": str,
@@ -273,68 +330,43 @@
 class GetResourcePermissionInputRequestTypeDef(
     _RequiredGetResourcePermissionInputRequestTypeDef,
     _OptionalGetResourcePermissionInputRequestTypeDef,
 ):
     pass
 
 
-GetResourcePermissionOutputTypeDef = TypedDict(
-    "GetResourcePermissionOutputTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsInputListApplicationsPaginateTypeDef",
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
 
 ListApplicationsInputRequestTypeDef = TypedDict(
     "ListApplicationsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListComponentsInputListComponentsPaginateTypeDef = TypedDict(
-    "ListComponentsInputListComponentsPaginateTypeDef",
-    {
-        "ApplicationId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListComponentsInputRequestTypeDef = TypedDict(
     "ListComponentsInputRequestTypeDef",
     {
         "ApplicationId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
-    "ListDatabasesInputListDatabasesPaginateTypeDef",
-    {
-        "ApplicationId": str,
-        "ComponentId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDatabasesInputRequestTypeDef = TypedDict(
     "ListDatabasesInputRequestTypeDef",
     {
         "ApplicationId": str,
         "ComponentId": str,
         "NextToken": str,
         "MaxResults": int,
@@ -345,57 +377,27 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
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
 PutResourcePermissionInputRequestTypeDef = TypedDict(
     "PutResourcePermissionInputRequestTypeDef",
     {
         "ActionType": Literal["RESTORE"],
         "SourceResourceArn": str,
         "ResourceArn": str,
     },
 )
 
-PutResourcePermissionOutputTypeDef = TypedDict(
-    "PutResourcePermissionOutputTypeDef",
+StartApplicationRefreshInputRequestTypeDef = TypedDict(
+    "StartApplicationRefreshInputRequestTypeDef",
     {
-        "Policy": str,
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
+        "ApplicationId": str,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -407,29 +409,20 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateApplicationSettingsOutputTypeDef = TypedDict(
-    "UpdateApplicationSettingsOutputTypeDef",
-    {
-        "Message": str,
-        "OperationIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DatabaseTypeDef = TypedDict(
     "DatabaseTypeDef",
     {
         "ApplicationId": str,
         "ComponentId": str,
-        "Credentials": List[ApplicationCredentialTypeDef],
+        "Credentials": List[ApplicationCredentialOutputTypeDef],
         "DatabaseId": str,
         "DatabaseName": str,
         "DatabaseType": DatabaseTypeType,
         "Arn": str,
         "Status": DatabaseStatusType,
         "PrimaryHost": str,
         "SQLPort": int,
@@ -471,108 +464,143 @@
     },
 )
 _OptionalUpdateApplicationSettingsInputRequestTypeDef = TypedDict(
     "_OptionalUpdateApplicationSettingsInputRequestTypeDef",
     {
         "CredentialsToAddOrUpdate": Sequence[ApplicationCredentialTypeDef],
         "CredentialsToRemove": Sequence[ApplicationCredentialTypeDef],
+        "Backint": BackintConfigTypeDef,
     },
     total=False,
 )
 
 
 class UpdateApplicationSettingsInputRequestTypeDef(
     _RequiredUpdateApplicationSettingsInputRequestTypeDef,
     _OptionalUpdateApplicationSettingsInputRequestTypeDef,
 ):
     pass
 
 
-ListApplicationsOutputTypeDef = TypedDict(
-    "ListApplicationsOutputTypeDef",
+ComponentTypeDef = TypedDict(
+    "ComponentTypeDef",
     {
-        "Applications": List[ApplicationSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ComponentId": str,
+        "ParentComponent": str,
+        "ChildComponents": List[str],
+        "ApplicationId": str,
+        "ComponentType": ComponentTypeType,
+        "Status": ComponentStatusType,
+        "SapHostname": str,
+        "SapKernelVersion": str,
+        "HdbVersion": str,
+        "Resilience": ResilienceTypeDef,
+        "AssociatedHost": AssociatedHostTypeDef,
+        "Databases": List[str],
+        "Hosts": List[HostTypeDef],
+        "PrimaryHost": str,
+        "LastUpdated": datetime,
+        "Arn": str,
+    },
+    total=False,
+)
+
+DeleteResourcePermissionOutputTypeDef = TypedDict(
+    "DeleteResourcePermissionOutputTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApplicationOutputTypeDef = TypedDict(
     "GetApplicationOutputTypeDef",
     {
         "Application": ApplicationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RegisterApplicationOutputTypeDef = TypedDict(
-    "RegisterApplicationOutputTypeDef",
+GetResourcePermissionOutputTypeDef = TypedDict(
+    "GetResourcePermissionOutputTypeDef",
     {
-        "Application": ApplicationTypeDef,
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListComponentsOutputTypeDef = TypedDict(
-    "ListComponentsOutputTypeDef",
+ListApplicationsOutputTypeDef = TypedDict(
+    "ListApplicationsOutputTypeDef",
     {
-        "Components": List[ComponentSummaryTypeDef],
+        "Applications": List[ApplicationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ComponentTypeDef = TypedDict(
-    "ComponentTypeDef",
+ListComponentsOutputTypeDef = TypedDict(
+    "ListComponentsOutputTypeDef",
     {
-        "ComponentId": str,
-        "ApplicationId": str,
-        "ComponentType": Literal["HANA"],
-        "Status": Literal["ACTIVATED"],
-        "Databases": List[str],
-        "Hosts": List[HostTypeDef],
-        "PrimaryHost": str,
-        "LastUpdated": datetime,
+        "Components": List[ComponentSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ListDatabasesOutputTypeDef = TypedDict(
     "ListDatabasesOutputTypeDef",
     {
         "Databases": List[DatabaseSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListOperationsInputListOperationsPaginateTypeDef = TypedDict(
-    "_RequiredListOperationsInputListOperationsPaginateTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ApplicationId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalListOperationsInputListOperationsPaginateTypeDef = TypedDict(
-    "_OptionalListOperationsInputListOperationsPaginateTypeDef",
+
+PutResourcePermissionOutputTypeDef = TypedDict(
+    "PutResourcePermissionOutputTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+RegisterApplicationOutputTypeDef = TypedDict(
+    "RegisterApplicationOutputTypeDef",
+    {
+        "Application": ApplicationTypeDef,
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ListOperationsInputListOperationsPaginateTypeDef(
-    _RequiredListOperationsInputListOperationsPaginateTypeDef,
-    _OptionalListOperationsInputListOperationsPaginateTypeDef,
-):
-    pass
+StartApplicationRefreshOutputTypeDef = TypedDict(
+    "StartApplicationRefreshOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+UpdateApplicationSettingsOutputTypeDef = TypedDict(
+    "UpdateApplicationSettingsOutputTypeDef",
+    {
+        "Message": str,
+        "OperationIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredListOperationsInputRequestTypeDef = TypedDict(
     "_RequiredListOperationsInputRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
@@ -593,36 +621,87 @@
     pass
 
 
 GetOperationOutputTypeDef = TypedDict(
     "GetOperationOutputTypeDef",
     {
         "Operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOperationsOutputTypeDef = TypedDict(
     "ListOperationsOutputTypeDef",
     {
         "Operations": List[OperationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsInputListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListComponentsInputListComponentsPaginateTypeDef = TypedDict(
+    "ListComponentsInputListComponentsPaginateTypeDef",
+    {
+        "ApplicationId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+ListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
+    "ListDatabasesInputListDatabasesPaginateTypeDef",
+    {
+        "ApplicationId": str,
+        "ComponentId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListOperationsInputListOperationsPaginateTypeDef = TypedDict(
+    "_RequiredListOperationsInputListOperationsPaginateTypeDef",
+    {
+        "ApplicationId": str,
+    },
+)
+_OptionalListOperationsInputListOperationsPaginateTypeDef = TypedDict(
+    "_OptionalListOperationsInputListOperationsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListOperationsInputListOperationsPaginateTypeDef(
+    _RequiredListOperationsInputListOperationsPaginateTypeDef,
+    _OptionalListOperationsInputListOperationsPaginateTypeDef,
+):
+    pass
+
+
 GetDatabaseOutputTypeDef = TypedDict(
     "GetDatabaseOutputTypeDef",
     {
         "Database": DatabaseTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetComponentOutputTypeDef = TypedDict(
     "GetComponentOutputTypeDef",
     {
         "Component": ComponentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap/type_defs.pyi` & `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -2,91 +2,112 @@
 Type annotations for ssm-sap service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_ssm_sap.type_defs import ApplicationCredentialTypeDef
+    from mypy_boto3_ssm_sap.type_defs import ApplicationCredentialOutputTypeDef
 
-    data: ApplicationCredentialTypeDef = {...}
+    data: ApplicationCredentialOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
+    ApplicationDiscoveryStatusType,
     ApplicationStatusType,
+    ClusterStatusType,
+    ComponentStatusType,
+    ComponentTypeType,
     DatabaseStatusType,
     DatabaseTypeType,
     FilterOperatorType,
     HostRoleType,
+    OperationModeType,
     OperationStatusType,
+    ReplicationModeType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "ApplicationCredentialOutputTypeDef",
     "ApplicationCredentialTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationTypeDef",
+    "AssociatedHostTypeDef",
+    "BackintConfigTypeDef",
     "ComponentSummaryTypeDef",
     "HostTypeDef",
+    "ResilienceTypeDef",
     "DatabaseSummaryTypeDef",
     "DeleteResourcePermissionInputRequestTypeDef",
-    "DeleteResourcePermissionOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DeregisterApplicationInputRequestTypeDef",
     "FilterTypeDef",
     "GetApplicationInputRequestTypeDef",
     "GetComponentInputRequestTypeDef",
     "GetDatabaseInputRequestTypeDef",
     "GetOperationInputRequestTypeDef",
     "OperationTypeDef",
     "GetResourcePermissionInputRequestTypeDef",
-    "GetResourcePermissionOutputTypeDef",
-    "ListApplicationsInputListApplicationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationsInputRequestTypeDef",
-    "ListComponentsInputListComponentsPaginateTypeDef",
     "ListComponentsInputRequestTypeDef",
-    "ListDatabasesInputListDatabasesPaginateTypeDef",
     "ListDatabasesInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PutResourcePermissionInputRequestTypeDef",
-    "PutResourcePermissionOutputTypeDef",
-    "ResponseMetadataTypeDef",
+    "StartApplicationRefreshInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateApplicationSettingsOutputTypeDef",
     "DatabaseTypeDef",
     "RegisterApplicationInputRequestTypeDef",
     "UpdateApplicationSettingsInputRequestTypeDef",
-    "ListApplicationsOutputTypeDef",
+    "ComponentTypeDef",
+    "DeleteResourcePermissionOutputTypeDef",
     "GetApplicationOutputTypeDef",
-    "RegisterApplicationOutputTypeDef",
+    "GetResourcePermissionOutputTypeDef",
+    "ListApplicationsOutputTypeDef",
     "ListComponentsOutputTypeDef",
-    "ComponentTypeDef",
     "ListDatabasesOutputTypeDef",
-    "ListOperationsInputListOperationsPaginateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutResourcePermissionOutputTypeDef",
+    "RegisterApplicationOutputTypeDef",
+    "StartApplicationRefreshOutputTypeDef",
+    "UpdateApplicationSettingsOutputTypeDef",
     "ListOperationsInputRequestTypeDef",
     "GetOperationOutputTypeDef",
     "ListOperationsOutputTypeDef",
+    "ListApplicationsInputListApplicationsPaginateTypeDef",
+    "ListComponentsInputListComponentsPaginateTypeDef",
+    "ListDatabasesInputListDatabasesPaginateTypeDef",
+    "ListOperationsInputListOperationsPaginateTypeDef",
     "GetDatabaseOutputTypeDef",
     "GetComponentOutputTypeDef",
 )
 
+ApplicationCredentialOutputTypeDef = TypedDict(
+    "ApplicationCredentialOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "CredentialType": Literal["ADMIN"],
+        "SecretId": str,
+    },
+)
+
 ApplicationCredentialTypeDef = TypedDict(
     "ApplicationCredentialTypeDef",
     {
         "DatabaseName": str,
         "CredentialType": Literal["ADMIN"],
         "SecretId": str,
     },
@@ -107,39 +128,72 @@
     "ApplicationTypeDef",
     {
         "Id": str,
         "Type": Literal["HANA"],
         "Arn": str,
         "AppRegistryArn": str,
         "Status": ApplicationStatusType,
+        "DiscoveryStatus": ApplicationDiscoveryStatusType,
         "Components": List[str],
         "LastUpdated": datetime,
         "StatusMessage": str,
     },
     total=False,
 )
 
+AssociatedHostTypeDef = TypedDict(
+    "AssociatedHostTypeDef",
+    {
+        "Hostname": str,
+        "Ec2InstanceId": str,
+        "OsVersion": str,
+    },
+    total=False,
+)
+
+BackintConfigTypeDef = TypedDict(
+    "BackintConfigTypeDef",
+    {
+        "BackintMode": Literal["AWSBackup"],
+        "EnsureNoBackupInProcess": bool,
+    },
+)
+
 ComponentSummaryTypeDef = TypedDict(
     "ComponentSummaryTypeDef",
     {
         "ApplicationId": str,
         "ComponentId": str,
-        "ComponentType": Literal["HANA"],
+        "ComponentType": ComponentTypeType,
         "Tags": Dict[str, str],
+        "Arn": str,
     },
     total=False,
 )
 
 HostTypeDef = TypedDict(
     "HostTypeDef",
     {
         "HostName": str,
-        "HostRole": HostRoleType,
         "HostIp": str,
+        "EC2InstanceId": str,
         "InstanceId": str,
+        "HostRole": HostRoleType,
+        "OsVersion": str,
+    },
+    total=False,
+)
+
+ResilienceTypeDef = TypedDict(
+    "ResilienceTypeDef",
+    {
+        "HsrTier": str,
+        "HsrReplicationMode": ReplicationModeType,
+        "HsrOperationMode": OperationModeType,
+        "ClusterStatus": ClusterStatusType,
     },
     total=False,
 )
 
 DatabaseSummaryTypeDef = TypedDict(
     "DatabaseSummaryTypeDef",
     {
@@ -170,19 +224,22 @@
 
 class DeleteResourcePermissionInputRequestTypeDef(
     _RequiredDeleteResourcePermissionInputRequestTypeDef,
     _OptionalDeleteResourcePermissionInputRequestTypeDef,
 ):
     pass
 
-DeleteResourcePermissionOutputTypeDef = TypedDict(
-    "DeleteResourcePermissionOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeregisterApplicationInputRequestTypeDef = TypedDict(
     "DeregisterApplicationInputRequestTypeDef",
     {
         "ApplicationId": str,
@@ -268,68 +325,43 @@
 
 class GetResourcePermissionInputRequestTypeDef(
     _RequiredGetResourcePermissionInputRequestTypeDef,
     _OptionalGetResourcePermissionInputRequestTypeDef,
 ):
     pass
 
-GetResourcePermissionOutputTypeDef = TypedDict(
-    "GetResourcePermissionOutputTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsInputListApplicationsPaginateTypeDef",
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
 
 ListApplicationsInputRequestTypeDef = TypedDict(
     "ListApplicationsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListComponentsInputListComponentsPaginateTypeDef = TypedDict(
-    "ListComponentsInputListComponentsPaginateTypeDef",
-    {
-        "ApplicationId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListComponentsInputRequestTypeDef = TypedDict(
     "ListComponentsInputRequestTypeDef",
     {
         "ApplicationId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
-    "ListDatabasesInputListDatabasesPaginateTypeDef",
-    {
-        "ApplicationId": str,
-        "ComponentId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDatabasesInputRequestTypeDef = TypedDict(
     "ListDatabasesInputRequestTypeDef",
     {
         "ApplicationId": str,
         "ComponentId": str,
         "NextToken": str,
         "MaxResults": int,
@@ -340,57 +372,27 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
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
 PutResourcePermissionInputRequestTypeDef = TypedDict(
     "PutResourcePermissionInputRequestTypeDef",
     {
         "ActionType": Literal["RESTORE"],
         "SourceResourceArn": str,
         "ResourceArn": str,
     },
 )
 
-PutResourcePermissionOutputTypeDef = TypedDict(
-    "PutResourcePermissionOutputTypeDef",
+StartApplicationRefreshInputRequestTypeDef = TypedDict(
+    "StartApplicationRefreshInputRequestTypeDef",
     {
-        "Policy": str,
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
+        "ApplicationId": str,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -402,29 +404,20 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateApplicationSettingsOutputTypeDef = TypedDict(
-    "UpdateApplicationSettingsOutputTypeDef",
-    {
-        "Message": str,
-        "OperationIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DatabaseTypeDef = TypedDict(
     "DatabaseTypeDef",
     {
         "ApplicationId": str,
         "ComponentId": str,
-        "Credentials": List[ApplicationCredentialTypeDef],
+        "Credentials": List[ApplicationCredentialOutputTypeDef],
         "DatabaseId": str,
         "DatabaseName": str,
         "DatabaseType": DatabaseTypeType,
         "Arn": str,
         "Status": DatabaseStatusType,
         "PrimaryHost": str,
         "SQLPort": int,
@@ -464,104 +457,141 @@
     },
 )
 _OptionalUpdateApplicationSettingsInputRequestTypeDef = TypedDict(
     "_OptionalUpdateApplicationSettingsInputRequestTypeDef",
     {
         "CredentialsToAddOrUpdate": Sequence[ApplicationCredentialTypeDef],
         "CredentialsToRemove": Sequence[ApplicationCredentialTypeDef],
+        "Backint": BackintConfigTypeDef,
     },
     total=False,
 )
 
 class UpdateApplicationSettingsInputRequestTypeDef(
     _RequiredUpdateApplicationSettingsInputRequestTypeDef,
     _OptionalUpdateApplicationSettingsInputRequestTypeDef,
 ):
     pass
 
-ListApplicationsOutputTypeDef = TypedDict(
-    "ListApplicationsOutputTypeDef",
+ComponentTypeDef = TypedDict(
+    "ComponentTypeDef",
     {
-        "Applications": List[ApplicationSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ComponentId": str,
+        "ParentComponent": str,
+        "ChildComponents": List[str],
+        "ApplicationId": str,
+        "ComponentType": ComponentTypeType,
+        "Status": ComponentStatusType,
+        "SapHostname": str,
+        "SapKernelVersion": str,
+        "HdbVersion": str,
+        "Resilience": ResilienceTypeDef,
+        "AssociatedHost": AssociatedHostTypeDef,
+        "Databases": List[str],
+        "Hosts": List[HostTypeDef],
+        "PrimaryHost": str,
+        "LastUpdated": datetime,
+        "Arn": str,
+    },
+    total=False,
+)
+
+DeleteResourcePermissionOutputTypeDef = TypedDict(
+    "DeleteResourcePermissionOutputTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApplicationOutputTypeDef = TypedDict(
     "GetApplicationOutputTypeDef",
     {
         "Application": ApplicationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RegisterApplicationOutputTypeDef = TypedDict(
-    "RegisterApplicationOutputTypeDef",
+GetResourcePermissionOutputTypeDef = TypedDict(
+    "GetResourcePermissionOutputTypeDef",
     {
-        "Application": ApplicationTypeDef,
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListComponentsOutputTypeDef = TypedDict(
-    "ListComponentsOutputTypeDef",
+ListApplicationsOutputTypeDef = TypedDict(
+    "ListApplicationsOutputTypeDef",
     {
-        "Components": List[ComponentSummaryTypeDef],
+        "Applications": List[ApplicationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ComponentTypeDef = TypedDict(
-    "ComponentTypeDef",
+ListComponentsOutputTypeDef = TypedDict(
+    "ListComponentsOutputTypeDef",
     {
-        "ComponentId": str,
-        "ApplicationId": str,
-        "ComponentType": Literal["HANA"],
-        "Status": Literal["ACTIVATED"],
-        "Databases": List[str],
-        "Hosts": List[HostTypeDef],
-        "PrimaryHost": str,
-        "LastUpdated": datetime,
+        "Components": List[ComponentSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ListDatabasesOutputTypeDef = TypedDict(
     "ListDatabasesOutputTypeDef",
     {
         "Databases": List[DatabaseSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListOperationsInputListOperationsPaginateTypeDef = TypedDict(
-    "_RequiredListOperationsInputListOperationsPaginateTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ApplicationId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalListOperationsInputListOperationsPaginateTypeDef = TypedDict(
-    "_OptionalListOperationsInputListOperationsPaginateTypeDef",
+
+PutResourcePermissionOutputTypeDef = TypedDict(
+    "PutResourcePermissionOutputTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ListOperationsInputListOperationsPaginateTypeDef(
-    _RequiredListOperationsInputListOperationsPaginateTypeDef,
-    _OptionalListOperationsInputListOperationsPaginateTypeDef,
-):
-    pass
+RegisterApplicationOutputTypeDef = TypedDict(
+    "RegisterApplicationOutputTypeDef",
+    {
+        "Application": ApplicationTypeDef,
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartApplicationRefreshOutputTypeDef = TypedDict(
+    "StartApplicationRefreshOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApplicationSettingsOutputTypeDef = TypedDict(
+    "UpdateApplicationSettingsOutputTypeDef",
+    {
+        "Message": str,
+        "OperationIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredListOperationsInputRequestTypeDef = TypedDict(
     "_RequiredListOperationsInputRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
@@ -580,36 +610,85 @@
 ):
     pass
 
 GetOperationOutputTypeDef = TypedDict(
     "GetOperationOutputTypeDef",
     {
         "Operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOperationsOutputTypeDef = TypedDict(
     "ListOperationsOutputTypeDef",
     {
         "Operations": List[OperationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsInputListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListComponentsInputListComponentsPaginateTypeDef = TypedDict(
+    "ListComponentsInputListComponentsPaginateTypeDef",
+    {
+        "ApplicationId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+ListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
+    "ListDatabasesInputListDatabasesPaginateTypeDef",
+    {
+        "ApplicationId": str,
+        "ComponentId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListOperationsInputListOperationsPaginateTypeDef = TypedDict(
+    "_RequiredListOperationsInputListOperationsPaginateTypeDef",
+    {
+        "ApplicationId": str,
+    },
+)
+_OptionalListOperationsInputListOperationsPaginateTypeDef = TypedDict(
+    "_OptionalListOperationsInputListOperationsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListOperationsInputListOperationsPaginateTypeDef(
+    _RequiredListOperationsInputListOperationsPaginateTypeDef,
+    _OptionalListOperationsInputListOperationsPaginateTypeDef,
+):
+    pass
+
 GetDatabaseOutputTypeDef = TypedDict(
     "GetDatabaseOutputTypeDef",
     {
         "Database": DatabaseTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetComponentOutputTypeDef = TypedDict(
     "GetComponentOutputTypeDef",
     {
         "Component": ComponentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap.egg-info/PKG-INFO` & `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-sap
-Version: 1.28.0
-Summary: Type annotations for boto3.SsmSap 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SsmSap 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ssm-sap"></a>
 
 # mypy-boto3-ssm-sap
 
 [![PyPI - mypy-boto3-ssm-sap](https://img.shields.io/pypi/v/mypy-boto3-ssm-sap.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-sap)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-sap.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-sap)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm-sap?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm-sap)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-sap)](https://pepy.tech/project/mypy-boto3-ssm-sap)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SsmSap 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
+[boto3.SsmSap 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
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
 [mypy-boto3-ssm-sap docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,101 +304,112 @@
 ### Literals
 
 `mypy_boto3_ssm_sap.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_ssm_sap.literals import (
+    ApplicationDiscoveryStatusType,
     ApplicationStatusType,
     ApplicationTypeType,
+    BackintModeType,
+    ClusterStatusType,
     ComponentStatusType,
     ComponentTypeType,
     CredentialTypeType,
     DatabaseStatusType,
     DatabaseTypeType,
     FilterOperatorType,
     HostRoleType,
     ListApplicationsPaginatorName,
     ListComponentsPaginatorName,
     ListDatabasesPaginatorName,
     ListOperationsPaginatorName,
+    OperationModeType,
     OperationStatusType,
     PermissionActionTypeType,
+    ReplicationModeType,
     SsmSapServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: ApplicationStatusType) -> bool:
+def check_value(value: ApplicationDiscoveryStatusType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_ssm_sap.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ssm_sap.type_defs import (
+    ApplicationCredentialOutputTypeDef,
     ApplicationCredentialTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationTypeDef,
+    AssociatedHostTypeDef,
+    BackintConfigTypeDef,
     ComponentSummaryTypeDef,
     HostTypeDef,
+    ResilienceTypeDef,
     DatabaseSummaryTypeDef,
     DeleteResourcePermissionInputRequestTypeDef,
-    DeleteResourcePermissionOutputTypeDef,
+    ResponseMetadataTypeDef,
     DeregisterApplicationInputRequestTypeDef,
     FilterTypeDef,
     GetApplicationInputRequestTypeDef,
     GetComponentInputRequestTypeDef,
     GetDatabaseInputRequestTypeDef,
     GetOperationInputRequestTypeDef,
     OperationTypeDef,
     GetResourcePermissionInputRequestTypeDef,
-    GetResourcePermissionOutputTypeDef,
-    ListApplicationsInputListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsInputRequestTypeDef,
-    ListComponentsInputListComponentsPaginateTypeDef,
     ListComponentsInputRequestTypeDef,
-    ListDatabasesInputListDatabasesPaginateTypeDef,
     ListDatabasesInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePermissionInputRequestTypeDef,
-    PutResourcePermissionOutputTypeDef,
-    ResponseMetadataTypeDef,
+    StartApplicationRefreshInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateApplicationSettingsOutputTypeDef,
     DatabaseTypeDef,
     RegisterApplicationInputRequestTypeDef,
     UpdateApplicationSettingsInputRequestTypeDef,
-    ListApplicationsOutputTypeDef,
+    ComponentTypeDef,
+    DeleteResourcePermissionOutputTypeDef,
     GetApplicationOutputTypeDef,
-    RegisterApplicationOutputTypeDef,
+    GetResourcePermissionOutputTypeDef,
+    ListApplicationsOutputTypeDef,
     ListComponentsOutputTypeDef,
-    ComponentTypeDef,
     ListDatabasesOutputTypeDef,
-    ListOperationsInputListOperationsPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutResourcePermissionOutputTypeDef,
+    RegisterApplicationOutputTypeDef,
+    StartApplicationRefreshOutputTypeDef,
+    UpdateApplicationSettingsOutputTypeDef,
     ListOperationsInputRequestTypeDef,
     GetOperationOutputTypeDef,
     ListOperationsOutputTypeDef,
+    ListApplicationsInputListApplicationsPaginateTypeDef,
+    ListComponentsInputListComponentsPaginateTypeDef,
+    ListDatabasesInputListDatabasesPaginateTypeDef,
+    ListOperationsInputListOperationsPaginateTypeDef,
     GetDatabaseOutputTypeDef,
     GetComponentOutputTypeDef,
 )
 
 
-def get_structure() -> ApplicationCredentialTypeDef:
+def get_structure() -> ApplicationCredentialOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ssm-sap-1.28.0/mypy_boto3_ssm_sap.egg-info/SOURCES.txt` & `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-sap-1.28.0/setup.py` & `mypy-boto3-ssm-sap-1.28.12/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ssm-sap",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_ssm_sap"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SsmSap 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SsmSap 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

