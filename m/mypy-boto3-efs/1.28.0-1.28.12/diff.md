# Comparing `tmp/mypy-boto3-efs-1.28.0.tar.gz` & `tmp/mypy-boto3-efs-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-efs-1.28.0.tar", last modified: Thu Jul  6 20:59:29 2023, max compression
+gzip compressed data, was "mypy-boto3-efs-1.28.12.tar", last modified: Thu Jul 27 05:34:38 2023, max compression
```

## Comparing `mypy-boto3-efs-1.28.0.tar` & `mypy-boto3-efs-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:29.938291 mypy-boto3-efs-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:40:02.000000 mypy-boto3-efs-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15688 2023-07-06 20:59:29.934291 mypy-boto3-efs-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14219 2023-07-06 20:40:02.000000 mypy-boto3-efs-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:29.926291 mypy-boto3-efs-1.28.0/mypy_boto3_efs/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-06 20:40:02.000000 mypy-boto3-efs-1.28.0/mypy_boto3_efs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-06 20:40:02.000000 mypy-boto3-efs-1.28.0/mypy_boto3_efs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:40:02.000000 mypy-boto3-efs-1.28.0/mypy_boto3_efs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23575 2023-07-06 20:40:02.000000 mypy-boto3-efs-1.28.0/mypy_boto3_efs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23535 2023-07-06 20:40:02.000000 mypy-boto3-efs-1.28.0/mypy_boto3_efs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-07-06 20:40:03.000000 mypy-boto3-efs-1.28.0/mypy_boto3_efs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9480 2023-07-06 20:40:03.000000 mypy-boto3-efs-1.28.0/mypy_boto3_efs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-06 20:40:02.000000 mypy-boto3-efs-1.28.0/mypy_boto3_efs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-07-06 20:40:02.000000 mypy-boto3-efs-1.28.0/mypy_boto3_efs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:40:02.000000 mypy-boto3-efs-1.28.0/mypy_boto3_efs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24266 2023-07-06 20:40:03.000000 mypy-boto3-efs-1.28.0/mypy_boto3_efs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24237 2023-07-06 20:40:03.000000 mypy-boto3-efs-1.28.0/mypy_boto3_efs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:40:02.000000 mypy-boto3-efs-1.28.0/mypy_boto3_efs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:29.934291 mypy-boto3-efs-1.28.0/mypy_boto3_efs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15688 2023-07-06 20:59:29.000000 mypy-boto3-efs-1.28.0/mypy_boto3_efs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 20:59:29.000000 mypy-boto3-efs-1.28.0/mypy_boto3_efs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:29.000000 mypy-boto3-efs-1.28.0/mypy_boto3_efs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:29.000000 mypy-boto3-efs-1.28.0/mypy_boto3_efs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:29.000000 mypy-boto3-efs-1.28.0/mypy_boto3_efs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:29.000000 mypy-boto3-efs-1.28.0/mypy_boto3_efs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:29.938291 mypy-boto3-efs-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:40:02.000000 mypy-boto3-efs-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.068522 mypy-boto3-efs-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15859 2023-07-27 05:34:38.068522 mypy-boto3-efs-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14388 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.064522 mypy-boto3-efs-1.28.12/mypy_boto3_efs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23575 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23535 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25747 2023-07-27 05:21:39.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25716 2023-07-27 05:21:38.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.068522 mypy-boto3-efs-1.28.12/mypy_boto3_efs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15859 2023-07-27 05:34:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 05:34:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:38.068522 mypy-boto3-efs-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/setup.py
```

### Comparing `mypy-boto3-efs-1.28.0/LICENSE` & `mypy-boto3-efs-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.0/PKG-INFO` & `mypy-boto3-efs-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-efs
-Version: 1.28.0
-Summary: Type annotations for boto3.EFS 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.EFS 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-efs"></a>
 
 # mypy-boto3-efs
 
 [![PyPI - mypy-boto3-efs](https://img.shields.io/pypi/v/mypy-boto3-efs.svg?color=blue)](https://pypi.org/project/mypy-boto3-efs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-efs.svg?color=blue)](https://pypi.org/project/mypy-boto3-efs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-efs?color=blue)](https://pypistats.org/packages/mypy-boto3-efs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-efs)](https://pepy.tech/project/mypy-boto3-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EFS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
+[boto3.EFS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
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
 [mypy-boto3-efs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,19 +338,23 @@
 ### Typed dictionaries
 
 `mypy_boto3_efs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_efs.type_defs import (
+    PosixUserOutputTypeDef,
+    TagOutputTypeDef,
+    BackupPolicyOutputTypeDef,
+    BackupPolicyTypeDef,
     PosixUserTypeDef,
     TagTypeDef,
-    BackupPolicyTypeDef,
     CreateMountTargetRequestRequestTypeDef,
     DestinationToCreateTypeDef,
+    CreationInfoOutputTypeDef,
     CreationInfoTypeDef,
     DeleteAccessPointRequestRequestTypeDef,
     DeleteFileSystemPolicyRequestRequestTypeDef,
     DeleteFileSystemRequestRequestTypeDef,
     DeleteMountTargetRequestRequestTypeDef,
     DeleteReplicationConfigurationRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
@@ -370,32 +374,34 @@
     DescribeReplicationConfigurationsRequestRequestTypeDef,
     DescribeTagsRequestDescribeTagsPaginateTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DestinationTypeDef,
     EmptyResponseMetadataTypeDef,
     FileSystemSizeTypeDef,
     FileSystemPolicyDescriptionTypeDef,
+    LifecyclePolicyOutputTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModifyMountTargetSecurityGroupsRequestRequestTypeDef,
     MountTargetDescriptionResponseMetadataTypeDef,
     PaginatorConfigTypeDef,
     PutAccountPreferencesRequestRequestTypeDef,
     PutFileSystemPolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileSystemRequestRequestTypeDef,
-    CreateFileSystemRequestRequestTypeDef,
-    CreateTagsRequestRequestTypeDef,
     DescribeTagsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     BackupPolicyDescriptionTypeDef,
     PutBackupPolicyRequestRequestTypeDef,
+    CreateFileSystemRequestRequestTypeDef,
+    CreateTagsRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateReplicationConfigurationRequestRequestTypeDef,
+    RootDirectoryOutputTypeDef,
     RootDirectoryTypeDef,
     DescribeAccountPreferencesResponseTypeDef,
     PutAccountPreferencesResponseTypeDef,
     DescribeMountTargetsResponseTypeDef,
     ReplicationConfigurationDescriptionResponseMetadataTypeDef,
     ReplicationConfigurationDescriptionTypeDef,
     FileSystemDescriptionResponseMetadataTypeDef,
@@ -407,15 +413,15 @@
     CreateAccessPointRequestRequestTypeDef,
     DescribeReplicationConfigurationsResponseTypeDef,
     DescribeFileSystemsResponseTypeDef,
     DescribeAccessPointsResponseTypeDef,
 )
 
 
-def get_structure() -> PosixUserTypeDef:
+def get_structure() -> PosixUserOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-efs-1.28.0/README.md` & `mypy-boto3-efs-1.28.12/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-efs"></a>
 
 # mypy-boto3-efs
 
 [![PyPI - mypy-boto3-efs](https://img.shields.io/pypi/v/mypy-boto3-efs.svg?color=blue)](https://pypi.org/project/mypy-boto3-efs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-efs.svg?color=blue)](https://pypi.org/project/mypy-boto3-efs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-efs?color=blue)](https://pypistats.org/packages/mypy-boto3-efs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-efs)](https://pepy.tech/project/mypy-boto3-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EFS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
+[boto3.EFS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
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
 [mypy-boto3-efs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,19 +306,23 @@
 ### Typed dictionaries
 
 `mypy_boto3_efs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_efs.type_defs import (
+    PosixUserOutputTypeDef,
+    TagOutputTypeDef,
+    BackupPolicyOutputTypeDef,
+    BackupPolicyTypeDef,
     PosixUserTypeDef,
     TagTypeDef,
-    BackupPolicyTypeDef,
     CreateMountTargetRequestRequestTypeDef,
     DestinationToCreateTypeDef,
+    CreationInfoOutputTypeDef,
     CreationInfoTypeDef,
     DeleteAccessPointRequestRequestTypeDef,
     DeleteFileSystemPolicyRequestRequestTypeDef,
     DeleteFileSystemRequestRequestTypeDef,
     DeleteMountTargetRequestRequestTypeDef,
     DeleteReplicationConfigurationRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
@@ -338,32 +342,34 @@
     DescribeReplicationConfigurationsRequestRequestTypeDef,
     DescribeTagsRequestDescribeTagsPaginateTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DestinationTypeDef,
     EmptyResponseMetadataTypeDef,
     FileSystemSizeTypeDef,
     FileSystemPolicyDescriptionTypeDef,
+    LifecyclePolicyOutputTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModifyMountTargetSecurityGroupsRequestRequestTypeDef,
     MountTargetDescriptionResponseMetadataTypeDef,
     PaginatorConfigTypeDef,
     PutAccountPreferencesRequestRequestTypeDef,
     PutFileSystemPolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileSystemRequestRequestTypeDef,
-    CreateFileSystemRequestRequestTypeDef,
-    CreateTagsRequestRequestTypeDef,
     DescribeTagsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     BackupPolicyDescriptionTypeDef,
     PutBackupPolicyRequestRequestTypeDef,
+    CreateFileSystemRequestRequestTypeDef,
+    CreateTagsRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateReplicationConfigurationRequestRequestTypeDef,
+    RootDirectoryOutputTypeDef,
     RootDirectoryTypeDef,
     DescribeAccountPreferencesResponseTypeDef,
     PutAccountPreferencesResponseTypeDef,
     DescribeMountTargetsResponseTypeDef,
     ReplicationConfigurationDescriptionResponseMetadataTypeDef,
     ReplicationConfigurationDescriptionTypeDef,
     FileSystemDescriptionResponseMetadataTypeDef,
@@ -375,15 +381,15 @@
     CreateAccessPointRequestRequestTypeDef,
     DescribeReplicationConfigurationsResponseTypeDef,
     DescribeFileSystemsResponseTypeDef,
     DescribeAccessPointsResponseTypeDef,
 )
 
 
-def get_structure() -> PosixUserTypeDef:
+def get_structure() -> PosixUserOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-efs-1.28.0/mypy_boto3_efs/__init__.py` & `mypy-boto3-efs-1.28.12/mypy_boto3_efs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.0/mypy_boto3_efs/__init__.pyi` & `mypy-boto3-efs-1.28.12/mypy_boto3_efs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.0/mypy_boto3_efs/__main__.py` & `mypy-boto3-efs-1.28.12/mypy_boto3_efs/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EFS 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.EFS 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS\nOther"
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

### Comparing `mypy-boto3-efs-1.28.0/mypy_boto3_efs/client.py` & `mypy-boto3-efs-1.28.12/mypy_boto3_efs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.0/mypy_boto3_efs/client.pyi` & `mypy-boto3-efs-1.28.12/mypy_boto3_efs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.0/mypy_boto3_efs/literals.py` & `mypy-boto3-efs-1.28.12/mypy_boto3_efs/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,15 @@
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
@@ -261,26 +262,28 @@
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

### Comparing `mypy-boto3-efs-1.28.0/mypy_boto3_efs/literals.pyi` & `mypy-boto3-efs-1.28.12/mypy_boto3_efs/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,15 @@
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
@@ -259,26 +260,28 @@
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

### Comparing `mypy-boto3-efs-1.28.0/mypy_boto3_efs/paginator.py` & `mypy-boto3-efs-1.28.12/mypy_boto3_efs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.0/mypy_boto3_efs/paginator.pyi` & `mypy-boto3-efs-1.28.12/mypy_boto3_efs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.0/mypy_boto3_efs/type_defs.py` & `mypy-boto3-efs-1.28.12/mypy_boto3_efs/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for efs service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_efs.type_defs import PosixUserTypeDef
+    from mypy_boto3_efs.type_defs import PosixUserOutputTypeDef
 
-    data: PosixUserTypeDef = {...}
+    data: PosixUserOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -31,21 +31,24 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "PosixUserOutputTypeDef",
+    "TagOutputTypeDef",
+    "BackupPolicyOutputTypeDef",
+    "BackupPolicyTypeDef",
     "PosixUserTypeDef",
     "TagTypeDef",
-    "BackupPolicyTypeDef",
     "CreateMountTargetRequestRequestTypeDef",
     "DestinationToCreateTypeDef",
+    "CreationInfoOutputTypeDef",
     "CreationInfoTypeDef",
     "DeleteAccessPointRequestRequestTypeDef",
     "DeleteFileSystemPolicyRequestRequestTypeDef",
     "DeleteFileSystemRequestRequestTypeDef",
     "DeleteMountTargetRequestRequestTypeDef",
     "DeleteReplicationConfigurationRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
@@ -65,32 +68,34 @@
     "DescribeReplicationConfigurationsRequestRequestTypeDef",
     "DescribeTagsRequestDescribeTagsPaginateTypeDef",
     "DescribeTagsRequestRequestTypeDef",
     "DestinationTypeDef",
     "EmptyResponseMetadataTypeDef",
     "FileSystemSizeTypeDef",
     "FileSystemPolicyDescriptionTypeDef",
+    "LifecyclePolicyOutputTypeDef",
     "LifecyclePolicyTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ModifyMountTargetSecurityGroupsRequestRequestTypeDef",
     "MountTargetDescriptionResponseMetadataTypeDef",
     "PaginatorConfigTypeDef",
     "PutAccountPreferencesRequestRequestTypeDef",
     "PutFileSystemPolicyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFileSystemRequestRequestTypeDef",
-    "CreateFileSystemRequestRequestTypeDef",
-    "CreateTagsRequestRequestTypeDef",
     "DescribeTagsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "BackupPolicyDescriptionTypeDef",
     "PutBackupPolicyRequestRequestTypeDef",
+    "CreateFileSystemRequestRequestTypeDef",
+    "CreateTagsRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateReplicationConfigurationRequestRequestTypeDef",
+    "RootDirectoryOutputTypeDef",
     "RootDirectoryTypeDef",
     "DescribeAccountPreferencesResponseTypeDef",
     "PutAccountPreferencesResponseTypeDef",
     "DescribeMountTargetsResponseTypeDef",
     "ReplicationConfigurationDescriptionResponseMetadataTypeDef",
     "ReplicationConfigurationDescriptionTypeDef",
     "FileSystemDescriptionResponseMetadataTypeDef",
@@ -101,14 +106,54 @@
     "AccessPointDescriptionTypeDef",
     "CreateAccessPointRequestRequestTypeDef",
     "DescribeReplicationConfigurationsResponseTypeDef",
     "DescribeFileSystemsResponseTypeDef",
     "DescribeAccessPointsResponseTypeDef",
 )
 
+_RequiredPosixUserOutputTypeDef = TypedDict(
+    "_RequiredPosixUserOutputTypeDef",
+    {
+        "Uid": int,
+        "Gid": int,
+    },
+)
+_OptionalPosixUserOutputTypeDef = TypedDict(
+    "_OptionalPosixUserOutputTypeDef",
+    {
+        "SecondaryGids": List[int],
+    },
+    total=False,
+)
+
+class PosixUserOutputTypeDef(_RequiredPosixUserOutputTypeDef, _OptionalPosixUserOutputTypeDef):
+    pass
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+BackupPolicyOutputTypeDef = TypedDict(
+    "BackupPolicyOutputTypeDef",
+    {
+        "Status": StatusType,
+    },
+)
+
+BackupPolicyTypeDef = TypedDict(
+    "BackupPolicyTypeDef",
+    {
+        "Status": StatusType,
+    },
+)
+
 _RequiredPosixUserTypeDef = TypedDict(
     "_RequiredPosixUserTypeDef",
     {
         "Uid": int,
         "Gid": int,
     },
 )
@@ -116,34 +161,25 @@
     "_OptionalPosixUserTypeDef",
     {
         "SecondaryGids": Sequence[int],
     },
     total=False,
 )
 
-
 class PosixUserTypeDef(_RequiredPosixUserTypeDef, _OptionalPosixUserTypeDef):
     pass
 
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-BackupPolicyTypeDef = TypedDict(
-    "BackupPolicyTypeDef",
-    {
-        "Status": StatusType,
-    },
-)
-
 _RequiredCreateMountTargetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMountTargetRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "SubnetId": str,
     },
 )
@@ -152,31 +188,38 @@
     {
         "IpAddress": str,
         "SecurityGroups": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateMountTargetRequestRequestTypeDef(
     _RequiredCreateMountTargetRequestRequestTypeDef, _OptionalCreateMountTargetRequestRequestTypeDef
 ):
     pass
 
-
 DestinationToCreateTypeDef = TypedDict(
     "DestinationToCreateTypeDef",
     {
         "Region": str,
         "AvailabilityZoneName": str,
         "KmsKeyId": str,
     },
     total=False,
 )
 
+CreationInfoOutputTypeDef = TypedDict(
+    "CreationInfoOutputTypeDef",
+    {
+        "OwnerUid": int,
+        "OwnerGid": int,
+        "Permissions": str,
+    },
+)
+
 CreationInfoTypeDef = TypedDict(
     "CreationInfoTypeDef",
     {
         "OwnerUid": int,
         "OwnerGid": int,
         "Permissions": str,
     },
@@ -352,21 +395,19 @@
         "AvailabilityZoneId": str,
         "AvailabilityZoneName": str,
         "VpcId": str,
     },
     total=False,
 )
 
-
 class MountTargetDescriptionTypeDef(
     _RequiredMountTargetDescriptionTypeDef, _OptionalMountTargetDescriptionTypeDef
 ):
     pass
 
-
 DescribeReplicationConfigurationsRequestRequestTypeDef = TypedDict(
     "DescribeReplicationConfigurationsRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -383,22 +424,20 @@
     "_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeTagsRequestDescribeTagsPaginateTypeDef(
     _RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef,
     _OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeTagsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTagsRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalDescribeTagsRequestRequestTypeDef = TypedDict(
@@ -406,21 +445,19 @@
     {
         "MaxItems": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeTagsRequestRequestTypeDef(
     _RequiredDescribeTagsRequestRequestTypeDef, _OptionalDescribeTagsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDestinationTypeDef = TypedDict(
     "_RequiredDestinationTypeDef",
     {
         "Status": ReplicationStatusType,
         "FileSystemId": str,
         "Region": str,
     },
@@ -429,19 +466,17 @@
     "_OptionalDestinationTypeDef",
     {
         "LastReplicatedTimestamp": datetime,
     },
     total=False,
 )
 
-
 class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
     pass
 
-
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -457,28 +492,35 @@
         "Timestamp": datetime,
         "ValueInIA": int,
         "ValueInStandard": int,
     },
     total=False,
 )
 
-
 class FileSystemSizeTypeDef(_RequiredFileSystemSizeTypeDef, _OptionalFileSystemSizeTypeDef):
     pass
 
-
 FileSystemPolicyDescriptionTypeDef = TypedDict(
     "FileSystemPolicyDescriptionTypeDef",
     {
         "FileSystemId": str,
         "Policy": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LifecyclePolicyOutputTypeDef = TypedDict(
+    "LifecyclePolicyOutputTypeDef",
+    {
+        "TransitionToIA": TransitionToIARulesType,
+        "TransitionToPrimaryStorageClass": Literal["AFTER_1_ACCESS"],
+    },
+    total=False,
+)
+
 LifecyclePolicyTypeDef = TypedDict(
     "LifecyclePolicyTypeDef",
     {
         "TransitionToIA": TransitionToIARulesType,
         "TransitionToPrimaryStorageClass": Literal["AFTER_1_ACCESS"],
     },
     total=False,
@@ -495,44 +537,40 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyMountTargetSecurityGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredModifyMountTargetSecurityGroupsRequestRequestTypeDef",
     {
         "MountTargetId": str,
     },
 )
 _OptionalModifyMountTargetSecurityGroupsRequestRequestTypeDef = TypedDict(
     "_OptionalModifyMountTargetSecurityGroupsRequestRequestTypeDef",
     {
         "SecurityGroups": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyMountTargetSecurityGroupsRequestRequestTypeDef(
     _RequiredModifyMountTargetSecurityGroupsRequestRequestTypeDef,
     _OptionalModifyMountTargetSecurityGroupsRequestRequestTypeDef,
 ):
     pass
 
-
 MountTargetDescriptionResponseMetadataTypeDef = TypedDict(
     "MountTargetDescriptionResponseMetadataTypeDef",
     {
         "OwnerId": str,
         "MountTargetId": str,
         "FileSystemId": str,
         "SubnetId": str,
@@ -574,22 +612,20 @@
     "_OptionalPutFileSystemPolicyRequestRequestTypeDef",
     {
         "BypassPolicyLockoutSafetyCheck": bool,
     },
     total=False,
 )
 
-
 class PutFileSystemPolicyRequestRequestTypeDef(
     _RequiredPutFileSystemPolicyRequestRequestTypeDef,
     _OptionalPutFileSystemPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -616,20 +652,53 @@
     {
         "ThroughputMode": ThroughputModeType,
         "ProvisionedThroughputInMibps": float,
     },
     total=False,
 )
 
-
 class UpdateFileSystemRequestRequestTypeDef(
     _RequiredUpdateFileSystemRequestRequestTypeDef, _OptionalUpdateFileSystemRequestRequestTypeDef
 ):
     pass
 
+DescribeTagsResponseTypeDef = TypedDict(
+    "DescribeTagsResponseTypeDef",
+    {
+        "Marker": str,
+        "Tags": List[TagOutputTypeDef],
+        "NextMarker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BackupPolicyDescriptionTypeDef = TypedDict(
+    "BackupPolicyDescriptionTypeDef",
+    {
+        "BackupPolicy": BackupPolicyOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutBackupPolicyRequestRequestTypeDef = TypedDict(
+    "PutBackupPolicyRequestRequestTypeDef",
+    {
+        "FileSystemId": str,
+        "BackupPolicy": BackupPolicyTypeDef,
+    },
+)
 
 _RequiredCreateFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileSystemRequestRequestTypeDef",
     {
         "CreationToken": str,
     },
 )
@@ -644,80 +713,52 @@
         "AvailabilityZoneName": str,
         "Backup": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateFileSystemRequestRequestTypeDef(
     _RequiredCreateFileSystemRequestRequestTypeDef, _OptionalCreateFileSystemRequestRequestTypeDef
 ):
     pass
 
-
 CreateTagsRequestRequestTypeDef = TypedDict(
     "CreateTagsRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-DescribeTagsResponseTypeDef = TypedDict(
-    "DescribeTagsResponseTypeDef",
-    {
-        "Marker": str,
-        "Tags": List[TagTypeDef],
-        "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-BackupPolicyDescriptionTypeDef = TypedDict(
-    "BackupPolicyDescriptionTypeDef",
-    {
-        "BackupPolicy": BackupPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutBackupPolicyRequestRequestTypeDef = TypedDict(
-    "PutBackupPolicyRequestRequestTypeDef",
-    {
-        "FileSystemId": str,
-        "BackupPolicy": BackupPolicyTypeDef,
-    },
-)
-
 CreateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "CreateReplicationConfigurationRequestRequestTypeDef",
     {
         "SourceFileSystemId": str,
         "Destinations": Sequence[DestinationToCreateTypeDef],
     },
 )
 
+RootDirectoryOutputTypeDef = TypedDict(
+    "RootDirectoryOutputTypeDef",
+    {
+        "Path": str,
+        "CreationInfo": CreationInfoOutputTypeDef,
+    },
+    total=False,
+)
+
 RootDirectoryTypeDef = TypedDict(
     "RootDirectoryTypeDef",
     {
         "Path": str,
         "CreationInfo": CreationInfoTypeDef,
     },
     total=False,
@@ -790,15 +831,15 @@
         "PerformanceMode": PerformanceModeType,
         "Encrypted": bool,
         "KmsKeyId": str,
         "ThroughputMode": ThroughputModeType,
         "ProvisionedThroughputInMibps": float,
         "AvailabilityZoneName": str,
         "AvailabilityZoneId": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFileSystemDescriptionTypeDef = TypedDict(
     "_RequiredFileSystemDescriptionTypeDef",
     {
@@ -806,15 +847,15 @@
         "CreationToken": str,
         "FileSystemId": str,
         "CreationTime": datetime,
         "LifeCycleState": LifeCycleStateType,
         "NumberOfMountTargets": int,
         "SizeInBytes": FileSystemSizeTypeDef,
         "PerformanceMode": PerformanceModeType,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
 )
 _OptionalFileSystemDescriptionTypeDef = TypedDict(
     "_OptionalFileSystemDescriptionTypeDef",
     {
         "FileSystemArn": str,
         "Name": str,
@@ -824,25 +865,23 @@
         "ProvisionedThroughputInMibps": float,
         "AvailabilityZoneName": str,
         "AvailabilityZoneId": str,
     },
     total=False,
 )
 
-
 class FileSystemDescriptionTypeDef(
     _RequiredFileSystemDescriptionTypeDef, _OptionalFileSystemDescriptionTypeDef
 ):
     pass
 
-
 LifecycleConfigurationDescriptionTypeDef = TypedDict(
     "LifecycleConfigurationDescriptionTypeDef",
     {
-        "LifecyclePolicies": List[LifecyclePolicyTypeDef],
+        "LifecyclePolicies": List[LifecyclePolicyOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutLifecycleConfigurationRequestRequestTypeDef = TypedDict(
     "PutLifecycleConfigurationRequestRequestTypeDef",
     {
@@ -852,37 +891,37 @@
 )
 
 AccessPointDescriptionResponseMetadataTypeDef = TypedDict(
     "AccessPointDescriptionResponseMetadataTypeDef",
     {
         "ClientToken": str,
         "Name": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "AccessPointId": str,
         "AccessPointArn": str,
         "FileSystemId": str,
-        "PosixUser": PosixUserTypeDef,
-        "RootDirectory": RootDirectoryTypeDef,
+        "PosixUser": PosixUserOutputTypeDef,
+        "RootDirectory": RootDirectoryOutputTypeDef,
         "OwnerId": str,
         "LifeCycleState": LifeCycleStateType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AccessPointDescriptionTypeDef = TypedDict(
     "AccessPointDescriptionTypeDef",
     {
         "ClientToken": str,
         "Name": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "AccessPointId": str,
         "AccessPointArn": str,
         "FileSystemId": str,
-        "PosixUser": PosixUserTypeDef,
-        "RootDirectory": RootDirectoryTypeDef,
+        "PosixUser": PosixUserOutputTypeDef,
+        "RootDirectory": RootDirectoryOutputTypeDef,
         "OwnerId": str,
         "LifeCycleState": LifeCycleStateType,
     },
     total=False,
 )
 
 _RequiredCreateAccessPointRequestRequestTypeDef = TypedDict(
@@ -898,21 +937,19 @@
         "Tags": Sequence[TagTypeDef],
         "PosixUser": PosixUserTypeDef,
         "RootDirectory": RootDirectoryTypeDef,
     },
     total=False,
 )
 
-
 class CreateAccessPointRequestRequestTypeDef(
     _RequiredCreateAccessPointRequestRequestTypeDef, _OptionalCreateAccessPointRequestRequestTypeDef
 ):
     pass
 
-
 DescribeReplicationConfigurationsResponseTypeDef = TypedDict(
     "DescribeReplicationConfigurationsResponseTypeDef",
     {
         "Replications": List[ReplicationConfigurationDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-efs-1.28.0/mypy_boto3_efs/type_defs.pyi` & `mypy-boto3-efs-1.28.12/mypy_boto3_efs/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for efs service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_efs.type_defs import PosixUserTypeDef
+    from mypy_boto3_efs.type_defs import PosixUserOutputTypeDef
 
-    data: PosixUserTypeDef = {...}
+    data: PosixUserOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -31,20 +31,25 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "PosixUserOutputTypeDef",
+    "TagOutputTypeDef",
+    "BackupPolicyOutputTypeDef",
+    "BackupPolicyTypeDef",
     "PosixUserTypeDef",
     "TagTypeDef",
-    "BackupPolicyTypeDef",
     "CreateMountTargetRequestRequestTypeDef",
     "DestinationToCreateTypeDef",
+    "CreationInfoOutputTypeDef",
     "CreationInfoTypeDef",
     "DeleteAccessPointRequestRequestTypeDef",
     "DeleteFileSystemPolicyRequestRequestTypeDef",
     "DeleteFileSystemRequestRequestTypeDef",
     "DeleteMountTargetRequestRequestTypeDef",
     "DeleteReplicationConfigurationRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
@@ -64,32 +69,34 @@
     "DescribeReplicationConfigurationsRequestRequestTypeDef",
     "DescribeTagsRequestDescribeTagsPaginateTypeDef",
     "DescribeTagsRequestRequestTypeDef",
     "DestinationTypeDef",
     "EmptyResponseMetadataTypeDef",
     "FileSystemSizeTypeDef",
     "FileSystemPolicyDescriptionTypeDef",
+    "LifecyclePolicyOutputTypeDef",
     "LifecyclePolicyTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ModifyMountTargetSecurityGroupsRequestRequestTypeDef",
     "MountTargetDescriptionResponseMetadataTypeDef",
     "PaginatorConfigTypeDef",
     "PutAccountPreferencesRequestRequestTypeDef",
     "PutFileSystemPolicyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFileSystemRequestRequestTypeDef",
-    "CreateFileSystemRequestRequestTypeDef",
-    "CreateTagsRequestRequestTypeDef",
     "DescribeTagsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "BackupPolicyDescriptionTypeDef",
     "PutBackupPolicyRequestRequestTypeDef",
+    "CreateFileSystemRequestRequestTypeDef",
+    "CreateTagsRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateReplicationConfigurationRequestRequestTypeDef",
+    "RootDirectoryOutputTypeDef",
     "RootDirectoryTypeDef",
     "DescribeAccountPreferencesResponseTypeDef",
     "PutAccountPreferencesResponseTypeDef",
     "DescribeMountTargetsResponseTypeDef",
     "ReplicationConfigurationDescriptionResponseMetadataTypeDef",
     "ReplicationConfigurationDescriptionTypeDef",
     "FileSystemDescriptionResponseMetadataTypeDef",
@@ -100,14 +107,56 @@
     "AccessPointDescriptionTypeDef",
     "CreateAccessPointRequestRequestTypeDef",
     "DescribeReplicationConfigurationsResponseTypeDef",
     "DescribeFileSystemsResponseTypeDef",
     "DescribeAccessPointsResponseTypeDef",
 )
 
+_RequiredPosixUserOutputTypeDef = TypedDict(
+    "_RequiredPosixUserOutputTypeDef",
+    {
+        "Uid": int,
+        "Gid": int,
+    },
+)
+_OptionalPosixUserOutputTypeDef = TypedDict(
+    "_OptionalPosixUserOutputTypeDef",
+    {
+        "SecondaryGids": List[int],
+    },
+    total=False,
+)
+
+
+class PosixUserOutputTypeDef(_RequiredPosixUserOutputTypeDef, _OptionalPosixUserOutputTypeDef):
+    pass
+
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+BackupPolicyOutputTypeDef = TypedDict(
+    "BackupPolicyOutputTypeDef",
+    {
+        "Status": StatusType,
+    },
+)
+
+BackupPolicyTypeDef = TypedDict(
+    "BackupPolicyTypeDef",
+    {
+        "Status": StatusType,
+    },
+)
+
 _RequiredPosixUserTypeDef = TypedDict(
     "_RequiredPosixUserTypeDef",
     {
         "Uid": int,
         "Gid": int,
     },
 )
@@ -115,32 +164,27 @@
     "_OptionalPosixUserTypeDef",
     {
         "SecondaryGids": Sequence[int],
     },
     total=False,
 )
 
+
 class PosixUserTypeDef(_RequiredPosixUserTypeDef, _OptionalPosixUserTypeDef):
     pass
 
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-BackupPolicyTypeDef = TypedDict(
-    "BackupPolicyTypeDef",
-    {
-        "Status": StatusType,
-    },
-)
-
 _RequiredCreateMountTargetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMountTargetRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "SubnetId": str,
     },
 )
@@ -149,29 +193,40 @@
     {
         "IpAddress": str,
         "SecurityGroups": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateMountTargetRequestRequestTypeDef(
     _RequiredCreateMountTargetRequestRequestTypeDef, _OptionalCreateMountTargetRequestRequestTypeDef
 ):
     pass
 
+
 DestinationToCreateTypeDef = TypedDict(
     "DestinationToCreateTypeDef",
     {
         "Region": str,
         "AvailabilityZoneName": str,
         "KmsKeyId": str,
     },
     total=False,
 )
 
+CreationInfoOutputTypeDef = TypedDict(
+    "CreationInfoOutputTypeDef",
+    {
+        "OwnerUid": int,
+        "OwnerGid": int,
+        "Permissions": str,
+    },
+)
+
 CreationInfoTypeDef = TypedDict(
     "CreationInfoTypeDef",
     {
         "OwnerUid": int,
         "OwnerGid": int,
         "Permissions": str,
     },
@@ -347,19 +402,21 @@
         "AvailabilityZoneId": str,
         "AvailabilityZoneName": str,
         "VpcId": str,
     },
     total=False,
 )
 
+
 class MountTargetDescriptionTypeDef(
     _RequiredMountTargetDescriptionTypeDef, _OptionalMountTargetDescriptionTypeDef
 ):
     pass
 
+
 DescribeReplicationConfigurationsRequestRequestTypeDef = TypedDict(
     "DescribeReplicationConfigurationsRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -376,20 +433,22 @@
     "_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeTagsRequestDescribeTagsPaginateTypeDef(
     _RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef,
     _OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeTagsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTagsRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalDescribeTagsRequestRequestTypeDef = TypedDict(
@@ -397,19 +456,21 @@
     {
         "MaxItems": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeTagsRequestRequestTypeDef(
     _RequiredDescribeTagsRequestRequestTypeDef, _OptionalDescribeTagsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDestinationTypeDef = TypedDict(
     "_RequiredDestinationTypeDef",
     {
         "Status": ReplicationStatusType,
         "FileSystemId": str,
         "Region": str,
     },
@@ -418,17 +479,19 @@
     "_OptionalDestinationTypeDef",
     {
         "LastReplicatedTimestamp": datetime,
     },
     total=False,
 )
 
+
 class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
     pass
 
+
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -444,26 +507,37 @@
         "Timestamp": datetime,
         "ValueInIA": int,
         "ValueInStandard": int,
     },
     total=False,
 )
 
+
 class FileSystemSizeTypeDef(_RequiredFileSystemSizeTypeDef, _OptionalFileSystemSizeTypeDef):
     pass
 
+
 FileSystemPolicyDescriptionTypeDef = TypedDict(
     "FileSystemPolicyDescriptionTypeDef",
     {
         "FileSystemId": str,
         "Policy": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LifecyclePolicyOutputTypeDef = TypedDict(
+    "LifecyclePolicyOutputTypeDef",
+    {
+        "TransitionToIA": TransitionToIARulesType,
+        "TransitionToPrimaryStorageClass": Literal["AFTER_1_ACCESS"],
+    },
+    total=False,
+)
+
 LifecyclePolicyTypeDef = TypedDict(
     "LifecyclePolicyTypeDef",
     {
         "TransitionToIA": TransitionToIARulesType,
         "TransitionToPrimaryStorageClass": Literal["AFTER_1_ACCESS"],
     },
     total=False,
@@ -480,40 +554,44 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyMountTargetSecurityGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredModifyMountTargetSecurityGroupsRequestRequestTypeDef",
     {
         "MountTargetId": str,
     },
 )
 _OptionalModifyMountTargetSecurityGroupsRequestRequestTypeDef = TypedDict(
     "_OptionalModifyMountTargetSecurityGroupsRequestRequestTypeDef",
     {
         "SecurityGroups": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyMountTargetSecurityGroupsRequestRequestTypeDef(
     _RequiredModifyMountTargetSecurityGroupsRequestRequestTypeDef,
     _OptionalModifyMountTargetSecurityGroupsRequestRequestTypeDef,
 ):
     pass
 
+
 MountTargetDescriptionResponseMetadataTypeDef = TypedDict(
     "MountTargetDescriptionResponseMetadataTypeDef",
     {
         "OwnerId": str,
         "MountTargetId": str,
         "FileSystemId": str,
         "SubnetId": str,
@@ -555,20 +633,22 @@
     "_OptionalPutFileSystemPolicyRequestRequestTypeDef",
     {
         "BypassPolicyLockoutSafetyCheck": bool,
     },
     total=False,
 )
 
+
 class PutFileSystemPolicyRequestRequestTypeDef(
     _RequiredPutFileSystemPolicyRequestRequestTypeDef,
     _OptionalPutFileSystemPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -595,19 +675,56 @@
     {
         "ThroughputMode": ThroughputModeType,
         "ProvisionedThroughputInMibps": float,
     },
     total=False,
 )
 
+
 class UpdateFileSystemRequestRequestTypeDef(
     _RequiredUpdateFileSystemRequestRequestTypeDef, _OptionalUpdateFileSystemRequestRequestTypeDef
 ):
     pass
 
+
+DescribeTagsResponseTypeDef = TypedDict(
+    "DescribeTagsResponseTypeDef",
+    {
+        "Marker": str,
+        "Tags": List[TagOutputTypeDef],
+        "NextMarker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BackupPolicyDescriptionTypeDef = TypedDict(
+    "BackupPolicyDescriptionTypeDef",
+    {
+        "BackupPolicy": BackupPolicyOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutBackupPolicyRequestRequestTypeDef = TypedDict(
+    "PutBackupPolicyRequestRequestTypeDef",
+    {
+        "FileSystemId": str,
+        "BackupPolicy": BackupPolicyTypeDef,
+    },
+)
+
 _RequiredCreateFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileSystemRequestRequestTypeDef",
     {
         "CreationToken": str,
     },
 )
 _OptionalCreateFileSystemRequestRequestTypeDef = TypedDict(
@@ -621,78 +738,54 @@
         "AvailabilityZoneName": str,
         "Backup": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateFileSystemRequestRequestTypeDef(
     _RequiredCreateFileSystemRequestRequestTypeDef, _OptionalCreateFileSystemRequestRequestTypeDef
 ):
     pass
 
+
 CreateTagsRequestRequestTypeDef = TypedDict(
     "CreateTagsRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-DescribeTagsResponseTypeDef = TypedDict(
-    "DescribeTagsResponseTypeDef",
-    {
-        "Marker": str,
-        "Tags": List[TagTypeDef],
-        "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-BackupPolicyDescriptionTypeDef = TypedDict(
-    "BackupPolicyDescriptionTypeDef",
-    {
-        "BackupPolicy": BackupPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutBackupPolicyRequestRequestTypeDef = TypedDict(
-    "PutBackupPolicyRequestRequestTypeDef",
-    {
-        "FileSystemId": str,
-        "BackupPolicy": BackupPolicyTypeDef,
-    },
-)
-
 CreateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "CreateReplicationConfigurationRequestRequestTypeDef",
     {
         "SourceFileSystemId": str,
         "Destinations": Sequence[DestinationToCreateTypeDef],
     },
 )
 
+RootDirectoryOutputTypeDef = TypedDict(
+    "RootDirectoryOutputTypeDef",
+    {
+        "Path": str,
+        "CreationInfo": CreationInfoOutputTypeDef,
+    },
+    total=False,
+)
+
 RootDirectoryTypeDef = TypedDict(
     "RootDirectoryTypeDef",
     {
         "Path": str,
         "CreationInfo": CreationInfoTypeDef,
     },
     total=False,
@@ -765,15 +858,15 @@
         "PerformanceMode": PerformanceModeType,
         "Encrypted": bool,
         "KmsKeyId": str,
         "ThroughputMode": ThroughputModeType,
         "ProvisionedThroughputInMibps": float,
         "AvailabilityZoneName": str,
         "AvailabilityZoneId": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFileSystemDescriptionTypeDef = TypedDict(
     "_RequiredFileSystemDescriptionTypeDef",
     {
@@ -781,15 +874,15 @@
         "CreationToken": str,
         "FileSystemId": str,
         "CreationTime": datetime,
         "LifeCycleState": LifeCycleStateType,
         "NumberOfMountTargets": int,
         "SizeInBytes": FileSystemSizeTypeDef,
         "PerformanceMode": PerformanceModeType,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
 )
 _OptionalFileSystemDescriptionTypeDef = TypedDict(
     "_OptionalFileSystemDescriptionTypeDef",
     {
         "FileSystemArn": str,
         "Name": str,
@@ -799,23 +892,25 @@
         "ProvisionedThroughputInMibps": float,
         "AvailabilityZoneName": str,
         "AvailabilityZoneId": str,
     },
     total=False,
 )
 
+
 class FileSystemDescriptionTypeDef(
     _RequiredFileSystemDescriptionTypeDef, _OptionalFileSystemDescriptionTypeDef
 ):
     pass
 
+
 LifecycleConfigurationDescriptionTypeDef = TypedDict(
     "LifecycleConfigurationDescriptionTypeDef",
     {
-        "LifecyclePolicies": List[LifecyclePolicyTypeDef],
+        "LifecyclePolicies": List[LifecyclePolicyOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutLifecycleConfigurationRequestRequestTypeDef = TypedDict(
     "PutLifecycleConfigurationRequestRequestTypeDef",
     {
@@ -825,37 +920,37 @@
 )
 
 AccessPointDescriptionResponseMetadataTypeDef = TypedDict(
     "AccessPointDescriptionResponseMetadataTypeDef",
     {
         "ClientToken": str,
         "Name": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "AccessPointId": str,
         "AccessPointArn": str,
         "FileSystemId": str,
-        "PosixUser": PosixUserTypeDef,
-        "RootDirectory": RootDirectoryTypeDef,
+        "PosixUser": PosixUserOutputTypeDef,
+        "RootDirectory": RootDirectoryOutputTypeDef,
         "OwnerId": str,
         "LifeCycleState": LifeCycleStateType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AccessPointDescriptionTypeDef = TypedDict(
     "AccessPointDescriptionTypeDef",
     {
         "ClientToken": str,
         "Name": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "AccessPointId": str,
         "AccessPointArn": str,
         "FileSystemId": str,
-        "PosixUser": PosixUserTypeDef,
-        "RootDirectory": RootDirectoryTypeDef,
+        "PosixUser": PosixUserOutputTypeDef,
+        "RootDirectory": RootDirectoryOutputTypeDef,
         "OwnerId": str,
         "LifeCycleState": LifeCycleStateType,
     },
     total=False,
 )
 
 _RequiredCreateAccessPointRequestRequestTypeDef = TypedDict(
@@ -871,19 +966,21 @@
         "Tags": Sequence[TagTypeDef],
         "PosixUser": PosixUserTypeDef,
         "RootDirectory": RootDirectoryTypeDef,
     },
     total=False,
 )
 
+
 class CreateAccessPointRequestRequestTypeDef(
     _RequiredCreateAccessPointRequestRequestTypeDef, _OptionalCreateAccessPointRequestRequestTypeDef
 ):
     pass
 
+
 DescribeReplicationConfigurationsResponseTypeDef = TypedDict(
     "DescribeReplicationConfigurationsResponseTypeDef",
     {
         "Replications": List[ReplicationConfigurationDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-efs-1.28.0/mypy_boto3_efs.egg-info/PKG-INFO` & `mypy-boto3-efs-1.28.12/mypy_boto3_efs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-efs
-Version: 1.28.0
-Summary: Type annotations for boto3.EFS 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.EFS 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-efs"></a>
 
 # mypy-boto3-efs
 
 [![PyPI - mypy-boto3-efs](https://img.shields.io/pypi/v/mypy-boto3-efs.svg?color=blue)](https://pypi.org/project/mypy-boto3-efs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-efs.svg?color=blue)](https://pypi.org/project/mypy-boto3-efs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-efs?color=blue)](https://pypistats.org/packages/mypy-boto3-efs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-efs)](https://pepy.tech/project/mypy-boto3-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EFS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
+[boto3.EFS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
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
 [mypy-boto3-efs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,19 +338,23 @@
 ### Typed dictionaries
 
 `mypy_boto3_efs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_efs.type_defs import (
+    PosixUserOutputTypeDef,
+    TagOutputTypeDef,
+    BackupPolicyOutputTypeDef,
+    BackupPolicyTypeDef,
     PosixUserTypeDef,
     TagTypeDef,
-    BackupPolicyTypeDef,
     CreateMountTargetRequestRequestTypeDef,
     DestinationToCreateTypeDef,
+    CreationInfoOutputTypeDef,
     CreationInfoTypeDef,
     DeleteAccessPointRequestRequestTypeDef,
     DeleteFileSystemPolicyRequestRequestTypeDef,
     DeleteFileSystemRequestRequestTypeDef,
     DeleteMountTargetRequestRequestTypeDef,
     DeleteReplicationConfigurationRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
@@ -370,32 +374,34 @@
     DescribeReplicationConfigurationsRequestRequestTypeDef,
     DescribeTagsRequestDescribeTagsPaginateTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DestinationTypeDef,
     EmptyResponseMetadataTypeDef,
     FileSystemSizeTypeDef,
     FileSystemPolicyDescriptionTypeDef,
+    LifecyclePolicyOutputTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModifyMountTargetSecurityGroupsRequestRequestTypeDef,
     MountTargetDescriptionResponseMetadataTypeDef,
     PaginatorConfigTypeDef,
     PutAccountPreferencesRequestRequestTypeDef,
     PutFileSystemPolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileSystemRequestRequestTypeDef,
-    CreateFileSystemRequestRequestTypeDef,
-    CreateTagsRequestRequestTypeDef,
     DescribeTagsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     BackupPolicyDescriptionTypeDef,
     PutBackupPolicyRequestRequestTypeDef,
+    CreateFileSystemRequestRequestTypeDef,
+    CreateTagsRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateReplicationConfigurationRequestRequestTypeDef,
+    RootDirectoryOutputTypeDef,
     RootDirectoryTypeDef,
     DescribeAccountPreferencesResponseTypeDef,
     PutAccountPreferencesResponseTypeDef,
     DescribeMountTargetsResponseTypeDef,
     ReplicationConfigurationDescriptionResponseMetadataTypeDef,
     ReplicationConfigurationDescriptionTypeDef,
     FileSystemDescriptionResponseMetadataTypeDef,
@@ -407,15 +413,15 @@
     CreateAccessPointRequestRequestTypeDef,
     DescribeReplicationConfigurationsResponseTypeDef,
     DescribeFileSystemsResponseTypeDef,
     DescribeAccessPointsResponseTypeDef,
 )
 
 
-def get_structure() -> PosixUserTypeDef:
+def get_structure() -> PosixUserOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-efs-1.28.0/mypy_boto3_efs.egg-info/SOURCES.txt` & `mypy-boto3-efs-1.28.12/mypy_boto3_efs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.0/setup.py` & `mypy-boto3-efs-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-efs",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_efs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EFS 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.EFS 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

