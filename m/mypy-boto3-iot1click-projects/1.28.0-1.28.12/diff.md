# Comparing `tmp/mypy-boto3-iot1click-projects-1.28.0.tar.gz` & `tmp/mypy-boto3-iot1click-projects-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iot1click-projects-1.28.0.tar", last modified: Thu Jul  6 20:59:45 2023, max compression
+gzip compressed data, was "mypy-boto3-iot1click-projects-1.28.12.tar", last modified: Thu Jul 27 05:34:47 2023, max compression
```

## Comparing `mypy-boto3-iot1click-projects-1.28.0.tar` & `mypy-boto3-iot1click-projects-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:45.454325 mypy-boto3-iot1click-projects-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:43:35.000000 mypy-boto3-iot1click-projects-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-06 20:59:45.446325 mypy-boto3-iot1click-projects-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12989 2023-07-06 20:43:35.000000 mypy-boto3-iot1click-projects-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:45.446325 mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-06 20:43:35.000000 mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-06 20:43:35.000000 mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-06 20:43:35.000000 mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-07-06 20:43:35.000000 mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13264 2023-07-06 20:43:35.000000 mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-06 20:43:36.000000 mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-06 20:43:36.000000 mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-06 20:43:36.000000 mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-06 20:43:35.000000 mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:43:35.000000 mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10880 2023-07-06 20:43:36.000000 mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-07-06 20:43:36.000000 mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:43:35.000000 mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:45.446325 mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-06 20:59:45.000000 mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-06 20:59:45.000000 mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:45.000000 mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:45.000000 mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:45.000000 mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-06 20:59:45.000000 mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:45.454325 mypy-boto3-iot1click-projects-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-06 20:43:35.000000 mypy-boto3-iot1click-projects-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.832488 mypy-boto3-iot1click-projects-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-07-27 05:34:47.832488 mypy-boto3-iot1click-projects-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.832488 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13264 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.832488 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:47.832488 mypy-boto3-iot1click-projects-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-27 05:23:56.000000 mypy-boto3-iot1click-projects-1.28.12/setup.py
```

### Comparing `mypy-boto3-iot1click-projects-1.28.0/LICENSE` & `mypy-boto3-iot1click-projects-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.0/PKG-INFO` & `mypy-boto3-iot1click-projects-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot1click-projects
-Version: 1.28.0
-Summary: Type annotations for boto3.IoT1ClickProjects 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoT1ClickProjects 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iot1click-projects"></a>
 
 # mypy-boto3-iot1click-projects
 
 [![PyPI - mypy-boto3-iot1click-projects](https://img.shields.io/pypi/v/mypy-boto3-iot1click-projects.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-projects)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-projects.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-projects)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot1click-projects?color=blue)](https://pypistats.org/packages/mypy-boto3-iot1click-projects)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot1click-projects)](https://pepy.tech/project/mypy-boto3-iot1click-projects)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickProjects 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
+[boto3.IoT1ClickProjects 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
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
 [mypy-boto3-iot1click-projects docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,14 +329,15 @@
     AssociateDeviceWithPlacementRequestRequestTypeDef,
     CreatePlacementRequestRequestTypeDef,
     DeletePlacementRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DescribePlacementRequestRequestTypeDef,
     PlacementDescriptionTypeDef,
     DescribeProjectRequestRequestTypeDef,
+    DeviceTemplateOutputTypeDef,
     DeviceTemplateTypeDef,
     DisassociateDeviceFromPlacementRequestRequestTypeDef,
     GetDevicesInPlacementRequestRequestTypeDef,
     GetDevicesInPlacementResponseTypeDef,
     ListPlacementsRequestListPlacementsPaginateTypeDef,
     ListPlacementsRequestRequestTypeDef,
     PlacementSummaryTypeDef,
@@ -347,19 +348,20 @@
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePlacementRequestRequestTypeDef,
     DescribePlacementResponseTypeDef,
+    PlacementTemplateOutputTypeDef,
     PlacementTemplateTypeDef,
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
-    CreateProjectRequestRequestTypeDef,
     ProjectDescriptionTypeDef,
+    CreateProjectRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     DescribeProjectResponseTypeDef,
 )
 
 
 def get_structure() -> AssociateDeviceWithPlacementRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-iot1click-projects-1.28.0/README.md` & `mypy-boto3-iot1click-projects-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iot1click-projects"></a>
 
 # mypy-boto3-iot1click-projects
 
 [![PyPI - mypy-boto3-iot1click-projects](https://img.shields.io/pypi/v/mypy-boto3-iot1click-projects.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-projects)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-projects.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-projects)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot1click-projects?color=blue)](https://pypistats.org/packages/mypy-boto3-iot1click-projects)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot1click-projects)](https://pepy.tech/project/mypy-boto3-iot1click-projects)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickProjects 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
+[boto3.IoT1ClickProjects 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
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
 [mypy-boto3-iot1click-projects docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,14 +297,15 @@
     AssociateDeviceWithPlacementRequestRequestTypeDef,
     CreatePlacementRequestRequestTypeDef,
     DeletePlacementRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DescribePlacementRequestRequestTypeDef,
     PlacementDescriptionTypeDef,
     DescribeProjectRequestRequestTypeDef,
+    DeviceTemplateOutputTypeDef,
     DeviceTemplateTypeDef,
     DisassociateDeviceFromPlacementRequestRequestTypeDef,
     GetDevicesInPlacementRequestRequestTypeDef,
     GetDevicesInPlacementResponseTypeDef,
     ListPlacementsRequestListPlacementsPaginateTypeDef,
     ListPlacementsRequestRequestTypeDef,
     PlacementSummaryTypeDef,
@@ -315,19 +316,20 @@
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePlacementRequestRequestTypeDef,
     DescribePlacementResponseTypeDef,
+    PlacementTemplateOutputTypeDef,
     PlacementTemplateTypeDef,
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
-    CreateProjectRequestRequestTypeDef,
     ProjectDescriptionTypeDef,
+    CreateProjectRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     DescribeProjectResponseTypeDef,
 )
 
 
 def get_structure() -> AssociateDeviceWithPlacementRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/__init__.py` & `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/__init__.pyi` & `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/__main__.py` & `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoT1ClickProjects 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.IoT1ClickProjects 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects\nOther"
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

### Comparing `mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/client.py` & `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/client.pyi` & `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/literals.py` & `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,15 @@
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
@@ -234,26 +235,28 @@
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

### Comparing `mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/literals.pyi` & `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,15 @@
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
@@ -232,26 +233,28 @@
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

### Comparing `mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/paginator.py` & `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/paginator.pyi` & `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/type_defs.py` & `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     "AssociateDeviceWithPlacementRequestRequestTypeDef",
     "CreatePlacementRequestRequestTypeDef",
     "DeletePlacementRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DescribePlacementRequestRequestTypeDef",
     "PlacementDescriptionTypeDef",
     "DescribeProjectRequestRequestTypeDef",
+    "DeviceTemplateOutputTypeDef",
     "DeviceTemplateTypeDef",
     "DisassociateDeviceFromPlacementRequestRequestTypeDef",
     "GetDevicesInPlacementRequestRequestTypeDef",
     "GetDevicesInPlacementResponseTypeDef",
     "ListPlacementsRequestListPlacementsPaginateTypeDef",
     "ListPlacementsRequestRequestTypeDef",
     "PlacementSummaryTypeDef",
@@ -43,19 +44,20 @@
     "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePlacementRequestRequestTypeDef",
     "DescribePlacementResponseTypeDef",
+    "PlacementTemplateOutputTypeDef",
     "PlacementTemplateTypeDef",
     "ListPlacementsResponseTypeDef",
     "ListProjectsResponseTypeDef",
-    "CreateProjectRequestRequestTypeDef",
     "ProjectDescriptionTypeDef",
+    "CreateProjectRequestRequestTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "DescribeProjectResponseTypeDef",
 )
 
 AssociateDeviceWithPlacementRequestRequestTypeDef = TypedDict(
     "AssociateDeviceWithPlacementRequestRequestTypeDef",
     {
@@ -125,14 +127,23 @@
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
+DeviceTemplateOutputTypeDef = TypedDict(
+    "DeviceTemplateOutputTypeDef",
+    {
+        "deviceType": str,
+        "callbackOverrides": Dict[str, str],
+    },
+    total=False,
+)
+
 DeviceTemplateTypeDef = TypedDict(
     "DeviceTemplateTypeDef",
     {
         "deviceType": str,
         "callbackOverrides": Mapping[str, str],
     },
     total=False,
@@ -334,14 +345,23 @@
     "DescribePlacementResponseTypeDef",
     {
         "placement": PlacementDescriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PlacementTemplateOutputTypeDef = TypedDict(
+    "PlacementTemplateOutputTypeDef",
+    {
+        "defaultAttributes": Dict[str, str],
+        "deviceTemplates": Dict[str, DeviceTemplateOutputTypeDef],
+    },
+    total=False,
+)
+
 PlacementTemplateTypeDef = TypedDict(
     "PlacementTemplateTypeDef",
     {
         "defaultAttributes": Mapping[str, str],
         "deviceTemplates": Mapping[str, DeviceTemplateTypeDef],
     },
     total=False,
@@ -361,59 +381,59 @@
     {
         "projects": List[ProjectSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateProjectRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProjectRequestRequestTypeDef",
+_RequiredProjectDescriptionTypeDef = TypedDict(
+    "_RequiredProjectDescriptionTypeDef",
     {
         "projectName": str,
+        "createdDate": datetime,
+        "updatedDate": datetime,
     },
 )
-_OptionalCreateProjectRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProjectRequestRequestTypeDef",
+_OptionalProjectDescriptionTypeDef = TypedDict(
+    "_OptionalProjectDescriptionTypeDef",
     {
+        "arn": str,
         "description": str,
-        "placementTemplate": PlacementTemplateTypeDef,
-        "tags": Mapping[str, str],
+        "placementTemplate": PlacementTemplateOutputTypeDef,
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
 
-class CreateProjectRequestRequestTypeDef(
-    _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
+class ProjectDescriptionTypeDef(
+    _RequiredProjectDescriptionTypeDef, _OptionalProjectDescriptionTypeDef
 ):
     pass
 
 
-_RequiredProjectDescriptionTypeDef = TypedDict(
-    "_RequiredProjectDescriptionTypeDef",
+_RequiredCreateProjectRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "projectName": str,
-        "createdDate": datetime,
-        "updatedDate": datetime,
     },
 )
-_OptionalProjectDescriptionTypeDef = TypedDict(
-    "_OptionalProjectDescriptionTypeDef",
+_OptionalCreateProjectRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProjectRequestRequestTypeDef",
     {
-        "arn": str,
         "description": str,
         "placementTemplate": PlacementTemplateTypeDef,
-        "tags": Dict[str, str],
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class ProjectDescriptionTypeDef(
-    _RequiredProjectDescriptionTypeDef, _OptionalProjectDescriptionTypeDef
+class CreateProjectRequestRequestTypeDef(
+    _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
 
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects/type_defs.pyi` & `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "AssociateDeviceWithPlacementRequestRequestTypeDef",
     "CreatePlacementRequestRequestTypeDef",
     "DeletePlacementRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DescribePlacementRequestRequestTypeDef",
     "PlacementDescriptionTypeDef",
     "DescribeProjectRequestRequestTypeDef",
+    "DeviceTemplateOutputTypeDef",
     "DeviceTemplateTypeDef",
     "DisassociateDeviceFromPlacementRequestRequestTypeDef",
     "GetDevicesInPlacementRequestRequestTypeDef",
     "GetDevicesInPlacementResponseTypeDef",
     "ListPlacementsRequestListPlacementsPaginateTypeDef",
     "ListPlacementsRequestRequestTypeDef",
     "PlacementSummaryTypeDef",
@@ -42,19 +43,20 @@
     "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePlacementRequestRequestTypeDef",
     "DescribePlacementResponseTypeDef",
+    "PlacementTemplateOutputTypeDef",
     "PlacementTemplateTypeDef",
     "ListPlacementsResponseTypeDef",
     "ListProjectsResponseTypeDef",
-    "CreateProjectRequestRequestTypeDef",
     "ProjectDescriptionTypeDef",
+    "CreateProjectRequestRequestTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "DescribeProjectResponseTypeDef",
 )
 
 AssociateDeviceWithPlacementRequestRequestTypeDef = TypedDict(
     "AssociateDeviceWithPlacementRequestRequestTypeDef",
     {
@@ -122,14 +124,23 @@
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
+DeviceTemplateOutputTypeDef = TypedDict(
+    "DeviceTemplateOutputTypeDef",
+    {
+        "deviceType": str,
+        "callbackOverrides": Dict[str, str],
+    },
+    total=False,
+)
+
 DeviceTemplateTypeDef = TypedDict(
     "DeviceTemplateTypeDef",
     {
         "deviceType": str,
         "callbackOverrides": Mapping[str, str],
     },
     total=False,
@@ -323,14 +334,23 @@
     "DescribePlacementResponseTypeDef",
     {
         "placement": PlacementDescriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PlacementTemplateOutputTypeDef = TypedDict(
+    "PlacementTemplateOutputTypeDef",
+    {
+        "defaultAttributes": Dict[str, str],
+        "deviceTemplates": Dict[str, DeviceTemplateOutputTypeDef],
+    },
+    total=False,
+)
+
 PlacementTemplateTypeDef = TypedDict(
     "PlacementTemplateTypeDef",
     {
         "defaultAttributes": Mapping[str, str],
         "deviceTemplates": Mapping[str, DeviceTemplateTypeDef],
     },
     total=False,
@@ -350,56 +370,56 @@
     {
         "projects": List[ProjectSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateProjectRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProjectRequestRequestTypeDef",
+_RequiredProjectDescriptionTypeDef = TypedDict(
+    "_RequiredProjectDescriptionTypeDef",
     {
         "projectName": str,
+        "createdDate": datetime,
+        "updatedDate": datetime,
     },
 )
-_OptionalCreateProjectRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProjectRequestRequestTypeDef",
+_OptionalProjectDescriptionTypeDef = TypedDict(
+    "_OptionalProjectDescriptionTypeDef",
     {
+        "arn": str,
         "description": str,
-        "placementTemplate": PlacementTemplateTypeDef,
-        "tags": Mapping[str, str],
+        "placementTemplate": PlacementTemplateOutputTypeDef,
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
-class CreateProjectRequestRequestTypeDef(
-    _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
+class ProjectDescriptionTypeDef(
+    _RequiredProjectDescriptionTypeDef, _OptionalProjectDescriptionTypeDef
 ):
     pass
 
-_RequiredProjectDescriptionTypeDef = TypedDict(
-    "_RequiredProjectDescriptionTypeDef",
+_RequiredCreateProjectRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "projectName": str,
-        "createdDate": datetime,
-        "updatedDate": datetime,
     },
 )
-_OptionalProjectDescriptionTypeDef = TypedDict(
-    "_OptionalProjectDescriptionTypeDef",
+_OptionalCreateProjectRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProjectRequestRequestTypeDef",
     {
-        "arn": str,
         "description": str,
         "placementTemplate": PlacementTemplateTypeDef,
-        "tags": Dict[str, str],
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class ProjectDescriptionTypeDef(
-    _RequiredProjectDescriptionTypeDef, _OptionalProjectDescriptionTypeDef
+class CreateProjectRequestRequestTypeDef(
+    _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "projectName": str,
```

### Comparing `mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects.egg-info/PKG-INFO` & `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot1click-projects
-Version: 1.28.0
-Summary: Type annotations for boto3.IoT1ClickProjects 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoT1ClickProjects 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iot1click-projects"></a>
 
 # mypy-boto3-iot1click-projects
 
 [![PyPI - mypy-boto3-iot1click-projects](https://img.shields.io/pypi/v/mypy-boto3-iot1click-projects.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-projects)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-projects.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-projects)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot1click-projects?color=blue)](https://pypistats.org/packages/mypy-boto3-iot1click-projects)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot1click-projects)](https://pepy.tech/project/mypy-boto3-iot1click-projects)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickProjects 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
+[boto3.IoT1ClickProjects 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
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
 [mypy-boto3-iot1click-projects docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,14 +329,15 @@
     AssociateDeviceWithPlacementRequestRequestTypeDef,
     CreatePlacementRequestRequestTypeDef,
     DeletePlacementRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DescribePlacementRequestRequestTypeDef,
     PlacementDescriptionTypeDef,
     DescribeProjectRequestRequestTypeDef,
+    DeviceTemplateOutputTypeDef,
     DeviceTemplateTypeDef,
     DisassociateDeviceFromPlacementRequestRequestTypeDef,
     GetDevicesInPlacementRequestRequestTypeDef,
     GetDevicesInPlacementResponseTypeDef,
     ListPlacementsRequestListPlacementsPaginateTypeDef,
     ListPlacementsRequestRequestTypeDef,
     PlacementSummaryTypeDef,
@@ -347,19 +348,20 @@
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePlacementRequestRequestTypeDef,
     DescribePlacementResponseTypeDef,
+    PlacementTemplateOutputTypeDef,
     PlacementTemplateTypeDef,
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
-    CreateProjectRequestRequestTypeDef,
     ProjectDescriptionTypeDef,
+    CreateProjectRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     DescribeProjectResponseTypeDef,
 )
 
 
 def get_structure() -> AssociateDeviceWithPlacementRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-iot1click-projects-1.28.0/mypy_boto3_iot1click_projects.egg-info/SOURCES.txt` & `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.0/setup.py` & `mypy-boto3-iot1click-projects-1.28.12/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iot1click-projects",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_iot1click_projects"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoT1ClickProjects 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.IoT1ClickProjects 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

