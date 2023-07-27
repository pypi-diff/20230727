# Comparing `tmp/mypy-boto3-opsworkscm-1.28.0.tar.gz` & `tmp/mypy-boto3-opsworkscm-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-opsworkscm-1.28.0.tar", last modified: Thu Jul  6 21:00:15 2023, max compression
+gzip compressed data, was "mypy-boto3-opsworkscm-1.28.12.tar", last modified: Thu Jul 27 11:49:21 2023, max compression
```

## Comparing `mypy-boto3-opsworkscm-1.28.0.tar` & `mypy-boto3-opsworkscm-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:15.014385 mypy-boto3-opsworkscm-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:48:50.000000 mypy-boto3-opsworkscm-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-07-06 21:00:15.014385 mypy-boto3-opsworkscm-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-07-06 20:48:50.000000 mypy-boto3-opsworkscm-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:15.010385 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-06 20:48:50.000000 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-06 20:48:50.000000 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 20:48:50.000000 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17657 2023-07-06 20:48:50.000000 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17626 2023-07-06 20:48:50.000000 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-07-06 20:48:50.000000 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-07-06 20:48:50.000000 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-06 20:48:50.000000 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-07-06 20:48:50.000000 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:48:50.000000 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18796 2023-07-06 20:48:51.000000 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18769 2023-07-06 20:48:50.000000 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:48:50.000000 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-06 20:48:50.000000 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-06 20:48:50.000000 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:15.014385 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-07-06 21:00:14.000000 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-06 21:00:14.000000 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:14.000000 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:14.000000 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:14.000000 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 21:00:14.000000 mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:15.014385 mypy-boto3-opsworkscm-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:48:49.000000 mypy-boto3-opsworkscm-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.801132 mypy-boto3-opsworkscm-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-07-27 11:49:21.801132 mypy-boto3-opsworkscm-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.801132 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17657 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17626 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19108 2023-07-27 11:41:04.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19081 2023-07-27 11:41:04.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.801132 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-07-27 11:49:21.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-27 11:49:21.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:21.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 11:49:21.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:21.801132 mypy-boto3-opsworkscm-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/setup.py
```

### Comparing `mypy-boto3-opsworkscm-1.28.0/LICENSE` & `mypy-boto3-opsworkscm-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.0/PKG-INFO` & `mypy-boto3-opsworkscm-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opsworkscm
-Version: 1.28.0
-Summary: Type annotations for boto3.OpsWorksCM 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.OpsWorksCM 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-opsworkscm"></a>
 
 # mypy-boto3-opsworkscm
 
 [![PyPI - mypy-boto3-opsworkscm](https://img.shields.io/pypi/v/mypy-boto3-opsworkscm.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworkscm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworkscm.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworkscm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opsworkscm?color=blue)](https://pypistats.org/packages/mypy-boto3-opsworkscm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opsworkscm)](https://pepy.tech/project/mypy-boto3-opsworkscm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorksCM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
+[boto3.OpsWorksCM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
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
 [mypy-boto3-opsworkscm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -361,53 +361,55 @@
 `mypy_boto3_opsworkscm.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opsworkscm.type_defs import (
     AccountAttributeTypeDef,
     EngineAttributeTypeDef,
-    AssociateNodeResponseTypeDef,
+    ResponseMetadataTypeDef,
     BackupTypeDef,
     TagTypeDef,
     DeleteBackupRequestRequestTypeDef,
     DeleteServerRequestRequestTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeBackupsRequestRequestTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     ServerEventTypeDef,
     WaiterConfigTypeDef,
     DescribeNodeAssociationStatusRequestRequestTypeDef,
-    DescribeServersRequestDescribeServersPaginateTypeDef,
+    EngineAttributeOutputTypeDef,
     DescribeServersRequestRequestTypeDef,
-    DisassociateNodeResponseTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    TagOutputTypeDef,
     RestoreServerRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateServerEngineAttributesRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
     AssociateNodeRequestRequestTypeDef,
-    DescribeNodeAssociationStatusResponseTypeDef,
     DisassociateNodeRequestRequestTypeDef,
     ExportServerEngineAttributeRequestRequestTypeDef,
-    ExportServerEngineAttributeResponseTypeDef,
-    ServerTypeDef,
     StartMaintenanceRequestRequestTypeDef,
+    AssociateNodeResponseTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
+    DisassociateNodeResponseTypeDef,
     CreateBackupResponseTypeDef,
     DescribeBackupsResponseTypeDef,
     CreateBackupRequestRequestTypeDef,
     CreateServerRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
+    DescribeServersRequestDescribeServersPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
+    DescribeNodeAssociationStatusResponseTypeDef,
+    ExportServerEngineAttributeResponseTypeDef,
+    ServerTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateServerResponseTypeDef,
     DescribeServersResponseTypeDef,
     RestoreServerResponseTypeDef,
     StartMaintenanceResponseTypeDef,
     UpdateServerEngineAttributesResponseTypeDef,
     UpdateServerResponseTypeDef,
 )
```

### Comparing `mypy-boto3-opsworkscm-1.28.0/README.md` & `mypy-boto3-opsworkscm-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-opsworkscm"></a>
 
 # mypy-boto3-opsworkscm
 
 [![PyPI - mypy-boto3-opsworkscm](https://img.shields.io/pypi/v/mypy-boto3-opsworkscm.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworkscm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworkscm.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworkscm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opsworkscm?color=blue)](https://pypistats.org/packages/mypy-boto3-opsworkscm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opsworkscm)](https://pepy.tech/project/mypy-boto3-opsworkscm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorksCM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
+[boto3.OpsWorksCM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
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
 [mypy-boto3-opsworkscm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,53 +329,55 @@
 `mypy_boto3_opsworkscm.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opsworkscm.type_defs import (
     AccountAttributeTypeDef,
     EngineAttributeTypeDef,
-    AssociateNodeResponseTypeDef,
+    ResponseMetadataTypeDef,
     BackupTypeDef,
     TagTypeDef,
     DeleteBackupRequestRequestTypeDef,
     DeleteServerRequestRequestTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeBackupsRequestRequestTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     ServerEventTypeDef,
     WaiterConfigTypeDef,
     DescribeNodeAssociationStatusRequestRequestTypeDef,
-    DescribeServersRequestDescribeServersPaginateTypeDef,
+    EngineAttributeOutputTypeDef,
     DescribeServersRequestRequestTypeDef,
-    DisassociateNodeResponseTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    TagOutputTypeDef,
     RestoreServerRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateServerEngineAttributesRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
     AssociateNodeRequestRequestTypeDef,
-    DescribeNodeAssociationStatusResponseTypeDef,
     DisassociateNodeRequestRequestTypeDef,
     ExportServerEngineAttributeRequestRequestTypeDef,
-    ExportServerEngineAttributeResponseTypeDef,
-    ServerTypeDef,
     StartMaintenanceRequestRequestTypeDef,
+    AssociateNodeResponseTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
+    DisassociateNodeResponseTypeDef,
     CreateBackupResponseTypeDef,
     DescribeBackupsResponseTypeDef,
     CreateBackupRequestRequestTypeDef,
     CreateServerRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
+    DescribeServersRequestDescribeServersPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
+    DescribeNodeAssociationStatusResponseTypeDef,
+    ExportServerEngineAttributeResponseTypeDef,
+    ServerTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateServerResponseTypeDef,
     DescribeServersResponseTypeDef,
     RestoreServerResponseTypeDef,
     StartMaintenanceResponseTypeDef,
     UpdateServerEngineAttributesResponseTypeDef,
     UpdateServerResponseTypeDef,
 )
```

### Comparing `mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/__init__.py` & `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/__init__.pyi` & `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/__main__.py` & `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpsWorksCM 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.OpsWorksCM 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM\nOther"
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

### Comparing `mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/client.py` & `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/client.pyi` & `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/literals.py` & `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,14 +179,15 @@
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
@@ -265,26 +266,28 @@
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

### Comparing `mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/literals.pyi` & `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,15 @@
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
@@ -263,26 +264,28 @@
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

### Comparing `mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/paginator.py` & `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,58 +62,58 @@
     """
 
     def paginate(
         self,
         *,
         BackupId: str = ...,
         ServerName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#describebackupspaginator)
         """
 
 
 class DescribeEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#describeeventspaginator)
     """
 
     def paginate(
-        self, *, ServerName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#describeeventspaginator)
         """
 
 
 class DescribeServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#describeserverspaginator)
     """
 
     def paginate(
-        self, *, ServerName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#describeserverspaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/paginator.pyi` & `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -59,55 +59,55 @@
     """
 
     def paginate(
         self,
         *,
         BackupId: str = ...,
         ServerName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#describebackupspaginator)
         """
 
 class DescribeEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#describeeventspaginator)
     """
 
     def paginate(
-        self, *, ServerName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#describeeventspaginator)
         """
 
 class DescribeServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#describeserverspaginator)
     """
 
     def paginate(
-        self, *, ServerName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#describeserverspaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/type_defs.py` & `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,53 +28,55 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountAttributeTypeDef",
     "EngineAttributeTypeDef",
-    "AssociateNodeResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "BackupTypeDef",
     "TagTypeDef",
     "DeleteBackupRequestRequestTypeDef",
     "DeleteServerRequestRequestTypeDef",
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeEventsRequestRequestTypeDef",
     "ServerEventTypeDef",
     "WaiterConfigTypeDef",
     "DescribeNodeAssociationStatusRequestRequestTypeDef",
-    "DescribeServersRequestDescribeServersPaginateTypeDef",
+    "EngineAttributeOutputTypeDef",
     "DescribeServersRequestRequestTypeDef",
-    "DisassociateNodeResponseTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "TagOutputTypeDef",
     "RestoreServerRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateServerEngineAttributesRequestRequestTypeDef",
     "UpdateServerRequestRequestTypeDef",
-    "DescribeAccountAttributesResponseTypeDef",
     "AssociateNodeRequestRequestTypeDef",
-    "DescribeNodeAssociationStatusResponseTypeDef",
     "DisassociateNodeRequestRequestTypeDef",
     "ExportServerEngineAttributeRequestRequestTypeDef",
-    "ExportServerEngineAttributeResponseTypeDef",
-    "ServerTypeDef",
     "StartMaintenanceRequestRequestTypeDef",
+    "AssociateNodeResponseTypeDef",
+    "DescribeAccountAttributesResponseTypeDef",
+    "DisassociateNodeResponseTypeDef",
     "CreateBackupResponseTypeDef",
     "DescribeBackupsResponseTypeDef",
     "CreateBackupRequestRequestTypeDef",
     "CreateServerRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
+    "DescribeServersRequestDescribeServersPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "DescribeEventsResponseTypeDef",
     "DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef",
+    "DescribeNodeAssociationStatusResponseTypeDef",
+    "ExportServerEngineAttributeResponseTypeDef",
+    "ServerTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateServerResponseTypeDef",
     "DescribeServersResponseTypeDef",
     "RestoreServerResponseTypeDef",
     "StartMaintenanceResponseTypeDef",
     "UpdateServerEngineAttributesResponseTypeDef",
     "UpdateServerResponseTypeDef",
 )
@@ -94,19 +96,22 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-AssociateNodeResponseTypeDef = TypedDict(
-    "AssociateNodeResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "NodeAssociationStatusToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 BackupTypeDef = TypedDict(
     "BackupTypeDef",
     {
         "BackupArn": str,
@@ -155,20 +160,20 @@
 DeleteServerRequestRequestTypeDef = TypedDict(
     "DeleteServerRequestRequestTypeDef",
     {
         "ServerName": str,
     },
 )
 
-DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "BackupId": str,
-        "ServerName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeBackupsRequestRequestTypeDef = TypedDict(
     "DescribeBackupsRequestRequestTypeDef",
     {
@@ -176,36 +181,14 @@
         "ServerName": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "ServerName": str,
-    },
-)
-_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeEventsRequestDescribeEventsPaginateTypeDef(
-    _RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef,
-    _OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeEventsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEventsRequestRequestTypeDef",
     {
         "ServerName": str,
     },
 )
 _OptionalDescribeEventsRequestRequestTypeDef = TypedDict(
@@ -248,63 +231,33 @@
     "DescribeNodeAssociationStatusRequestRequestTypeDef",
     {
         "NodeAssociationStatusToken": str,
         "ServerName": str,
     },
 )
 
-DescribeServersRequestDescribeServersPaginateTypeDef = TypedDict(
-    "DescribeServersRequestDescribeServersPaginateTypeDef",
+EngineAttributeOutputTypeDef = TypedDict(
+    "EngineAttributeOutputTypeDef",
     {
-        "ServerName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "Name": str,
+        "Value": str,
     },
     total=False,
 )
 
 DescribeServersRequestRequestTypeDef = TypedDict(
     "DescribeServersRequestRequestTypeDef",
     {
         "ServerName": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-DisassociateNodeResponseTypeDef = TypedDict(
-    "DisassociateNodeResponseTypeDef",
-    {
-        "NodeAssociationStatusToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -320,32 +273,19 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
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
+        "Key": str,
+        "Value": str,
     },
 )
 
 _RequiredRestoreServerRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreServerRequestRequestTypeDef",
     {
         "BackupId": str,
@@ -419,40 +359,23 @@
 
 class UpdateServerRequestRequestTypeDef(
     _RequiredUpdateServerRequestRequestTypeDef, _OptionalUpdateServerRequestRequestTypeDef
 ):
     pass
 
 
-DescribeAccountAttributesResponseTypeDef = TypedDict(
-    "DescribeAccountAttributesResponseTypeDef",
-    {
-        "Attributes": List[AccountAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateNodeRequestRequestTypeDef = TypedDict(
     "AssociateNodeRequestRequestTypeDef",
     {
         "ServerName": str,
         "NodeName": str,
         "EngineAttributes": Sequence[EngineAttributeTypeDef],
     },
 )
 
-DescribeNodeAssociationStatusResponseTypeDef = TypedDict(
-    "DescribeNodeAssociationStatusResponseTypeDef",
-    {
-        "NodeAssociationStatus": NodeAssociationStatusType,
-        "EngineAttributes": List[EngineAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDisassociateNodeRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateNodeRequestRequestTypeDef",
     {
         "ServerName": str,
         "NodeName": str,
     },
 )
@@ -490,54 +413,14 @@
 class ExportServerEngineAttributeRequestRequestTypeDef(
     _RequiredExportServerEngineAttributeRequestRequestTypeDef,
     _OptionalExportServerEngineAttributeRequestRequestTypeDef,
 ):
     pass
 
 
-ExportServerEngineAttributeResponseTypeDef = TypedDict(
-    "ExportServerEngineAttributeResponseTypeDef",
-    {
-        "EngineAttribute": EngineAttributeTypeDef,
-        "ServerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ServerTypeDef = TypedDict(
-    "ServerTypeDef",
-    {
-        "AssociatePublicIpAddress": bool,
-        "BackupRetentionCount": int,
-        "ServerName": str,
-        "CreatedAt": datetime,
-        "CloudFormationStackArn": str,
-        "CustomDomain": str,
-        "DisableAutomatedBackup": bool,
-        "Endpoint": str,
-        "Engine": str,
-        "EngineModel": str,
-        "EngineAttributes": List[EngineAttributeTypeDef],
-        "EngineVersion": str,
-        "InstanceProfileArn": str,
-        "InstanceType": str,
-        "KeyPair": str,
-        "MaintenanceStatus": MaintenanceStatusType,
-        "PreferredMaintenanceWindow": str,
-        "PreferredBackupWindow": str,
-        "SecurityGroupIds": List[str],
-        "ServiceRoleArn": str,
-        "Status": ServerStatusType,
-        "StatusReason": str,
-        "SubnetIds": List[str],
-        "ServerArn": str,
-    },
-    total=False,
-)
-
 _RequiredStartMaintenanceRequestRequestTypeDef = TypedDict(
     "_RequiredStartMaintenanceRequestRequestTypeDef",
     {
         "ServerName": str,
     },
 )
 _OptionalStartMaintenanceRequestRequestTypeDef = TypedDict(
@@ -551,28 +434,52 @@
 
 class StartMaintenanceRequestRequestTypeDef(
     _RequiredStartMaintenanceRequestRequestTypeDef, _OptionalStartMaintenanceRequestRequestTypeDef
 ):
     pass
 
 
+AssociateNodeResponseTypeDef = TypedDict(
+    "AssociateNodeResponseTypeDef",
+    {
+        "NodeAssociationStatusToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountAttributesResponseTypeDef = TypedDict(
+    "DescribeAccountAttributesResponseTypeDef",
+    {
+        "Attributes": List[AccountAttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateNodeResponseTypeDef = TypedDict(
+    "DisassociateNodeResponseTypeDef",
+    {
+        "NodeAssociationStatusToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateBackupResponseTypeDef = TypedDict(
     "CreateBackupResponseTypeDef",
     {
         "Backup": BackupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBackupsResponseTypeDef = TypedDict(
     "DescribeBackupsResponseTypeDef",
     {
         "Backups": List[BackupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBackupRequestRequestTypeDef",
     {
         "ServerName": str,
@@ -630,37 +537,91 @@
 
 class CreateServerRequestRequestTypeDef(
     _RequiredCreateServerRequestRequestTypeDef, _OptionalCreateServerRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    {
+        "BackupId": str,
+        "ServerName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef",
+    {
+        "ServerName": str,
+    },
+)
+_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeEventsRequestDescribeEventsPaginateTypeDef(
+    _RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef,
+    _OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef,
+):
+    pass
+
+
+DescribeServersRequestDescribeServersPaginateTypeDef = TypedDict(
+    "DescribeServersRequestDescribeServersPaginateTypeDef",
+    {
+        "ServerName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
     },
 )
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
 
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "ServerEvents": List[ServerEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef = TypedDict(
     "_RequiredDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef",
     {
         "NodeAssociationStatusToken": str,
@@ -679,55 +640,113 @@
 class DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef(
     _RequiredDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
     _OptionalDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
 ):
     pass
 
 
+DescribeNodeAssociationStatusResponseTypeDef = TypedDict(
+    "DescribeNodeAssociationStatusResponseTypeDef",
+    {
+        "NodeAssociationStatus": NodeAssociationStatusType,
+        "EngineAttributes": List[EngineAttributeOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportServerEngineAttributeResponseTypeDef = TypedDict(
+    "ExportServerEngineAttributeResponseTypeDef",
+    {
+        "EngineAttribute": EngineAttributeOutputTypeDef,
+        "ServerName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ServerTypeDef = TypedDict(
+    "ServerTypeDef",
+    {
+        "AssociatePublicIpAddress": bool,
+        "BackupRetentionCount": int,
+        "ServerName": str,
+        "CreatedAt": datetime,
+        "CloudFormationStackArn": str,
+        "CustomDomain": str,
+        "DisableAutomatedBackup": bool,
+        "Endpoint": str,
+        "Engine": str,
+        "EngineModel": str,
+        "EngineAttributes": List[EngineAttributeOutputTypeDef],
+        "EngineVersion": str,
+        "InstanceProfileArn": str,
+        "InstanceType": str,
+        "KeyPair": str,
+        "MaintenanceStatus": MaintenanceStatusType,
+        "PreferredMaintenanceWindow": str,
+        "PreferredBackupWindow": str,
+        "SecurityGroupIds": List[str],
+        "ServiceRoleArn": str,
+        "Status": ServerStatusType,
+        "StatusReason": str,
+        "SubnetIds": List[str],
+        "ServerArn": str,
+    },
+    total=False,
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateServerResponseTypeDef = TypedDict(
     "CreateServerResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServersResponseTypeDef = TypedDict(
     "DescribeServersResponseTypeDef",
     {
         "Servers": List[ServerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreServerResponseTypeDef = TypedDict(
     "RestoreServerResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartMaintenanceResponseTypeDef = TypedDict(
     "StartMaintenanceResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServerEngineAttributesResponseTypeDef = TypedDict(
     "UpdateServerEngineAttributesResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServerResponseTypeDef = TypedDict(
     "UpdateServerResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/type_defs.pyi` & `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -27,53 +27,55 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountAttributeTypeDef",
     "EngineAttributeTypeDef",
-    "AssociateNodeResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "BackupTypeDef",
     "TagTypeDef",
     "DeleteBackupRequestRequestTypeDef",
     "DeleteServerRequestRequestTypeDef",
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeEventsRequestRequestTypeDef",
     "ServerEventTypeDef",
     "WaiterConfigTypeDef",
     "DescribeNodeAssociationStatusRequestRequestTypeDef",
-    "DescribeServersRequestDescribeServersPaginateTypeDef",
+    "EngineAttributeOutputTypeDef",
     "DescribeServersRequestRequestTypeDef",
-    "DisassociateNodeResponseTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "TagOutputTypeDef",
     "RestoreServerRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateServerEngineAttributesRequestRequestTypeDef",
     "UpdateServerRequestRequestTypeDef",
-    "DescribeAccountAttributesResponseTypeDef",
     "AssociateNodeRequestRequestTypeDef",
-    "DescribeNodeAssociationStatusResponseTypeDef",
     "DisassociateNodeRequestRequestTypeDef",
     "ExportServerEngineAttributeRequestRequestTypeDef",
-    "ExportServerEngineAttributeResponseTypeDef",
-    "ServerTypeDef",
     "StartMaintenanceRequestRequestTypeDef",
+    "AssociateNodeResponseTypeDef",
+    "DescribeAccountAttributesResponseTypeDef",
+    "DisassociateNodeResponseTypeDef",
     "CreateBackupResponseTypeDef",
     "DescribeBackupsResponseTypeDef",
     "CreateBackupRequestRequestTypeDef",
     "CreateServerRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
+    "DescribeServersRequestDescribeServersPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "DescribeEventsResponseTypeDef",
     "DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef",
+    "DescribeNodeAssociationStatusResponseTypeDef",
+    "ExportServerEngineAttributeResponseTypeDef",
+    "ServerTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateServerResponseTypeDef",
     "DescribeServersResponseTypeDef",
     "RestoreServerResponseTypeDef",
     "StartMaintenanceResponseTypeDef",
     "UpdateServerEngineAttributesResponseTypeDef",
     "UpdateServerResponseTypeDef",
 )
@@ -93,19 +95,22 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-AssociateNodeResponseTypeDef = TypedDict(
-    "AssociateNodeResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "NodeAssociationStatusToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 BackupTypeDef = TypedDict(
     "BackupTypeDef",
     {
         "BackupArn": str,
@@ -154,20 +159,20 @@
 DeleteServerRequestRequestTypeDef = TypedDict(
     "DeleteServerRequestRequestTypeDef",
     {
         "ServerName": str,
     },
 )
 
-DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "BackupId": str,
-        "ServerName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeBackupsRequestRequestTypeDef = TypedDict(
     "DescribeBackupsRequestRequestTypeDef",
     {
@@ -175,34 +180,14 @@
         "ServerName": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "ServerName": str,
-    },
-)
-_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeEventsRequestDescribeEventsPaginateTypeDef(
-    _RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef,
-    _OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeEventsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEventsRequestRequestTypeDef",
     {
         "ServerName": str,
     },
 )
 _OptionalDescribeEventsRequestRequestTypeDef = TypedDict(
@@ -243,61 +228,33 @@
     "DescribeNodeAssociationStatusRequestRequestTypeDef",
     {
         "NodeAssociationStatusToken": str,
         "ServerName": str,
     },
 )
 
-DescribeServersRequestDescribeServersPaginateTypeDef = TypedDict(
-    "DescribeServersRequestDescribeServersPaginateTypeDef",
+EngineAttributeOutputTypeDef = TypedDict(
+    "EngineAttributeOutputTypeDef",
     {
-        "ServerName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "Name": str,
+        "Value": str,
     },
     total=False,
 )
 
 DescribeServersRequestRequestTypeDef = TypedDict(
     "DescribeServersRequestRequestTypeDef",
     {
         "ServerName": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-DisassociateNodeResponseTypeDef = TypedDict(
-    "DisassociateNodeResponseTypeDef",
-    {
-        "NodeAssociationStatusToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -311,32 +268,19 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
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
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Key": str,
+        "Value": str,
     },
 )
 
 _RequiredRestoreServerRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreServerRequestRequestTypeDef",
     {
         "BackupId": str,
@@ -404,40 +348,23 @@
 )
 
 class UpdateServerRequestRequestTypeDef(
     _RequiredUpdateServerRequestRequestTypeDef, _OptionalUpdateServerRequestRequestTypeDef
 ):
     pass
 
-DescribeAccountAttributesResponseTypeDef = TypedDict(
-    "DescribeAccountAttributesResponseTypeDef",
-    {
-        "Attributes": List[AccountAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateNodeRequestRequestTypeDef = TypedDict(
     "AssociateNodeRequestRequestTypeDef",
     {
         "ServerName": str,
         "NodeName": str,
         "EngineAttributes": Sequence[EngineAttributeTypeDef],
     },
 )
 
-DescribeNodeAssociationStatusResponseTypeDef = TypedDict(
-    "DescribeNodeAssociationStatusResponseTypeDef",
-    {
-        "NodeAssociationStatus": NodeAssociationStatusType,
-        "EngineAttributes": List[EngineAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDisassociateNodeRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateNodeRequestRequestTypeDef",
     {
         "ServerName": str,
         "NodeName": str,
     },
 )
@@ -471,54 +398,14 @@
 
 class ExportServerEngineAttributeRequestRequestTypeDef(
     _RequiredExportServerEngineAttributeRequestRequestTypeDef,
     _OptionalExportServerEngineAttributeRequestRequestTypeDef,
 ):
     pass
 
-ExportServerEngineAttributeResponseTypeDef = TypedDict(
-    "ExportServerEngineAttributeResponseTypeDef",
-    {
-        "EngineAttribute": EngineAttributeTypeDef,
-        "ServerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ServerTypeDef = TypedDict(
-    "ServerTypeDef",
-    {
-        "AssociatePublicIpAddress": bool,
-        "BackupRetentionCount": int,
-        "ServerName": str,
-        "CreatedAt": datetime,
-        "CloudFormationStackArn": str,
-        "CustomDomain": str,
-        "DisableAutomatedBackup": bool,
-        "Endpoint": str,
-        "Engine": str,
-        "EngineModel": str,
-        "EngineAttributes": List[EngineAttributeTypeDef],
-        "EngineVersion": str,
-        "InstanceProfileArn": str,
-        "InstanceType": str,
-        "KeyPair": str,
-        "MaintenanceStatus": MaintenanceStatusType,
-        "PreferredMaintenanceWindow": str,
-        "PreferredBackupWindow": str,
-        "SecurityGroupIds": List[str],
-        "ServiceRoleArn": str,
-        "Status": ServerStatusType,
-        "StatusReason": str,
-        "SubnetIds": List[str],
-        "ServerArn": str,
-    },
-    total=False,
-)
-
 _RequiredStartMaintenanceRequestRequestTypeDef = TypedDict(
     "_RequiredStartMaintenanceRequestRequestTypeDef",
     {
         "ServerName": str,
     },
 )
 _OptionalStartMaintenanceRequestRequestTypeDef = TypedDict(
@@ -530,28 +417,52 @@
 )
 
 class StartMaintenanceRequestRequestTypeDef(
     _RequiredStartMaintenanceRequestRequestTypeDef, _OptionalStartMaintenanceRequestRequestTypeDef
 ):
     pass
 
+AssociateNodeResponseTypeDef = TypedDict(
+    "AssociateNodeResponseTypeDef",
+    {
+        "NodeAssociationStatusToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountAttributesResponseTypeDef = TypedDict(
+    "DescribeAccountAttributesResponseTypeDef",
+    {
+        "Attributes": List[AccountAttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateNodeResponseTypeDef = TypedDict(
+    "DisassociateNodeResponseTypeDef",
+    {
+        "NodeAssociationStatusToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateBackupResponseTypeDef = TypedDict(
     "CreateBackupResponseTypeDef",
     {
         "Backup": BackupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBackupsResponseTypeDef = TypedDict(
     "DescribeBackupsResponseTypeDef",
     {
         "Backups": List[BackupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBackupRequestRequestTypeDef",
     {
         "ServerName": str,
@@ -605,37 +516,87 @@
 )
 
 class CreateServerRequestRequestTypeDef(
     _RequiredCreateServerRequestRequestTypeDef, _OptionalCreateServerRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    {
+        "BackupId": str,
+        "ServerName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef",
+    {
+        "ServerName": str,
+    },
+)
+_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeEventsRequestDescribeEventsPaginateTypeDef(
+    _RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef,
+    _OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef,
+):
+    pass
+
+DescribeServersRequestDescribeServersPaginateTypeDef = TypedDict(
+    "DescribeServersRequestDescribeServersPaginateTypeDef",
+    {
+        "ServerName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
     },
 )
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
 
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "ServerEvents": List[ServerEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef = TypedDict(
     "_RequiredDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef",
     {
         "NodeAssociationStatusToken": str,
@@ -652,55 +613,113 @@
 
 class DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef(
     _RequiredDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
     _OptionalDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
 ):
     pass
 
+DescribeNodeAssociationStatusResponseTypeDef = TypedDict(
+    "DescribeNodeAssociationStatusResponseTypeDef",
+    {
+        "NodeAssociationStatus": NodeAssociationStatusType,
+        "EngineAttributes": List[EngineAttributeOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportServerEngineAttributeResponseTypeDef = TypedDict(
+    "ExportServerEngineAttributeResponseTypeDef",
+    {
+        "EngineAttribute": EngineAttributeOutputTypeDef,
+        "ServerName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ServerTypeDef = TypedDict(
+    "ServerTypeDef",
+    {
+        "AssociatePublicIpAddress": bool,
+        "BackupRetentionCount": int,
+        "ServerName": str,
+        "CreatedAt": datetime,
+        "CloudFormationStackArn": str,
+        "CustomDomain": str,
+        "DisableAutomatedBackup": bool,
+        "Endpoint": str,
+        "Engine": str,
+        "EngineModel": str,
+        "EngineAttributes": List[EngineAttributeOutputTypeDef],
+        "EngineVersion": str,
+        "InstanceProfileArn": str,
+        "InstanceType": str,
+        "KeyPair": str,
+        "MaintenanceStatus": MaintenanceStatusType,
+        "PreferredMaintenanceWindow": str,
+        "PreferredBackupWindow": str,
+        "SecurityGroupIds": List[str],
+        "ServiceRoleArn": str,
+        "Status": ServerStatusType,
+        "StatusReason": str,
+        "SubnetIds": List[str],
+        "ServerArn": str,
+    },
+    total=False,
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateServerResponseTypeDef = TypedDict(
     "CreateServerResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServersResponseTypeDef = TypedDict(
     "DescribeServersResponseTypeDef",
     {
         "Servers": List[ServerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreServerResponseTypeDef = TypedDict(
     "RestoreServerResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartMaintenanceResponseTypeDef = TypedDict(
     "StartMaintenanceResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServerEngineAttributesResponseTypeDef = TypedDict(
     "UpdateServerEngineAttributesResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServerResponseTypeDef = TypedDict(
     "UpdateServerResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/waiter.py` & `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm/waiter.pyi` & `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm.egg-info/PKG-INFO` & `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opsworkscm
-Version: 1.28.0
-Summary: Type annotations for boto3.OpsWorksCM 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.OpsWorksCM 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-opsworkscm"></a>
 
 # mypy-boto3-opsworkscm
 
 [![PyPI - mypy-boto3-opsworkscm](https://img.shields.io/pypi/v/mypy-boto3-opsworkscm.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworkscm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworkscm.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworkscm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opsworkscm?color=blue)](https://pypistats.org/packages/mypy-boto3-opsworkscm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opsworkscm)](https://pepy.tech/project/mypy-boto3-opsworkscm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorksCM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
+[boto3.OpsWorksCM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
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
 [mypy-boto3-opsworkscm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -361,53 +361,55 @@
 `mypy_boto3_opsworkscm.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opsworkscm.type_defs import (
     AccountAttributeTypeDef,
     EngineAttributeTypeDef,
-    AssociateNodeResponseTypeDef,
+    ResponseMetadataTypeDef,
     BackupTypeDef,
     TagTypeDef,
     DeleteBackupRequestRequestTypeDef,
     DeleteServerRequestRequestTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeBackupsRequestRequestTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     ServerEventTypeDef,
     WaiterConfigTypeDef,
     DescribeNodeAssociationStatusRequestRequestTypeDef,
-    DescribeServersRequestDescribeServersPaginateTypeDef,
+    EngineAttributeOutputTypeDef,
     DescribeServersRequestRequestTypeDef,
-    DisassociateNodeResponseTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    TagOutputTypeDef,
     RestoreServerRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateServerEngineAttributesRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
     AssociateNodeRequestRequestTypeDef,
-    DescribeNodeAssociationStatusResponseTypeDef,
     DisassociateNodeRequestRequestTypeDef,
     ExportServerEngineAttributeRequestRequestTypeDef,
-    ExportServerEngineAttributeResponseTypeDef,
-    ServerTypeDef,
     StartMaintenanceRequestRequestTypeDef,
+    AssociateNodeResponseTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
+    DisassociateNodeResponseTypeDef,
     CreateBackupResponseTypeDef,
     DescribeBackupsResponseTypeDef,
     CreateBackupRequestRequestTypeDef,
     CreateServerRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
+    DescribeServersRequestDescribeServersPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
+    DescribeNodeAssociationStatusResponseTypeDef,
+    ExportServerEngineAttributeResponseTypeDef,
+    ServerTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateServerResponseTypeDef,
     DescribeServersResponseTypeDef,
     RestoreServerResponseTypeDef,
     StartMaintenanceResponseTypeDef,
     UpdateServerEngineAttributesResponseTypeDef,
     UpdateServerResponseTypeDef,
 )
```

### Comparing `mypy-boto3-opsworkscm-1.28.0/mypy_boto3_opsworkscm.egg-info/SOURCES.txt` & `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.0/setup.py` & `mypy-boto3-opsworkscm-1.28.12/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-opsworkscm",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_opsworkscm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.OpsWorksCM 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.OpsWorksCM 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

