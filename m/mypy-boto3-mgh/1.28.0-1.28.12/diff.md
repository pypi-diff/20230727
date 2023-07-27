# Comparing `tmp/mypy-boto3-mgh-1.28.0.tar.gz` & `tmp/mypy-boto3-mgh-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mgh-1.28.0.tar", last modified: Thu Jul  6 21:00:08 2023, max compression
+gzip compressed data, was "mypy-boto3-mgh-1.28.12.tar", last modified: Thu Jul 27 05:35:02 2023, max compression
```

## Comparing `mypy-boto3-mgh-1.28.0.tar` & `mypy-boto3-mgh-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:08.578372 mypy-boto3-mgh-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:47:36.000000 mypy-boto3-mgh-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15051 2023-07-06 21:00:08.574372 mypy-boto3-mgh-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13573 2023-07-06 20:47:36.000000 mypy-boto3-mgh-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:08.570372 mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-06 20:47:36.000000 mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-06 20:47:36.000000 mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-06 20:47:36.000000 mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17205 2023-07-06 20:47:36.000000 mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-07-06 20:47:36.000000 mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-07-06 20:47:37.000000 mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-06 20:47:37.000000 mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-07-06 20:47:36.000000 mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-07-06 20:47:36.000000 mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:47:36.000000 mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-07-06 20:47:37.000000 mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-07-06 20:47:37.000000 mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:47:36.000000 mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:08.574372 mypy-boto3-mgh-1.28.0/mypy_boto3_mgh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15051 2023-07-06 21:00:08.000000 mypy-boto3-mgh-1.28.0/mypy_boto3_mgh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 21:00:08.000000 mypy-boto3-mgh-1.28.0/mypy_boto3_mgh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:08.000000 mypy-boto3-mgh-1.28.0/mypy_boto3_mgh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:08.000000 mypy-boto3-mgh-1.28.0/mypy_boto3_mgh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:08.000000 mypy-boto3-mgh-1.28.0/mypy_boto3_mgh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 21:00:08.000000 mypy-boto3-mgh-1.28.0/mypy_boto3_mgh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:08.578372 mypy-boto3-mgh-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-06 20:47:36.000000 mypy-boto3-mgh-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.868434 mypy-boto3-mgh-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:33.000000 mypy-boto3-mgh-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15168 2023-07-27 05:35:02.868434 mypy-boto3-mgh-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-07-27 05:26:33.000000 mypy-boto3-mgh-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.864434 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-27 05:26:33.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-27 05:26:33.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-27 05:26:33.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17205 2023-07-27 05:26:34.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-07-27 05:26:33.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-07-27 05:26:34.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-07-27 05:26:34.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-07-27 05:26:34.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-07-27 05:26:34.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:33.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-07-27 05:26:34.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19226 2023-07-27 05:26:34.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:33.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.868434 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15168 2023-07-27 05:35:02.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 05:35:02.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:02.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:02.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:02.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:35:02.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:02.868434 mypy-boto3-mgh-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-27 05:26:33.000000 mypy-boto3-mgh-1.28.12/setup.py
```

### Comparing `mypy-boto3-mgh-1.28.0/LICENSE` & `mypy-boto3-mgh-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.0/PKG-INFO` & `mypy-boto3-mgh-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mgh
-Version: 1.28.0
-Summary: Type annotations for boto3.MigrationHub 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MigrationHub 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mgh"></a>
 
 # mypy-boto3-mgh
 
 [![PyPI - mypy-boto3-mgh](https://img.shields.io/pypi/v/mypy-boto3-mgh.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgh.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgh)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mgh?color=blue)](https://pypistats.org/packages/mypy-boto3-mgh)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mgh)](https://pepy.tech/project/mypy-boto3-mgh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHub 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
+[boto3.MigrationHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
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
 [mypy-boto3-mgh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/).
 
 See how it helps to find and fix potential bugs:
 
@@ -348,48 +348,52 @@
 
 ```python
 from mypy_boto3_mgh.type_defs import (
     ApplicationStateTypeDef,
     CreatedArtifactTypeDef,
     DiscoveredResourceTypeDef,
     CreateProgressUpdateStreamRequestRequestTypeDef,
+    CreatedArtifactOutputTypeDef,
     DeleteProgressUpdateStreamRequestRequestTypeDef,
     DescribeApplicationStateRequestRequestTypeDef,
     DescribeApplicationStateResultTypeDef,
     DescribeMigrationTaskRequestRequestTypeDef,
     DisassociateCreatedArtifactRequestRequestTypeDef,
     DisassociateDiscoveredResourceRequestRequestTypeDef,
+    DiscoveredResourceOutputTypeDef,
     ImportMigrationTaskRequestRequestTypeDef,
     ListApplicationStatesRequestListApplicationStatesPaginateTypeDef,
     ListApplicationStatesRequestRequestTypeDef,
     ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
     ListCreatedArtifactsRequestRequestTypeDef,
     ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
     ListMigrationTasksRequestListMigrationTasksPaginateTypeDef,
     ListMigrationTasksRequestRequestTypeDef,
     MigrationTaskSummaryTypeDef,
     ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef,
     ListProgressUpdateStreamsRequestRequestTypeDef,
     ProgressUpdateStreamSummaryTypeDef,
-    ResourceAttributeTypeDef,
-    TaskTypeDef,
+    ResourceAttributeOutputTypeDef,
+    TaskOutputTypeDef,
     NotifyApplicationStateRequestRequestTypeDef,
+    TaskTypeDef,
     PaginatorConfigTypeDef,
+    ResourceAttributeTypeDef,
     ResponseMetadataTypeDef,
     ListApplicationStatesResultTypeDef,
     AssociateCreatedArtifactRequestRequestTypeDef,
-    ListCreatedArtifactsResultTypeDef,
     AssociateDiscoveredResourceRequestRequestTypeDef,
+    ListCreatedArtifactsResultTypeDef,
     ListDiscoveredResourcesResultTypeDef,
     ListMigrationTasksResultTypeDef,
     ListProgressUpdateStreamsResultTypeDef,
-    PutResourceAttributesRequestRequestTypeDef,
     MigrationTaskTypeDef,
     NotifyMigrationTaskStateRequestRequestTypeDef,
+    PutResourceAttributesRequestRequestTypeDef,
     DescribeMigrationTaskResultTypeDef,
 )
 
 
 def get_structure() -> ApplicationStateTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-mgh-1.28.0/README.md` & `mypy-boto3-mgh-1.28.12/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-mgh"></a>
 
 # mypy-boto3-mgh
 
 [![PyPI - mypy-boto3-mgh](https://img.shields.io/pypi/v/mypy-boto3-mgh.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgh.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgh)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mgh?color=blue)](https://pypistats.org/packages/mypy-boto3-mgh)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mgh)](https://pepy.tech/project/mypy-boto3-mgh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHub 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
+[boto3.MigrationHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
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
 [mypy-boto3-mgh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/).
 
 See how it helps to find and fix potential bugs:
 
@@ -316,48 +316,52 @@
 
 ```python
 from mypy_boto3_mgh.type_defs import (
     ApplicationStateTypeDef,
     CreatedArtifactTypeDef,
     DiscoveredResourceTypeDef,
     CreateProgressUpdateStreamRequestRequestTypeDef,
+    CreatedArtifactOutputTypeDef,
     DeleteProgressUpdateStreamRequestRequestTypeDef,
     DescribeApplicationStateRequestRequestTypeDef,
     DescribeApplicationStateResultTypeDef,
     DescribeMigrationTaskRequestRequestTypeDef,
     DisassociateCreatedArtifactRequestRequestTypeDef,
     DisassociateDiscoveredResourceRequestRequestTypeDef,
+    DiscoveredResourceOutputTypeDef,
     ImportMigrationTaskRequestRequestTypeDef,
     ListApplicationStatesRequestListApplicationStatesPaginateTypeDef,
     ListApplicationStatesRequestRequestTypeDef,
     ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
     ListCreatedArtifactsRequestRequestTypeDef,
     ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
     ListMigrationTasksRequestListMigrationTasksPaginateTypeDef,
     ListMigrationTasksRequestRequestTypeDef,
     MigrationTaskSummaryTypeDef,
     ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef,
     ListProgressUpdateStreamsRequestRequestTypeDef,
     ProgressUpdateStreamSummaryTypeDef,
-    ResourceAttributeTypeDef,
-    TaskTypeDef,
+    ResourceAttributeOutputTypeDef,
+    TaskOutputTypeDef,
     NotifyApplicationStateRequestRequestTypeDef,
+    TaskTypeDef,
     PaginatorConfigTypeDef,
+    ResourceAttributeTypeDef,
     ResponseMetadataTypeDef,
     ListApplicationStatesResultTypeDef,
     AssociateCreatedArtifactRequestRequestTypeDef,
-    ListCreatedArtifactsResultTypeDef,
     AssociateDiscoveredResourceRequestRequestTypeDef,
+    ListCreatedArtifactsResultTypeDef,
     ListDiscoveredResourcesResultTypeDef,
     ListMigrationTasksResultTypeDef,
     ListProgressUpdateStreamsResultTypeDef,
-    PutResourceAttributesRequestRequestTypeDef,
     MigrationTaskTypeDef,
     NotifyMigrationTaskStateRequestRequestTypeDef,
+    PutResourceAttributesRequestRequestTypeDef,
     DescribeMigrationTaskResultTypeDef,
 )
 
 
 def get_structure() -> ApplicationStateTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/__init__.py` & `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/__init__.pyi` & `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/__main__.py` & `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MigrationHub 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.MigrationHub 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub\nOther"
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

### Comparing `mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/client.py` & `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/client.pyi` & `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/literals.py` & `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ApplicationStatusType",
     "ListApplicationStatesPaginatorName",
     "ListCreatedArtifactsPaginatorName",
     "ListDiscoveredResourcesPaginatorName",
     "ListMigrationTasksPaginatorName",
     "ListProgressUpdateStreamsPaginatorName",
@@ -31,15 +30,14 @@
     "MigrationHubServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApplicationStatusType = Literal["COMPLETED", "IN_PROGRESS", "NOT_STARTED"]
 ListApplicationStatesPaginatorName = Literal["list_application_states"]
 ListCreatedArtifactsPaginatorName = Literal["list_created_artifacts"]
 ListDiscoveredResourcesPaginatorName = Literal["list_discovered_resources"]
 ListMigrationTasksPaginatorName = Literal["list_migration_tasks"]
 ListProgressUpdateStreamsPaginatorName = Literal["list_progress_update_streams"]
 ResourceAttributeTypeType = Literal[
@@ -171,14 +169,15 @@
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
@@ -257,26 +256,28 @@
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

### Comparing `mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/literals.pyi` & `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/literals.py`

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
     "ApplicationStatusType",
     "ListApplicationStatesPaginatorName",
     "ListCreatedArtifactsPaginatorName",
     "ListDiscoveredResourcesPaginatorName",
     "ListMigrationTasksPaginatorName",
     "ListProgressUpdateStreamsPaginatorName",
@@ -30,14 +31,15 @@
     "MigrationHubServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ApplicationStatusType = Literal["COMPLETED", "IN_PROGRESS", "NOT_STARTED"]
 ListApplicationStatesPaginatorName = Literal["list_application_states"]
 ListCreatedArtifactsPaginatorName = Literal["list_created_artifacts"]
 ListDiscoveredResourcesPaginatorName = Literal["list_discovered_resources"]
 ListMigrationTasksPaginatorName = Literal["list_migration_tasks"]
 ListProgressUpdateStreamsPaginatorName = Literal["list_progress_update_streams"]
 ResourceAttributeTypeType = Literal[
@@ -169,14 +171,15 @@
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
@@ -255,26 +258,28 @@
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

### Comparing `mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/paginator.py` & `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/paginator.pyi` & `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/type_defs.py` & `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,48 +24,52 @@
 
 
 __all__ = (
     "ApplicationStateTypeDef",
     "CreatedArtifactTypeDef",
     "DiscoveredResourceTypeDef",
     "CreateProgressUpdateStreamRequestRequestTypeDef",
+    "CreatedArtifactOutputTypeDef",
     "DeleteProgressUpdateStreamRequestRequestTypeDef",
     "DescribeApplicationStateRequestRequestTypeDef",
     "DescribeApplicationStateResultTypeDef",
     "DescribeMigrationTaskRequestRequestTypeDef",
     "DisassociateCreatedArtifactRequestRequestTypeDef",
     "DisassociateDiscoveredResourceRequestRequestTypeDef",
+    "DiscoveredResourceOutputTypeDef",
     "ImportMigrationTaskRequestRequestTypeDef",
     "ListApplicationStatesRequestListApplicationStatesPaginateTypeDef",
     "ListApplicationStatesRequestRequestTypeDef",
     "ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
     "ListCreatedArtifactsRequestRequestTypeDef",
     "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     "ListDiscoveredResourcesRequestRequestTypeDef",
     "ListMigrationTasksRequestListMigrationTasksPaginateTypeDef",
     "ListMigrationTasksRequestRequestTypeDef",
     "MigrationTaskSummaryTypeDef",
     "ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef",
     "ListProgressUpdateStreamsRequestRequestTypeDef",
     "ProgressUpdateStreamSummaryTypeDef",
-    "ResourceAttributeTypeDef",
-    "TaskTypeDef",
+    "ResourceAttributeOutputTypeDef",
+    "TaskOutputTypeDef",
     "NotifyApplicationStateRequestRequestTypeDef",
+    "TaskTypeDef",
     "PaginatorConfigTypeDef",
+    "ResourceAttributeTypeDef",
     "ResponseMetadataTypeDef",
     "ListApplicationStatesResultTypeDef",
     "AssociateCreatedArtifactRequestRequestTypeDef",
-    "ListCreatedArtifactsResultTypeDef",
     "AssociateDiscoveredResourceRequestRequestTypeDef",
+    "ListCreatedArtifactsResultTypeDef",
     "ListDiscoveredResourcesResultTypeDef",
     "ListMigrationTasksResultTypeDef",
     "ListProgressUpdateStreamsResultTypeDef",
-    "PutResourceAttributesRequestRequestTypeDef",
     "MigrationTaskTypeDef",
     "NotifyMigrationTaskStateRequestRequestTypeDef",
+    "PutResourceAttributesRequestRequestTypeDef",
     "DescribeMigrationTaskResultTypeDef",
 )
 
 ApplicationStateTypeDef = TypedDict(
     "ApplicationStateTypeDef",
     {
         "ApplicationId": str,
@@ -133,14 +137,35 @@
 class CreateProgressUpdateStreamRequestRequestTypeDef(
     _RequiredCreateProgressUpdateStreamRequestRequestTypeDef,
     _OptionalCreateProgressUpdateStreamRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredCreatedArtifactOutputTypeDef = TypedDict(
+    "_RequiredCreatedArtifactOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreatedArtifactOutputTypeDef = TypedDict(
+    "_OptionalCreatedArtifactOutputTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+
+class CreatedArtifactOutputTypeDef(
+    _RequiredCreatedArtifactOutputTypeDef, _OptionalCreatedArtifactOutputTypeDef
+):
+    pass
+
+
 _RequiredDeleteProgressUpdateStreamRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteProgressUpdateStreamRequestRequestTypeDef",
     {
         "ProgressUpdateStreamName": str,
     },
 )
 _OptionalDeleteProgressUpdateStreamRequestRequestTypeDef = TypedDict(
@@ -227,14 +252,35 @@
 class DisassociateDiscoveredResourceRequestRequestTypeDef(
     _RequiredDisassociateDiscoveredResourceRequestRequestTypeDef,
     _OptionalDisassociateDiscoveredResourceRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredDiscoveredResourceOutputTypeDef = TypedDict(
+    "_RequiredDiscoveredResourceOutputTypeDef",
+    {
+        "ConfigurationId": str,
+    },
+)
+_OptionalDiscoveredResourceOutputTypeDef = TypedDict(
+    "_OptionalDiscoveredResourceOutputTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+
+class DiscoveredResourceOutputTypeDef(
+    _RequiredDiscoveredResourceOutputTypeDef, _OptionalDiscoveredResourceOutputTypeDef
+):
+    pass
+
+
 _RequiredImportMigrationTaskRequestRequestTypeDef = TypedDict(
     "_RequiredImportMigrationTaskRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
     },
 )
@@ -420,39 +466,39 @@
     "ProgressUpdateStreamSummaryTypeDef",
     {
         "ProgressUpdateStreamName": str,
     },
     total=False,
 )
 
-ResourceAttributeTypeDef = TypedDict(
-    "ResourceAttributeTypeDef",
+ResourceAttributeOutputTypeDef = TypedDict(
+    "ResourceAttributeOutputTypeDef",
     {
         "Type": ResourceAttributeTypeType,
         "Value": str,
     },
 )
 
-_RequiredTaskTypeDef = TypedDict(
-    "_RequiredTaskTypeDef",
+_RequiredTaskOutputTypeDef = TypedDict(
+    "_RequiredTaskOutputTypeDef",
     {
         "Status": StatusType,
     },
 )
-_OptionalTaskTypeDef = TypedDict(
-    "_OptionalTaskTypeDef",
+_OptionalTaskOutputTypeDef = TypedDict(
+    "_OptionalTaskOutputTypeDef",
     {
         "StatusDetail": str,
         "ProgressPercent": int,
     },
     total=False,
 )
 
 
-class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
+class TaskOutputTypeDef(_RequiredTaskOutputTypeDef, _OptionalTaskOutputTypeDef):
     pass
 
 
 _RequiredNotifyApplicationStateRequestRequestTypeDef = TypedDict(
     "_RequiredNotifyApplicationStateRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -472,24 +518,52 @@
 class NotifyApplicationStateRequestRequestTypeDef(
     _RequiredNotifyApplicationStateRequestRequestTypeDef,
     _OptionalNotifyApplicationStateRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredTaskTypeDef = TypedDict(
+    "_RequiredTaskTypeDef",
+    {
+        "Status": StatusType,
+    },
+)
+_OptionalTaskTypeDef = TypedDict(
+    "_OptionalTaskTypeDef",
+    {
+        "StatusDetail": str,
+        "ProgressPercent": int,
+    },
+    total=False,
+)
+
+
+class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
+    pass
+
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+ResourceAttributeTypeDef = TypedDict(
+    "ResourceAttributeTypeDef",
+    {
+        "Type": ResourceAttributeTypeType,
+        "Value": str,
+    },
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -526,23 +600,14 @@
 class AssociateCreatedArtifactRequestRequestTypeDef(
     _RequiredAssociateCreatedArtifactRequestRequestTypeDef,
     _OptionalAssociateCreatedArtifactRequestRequestTypeDef,
 ):
     pass
 
 
-ListCreatedArtifactsResultTypeDef = TypedDict(
-    "ListCreatedArtifactsResultTypeDef",
-    {
-        "NextToken": str,
-        "CreatedArtifactList": List[CreatedArtifactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAssociateDiscoveredResourceRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateDiscoveredResourceRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
         "DiscoveredResource": DiscoveredResourceTypeDef,
     },
@@ -559,19 +624,28 @@
 class AssociateDiscoveredResourceRequestRequestTypeDef(
     _RequiredAssociateDiscoveredResourceRequestRequestTypeDef,
     _OptionalAssociateDiscoveredResourceRequestRequestTypeDef,
 ):
     pass
 
 
+ListCreatedArtifactsResultTypeDef = TypedDict(
+    "ListCreatedArtifactsResultTypeDef",
+    {
+        "NextToken": str,
+        "CreatedArtifactList": List[CreatedArtifactOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListDiscoveredResourcesResultTypeDef = TypedDict(
     "ListDiscoveredResourcesResultTypeDef",
     {
         "NextToken": str,
-        "DiscoveredResourceList": List[DiscoveredResourceTypeDef],
+        "DiscoveredResourceList": List[DiscoveredResourceOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMigrationTasksResultTypeDef = TypedDict(
     "ListMigrationTasksResultTypeDef",
     {
@@ -586,46 +660,22 @@
     {
         "ProgressUpdateStreamSummaryList": List[ProgressUpdateStreamSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPutResourceAttributesRequestRequestTypeDef = TypedDict(
-    "_RequiredPutResourceAttributesRequestRequestTypeDef",
-    {
-        "ProgressUpdateStream": str,
-        "MigrationTaskName": str,
-        "ResourceAttributeList": Sequence[ResourceAttributeTypeDef],
-    },
-)
-_OptionalPutResourceAttributesRequestRequestTypeDef = TypedDict(
-    "_OptionalPutResourceAttributesRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class PutResourceAttributesRequestRequestTypeDef(
-    _RequiredPutResourceAttributesRequestRequestTypeDef,
-    _OptionalPutResourceAttributesRequestRequestTypeDef,
-):
-    pass
-
-
 MigrationTaskTypeDef = TypedDict(
     "MigrationTaskTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
-        "Task": TaskTypeDef,
+        "Task": TaskOutputTypeDef,
         "UpdateDateTime": datetime,
-        "ResourceAttributeList": List[ResourceAttributeTypeDef],
+        "ResourceAttributeList": List[ResourceAttributeOutputTypeDef],
     },
     total=False,
 )
 
 _RequiredNotifyMigrationTaskStateRequestRequestTypeDef = TypedDict(
     "_RequiredNotifyMigrationTaskStateRequestRequestTypeDef",
     {
@@ -648,14 +698,38 @@
 class NotifyMigrationTaskStateRequestRequestTypeDef(
     _RequiredNotifyMigrationTaskStateRequestRequestTypeDef,
     _OptionalNotifyMigrationTaskStateRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredPutResourceAttributesRequestRequestTypeDef = TypedDict(
+    "_RequiredPutResourceAttributesRequestRequestTypeDef",
+    {
+        "ProgressUpdateStream": str,
+        "MigrationTaskName": str,
+        "ResourceAttributeList": Sequence[ResourceAttributeTypeDef],
+    },
+)
+_OptionalPutResourceAttributesRequestRequestTypeDef = TypedDict(
+    "_OptionalPutResourceAttributesRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class PutResourceAttributesRequestRequestTypeDef(
+    _RequiredPutResourceAttributesRequestRequestTypeDef,
+    _OptionalPutResourceAttributesRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeMigrationTaskResultTypeDef = TypedDict(
     "DescribeMigrationTaskResultTypeDef",
     {
         "MigrationTask": MigrationTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mgh-1.28.0/mypy_boto3_mgh/type_defs.pyi` & `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -23,48 +23,52 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ApplicationStateTypeDef",
     "CreatedArtifactTypeDef",
     "DiscoveredResourceTypeDef",
     "CreateProgressUpdateStreamRequestRequestTypeDef",
+    "CreatedArtifactOutputTypeDef",
     "DeleteProgressUpdateStreamRequestRequestTypeDef",
     "DescribeApplicationStateRequestRequestTypeDef",
     "DescribeApplicationStateResultTypeDef",
     "DescribeMigrationTaskRequestRequestTypeDef",
     "DisassociateCreatedArtifactRequestRequestTypeDef",
     "DisassociateDiscoveredResourceRequestRequestTypeDef",
+    "DiscoveredResourceOutputTypeDef",
     "ImportMigrationTaskRequestRequestTypeDef",
     "ListApplicationStatesRequestListApplicationStatesPaginateTypeDef",
     "ListApplicationStatesRequestRequestTypeDef",
     "ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
     "ListCreatedArtifactsRequestRequestTypeDef",
     "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     "ListDiscoveredResourcesRequestRequestTypeDef",
     "ListMigrationTasksRequestListMigrationTasksPaginateTypeDef",
     "ListMigrationTasksRequestRequestTypeDef",
     "MigrationTaskSummaryTypeDef",
     "ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef",
     "ListProgressUpdateStreamsRequestRequestTypeDef",
     "ProgressUpdateStreamSummaryTypeDef",
-    "ResourceAttributeTypeDef",
-    "TaskTypeDef",
+    "ResourceAttributeOutputTypeDef",
+    "TaskOutputTypeDef",
     "NotifyApplicationStateRequestRequestTypeDef",
+    "TaskTypeDef",
     "PaginatorConfigTypeDef",
+    "ResourceAttributeTypeDef",
     "ResponseMetadataTypeDef",
     "ListApplicationStatesResultTypeDef",
     "AssociateCreatedArtifactRequestRequestTypeDef",
-    "ListCreatedArtifactsResultTypeDef",
     "AssociateDiscoveredResourceRequestRequestTypeDef",
+    "ListCreatedArtifactsResultTypeDef",
     "ListDiscoveredResourcesResultTypeDef",
     "ListMigrationTasksResultTypeDef",
     "ListProgressUpdateStreamsResultTypeDef",
-    "PutResourceAttributesRequestRequestTypeDef",
     "MigrationTaskTypeDef",
     "NotifyMigrationTaskStateRequestRequestTypeDef",
+    "PutResourceAttributesRequestRequestTypeDef",
     "DescribeMigrationTaskResultTypeDef",
 )
 
 ApplicationStateTypeDef = TypedDict(
     "ApplicationStateTypeDef",
     {
         "ApplicationId": str,
@@ -126,14 +130,33 @@
 
 class CreateProgressUpdateStreamRequestRequestTypeDef(
     _RequiredCreateProgressUpdateStreamRequestRequestTypeDef,
     _OptionalCreateProgressUpdateStreamRequestRequestTypeDef,
 ):
     pass
 
+_RequiredCreatedArtifactOutputTypeDef = TypedDict(
+    "_RequiredCreatedArtifactOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreatedArtifactOutputTypeDef = TypedDict(
+    "_OptionalCreatedArtifactOutputTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+class CreatedArtifactOutputTypeDef(
+    _RequiredCreatedArtifactOutputTypeDef, _OptionalCreatedArtifactOutputTypeDef
+):
+    pass
+
 _RequiredDeleteProgressUpdateStreamRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteProgressUpdateStreamRequestRequestTypeDef",
     {
         "ProgressUpdateStreamName": str,
     },
 )
 _OptionalDeleteProgressUpdateStreamRequestRequestTypeDef = TypedDict(
@@ -214,14 +237,33 @@
 
 class DisassociateDiscoveredResourceRequestRequestTypeDef(
     _RequiredDisassociateDiscoveredResourceRequestRequestTypeDef,
     _OptionalDisassociateDiscoveredResourceRequestRequestTypeDef,
 ):
     pass
 
+_RequiredDiscoveredResourceOutputTypeDef = TypedDict(
+    "_RequiredDiscoveredResourceOutputTypeDef",
+    {
+        "ConfigurationId": str,
+    },
+)
+_OptionalDiscoveredResourceOutputTypeDef = TypedDict(
+    "_OptionalDiscoveredResourceOutputTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+class DiscoveredResourceOutputTypeDef(
+    _RequiredDiscoveredResourceOutputTypeDef, _OptionalDiscoveredResourceOutputTypeDef
+):
+    pass
+
 _RequiredImportMigrationTaskRequestRequestTypeDef = TypedDict(
     "_RequiredImportMigrationTaskRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
     },
 )
@@ -397,38 +439,38 @@
     "ProgressUpdateStreamSummaryTypeDef",
     {
         "ProgressUpdateStreamName": str,
     },
     total=False,
 )
 
-ResourceAttributeTypeDef = TypedDict(
-    "ResourceAttributeTypeDef",
+ResourceAttributeOutputTypeDef = TypedDict(
+    "ResourceAttributeOutputTypeDef",
     {
         "Type": ResourceAttributeTypeType,
         "Value": str,
     },
 )
 
-_RequiredTaskTypeDef = TypedDict(
-    "_RequiredTaskTypeDef",
+_RequiredTaskOutputTypeDef = TypedDict(
+    "_RequiredTaskOutputTypeDef",
     {
         "Status": StatusType,
     },
 )
-_OptionalTaskTypeDef = TypedDict(
-    "_OptionalTaskTypeDef",
+_OptionalTaskOutputTypeDef = TypedDict(
+    "_OptionalTaskOutputTypeDef",
     {
         "StatusDetail": str,
         "ProgressPercent": int,
     },
     total=False,
 )
 
-class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
+class TaskOutputTypeDef(_RequiredTaskOutputTypeDef, _OptionalTaskOutputTypeDef):
     pass
 
 _RequiredNotifyApplicationStateRequestRequestTypeDef = TypedDict(
     "_RequiredNotifyApplicationStateRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "Status": ApplicationStatusType,
@@ -445,24 +487,50 @@
 
 class NotifyApplicationStateRequestRequestTypeDef(
     _RequiredNotifyApplicationStateRequestRequestTypeDef,
     _OptionalNotifyApplicationStateRequestRequestTypeDef,
 ):
     pass
 
+_RequiredTaskTypeDef = TypedDict(
+    "_RequiredTaskTypeDef",
+    {
+        "Status": StatusType,
+    },
+)
+_OptionalTaskTypeDef = TypedDict(
+    "_OptionalTaskTypeDef",
+    {
+        "StatusDetail": str,
+        "ProgressPercent": int,
+    },
+    total=False,
+)
+
+class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
+    pass
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+ResourceAttributeTypeDef = TypedDict(
+    "ResourceAttributeTypeDef",
+    {
+        "Type": ResourceAttributeTypeType,
+        "Value": str,
+    },
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -497,23 +565,14 @@
 
 class AssociateCreatedArtifactRequestRequestTypeDef(
     _RequiredAssociateCreatedArtifactRequestRequestTypeDef,
     _OptionalAssociateCreatedArtifactRequestRequestTypeDef,
 ):
     pass
 
-ListCreatedArtifactsResultTypeDef = TypedDict(
-    "ListCreatedArtifactsResultTypeDef",
-    {
-        "NextToken": str,
-        "CreatedArtifactList": List[CreatedArtifactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAssociateDiscoveredResourceRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateDiscoveredResourceRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
         "DiscoveredResource": DiscoveredResourceTypeDef,
     },
@@ -528,19 +587,28 @@
 
 class AssociateDiscoveredResourceRequestRequestTypeDef(
     _RequiredAssociateDiscoveredResourceRequestRequestTypeDef,
     _OptionalAssociateDiscoveredResourceRequestRequestTypeDef,
 ):
     pass
 
+ListCreatedArtifactsResultTypeDef = TypedDict(
+    "ListCreatedArtifactsResultTypeDef",
+    {
+        "NextToken": str,
+        "CreatedArtifactList": List[CreatedArtifactOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListDiscoveredResourcesResultTypeDef = TypedDict(
     "ListDiscoveredResourcesResultTypeDef",
     {
         "NextToken": str,
-        "DiscoveredResourceList": List[DiscoveredResourceTypeDef],
+        "DiscoveredResourceList": List[DiscoveredResourceOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMigrationTasksResultTypeDef = TypedDict(
     "ListMigrationTasksResultTypeDef",
     {
@@ -555,44 +623,22 @@
     {
         "ProgressUpdateStreamSummaryList": List[ProgressUpdateStreamSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPutResourceAttributesRequestRequestTypeDef = TypedDict(
-    "_RequiredPutResourceAttributesRequestRequestTypeDef",
-    {
-        "ProgressUpdateStream": str,
-        "MigrationTaskName": str,
-        "ResourceAttributeList": Sequence[ResourceAttributeTypeDef],
-    },
-)
-_OptionalPutResourceAttributesRequestRequestTypeDef = TypedDict(
-    "_OptionalPutResourceAttributesRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class PutResourceAttributesRequestRequestTypeDef(
-    _RequiredPutResourceAttributesRequestRequestTypeDef,
-    _OptionalPutResourceAttributesRequestRequestTypeDef,
-):
-    pass
-
 MigrationTaskTypeDef = TypedDict(
     "MigrationTaskTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
-        "Task": TaskTypeDef,
+        "Task": TaskOutputTypeDef,
         "UpdateDateTime": datetime,
-        "ResourceAttributeList": List[ResourceAttributeTypeDef],
+        "ResourceAttributeList": List[ResourceAttributeOutputTypeDef],
     },
     total=False,
 )
 
 _RequiredNotifyMigrationTaskStateRequestRequestTypeDef = TypedDict(
     "_RequiredNotifyMigrationTaskStateRequestRequestTypeDef",
     {
@@ -613,14 +659,36 @@
 
 class NotifyMigrationTaskStateRequestRequestTypeDef(
     _RequiredNotifyMigrationTaskStateRequestRequestTypeDef,
     _OptionalNotifyMigrationTaskStateRequestRequestTypeDef,
 ):
     pass
 
+_RequiredPutResourceAttributesRequestRequestTypeDef = TypedDict(
+    "_RequiredPutResourceAttributesRequestRequestTypeDef",
+    {
+        "ProgressUpdateStream": str,
+        "MigrationTaskName": str,
+        "ResourceAttributeList": Sequence[ResourceAttributeTypeDef],
+    },
+)
+_OptionalPutResourceAttributesRequestRequestTypeDef = TypedDict(
+    "_OptionalPutResourceAttributesRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class PutResourceAttributesRequestRequestTypeDef(
+    _RequiredPutResourceAttributesRequestRequestTypeDef,
+    _OptionalPutResourceAttributesRequestRequestTypeDef,
+):
+    pass
+
 DescribeMigrationTaskResultTypeDef = TypedDict(
     "DescribeMigrationTaskResultTypeDef",
     {
         "MigrationTask": MigrationTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mgh-1.28.0/mypy_boto3_mgh.egg-info/PKG-INFO` & `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mgh
-Version: 1.28.0
-Summary: Type annotations for boto3.MigrationHub 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MigrationHub 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mgh"></a>
 
 # mypy-boto3-mgh
 
 [![PyPI - mypy-boto3-mgh](https://img.shields.io/pypi/v/mypy-boto3-mgh.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgh.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgh)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mgh?color=blue)](https://pypistats.org/packages/mypy-boto3-mgh)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mgh)](https://pepy.tech/project/mypy-boto3-mgh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHub 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
+[boto3.MigrationHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
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
 [mypy-boto3-mgh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/).
 
 See how it helps to find and fix potential bugs:
 
@@ -348,48 +348,52 @@
 
 ```python
 from mypy_boto3_mgh.type_defs import (
     ApplicationStateTypeDef,
     CreatedArtifactTypeDef,
     DiscoveredResourceTypeDef,
     CreateProgressUpdateStreamRequestRequestTypeDef,
+    CreatedArtifactOutputTypeDef,
     DeleteProgressUpdateStreamRequestRequestTypeDef,
     DescribeApplicationStateRequestRequestTypeDef,
     DescribeApplicationStateResultTypeDef,
     DescribeMigrationTaskRequestRequestTypeDef,
     DisassociateCreatedArtifactRequestRequestTypeDef,
     DisassociateDiscoveredResourceRequestRequestTypeDef,
+    DiscoveredResourceOutputTypeDef,
     ImportMigrationTaskRequestRequestTypeDef,
     ListApplicationStatesRequestListApplicationStatesPaginateTypeDef,
     ListApplicationStatesRequestRequestTypeDef,
     ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
     ListCreatedArtifactsRequestRequestTypeDef,
     ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
     ListMigrationTasksRequestListMigrationTasksPaginateTypeDef,
     ListMigrationTasksRequestRequestTypeDef,
     MigrationTaskSummaryTypeDef,
     ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef,
     ListProgressUpdateStreamsRequestRequestTypeDef,
     ProgressUpdateStreamSummaryTypeDef,
-    ResourceAttributeTypeDef,
-    TaskTypeDef,
+    ResourceAttributeOutputTypeDef,
+    TaskOutputTypeDef,
     NotifyApplicationStateRequestRequestTypeDef,
+    TaskTypeDef,
     PaginatorConfigTypeDef,
+    ResourceAttributeTypeDef,
     ResponseMetadataTypeDef,
     ListApplicationStatesResultTypeDef,
     AssociateCreatedArtifactRequestRequestTypeDef,
-    ListCreatedArtifactsResultTypeDef,
     AssociateDiscoveredResourceRequestRequestTypeDef,
+    ListCreatedArtifactsResultTypeDef,
     ListDiscoveredResourcesResultTypeDef,
     ListMigrationTasksResultTypeDef,
     ListProgressUpdateStreamsResultTypeDef,
-    PutResourceAttributesRequestRequestTypeDef,
     MigrationTaskTypeDef,
     NotifyMigrationTaskStateRequestRequestTypeDef,
+    PutResourceAttributesRequestRequestTypeDef,
     DescribeMigrationTaskResultTypeDef,
 )
 
 
 def get_structure() -> ApplicationStateTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-mgh-1.28.0/mypy_boto3_mgh.egg-info/SOURCES.txt` & `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.0/setup.py` & `mypy-boto3-mgh-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mgh",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_mgh"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MigrationHub 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.MigrationHub 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

