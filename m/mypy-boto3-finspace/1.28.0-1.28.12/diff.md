# Comparing `tmp/mypy-boto3-finspace-1.28.0.tar.gz` & `tmp/mypy-boto3-finspace-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-finspace-1.28.0.tar", last modified: Thu Jul  6 20:59:35 2023, max compression
+gzip compressed data, was "mypy-boto3-finspace-1.28.12.tar", last modified: Thu Jul 27 05:34:42 2023, max compression
```

## Comparing `mypy-boto3-finspace-1.28.0.tar` & `mypy-boto3-finspace-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:35.070302 mypy-boto3-finspace-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:40:56.000000 mypy-boto3-finspace-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-07-06 20:59:35.066302 mypy-boto3-finspace-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14586 2023-07-06 20:40:56.000000 mypy-boto3-finspace-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:35.054302 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-06 20:40:56.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-06 20:40:56.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:40:56.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24718 2023-07-06 20:40:58.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24676 2023-07-06 20:40:58.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-07-06 20:40:58.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9692 2023-07-06 20:40:58.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-06 20:40:58.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-06 20:40:58.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:40:56.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34927 2023-07-06 20:40:59.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34889 2023-07-06 20:40:59.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:40:56.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:35.066302 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-07-06 20:59:34.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 20:59:34.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:34.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:34.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:34.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 20:59:34.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:35.070302 mypy-boto3-finspace-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:40:56.000000 mypy-boto3-finspace-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.000509 mypy-boto3-finspace-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:13.000000 mypy-boto3-finspace-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16597 2023-07-27 05:34:42.000509 mypy-boto3-finspace-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-07-27 05:22:13.000000 mypy-boto3-finspace-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.000509 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-27 05:22:13.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-27 05:22:13.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 05:22:13.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24718 2023-07-27 05:22:14.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24676 2023-07-27 05:22:13.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-07-27 05:22:14.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-07-27 05:22:14.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-27 05:22:14.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-27 05:22:14.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:13.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39016 2023-07-27 05:22:14.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38974 2023-07-27 05:22:14.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:13.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.000509 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16597 2023-07-27 05:34:41.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 05:34:41.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:41.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:41.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:41.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 05:34:41.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:42.000509 mypy-boto3-finspace-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 05:22:13.000000 mypy-boto3-finspace-1.28.12/setup.py
```

### Comparing `mypy-boto3-finspace-1.28.0/LICENSE` & `mypy-boto3-finspace-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.0/PKG-INFO` & `mypy-boto3-finspace-1.28.12/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-finspace
-Version: 1.28.0
-Summary: Type annotations for boto3.finspace 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.finspace 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-finspace"></a>
 
 # mypy-boto3-finspace
 
 [![PyPI - mypy-boto3-finspace](https://img.shields.io/pypi/v/mypy-boto3-finspace.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-finspace?color=blue)](https://pypistats.org/packages/mypy-boto3-finspace)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-finspace)](https://pepy.tech/project/mypy-boto3-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.finspace 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
+[boto3.finspace 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
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
 [mypy-boto3-finspace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,51 +333,62 @@
 ### Typed dictionaries
 
 `mypy_boto3_finspace.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_finspace.type_defs import (
+    AutoScalingConfigurationOutputTypeDef,
     AutoScalingConfigurationTypeDef,
+    CapacityConfigurationOutputTypeDef,
     CapacityConfigurationTypeDef,
+    ChangeRequestOutputTypeDef,
     ChangeRequestTypeDef,
+    CodeConfigurationOutputTypeDef,
     CodeConfigurationTypeDef,
     FederationParametersTypeDef,
     SuperuserParametersTypeDef,
     CreateEnvironmentResponseTypeDef,
     ErrorInfoTypeDef,
     KxCacheStorageConfigurationTypeDef,
     KxCommandLineArgumentTypeDef,
     KxSavedownStorageConfigurationTypeDef,
     VpcConfigurationTypeDef,
+    KxCacheStorageConfigurationOutputTypeDef,
+    KxCommandLineArgumentOutputTypeDef,
+    KxSavedownStorageConfigurationOutputTypeDef,
+    VpcConfigurationOutputTypeDef,
     CreateKxDatabaseRequestRequestTypeDef,
     CreateKxDatabaseResponseTypeDef,
     CreateKxEnvironmentRequestRequestTypeDef,
     CreateKxEnvironmentResponseTypeDef,
     CreateKxUserRequestRequestTypeDef,
     CreateKxUserResponseTypeDef,
+    CustomDNSServerOutputTypeDef,
     CustomDNSServerTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteKxClusterRequestRequestTypeDef,
     DeleteKxDatabaseRequestRequestTypeDef,
     DeleteKxEnvironmentRequestRequestTypeDef,
     DeleteKxUserRequestRequestTypeDef,
+    FederationParametersOutputTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetKxChangesetRequestRequestTypeDef,
     GetKxClusterRequestRequestTypeDef,
     GetKxConnectionStringRequestRequestTypeDef,
     GetKxConnectionStringResponseTypeDef,
     GetKxDatabaseRequestRequestTypeDef,
     GetKxDatabaseResponseTypeDef,
     GetKxEnvironmentRequestRequestTypeDef,
-    TransitGatewayConfigurationTypeDef,
+    TransitGatewayConfigurationOutputTypeDef,
     GetKxUserRequestRequestTypeDef,
     GetKxUserResponseTypeDef,
     KxChangesetListEntryTypeDef,
     KxClusterTypeDef,
+    KxDatabaseCacheConfigurationOutputTypeDef,
     KxDatabaseCacheConfigurationTypeDef,
     KxDatabaseListEntryTypeDef,
     KxNodeTypeDef,
     KxUserTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListKxChangesetsRequestRequestTypeDef,
     ListKxClusterNodesRequestRequestTypeDef,
@@ -387,49 +398,51 @@
     ListKxEnvironmentsRequestRequestTypeDef,
     ListKxUsersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
+    TransitGatewayConfigurationTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateKxDatabaseRequestRequestTypeDef,
     UpdateKxDatabaseResponseTypeDef,
     UpdateKxEnvironmentRequestRequestTypeDef,
     UpdateKxUserRequestRequestTypeDef,
     UpdateKxUserResponseTypeDef,
     CreateKxChangesetRequestRequestTypeDef,
-    EnvironmentTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
     CreateKxChangesetResponseTypeDef,
     GetKxChangesetResponseTypeDef,
+    EnvironmentTypeDef,
     GetKxEnvironmentResponseTypeDef,
     KxEnvironmentTypeDef,
-    UpdateKxEnvironmentNetworkRequestRequestTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClustersResponseTypeDef,
+    KxDatabaseConfigurationOutputTypeDef,
     KxDatabaseConfigurationTypeDef,
     ListKxDatabasesResponseTypeDef,
     ListKxClusterNodesResponseTypeDef,
     ListKxUsersResponseTypeDef,
+    UpdateKxEnvironmentNetworkRequestRequestTypeDef,
     GetEnvironmentResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
     ListKxEnvironmentsResponseTypeDef,
-    CreateKxClusterRequestRequestTypeDef,
     CreateKxClusterResponseTypeDef,
     GetKxClusterResponseTypeDef,
+    CreateKxClusterRequestRequestTypeDef,
     UpdateKxClusterDatabasesRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AutoScalingConfigurationTypeDef:
+def get_structure() -> AutoScalingConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-finspace-1.28.0/README.md` & `mypy-boto3-finspace-1.28.12/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-finspace"></a>
 
 # mypy-boto3-finspace
 
 [![PyPI - mypy-boto3-finspace](https://img.shields.io/pypi/v/mypy-boto3-finspace.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-finspace?color=blue)](https://pypistats.org/packages/mypy-boto3-finspace)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-finspace)](https://pepy.tech/project/mypy-boto3-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.finspace 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
+[boto3.finspace 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
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
 [mypy-boto3-finspace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,51 +301,62 @@
 ### Typed dictionaries
 
 `mypy_boto3_finspace.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_finspace.type_defs import (
+    AutoScalingConfigurationOutputTypeDef,
     AutoScalingConfigurationTypeDef,
+    CapacityConfigurationOutputTypeDef,
     CapacityConfigurationTypeDef,
+    ChangeRequestOutputTypeDef,
     ChangeRequestTypeDef,
+    CodeConfigurationOutputTypeDef,
     CodeConfigurationTypeDef,
     FederationParametersTypeDef,
     SuperuserParametersTypeDef,
     CreateEnvironmentResponseTypeDef,
     ErrorInfoTypeDef,
     KxCacheStorageConfigurationTypeDef,
     KxCommandLineArgumentTypeDef,
     KxSavedownStorageConfigurationTypeDef,
     VpcConfigurationTypeDef,
+    KxCacheStorageConfigurationOutputTypeDef,
+    KxCommandLineArgumentOutputTypeDef,
+    KxSavedownStorageConfigurationOutputTypeDef,
+    VpcConfigurationOutputTypeDef,
     CreateKxDatabaseRequestRequestTypeDef,
     CreateKxDatabaseResponseTypeDef,
     CreateKxEnvironmentRequestRequestTypeDef,
     CreateKxEnvironmentResponseTypeDef,
     CreateKxUserRequestRequestTypeDef,
     CreateKxUserResponseTypeDef,
+    CustomDNSServerOutputTypeDef,
     CustomDNSServerTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteKxClusterRequestRequestTypeDef,
     DeleteKxDatabaseRequestRequestTypeDef,
     DeleteKxEnvironmentRequestRequestTypeDef,
     DeleteKxUserRequestRequestTypeDef,
+    FederationParametersOutputTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetKxChangesetRequestRequestTypeDef,
     GetKxClusterRequestRequestTypeDef,
     GetKxConnectionStringRequestRequestTypeDef,
     GetKxConnectionStringResponseTypeDef,
     GetKxDatabaseRequestRequestTypeDef,
     GetKxDatabaseResponseTypeDef,
     GetKxEnvironmentRequestRequestTypeDef,
-    TransitGatewayConfigurationTypeDef,
+    TransitGatewayConfigurationOutputTypeDef,
     GetKxUserRequestRequestTypeDef,
     GetKxUserResponseTypeDef,
     KxChangesetListEntryTypeDef,
     KxClusterTypeDef,
+    KxDatabaseCacheConfigurationOutputTypeDef,
     KxDatabaseCacheConfigurationTypeDef,
     KxDatabaseListEntryTypeDef,
     KxNodeTypeDef,
     KxUserTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListKxChangesetsRequestRequestTypeDef,
     ListKxClusterNodesRequestRequestTypeDef,
@@ -355,49 +366,51 @@
     ListKxEnvironmentsRequestRequestTypeDef,
     ListKxUsersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
+    TransitGatewayConfigurationTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateKxDatabaseRequestRequestTypeDef,
     UpdateKxDatabaseResponseTypeDef,
     UpdateKxEnvironmentRequestRequestTypeDef,
     UpdateKxUserRequestRequestTypeDef,
     UpdateKxUserResponseTypeDef,
     CreateKxChangesetRequestRequestTypeDef,
-    EnvironmentTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
     CreateKxChangesetResponseTypeDef,
     GetKxChangesetResponseTypeDef,
+    EnvironmentTypeDef,
     GetKxEnvironmentResponseTypeDef,
     KxEnvironmentTypeDef,
-    UpdateKxEnvironmentNetworkRequestRequestTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClustersResponseTypeDef,
+    KxDatabaseConfigurationOutputTypeDef,
     KxDatabaseConfigurationTypeDef,
     ListKxDatabasesResponseTypeDef,
     ListKxClusterNodesResponseTypeDef,
     ListKxUsersResponseTypeDef,
+    UpdateKxEnvironmentNetworkRequestRequestTypeDef,
     GetEnvironmentResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
     ListKxEnvironmentsResponseTypeDef,
-    CreateKxClusterRequestRequestTypeDef,
     CreateKxClusterResponseTypeDef,
     GetKxClusterResponseTypeDef,
+    CreateKxClusterRequestRequestTypeDef,
     UpdateKxClusterDatabasesRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AutoScalingConfigurationTypeDef:
+def get_structure() -> AutoScalingConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/__init__.py` & `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/__init__.pyi` & `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/__main__.py` & `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.finspace 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.finspace 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace\nOther"
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

### Comparing `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/client.py` & `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/client.pyi` & `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/literals.py` & `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,14 +208,15 @@
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
@@ -294,26 +295,28 @@
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

### Comparing `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/literals.pyi` & `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -206,14 +206,15 @@
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
@@ -292,26 +293,28 @@
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

### Comparing `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/paginator.py` & `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/paginator.pyi` & `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/type_defs.py` & `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for finspace service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_finspace.type_defs import AutoScalingConfigurationTypeDef
+    from mypy_boto3_finspace.type_defs import AutoScalingConfigurationOutputTypeDef
 
-    data: AutoScalingConfigurationTypeDef = {...}
+    data: AutoScalingConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -35,51 +35,62 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AutoScalingConfigurationOutputTypeDef",
     "AutoScalingConfigurationTypeDef",
+    "CapacityConfigurationOutputTypeDef",
     "CapacityConfigurationTypeDef",
+    "ChangeRequestOutputTypeDef",
     "ChangeRequestTypeDef",
+    "CodeConfigurationOutputTypeDef",
     "CodeConfigurationTypeDef",
     "FederationParametersTypeDef",
     "SuperuserParametersTypeDef",
     "CreateEnvironmentResponseTypeDef",
     "ErrorInfoTypeDef",
     "KxCacheStorageConfigurationTypeDef",
     "KxCommandLineArgumentTypeDef",
     "KxSavedownStorageConfigurationTypeDef",
     "VpcConfigurationTypeDef",
+    "KxCacheStorageConfigurationOutputTypeDef",
+    "KxCommandLineArgumentOutputTypeDef",
+    "KxSavedownStorageConfigurationOutputTypeDef",
+    "VpcConfigurationOutputTypeDef",
     "CreateKxDatabaseRequestRequestTypeDef",
     "CreateKxDatabaseResponseTypeDef",
     "CreateKxEnvironmentRequestRequestTypeDef",
     "CreateKxEnvironmentResponseTypeDef",
     "CreateKxUserRequestRequestTypeDef",
     "CreateKxUserResponseTypeDef",
+    "CustomDNSServerOutputTypeDef",
     "CustomDNSServerTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteKxClusterRequestRequestTypeDef",
     "DeleteKxDatabaseRequestRequestTypeDef",
     "DeleteKxEnvironmentRequestRequestTypeDef",
     "DeleteKxUserRequestRequestTypeDef",
+    "FederationParametersOutputTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetKxChangesetRequestRequestTypeDef",
     "GetKxClusterRequestRequestTypeDef",
     "GetKxConnectionStringRequestRequestTypeDef",
     "GetKxConnectionStringResponseTypeDef",
     "GetKxDatabaseRequestRequestTypeDef",
     "GetKxDatabaseResponseTypeDef",
     "GetKxEnvironmentRequestRequestTypeDef",
-    "TransitGatewayConfigurationTypeDef",
+    "TransitGatewayConfigurationOutputTypeDef",
     "GetKxUserRequestRequestTypeDef",
     "GetKxUserResponseTypeDef",
     "KxChangesetListEntryTypeDef",
     "KxClusterTypeDef",
+    "KxDatabaseCacheConfigurationOutputTypeDef",
     "KxDatabaseCacheConfigurationTypeDef",
     "KxDatabaseListEntryTypeDef",
     "KxNodeTypeDef",
     "KxUserTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListKxChangesetsRequestRequestTypeDef",
     "ListKxClusterNodesRequestRequestTypeDef",
@@ -89,69 +100,115 @@
     "ListKxEnvironmentsRequestRequestTypeDef",
     "ListKxUsersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "TransitGatewayConfigurationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateKxDatabaseRequestRequestTypeDef",
     "UpdateKxDatabaseResponseTypeDef",
     "UpdateKxEnvironmentRequestRequestTypeDef",
     "UpdateKxUserRequestRequestTypeDef",
     "UpdateKxUserResponseTypeDef",
     "CreateKxChangesetRequestRequestTypeDef",
-    "EnvironmentTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
     "CreateKxChangesetResponseTypeDef",
     "GetKxChangesetResponseTypeDef",
+    "EnvironmentTypeDef",
     "GetKxEnvironmentResponseTypeDef",
     "KxEnvironmentTypeDef",
-    "UpdateKxEnvironmentNetworkRequestRequestTypeDef",
     "UpdateKxEnvironmentNetworkResponseTypeDef",
     "UpdateKxEnvironmentResponseTypeDef",
     "ListKxChangesetsResponseTypeDef",
     "ListKxClustersResponseTypeDef",
+    "KxDatabaseConfigurationOutputTypeDef",
     "KxDatabaseConfigurationTypeDef",
     "ListKxDatabasesResponseTypeDef",
     "ListKxClusterNodesResponseTypeDef",
     "ListKxUsersResponseTypeDef",
+    "UpdateKxEnvironmentNetworkRequestRequestTypeDef",
     "GetEnvironmentResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "UpdateEnvironmentResponseTypeDef",
     "ListKxEnvironmentsResponseTypeDef",
-    "CreateKxClusterRequestRequestTypeDef",
     "CreateKxClusterResponseTypeDef",
     "GetKxClusterResponseTypeDef",
+    "CreateKxClusterRequestRequestTypeDef",
     "UpdateKxClusterDatabasesRequestRequestTypeDef",
 )
 
+AutoScalingConfigurationOutputTypeDef = TypedDict(
+    "AutoScalingConfigurationOutputTypeDef",
+    {
+        "minNodeCount": int,
+        "maxNodeCount": int,
+        "autoScalingMetric": Literal["CPU_UTILIZATION_PERCENTAGE"],
+        "metricTarget": float,
+        "scaleInCooldownSeconds": float,
+        "scaleOutCooldownSeconds": float,
+    },
+    total=False,
+)
+
 AutoScalingConfigurationTypeDef = TypedDict(
     "AutoScalingConfigurationTypeDef",
     {
         "minNodeCount": int,
         "maxNodeCount": int,
         "autoScalingMetric": Literal["CPU_UTILIZATION_PERCENTAGE"],
         "metricTarget": float,
         "scaleInCooldownSeconds": float,
         "scaleOutCooldownSeconds": float,
     },
     total=False,
 )
 
+CapacityConfigurationOutputTypeDef = TypedDict(
+    "CapacityConfigurationOutputTypeDef",
+    {
+        "nodeType": str,
+        "nodeCount": int,
+    },
+    total=False,
+)
+
 CapacityConfigurationTypeDef = TypedDict(
     "CapacityConfigurationTypeDef",
     {
         "nodeType": str,
         "nodeCount": int,
     },
     total=False,
 )
 
+_RequiredChangeRequestOutputTypeDef = TypedDict(
+    "_RequiredChangeRequestOutputTypeDef",
+    {
+        "changeType": ChangeTypeType,
+        "dbPath": str,
+    },
+)
+_OptionalChangeRequestOutputTypeDef = TypedDict(
+    "_OptionalChangeRequestOutputTypeDef",
+    {
+        "s3Path": str,
+    },
+    total=False,
+)
+
+
+class ChangeRequestOutputTypeDef(
+    _RequiredChangeRequestOutputTypeDef, _OptionalChangeRequestOutputTypeDef
+):
+    pass
+
+
 _RequiredChangeRequestTypeDef = TypedDict(
     "_RequiredChangeRequestTypeDef",
     {
         "changeType": ChangeTypeType,
         "dbPath": str,
     },
 )
@@ -164,14 +221,24 @@
 )
 
 
 class ChangeRequestTypeDef(_RequiredChangeRequestTypeDef, _OptionalChangeRequestTypeDef):
     pass
 
 
+CodeConfigurationOutputTypeDef = TypedDict(
+    "CodeConfigurationOutputTypeDef",
+    {
+        "s3Bucket": str,
+        "s3Key": str,
+        "s3ObjectVersion": str,
+    },
+    total=False,
+)
+
 CodeConfigurationTypeDef = TypedDict(
     "CodeConfigurationTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
         "s3ObjectVersion": str,
     },
@@ -251,14 +318,50 @@
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
         "ipAddressType": Literal["IP_V4"],
     },
     total=False,
 )
 
+KxCacheStorageConfigurationOutputTypeDef = TypedDict(
+    "KxCacheStorageConfigurationOutputTypeDef",
+    {
+        "type": str,
+        "size": int,
+    },
+)
+
+KxCommandLineArgumentOutputTypeDef = TypedDict(
+    "KxCommandLineArgumentOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+    total=False,
+)
+
+KxSavedownStorageConfigurationOutputTypeDef = TypedDict(
+    "KxSavedownStorageConfigurationOutputTypeDef",
+    {
+        "type": Literal["SDS01"],
+        "size": int,
+    },
+)
+
+VpcConfigurationOutputTypeDef = TypedDict(
+    "VpcConfigurationOutputTypeDef",
+    {
+        "vpcId": str,
+        "securityGroupIds": List[str],
+        "subnetIds": List[str],
+        "ipAddressType": Literal["IP_V4"],
+    },
+    total=False,
+)
+
 _RequiredCreateKxDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxDatabaseRequestRequestTypeDef",
     {
         "environmentId": str,
         "databaseName": str,
         "clientToken": str,
     },
@@ -362,14 +465,22 @@
         "userArn": str,
         "environmentId": str,
         "iamRole": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CustomDNSServerOutputTypeDef = TypedDict(
+    "CustomDNSServerOutputTypeDef",
+    {
+        "customDNSServerName": str,
+        "customDNSServerIP": str,
+    },
+)
+
 CustomDNSServerTypeDef = TypedDict(
     "CustomDNSServerTypeDef",
     {
         "customDNSServerName": str,
         "customDNSServerIP": str,
     },
 )
@@ -423,14 +534,27 @@
     "DeleteKxUserRequestRequestTypeDef",
     {
         "userName": str,
         "environmentId": str,
     },
 )
 
+FederationParametersOutputTypeDef = TypedDict(
+    "FederationParametersOutputTypeDef",
+    {
+        "samlMetadataDocument": str,
+        "samlMetadataURL": str,
+        "applicationCallBackURL": str,
+        "federationURN": str,
+        "federationProviderName": str,
+        "attributeMap": Dict[str, str],
+    },
+    total=False,
+)
+
 GetEnvironmentRequestRequestTypeDef = TypedDict(
     "GetEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
@@ -496,16 +620,16 @@
 GetKxEnvironmentRequestRequestTypeDef = TypedDict(
     "GetKxEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-TransitGatewayConfigurationTypeDef = TypedDict(
-    "TransitGatewayConfigurationTypeDef",
+TransitGatewayConfigurationOutputTypeDef = TypedDict(
+    "TransitGatewayConfigurationOutputTypeDef",
     {
         "transitGatewayID": str,
         "routableCIDRSpace": str,
     },
 )
 
 GetKxUserRequestRequestTypeDef = TypedDict(
@@ -554,14 +678,22 @@
         "availabilityZoneId": str,
         "lastModifiedTimestamp": datetime,
         "createdTimestamp": datetime,
     },
     total=False,
 )
 
+KxDatabaseCacheConfigurationOutputTypeDef = TypedDict(
+    "KxDatabaseCacheConfigurationOutputTypeDef",
+    {
+        "cacheType": str,
+        "dbPaths": List[str],
+    },
+)
+
 KxDatabaseCacheConfigurationTypeDef = TypedDict(
     "KxDatabaseCacheConfigurationTypeDef",
     {
         "cacheType": str,
         "dbPaths": Sequence[str],
     },
 )
@@ -778,14 +910,22 @@
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
 
+TransitGatewayConfigurationTypeDef = TypedDict(
+    "TransitGatewayConfigurationTypeDef",
+    {
+        "transitGatewayID": str,
+        "routableCIDRSpace": str,
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -888,33 +1028,14 @@
         "environmentId": str,
         "databaseName": str,
         "changeRequests": Sequence[ChangeRequestTypeDef],
         "clientToken": str,
     },
 )
 
-EnvironmentTypeDef = TypedDict(
-    "EnvironmentTypeDef",
-    {
-        "name": str,
-        "environmentId": str,
-        "awsAccountId": str,
-        "status": EnvironmentStatusType,
-        "environmentUrl": str,
-        "description": str,
-        "environmentArn": str,
-        "sageMakerStudioDomainUrl": str,
-        "kmsKeyId": str,
-        "dedicatedServiceAccountId": str,
-        "federationMode": FederationModeType,
-        "federationParameters": FederationParametersTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 _OptionalUpdateEnvironmentRequestRequestTypeDef = TypedDict(
@@ -964,55 +1085,74 @@
 
 CreateKxChangesetResponseTypeDef = TypedDict(
     "CreateKxChangesetResponseTypeDef",
     {
         "changesetId": str,
         "databaseName": str,
         "environmentId": str,
-        "changeRequests": List[ChangeRequestTypeDef],
+        "changeRequests": List[ChangeRequestOutputTypeDef],
         "createdTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
         "status": ChangesetStatusType,
         "errorInfo": ErrorInfoTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetKxChangesetResponseTypeDef = TypedDict(
     "GetKxChangesetResponseTypeDef",
     {
         "changesetId": str,
         "databaseName": str,
         "environmentId": str,
-        "changeRequests": List[ChangeRequestTypeDef],
+        "changeRequests": List[ChangeRequestOutputTypeDef],
         "createdTimestamp": datetime,
         "activeFromTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
         "status": ChangesetStatusType,
         "errorInfo": ErrorInfoTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EnvironmentTypeDef = TypedDict(
+    "EnvironmentTypeDef",
+    {
+        "name": str,
+        "environmentId": str,
+        "awsAccountId": str,
+        "status": EnvironmentStatusType,
+        "environmentUrl": str,
+        "description": str,
+        "environmentArn": str,
+        "sageMakerStudioDomainUrl": str,
+        "kmsKeyId": str,
+        "dedicatedServiceAccountId": str,
+        "federationMode": FederationModeType,
+        "federationParameters": FederationParametersOutputTypeDef,
+    },
+    total=False,
+)
+
 GetKxEnvironmentResponseTypeDef = TypedDict(
     "GetKxEnvironmentResponseTypeDef",
     {
         "name": str,
         "environmentId": str,
         "awsAccountId": str,
         "status": EnvironmentStatusType,
         "tgwStatus": tgwStatusType,
         "dnsStatus": dnsStatusType,
         "errorMessage": str,
         "description": str,
         "environmentArn": str,
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
-        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
-        "customDNSConfiguration": List[CustomDNSServerTypeDef],
+        "transitGatewayConfiguration": TransitGatewayConfigurationOutputTypeDef,
+        "customDNSConfiguration": List[CustomDNSServerOutputTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
         "certificateAuthorityArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1027,64 +1167,40 @@
         "tgwStatus": tgwStatusType,
         "dnsStatus": dnsStatusType,
         "errorMessage": str,
         "description": str,
         "environmentArn": str,
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
-        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
-        "customDNSConfiguration": List[CustomDNSServerTypeDef],
+        "transitGatewayConfiguration": TransitGatewayConfigurationOutputTypeDef,
+        "customDNSConfiguration": List[CustomDNSServerOutputTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
         "certificateAuthorityArn": str,
     },
     total=False,
 )
 
-_RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef",
-    {
-        "environmentId": str,
-    },
-)
-_OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef",
-    {
-        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
-        "customDNSConfiguration": Sequence[CustomDNSServerTypeDef],
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class UpdateKxEnvironmentNetworkRequestRequestTypeDef(
-    _RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef,
-    _OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef,
-):
-    pass
-
-
 UpdateKxEnvironmentNetworkResponseTypeDef = TypedDict(
     "UpdateKxEnvironmentNetworkResponseTypeDef",
     {
         "name": str,
         "environmentId": str,
         "awsAccountId": str,
         "status": EnvironmentStatusType,
         "tgwStatus": tgwStatusType,
         "dnsStatus": dnsStatusType,
         "errorMessage": str,
         "description": str,
         "environmentArn": str,
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
-        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
-        "customDNSConfiguration": List[CustomDNSServerTypeDef],
+        "transitGatewayConfiguration": TransitGatewayConfigurationOutputTypeDef,
+        "customDNSConfiguration": List[CustomDNSServerOutputTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1098,16 +1214,16 @@
         "tgwStatus": tgwStatusType,
         "dnsStatus": dnsStatusType,
         "errorMessage": str,
         "description": str,
         "environmentArn": str,
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
-        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
-        "customDNSConfiguration": List[CustomDNSServerTypeDef],
+        "transitGatewayConfiguration": TransitGatewayConfigurationOutputTypeDef,
+        "customDNSConfiguration": List[CustomDNSServerOutputTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1125,14 +1241,36 @@
     {
         "kxClusterSummaries": List[KxClusterTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredKxDatabaseConfigurationOutputTypeDef = TypedDict(
+    "_RequiredKxDatabaseConfigurationOutputTypeDef",
+    {
+        "databaseName": str,
+    },
+)
+_OptionalKxDatabaseConfigurationOutputTypeDef = TypedDict(
+    "_OptionalKxDatabaseConfigurationOutputTypeDef",
+    {
+        "cacheConfigurations": List[KxDatabaseCacheConfigurationOutputTypeDef],
+        "changesetId": str,
+    },
+    total=False,
+)
+
+
+class KxDatabaseConfigurationOutputTypeDef(
+    _RequiredKxDatabaseConfigurationOutputTypeDef, _OptionalKxDatabaseConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredKxDatabaseConfigurationTypeDef = TypedDict(
     "_RequiredKxDatabaseConfigurationTypeDef",
     {
         "databaseName": str,
     },
 )
 _OptionalKxDatabaseConfigurationTypeDef = TypedDict(
@@ -1174,14 +1312,38 @@
     {
         "users": List[KxUserTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef",
+    {
+        "environmentId": str,
+    },
+)
+_OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef",
+    {
+        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
+        "customDNSConfiguration": Sequence[CustomDNSServerTypeDef],
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class UpdateKxEnvironmentNetworkRequestRequestTypeDef(
+    _RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef,
+    _OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef,
+):
+    pass
+
+
 GetEnvironmentResponseTypeDef = TypedDict(
     "GetEnvironmentResponseTypeDef",
     {
         "environment": EnvironmentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1208,107 +1370,107 @@
     {
         "environments": List[KxEnvironmentTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateKxClusterRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKxClusterRequestRequestTypeDef",
+CreateKxClusterResponseTypeDef = TypedDict(
+    "CreateKxClusterResponseTypeDef",
     {
         "environmentId": str,
+        "status": KxClusterStatusType,
+        "statusReason": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
-        "capacityConfiguration": CapacityConfigurationTypeDef,
-        "releaseLabel": str,
-        "azMode": KxAzModeType,
-    },
-)
-_OptionalCreateKxClusterRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKxClusterRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "databases": Sequence[KxDatabaseConfigurationTypeDef],
-        "cacheStorageConfigurations": Sequence[KxCacheStorageConfigurationTypeDef],
-        "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
+        "databases": List[KxDatabaseConfigurationOutputTypeDef],
+        "cacheStorageConfigurations": List[KxCacheStorageConfigurationOutputTypeDef],
+        "autoScalingConfiguration": AutoScalingConfigurationOutputTypeDef,
         "clusterDescription": str,
-        "vpcConfiguration": VpcConfigurationTypeDef,
+        "capacityConfiguration": CapacityConfigurationOutputTypeDef,
+        "releaseLabel": str,
+        "vpcConfiguration": VpcConfigurationOutputTypeDef,
         "initializationScript": str,
-        "commandLineArguments": Sequence[KxCommandLineArgumentTypeDef],
-        "code": CodeConfigurationTypeDef,
+        "commandLineArguments": List[KxCommandLineArgumentOutputTypeDef],
+        "code": CodeConfigurationOutputTypeDef,
         "executionRole": str,
-        "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
+        "lastModifiedTimestamp": datetime,
+        "savedownStorageConfiguration": KxSavedownStorageConfigurationOutputTypeDef,
+        "azMode": KxAzModeType,
         "availabilityZoneId": str,
-        "tags": Mapping[str, str],
+        "createdTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class CreateKxClusterRequestRequestTypeDef(
-    _RequiredCreateKxClusterRequestRequestTypeDef, _OptionalCreateKxClusterRequestRequestTypeDef
-):
-    pass
-
-
-CreateKxClusterResponseTypeDef = TypedDict(
-    "CreateKxClusterResponseTypeDef",
+GetKxClusterResponseTypeDef = TypedDict(
+    "GetKxClusterResponseTypeDef",
     {
-        "environmentId": str,
         "status": KxClusterStatusType,
         "statusReason": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
-        "databases": List[KxDatabaseConfigurationTypeDef],
-        "cacheStorageConfigurations": List[KxCacheStorageConfigurationTypeDef],
-        "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
+        "databases": List[KxDatabaseConfigurationOutputTypeDef],
+        "cacheStorageConfigurations": List[KxCacheStorageConfigurationOutputTypeDef],
+        "autoScalingConfiguration": AutoScalingConfigurationOutputTypeDef,
         "clusterDescription": str,
-        "capacityConfiguration": CapacityConfigurationTypeDef,
+        "capacityConfiguration": CapacityConfigurationOutputTypeDef,
         "releaseLabel": str,
-        "vpcConfiguration": VpcConfigurationTypeDef,
+        "vpcConfiguration": VpcConfigurationOutputTypeDef,
         "initializationScript": str,
-        "commandLineArguments": List[KxCommandLineArgumentTypeDef],
-        "code": CodeConfigurationTypeDef,
+        "commandLineArguments": List[KxCommandLineArgumentOutputTypeDef],
+        "code": CodeConfigurationOutputTypeDef,
         "executionRole": str,
         "lastModifiedTimestamp": datetime,
-        "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
+        "savedownStorageConfiguration": KxSavedownStorageConfigurationOutputTypeDef,
         "azMode": KxAzModeType,
         "availabilityZoneId": str,
         "createdTimestamp": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetKxClusterResponseTypeDef = TypedDict(
-    "GetKxClusterResponseTypeDef",
+_RequiredCreateKxClusterRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKxClusterRequestRequestTypeDef",
     {
-        "status": KxClusterStatusType,
-        "statusReason": str,
+        "environmentId": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
-        "databases": List[KxDatabaseConfigurationTypeDef],
-        "cacheStorageConfigurations": List[KxCacheStorageConfigurationTypeDef],
-        "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
-        "clusterDescription": str,
         "capacityConfiguration": CapacityConfigurationTypeDef,
         "releaseLabel": str,
+        "azMode": KxAzModeType,
+    },
+)
+_OptionalCreateKxClusterRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKxClusterRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "databases": Sequence[KxDatabaseConfigurationTypeDef],
+        "cacheStorageConfigurations": Sequence[KxCacheStorageConfigurationTypeDef],
+        "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
+        "clusterDescription": str,
         "vpcConfiguration": VpcConfigurationTypeDef,
         "initializationScript": str,
-        "commandLineArguments": List[KxCommandLineArgumentTypeDef],
+        "commandLineArguments": Sequence[KxCommandLineArgumentTypeDef],
         "code": CodeConfigurationTypeDef,
         "executionRole": str,
-        "lastModifiedTimestamp": datetime,
         "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
-        "azMode": KxAzModeType,
         "availabilityZoneId": str,
-        "createdTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": Mapping[str, str],
     },
+    total=False,
 )
 
+
+class CreateKxClusterRequestRequestTypeDef(
+    _RequiredCreateKxClusterRequestRequestTypeDef, _OptionalCreateKxClusterRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredUpdateKxClusterDatabasesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "environmentId": str,
         "clusterName": str,
         "databases": Sequence[KxDatabaseConfigurationTypeDef],
     },
```

### Comparing `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/type_defs.pyi` & `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for finspace service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_finspace.type_defs import AutoScalingConfigurationTypeDef
+    from mypy_boto3_finspace.type_defs import AutoScalingConfigurationOutputTypeDef
 
-    data: AutoScalingConfigurationTypeDef = {...}
+    data: AutoScalingConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -34,51 +34,62 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AutoScalingConfigurationOutputTypeDef",
     "AutoScalingConfigurationTypeDef",
+    "CapacityConfigurationOutputTypeDef",
     "CapacityConfigurationTypeDef",
+    "ChangeRequestOutputTypeDef",
     "ChangeRequestTypeDef",
+    "CodeConfigurationOutputTypeDef",
     "CodeConfigurationTypeDef",
     "FederationParametersTypeDef",
     "SuperuserParametersTypeDef",
     "CreateEnvironmentResponseTypeDef",
     "ErrorInfoTypeDef",
     "KxCacheStorageConfigurationTypeDef",
     "KxCommandLineArgumentTypeDef",
     "KxSavedownStorageConfigurationTypeDef",
     "VpcConfigurationTypeDef",
+    "KxCacheStorageConfigurationOutputTypeDef",
+    "KxCommandLineArgumentOutputTypeDef",
+    "KxSavedownStorageConfigurationOutputTypeDef",
+    "VpcConfigurationOutputTypeDef",
     "CreateKxDatabaseRequestRequestTypeDef",
     "CreateKxDatabaseResponseTypeDef",
     "CreateKxEnvironmentRequestRequestTypeDef",
     "CreateKxEnvironmentResponseTypeDef",
     "CreateKxUserRequestRequestTypeDef",
     "CreateKxUserResponseTypeDef",
+    "CustomDNSServerOutputTypeDef",
     "CustomDNSServerTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteKxClusterRequestRequestTypeDef",
     "DeleteKxDatabaseRequestRequestTypeDef",
     "DeleteKxEnvironmentRequestRequestTypeDef",
     "DeleteKxUserRequestRequestTypeDef",
+    "FederationParametersOutputTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetKxChangesetRequestRequestTypeDef",
     "GetKxClusterRequestRequestTypeDef",
     "GetKxConnectionStringRequestRequestTypeDef",
     "GetKxConnectionStringResponseTypeDef",
     "GetKxDatabaseRequestRequestTypeDef",
     "GetKxDatabaseResponseTypeDef",
     "GetKxEnvironmentRequestRequestTypeDef",
-    "TransitGatewayConfigurationTypeDef",
+    "TransitGatewayConfigurationOutputTypeDef",
     "GetKxUserRequestRequestTypeDef",
     "GetKxUserResponseTypeDef",
     "KxChangesetListEntryTypeDef",
     "KxClusterTypeDef",
+    "KxDatabaseCacheConfigurationOutputTypeDef",
     "KxDatabaseCacheConfigurationTypeDef",
     "KxDatabaseListEntryTypeDef",
     "KxNodeTypeDef",
     "KxUserTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListKxChangesetsRequestRequestTypeDef",
     "ListKxClusterNodesRequestRequestTypeDef",
@@ -88,69 +99,113 @@
     "ListKxEnvironmentsRequestRequestTypeDef",
     "ListKxUsersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "TransitGatewayConfigurationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateKxDatabaseRequestRequestTypeDef",
     "UpdateKxDatabaseResponseTypeDef",
     "UpdateKxEnvironmentRequestRequestTypeDef",
     "UpdateKxUserRequestRequestTypeDef",
     "UpdateKxUserResponseTypeDef",
     "CreateKxChangesetRequestRequestTypeDef",
-    "EnvironmentTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
     "CreateKxChangesetResponseTypeDef",
     "GetKxChangesetResponseTypeDef",
+    "EnvironmentTypeDef",
     "GetKxEnvironmentResponseTypeDef",
     "KxEnvironmentTypeDef",
-    "UpdateKxEnvironmentNetworkRequestRequestTypeDef",
     "UpdateKxEnvironmentNetworkResponseTypeDef",
     "UpdateKxEnvironmentResponseTypeDef",
     "ListKxChangesetsResponseTypeDef",
     "ListKxClustersResponseTypeDef",
+    "KxDatabaseConfigurationOutputTypeDef",
     "KxDatabaseConfigurationTypeDef",
     "ListKxDatabasesResponseTypeDef",
     "ListKxClusterNodesResponseTypeDef",
     "ListKxUsersResponseTypeDef",
+    "UpdateKxEnvironmentNetworkRequestRequestTypeDef",
     "GetEnvironmentResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "UpdateEnvironmentResponseTypeDef",
     "ListKxEnvironmentsResponseTypeDef",
-    "CreateKxClusterRequestRequestTypeDef",
     "CreateKxClusterResponseTypeDef",
     "GetKxClusterResponseTypeDef",
+    "CreateKxClusterRequestRequestTypeDef",
     "UpdateKxClusterDatabasesRequestRequestTypeDef",
 )
 
+AutoScalingConfigurationOutputTypeDef = TypedDict(
+    "AutoScalingConfigurationOutputTypeDef",
+    {
+        "minNodeCount": int,
+        "maxNodeCount": int,
+        "autoScalingMetric": Literal["CPU_UTILIZATION_PERCENTAGE"],
+        "metricTarget": float,
+        "scaleInCooldownSeconds": float,
+        "scaleOutCooldownSeconds": float,
+    },
+    total=False,
+)
+
 AutoScalingConfigurationTypeDef = TypedDict(
     "AutoScalingConfigurationTypeDef",
     {
         "minNodeCount": int,
         "maxNodeCount": int,
         "autoScalingMetric": Literal["CPU_UTILIZATION_PERCENTAGE"],
         "metricTarget": float,
         "scaleInCooldownSeconds": float,
         "scaleOutCooldownSeconds": float,
     },
     total=False,
 )
 
+CapacityConfigurationOutputTypeDef = TypedDict(
+    "CapacityConfigurationOutputTypeDef",
+    {
+        "nodeType": str,
+        "nodeCount": int,
+    },
+    total=False,
+)
+
 CapacityConfigurationTypeDef = TypedDict(
     "CapacityConfigurationTypeDef",
     {
         "nodeType": str,
         "nodeCount": int,
     },
     total=False,
 )
 
+_RequiredChangeRequestOutputTypeDef = TypedDict(
+    "_RequiredChangeRequestOutputTypeDef",
+    {
+        "changeType": ChangeTypeType,
+        "dbPath": str,
+    },
+)
+_OptionalChangeRequestOutputTypeDef = TypedDict(
+    "_OptionalChangeRequestOutputTypeDef",
+    {
+        "s3Path": str,
+    },
+    total=False,
+)
+
+class ChangeRequestOutputTypeDef(
+    _RequiredChangeRequestOutputTypeDef, _OptionalChangeRequestOutputTypeDef
+):
+    pass
+
 _RequiredChangeRequestTypeDef = TypedDict(
     "_RequiredChangeRequestTypeDef",
     {
         "changeType": ChangeTypeType,
         "dbPath": str,
     },
 )
@@ -161,14 +216,24 @@
     },
     total=False,
 )
 
 class ChangeRequestTypeDef(_RequiredChangeRequestTypeDef, _OptionalChangeRequestTypeDef):
     pass
 
+CodeConfigurationOutputTypeDef = TypedDict(
+    "CodeConfigurationOutputTypeDef",
+    {
+        "s3Bucket": str,
+        "s3Key": str,
+        "s3ObjectVersion": str,
+    },
+    total=False,
+)
+
 CodeConfigurationTypeDef = TypedDict(
     "CodeConfigurationTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
         "s3ObjectVersion": str,
     },
@@ -248,14 +313,50 @@
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
         "ipAddressType": Literal["IP_V4"],
     },
     total=False,
 )
 
+KxCacheStorageConfigurationOutputTypeDef = TypedDict(
+    "KxCacheStorageConfigurationOutputTypeDef",
+    {
+        "type": str,
+        "size": int,
+    },
+)
+
+KxCommandLineArgumentOutputTypeDef = TypedDict(
+    "KxCommandLineArgumentOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+    total=False,
+)
+
+KxSavedownStorageConfigurationOutputTypeDef = TypedDict(
+    "KxSavedownStorageConfigurationOutputTypeDef",
+    {
+        "type": Literal["SDS01"],
+        "size": int,
+    },
+)
+
+VpcConfigurationOutputTypeDef = TypedDict(
+    "VpcConfigurationOutputTypeDef",
+    {
+        "vpcId": str,
+        "securityGroupIds": List[str],
+        "subnetIds": List[str],
+        "ipAddressType": Literal["IP_V4"],
+    },
+    total=False,
+)
+
 _RequiredCreateKxDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxDatabaseRequestRequestTypeDef",
     {
         "environmentId": str,
         "databaseName": str,
         "clientToken": str,
     },
@@ -353,14 +454,22 @@
         "userArn": str,
         "environmentId": str,
         "iamRole": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CustomDNSServerOutputTypeDef = TypedDict(
+    "CustomDNSServerOutputTypeDef",
+    {
+        "customDNSServerName": str,
+        "customDNSServerIP": str,
+    },
+)
+
 CustomDNSServerTypeDef = TypedDict(
     "CustomDNSServerTypeDef",
     {
         "customDNSServerName": str,
         "customDNSServerIP": str,
     },
 )
@@ -412,14 +521,27 @@
     "DeleteKxUserRequestRequestTypeDef",
     {
         "userName": str,
         "environmentId": str,
     },
 )
 
+FederationParametersOutputTypeDef = TypedDict(
+    "FederationParametersOutputTypeDef",
+    {
+        "samlMetadataDocument": str,
+        "samlMetadataURL": str,
+        "applicationCallBackURL": str,
+        "federationURN": str,
+        "federationProviderName": str,
+        "attributeMap": Dict[str, str],
+    },
+    total=False,
+)
+
 GetEnvironmentRequestRequestTypeDef = TypedDict(
     "GetEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
@@ -485,16 +607,16 @@
 GetKxEnvironmentRequestRequestTypeDef = TypedDict(
     "GetKxEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-TransitGatewayConfigurationTypeDef = TypedDict(
-    "TransitGatewayConfigurationTypeDef",
+TransitGatewayConfigurationOutputTypeDef = TypedDict(
+    "TransitGatewayConfigurationOutputTypeDef",
     {
         "transitGatewayID": str,
         "routableCIDRSpace": str,
     },
 )
 
 GetKxUserRequestRequestTypeDef = TypedDict(
@@ -543,14 +665,22 @@
         "availabilityZoneId": str,
         "lastModifiedTimestamp": datetime,
         "createdTimestamp": datetime,
     },
     total=False,
 )
 
+KxDatabaseCacheConfigurationOutputTypeDef = TypedDict(
+    "KxDatabaseCacheConfigurationOutputTypeDef",
+    {
+        "cacheType": str,
+        "dbPaths": List[str],
+    },
+)
+
 KxDatabaseCacheConfigurationTypeDef = TypedDict(
     "KxDatabaseCacheConfigurationTypeDef",
     {
         "cacheType": str,
         "dbPaths": Sequence[str],
     },
 )
@@ -757,14 +887,22 @@
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
 
+TransitGatewayConfigurationTypeDef = TypedDict(
+    "TransitGatewayConfigurationTypeDef",
+    {
+        "transitGatewayID": str,
+        "routableCIDRSpace": str,
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -861,33 +999,14 @@
         "environmentId": str,
         "databaseName": str,
         "changeRequests": Sequence[ChangeRequestTypeDef],
         "clientToken": str,
     },
 )
 
-EnvironmentTypeDef = TypedDict(
-    "EnvironmentTypeDef",
-    {
-        "name": str,
-        "environmentId": str,
-        "awsAccountId": str,
-        "status": EnvironmentStatusType,
-        "environmentUrl": str,
-        "description": str,
-        "environmentArn": str,
-        "sageMakerStudioDomainUrl": str,
-        "kmsKeyId": str,
-        "dedicatedServiceAccountId": str,
-        "federationMode": FederationModeType,
-        "federationParameters": FederationParametersTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 _OptionalUpdateEnvironmentRequestRequestTypeDef = TypedDict(
@@ -933,55 +1052,74 @@
 
 CreateKxChangesetResponseTypeDef = TypedDict(
     "CreateKxChangesetResponseTypeDef",
     {
         "changesetId": str,
         "databaseName": str,
         "environmentId": str,
-        "changeRequests": List[ChangeRequestTypeDef],
+        "changeRequests": List[ChangeRequestOutputTypeDef],
         "createdTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
         "status": ChangesetStatusType,
         "errorInfo": ErrorInfoTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetKxChangesetResponseTypeDef = TypedDict(
     "GetKxChangesetResponseTypeDef",
     {
         "changesetId": str,
         "databaseName": str,
         "environmentId": str,
-        "changeRequests": List[ChangeRequestTypeDef],
+        "changeRequests": List[ChangeRequestOutputTypeDef],
         "createdTimestamp": datetime,
         "activeFromTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
         "status": ChangesetStatusType,
         "errorInfo": ErrorInfoTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EnvironmentTypeDef = TypedDict(
+    "EnvironmentTypeDef",
+    {
+        "name": str,
+        "environmentId": str,
+        "awsAccountId": str,
+        "status": EnvironmentStatusType,
+        "environmentUrl": str,
+        "description": str,
+        "environmentArn": str,
+        "sageMakerStudioDomainUrl": str,
+        "kmsKeyId": str,
+        "dedicatedServiceAccountId": str,
+        "federationMode": FederationModeType,
+        "federationParameters": FederationParametersOutputTypeDef,
+    },
+    total=False,
+)
+
 GetKxEnvironmentResponseTypeDef = TypedDict(
     "GetKxEnvironmentResponseTypeDef",
     {
         "name": str,
         "environmentId": str,
         "awsAccountId": str,
         "status": EnvironmentStatusType,
         "tgwStatus": tgwStatusType,
         "dnsStatus": dnsStatusType,
         "errorMessage": str,
         "description": str,
         "environmentArn": str,
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
-        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
-        "customDNSConfiguration": List[CustomDNSServerTypeDef],
+        "transitGatewayConfiguration": TransitGatewayConfigurationOutputTypeDef,
+        "customDNSConfiguration": List[CustomDNSServerOutputTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
         "certificateAuthorityArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -996,62 +1134,40 @@
         "tgwStatus": tgwStatusType,
         "dnsStatus": dnsStatusType,
         "errorMessage": str,
         "description": str,
         "environmentArn": str,
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
-        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
-        "customDNSConfiguration": List[CustomDNSServerTypeDef],
+        "transitGatewayConfiguration": TransitGatewayConfigurationOutputTypeDef,
+        "customDNSConfiguration": List[CustomDNSServerOutputTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
         "certificateAuthorityArn": str,
     },
     total=False,
 )
 
-_RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef",
-    {
-        "environmentId": str,
-    },
-)
-_OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef",
-    {
-        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
-        "customDNSConfiguration": Sequence[CustomDNSServerTypeDef],
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class UpdateKxEnvironmentNetworkRequestRequestTypeDef(
-    _RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef,
-    _OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef,
-):
-    pass
-
 UpdateKxEnvironmentNetworkResponseTypeDef = TypedDict(
     "UpdateKxEnvironmentNetworkResponseTypeDef",
     {
         "name": str,
         "environmentId": str,
         "awsAccountId": str,
         "status": EnvironmentStatusType,
         "tgwStatus": tgwStatusType,
         "dnsStatus": dnsStatusType,
         "errorMessage": str,
         "description": str,
         "environmentArn": str,
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
-        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
-        "customDNSConfiguration": List[CustomDNSServerTypeDef],
+        "transitGatewayConfiguration": TransitGatewayConfigurationOutputTypeDef,
+        "customDNSConfiguration": List[CustomDNSServerOutputTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1065,16 +1181,16 @@
         "tgwStatus": tgwStatusType,
         "dnsStatus": dnsStatusType,
         "errorMessage": str,
         "description": str,
         "environmentArn": str,
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
-        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
-        "customDNSConfiguration": List[CustomDNSServerTypeDef],
+        "transitGatewayConfiguration": TransitGatewayConfigurationOutputTypeDef,
+        "customDNSConfiguration": List[CustomDNSServerOutputTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1092,14 +1208,34 @@
     {
         "kxClusterSummaries": List[KxClusterTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredKxDatabaseConfigurationOutputTypeDef = TypedDict(
+    "_RequiredKxDatabaseConfigurationOutputTypeDef",
+    {
+        "databaseName": str,
+    },
+)
+_OptionalKxDatabaseConfigurationOutputTypeDef = TypedDict(
+    "_OptionalKxDatabaseConfigurationOutputTypeDef",
+    {
+        "cacheConfigurations": List[KxDatabaseCacheConfigurationOutputTypeDef],
+        "changesetId": str,
+    },
+    total=False,
+)
+
+class KxDatabaseConfigurationOutputTypeDef(
+    _RequiredKxDatabaseConfigurationOutputTypeDef, _OptionalKxDatabaseConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredKxDatabaseConfigurationTypeDef = TypedDict(
     "_RequiredKxDatabaseConfigurationTypeDef",
     {
         "databaseName": str,
     },
 )
 _OptionalKxDatabaseConfigurationTypeDef = TypedDict(
@@ -1139,14 +1275,36 @@
     {
         "users": List[KxUserTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef",
+    {
+        "environmentId": str,
+    },
+)
+_OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef",
+    {
+        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
+        "customDNSConfiguration": Sequence[CustomDNSServerTypeDef],
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class UpdateKxEnvironmentNetworkRequestRequestTypeDef(
+    _RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef,
+    _OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef,
+):
+    pass
+
 GetEnvironmentResponseTypeDef = TypedDict(
     "GetEnvironmentResponseTypeDef",
     {
         "environment": EnvironmentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1173,105 +1331,105 @@
     {
         "environments": List[KxEnvironmentTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateKxClusterRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKxClusterRequestRequestTypeDef",
+CreateKxClusterResponseTypeDef = TypedDict(
+    "CreateKxClusterResponseTypeDef",
     {
         "environmentId": str,
+        "status": KxClusterStatusType,
+        "statusReason": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
-        "capacityConfiguration": CapacityConfigurationTypeDef,
-        "releaseLabel": str,
-        "azMode": KxAzModeType,
-    },
-)
-_OptionalCreateKxClusterRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKxClusterRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "databases": Sequence[KxDatabaseConfigurationTypeDef],
-        "cacheStorageConfigurations": Sequence[KxCacheStorageConfigurationTypeDef],
-        "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
+        "databases": List[KxDatabaseConfigurationOutputTypeDef],
+        "cacheStorageConfigurations": List[KxCacheStorageConfigurationOutputTypeDef],
+        "autoScalingConfiguration": AutoScalingConfigurationOutputTypeDef,
         "clusterDescription": str,
-        "vpcConfiguration": VpcConfigurationTypeDef,
+        "capacityConfiguration": CapacityConfigurationOutputTypeDef,
+        "releaseLabel": str,
+        "vpcConfiguration": VpcConfigurationOutputTypeDef,
         "initializationScript": str,
-        "commandLineArguments": Sequence[KxCommandLineArgumentTypeDef],
-        "code": CodeConfigurationTypeDef,
+        "commandLineArguments": List[KxCommandLineArgumentOutputTypeDef],
+        "code": CodeConfigurationOutputTypeDef,
         "executionRole": str,
-        "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
+        "lastModifiedTimestamp": datetime,
+        "savedownStorageConfiguration": KxSavedownStorageConfigurationOutputTypeDef,
+        "azMode": KxAzModeType,
         "availabilityZoneId": str,
-        "tags": Mapping[str, str],
+        "createdTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class CreateKxClusterRequestRequestTypeDef(
-    _RequiredCreateKxClusterRequestRequestTypeDef, _OptionalCreateKxClusterRequestRequestTypeDef
-):
-    pass
-
-CreateKxClusterResponseTypeDef = TypedDict(
-    "CreateKxClusterResponseTypeDef",
+GetKxClusterResponseTypeDef = TypedDict(
+    "GetKxClusterResponseTypeDef",
     {
-        "environmentId": str,
         "status": KxClusterStatusType,
         "statusReason": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
-        "databases": List[KxDatabaseConfigurationTypeDef],
-        "cacheStorageConfigurations": List[KxCacheStorageConfigurationTypeDef],
-        "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
+        "databases": List[KxDatabaseConfigurationOutputTypeDef],
+        "cacheStorageConfigurations": List[KxCacheStorageConfigurationOutputTypeDef],
+        "autoScalingConfiguration": AutoScalingConfigurationOutputTypeDef,
         "clusterDescription": str,
-        "capacityConfiguration": CapacityConfigurationTypeDef,
+        "capacityConfiguration": CapacityConfigurationOutputTypeDef,
         "releaseLabel": str,
-        "vpcConfiguration": VpcConfigurationTypeDef,
+        "vpcConfiguration": VpcConfigurationOutputTypeDef,
         "initializationScript": str,
-        "commandLineArguments": List[KxCommandLineArgumentTypeDef],
-        "code": CodeConfigurationTypeDef,
+        "commandLineArguments": List[KxCommandLineArgumentOutputTypeDef],
+        "code": CodeConfigurationOutputTypeDef,
         "executionRole": str,
         "lastModifiedTimestamp": datetime,
-        "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
+        "savedownStorageConfiguration": KxSavedownStorageConfigurationOutputTypeDef,
         "azMode": KxAzModeType,
         "availabilityZoneId": str,
         "createdTimestamp": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetKxClusterResponseTypeDef = TypedDict(
-    "GetKxClusterResponseTypeDef",
+_RequiredCreateKxClusterRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKxClusterRequestRequestTypeDef",
     {
-        "status": KxClusterStatusType,
-        "statusReason": str,
+        "environmentId": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
-        "databases": List[KxDatabaseConfigurationTypeDef],
-        "cacheStorageConfigurations": List[KxCacheStorageConfigurationTypeDef],
-        "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
-        "clusterDescription": str,
         "capacityConfiguration": CapacityConfigurationTypeDef,
         "releaseLabel": str,
+        "azMode": KxAzModeType,
+    },
+)
+_OptionalCreateKxClusterRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKxClusterRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "databases": Sequence[KxDatabaseConfigurationTypeDef],
+        "cacheStorageConfigurations": Sequence[KxCacheStorageConfigurationTypeDef],
+        "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
+        "clusterDescription": str,
         "vpcConfiguration": VpcConfigurationTypeDef,
         "initializationScript": str,
-        "commandLineArguments": List[KxCommandLineArgumentTypeDef],
+        "commandLineArguments": Sequence[KxCommandLineArgumentTypeDef],
         "code": CodeConfigurationTypeDef,
         "executionRole": str,
-        "lastModifiedTimestamp": datetime,
         "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
-        "azMode": KxAzModeType,
         "availabilityZoneId": str,
-        "createdTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": Mapping[str, str],
     },
+    total=False,
 )
 
+class CreateKxClusterRequestRequestTypeDef(
+    _RequiredCreateKxClusterRequestRequestTypeDef, _OptionalCreateKxClusterRequestRequestTypeDef
+):
+    pass
+
 _RequiredUpdateKxClusterDatabasesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "environmentId": str,
         "clusterName": str,
         "databases": Sequence[KxDatabaseConfigurationTypeDef],
     },
```

### Comparing `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace.egg-info/PKG-INFO` & `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-finspace
-Version: 1.28.0
-Summary: Type annotations for boto3.finspace 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.finspace 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-finspace"></a>
 
 # mypy-boto3-finspace
 
 [![PyPI - mypy-boto3-finspace](https://img.shields.io/pypi/v/mypy-boto3-finspace.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-finspace?color=blue)](https://pypistats.org/packages/mypy-boto3-finspace)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-finspace)](https://pepy.tech/project/mypy-boto3-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.finspace 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
+[boto3.finspace 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
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
 [mypy-boto3-finspace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,51 +333,62 @@
 ### Typed dictionaries
 
 `mypy_boto3_finspace.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_finspace.type_defs import (
+    AutoScalingConfigurationOutputTypeDef,
     AutoScalingConfigurationTypeDef,
+    CapacityConfigurationOutputTypeDef,
     CapacityConfigurationTypeDef,
+    ChangeRequestOutputTypeDef,
     ChangeRequestTypeDef,
+    CodeConfigurationOutputTypeDef,
     CodeConfigurationTypeDef,
     FederationParametersTypeDef,
     SuperuserParametersTypeDef,
     CreateEnvironmentResponseTypeDef,
     ErrorInfoTypeDef,
     KxCacheStorageConfigurationTypeDef,
     KxCommandLineArgumentTypeDef,
     KxSavedownStorageConfigurationTypeDef,
     VpcConfigurationTypeDef,
+    KxCacheStorageConfigurationOutputTypeDef,
+    KxCommandLineArgumentOutputTypeDef,
+    KxSavedownStorageConfigurationOutputTypeDef,
+    VpcConfigurationOutputTypeDef,
     CreateKxDatabaseRequestRequestTypeDef,
     CreateKxDatabaseResponseTypeDef,
     CreateKxEnvironmentRequestRequestTypeDef,
     CreateKxEnvironmentResponseTypeDef,
     CreateKxUserRequestRequestTypeDef,
     CreateKxUserResponseTypeDef,
+    CustomDNSServerOutputTypeDef,
     CustomDNSServerTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteKxClusterRequestRequestTypeDef,
     DeleteKxDatabaseRequestRequestTypeDef,
     DeleteKxEnvironmentRequestRequestTypeDef,
     DeleteKxUserRequestRequestTypeDef,
+    FederationParametersOutputTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetKxChangesetRequestRequestTypeDef,
     GetKxClusterRequestRequestTypeDef,
     GetKxConnectionStringRequestRequestTypeDef,
     GetKxConnectionStringResponseTypeDef,
     GetKxDatabaseRequestRequestTypeDef,
     GetKxDatabaseResponseTypeDef,
     GetKxEnvironmentRequestRequestTypeDef,
-    TransitGatewayConfigurationTypeDef,
+    TransitGatewayConfigurationOutputTypeDef,
     GetKxUserRequestRequestTypeDef,
     GetKxUserResponseTypeDef,
     KxChangesetListEntryTypeDef,
     KxClusterTypeDef,
+    KxDatabaseCacheConfigurationOutputTypeDef,
     KxDatabaseCacheConfigurationTypeDef,
     KxDatabaseListEntryTypeDef,
     KxNodeTypeDef,
     KxUserTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListKxChangesetsRequestRequestTypeDef,
     ListKxClusterNodesRequestRequestTypeDef,
@@ -387,49 +398,51 @@
     ListKxEnvironmentsRequestRequestTypeDef,
     ListKxUsersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
+    TransitGatewayConfigurationTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateKxDatabaseRequestRequestTypeDef,
     UpdateKxDatabaseResponseTypeDef,
     UpdateKxEnvironmentRequestRequestTypeDef,
     UpdateKxUserRequestRequestTypeDef,
     UpdateKxUserResponseTypeDef,
     CreateKxChangesetRequestRequestTypeDef,
-    EnvironmentTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
     CreateKxChangesetResponseTypeDef,
     GetKxChangesetResponseTypeDef,
+    EnvironmentTypeDef,
     GetKxEnvironmentResponseTypeDef,
     KxEnvironmentTypeDef,
-    UpdateKxEnvironmentNetworkRequestRequestTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClustersResponseTypeDef,
+    KxDatabaseConfigurationOutputTypeDef,
     KxDatabaseConfigurationTypeDef,
     ListKxDatabasesResponseTypeDef,
     ListKxClusterNodesResponseTypeDef,
     ListKxUsersResponseTypeDef,
+    UpdateKxEnvironmentNetworkRequestRequestTypeDef,
     GetEnvironmentResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
     ListKxEnvironmentsResponseTypeDef,
-    CreateKxClusterRequestRequestTypeDef,
     CreateKxClusterResponseTypeDef,
     GetKxClusterResponseTypeDef,
+    CreateKxClusterRequestRequestTypeDef,
     UpdateKxClusterDatabasesRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AutoScalingConfigurationTypeDef:
+def get_structure() -> AutoScalingConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace.egg-info/SOURCES.txt` & `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.0/setup.py` & `mypy-boto3-finspace-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-finspace",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_finspace"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.finspace 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.finspace 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

