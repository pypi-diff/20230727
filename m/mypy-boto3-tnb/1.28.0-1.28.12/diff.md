# Comparing `tmp/mypy-boto3-tnb-1.28.0.tar.gz` & `tmp/mypy-boto3-tnb-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-tnb-1.28.0.tar", last modified: Thu Jul  6 21:00:47 2023, max compression
+gzip compressed data, was "mypy-boto3-tnb-1.28.12.tar", last modified: Thu Jul 27 11:49:46 2023, max compression
```

## Comparing `mypy-boto3-tnb-1.28.0.tar` & `mypy-boto3-tnb-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:47.714452 mypy-boto3-tnb-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:57:15.000000 mypy-boto3-tnb-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-07-06 21:00:47.714452 mypy-boto3-tnb-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-07-06 20:57:15.000000 mypy-boto3-tnb-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:47.702452 mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-06 20:57:15.000000 mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-06 20:57:15.000000 mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-06 20:57:15.000000 mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25341 2023-07-06 20:57:15.000000 mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25296 2023-07-06 20:57:15.000000 mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-07-06 20:57:16.000000 mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-07-06 20:57:16.000000 mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-07-06 20:57:15.000000 mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-07-06 20:57:15.000000 mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:57:15.000000 mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34750 2023-07-06 20:57:17.000000 mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34719 2023-07-06 20:57:16.000000 mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:57:15.000000 mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:47.714452 mypy-boto3-tnb-1.28.0/mypy_boto3_tnb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-07-06 21:00:47.000000 mypy-boto3-tnb-1.28.0/mypy_boto3_tnb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 21:00:47.000000 mypy-boto3-tnb-1.28.0/mypy_boto3_tnb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:47.000000 mypy-boto3-tnb-1.28.0/mypy_boto3_tnb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:47.000000 mypy-boto3-tnb-1.28.0/mypy_boto3_tnb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:47.000000 mypy-boto3-tnb-1.28.0/mypy_boto3_tnb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 21:00:47.000000 mypy-boto3-tnb-1.28.0/mypy_boto3_tnb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:47.714452 mypy-boto3-tnb-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-06 20:57:15.000000 mypy-boto3-tnb-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.745445 mypy-boto3-tnb-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:02.000000 mypy-boto3-tnb-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18190 2023-07-27 11:49:46.745445 mypy-boto3-tnb-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-07-27 11:48:02.000000 mypy-boto3-tnb-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.725444 mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-27 11:48:02.000000 mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-27 11:48:02.000000 mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-27 11:48:02.000000 mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25341 2023-07-27 11:48:02.000000 mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25296 2023-07-27 11:48:02.000000 mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-07-27 11:48:03.000000 mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-07-27 11:48:03.000000 mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-07-27 11:48:02.000000 mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-27 11:48:02.000000 mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:02.000000 mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34684 2023-07-27 11:48:03.000000 mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34653 2023-07-27 11:48:03.000000 mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:02.000000 mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.745445 mypy-boto3-tnb-1.28.12/mypy_boto3_tnb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18190 2023-07-27 11:49:46.000000 mypy-boto3-tnb-1.28.12/mypy_boto3_tnb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 11:49:46.000000 mypy-boto3-tnb-1.28.12/mypy_boto3_tnb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-tnb-1.28.12/mypy_boto3_tnb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-tnb-1.28.12/mypy_boto3_tnb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:46.000000 mypy-boto3-tnb-1.28.12/mypy_boto3_tnb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:46.000000 mypy-boto3-tnb-1.28.12/mypy_boto3_tnb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:46.745445 mypy-boto3-tnb-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-27 11:48:02.000000 mypy-boto3-tnb-1.28.12/setup.py
```

### Comparing `mypy-boto3-tnb-1.28.0/LICENSE` & `mypy-boto3-tnb-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-tnb-1.28.0/PKG-INFO` & `mypy-boto3-tnb-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-tnb
-Version: 1.28.0
-Summary: Type annotations for boto3.TelcoNetworkBuilder 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.TelcoNetworkBuilder 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-tnb"></a>
 
 # mypy-boto3-tnb
 
 [![PyPI - mypy-boto3-tnb](https://img.shields.io/pypi/v/mypy-boto3-tnb.svg?color=blue)](https://pypi.org/project/mypy-boto3-tnb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-tnb.svg?color=blue)](https://pypi.org/project/mypy-boto3-tnb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-tnb?color=blue)](https://pypistats.org/packages/mypy-boto3-tnb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-tnb)](https://pepy.tech/project/mypy-boto3-tnb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TelcoNetworkBuilder 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
+[boto3.TelcoNetworkBuilder 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
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
 [mypy-boto3-tnb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,86 +357,86 @@
 `mypy_boto3_tnb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_tnb.type_defs import (
     CancelSolNetworkOperationInputRequestTypeDef,
     CreateSolFunctionPackageInputRequestTypeDef,
-    CreateSolFunctionPackageOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateSolNetworkInstanceInputRequestTypeDef,
-    CreateSolNetworkInstanceOutputTypeDef,
     CreateSolNetworkPackageInputRequestTypeDef,
-    CreateSolNetworkPackageOutputTypeDef,
     DeleteSolFunctionPackageInputRequestTypeDef,
     DeleteSolNetworkInstanceInputRequestTypeDef,
     DeleteSolNetworkPackageInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ErrorInfoTypeDef,
     ToscaOverrideTypeDef,
     GetSolFunctionInstanceInputRequestTypeDef,
     GetSolFunctionInstanceMetadataTypeDef,
     GetSolFunctionPackageContentInputRequestTypeDef,
-    GetSolFunctionPackageContentOutputTypeDef,
     GetSolFunctionPackageDescriptorInputRequestTypeDef,
-    GetSolFunctionPackageDescriptorOutputTypeDef,
     GetSolFunctionPackageInputRequestTypeDef,
     GetSolInstantiatedVnfInfoTypeDef,
     GetSolNetworkInstanceInputRequestTypeDef,
     GetSolNetworkInstanceMetadataTypeDef,
     LcmOperationInfoTypeDef,
     GetSolNetworkOperationInputRequestTypeDef,
     GetSolNetworkOperationMetadataTypeDef,
     ProblemDetailsTypeDef,
     GetSolNetworkPackageContentInputRequestTypeDef,
-    GetSolNetworkPackageContentOutputTypeDef,
     GetSolNetworkPackageDescriptorInputRequestTypeDef,
-    GetSolNetworkPackageDescriptorOutputTypeDef,
     GetSolNetworkPackageInputRequestTypeDef,
     GetSolVnfcResourceInfoMetadataTypeDef,
     InstantiateSolNetworkInstanceInputRequestTypeDef,
-    InstantiateSolNetworkInstanceOutputTypeDef,
     ListSolFunctionInstanceMetadataTypeDef,
-    ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListSolFunctionInstancesInputRequestTypeDef,
     ListSolFunctionPackageMetadataTypeDef,
-    ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef,
     ListSolFunctionPackagesInputRequestTypeDef,
     ListSolNetworkInstanceMetadataTypeDef,
-    ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef,
     ListSolNetworkInstancesInputRequestTypeDef,
     ListSolNetworkOperationsMetadataTypeDef,
-    ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef,
     ListSolNetworkOperationsInputRequestTypeDef,
     ListSolNetworkPackageMetadataTypeDef,
-    ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef,
     ListSolNetworkPackagesInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PaginatorConfigTypeDef,
     PutSolFunctionPackageContentInputRequestTypeDef,
     PutSolNetworkPackageContentInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     TerminateSolNetworkInstanceInputRequestTypeDef,
-    TerminateSolNetworkInstanceOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateSolFunctionPackageInputRequestTypeDef,
-    UpdateSolFunctionPackageOutputTypeDef,
     UpdateSolNetworkModifyTypeDef,
-    UpdateSolNetworkInstanceOutputTypeDef,
     UpdateSolNetworkPackageInputRequestTypeDef,
-    UpdateSolNetworkPackageOutputTypeDef,
     ValidateSolFunctionPackageContentInputRequestTypeDef,
     ValidateSolNetworkPackageContentInputRequestTypeDef,
+    CreateSolFunctionPackageOutputTypeDef,
+    CreateSolNetworkInstanceOutputTypeDef,
+    CreateSolNetworkPackageOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetSolFunctionPackageContentOutputTypeDef,
+    GetSolFunctionPackageDescriptorOutputTypeDef,
+    GetSolNetworkPackageContentOutputTypeDef,
+    GetSolNetworkPackageDescriptorOutputTypeDef,
+    InstantiateSolNetworkInstanceOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    TerminateSolNetworkInstanceOutputTypeDef,
+    UpdateSolFunctionPackageOutputTypeDef,
+    UpdateSolNetworkInstanceOutputTypeDef,
+    UpdateSolNetworkPackageOutputTypeDef,
     GetSolNetworkOperationTaskDetailsTypeDef,
     FunctionArtifactMetaTypeDef,
     NetworkArtifactMetaTypeDef,
     GetSolNetworkInstanceOutputTypeDef,
     GetSolVnfcResourceInfoTypeDef,
     ListSolFunctionInstanceInfoTypeDef,
+    ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef,
+    ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef,
+    ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef,
+    ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef,
+    ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef,
     ListSolFunctionPackageInfoTypeDef,
     ListSolNetworkInstanceInfoTypeDef,
     ListSolNetworkOperationsInfoTypeDef,
     ListSolNetworkPackageInfoTypeDef,
     UpdateSolNetworkInstanceInputRequestTypeDef,
     GetSolNetworkOperationOutputTypeDef,
     GetSolFunctionPackageMetadataTypeDef,
```

### Comparing `mypy-boto3-tnb-1.28.0/README.md` & `mypy-boto3-tnb-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-tnb"></a>
 
 # mypy-boto3-tnb
 
 [![PyPI - mypy-boto3-tnb](https://img.shields.io/pypi/v/mypy-boto3-tnb.svg?color=blue)](https://pypi.org/project/mypy-boto3-tnb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-tnb.svg?color=blue)](https://pypi.org/project/mypy-boto3-tnb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-tnb?color=blue)](https://pypistats.org/packages/mypy-boto3-tnb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-tnb)](https://pepy.tech/project/mypy-boto3-tnb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TelcoNetworkBuilder 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
+[boto3.TelcoNetworkBuilder 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
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
 [mypy-boto3-tnb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,86 +325,86 @@
 `mypy_boto3_tnb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_tnb.type_defs import (
     CancelSolNetworkOperationInputRequestTypeDef,
     CreateSolFunctionPackageInputRequestTypeDef,
-    CreateSolFunctionPackageOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateSolNetworkInstanceInputRequestTypeDef,
-    CreateSolNetworkInstanceOutputTypeDef,
     CreateSolNetworkPackageInputRequestTypeDef,
-    CreateSolNetworkPackageOutputTypeDef,
     DeleteSolFunctionPackageInputRequestTypeDef,
     DeleteSolNetworkInstanceInputRequestTypeDef,
     DeleteSolNetworkPackageInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ErrorInfoTypeDef,
     ToscaOverrideTypeDef,
     GetSolFunctionInstanceInputRequestTypeDef,
     GetSolFunctionInstanceMetadataTypeDef,
     GetSolFunctionPackageContentInputRequestTypeDef,
-    GetSolFunctionPackageContentOutputTypeDef,
     GetSolFunctionPackageDescriptorInputRequestTypeDef,
-    GetSolFunctionPackageDescriptorOutputTypeDef,
     GetSolFunctionPackageInputRequestTypeDef,
     GetSolInstantiatedVnfInfoTypeDef,
     GetSolNetworkInstanceInputRequestTypeDef,
     GetSolNetworkInstanceMetadataTypeDef,
     LcmOperationInfoTypeDef,
     GetSolNetworkOperationInputRequestTypeDef,
     GetSolNetworkOperationMetadataTypeDef,
     ProblemDetailsTypeDef,
     GetSolNetworkPackageContentInputRequestTypeDef,
-    GetSolNetworkPackageContentOutputTypeDef,
     GetSolNetworkPackageDescriptorInputRequestTypeDef,
-    GetSolNetworkPackageDescriptorOutputTypeDef,
     GetSolNetworkPackageInputRequestTypeDef,
     GetSolVnfcResourceInfoMetadataTypeDef,
     InstantiateSolNetworkInstanceInputRequestTypeDef,
-    InstantiateSolNetworkInstanceOutputTypeDef,
     ListSolFunctionInstanceMetadataTypeDef,
-    ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListSolFunctionInstancesInputRequestTypeDef,
     ListSolFunctionPackageMetadataTypeDef,
-    ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef,
     ListSolFunctionPackagesInputRequestTypeDef,
     ListSolNetworkInstanceMetadataTypeDef,
-    ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef,
     ListSolNetworkInstancesInputRequestTypeDef,
     ListSolNetworkOperationsMetadataTypeDef,
-    ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef,
     ListSolNetworkOperationsInputRequestTypeDef,
     ListSolNetworkPackageMetadataTypeDef,
-    ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef,
     ListSolNetworkPackagesInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PaginatorConfigTypeDef,
     PutSolFunctionPackageContentInputRequestTypeDef,
     PutSolNetworkPackageContentInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     TerminateSolNetworkInstanceInputRequestTypeDef,
-    TerminateSolNetworkInstanceOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateSolFunctionPackageInputRequestTypeDef,
-    UpdateSolFunctionPackageOutputTypeDef,
     UpdateSolNetworkModifyTypeDef,
-    UpdateSolNetworkInstanceOutputTypeDef,
     UpdateSolNetworkPackageInputRequestTypeDef,
-    UpdateSolNetworkPackageOutputTypeDef,
     ValidateSolFunctionPackageContentInputRequestTypeDef,
     ValidateSolNetworkPackageContentInputRequestTypeDef,
+    CreateSolFunctionPackageOutputTypeDef,
+    CreateSolNetworkInstanceOutputTypeDef,
+    CreateSolNetworkPackageOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetSolFunctionPackageContentOutputTypeDef,
+    GetSolFunctionPackageDescriptorOutputTypeDef,
+    GetSolNetworkPackageContentOutputTypeDef,
+    GetSolNetworkPackageDescriptorOutputTypeDef,
+    InstantiateSolNetworkInstanceOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    TerminateSolNetworkInstanceOutputTypeDef,
+    UpdateSolFunctionPackageOutputTypeDef,
+    UpdateSolNetworkInstanceOutputTypeDef,
+    UpdateSolNetworkPackageOutputTypeDef,
     GetSolNetworkOperationTaskDetailsTypeDef,
     FunctionArtifactMetaTypeDef,
     NetworkArtifactMetaTypeDef,
     GetSolNetworkInstanceOutputTypeDef,
     GetSolVnfcResourceInfoTypeDef,
     ListSolFunctionInstanceInfoTypeDef,
+    ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef,
+    ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef,
+    ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef,
+    ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef,
+    ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef,
     ListSolFunctionPackageInfoTypeDef,
     ListSolNetworkInstanceInfoTypeDef,
     ListSolNetworkOperationsInfoTypeDef,
     ListSolNetworkPackageInfoTypeDef,
     UpdateSolNetworkInstanceInputRequestTypeDef,
     GetSolNetworkOperationOutputTypeDef,
     GetSolFunctionPackageMetadataTypeDef,
```

### Comparing `mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/__init__.py` & `mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/__init__.pyi` & `mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/__main__.py` & `mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.TelcoNetworkBuilder 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.TelcoNetworkBuilder 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder\nOther"
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

### Comparing `mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/client.py` & `mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/client.pyi` & `mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/literals.py` & `mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/literals.py`

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

### Comparing `mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/literals.pyi` & `mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/literals.pyi`

 * *Files 2% similar despite different names*

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

### Comparing `mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/paginator.py` & `mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/paginator.py`

 * *Files 13% similar despite different names*

```diff
@@ -62,73 +62,73 @@
 class ListSolFunctionInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolfunctioninstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSolFunctionInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolfunctioninstancespaginator)
         """
 
 
 class ListSolFunctionPackagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionPackages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolfunctionpackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSolFunctionPackagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionPackages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolfunctionpackagespaginator)
         """
 
 
 class ListSolNetworkInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSolNetworkInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkinstancespaginator)
         """
 
 
 class ListSolNetworkOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkoperationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSolNetworkOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkoperationspaginator)
         """
 
 
 class ListSolNetworkPackagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkPackages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkpackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSolNetworkPackagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkPackages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkpackagespaginator)
         """
```

### Comparing `mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/paginator.pyi` & `mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -59,69 +59,69 @@
 class ListSolFunctionInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolfunctioninstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSolFunctionInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolfunctioninstancespaginator)
         """
 
 class ListSolFunctionPackagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionPackages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolfunctionpackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSolFunctionPackagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionPackages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolfunctionpackagespaginator)
         """
 
 class ListSolNetworkInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSolNetworkInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkinstancespaginator)
         """
 
 class ListSolNetworkOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkoperationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSolNetworkOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkoperationspaginator)
         """
 
 class ListSolNetworkPackagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkPackages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkpackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSolNetworkPackagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkPackages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/paginators/#listsolnetworkpackagespaginator)
         """
```

### Comparing `mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/type_defs.py` & `mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,86 +41,86 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CancelSolNetworkOperationInputRequestTypeDef",
     "CreateSolFunctionPackageInputRequestTypeDef",
-    "CreateSolFunctionPackageOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateSolNetworkInstanceInputRequestTypeDef",
-    "CreateSolNetworkInstanceOutputTypeDef",
     "CreateSolNetworkPackageInputRequestTypeDef",
-    "CreateSolNetworkPackageOutputTypeDef",
     "DeleteSolFunctionPackageInputRequestTypeDef",
     "DeleteSolNetworkInstanceInputRequestTypeDef",
     "DeleteSolNetworkPackageInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ErrorInfoTypeDef",
     "ToscaOverrideTypeDef",
     "GetSolFunctionInstanceInputRequestTypeDef",
     "GetSolFunctionInstanceMetadataTypeDef",
     "GetSolFunctionPackageContentInputRequestTypeDef",
-    "GetSolFunctionPackageContentOutputTypeDef",
     "GetSolFunctionPackageDescriptorInputRequestTypeDef",
-    "GetSolFunctionPackageDescriptorOutputTypeDef",
     "GetSolFunctionPackageInputRequestTypeDef",
     "GetSolInstantiatedVnfInfoTypeDef",
     "GetSolNetworkInstanceInputRequestTypeDef",
     "GetSolNetworkInstanceMetadataTypeDef",
     "LcmOperationInfoTypeDef",
     "GetSolNetworkOperationInputRequestTypeDef",
     "GetSolNetworkOperationMetadataTypeDef",
     "ProblemDetailsTypeDef",
     "GetSolNetworkPackageContentInputRequestTypeDef",
-    "GetSolNetworkPackageContentOutputTypeDef",
     "GetSolNetworkPackageDescriptorInputRequestTypeDef",
-    "GetSolNetworkPackageDescriptorOutputTypeDef",
     "GetSolNetworkPackageInputRequestTypeDef",
     "GetSolVnfcResourceInfoMetadataTypeDef",
     "InstantiateSolNetworkInstanceInputRequestTypeDef",
-    "InstantiateSolNetworkInstanceOutputTypeDef",
     "ListSolFunctionInstanceMetadataTypeDef",
-    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListSolFunctionInstancesInputRequestTypeDef",
     "ListSolFunctionPackageMetadataTypeDef",
-    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
     "ListSolFunctionPackagesInputRequestTypeDef",
     "ListSolNetworkInstanceMetadataTypeDef",
-    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
     "ListSolNetworkInstancesInputRequestTypeDef",
     "ListSolNetworkOperationsMetadataTypeDef",
-    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
     "ListSolNetworkOperationsInputRequestTypeDef",
     "ListSolNetworkPackageMetadataTypeDef",
-    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
     "ListSolNetworkPackagesInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "PutSolFunctionPackageContentInputRequestTypeDef",
     "PutSolNetworkPackageContentInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "TerminateSolNetworkInstanceInputRequestTypeDef",
-    "TerminateSolNetworkInstanceOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateSolFunctionPackageInputRequestTypeDef",
-    "UpdateSolFunctionPackageOutputTypeDef",
     "UpdateSolNetworkModifyTypeDef",
-    "UpdateSolNetworkInstanceOutputTypeDef",
     "UpdateSolNetworkPackageInputRequestTypeDef",
-    "UpdateSolNetworkPackageOutputTypeDef",
     "ValidateSolFunctionPackageContentInputRequestTypeDef",
     "ValidateSolNetworkPackageContentInputRequestTypeDef",
+    "CreateSolFunctionPackageOutputTypeDef",
+    "CreateSolNetworkInstanceOutputTypeDef",
+    "CreateSolNetworkPackageOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetSolFunctionPackageContentOutputTypeDef",
+    "GetSolFunctionPackageDescriptorOutputTypeDef",
+    "GetSolNetworkPackageContentOutputTypeDef",
+    "GetSolNetworkPackageDescriptorOutputTypeDef",
+    "InstantiateSolNetworkInstanceOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "TerminateSolNetworkInstanceOutputTypeDef",
+    "UpdateSolFunctionPackageOutputTypeDef",
+    "UpdateSolNetworkInstanceOutputTypeDef",
+    "UpdateSolNetworkPackageOutputTypeDef",
     "GetSolNetworkOperationTaskDetailsTypeDef",
     "FunctionArtifactMetaTypeDef",
     "NetworkArtifactMetaTypeDef",
     "GetSolNetworkInstanceOutputTypeDef",
     "GetSolVnfcResourceInfoTypeDef",
     "ListSolFunctionInstanceInfoTypeDef",
+    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
+    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
+    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
+    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
+    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
     "ListSolFunctionPackageInfoTypeDef",
     "ListSolNetworkInstanceInfoTypeDef",
     "ListSolNetworkOperationsInfoTypeDef",
     "ListSolNetworkPackageInfoTypeDef",
     "UpdateSolNetworkInstanceInputRequestTypeDef",
     "GetSolNetworkOperationOutputTypeDef",
     "GetSolFunctionPackageMetadataTypeDef",
@@ -155,24 +155,22 @@
     "CreateSolFunctionPackageInputRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-CreateSolFunctionPackageOutputTypeDef = TypedDict(
-    "CreateSolFunctionPackageOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "arn": str,
-        "id": str,
-        "onboardingState": OnboardingStateType,
-        "operationalState": OperationalStateType,
-        "tags": Dict[str, str],
-        "usageState": UsageStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateSolNetworkInstanceInputRequestTypeDef = TypedDict(
     "_RequiredCreateSolNetworkInstanceInputRequestTypeDef",
     {
         "nsName": str,
@@ -192,47 +190,22 @@
 class CreateSolNetworkInstanceInputRequestTypeDef(
     _RequiredCreateSolNetworkInstanceInputRequestTypeDef,
     _OptionalCreateSolNetworkInstanceInputRequestTypeDef,
 ):
     pass
 
 
-CreateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "CreateSolNetworkInstanceOutputTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "nsInstanceName": str,
-        "nsdInfoId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateSolNetworkPackageInputRequestTypeDef = TypedDict(
     "CreateSolNetworkPackageInputRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-CreateSolNetworkPackageOutputTypeDef = TypedDict(
-    "CreateSolNetworkPackageOutputTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "nsdOnboardingState": NsdOnboardingStateType,
-        "nsdOperationalState": NsdOperationalStateType,
-        "nsdUsageState": NsdUsageStateType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSolFunctionPackageInputRequestTypeDef = TypedDict(
     "DeleteSolFunctionPackageInputRequestTypeDef",
     {
         "vnfPkgId": str,
     },
 )
 
@@ -246,21 +219,14 @@
 DeleteSolNetworkPackageInputRequestTypeDef = TypedDict(
     "DeleteSolNetworkPackageInputRequestTypeDef",
     {
         "nsdInfoId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ErrorInfoTypeDef = TypedDict(
     "ErrorInfoTypeDef",
     {
         "cause": str,
         "details": str,
     },
     total=False,
@@ -294,40 +260,22 @@
     "GetSolFunctionPackageContentInputRequestTypeDef",
     {
         "accept": Literal["application/zip"],
         "vnfPkgId": str,
     },
 )
 
-GetSolFunctionPackageContentOutputTypeDef = TypedDict(
-    "GetSolFunctionPackageContentOutputTypeDef",
-    {
-        "contentType": Literal["application/zip"],
-        "packageContent": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSolFunctionPackageDescriptorInputRequestTypeDef = TypedDict(
     "GetSolFunctionPackageDescriptorInputRequestTypeDef",
     {
         "accept": Literal["text/plain"],
         "vnfPkgId": str,
     },
 )
 
-GetSolFunctionPackageDescriptorOutputTypeDef = TypedDict(
-    "GetSolFunctionPackageDescriptorOutputTypeDef",
-    {
-        "contentType": Literal["text/plain"],
-        "vnfd": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSolFunctionPackageInputRequestTypeDef = TypedDict(
     "GetSolFunctionPackageInputRequestTypeDef",
     {
         "vnfPkgId": str,
     },
 )
 
@@ -399,39 +347,21 @@
     "GetSolNetworkPackageContentInputRequestTypeDef",
     {
         "accept": Literal["application/zip"],
         "nsdInfoId": str,
     },
 )
 
-GetSolNetworkPackageContentOutputTypeDef = TypedDict(
-    "GetSolNetworkPackageContentOutputTypeDef",
-    {
-        "contentType": Literal["application/zip"],
-        "nsdContent": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSolNetworkPackageDescriptorInputRequestTypeDef = TypedDict(
     "GetSolNetworkPackageDescriptorInputRequestTypeDef",
     {
         "nsdInfoId": str,
     },
 )
 
-GetSolNetworkPackageDescriptorOutputTypeDef = TypedDict(
-    "GetSolNetworkPackageDescriptorOutputTypeDef",
-    {
-        "contentType": Literal["text/plain"],
-        "nsd": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSolNetworkPackageInputRequestTypeDef = TypedDict(
     "GetSolNetworkPackageInputRequestTypeDef",
     {
         "nsdInfoId": str,
     },
 )
 
@@ -465,35 +395,28 @@
 class InstantiateSolNetworkInstanceInputRequestTypeDef(
     _RequiredInstantiateSolNetworkInstanceInputRequestTypeDef,
     _OptionalInstantiateSolNetworkInstanceInputRequestTypeDef,
 ):
     pass
 
 
-InstantiateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "InstantiateSolNetworkInstanceOutputTypeDef",
-    {
-        "nsLcmOpOccId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListSolFunctionInstanceMetadataTypeDef = TypedDict(
     "ListSolFunctionInstanceMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef = TypedDict(
-    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
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
 
 ListSolFunctionInstancesInputRequestTypeDef = TypedDict(
     "ListSolFunctionInstancesInputRequestTypeDef",
     {
@@ -507,22 +430,14 @@
     "ListSolFunctionPackageMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef = TypedDict(
-    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSolFunctionPackagesInputRequestTypeDef = TypedDict(
     "ListSolFunctionPackagesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -532,22 +447,14 @@
     "ListSolNetworkInstanceMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef = TypedDict(
-    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSolNetworkInstancesInputRequestTypeDef = TypedDict(
     "ListSolNetworkInstancesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -557,22 +464,14 @@
     "ListSolNetworkOperationsMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef = TypedDict(
-    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSolNetworkOperationsInputRequestTypeDef = TypedDict(
     "ListSolNetworkOperationsInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -582,22 +481,14 @@
     "ListSolNetworkPackageMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef = TypedDict(
-    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSolNetworkPackagesInputRequestTypeDef = TypedDict(
     "ListSolNetworkPackagesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -606,32 +497,14 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
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
 _RequiredPutSolFunctionPackageContentInputRequestTypeDef = TypedDict(
     "_RequiredPutSolFunctionPackageContentInputRequestTypeDef",
     {
         "file": Union[str, bytes, IO[Any], StreamingBody],
         "vnfPkgId": str,
     },
 )
@@ -670,25 +543,14 @@
 class PutSolNetworkPackageContentInputRequestTypeDef(
     _RequiredPutSolNetworkPackageContentInputRequestTypeDef,
     _OptionalPutSolNetworkPackageContentInputRequestTypeDef,
 ):
     pass
 
 
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
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -711,23 +573,14 @@
 class TerminateSolNetworkInstanceInputRequestTypeDef(
     _RequiredTerminateSolNetworkInstanceInputRequestTypeDef,
     _OptionalTerminateSolNetworkInstanceInputRequestTypeDef,
 ):
     pass
 
 
-TerminateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "TerminateSolNetworkInstanceOutputTypeDef",
-    {
-        "nsLcmOpOccId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -736,55 +589,30 @@
     "UpdateSolFunctionPackageInputRequestTypeDef",
     {
         "operationalState": OperationalStateType,
         "vnfPkgId": str,
     },
 )
 
-UpdateSolFunctionPackageOutputTypeDef = TypedDict(
-    "UpdateSolFunctionPackageOutputTypeDef",
-    {
-        "operationalState": OperationalStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSolNetworkModifyTypeDef = TypedDict(
     "UpdateSolNetworkModifyTypeDef",
     {
         "vnfConfigurableProperties": Mapping[str, Any],
         "vnfInstanceId": str,
     },
 )
 
-UpdateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "UpdateSolNetworkInstanceOutputTypeDef",
-    {
-        "nsLcmOpOccId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSolNetworkPackageInputRequestTypeDef = TypedDict(
     "UpdateSolNetworkPackageInputRequestTypeDef",
     {
         "nsdInfoId": str,
         "nsdOperationalState": NsdOperationalStateType,
     },
 )
 
-UpdateSolNetworkPackageOutputTypeDef = TypedDict(
-    "UpdateSolNetworkPackageOutputTypeDef",
-    {
-        "nsdOperationalState": NsdOperationalStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredValidateSolFunctionPackageContentInputRequestTypeDef = TypedDict(
     "_RequiredValidateSolFunctionPackageContentInputRequestTypeDef",
     {
         "file": Union[str, bytes, IO[Any], StreamingBody],
         "vnfPkgId": str,
     },
 )
@@ -823,14 +651,146 @@
 class ValidateSolNetworkPackageContentInputRequestTypeDef(
     _RequiredValidateSolNetworkPackageContentInputRequestTypeDef,
     _OptionalValidateSolNetworkPackageContentInputRequestTypeDef,
 ):
     pass
 
 
+CreateSolFunctionPackageOutputTypeDef = TypedDict(
+    "CreateSolFunctionPackageOutputTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "onboardingState": OnboardingStateType,
+        "operationalState": OperationalStateType,
+        "tags": Dict[str, str],
+        "usageState": UsageStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "CreateSolNetworkInstanceOutputTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "nsInstanceName": str,
+        "nsdInfoId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSolNetworkPackageOutputTypeDef = TypedDict(
+    "CreateSolNetworkPackageOutputTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "nsdOnboardingState": NsdOnboardingStateType,
+        "nsdOperationalState": NsdOperationalStateType,
+        "nsdUsageState": NsdUsageStateType,
+        "tags": Dict[str, str],
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
+GetSolFunctionPackageContentOutputTypeDef = TypedDict(
+    "GetSolFunctionPackageContentOutputTypeDef",
+    {
+        "contentType": Literal["application/zip"],
+        "packageContent": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSolFunctionPackageDescriptorOutputTypeDef = TypedDict(
+    "GetSolFunctionPackageDescriptorOutputTypeDef",
+    {
+        "contentType": Literal["text/plain"],
+        "vnfd": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSolNetworkPackageContentOutputTypeDef = TypedDict(
+    "GetSolNetworkPackageContentOutputTypeDef",
+    {
+        "contentType": Literal["application/zip"],
+        "nsdContent": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSolNetworkPackageDescriptorOutputTypeDef = TypedDict(
+    "GetSolNetworkPackageDescriptorOutputTypeDef",
+    {
+        "contentType": Literal["text/plain"],
+        "nsd": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InstantiateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "InstantiateSolNetworkInstanceOutputTypeDef",
+    {
+        "nsLcmOpOccId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TerminateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "TerminateSolNetworkInstanceOutputTypeDef",
+    {
+        "nsLcmOpOccId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSolFunctionPackageOutputTypeDef = TypedDict(
+    "UpdateSolFunctionPackageOutputTypeDef",
+    {
+        "operationalState": OperationalStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "UpdateSolNetworkInstanceOutputTypeDef",
+    {
+        "nsLcmOpOccId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSolNetworkPackageOutputTypeDef = TypedDict(
+    "UpdateSolNetworkPackageOutputTypeDef",
+    {
+        "nsdOperationalState": NsdOperationalStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetSolNetworkOperationTaskDetailsTypeDef = TypedDict(
     "GetSolNetworkOperationTaskDetailsTypeDef",
     {
         "taskContext": Dict[str, str],
         "taskEndTime": datetime,
         "taskErrorDetails": ErrorInfoTypeDef,
         "taskName": str,
@@ -865,15 +825,15 @@
         "metadata": GetSolNetworkInstanceMetadataTypeDef,
         "nsInstanceDescription": str,
         "nsInstanceName": str,
         "nsState": NsStateType,
         "nsdId": str,
         "nsdInfoId": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSolVnfcResourceInfoTypeDef = TypedDict(
     "GetSolVnfcResourceInfoTypeDef",
     {
         "metadata": GetSolVnfcResourceInfoMetadataTypeDef,
@@ -904,14 +864,54 @@
 
 class ListSolFunctionInstanceInfoTypeDef(
     _RequiredListSolFunctionInstanceInfoTypeDef, _OptionalListSolFunctionInstanceInfoTypeDef
 ):
     pass
 
 
+ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef = TypedDict(
+    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef = TypedDict(
+    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef = TypedDict(
+    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef = TypedDict(
+    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef = TypedDict(
+    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredListSolFunctionPackageInfoTypeDef = TypedDict(
     "_RequiredListSolFunctionPackageInfoTypeDef",
     {
         "arn": str,
         "id": str,
         "onboardingState": OnboardingStateType,
         "operationalState": OperationalStateType,
@@ -1040,15 +1040,15 @@
         "id": str,
         "lcmOperationType": LcmOperationTypeType,
         "metadata": GetSolNetworkOperationMetadataTypeDef,
         "nsInstanceId": str,
         "operationState": NsLcmOperationStateType,
         "tags": Dict[str, str],
         "tasks": List[GetSolNetworkOperationTaskDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetSolFunctionPackageMetadataTypeDef = TypedDict(
     "_RequiredGetSolFunctionPackageMetadataTypeDef",
     {
         "createdAt": datetime,
@@ -1134,51 +1134,51 @@
 )
 
 ListSolFunctionInstancesOutputTypeDef = TypedDict(
     "ListSolFunctionInstancesOutputTypeDef",
     {
         "functionInstances": List[ListSolFunctionInstanceInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSolFunctionPackagesOutputTypeDef = TypedDict(
     "ListSolFunctionPackagesOutputTypeDef",
     {
         "functionPackages": List[ListSolFunctionPackageInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSolNetworkInstancesOutputTypeDef = TypedDict(
     "ListSolNetworkInstancesOutputTypeDef",
     {
         "networkInstances": List[ListSolNetworkInstanceInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSolNetworkOperationsOutputTypeDef = TypedDict(
     "ListSolNetworkOperationsOutputTypeDef",
     {
         "networkOperations": List[ListSolNetworkOperationsInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSolNetworkPackagesOutputTypeDef = TypedDict(
     "ListSolNetworkPackagesOutputTypeDef",
     {
         "networkPackages": List[ListSolNetworkPackageInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSolFunctionPackageOutputTypeDef = TypedDict(
     "GetSolFunctionPackageOutputTypeDef",
     {
         "arn": str,
@@ -1188,41 +1188,41 @@
         "operationalState": OperationalStateType,
         "tags": Dict[str, str],
         "usageState": UsageStateType,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutSolFunctionPackageContentOutputTypeDef = TypedDict(
     "PutSolFunctionPackageContentOutputTypeDef",
     {
         "id": str,
         "metadata": PutSolFunctionPackageContentMetadataTypeDef,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ValidateSolFunctionPackageContentOutputTypeDef = TypedDict(
     "ValidateSolFunctionPackageContentOutputTypeDef",
     {
         "id": str,
         "metadata": ValidateSolFunctionPackageContentMetadataTypeDef,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSolNetworkPackageOutputTypeDef = TypedDict(
     "GetSolNetworkPackageOutputTypeDef",
     {
         "arn": str,
@@ -1232,43 +1232,43 @@
         "nsdName": str,
         "nsdOnboardingState": NsdOnboardingStateType,
         "nsdOperationalState": NsdOperationalStateType,
         "nsdUsageState": NsdUsageStateType,
         "nsdVersion": str,
         "tags": Dict[str, str],
         "vnfPkgIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutSolNetworkPackageContentOutputTypeDef = TypedDict(
     "PutSolNetworkPackageContentOutputTypeDef",
     {
         "arn": str,
         "id": str,
         "metadata": PutSolNetworkPackageContentMetadataTypeDef,
         "nsdId": str,
         "nsdName": str,
         "nsdVersion": str,
         "vnfPkgIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ValidateSolNetworkPackageContentOutputTypeDef = TypedDict(
     "ValidateSolNetworkPackageContentOutputTypeDef",
     {
         "arn": str,
         "id": str,
         "metadata": ValidateSolNetworkPackageContentMetadataTypeDef,
         "nsdId": str,
         "nsdName": str,
         "nsdVersion": str,
         "vnfPkgIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSolFunctionInstanceOutputTypeDef = TypedDict(
     "GetSolFunctionInstanceOutputTypeDef",
     {
         "arn": str,
@@ -1279,10 +1279,10 @@
         "nsInstanceId": str,
         "tags": Dict[str, str],
         "vnfPkgId": str,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-tnb-1.28.0/mypy_boto3_tnb/type_defs.pyi` & `mypy-boto3-tnb-1.28.12/mypy_boto3_tnb/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,86 +40,86 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CancelSolNetworkOperationInputRequestTypeDef",
     "CreateSolFunctionPackageInputRequestTypeDef",
-    "CreateSolFunctionPackageOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateSolNetworkInstanceInputRequestTypeDef",
-    "CreateSolNetworkInstanceOutputTypeDef",
     "CreateSolNetworkPackageInputRequestTypeDef",
-    "CreateSolNetworkPackageOutputTypeDef",
     "DeleteSolFunctionPackageInputRequestTypeDef",
     "DeleteSolNetworkInstanceInputRequestTypeDef",
     "DeleteSolNetworkPackageInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ErrorInfoTypeDef",
     "ToscaOverrideTypeDef",
     "GetSolFunctionInstanceInputRequestTypeDef",
     "GetSolFunctionInstanceMetadataTypeDef",
     "GetSolFunctionPackageContentInputRequestTypeDef",
-    "GetSolFunctionPackageContentOutputTypeDef",
     "GetSolFunctionPackageDescriptorInputRequestTypeDef",
-    "GetSolFunctionPackageDescriptorOutputTypeDef",
     "GetSolFunctionPackageInputRequestTypeDef",
     "GetSolInstantiatedVnfInfoTypeDef",
     "GetSolNetworkInstanceInputRequestTypeDef",
     "GetSolNetworkInstanceMetadataTypeDef",
     "LcmOperationInfoTypeDef",
     "GetSolNetworkOperationInputRequestTypeDef",
     "GetSolNetworkOperationMetadataTypeDef",
     "ProblemDetailsTypeDef",
     "GetSolNetworkPackageContentInputRequestTypeDef",
-    "GetSolNetworkPackageContentOutputTypeDef",
     "GetSolNetworkPackageDescriptorInputRequestTypeDef",
-    "GetSolNetworkPackageDescriptorOutputTypeDef",
     "GetSolNetworkPackageInputRequestTypeDef",
     "GetSolVnfcResourceInfoMetadataTypeDef",
     "InstantiateSolNetworkInstanceInputRequestTypeDef",
-    "InstantiateSolNetworkInstanceOutputTypeDef",
     "ListSolFunctionInstanceMetadataTypeDef",
-    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListSolFunctionInstancesInputRequestTypeDef",
     "ListSolFunctionPackageMetadataTypeDef",
-    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
     "ListSolFunctionPackagesInputRequestTypeDef",
     "ListSolNetworkInstanceMetadataTypeDef",
-    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
     "ListSolNetworkInstancesInputRequestTypeDef",
     "ListSolNetworkOperationsMetadataTypeDef",
-    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
     "ListSolNetworkOperationsInputRequestTypeDef",
     "ListSolNetworkPackageMetadataTypeDef",
-    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
     "ListSolNetworkPackagesInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "PutSolFunctionPackageContentInputRequestTypeDef",
     "PutSolNetworkPackageContentInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "TerminateSolNetworkInstanceInputRequestTypeDef",
-    "TerminateSolNetworkInstanceOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateSolFunctionPackageInputRequestTypeDef",
-    "UpdateSolFunctionPackageOutputTypeDef",
     "UpdateSolNetworkModifyTypeDef",
-    "UpdateSolNetworkInstanceOutputTypeDef",
     "UpdateSolNetworkPackageInputRequestTypeDef",
-    "UpdateSolNetworkPackageOutputTypeDef",
     "ValidateSolFunctionPackageContentInputRequestTypeDef",
     "ValidateSolNetworkPackageContentInputRequestTypeDef",
+    "CreateSolFunctionPackageOutputTypeDef",
+    "CreateSolNetworkInstanceOutputTypeDef",
+    "CreateSolNetworkPackageOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetSolFunctionPackageContentOutputTypeDef",
+    "GetSolFunctionPackageDescriptorOutputTypeDef",
+    "GetSolNetworkPackageContentOutputTypeDef",
+    "GetSolNetworkPackageDescriptorOutputTypeDef",
+    "InstantiateSolNetworkInstanceOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "TerminateSolNetworkInstanceOutputTypeDef",
+    "UpdateSolFunctionPackageOutputTypeDef",
+    "UpdateSolNetworkInstanceOutputTypeDef",
+    "UpdateSolNetworkPackageOutputTypeDef",
     "GetSolNetworkOperationTaskDetailsTypeDef",
     "FunctionArtifactMetaTypeDef",
     "NetworkArtifactMetaTypeDef",
     "GetSolNetworkInstanceOutputTypeDef",
     "GetSolVnfcResourceInfoTypeDef",
     "ListSolFunctionInstanceInfoTypeDef",
+    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
+    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
+    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
+    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
+    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
     "ListSolFunctionPackageInfoTypeDef",
     "ListSolNetworkInstanceInfoTypeDef",
     "ListSolNetworkOperationsInfoTypeDef",
     "ListSolNetworkPackageInfoTypeDef",
     "UpdateSolNetworkInstanceInputRequestTypeDef",
     "GetSolNetworkOperationOutputTypeDef",
     "GetSolFunctionPackageMetadataTypeDef",
@@ -154,24 +154,22 @@
     "CreateSolFunctionPackageInputRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-CreateSolFunctionPackageOutputTypeDef = TypedDict(
-    "CreateSolFunctionPackageOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "arn": str,
-        "id": str,
-        "onboardingState": OnboardingStateType,
-        "operationalState": OperationalStateType,
-        "tags": Dict[str, str],
-        "usageState": UsageStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateSolNetworkInstanceInputRequestTypeDef = TypedDict(
     "_RequiredCreateSolNetworkInstanceInputRequestTypeDef",
     {
         "nsName": str,
@@ -189,47 +187,22 @@
 
 class CreateSolNetworkInstanceInputRequestTypeDef(
     _RequiredCreateSolNetworkInstanceInputRequestTypeDef,
     _OptionalCreateSolNetworkInstanceInputRequestTypeDef,
 ):
     pass
 
-CreateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "CreateSolNetworkInstanceOutputTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "nsInstanceName": str,
-        "nsdInfoId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateSolNetworkPackageInputRequestTypeDef = TypedDict(
     "CreateSolNetworkPackageInputRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-CreateSolNetworkPackageOutputTypeDef = TypedDict(
-    "CreateSolNetworkPackageOutputTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "nsdOnboardingState": NsdOnboardingStateType,
-        "nsdOperationalState": NsdOperationalStateType,
-        "nsdUsageState": NsdUsageStateType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSolFunctionPackageInputRequestTypeDef = TypedDict(
     "DeleteSolFunctionPackageInputRequestTypeDef",
     {
         "vnfPkgId": str,
     },
 )
 
@@ -243,21 +216,14 @@
 DeleteSolNetworkPackageInputRequestTypeDef = TypedDict(
     "DeleteSolNetworkPackageInputRequestTypeDef",
     {
         "nsdInfoId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ErrorInfoTypeDef = TypedDict(
     "ErrorInfoTypeDef",
     {
         "cause": str,
         "details": str,
     },
     total=False,
@@ -291,40 +257,22 @@
     "GetSolFunctionPackageContentInputRequestTypeDef",
     {
         "accept": Literal["application/zip"],
         "vnfPkgId": str,
     },
 )
 
-GetSolFunctionPackageContentOutputTypeDef = TypedDict(
-    "GetSolFunctionPackageContentOutputTypeDef",
-    {
-        "contentType": Literal["application/zip"],
-        "packageContent": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSolFunctionPackageDescriptorInputRequestTypeDef = TypedDict(
     "GetSolFunctionPackageDescriptorInputRequestTypeDef",
     {
         "accept": Literal["text/plain"],
         "vnfPkgId": str,
     },
 )
 
-GetSolFunctionPackageDescriptorOutputTypeDef = TypedDict(
-    "GetSolFunctionPackageDescriptorOutputTypeDef",
-    {
-        "contentType": Literal["text/plain"],
-        "vnfd": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSolFunctionPackageInputRequestTypeDef = TypedDict(
     "GetSolFunctionPackageInputRequestTypeDef",
     {
         "vnfPkgId": str,
     },
 )
 
@@ -394,39 +342,21 @@
     "GetSolNetworkPackageContentInputRequestTypeDef",
     {
         "accept": Literal["application/zip"],
         "nsdInfoId": str,
     },
 )
 
-GetSolNetworkPackageContentOutputTypeDef = TypedDict(
-    "GetSolNetworkPackageContentOutputTypeDef",
-    {
-        "contentType": Literal["application/zip"],
-        "nsdContent": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSolNetworkPackageDescriptorInputRequestTypeDef = TypedDict(
     "GetSolNetworkPackageDescriptorInputRequestTypeDef",
     {
         "nsdInfoId": str,
     },
 )
 
-GetSolNetworkPackageDescriptorOutputTypeDef = TypedDict(
-    "GetSolNetworkPackageDescriptorOutputTypeDef",
-    {
-        "contentType": Literal["text/plain"],
-        "nsd": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSolNetworkPackageInputRequestTypeDef = TypedDict(
     "GetSolNetworkPackageInputRequestTypeDef",
     {
         "nsdInfoId": str,
     },
 )
 
@@ -458,35 +388,28 @@
 
 class InstantiateSolNetworkInstanceInputRequestTypeDef(
     _RequiredInstantiateSolNetworkInstanceInputRequestTypeDef,
     _OptionalInstantiateSolNetworkInstanceInputRequestTypeDef,
 ):
     pass
 
-InstantiateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "InstantiateSolNetworkInstanceOutputTypeDef",
-    {
-        "nsLcmOpOccId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListSolFunctionInstanceMetadataTypeDef = TypedDict(
     "ListSolFunctionInstanceMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef = TypedDict(
-    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
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
 
 ListSolFunctionInstancesInputRequestTypeDef = TypedDict(
     "ListSolFunctionInstancesInputRequestTypeDef",
     {
@@ -500,22 +423,14 @@
     "ListSolFunctionPackageMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef = TypedDict(
-    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSolFunctionPackagesInputRequestTypeDef = TypedDict(
     "ListSolFunctionPackagesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -525,22 +440,14 @@
     "ListSolNetworkInstanceMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef = TypedDict(
-    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSolNetworkInstancesInputRequestTypeDef = TypedDict(
     "ListSolNetworkInstancesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -550,22 +457,14 @@
     "ListSolNetworkOperationsMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef = TypedDict(
-    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSolNetworkOperationsInputRequestTypeDef = TypedDict(
     "ListSolNetworkOperationsInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -575,22 +474,14 @@
     "ListSolNetworkPackageMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef = TypedDict(
-    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSolNetworkPackagesInputRequestTypeDef = TypedDict(
     "ListSolNetworkPackagesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -599,32 +490,14 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
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
 _RequiredPutSolFunctionPackageContentInputRequestTypeDef = TypedDict(
     "_RequiredPutSolFunctionPackageContentInputRequestTypeDef",
     {
         "file": Union[str, bytes, IO[Any], StreamingBody],
         "vnfPkgId": str,
     },
 )
@@ -659,25 +532,14 @@
 
 class PutSolNetworkPackageContentInputRequestTypeDef(
     _RequiredPutSolNetworkPackageContentInputRequestTypeDef,
     _OptionalPutSolNetworkPackageContentInputRequestTypeDef,
 ):
     pass
 
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
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -698,23 +560,14 @@
 
 class TerminateSolNetworkInstanceInputRequestTypeDef(
     _RequiredTerminateSolNetworkInstanceInputRequestTypeDef,
     _OptionalTerminateSolNetworkInstanceInputRequestTypeDef,
 ):
     pass
 
-TerminateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "TerminateSolNetworkInstanceOutputTypeDef",
-    {
-        "nsLcmOpOccId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -723,55 +576,30 @@
     "UpdateSolFunctionPackageInputRequestTypeDef",
     {
         "operationalState": OperationalStateType,
         "vnfPkgId": str,
     },
 )
 
-UpdateSolFunctionPackageOutputTypeDef = TypedDict(
-    "UpdateSolFunctionPackageOutputTypeDef",
-    {
-        "operationalState": OperationalStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSolNetworkModifyTypeDef = TypedDict(
     "UpdateSolNetworkModifyTypeDef",
     {
         "vnfConfigurableProperties": Mapping[str, Any],
         "vnfInstanceId": str,
     },
 )
 
-UpdateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "UpdateSolNetworkInstanceOutputTypeDef",
-    {
-        "nsLcmOpOccId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSolNetworkPackageInputRequestTypeDef = TypedDict(
     "UpdateSolNetworkPackageInputRequestTypeDef",
     {
         "nsdInfoId": str,
         "nsdOperationalState": NsdOperationalStateType,
     },
 )
 
-UpdateSolNetworkPackageOutputTypeDef = TypedDict(
-    "UpdateSolNetworkPackageOutputTypeDef",
-    {
-        "nsdOperationalState": NsdOperationalStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredValidateSolFunctionPackageContentInputRequestTypeDef = TypedDict(
     "_RequiredValidateSolFunctionPackageContentInputRequestTypeDef",
     {
         "file": Union[str, bytes, IO[Any], StreamingBody],
         "vnfPkgId": str,
     },
 )
@@ -806,14 +634,146 @@
 
 class ValidateSolNetworkPackageContentInputRequestTypeDef(
     _RequiredValidateSolNetworkPackageContentInputRequestTypeDef,
     _OptionalValidateSolNetworkPackageContentInputRequestTypeDef,
 ):
     pass
 
+CreateSolFunctionPackageOutputTypeDef = TypedDict(
+    "CreateSolFunctionPackageOutputTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "onboardingState": OnboardingStateType,
+        "operationalState": OperationalStateType,
+        "tags": Dict[str, str],
+        "usageState": UsageStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "CreateSolNetworkInstanceOutputTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "nsInstanceName": str,
+        "nsdInfoId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSolNetworkPackageOutputTypeDef = TypedDict(
+    "CreateSolNetworkPackageOutputTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "nsdOnboardingState": NsdOnboardingStateType,
+        "nsdOperationalState": NsdOperationalStateType,
+        "nsdUsageState": NsdUsageStateType,
+        "tags": Dict[str, str],
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
+GetSolFunctionPackageContentOutputTypeDef = TypedDict(
+    "GetSolFunctionPackageContentOutputTypeDef",
+    {
+        "contentType": Literal["application/zip"],
+        "packageContent": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSolFunctionPackageDescriptorOutputTypeDef = TypedDict(
+    "GetSolFunctionPackageDescriptorOutputTypeDef",
+    {
+        "contentType": Literal["text/plain"],
+        "vnfd": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSolNetworkPackageContentOutputTypeDef = TypedDict(
+    "GetSolNetworkPackageContentOutputTypeDef",
+    {
+        "contentType": Literal["application/zip"],
+        "nsdContent": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSolNetworkPackageDescriptorOutputTypeDef = TypedDict(
+    "GetSolNetworkPackageDescriptorOutputTypeDef",
+    {
+        "contentType": Literal["text/plain"],
+        "nsd": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InstantiateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "InstantiateSolNetworkInstanceOutputTypeDef",
+    {
+        "nsLcmOpOccId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TerminateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "TerminateSolNetworkInstanceOutputTypeDef",
+    {
+        "nsLcmOpOccId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSolFunctionPackageOutputTypeDef = TypedDict(
+    "UpdateSolFunctionPackageOutputTypeDef",
+    {
+        "operationalState": OperationalStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "UpdateSolNetworkInstanceOutputTypeDef",
+    {
+        "nsLcmOpOccId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSolNetworkPackageOutputTypeDef = TypedDict(
+    "UpdateSolNetworkPackageOutputTypeDef",
+    {
+        "nsdOperationalState": NsdOperationalStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetSolNetworkOperationTaskDetailsTypeDef = TypedDict(
     "GetSolNetworkOperationTaskDetailsTypeDef",
     {
         "taskContext": Dict[str, str],
         "taskEndTime": datetime,
         "taskErrorDetails": ErrorInfoTypeDef,
         "taskName": str,
@@ -848,15 +808,15 @@
         "metadata": GetSolNetworkInstanceMetadataTypeDef,
         "nsInstanceDescription": str,
         "nsInstanceName": str,
         "nsState": NsStateType,
         "nsdId": str,
         "nsdInfoId": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSolVnfcResourceInfoTypeDef = TypedDict(
     "GetSolVnfcResourceInfoTypeDef",
     {
         "metadata": GetSolVnfcResourceInfoMetadataTypeDef,
@@ -885,14 +845,54 @@
 )
 
 class ListSolFunctionInstanceInfoTypeDef(
     _RequiredListSolFunctionInstanceInfoTypeDef, _OptionalListSolFunctionInstanceInfoTypeDef
 ):
     pass
 
+ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef = TypedDict(
+    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef = TypedDict(
+    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef = TypedDict(
+    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef = TypedDict(
+    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef = TypedDict(
+    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredListSolFunctionPackageInfoTypeDef = TypedDict(
     "_RequiredListSolFunctionPackageInfoTypeDef",
     {
         "arn": str,
         "id": str,
         "onboardingState": OnboardingStateType,
         "operationalState": OperationalStateType,
@@ -1013,15 +1013,15 @@
         "id": str,
         "lcmOperationType": LcmOperationTypeType,
         "metadata": GetSolNetworkOperationMetadataTypeDef,
         "nsInstanceId": str,
         "operationState": NsLcmOperationStateType,
         "tags": Dict[str, str],
         "tasks": List[GetSolNetworkOperationTaskDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetSolFunctionPackageMetadataTypeDef = TypedDict(
     "_RequiredGetSolFunctionPackageMetadataTypeDef",
     {
         "createdAt": datetime,
@@ -1103,51 +1103,51 @@
 )
 
 ListSolFunctionInstancesOutputTypeDef = TypedDict(
     "ListSolFunctionInstancesOutputTypeDef",
     {
         "functionInstances": List[ListSolFunctionInstanceInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSolFunctionPackagesOutputTypeDef = TypedDict(
     "ListSolFunctionPackagesOutputTypeDef",
     {
         "functionPackages": List[ListSolFunctionPackageInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSolNetworkInstancesOutputTypeDef = TypedDict(
     "ListSolNetworkInstancesOutputTypeDef",
     {
         "networkInstances": List[ListSolNetworkInstanceInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSolNetworkOperationsOutputTypeDef = TypedDict(
     "ListSolNetworkOperationsOutputTypeDef",
     {
         "networkOperations": List[ListSolNetworkOperationsInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSolNetworkPackagesOutputTypeDef = TypedDict(
     "ListSolNetworkPackagesOutputTypeDef",
     {
         "networkPackages": List[ListSolNetworkPackageInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSolFunctionPackageOutputTypeDef = TypedDict(
     "GetSolFunctionPackageOutputTypeDef",
     {
         "arn": str,
@@ -1157,41 +1157,41 @@
         "operationalState": OperationalStateType,
         "tags": Dict[str, str],
         "usageState": UsageStateType,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutSolFunctionPackageContentOutputTypeDef = TypedDict(
     "PutSolFunctionPackageContentOutputTypeDef",
     {
         "id": str,
         "metadata": PutSolFunctionPackageContentMetadataTypeDef,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ValidateSolFunctionPackageContentOutputTypeDef = TypedDict(
     "ValidateSolFunctionPackageContentOutputTypeDef",
     {
         "id": str,
         "metadata": ValidateSolFunctionPackageContentMetadataTypeDef,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSolNetworkPackageOutputTypeDef = TypedDict(
     "GetSolNetworkPackageOutputTypeDef",
     {
         "arn": str,
@@ -1201,43 +1201,43 @@
         "nsdName": str,
         "nsdOnboardingState": NsdOnboardingStateType,
         "nsdOperationalState": NsdOperationalStateType,
         "nsdUsageState": NsdUsageStateType,
         "nsdVersion": str,
         "tags": Dict[str, str],
         "vnfPkgIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutSolNetworkPackageContentOutputTypeDef = TypedDict(
     "PutSolNetworkPackageContentOutputTypeDef",
     {
         "arn": str,
         "id": str,
         "metadata": PutSolNetworkPackageContentMetadataTypeDef,
         "nsdId": str,
         "nsdName": str,
         "nsdVersion": str,
         "vnfPkgIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ValidateSolNetworkPackageContentOutputTypeDef = TypedDict(
     "ValidateSolNetworkPackageContentOutputTypeDef",
     {
         "arn": str,
         "id": str,
         "metadata": ValidateSolNetworkPackageContentMetadataTypeDef,
         "nsdId": str,
         "nsdName": str,
         "nsdVersion": str,
         "vnfPkgIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSolFunctionInstanceOutputTypeDef = TypedDict(
     "GetSolFunctionInstanceOutputTypeDef",
     {
         "arn": str,
@@ -1248,10 +1248,10 @@
         "nsInstanceId": str,
         "tags": Dict[str, str],
         "vnfPkgId": str,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-tnb-1.28.0/mypy_boto3_tnb.egg-info/PKG-INFO` & `mypy-boto3-tnb-1.28.12/mypy_boto3_tnb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-tnb
-Version: 1.28.0
-Summary: Type annotations for boto3.TelcoNetworkBuilder 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.TelcoNetworkBuilder 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-tnb"></a>
 
 # mypy-boto3-tnb
 
 [![PyPI - mypy-boto3-tnb](https://img.shields.io/pypi/v/mypy-boto3-tnb.svg?color=blue)](https://pypi.org/project/mypy-boto3-tnb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-tnb.svg?color=blue)](https://pypi.org/project/mypy-boto3-tnb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-tnb?color=blue)](https://pypistats.org/packages/mypy-boto3-tnb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-tnb)](https://pepy.tech/project/mypy-boto3-tnb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TelcoNetworkBuilder 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
+[boto3.TelcoNetworkBuilder 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
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
 [mypy-boto3-tnb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_tnb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,86 +357,86 @@
 `mypy_boto3_tnb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_tnb.type_defs import (
     CancelSolNetworkOperationInputRequestTypeDef,
     CreateSolFunctionPackageInputRequestTypeDef,
-    CreateSolFunctionPackageOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateSolNetworkInstanceInputRequestTypeDef,
-    CreateSolNetworkInstanceOutputTypeDef,
     CreateSolNetworkPackageInputRequestTypeDef,
-    CreateSolNetworkPackageOutputTypeDef,
     DeleteSolFunctionPackageInputRequestTypeDef,
     DeleteSolNetworkInstanceInputRequestTypeDef,
     DeleteSolNetworkPackageInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ErrorInfoTypeDef,
     ToscaOverrideTypeDef,
     GetSolFunctionInstanceInputRequestTypeDef,
     GetSolFunctionInstanceMetadataTypeDef,
     GetSolFunctionPackageContentInputRequestTypeDef,
-    GetSolFunctionPackageContentOutputTypeDef,
     GetSolFunctionPackageDescriptorInputRequestTypeDef,
-    GetSolFunctionPackageDescriptorOutputTypeDef,
     GetSolFunctionPackageInputRequestTypeDef,
     GetSolInstantiatedVnfInfoTypeDef,
     GetSolNetworkInstanceInputRequestTypeDef,
     GetSolNetworkInstanceMetadataTypeDef,
     LcmOperationInfoTypeDef,
     GetSolNetworkOperationInputRequestTypeDef,
     GetSolNetworkOperationMetadataTypeDef,
     ProblemDetailsTypeDef,
     GetSolNetworkPackageContentInputRequestTypeDef,
-    GetSolNetworkPackageContentOutputTypeDef,
     GetSolNetworkPackageDescriptorInputRequestTypeDef,
-    GetSolNetworkPackageDescriptorOutputTypeDef,
     GetSolNetworkPackageInputRequestTypeDef,
     GetSolVnfcResourceInfoMetadataTypeDef,
     InstantiateSolNetworkInstanceInputRequestTypeDef,
-    InstantiateSolNetworkInstanceOutputTypeDef,
     ListSolFunctionInstanceMetadataTypeDef,
-    ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListSolFunctionInstancesInputRequestTypeDef,
     ListSolFunctionPackageMetadataTypeDef,
-    ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef,
     ListSolFunctionPackagesInputRequestTypeDef,
     ListSolNetworkInstanceMetadataTypeDef,
-    ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef,
     ListSolNetworkInstancesInputRequestTypeDef,
     ListSolNetworkOperationsMetadataTypeDef,
-    ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef,
     ListSolNetworkOperationsInputRequestTypeDef,
     ListSolNetworkPackageMetadataTypeDef,
-    ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef,
     ListSolNetworkPackagesInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PaginatorConfigTypeDef,
     PutSolFunctionPackageContentInputRequestTypeDef,
     PutSolNetworkPackageContentInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     TerminateSolNetworkInstanceInputRequestTypeDef,
-    TerminateSolNetworkInstanceOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateSolFunctionPackageInputRequestTypeDef,
-    UpdateSolFunctionPackageOutputTypeDef,
     UpdateSolNetworkModifyTypeDef,
-    UpdateSolNetworkInstanceOutputTypeDef,
     UpdateSolNetworkPackageInputRequestTypeDef,
-    UpdateSolNetworkPackageOutputTypeDef,
     ValidateSolFunctionPackageContentInputRequestTypeDef,
     ValidateSolNetworkPackageContentInputRequestTypeDef,
+    CreateSolFunctionPackageOutputTypeDef,
+    CreateSolNetworkInstanceOutputTypeDef,
+    CreateSolNetworkPackageOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetSolFunctionPackageContentOutputTypeDef,
+    GetSolFunctionPackageDescriptorOutputTypeDef,
+    GetSolNetworkPackageContentOutputTypeDef,
+    GetSolNetworkPackageDescriptorOutputTypeDef,
+    InstantiateSolNetworkInstanceOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    TerminateSolNetworkInstanceOutputTypeDef,
+    UpdateSolFunctionPackageOutputTypeDef,
+    UpdateSolNetworkInstanceOutputTypeDef,
+    UpdateSolNetworkPackageOutputTypeDef,
     GetSolNetworkOperationTaskDetailsTypeDef,
     FunctionArtifactMetaTypeDef,
     NetworkArtifactMetaTypeDef,
     GetSolNetworkInstanceOutputTypeDef,
     GetSolVnfcResourceInfoTypeDef,
     ListSolFunctionInstanceInfoTypeDef,
+    ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef,
+    ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef,
+    ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef,
+    ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef,
+    ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef,
     ListSolFunctionPackageInfoTypeDef,
     ListSolNetworkInstanceInfoTypeDef,
     ListSolNetworkOperationsInfoTypeDef,
     ListSolNetworkPackageInfoTypeDef,
     UpdateSolNetworkInstanceInputRequestTypeDef,
     GetSolNetworkOperationOutputTypeDef,
     GetSolFunctionPackageMetadataTypeDef,
```

### Comparing `mypy-boto3-tnb-1.28.0/mypy_boto3_tnb.egg-info/SOURCES.txt` & `mypy-boto3-tnb-1.28.12/mypy_boto3_tnb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-tnb-1.28.0/setup.py` & `mypy-boto3-tnb-1.28.12/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-tnb",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_tnb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.TelcoNetworkBuilder 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.TelcoNetworkBuilder 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

