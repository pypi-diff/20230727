# Comparing `tmp/mypy-boto3-iot-roborunner-1.28.0.tar.gz` & `tmp/mypy-boto3-iot-roborunner-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iot-roborunner-1.28.0.tar", last modified: Thu Jul  6 20:59:47 2023, max compression
+gzip compressed data, was "mypy-boto3-iot-roborunner-1.28.12.tar", last modified: Thu Jul 27 05:34:49 2023, max compression
```

## Comparing `mypy-boto3-iot-roborunner-1.28.0.tar` & `mypy-boto3-iot-roborunner-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:47.490329 mypy-boto3-iot-roborunner-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:43:32.000000 mypy-boto3-iot-roborunner-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15161 2023-07-06 20:59:47.490329 mypy-boto3-iot-roborunner-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-07-06 20:43:32.000000 mypy-boto3-iot-roborunner-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:47.486329 mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-06 20:43:32.000000 mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-06 20:43:32.000000 mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-06 20:43:32.000000 mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19292 2023-07-06 20:43:32.000000 mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-07-06 20:43:32.000000 mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-07-06 20:43:32.000000 mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-07-06 20:43:32.000000 mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-06 20:43:32.000000 mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-06 20:43:32.000000 mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:43:32.000000 mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20256 2023-07-06 20:43:33.000000 mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20217 2023-07-06 20:43:33.000000 mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:43:32.000000 mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:47.490329 mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15161 2023-07-06 20:59:47.000000 mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 20:59:47.000000 mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:47.000000 mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:47.000000 mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:47.000000 mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 20:59:47.000000 mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:47.490329 mypy-boto3-iot-roborunner-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-06 20:43:32.000000 mypy-boto3-iot-roborunner-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.000484 mypy-boto3-iot-roborunner-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-07-27 05:34:48.992484 mypy-boto3-iot-roborunner-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13782 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:48.992484 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19292 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21802 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21759 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:48.992484 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-07-27 05:34:48.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 05:34:48.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:48.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:48.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:48.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:34:48.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:49.000484 mypy-boto3-iot-roborunner-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-27 05:23:53.000000 mypy-boto3-iot-roborunner-1.28.12/setup.py
```

### Comparing `mypy-boto3-iot-roborunner-1.28.0/LICENSE` & `mypy-boto3-iot-roborunner-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.0/PKG-INFO` & `mypy-boto3-iot-roborunner-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot-roborunner
-Version: 1.28.0
-Summary: Type annotations for boto3.IoTRoboRunner 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTRoboRunner 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iot-roborunner"></a>
 
 # mypy-boto3-iot-roborunner
 
 [![PyPI - mypy-boto3-iot-roborunner](https://img.shields.io/pypi/v/mypy-boto3-iot-roborunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-roborunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot-roborunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-roborunner)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot-roborunner?color=blue)](https://pypistats.org/packages/mypy-boto3-iot-roborunner)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot-roborunner)](https://pepy.tech/project/mypy-boto3-iot-roborunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTRoboRunner 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
+[boto3.IoTRoboRunner 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
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
 [mypy-boto3-iot-roborunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,14 +332,15 @@
 ### Typed dictionaries
 
 `mypy_boto3_iot_roborunner.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot_roborunner.type_defs import (
+    CartesianCoordinatesOutputTypeDef,
     CartesianCoordinatesTypeDef,
     CreateDestinationRequestRequestTypeDef,
     CreateDestinationResponseTypeDef,
     CreateSiteRequestRequestTypeDef,
     CreateSiteResponseTypeDef,
     CreateWorkerFleetRequestRequestTypeDef,
     CreateWorkerFleetResponseTypeDef,
@@ -354,14 +355,16 @@
     GetDestinationRequestRequestTypeDef,
     GetDestinationResponseTypeDef,
     GetSiteRequestRequestTypeDef,
     GetSiteResponseTypeDef,
     GetWorkerFleetRequestRequestTypeDef,
     GetWorkerFleetResponseTypeDef,
     GetWorkerRequestRequestTypeDef,
+    OrientationOutputTypeDef,
+    VendorPropertiesOutputTypeDef,
     ListDestinationsRequestListDestinationsPaginateTypeDef,
     ListDestinationsRequestRequestTypeDef,
     ListSitesRequestListSitesPaginateTypeDef,
     ListSitesRequestRequestTypeDef,
     SiteTypeDef,
     ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
     ListWorkerFleetsRequestRequestTypeDef,
@@ -372,28 +375,29 @@
     ResponseMetadataTypeDef,
     UpdateDestinationRequestRequestTypeDef,
     UpdateDestinationResponseTypeDef,
     UpdateSiteRequestRequestTypeDef,
     UpdateSiteResponseTypeDef,
     UpdateWorkerFleetRequestRequestTypeDef,
     UpdateWorkerFleetResponseTypeDef,
+    PositionCoordinatesOutputTypeDef,
     PositionCoordinatesTypeDef,
     ListDestinationsResponseTypeDef,
     ListSitesResponseTypeDef,
     ListWorkerFleetsResponseTypeDef,
-    CreateWorkerRequestRequestTypeDef,
     GetWorkerResponseTypeDef,
-    UpdateWorkerRequestRequestTypeDef,
     UpdateWorkerResponseTypeDef,
     WorkerTypeDef,
+    CreateWorkerRequestRequestTypeDef,
+    UpdateWorkerRequestRequestTypeDef,
     ListWorkersResponseTypeDef,
 )
 
 
-def get_structure() -> CartesianCoordinatesTypeDef:
+def get_structure() -> CartesianCoordinatesOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot-roborunner-1.28.0/README.md` & `mypy-boto3-iot-roborunner-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iot-roborunner"></a>
 
 # mypy-boto3-iot-roborunner
 
 [![PyPI - mypy-boto3-iot-roborunner](https://img.shields.io/pypi/v/mypy-boto3-iot-roborunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-roborunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot-roborunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-roborunner)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot-roborunner?color=blue)](https://pypistats.org/packages/mypy-boto3-iot-roborunner)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot-roborunner)](https://pepy.tech/project/mypy-boto3-iot-roborunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTRoboRunner 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
+[boto3.IoTRoboRunner 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
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
 [mypy-boto3-iot-roborunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,14 +300,15 @@
 ### Typed dictionaries
 
 `mypy_boto3_iot_roborunner.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot_roborunner.type_defs import (
+    CartesianCoordinatesOutputTypeDef,
     CartesianCoordinatesTypeDef,
     CreateDestinationRequestRequestTypeDef,
     CreateDestinationResponseTypeDef,
     CreateSiteRequestRequestTypeDef,
     CreateSiteResponseTypeDef,
     CreateWorkerFleetRequestRequestTypeDef,
     CreateWorkerFleetResponseTypeDef,
@@ -322,14 +323,16 @@
     GetDestinationRequestRequestTypeDef,
     GetDestinationResponseTypeDef,
     GetSiteRequestRequestTypeDef,
     GetSiteResponseTypeDef,
     GetWorkerFleetRequestRequestTypeDef,
     GetWorkerFleetResponseTypeDef,
     GetWorkerRequestRequestTypeDef,
+    OrientationOutputTypeDef,
+    VendorPropertiesOutputTypeDef,
     ListDestinationsRequestListDestinationsPaginateTypeDef,
     ListDestinationsRequestRequestTypeDef,
     ListSitesRequestListSitesPaginateTypeDef,
     ListSitesRequestRequestTypeDef,
     SiteTypeDef,
     ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
     ListWorkerFleetsRequestRequestTypeDef,
@@ -340,28 +343,29 @@
     ResponseMetadataTypeDef,
     UpdateDestinationRequestRequestTypeDef,
     UpdateDestinationResponseTypeDef,
     UpdateSiteRequestRequestTypeDef,
     UpdateSiteResponseTypeDef,
     UpdateWorkerFleetRequestRequestTypeDef,
     UpdateWorkerFleetResponseTypeDef,
+    PositionCoordinatesOutputTypeDef,
     PositionCoordinatesTypeDef,
     ListDestinationsResponseTypeDef,
     ListSitesResponseTypeDef,
     ListWorkerFleetsResponseTypeDef,
-    CreateWorkerRequestRequestTypeDef,
     GetWorkerResponseTypeDef,
-    UpdateWorkerRequestRequestTypeDef,
     UpdateWorkerResponseTypeDef,
     WorkerTypeDef,
+    CreateWorkerRequestRequestTypeDef,
+    UpdateWorkerRequestRequestTypeDef,
     ListWorkersResponseTypeDef,
 )
 
 
-def get_structure() -> CartesianCoordinatesTypeDef:
+def get_structure() -> CartesianCoordinatesOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/__init__.py` & `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/__init__.pyi` & `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/client.py` & `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/client.pyi` & `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/literals.py` & `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,15 @@
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
@@ -240,26 +241,28 @@
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

### Comparing `mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/literals.pyi` & `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,15 @@
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
@@ -238,26 +239,28 @@
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

### Comparing `mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/paginator.py` & `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/paginator.pyi` & `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/type_defs.py` & `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iot-roborunner service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iot_roborunner.type_defs import CartesianCoordinatesTypeDef
+    from mypy_boto3_iot_roborunner.type_defs import CartesianCoordinatesOutputTypeDef
 
-    data: CartesianCoordinatesTypeDef = {...}
+    data: CartesianCoordinatesOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List
 
 from .literals import DestinationStateType
@@ -20,14 +20,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "CartesianCoordinatesOutputTypeDef",
     "CartesianCoordinatesTypeDef",
     "CreateDestinationRequestRequestTypeDef",
     "CreateDestinationResponseTypeDef",
     "CreateSiteRequestRequestTypeDef",
     "CreateSiteResponseTypeDef",
     "CreateWorkerFleetRequestRequestTypeDef",
     "CreateWorkerFleetResponseTypeDef",
@@ -42,14 +43,16 @@
     "GetDestinationRequestRequestTypeDef",
     "GetDestinationResponseTypeDef",
     "GetSiteRequestRequestTypeDef",
     "GetSiteResponseTypeDef",
     "GetWorkerFleetRequestRequestTypeDef",
     "GetWorkerFleetResponseTypeDef",
     "GetWorkerRequestRequestTypeDef",
+    "OrientationOutputTypeDef",
+    "VendorPropertiesOutputTypeDef",
     "ListDestinationsRequestListDestinationsPaginateTypeDef",
     "ListDestinationsRequestRequestTypeDef",
     "ListSitesRequestListSitesPaginateTypeDef",
     "ListSitesRequestRequestTypeDef",
     "SiteTypeDef",
     "ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
     "ListWorkerFleetsRequestRequestTypeDef",
@@ -60,26 +63,49 @@
     "ResponseMetadataTypeDef",
     "UpdateDestinationRequestRequestTypeDef",
     "UpdateDestinationResponseTypeDef",
     "UpdateSiteRequestRequestTypeDef",
     "UpdateSiteResponseTypeDef",
     "UpdateWorkerFleetRequestRequestTypeDef",
     "UpdateWorkerFleetResponseTypeDef",
+    "PositionCoordinatesOutputTypeDef",
     "PositionCoordinatesTypeDef",
     "ListDestinationsResponseTypeDef",
     "ListSitesResponseTypeDef",
     "ListWorkerFleetsResponseTypeDef",
-    "CreateWorkerRequestRequestTypeDef",
     "GetWorkerResponseTypeDef",
-    "UpdateWorkerRequestRequestTypeDef",
     "UpdateWorkerResponseTypeDef",
     "WorkerTypeDef",
+    "CreateWorkerRequestRequestTypeDef",
+    "UpdateWorkerRequestRequestTypeDef",
     "ListWorkersResponseTypeDef",
 )
 
+_RequiredCartesianCoordinatesOutputTypeDef = TypedDict(
+    "_RequiredCartesianCoordinatesOutputTypeDef",
+    {
+        "x": float,
+        "y": float,
+    },
+)
+_OptionalCartesianCoordinatesOutputTypeDef = TypedDict(
+    "_OptionalCartesianCoordinatesOutputTypeDef",
+    {
+        "z": float,
+    },
+    total=False,
+)
+
+
+class CartesianCoordinatesOutputTypeDef(
+    _RequiredCartesianCoordinatesOutputTypeDef, _OptionalCartesianCoordinatesOutputTypeDef
+):
+    pass
+
+
 _RequiredCartesianCoordinatesTypeDef = TypedDict(
     "_RequiredCartesianCoordinatesTypeDef",
     {
         "x": float,
         "y": float,
     },
 )
@@ -363,14 +389,45 @@
 GetWorkerRequestRequestTypeDef = TypedDict(
     "GetWorkerRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+OrientationOutputTypeDef = TypedDict(
+    "OrientationOutputTypeDef",
+    {
+        "degrees": float,
+    },
+    total=False,
+)
+
+_RequiredVendorPropertiesOutputTypeDef = TypedDict(
+    "_RequiredVendorPropertiesOutputTypeDef",
+    {
+        "vendorWorkerId": str,
+    },
+)
+_OptionalVendorPropertiesOutputTypeDef = TypedDict(
+    "_OptionalVendorPropertiesOutputTypeDef",
+    {
+        "vendorWorkerIpAddress": str,
+        "vendorAdditionalTransientProperties": str,
+        "vendorAdditionalFixedProperties": str,
+    },
+    total=False,
+)
+
+
+class VendorPropertiesOutputTypeDef(
+    _RequiredVendorPropertiesOutputTypeDef, _OptionalVendorPropertiesOutputTypeDef
+):
+    pass
+
+
 _RequiredListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
     "_RequiredListDestinationsRequestListDestinationsPaginateTypeDef",
     {
         "site": str,
     },
 )
 _OptionalListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
@@ -677,14 +734,22 @@
         "name": str,
         "updatedAt": datetime,
         "additionalFixedProperties": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PositionCoordinatesOutputTypeDef = TypedDict(
+    "PositionCoordinatesOutputTypeDef",
+    {
+        "cartesianCoordinates": CartesianCoordinatesOutputTypeDef,
+    },
+    total=False,
+)
+
 PositionCoordinatesTypeDef = TypedDict(
     "PositionCoordinatesTypeDef",
     {
         "cartesianCoordinates": CartesianCoordinatesTypeDef,
     },
     total=False,
 )
@@ -712,129 +777,129 @@
     {
         "nextToken": str,
         "workerFleets": List[WorkerFleetTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateWorkerRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWorkerRequestRequestTypeDef",
+GetWorkerResponseTypeDef = TypedDict(
+    "GetWorkerResponseTypeDef",
     {
-        "name": str,
+        "arn": str,
+        "id": str,
         "fleet": str,
-    },
-)
-_OptionalCreateWorkerRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWorkerRequestRequestTypeDef",
-    {
-        "clientToken": str,
+        "site": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "name": str,
         "additionalTransientProperties": str,
         "additionalFixedProperties": str,
-        "vendorProperties": VendorPropertiesTypeDef,
-        "position": PositionCoordinatesTypeDef,
-        "orientation": OrientationTypeDef,
+        "vendorProperties": VendorPropertiesOutputTypeDef,
+        "position": PositionCoordinatesOutputTypeDef,
+        "orientation": OrientationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class CreateWorkerRequestRequestTypeDef(
-    _RequiredCreateWorkerRequestRequestTypeDef, _OptionalCreateWorkerRequestRequestTypeDef
-):
-    pass
-
-
-GetWorkerResponseTypeDef = TypedDict(
-    "GetWorkerResponseTypeDef",
+UpdateWorkerResponseTypeDef = TypedDict(
+    "UpdateWorkerResponseTypeDef",
     {
         "arn": str,
         "id": str,
         "fleet": str,
-        "site": str,
-        "createdAt": datetime,
         "updatedAt": datetime,
         "name": str,
         "additionalTransientProperties": str,
         "additionalFixedProperties": str,
-        "vendorProperties": VendorPropertiesTypeDef,
-        "position": PositionCoordinatesTypeDef,
-        "orientation": OrientationTypeDef,
+        "orientation": OrientationOutputTypeDef,
+        "vendorProperties": VendorPropertiesOutputTypeDef,
+        "position": PositionCoordinatesOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateWorkerRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateWorkerRequestRequestTypeDef",
+_RequiredWorkerTypeDef = TypedDict(
+    "_RequiredWorkerTypeDef",
     {
+        "arn": str,
         "id": str,
+        "fleet": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "name": str,
+        "site": str,
     },
 )
-_OptionalUpdateWorkerRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateWorkerRequestRequestTypeDef",
+_OptionalWorkerTypeDef = TypedDict(
+    "_OptionalWorkerTypeDef",
     {
-        "name": str,
         "additionalTransientProperties": str,
         "additionalFixedProperties": str,
-        "vendorProperties": VendorPropertiesTypeDef,
-        "position": PositionCoordinatesTypeDef,
-        "orientation": OrientationTypeDef,
+        "vendorProperties": VendorPropertiesOutputTypeDef,
+        "position": PositionCoordinatesOutputTypeDef,
+        "orientation": OrientationOutputTypeDef,
     },
     total=False,
 )
 
 
-class UpdateWorkerRequestRequestTypeDef(
-    _RequiredUpdateWorkerRequestRequestTypeDef, _OptionalUpdateWorkerRequestRequestTypeDef
-):
+class WorkerTypeDef(_RequiredWorkerTypeDef, _OptionalWorkerTypeDef):
     pass
 
 
-UpdateWorkerResponseTypeDef = TypedDict(
-    "UpdateWorkerResponseTypeDef",
+_RequiredCreateWorkerRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWorkerRequestRequestTypeDef",
     {
-        "arn": str,
-        "id": str,
-        "fleet": str,
-        "updatedAt": datetime,
         "name": str,
+        "fleet": str,
+    },
+)
+_OptionalCreateWorkerRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWorkerRequestRequestTypeDef",
+    {
+        "clientToken": str,
         "additionalTransientProperties": str,
         "additionalFixedProperties": str,
-        "orientation": OrientationTypeDef,
         "vendorProperties": VendorPropertiesTypeDef,
         "position": PositionCoordinatesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "orientation": OrientationTypeDef,
     },
+    total=False,
 )
 
-_RequiredWorkerTypeDef = TypedDict(
-    "_RequiredWorkerTypeDef",
+
+class CreateWorkerRequestRequestTypeDef(
+    _RequiredCreateWorkerRequestRequestTypeDef, _OptionalCreateWorkerRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateWorkerRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateWorkerRequestRequestTypeDef",
     {
-        "arn": str,
         "id": str,
-        "fleet": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "name": str,
-        "site": str,
     },
 )
-_OptionalWorkerTypeDef = TypedDict(
-    "_OptionalWorkerTypeDef",
+_OptionalUpdateWorkerRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateWorkerRequestRequestTypeDef",
     {
+        "name": str,
         "additionalTransientProperties": str,
         "additionalFixedProperties": str,
         "vendorProperties": VendorPropertiesTypeDef,
         "position": PositionCoordinatesTypeDef,
         "orientation": OrientationTypeDef,
     },
     total=False,
 )
 
 
-class WorkerTypeDef(_RequiredWorkerTypeDef, _OptionalWorkerTypeDef):
+class UpdateWorkerRequestRequestTypeDef(
+    _RequiredUpdateWorkerRequestRequestTypeDef, _OptionalUpdateWorkerRequestRequestTypeDef
+):
     pass
 
 
 ListWorkersResponseTypeDef = TypedDict(
     "ListWorkersResponseTypeDef",
     {
         "nextToken": str,
```

### Comparing `mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner/type_defs.pyi` & `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,31 +2,32 @@
 Type annotations for iot-roborunner service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iot_roborunner.type_defs import CartesianCoordinatesTypeDef
+    from mypy_boto3_iot_roborunner.type_defs import CartesianCoordinatesOutputTypeDef
 
-    data: CartesianCoordinatesTypeDef = {...}
+    data: CartesianCoordinatesOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List
 
 from .literals import DestinationStateType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "CartesianCoordinatesOutputTypeDef",
     "CartesianCoordinatesTypeDef",
     "CreateDestinationRequestRequestTypeDef",
     "CreateDestinationResponseTypeDef",
     "CreateSiteRequestRequestTypeDef",
     "CreateSiteResponseTypeDef",
     "CreateWorkerFleetRequestRequestTypeDef",
     "CreateWorkerFleetResponseTypeDef",
@@ -41,14 +42,16 @@
     "GetDestinationRequestRequestTypeDef",
     "GetDestinationResponseTypeDef",
     "GetSiteRequestRequestTypeDef",
     "GetSiteResponseTypeDef",
     "GetWorkerFleetRequestRequestTypeDef",
     "GetWorkerFleetResponseTypeDef",
     "GetWorkerRequestRequestTypeDef",
+    "OrientationOutputTypeDef",
+    "VendorPropertiesOutputTypeDef",
     "ListDestinationsRequestListDestinationsPaginateTypeDef",
     "ListDestinationsRequestRequestTypeDef",
     "ListSitesRequestListSitesPaginateTypeDef",
     "ListSitesRequestRequestTypeDef",
     "SiteTypeDef",
     "ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
     "ListWorkerFleetsRequestRequestTypeDef",
@@ -59,26 +62,47 @@
     "ResponseMetadataTypeDef",
     "UpdateDestinationRequestRequestTypeDef",
     "UpdateDestinationResponseTypeDef",
     "UpdateSiteRequestRequestTypeDef",
     "UpdateSiteResponseTypeDef",
     "UpdateWorkerFleetRequestRequestTypeDef",
     "UpdateWorkerFleetResponseTypeDef",
+    "PositionCoordinatesOutputTypeDef",
     "PositionCoordinatesTypeDef",
     "ListDestinationsResponseTypeDef",
     "ListSitesResponseTypeDef",
     "ListWorkerFleetsResponseTypeDef",
-    "CreateWorkerRequestRequestTypeDef",
     "GetWorkerResponseTypeDef",
-    "UpdateWorkerRequestRequestTypeDef",
     "UpdateWorkerResponseTypeDef",
     "WorkerTypeDef",
+    "CreateWorkerRequestRequestTypeDef",
+    "UpdateWorkerRequestRequestTypeDef",
     "ListWorkersResponseTypeDef",
 )
 
+_RequiredCartesianCoordinatesOutputTypeDef = TypedDict(
+    "_RequiredCartesianCoordinatesOutputTypeDef",
+    {
+        "x": float,
+        "y": float,
+    },
+)
+_OptionalCartesianCoordinatesOutputTypeDef = TypedDict(
+    "_OptionalCartesianCoordinatesOutputTypeDef",
+    {
+        "z": float,
+    },
+    total=False,
+)
+
+class CartesianCoordinatesOutputTypeDef(
+    _RequiredCartesianCoordinatesOutputTypeDef, _OptionalCartesianCoordinatesOutputTypeDef
+):
+    pass
+
 _RequiredCartesianCoordinatesTypeDef = TypedDict(
     "_RequiredCartesianCoordinatesTypeDef",
     {
         "x": float,
         "y": float,
     },
 )
@@ -350,14 +374,43 @@
 GetWorkerRequestRequestTypeDef = TypedDict(
     "GetWorkerRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+OrientationOutputTypeDef = TypedDict(
+    "OrientationOutputTypeDef",
+    {
+        "degrees": float,
+    },
+    total=False,
+)
+
+_RequiredVendorPropertiesOutputTypeDef = TypedDict(
+    "_RequiredVendorPropertiesOutputTypeDef",
+    {
+        "vendorWorkerId": str,
+    },
+)
+_OptionalVendorPropertiesOutputTypeDef = TypedDict(
+    "_OptionalVendorPropertiesOutputTypeDef",
+    {
+        "vendorWorkerIpAddress": str,
+        "vendorAdditionalTransientProperties": str,
+        "vendorAdditionalFixedProperties": str,
+    },
+    total=False,
+)
+
+class VendorPropertiesOutputTypeDef(
+    _RequiredVendorPropertiesOutputTypeDef, _OptionalVendorPropertiesOutputTypeDef
+):
+    pass
+
 _RequiredListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
     "_RequiredListDestinationsRequestListDestinationsPaginateTypeDef",
     {
         "site": str,
     },
 )
 _OptionalListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
@@ -644,14 +697,22 @@
         "name": str,
         "updatedAt": datetime,
         "additionalFixedProperties": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PositionCoordinatesOutputTypeDef = TypedDict(
+    "PositionCoordinatesOutputTypeDef",
+    {
+        "cartesianCoordinates": CartesianCoordinatesOutputTypeDef,
+    },
+    total=False,
+)
+
 PositionCoordinatesTypeDef = TypedDict(
     "PositionCoordinatesTypeDef",
     {
         "cartesianCoordinates": CartesianCoordinatesTypeDef,
     },
     total=False,
 )
@@ -679,124 +740,124 @@
     {
         "nextToken": str,
         "workerFleets": List[WorkerFleetTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateWorkerRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWorkerRequestRequestTypeDef",
+GetWorkerResponseTypeDef = TypedDict(
+    "GetWorkerResponseTypeDef",
     {
-        "name": str,
+        "arn": str,
+        "id": str,
         "fleet": str,
-    },
-)
-_OptionalCreateWorkerRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWorkerRequestRequestTypeDef",
-    {
-        "clientToken": str,
+        "site": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "name": str,
         "additionalTransientProperties": str,
         "additionalFixedProperties": str,
-        "vendorProperties": VendorPropertiesTypeDef,
-        "position": PositionCoordinatesTypeDef,
-        "orientation": OrientationTypeDef,
+        "vendorProperties": VendorPropertiesOutputTypeDef,
+        "position": PositionCoordinatesOutputTypeDef,
+        "orientation": OrientationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class CreateWorkerRequestRequestTypeDef(
-    _RequiredCreateWorkerRequestRequestTypeDef, _OptionalCreateWorkerRequestRequestTypeDef
-):
-    pass
-
-GetWorkerResponseTypeDef = TypedDict(
-    "GetWorkerResponseTypeDef",
+UpdateWorkerResponseTypeDef = TypedDict(
+    "UpdateWorkerResponseTypeDef",
     {
         "arn": str,
         "id": str,
         "fleet": str,
-        "site": str,
-        "createdAt": datetime,
         "updatedAt": datetime,
         "name": str,
         "additionalTransientProperties": str,
         "additionalFixedProperties": str,
-        "vendorProperties": VendorPropertiesTypeDef,
-        "position": PositionCoordinatesTypeDef,
-        "orientation": OrientationTypeDef,
+        "orientation": OrientationOutputTypeDef,
+        "vendorProperties": VendorPropertiesOutputTypeDef,
+        "position": PositionCoordinatesOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateWorkerRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateWorkerRequestRequestTypeDef",
+_RequiredWorkerTypeDef = TypedDict(
+    "_RequiredWorkerTypeDef",
     {
+        "arn": str,
         "id": str,
+        "fleet": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "name": str,
+        "site": str,
     },
 )
-_OptionalUpdateWorkerRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateWorkerRequestRequestTypeDef",
+_OptionalWorkerTypeDef = TypedDict(
+    "_OptionalWorkerTypeDef",
     {
-        "name": str,
         "additionalTransientProperties": str,
         "additionalFixedProperties": str,
-        "vendorProperties": VendorPropertiesTypeDef,
-        "position": PositionCoordinatesTypeDef,
-        "orientation": OrientationTypeDef,
+        "vendorProperties": VendorPropertiesOutputTypeDef,
+        "position": PositionCoordinatesOutputTypeDef,
+        "orientation": OrientationOutputTypeDef,
     },
     total=False,
 )
 
-class UpdateWorkerRequestRequestTypeDef(
-    _RequiredUpdateWorkerRequestRequestTypeDef, _OptionalUpdateWorkerRequestRequestTypeDef
-):
+class WorkerTypeDef(_RequiredWorkerTypeDef, _OptionalWorkerTypeDef):
     pass
 
-UpdateWorkerResponseTypeDef = TypedDict(
-    "UpdateWorkerResponseTypeDef",
+_RequiredCreateWorkerRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWorkerRequestRequestTypeDef",
     {
-        "arn": str,
-        "id": str,
-        "fleet": str,
-        "updatedAt": datetime,
         "name": str,
+        "fleet": str,
+    },
+)
+_OptionalCreateWorkerRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWorkerRequestRequestTypeDef",
+    {
+        "clientToken": str,
         "additionalTransientProperties": str,
         "additionalFixedProperties": str,
-        "orientation": OrientationTypeDef,
         "vendorProperties": VendorPropertiesTypeDef,
         "position": PositionCoordinatesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "orientation": OrientationTypeDef,
     },
+    total=False,
 )
 
-_RequiredWorkerTypeDef = TypedDict(
-    "_RequiredWorkerTypeDef",
+class CreateWorkerRequestRequestTypeDef(
+    _RequiredCreateWorkerRequestRequestTypeDef, _OptionalCreateWorkerRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateWorkerRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateWorkerRequestRequestTypeDef",
     {
-        "arn": str,
         "id": str,
-        "fleet": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "name": str,
-        "site": str,
     },
 )
-_OptionalWorkerTypeDef = TypedDict(
-    "_OptionalWorkerTypeDef",
+_OptionalUpdateWorkerRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateWorkerRequestRequestTypeDef",
     {
+        "name": str,
         "additionalTransientProperties": str,
         "additionalFixedProperties": str,
         "vendorProperties": VendorPropertiesTypeDef,
         "position": PositionCoordinatesTypeDef,
         "orientation": OrientationTypeDef,
     },
     total=False,
 )
 
-class WorkerTypeDef(_RequiredWorkerTypeDef, _OptionalWorkerTypeDef):
+class UpdateWorkerRequestRequestTypeDef(
+    _RequiredUpdateWorkerRequestRequestTypeDef, _OptionalUpdateWorkerRequestRequestTypeDef
+):
     pass
 
 ListWorkersResponseTypeDef = TypedDict(
     "ListWorkersResponseTypeDef",
     {
         "nextToken": str,
         "workers": List[WorkerTypeDef],
```

### Comparing `mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner.egg-info/PKG-INFO` & `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot-roborunner
-Version: 1.28.0
-Summary: Type annotations for boto3.IoTRoboRunner 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTRoboRunner 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iot-roborunner"></a>
 
 # mypy-boto3-iot-roborunner
 
 [![PyPI - mypy-boto3-iot-roborunner](https://img.shields.io/pypi/v/mypy-boto3-iot-roborunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-roborunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot-roborunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-roborunner)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot-roborunner?color=blue)](https://pypistats.org/packages/mypy-boto3-iot-roborunner)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot-roborunner)](https://pepy.tech/project/mypy-boto3-iot-roborunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTRoboRunner 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
+[boto3.IoTRoboRunner 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
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
 [mypy-boto3-iot-roborunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,14 +332,15 @@
 ### Typed dictionaries
 
 `mypy_boto3_iot_roborunner.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot_roborunner.type_defs import (
+    CartesianCoordinatesOutputTypeDef,
     CartesianCoordinatesTypeDef,
     CreateDestinationRequestRequestTypeDef,
     CreateDestinationResponseTypeDef,
     CreateSiteRequestRequestTypeDef,
     CreateSiteResponseTypeDef,
     CreateWorkerFleetRequestRequestTypeDef,
     CreateWorkerFleetResponseTypeDef,
@@ -354,14 +355,16 @@
     GetDestinationRequestRequestTypeDef,
     GetDestinationResponseTypeDef,
     GetSiteRequestRequestTypeDef,
     GetSiteResponseTypeDef,
     GetWorkerFleetRequestRequestTypeDef,
     GetWorkerFleetResponseTypeDef,
     GetWorkerRequestRequestTypeDef,
+    OrientationOutputTypeDef,
+    VendorPropertiesOutputTypeDef,
     ListDestinationsRequestListDestinationsPaginateTypeDef,
     ListDestinationsRequestRequestTypeDef,
     ListSitesRequestListSitesPaginateTypeDef,
     ListSitesRequestRequestTypeDef,
     SiteTypeDef,
     ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
     ListWorkerFleetsRequestRequestTypeDef,
@@ -372,28 +375,29 @@
     ResponseMetadataTypeDef,
     UpdateDestinationRequestRequestTypeDef,
     UpdateDestinationResponseTypeDef,
     UpdateSiteRequestRequestTypeDef,
     UpdateSiteResponseTypeDef,
     UpdateWorkerFleetRequestRequestTypeDef,
     UpdateWorkerFleetResponseTypeDef,
+    PositionCoordinatesOutputTypeDef,
     PositionCoordinatesTypeDef,
     ListDestinationsResponseTypeDef,
     ListSitesResponseTypeDef,
     ListWorkerFleetsResponseTypeDef,
-    CreateWorkerRequestRequestTypeDef,
     GetWorkerResponseTypeDef,
-    UpdateWorkerRequestRequestTypeDef,
     UpdateWorkerResponseTypeDef,
     WorkerTypeDef,
+    CreateWorkerRequestRequestTypeDef,
+    UpdateWorkerRequestRequestTypeDef,
     ListWorkersResponseTypeDef,
 )
 
 
-def get_structure() -> CartesianCoordinatesTypeDef:
+def get_structure() -> CartesianCoordinatesOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot-roborunner-1.28.0/mypy_boto3_iot_roborunner.egg-info/SOURCES.txt` & `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.0/setup.py` & `mypy-boto3-iot-roborunner-1.28.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iot-roborunner",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_iot_roborunner"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTRoboRunner 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.IoTRoboRunner 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

