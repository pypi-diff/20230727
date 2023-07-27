# Comparing `tmp/mypy-boto3-snow-device-management-1.28.0.tar.gz` & `tmp/mypy-boto3-snow-device-management-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-snow-device-management-1.28.0.tar", last modified: Thu Jul  6 21:00:40 2023, max compression
+gzip compressed data, was "mypy-boto3-snow-device-management-1.28.12.tar", last modified: Thu Jul 27 11:49:41 2023, max compression
```

## Comparing `mypy-boto3-snow-device-management-1.28.0.tar` & `mypy-boto3-snow-device-management-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:40.386437 mypy-boto3-snow-device-management-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:56:06.000000 mypy-boto3-snow-device-management-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-07-06 21:00:40.386437 mypy-boto3-snow-device-management-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13976 2023-07-06 20:56:06.000000 mypy-boto3-snow-device-management-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:40.378437 mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-06 20:56:06.000000 mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-06 20:56:06.000000 mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-06 20:56:06.000000 mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-07-06 20:56:06.000000 mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-07-06 20:56:06.000000 mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-07-06 20:56:06.000000 mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-07-06 20:56:06.000000 mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-06 20:56:06.000000 mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-06 20:56:06.000000 mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:56:06.000000 mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14769 2023-07-06 20:56:06.000000 mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-07-06 20:56:06.000000 mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:56:06.000000 mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:40.386437 mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-07-06 21:00:40.000000 mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-06 21:00:40.000000 mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:40.000000 mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:40.000000 mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:40.000000 mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-06 21:00:40.000000 mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:40.386437 mypy-boto3-snow-device-management-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-06 20:56:05.000000 mypy-boto3-snow-device-management-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.317317 mypy-boto3-snow-device-management-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:05.000000 mypy-boto3-snow-device-management-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-07-27 11:49:41.309317 mypy-boto3-snow-device-management-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-07-27 11:47:05.000000 mypy-boto3-snow-device-management-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.305317 mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-27 11:47:05.000000 mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-27 11:47:05.000000 mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-27 11:47:05.000000 mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-07-27 11:47:07.000000 mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-07-27 11:47:05.000000 mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-07-27 11:47:07.000000 mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-07-27 11:47:07.000000 mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-27 11:47:07.000000 mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-27 11:47:07.000000 mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:05.000000 mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-07-27 11:47:07.000000 mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14722 2023-07-27 11:47:07.000000 mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:05.000000 mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.309317 mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-07-27 11:49:41.000000 mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-27 11:49:41.000000 mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:41.000000 mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:41.000000 mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:41.000000 mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-27 11:49:41.000000 mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:41.317317 mypy-boto3-snow-device-management-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-27 11:47:05.000000 mypy-boto3-snow-device-management-1.28.12/setup.py
```

### Comparing `mypy-boto3-snow-device-management-1.28.0/LICENSE` & `mypy-boto3-snow-device-management-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snow-device-management-1.28.0/PKG-INFO` & `mypy-boto3-snow-device-management-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-snow-device-management
-Version: 1.28.0
-Summary: Type annotations for boto3.SnowDeviceManagement 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SnowDeviceManagement 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-snow-device-management"></a>
 
 # mypy-boto3-snow-device-management
 
 [![PyPI - mypy-boto3-snow-device-management](https://img.shields.io/pypi/v/mypy-boto3-snow-device-management.svg?color=blue)](https://pypi.org/project/mypy-boto3-snow-device-management)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-snow-device-management.svg?color=blue)](https://pypi.org/project/mypy-boto3-snow-device-management)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-snow-device-management?color=blue)](https://pypistats.org/packages/mypy-boto3-snow-device-management)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-snow-device-management)](https://pepy.tech/project/mypy-boto3-snow-device-management)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SnowDeviceManagement 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement)
+[boto3.SnowDeviceManagement 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement)
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
 [mypy-boto3-snow-device-management docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,54 +340,54 @@
 
 `mypy_boto3_snow_device_management.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_snow_device_management.type_defs import (
     CancelTaskInputRequestTypeDef,
-    CancelTaskOutputTypeDef,
+    ResponseMetadataTypeDef,
     CapacityTypeDef,
     CommandTypeDef,
     CpuOptionsTypeDef,
-    CreateTaskOutputTypeDef,
     DescribeDeviceEc2InputRequestTypeDef,
     DescribeDeviceInputRequestTypeDef,
     PhysicalNetworkInterfaceTypeDef,
     SoftwareInformationTypeDef,
     DescribeExecutionInputRequestTypeDef,
-    DescribeExecutionOutputTypeDef,
     DescribeTaskInputRequestTypeDef,
-    DescribeTaskOutputTypeDef,
     DeviceSummaryTypeDef,
     EbsInstanceBlockDeviceTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExecutionSummaryTypeDef,
     InstanceStateTypeDef,
     SecurityGroupIdentifierTypeDef,
-    ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDeviceResourcesInputRequestTypeDef,
     ResourceSummaryTypeDef,
-    ListDevicesInputListDevicesPaginateTypeDef,
     ListDevicesInputRequestTypeDef,
-    ListExecutionsInputListExecutionsPaginateTypeDef,
     ListExecutionsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListTasksInputListTasksPaginateTypeDef,
     ListTasksInputRequestTypeDef,
     TaskSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    CancelTaskOutputTypeDef,
+    CreateTaskOutputTypeDef,
+    DescribeExecutionOutputTypeDef,
+    DescribeTaskOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceOutputTypeDef,
     CreateTaskInputRequestTypeDef,
     DescribeDeviceOutputTypeDef,
     ListDevicesOutputTypeDef,
     InstanceBlockDeviceMappingTypeDef,
     ListExecutionsOutputTypeDef,
+    ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
+    ListDevicesInputListDevicesPaginateTypeDef,
+    ListExecutionsInputListExecutionsPaginateTypeDef,
+    ListTasksInputListTasksPaginateTypeDef,
     ListDeviceResourcesOutputTypeDef,
     ListTasksOutputTypeDef,
     InstanceTypeDef,
     InstanceSummaryTypeDef,
     DescribeDeviceEc2OutputTypeDef,
 )
```

### Comparing `mypy-boto3-snow-device-management-1.28.0/README.md` & `mypy-boto3-snow-device-management-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-snow-device-management"></a>
 
 # mypy-boto3-snow-device-management
 
 [![PyPI - mypy-boto3-snow-device-management](https://img.shields.io/pypi/v/mypy-boto3-snow-device-management.svg?color=blue)](https://pypi.org/project/mypy-boto3-snow-device-management)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-snow-device-management.svg?color=blue)](https://pypi.org/project/mypy-boto3-snow-device-management)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-snow-device-management?color=blue)](https://pypistats.org/packages/mypy-boto3-snow-device-management)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-snow-device-management)](https://pepy.tech/project/mypy-boto3-snow-device-management)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SnowDeviceManagement 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement)
+[boto3.SnowDeviceManagement 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement)
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
 [mypy-boto3-snow-device-management docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/).
 
 See how it helps to find and fix potential bugs:
 
@@ -308,54 +308,54 @@
 
 `mypy_boto3_snow_device_management.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_snow_device_management.type_defs import (
     CancelTaskInputRequestTypeDef,
-    CancelTaskOutputTypeDef,
+    ResponseMetadataTypeDef,
     CapacityTypeDef,
     CommandTypeDef,
     CpuOptionsTypeDef,
-    CreateTaskOutputTypeDef,
     DescribeDeviceEc2InputRequestTypeDef,
     DescribeDeviceInputRequestTypeDef,
     PhysicalNetworkInterfaceTypeDef,
     SoftwareInformationTypeDef,
     DescribeExecutionInputRequestTypeDef,
-    DescribeExecutionOutputTypeDef,
     DescribeTaskInputRequestTypeDef,
-    DescribeTaskOutputTypeDef,
     DeviceSummaryTypeDef,
     EbsInstanceBlockDeviceTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExecutionSummaryTypeDef,
     InstanceStateTypeDef,
     SecurityGroupIdentifierTypeDef,
-    ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDeviceResourcesInputRequestTypeDef,
     ResourceSummaryTypeDef,
-    ListDevicesInputListDevicesPaginateTypeDef,
     ListDevicesInputRequestTypeDef,
-    ListExecutionsInputListExecutionsPaginateTypeDef,
     ListExecutionsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListTasksInputListTasksPaginateTypeDef,
     ListTasksInputRequestTypeDef,
     TaskSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    CancelTaskOutputTypeDef,
+    CreateTaskOutputTypeDef,
+    DescribeExecutionOutputTypeDef,
+    DescribeTaskOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceOutputTypeDef,
     CreateTaskInputRequestTypeDef,
     DescribeDeviceOutputTypeDef,
     ListDevicesOutputTypeDef,
     InstanceBlockDeviceMappingTypeDef,
     ListExecutionsOutputTypeDef,
+    ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
+    ListDevicesInputListDevicesPaginateTypeDef,
+    ListExecutionsInputListExecutionsPaginateTypeDef,
+    ListTasksInputListTasksPaginateTypeDef,
     ListDeviceResourcesOutputTypeDef,
     ListTasksOutputTypeDef,
     InstanceTypeDef,
     InstanceSummaryTypeDef,
     DescribeDeviceEc2OutputTypeDef,
 )
```

### Comparing `mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/__init__.py` & `mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/__init__.pyi` & `mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/__main__.py` & `mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SnowDeviceManagement 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.SnowDeviceManagement 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement\nOther"
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

### Comparing `mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/client.py` & `mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/client.pyi` & `mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/literals.py` & `mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,14 +169,15 @@
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
@@ -255,26 +256,28 @@
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

### Comparing `mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/literals.pyi` & `mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -167,14 +167,15 @@
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
@@ -253,26 +254,28 @@
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

### Comparing `mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/paginator.py` & `mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,30 +63,30 @@
     """
 
     def paginate(
         self,
         *,
         managedDeviceId: str,
         type: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeviceResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListDeviceResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listdeviceresourcespaginator)
         """
 
 
 class ListDevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListDevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listdevicespaginator)
     """
 
     def paginate(
-        self, *, jobId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, jobId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listdevicespaginator)
         """
 
 
@@ -97,28 +97,28 @@
     """
 
     def paginate(
         self,
         *,
         taskId: str,
         state: ExecutionStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listexecutionspaginator)
         """
 
 
 class ListTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listtaskspaginator)
     """
 
     def paginate(
-        self, *, state: TaskStateType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, state: TaskStateType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTasksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listtaskspaginator)
         """
```

### Comparing `mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/paginator.pyi` & `mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -60,29 +60,29 @@
     """
 
     def paginate(
         self,
         *,
         managedDeviceId: str,
         type: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeviceResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListDeviceResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listdeviceresourcespaginator)
         """
 
 class ListDevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListDevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listdevicespaginator)
     """
 
     def paginate(
-        self, *, jobId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, jobId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listdevicespaginator)
         """
 
 class ListExecutionsPaginator(Paginator):
@@ -92,27 +92,27 @@
     """
 
     def paginate(
         self,
         *,
         taskId: str,
         state: ExecutionStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listexecutionspaginator)
         """
 
 class ListTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listtaskspaginator)
     """
 
     def paginate(
-        self, *, state: TaskStateType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, state: TaskStateType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTasksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listtaskspaginator)
         """
```

### Comparing `mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/type_defs.py` & `mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,73 +29,76 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CancelTaskInputRequestTypeDef",
-    "CancelTaskOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CapacityTypeDef",
     "CommandTypeDef",
     "CpuOptionsTypeDef",
-    "CreateTaskOutputTypeDef",
     "DescribeDeviceEc2InputRequestTypeDef",
     "DescribeDeviceInputRequestTypeDef",
     "PhysicalNetworkInterfaceTypeDef",
     "SoftwareInformationTypeDef",
     "DescribeExecutionInputRequestTypeDef",
-    "DescribeExecutionOutputTypeDef",
     "DescribeTaskInputRequestTypeDef",
-    "DescribeTaskOutputTypeDef",
     "DeviceSummaryTypeDef",
     "EbsInstanceBlockDeviceTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExecutionSummaryTypeDef",
     "InstanceStateTypeDef",
     "SecurityGroupIdentifierTypeDef",
-    "ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDeviceResourcesInputRequestTypeDef",
     "ResourceSummaryTypeDef",
-    "ListDevicesInputListDevicesPaginateTypeDef",
     "ListDevicesInputRequestTypeDef",
-    "ListExecutionsInputListExecutionsPaginateTypeDef",
     "ListExecutionsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "ListTasksInputListTasksPaginateTypeDef",
     "ListTasksInputRequestTypeDef",
     "TaskSummaryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "CancelTaskOutputTypeDef",
+    "CreateTaskOutputTypeDef",
+    "DescribeExecutionOutputTypeDef",
+    "DescribeTaskOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "CreateTaskInputRequestTypeDef",
     "DescribeDeviceOutputTypeDef",
     "ListDevicesOutputTypeDef",
     "InstanceBlockDeviceMappingTypeDef",
     "ListExecutionsOutputTypeDef",
+    "ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
+    "ListDevicesInputListDevicesPaginateTypeDef",
+    "ListExecutionsInputListExecutionsPaginateTypeDef",
+    "ListTasksInputListTasksPaginateTypeDef",
     "ListDeviceResourcesOutputTypeDef",
     "ListTasksOutputTypeDef",
     "InstanceTypeDef",
     "InstanceSummaryTypeDef",
     "DescribeDeviceEc2OutputTypeDef",
 )
 
 CancelTaskInputRequestTypeDef = TypedDict(
     "CancelTaskInputRequestTypeDef",
     {
         "taskId": str,
     },
 )
 
-CancelTaskOutputTypeDef = TypedDict(
-    "CancelTaskOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CapacityTypeDef = TypedDict(
     "CapacityTypeDef",
     {
         "available": int,
@@ -121,23 +124,14 @@
     {
         "coreCount": int,
         "threadsPerCore": int,
     },
     total=False,
 )
 
-CreateTaskOutputTypeDef = TypedDict(
-    "CreateTaskOutputTypeDef",
-    {
-        "taskArn": str,
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDeviceEc2InputRequestTypeDef = TypedDict(
     "DescribeDeviceEc2InputRequestTypeDef",
     {
         "instanceIds": Sequence[str],
         "managedDeviceId": str,
     },
 )
@@ -177,50 +171,21 @@
     "DescribeExecutionInputRequestTypeDef",
     {
         "managedDeviceId": str,
         "taskId": str,
     },
 )
 
-DescribeExecutionOutputTypeDef = TypedDict(
-    "DescribeExecutionOutputTypeDef",
-    {
-        "executionId": str,
-        "lastUpdatedAt": datetime,
-        "managedDeviceId": str,
-        "startedAt": datetime,
-        "state": ExecutionStateType,
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeTaskInputRequestTypeDef = TypedDict(
     "DescribeTaskInputRequestTypeDef",
     {
         "taskId": str,
     },
 )
 
-DescribeTaskOutputTypeDef = TypedDict(
-    "DescribeTaskOutputTypeDef",
-    {
-        "completedAt": datetime,
-        "createdAt": datetime,
-        "description": str,
-        "lastUpdatedAt": datetime,
-        "state": TaskStateType,
-        "tags": Dict[str, str],
-        "targets": List[str],
-        "taskArn": str,
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeviceSummaryTypeDef = TypedDict(
     "DeviceSummaryTypeDef",
     {
         "associatedWithJob": str,
         "managedDeviceArn": str,
         "managedDeviceId": str,
         "tags": Dict[str, str],
@@ -235,21 +200,14 @@
         "deleteOnTermination": bool,
         "status": AttachmentStatusType,
         "volumeId": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExecutionSummaryTypeDef = TypedDict(
     "ExecutionSummaryTypeDef",
     {
         "executionId": str,
         "managedDeviceId": str,
         "state": ExecutionStateType,
         "taskId": str,
@@ -271,37 +229,24 @@
     {
         "groupId": str,
         "groupName": str,
     },
     total=False,
 )
 
-_RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
-    {
-        "managedDeviceId": str,
-    },
-)
-_OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "type": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef(
-    _RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
-    _OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDeviceResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListDeviceResourcesInputRequestTypeDef",
     {
         "managedDeviceId": str,
     },
 )
 _OptionalListDeviceResourcesInputRequestTypeDef = TypedDict(
@@ -337,56 +282,24 @@
 )
 
 
 class ResourceSummaryTypeDef(_RequiredResourceSummaryTypeDef, _OptionalResourceSummaryTypeDef):
     pass
 
 
-ListDevicesInputListDevicesPaginateTypeDef = TypedDict(
-    "ListDevicesInputListDevicesPaginateTypeDef",
-    {
-        "jobId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDevicesInputRequestTypeDef = TypedDict(
     "ListDevicesInputRequestTypeDef",
     {
         "jobId": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListExecutionsInputListExecutionsPaginateTypeDef",
-    {
-        "taskId": str,
-    },
-)
-_OptionalListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListExecutionsInputListExecutionsPaginateTypeDef",
-    {
-        "state": ExecutionStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListExecutionsInputListExecutionsPaginateTypeDef(
-    _RequiredListExecutionsInputListExecutionsPaginateTypeDef,
-    _OptionalListExecutionsInputListExecutionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredListExecutionsInputRequestTypeDef",
     {
         "taskId": str,
     },
 )
 _OptionalListExecutionsInputRequestTypeDef = TypedDict(
@@ -409,31 +322,14 @@
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
-ListTasksInputListTasksPaginateTypeDef = TypedDict(
-    "ListTasksInputListTasksPaginateTypeDef",
-    {
-        "state": TaskStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTasksInputRequestTypeDef = TypedDict(
     "ListTasksInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "state": TaskStateType,
     },
@@ -457,35 +353,14 @@
 )
 
 
 class TaskSummaryTypeDef(_RequiredTaskSummaryTypeDef, _OptionalTaskSummaryTypeDef):
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
@@ -494,14 +369,75 @@
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+CancelTaskOutputTypeDef = TypedDict(
+    "CancelTaskOutputTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTaskOutputTypeDef = TypedDict(
+    "CreateTaskOutputTypeDef",
+    {
+        "taskArn": str,
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeExecutionOutputTypeDef = TypedDict(
+    "DescribeExecutionOutputTypeDef",
+    {
+        "executionId": str,
+        "lastUpdatedAt": datetime,
+        "managedDeviceId": str,
+        "startedAt": datetime,
+        "state": ExecutionStateType,
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTaskOutputTypeDef = TypedDict(
+    "DescribeTaskOutputTypeDef",
+    {
+        "completedAt": datetime,
+        "createdAt": datetime,
+        "description": str,
+        "lastUpdatedAt": datetime,
+        "state": TaskStateType,
+        "tags": Dict[str, str],
+        "targets": List[str],
+        "taskArn": str,
+        "taskId": str,
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
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateTaskInputRequestTypeDef = TypedDict(
     "_RequiredCreateTaskInputRequestTypeDef",
     {
         "command": CommandTypeDef,
         "targets": Sequence[str],
     },
 )
@@ -532,24 +468,24 @@
         "lastReachedOutAt": datetime,
         "lastUpdatedAt": datetime,
         "managedDeviceArn": str,
         "managedDeviceId": str,
         "physicalNetworkInterfaces": List[PhysicalNetworkInterfaceTypeDef],
         "software": SoftwareInformationTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDevicesOutputTypeDef = TypedDict(
     "ListDevicesOutputTypeDef",
     {
         "devices": List[DeviceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceBlockDeviceMappingTypeDef = TypedDict(
     "InstanceBlockDeviceMappingTypeDef",
     {
         "deviceName": str,
@@ -559,33 +495,97 @@
 )
 
 ListExecutionsOutputTypeDef = TypedDict(
     "ListExecutionsOutputTypeDef",
     {
         "executions": List[ExecutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
+    {
+        "managedDeviceId": str,
+    },
+)
+_OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
+    {
+        "type": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef(
+    _RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
+    _OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
+):
+    pass
+
+
+ListDevicesInputListDevicesPaginateTypeDef = TypedDict(
+    "ListDevicesInputListDevicesPaginateTypeDef",
+    {
+        "jobId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListExecutionsInputListExecutionsPaginateTypeDef",
+    {
+        "taskId": str,
+    },
+)
+_OptionalListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListExecutionsInputListExecutionsPaginateTypeDef",
+    {
+        "state": ExecutionStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListExecutionsInputListExecutionsPaginateTypeDef(
+    _RequiredListExecutionsInputListExecutionsPaginateTypeDef,
+    _OptionalListExecutionsInputListExecutionsPaginateTypeDef,
+):
+    pass
+
+
+ListTasksInputListTasksPaginateTypeDef = TypedDict(
+    "ListTasksInputListTasksPaginateTypeDef",
+    {
+        "state": TaskStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListDeviceResourcesOutputTypeDef = TypedDict(
     "ListDeviceResourcesOutputTypeDef",
     {
         "nextToken": str,
         "resources": List[ResourceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTasksOutputTypeDef = TypedDict(
     "ListTasksOutputTypeDef",
     {
         "nextToken": str,
         "tasks": List[TaskSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "amiLaunchIndex": int,
@@ -614,10 +614,10 @@
     total=False,
 )
 
 DescribeDeviceEc2OutputTypeDef = TypedDict(
     "DescribeDeviceEc2OutputTypeDef",
     {
         "instances": List[InstanceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management/type_defs.pyi` & `mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -28,73 +28,76 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CancelTaskInputRequestTypeDef",
-    "CancelTaskOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CapacityTypeDef",
     "CommandTypeDef",
     "CpuOptionsTypeDef",
-    "CreateTaskOutputTypeDef",
     "DescribeDeviceEc2InputRequestTypeDef",
     "DescribeDeviceInputRequestTypeDef",
     "PhysicalNetworkInterfaceTypeDef",
     "SoftwareInformationTypeDef",
     "DescribeExecutionInputRequestTypeDef",
-    "DescribeExecutionOutputTypeDef",
     "DescribeTaskInputRequestTypeDef",
-    "DescribeTaskOutputTypeDef",
     "DeviceSummaryTypeDef",
     "EbsInstanceBlockDeviceTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExecutionSummaryTypeDef",
     "InstanceStateTypeDef",
     "SecurityGroupIdentifierTypeDef",
-    "ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDeviceResourcesInputRequestTypeDef",
     "ResourceSummaryTypeDef",
-    "ListDevicesInputListDevicesPaginateTypeDef",
     "ListDevicesInputRequestTypeDef",
-    "ListExecutionsInputListExecutionsPaginateTypeDef",
     "ListExecutionsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "ListTasksInputListTasksPaginateTypeDef",
     "ListTasksInputRequestTypeDef",
     "TaskSummaryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "CancelTaskOutputTypeDef",
+    "CreateTaskOutputTypeDef",
+    "DescribeExecutionOutputTypeDef",
+    "DescribeTaskOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "CreateTaskInputRequestTypeDef",
     "DescribeDeviceOutputTypeDef",
     "ListDevicesOutputTypeDef",
     "InstanceBlockDeviceMappingTypeDef",
     "ListExecutionsOutputTypeDef",
+    "ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
+    "ListDevicesInputListDevicesPaginateTypeDef",
+    "ListExecutionsInputListExecutionsPaginateTypeDef",
+    "ListTasksInputListTasksPaginateTypeDef",
     "ListDeviceResourcesOutputTypeDef",
     "ListTasksOutputTypeDef",
     "InstanceTypeDef",
     "InstanceSummaryTypeDef",
     "DescribeDeviceEc2OutputTypeDef",
 )
 
 CancelTaskInputRequestTypeDef = TypedDict(
     "CancelTaskInputRequestTypeDef",
     {
         "taskId": str,
     },
 )
 
-CancelTaskOutputTypeDef = TypedDict(
-    "CancelTaskOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CapacityTypeDef = TypedDict(
     "CapacityTypeDef",
     {
         "available": int,
@@ -120,23 +123,14 @@
     {
         "coreCount": int,
         "threadsPerCore": int,
     },
     total=False,
 )
 
-CreateTaskOutputTypeDef = TypedDict(
-    "CreateTaskOutputTypeDef",
-    {
-        "taskArn": str,
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDeviceEc2InputRequestTypeDef = TypedDict(
     "DescribeDeviceEc2InputRequestTypeDef",
     {
         "instanceIds": Sequence[str],
         "managedDeviceId": str,
     },
 )
@@ -176,50 +170,21 @@
     "DescribeExecutionInputRequestTypeDef",
     {
         "managedDeviceId": str,
         "taskId": str,
     },
 )
 
-DescribeExecutionOutputTypeDef = TypedDict(
-    "DescribeExecutionOutputTypeDef",
-    {
-        "executionId": str,
-        "lastUpdatedAt": datetime,
-        "managedDeviceId": str,
-        "startedAt": datetime,
-        "state": ExecutionStateType,
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeTaskInputRequestTypeDef = TypedDict(
     "DescribeTaskInputRequestTypeDef",
     {
         "taskId": str,
     },
 )
 
-DescribeTaskOutputTypeDef = TypedDict(
-    "DescribeTaskOutputTypeDef",
-    {
-        "completedAt": datetime,
-        "createdAt": datetime,
-        "description": str,
-        "lastUpdatedAt": datetime,
-        "state": TaskStateType,
-        "tags": Dict[str, str],
-        "targets": List[str],
-        "taskArn": str,
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeviceSummaryTypeDef = TypedDict(
     "DeviceSummaryTypeDef",
     {
         "associatedWithJob": str,
         "managedDeviceArn": str,
         "managedDeviceId": str,
         "tags": Dict[str, str],
@@ -234,21 +199,14 @@
         "deleteOnTermination": bool,
         "status": AttachmentStatusType,
         "volumeId": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExecutionSummaryTypeDef = TypedDict(
     "ExecutionSummaryTypeDef",
     {
         "executionId": str,
         "managedDeviceId": str,
         "state": ExecutionStateType,
         "taskId": str,
@@ -270,35 +228,24 @@
     {
         "groupId": str,
         "groupName": str,
     },
     total=False,
 )
 
-_RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
-    {
-        "managedDeviceId": str,
-    },
-)
-_OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "type": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef(
-    _RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
-    _OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredListDeviceResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListDeviceResourcesInputRequestTypeDef",
     {
         "managedDeviceId": str,
     },
 )
 _OptionalListDeviceResourcesInputRequestTypeDef = TypedDict(
@@ -330,54 +277,24 @@
     },
     total=False,
 )
 
 class ResourceSummaryTypeDef(_RequiredResourceSummaryTypeDef, _OptionalResourceSummaryTypeDef):
     pass
 
-ListDevicesInputListDevicesPaginateTypeDef = TypedDict(
-    "ListDevicesInputListDevicesPaginateTypeDef",
-    {
-        "jobId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDevicesInputRequestTypeDef = TypedDict(
     "ListDevicesInputRequestTypeDef",
     {
         "jobId": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListExecutionsInputListExecutionsPaginateTypeDef",
-    {
-        "taskId": str,
-    },
-)
-_OptionalListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListExecutionsInputListExecutionsPaginateTypeDef",
-    {
-        "state": ExecutionStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListExecutionsInputListExecutionsPaginateTypeDef(
-    _RequiredListExecutionsInputListExecutionsPaginateTypeDef,
-    _OptionalListExecutionsInputListExecutionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredListExecutionsInputRequestTypeDef",
     {
         "taskId": str,
     },
 )
 _OptionalListExecutionsInputRequestTypeDef = TypedDict(
@@ -398,31 +315,14 @@
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
-ListTasksInputListTasksPaginateTypeDef = TypedDict(
-    "ListTasksInputListTasksPaginateTypeDef",
-    {
-        "state": TaskStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTasksInputRequestTypeDef = TypedDict(
     "ListTasksInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "state": TaskStateType,
     },
@@ -444,35 +344,14 @@
     },
     total=False,
 )
 
 class TaskSummaryTypeDef(_RequiredTaskSummaryTypeDef, _OptionalTaskSummaryTypeDef):
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
@@ -481,14 +360,75 @@
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+CancelTaskOutputTypeDef = TypedDict(
+    "CancelTaskOutputTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTaskOutputTypeDef = TypedDict(
+    "CreateTaskOutputTypeDef",
+    {
+        "taskArn": str,
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeExecutionOutputTypeDef = TypedDict(
+    "DescribeExecutionOutputTypeDef",
+    {
+        "executionId": str,
+        "lastUpdatedAt": datetime,
+        "managedDeviceId": str,
+        "startedAt": datetime,
+        "state": ExecutionStateType,
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTaskOutputTypeDef = TypedDict(
+    "DescribeTaskOutputTypeDef",
+    {
+        "completedAt": datetime,
+        "createdAt": datetime,
+        "description": str,
+        "lastUpdatedAt": datetime,
+        "state": TaskStateType,
+        "tags": Dict[str, str],
+        "targets": List[str],
+        "taskArn": str,
+        "taskId": str,
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
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateTaskInputRequestTypeDef = TypedDict(
     "_RequiredCreateTaskInputRequestTypeDef",
     {
         "command": CommandTypeDef,
         "targets": Sequence[str],
     },
 )
@@ -517,24 +457,24 @@
         "lastReachedOutAt": datetime,
         "lastUpdatedAt": datetime,
         "managedDeviceArn": str,
         "managedDeviceId": str,
         "physicalNetworkInterfaces": List[PhysicalNetworkInterfaceTypeDef],
         "software": SoftwareInformationTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDevicesOutputTypeDef = TypedDict(
     "ListDevicesOutputTypeDef",
     {
         "devices": List[DeviceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceBlockDeviceMappingTypeDef = TypedDict(
     "InstanceBlockDeviceMappingTypeDef",
     {
         "deviceName": str,
@@ -544,33 +484,93 @@
 )
 
 ListExecutionsOutputTypeDef = TypedDict(
     "ListExecutionsOutputTypeDef",
     {
         "executions": List[ExecutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
+    {
+        "managedDeviceId": str,
     },
 )
+_OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
+    {
+        "type": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef(
+    _RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
+    _OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
+):
+    pass
+
+ListDevicesInputListDevicesPaginateTypeDef = TypedDict(
+    "ListDevicesInputListDevicesPaginateTypeDef",
+    {
+        "jobId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListExecutionsInputListExecutionsPaginateTypeDef",
+    {
+        "taskId": str,
+    },
+)
+_OptionalListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListExecutionsInputListExecutionsPaginateTypeDef",
+    {
+        "state": ExecutionStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListExecutionsInputListExecutionsPaginateTypeDef(
+    _RequiredListExecutionsInputListExecutionsPaginateTypeDef,
+    _OptionalListExecutionsInputListExecutionsPaginateTypeDef,
+):
+    pass
+
+ListTasksInputListTasksPaginateTypeDef = TypedDict(
+    "ListTasksInputListTasksPaginateTypeDef",
+    {
+        "state": TaskStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 ListDeviceResourcesOutputTypeDef = TypedDict(
     "ListDeviceResourcesOutputTypeDef",
     {
         "nextToken": str,
         "resources": List[ResourceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTasksOutputTypeDef = TypedDict(
     "ListTasksOutputTypeDef",
     {
         "nextToken": str,
         "tasks": List[TaskSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "amiLaunchIndex": int,
@@ -599,10 +599,10 @@
     total=False,
 )
 
 DescribeDeviceEc2OutputTypeDef = TypedDict(
     "DescribeDeviceEc2OutputTypeDef",
     {
         "instances": List[InstanceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management.egg-info/PKG-INFO` & `mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-snow-device-management
-Version: 1.28.0
-Summary: Type annotations for boto3.SnowDeviceManagement 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SnowDeviceManagement 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-snow-device-management"></a>
 
 # mypy-boto3-snow-device-management
 
 [![PyPI - mypy-boto3-snow-device-management](https://img.shields.io/pypi/v/mypy-boto3-snow-device-management.svg?color=blue)](https://pypi.org/project/mypy-boto3-snow-device-management)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-snow-device-management.svg?color=blue)](https://pypi.org/project/mypy-boto3-snow-device-management)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-snow-device-management?color=blue)](https://pypistats.org/packages/mypy-boto3-snow-device-management)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-snow-device-management)](https://pepy.tech/project/mypy-boto3-snow-device-management)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SnowDeviceManagement 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement)
+[boto3.SnowDeviceManagement 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement)
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
 [mypy-boto3-snow-device-management docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,54 +340,54 @@
 
 `mypy_boto3_snow_device_management.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_snow_device_management.type_defs import (
     CancelTaskInputRequestTypeDef,
-    CancelTaskOutputTypeDef,
+    ResponseMetadataTypeDef,
     CapacityTypeDef,
     CommandTypeDef,
     CpuOptionsTypeDef,
-    CreateTaskOutputTypeDef,
     DescribeDeviceEc2InputRequestTypeDef,
     DescribeDeviceInputRequestTypeDef,
     PhysicalNetworkInterfaceTypeDef,
     SoftwareInformationTypeDef,
     DescribeExecutionInputRequestTypeDef,
-    DescribeExecutionOutputTypeDef,
     DescribeTaskInputRequestTypeDef,
-    DescribeTaskOutputTypeDef,
     DeviceSummaryTypeDef,
     EbsInstanceBlockDeviceTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExecutionSummaryTypeDef,
     InstanceStateTypeDef,
     SecurityGroupIdentifierTypeDef,
-    ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDeviceResourcesInputRequestTypeDef,
     ResourceSummaryTypeDef,
-    ListDevicesInputListDevicesPaginateTypeDef,
     ListDevicesInputRequestTypeDef,
-    ListExecutionsInputListExecutionsPaginateTypeDef,
     ListExecutionsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListTasksInputListTasksPaginateTypeDef,
     ListTasksInputRequestTypeDef,
     TaskSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    CancelTaskOutputTypeDef,
+    CreateTaskOutputTypeDef,
+    DescribeExecutionOutputTypeDef,
+    DescribeTaskOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceOutputTypeDef,
     CreateTaskInputRequestTypeDef,
     DescribeDeviceOutputTypeDef,
     ListDevicesOutputTypeDef,
     InstanceBlockDeviceMappingTypeDef,
     ListExecutionsOutputTypeDef,
+    ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
+    ListDevicesInputListDevicesPaginateTypeDef,
+    ListExecutionsInputListExecutionsPaginateTypeDef,
+    ListTasksInputListTasksPaginateTypeDef,
     ListDeviceResourcesOutputTypeDef,
     ListTasksOutputTypeDef,
     InstanceTypeDef,
     InstanceSummaryTypeDef,
     DescribeDeviceEc2OutputTypeDef,
 )
```

### Comparing `mypy-boto3-snow-device-management-1.28.0/mypy_boto3_snow_device_management.egg-info/SOURCES.txt` & `mypy-boto3-snow-device-management-1.28.12/mypy_boto3_snow_device_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snow-device-management-1.28.0/setup.py` & `mypy-boto3-snow-device-management-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-snow-device-management",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_snow_device_management"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SnowDeviceManagement 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SnowDeviceManagement 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

