# Comparing `tmp/mypy-boto3-cloudhsmv2-1.28.0.tar.gz` & `tmp/mypy-boto3-cloudhsmv2-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudhsmv2-1.28.0.tar", last modified: Thu Jul  6 20:59:09 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudhsmv2-1.28.12.tar", last modified: Thu Jul 27 05:34:25 2023, max compression
```

## Comparing `mypy-boto3-cloudhsmv2-1.28.0.tar` & `mypy-boto3-cloudhsmv2-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:09.322243 mypy-boto3-cloudhsmv2-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:35:25.000000 mypy-boto3-cloudhsmv2-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14487 2023-07-06 20:59:09.318243 mypy-boto3-cloudhsmv2-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12990 2023-07-06 20:35:25.000000 mypy-boto3-cloudhsmv2-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:09.310243 mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-06 20:35:25.000000 mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-06 20:35:25.000000 mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 20:35:25.000000 mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-07-06 20:35:25.000000 mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-07-06 20:35:25.000000 mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-07-06 20:35:25.000000 mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-06 20:35:25.000000 mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-06 20:35:25.000000 mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-06 20:35:25.000000 mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:25.000000 mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13062 2023-07-06 20:35:27.000000 mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13045 2023-07-06 20:35:25.000000 mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:35:25.000000 mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:09.318243 mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14487 2023-07-06 20:59:09.000000 mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-06 20:59:09.000000 mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:09.000000 mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:09.000000 mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:09.000000 mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 20:59:09.000000 mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:09.322243 mypy-boto3-cloudhsmv2-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:35:24.000000 mypy-boto3-cloudhsmv2-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.160562 mypy-boto3-cloudhsmv2-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsmv2-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-07-27 05:34:25.160562 mypy-boto3-cloudhsmv2-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsmv2-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.156562 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-07-27 05:18:44.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-07-27 05:18:44.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-07-27 05:18:44.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-27 05:18:44.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-27 05:18:44.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-27 05:18:44.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-07-27 05:18:44.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.160562 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:25.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:25.160562 mypy-boto3-cloudhsmv2-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsmv2-1.28.12/setup.py
```

### Comparing `mypy-boto3-cloudhsmv2-1.28.0/LICENSE` & `mypy-boto3-cloudhsmv2-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsmv2-1.28.0/PKG-INFO` & `mypy-boto3-cloudhsmv2-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudhsmv2
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudHSMV2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudHSMV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cloudhsmv2"></a>
 
 # mypy-boto3-cloudhsmv2
 
 [![PyPI - mypy-boto3-cloudhsmv2](https://img.shields.io/pypi/v/mypy-boto3-cloudhsmv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsmv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudhsmv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsmv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudhsmv2?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudhsmv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudhsmv2)](https://pepy.tech/project/mypy-boto3-cloudhsmv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudHSMV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
+[boto3.CloudHSMV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
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
 [mypy-boto3-cloudhsmv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -331,18 +331,20 @@
 ### Typed dictionaries
 
 `mypy_boto3_cloudhsmv2.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudhsmv2.type_defs import (
+    BackupRetentionPolicyOutputTypeDef,
     BackupRetentionPolicyTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     CertificatesTypeDef,
     HsmTypeDef,
+    TagTypeDef,
     DestinationBackupTypeDef,
     CreateHsmRequestRequestTypeDef,
     DeleteBackupRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteHsmRequestRequestTypeDef,
     DeleteHsmResponseTypeDef,
     DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
@@ -356,33 +358,33 @@
     ModifyBackupAttributesRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     RestoreBackupRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ModifyClusterRequestRequestTypeDef,
     BackupTypeDef,
-    CopyBackupToRegionRequestRequestTypeDef,
-    CreateClusterRequestRequestTypeDef,
     ListTagsResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     ClusterTypeDef,
     CreateHsmResponseTypeDef,
+    CopyBackupToRegionRequestRequestTypeDef,
+    CreateClusterRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
     CopyBackupToRegionResponseTypeDef,
     DeleteBackupResponseTypeDef,
     DescribeBackupsResponseTypeDef,
     ModifyBackupAttributesResponseTypeDef,
     RestoreBackupResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DescribeClustersResponseTypeDef,
     ModifyClusterResponseTypeDef,
 )
 
 
-def get_structure() -> BackupRetentionPolicyTypeDef:
+def get_structure() -> BackupRetentionPolicyOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cloudhsmv2-1.28.0/README.md` & `mypy-boto3-cloudhsmv2-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cloudhsmv2"></a>
 
 # mypy-boto3-cloudhsmv2
 
 [![PyPI - mypy-boto3-cloudhsmv2](https://img.shields.io/pypi/v/mypy-boto3-cloudhsmv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsmv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudhsmv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsmv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudhsmv2?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudhsmv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudhsmv2)](https://pepy.tech/project/mypy-boto3-cloudhsmv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudHSMV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
+[boto3.CloudHSMV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
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
 [mypy-boto3-cloudhsmv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,18 +299,20 @@
 ### Typed dictionaries
 
 `mypy_boto3_cloudhsmv2.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudhsmv2.type_defs import (
+    BackupRetentionPolicyOutputTypeDef,
     BackupRetentionPolicyTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     CertificatesTypeDef,
     HsmTypeDef,
+    TagTypeDef,
     DestinationBackupTypeDef,
     CreateHsmRequestRequestTypeDef,
     DeleteBackupRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteHsmRequestRequestTypeDef,
     DeleteHsmResponseTypeDef,
     DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
@@ -324,33 +326,33 @@
     ModifyBackupAttributesRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     RestoreBackupRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ModifyClusterRequestRequestTypeDef,
     BackupTypeDef,
-    CopyBackupToRegionRequestRequestTypeDef,
-    CreateClusterRequestRequestTypeDef,
     ListTagsResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     ClusterTypeDef,
     CreateHsmResponseTypeDef,
+    CopyBackupToRegionRequestRequestTypeDef,
+    CreateClusterRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
     CopyBackupToRegionResponseTypeDef,
     DeleteBackupResponseTypeDef,
     DescribeBackupsResponseTypeDef,
     ModifyBackupAttributesResponseTypeDef,
     RestoreBackupResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DescribeClustersResponseTypeDef,
     ModifyClusterResponseTypeDef,
 )
 
 
-def get_structure() -> BackupRetentionPolicyTypeDef:
+def get_structure() -> BackupRetentionPolicyOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/__init__.py` & `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/__init__.pyi` & `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/__main__.py` & `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudHSMV2 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.CloudHSMV2 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2\nOther"
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

### Comparing `mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/client.py` & `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/client.pyi` & `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/literals.py` & `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,15 @@
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
@@ -256,26 +257,28 @@
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

### Comparing `mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/literals.pyi` & `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -168,14 +168,15 @@
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
@@ -254,26 +255,28 @@
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

### Comparing `mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/paginator.py` & `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/paginator.pyi` & `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/type_defs.py` & `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for cloudhsmv2 service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_cloudhsmv2.type_defs import BackupRetentionPolicyTypeDef
+    from mypy_boto3_cloudhsmv2.type_defs import BackupRetentionPolicyOutputTypeDef
 
-    data: BackupRetentionPolicyTypeDef = {...}
+    data: BackupRetentionPolicyOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import BackupStateType, ClusterStateType, HsmStateType
@@ -22,20 +22,21 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "BackupRetentionPolicyOutputTypeDef",
     "BackupRetentionPolicyTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "CertificatesTypeDef",
     "HsmTypeDef",
+    "TagTypeDef",
     "DestinationBackupTypeDef",
     "CreateHsmRequestRequestTypeDef",
     "DeleteBackupRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteHsmRequestRequestTypeDef",
     "DeleteHsmResponseTypeDef",
     "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
@@ -49,42 +50,51 @@
     "ModifyBackupAttributesRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "RestoreBackupRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ModifyClusterRequestRequestTypeDef",
     "BackupTypeDef",
-    "CopyBackupToRegionRequestRequestTypeDef",
-    "CreateClusterRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "ClusterTypeDef",
     "CreateHsmResponseTypeDef",
+    "CopyBackupToRegionRequestRequestTypeDef",
+    "CreateClusterRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CopyBackupToRegionResponseTypeDef",
     "DeleteBackupResponseTypeDef",
     "DescribeBackupsResponseTypeDef",
     "ModifyBackupAttributesResponseTypeDef",
     "RestoreBackupResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
     "DescribeClustersResponseTypeDef",
     "ModifyClusterResponseTypeDef",
 )
 
+BackupRetentionPolicyOutputTypeDef = TypedDict(
+    "BackupRetentionPolicyOutputTypeDef",
+    {
+        "Type": Literal["DAYS"],
+        "Value": str,
+    },
+    total=False,
+)
+
 BackupRetentionPolicyTypeDef = TypedDict(
     "BackupRetentionPolicyTypeDef",
     {
         "Type": Literal["DAYS"],
         "Value": str,
     },
     total=False,
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
 CertificatesTypeDef = TypedDict(
@@ -115,18 +125,24 @@
         "EniIp": str,
         "State": HsmStateType,
         "StateMessage": str,
     },
     total=False,
 )
 
-
 class HsmTypeDef(_RequiredHsmTypeDef, _OptionalHsmTypeDef):
     pass
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
 
 DestinationBackupTypeDef = TypedDict(
     "DestinationBackupTypeDef",
     {
         "CreateTimestamp": datetime,
         "SourceRegion": str,
         "SourceBackup": str,
@@ -146,21 +162,19 @@
     "_OptionalCreateHsmRequestRequestTypeDef",
     {
         "IpAddress": str,
     },
     total=False,
 )
 
-
 class CreateHsmRequestRequestTypeDef(
     _RequiredCreateHsmRequestRequestTypeDef, _OptionalCreateHsmRequestRequestTypeDef
 ):
     pass
 
-
 DeleteBackupRequestRequestTypeDef = TypedDict(
     "DeleteBackupRequestRequestTypeDef",
     {
         "BackupId": str,
     },
 )
 
@@ -183,21 +197,19 @@
         "HsmId": str,
         "EniId": str,
         "EniIp": str,
     },
     total=False,
 )
 
-
 class DeleteHsmRequestRequestTypeDef(
     _RequiredDeleteHsmRequestRequestTypeDef, _OptionalDeleteHsmRequestRequestTypeDef
 ):
     pass
 
-
 DeleteHsmResponseTypeDef = TypedDict(
     "DeleteHsmResponseTypeDef",
     {
         "HsmId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -270,21 +282,19 @@
     "_OptionalListTagsRequestListTagsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListTagsRequestListTagsPaginateTypeDef(
     _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
 ):
     pass
 
-
 _RequiredListTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalListTagsRequestRequestTypeDef = TypedDict(
@@ -292,21 +302,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
-
 ModifyBackupAttributesRequestRequestTypeDef = TypedDict(
     "ModifyBackupAttributesRequestRequestTypeDef",
     {
         "BackupId": str,
         "NeverExpires": bool,
     },
 )
@@ -369,23 +377,60 @@
         "CreateTimestamp": datetime,
         "CopyTimestamp": datetime,
         "NeverExpires": bool,
         "SourceRegion": str,
         "SourceBackup": str,
         "SourceCluster": str,
         "DeleteTimestamp": datetime,
-        "TagList": List[TagTypeDef],
+        "TagList": List[TagOutputTypeDef],
     },
     total=False,
 )
 
-
 class BackupTypeDef(_RequiredBackupTypeDef, _OptionalBackupTypeDef):
     pass
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ClusterTypeDef = TypedDict(
+    "ClusterTypeDef",
+    {
+        "BackupPolicy": Literal["DEFAULT"],
+        "BackupRetentionPolicy": BackupRetentionPolicyOutputTypeDef,
+        "ClusterId": str,
+        "CreateTimestamp": datetime,
+        "Hsms": List[HsmTypeDef],
+        "HsmType": str,
+        "PreCoPassword": str,
+        "SecurityGroup": str,
+        "SourceBackupId": str,
+        "State": ClusterStateType,
+        "StateMessage": str,
+        "SubnetMapping": Dict[str, str],
+        "VpcId": str,
+        "Certificates": CertificatesTypeDef,
+        "TagList": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+CreateHsmResponseTypeDef = TypedDict(
+    "CreateHsmResponseTypeDef",
+    {
+        "Hsm": HsmTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredCopyBackupToRegionRequestRequestTypeDef = TypedDict(
     "_RequiredCopyBackupToRegionRequestRequestTypeDef",
     {
         "DestinationRegion": str,
         "BackupId": str,
     },
@@ -394,22 +439,20 @@
     "_OptionalCopyBackupToRegionRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CopyBackupToRegionRequestRequestTypeDef(
     _RequiredCopyBackupToRegionRequestRequestTypeDef,
     _OptionalCopyBackupToRegionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterRequestRequestTypeDef",
     {
         "HsmType": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -419,68 +462,27 @@
         "BackupRetentionPolicy": BackupRetentionPolicyTypeDef,
         "SourceBackupId": str,
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
-
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagList": Sequence[TagTypeDef],
     },
 )
 
-ClusterTypeDef = TypedDict(
-    "ClusterTypeDef",
-    {
-        "BackupPolicy": Literal["DEFAULT"],
-        "BackupRetentionPolicy": BackupRetentionPolicyTypeDef,
-        "ClusterId": str,
-        "CreateTimestamp": datetime,
-        "Hsms": List[HsmTypeDef],
-        "HsmType": str,
-        "PreCoPassword": str,
-        "SecurityGroup": str,
-        "SourceBackupId": str,
-        "State": ClusterStateType,
-        "StateMessage": str,
-        "SubnetMapping": Dict[str, str],
-        "VpcId": str,
-        "Certificates": CertificatesTypeDef,
-        "TagList": List[TagTypeDef],
-    },
-    total=False,
-)
-
-CreateHsmResponseTypeDef = TypedDict(
-    "CreateHsmResponseTypeDef",
-    {
-        "Hsm": HsmTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CopyBackupToRegionResponseTypeDef = TypedDict(
     "CopyBackupToRegionResponseTypeDef",
     {
         "DestinationBackup": DestinationBackupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2/type_defs.pyi` & `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for cloudhsmv2 service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_cloudhsmv2.type_defs import BackupRetentionPolicyTypeDef
+    from mypy_boto3_cloudhsmv2.type_defs import BackupRetentionPolicyOutputTypeDef
 
-    data: BackupRetentionPolicyTypeDef = {...}
+    data: BackupRetentionPolicyOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import BackupStateType, ClusterStateType, HsmStateType
@@ -22,19 +22,22 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "BackupRetentionPolicyOutputTypeDef",
     "BackupRetentionPolicyTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "CertificatesTypeDef",
     "HsmTypeDef",
+    "TagTypeDef",
     "DestinationBackupTypeDef",
     "CreateHsmRequestRequestTypeDef",
     "DeleteBackupRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteHsmRequestRequestTypeDef",
     "DeleteHsmResponseTypeDef",
     "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
@@ -48,42 +51,51 @@
     "ModifyBackupAttributesRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "RestoreBackupRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ModifyClusterRequestRequestTypeDef",
     "BackupTypeDef",
-    "CopyBackupToRegionRequestRequestTypeDef",
-    "CreateClusterRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "ClusterTypeDef",
     "CreateHsmResponseTypeDef",
+    "CopyBackupToRegionRequestRequestTypeDef",
+    "CreateClusterRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CopyBackupToRegionResponseTypeDef",
     "DeleteBackupResponseTypeDef",
     "DescribeBackupsResponseTypeDef",
     "ModifyBackupAttributesResponseTypeDef",
     "RestoreBackupResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
     "DescribeClustersResponseTypeDef",
     "ModifyClusterResponseTypeDef",
 )
 
+BackupRetentionPolicyOutputTypeDef = TypedDict(
+    "BackupRetentionPolicyOutputTypeDef",
+    {
+        "Type": Literal["DAYS"],
+        "Value": str,
+    },
+    total=False,
+)
+
 BackupRetentionPolicyTypeDef = TypedDict(
     "BackupRetentionPolicyTypeDef",
     {
         "Type": Literal["DAYS"],
         "Value": str,
     },
     total=False,
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
 CertificatesTypeDef = TypedDict(
@@ -114,17 +126,27 @@
         "EniIp": str,
         "State": HsmStateType,
         "StateMessage": str,
     },
     total=False,
 )
 
+
 class HsmTypeDef(_RequiredHsmTypeDef, _OptionalHsmTypeDef):
     pass
 
+
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 DestinationBackupTypeDef = TypedDict(
     "DestinationBackupTypeDef",
     {
         "CreateTimestamp": datetime,
         "SourceRegion": str,
         "SourceBackup": str,
         "SourceCluster": str,
@@ -143,19 +165,21 @@
     "_OptionalCreateHsmRequestRequestTypeDef",
     {
         "IpAddress": str,
     },
     total=False,
 )
 
+
 class CreateHsmRequestRequestTypeDef(
     _RequiredCreateHsmRequestRequestTypeDef, _OptionalCreateHsmRequestRequestTypeDef
 ):
     pass
 
+
 DeleteBackupRequestRequestTypeDef = TypedDict(
     "DeleteBackupRequestRequestTypeDef",
     {
         "BackupId": str,
     },
 )
 
@@ -178,19 +202,21 @@
         "HsmId": str,
         "EniId": str,
         "EniIp": str,
     },
     total=False,
 )
 
+
 class DeleteHsmRequestRequestTypeDef(
     _RequiredDeleteHsmRequestRequestTypeDef, _OptionalDeleteHsmRequestRequestTypeDef
 ):
     pass
 
+
 DeleteHsmResponseTypeDef = TypedDict(
     "DeleteHsmResponseTypeDef",
     {
         "HsmId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -263,19 +289,21 @@
     "_OptionalListTagsRequestListTagsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListTagsRequestListTagsPaginateTypeDef(
     _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
 ):
     pass
 
+
 _RequiredListTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalListTagsRequestRequestTypeDef = TypedDict(
@@ -283,19 +311,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
+
 ModifyBackupAttributesRequestRequestTypeDef = TypedDict(
     "ModifyBackupAttributesRequestRequestTypeDef",
     {
         "BackupId": str,
         "NeverExpires": bool,
     },
 )
@@ -358,22 +388,63 @@
         "CreateTimestamp": datetime,
         "CopyTimestamp": datetime,
         "NeverExpires": bool,
         "SourceRegion": str,
         "SourceBackup": str,
         "SourceCluster": str,
         "DeleteTimestamp": datetime,
-        "TagList": List[TagTypeDef],
+        "TagList": List[TagOutputTypeDef],
     },
     total=False,
 )
 
+
 class BackupTypeDef(_RequiredBackupTypeDef, _OptionalBackupTypeDef):
     pass
 
+
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ClusterTypeDef = TypedDict(
+    "ClusterTypeDef",
+    {
+        "BackupPolicy": Literal["DEFAULT"],
+        "BackupRetentionPolicy": BackupRetentionPolicyOutputTypeDef,
+        "ClusterId": str,
+        "CreateTimestamp": datetime,
+        "Hsms": List[HsmTypeDef],
+        "HsmType": str,
+        "PreCoPassword": str,
+        "SecurityGroup": str,
+        "SourceBackupId": str,
+        "State": ClusterStateType,
+        "StateMessage": str,
+        "SubnetMapping": Dict[str, str],
+        "VpcId": str,
+        "Certificates": CertificatesTypeDef,
+        "TagList": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+CreateHsmResponseTypeDef = TypedDict(
+    "CreateHsmResponseTypeDef",
+    {
+        "Hsm": HsmTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCopyBackupToRegionRequestRequestTypeDef = TypedDict(
     "_RequiredCopyBackupToRegionRequestRequestTypeDef",
     {
         "DestinationRegion": str,
         "BackupId": str,
     },
 )
@@ -381,20 +452,22 @@
     "_OptionalCopyBackupToRegionRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CopyBackupToRegionRequestRequestTypeDef(
     _RequiredCopyBackupToRegionRequestRequestTypeDef,
     _OptionalCopyBackupToRegionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterRequestRequestTypeDef",
     {
         "HsmType": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -404,66 +477,29 @@
         "BackupRetentionPolicy": BackupRetentionPolicyTypeDef,
         "SourceBackupId": str,
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagList": Sequence[TagTypeDef],
     },
 )
 
-ClusterTypeDef = TypedDict(
-    "ClusterTypeDef",
-    {
-        "BackupPolicy": Literal["DEFAULT"],
-        "BackupRetentionPolicy": BackupRetentionPolicyTypeDef,
-        "ClusterId": str,
-        "CreateTimestamp": datetime,
-        "Hsms": List[HsmTypeDef],
-        "HsmType": str,
-        "PreCoPassword": str,
-        "SecurityGroup": str,
-        "SourceBackupId": str,
-        "State": ClusterStateType,
-        "StateMessage": str,
-        "SubnetMapping": Dict[str, str],
-        "VpcId": str,
-        "Certificates": CertificatesTypeDef,
-        "TagList": List[TagTypeDef],
-    },
-    total=False,
-)
-
-CreateHsmResponseTypeDef = TypedDict(
-    "CreateHsmResponseTypeDef",
-    {
-        "Hsm": HsmTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CopyBackupToRegionResponseTypeDef = TypedDict(
     "CopyBackupToRegionResponseTypeDef",
     {
         "DestinationBackup": DestinationBackupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2.egg-info/PKG-INFO` & `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudhsmv2
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudHSMV2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudHSMV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cloudhsmv2"></a>
 
 # mypy-boto3-cloudhsmv2
 
 [![PyPI - mypy-boto3-cloudhsmv2](https://img.shields.io/pypi/v/mypy-boto3-cloudhsmv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsmv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudhsmv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsmv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudhsmv2?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudhsmv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudhsmv2)](https://pepy.tech/project/mypy-boto3-cloudhsmv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudHSMV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
+[boto3.CloudHSMV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
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
 [mypy-boto3-cloudhsmv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -331,18 +331,20 @@
 ### Typed dictionaries
 
 `mypy_boto3_cloudhsmv2.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudhsmv2.type_defs import (
+    BackupRetentionPolicyOutputTypeDef,
     BackupRetentionPolicyTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     CertificatesTypeDef,
     HsmTypeDef,
+    TagTypeDef,
     DestinationBackupTypeDef,
     CreateHsmRequestRequestTypeDef,
     DeleteBackupRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteHsmRequestRequestTypeDef,
     DeleteHsmResponseTypeDef,
     DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
@@ -356,33 +358,33 @@
     ModifyBackupAttributesRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     RestoreBackupRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ModifyClusterRequestRequestTypeDef,
     BackupTypeDef,
-    CopyBackupToRegionRequestRequestTypeDef,
-    CreateClusterRequestRequestTypeDef,
     ListTagsResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     ClusterTypeDef,
     CreateHsmResponseTypeDef,
+    CopyBackupToRegionRequestRequestTypeDef,
+    CreateClusterRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
     CopyBackupToRegionResponseTypeDef,
     DeleteBackupResponseTypeDef,
     DescribeBackupsResponseTypeDef,
     ModifyBackupAttributesResponseTypeDef,
     RestoreBackupResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DescribeClustersResponseTypeDef,
     ModifyClusterResponseTypeDef,
 )
 
 
-def get_structure() -> BackupRetentionPolicyTypeDef:
+def get_structure() -> BackupRetentionPolicyOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cloudhsmv2-1.28.0/mypy_boto3_cloudhsmv2.egg-info/SOURCES.txt` & `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsmv2-1.28.0/setup.py` & `mypy-boto3-cloudhsmv2-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudhsmv2",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_cloudhsmv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudHSMV2 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.CloudHSMV2 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

