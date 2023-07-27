# Comparing `tmp/mypy-boto3-iot1click-devices-1.28.0.tar.gz` & `tmp/mypy-boto3-iot1click-devices-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iot1click-devices-1.28.0.tar", last modified: Thu Jul  6 20:59:45 2023, max compression
+gzip compressed data, was "mypy-boto3-iot1click-devices-1.28.12.tar", last modified: Thu Jul 27 05:34:47 2023, max compression
```

## Comparing `mypy-boto3-iot1click-devices-1.28.0.tar` & `mypy-boto3-iot1click-devices-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:45.478325 mypy-boto3-iot1click-devices-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:43:34.000000 mypy-boto3-iot1click-devices-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-07-06 20:59:45.478325 mypy-boto3-iot1click-devices-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12968 2023-07-06 20:43:34.000000 mypy-boto3-iot1click-devices-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:45.470325 mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-06 20:43:34.000000 mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-06 20:43:34.000000 mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-06 20:43:34.000000 mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-07-06 20:43:34.000000 mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-07-06 20:43:34.000000 mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-07-06 20:43:34.000000 mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-07-06 20:43:34.000000 mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-06 20:43:34.000000 mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-06 20:43:34.000000 mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:43:34.000000 mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-07-06 20:43:34.000000 mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-07-06 20:43:34.000000 mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:43:34.000000 mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:45.478325 mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-07-06 20:59:45.000000 mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-06 20:59:45.000000 mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:45.000000 mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:45.000000 mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:45.000000 mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 20:59:45.000000 mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:45.478325 mypy-boto3-iot1click-devices-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-06 20:43:34.000000 mypy-boto3-iot1click-devices-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.660489 mypy-boto3-iot1click-devices-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:55.000000 mypy-boto3-iot1click-devices-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-27 05:34:47.660489 mypy-boto3-iot1click-devices-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12984 2023-07-27 05:23:55.000000 mypy-boto3-iot1click-devices-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.656489 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-27 05:23:55.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-27 05:23:55.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-27 05:23:55.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-07-27 05:23:56.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-07-27 05:23:56.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-07-27 05:23:56.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-07-27 05:23:56.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-27 05:23:56.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-27 05:23:56.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:55.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-07-27 05:23:56.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-07-27 05:23:56.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:55.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.660489 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:47.660489 mypy-boto3-iot1click-devices-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-27 05:23:54.000000 mypy-boto3-iot1click-devices-1.28.12/setup.py
```

### Comparing `mypy-boto3-iot1click-devices-1.28.0/LICENSE` & `mypy-boto3-iot1click-devices-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.0/PKG-INFO` & `mypy-boto3-iot1click-devices-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot1click-devices
-Version: 1.28.0
-Summary: Type annotations for boto3.IoT1ClickDevicesService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoT1ClickDevicesService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iot1click-devices"></a>
 
 # mypy-boto3-iot1click-devices
 
 [![PyPI - mypy-boto3-iot1click-devices](https://img.shields.io/pypi/v/mypy-boto3-iot1click-devices.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-devices)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-devices.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-devices)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot1click-devices?color=blue)](https://pypistats.org/packages/mypy-boto3-iot1click-devices)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot1click-devices)](https://pepy.tech/project/mypy-boto3-iot1click-devices)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickDevicesService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
+[boto3.IoT1ClickDevicesService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
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
 [mypy-boto3-iot1click-devices docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,14 +326,15 @@
 ```python
 from mypy_boto3_iot1click_devices.type_defs import (
     ClaimDevicesByClaimCodeRequestRequestTypeDef,
     ClaimDevicesByClaimCodeResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     DeviceDescriptionTypeDef,
     DeviceTypeDef,
+    DeviceMethodOutputTypeDef,
     DeviceMethodTypeDef,
     EmptyResponseMetadataTypeDef,
     FinalizeDeviceClaimRequestRequestTypeDef,
     FinalizeDeviceClaimResponseTypeDef,
     GetDeviceMethodsRequestRequestTypeDef,
     InitiateDeviceClaimRequestRequestTypeDef,
     InitiateDeviceClaimResponseTypeDef,
```

### Comparing `mypy-boto3-iot1click-devices-1.28.0/README.md` & `mypy-boto3-iot1click-devices-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iot1click-devices"></a>
 
 # mypy-boto3-iot1click-devices
 
 [![PyPI - mypy-boto3-iot1click-devices](https://img.shields.io/pypi/v/mypy-boto3-iot1click-devices.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-devices)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-devices.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-devices)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot1click-devices?color=blue)](https://pypistats.org/packages/mypy-boto3-iot1click-devices)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot1click-devices)](https://pepy.tech/project/mypy-boto3-iot1click-devices)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickDevicesService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
+[boto3.IoT1ClickDevicesService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
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
 [mypy-boto3-iot1click-devices docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/).
 
 See how it helps to find and fix potential bugs:
 
@@ -294,14 +294,15 @@
 ```python
 from mypy_boto3_iot1click_devices.type_defs import (
     ClaimDevicesByClaimCodeRequestRequestTypeDef,
     ClaimDevicesByClaimCodeResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     DeviceDescriptionTypeDef,
     DeviceTypeDef,
+    DeviceMethodOutputTypeDef,
     DeviceMethodTypeDef,
     EmptyResponseMetadataTypeDef,
     FinalizeDeviceClaimRequestRequestTypeDef,
     FinalizeDeviceClaimResponseTypeDef,
     GetDeviceMethodsRequestRequestTypeDef,
     InitiateDeviceClaimRequestRequestTypeDef,
     InitiateDeviceClaimResponseTypeDef,
```

### Comparing `mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/__init__.py` & `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/__init__.pyi` & `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/client.py` & `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/client.pyi` & `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/literals.py` & `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,15 @@
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
@@ -233,26 +234,28 @@
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

### Comparing `mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/literals.pyi` & `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,15 @@
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
@@ -231,26 +232,28 @@
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

### Comparing `mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/paginator.py` & `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/paginator.pyi` & `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/type_defs.py` & `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ClaimDevicesByClaimCodeRequestRequestTypeDef",
     "ClaimDevicesByClaimCodeResponseTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "DeviceDescriptionTypeDef",
     "DeviceTypeDef",
+    "DeviceMethodOutputTypeDef",
     "DeviceMethodTypeDef",
     "EmptyResponseMetadataTypeDef",
     "FinalizeDeviceClaimRequestRequestTypeDef",
     "FinalizeDeviceClaimResponseTypeDef",
     "GetDeviceMethodsRequestRequestTypeDef",
     "InitiateDeviceClaimRequestRequestTypeDef",
     "InitiateDeviceClaimResponseTypeDef",
@@ -99,14 +99,23 @@
         "Attributes": Dict[str, Any],
         "DeviceId": str,
         "Type": str,
     },
     total=False,
 )
 
+DeviceMethodOutputTypeDef = TypedDict(
+    "DeviceMethodOutputTypeDef",
+    {
+        "DeviceType": str,
+        "MethodName": str,
+    },
+    total=False,
+)
+
 DeviceMethodTypeDef = TypedDict(
     "DeviceMethodTypeDef",
     {
         "DeviceType": str,
         "MethodName": str,
     },
     total=False,
@@ -129,22 +138,20 @@
     "_OptionalFinalizeDeviceClaimRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class FinalizeDeviceClaimRequestRequestTypeDef(
     _RequiredFinalizeDeviceClaimRequestRequestTypeDef,
     _OptionalFinalizeDeviceClaimRequestRequestTypeDef,
 ):
     pass
 
-
 FinalizeDeviceClaimResponseTypeDef = TypedDict(
     "FinalizeDeviceClaimResponseTypeDef",
     {
         "State": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -191,22 +198,20 @@
     "_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListDeviceEventsRequestListDeviceEventsPaginateTypeDef(
     _RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
     _OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListDeviceEventsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeviceEventsRequestRequestTypeDef",
     {
         "DeviceId": str,
         "FromTimeStamp": Union[datetime, str],
         "ToTimeStamp": Union[datetime, str],
     },
@@ -216,21 +221,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListDeviceEventsRequestRequestTypeDef(
     _RequiredListDeviceEventsRequestRequestTypeDef, _OptionalListDeviceEventsRequestRequestTypeDef
 ):
     pass
 
-
 ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
     "ListDevicesRequestListDevicesPaginateTypeDef",
     {
         "DeviceType": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -323,21 +326,19 @@
     "_OptionalUpdateDeviceStateRequestRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-
 class UpdateDeviceStateRequestRequestTypeDef(
     _RequiredUpdateDeviceStateRequestRequestTypeDef, _OptionalUpdateDeviceStateRequestRequestTypeDef
 ):
     pass
 
-
 DescribeDeviceResponseTypeDef = TypedDict(
     "DescribeDeviceResponseTypeDef",
     {
         "DeviceDescription": DeviceDescriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -359,15 +360,15 @@
     },
     total=False,
 )
 
 GetDeviceMethodsResponseTypeDef = TypedDict(
     "GetDeviceMethodsResponseTypeDef",
     {
-        "DeviceMethods": List[DeviceMethodTypeDef],
+        "DeviceMethods": List[DeviceMethodOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredInvokeDeviceMethodRequestRequestTypeDef = TypedDict(
     "_RequiredInvokeDeviceMethodRequestRequestTypeDef",
     {
@@ -379,22 +380,20 @@
     {
         "DeviceMethod": DeviceMethodTypeDef,
         "DeviceMethodParameters": str,
     },
     total=False,
 )
 
-
 class InvokeDeviceMethodRequestRequestTypeDef(
     _RequiredInvokeDeviceMethodRequestRequestTypeDef,
     _OptionalInvokeDeviceMethodRequestRequestTypeDef,
 ):
     pass
 
-
 ListDeviceEventsResponseTypeDef = TypedDict(
     "ListDeviceEventsResponseTypeDef",
     {
         "Events": List[DeviceEventTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices/type_defs.pyi` & `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ClaimDevicesByClaimCodeRequestRequestTypeDef",
     "ClaimDevicesByClaimCodeResponseTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "DeviceDescriptionTypeDef",
     "DeviceTypeDef",
+    "DeviceMethodOutputTypeDef",
     "DeviceMethodTypeDef",
     "EmptyResponseMetadataTypeDef",
     "FinalizeDeviceClaimRequestRequestTypeDef",
     "FinalizeDeviceClaimResponseTypeDef",
     "GetDeviceMethodsRequestRequestTypeDef",
     "InitiateDeviceClaimRequestRequestTypeDef",
     "InitiateDeviceClaimResponseTypeDef",
@@ -98,14 +100,23 @@
         "Attributes": Dict[str, Any],
         "DeviceId": str,
         "Type": str,
     },
     total=False,
 )
 
+DeviceMethodOutputTypeDef = TypedDict(
+    "DeviceMethodOutputTypeDef",
+    {
+        "DeviceType": str,
+        "MethodName": str,
+    },
+    total=False,
+)
+
 DeviceMethodTypeDef = TypedDict(
     "DeviceMethodTypeDef",
     {
         "DeviceType": str,
         "MethodName": str,
     },
     total=False,
@@ -128,20 +139,22 @@
     "_OptionalFinalizeDeviceClaimRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class FinalizeDeviceClaimRequestRequestTypeDef(
     _RequiredFinalizeDeviceClaimRequestRequestTypeDef,
     _OptionalFinalizeDeviceClaimRequestRequestTypeDef,
 ):
     pass
 
+
 FinalizeDeviceClaimResponseTypeDef = TypedDict(
     "FinalizeDeviceClaimResponseTypeDef",
     {
         "State": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -188,20 +201,22 @@
     "_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListDeviceEventsRequestListDeviceEventsPaginateTypeDef(
     _RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
     _OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListDeviceEventsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeviceEventsRequestRequestTypeDef",
     {
         "DeviceId": str,
         "FromTimeStamp": Union[datetime, str],
         "ToTimeStamp": Union[datetime, str],
     },
@@ -211,19 +226,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListDeviceEventsRequestRequestTypeDef(
     _RequiredListDeviceEventsRequestRequestTypeDef, _OptionalListDeviceEventsRequestRequestTypeDef
 ):
     pass
 
+
 ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
     "ListDevicesRequestListDevicesPaginateTypeDef",
     {
         "DeviceType": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -316,19 +333,21 @@
     "_OptionalUpdateDeviceStateRequestRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+
 class UpdateDeviceStateRequestRequestTypeDef(
     _RequiredUpdateDeviceStateRequestRequestTypeDef, _OptionalUpdateDeviceStateRequestRequestTypeDef
 ):
     pass
 
+
 DescribeDeviceResponseTypeDef = TypedDict(
     "DescribeDeviceResponseTypeDef",
     {
         "DeviceDescription": DeviceDescriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -350,15 +369,15 @@
     },
     total=False,
 )
 
 GetDeviceMethodsResponseTypeDef = TypedDict(
     "GetDeviceMethodsResponseTypeDef",
     {
-        "DeviceMethods": List[DeviceMethodTypeDef],
+        "DeviceMethods": List[DeviceMethodOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredInvokeDeviceMethodRequestRequestTypeDef = TypedDict(
     "_RequiredInvokeDeviceMethodRequestRequestTypeDef",
     {
@@ -370,20 +389,22 @@
     {
         "DeviceMethod": DeviceMethodTypeDef,
         "DeviceMethodParameters": str,
     },
     total=False,
 )
 
+
 class InvokeDeviceMethodRequestRequestTypeDef(
     _RequiredInvokeDeviceMethodRequestRequestTypeDef,
     _OptionalInvokeDeviceMethodRequestRequestTypeDef,
 ):
     pass
 
+
 ListDeviceEventsResponseTypeDef = TypedDict(
     "ListDeviceEventsResponseTypeDef",
     {
         "Events": List[DeviceEventTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices.egg-info/PKG-INFO` & `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot1click-devices
-Version: 1.28.0
-Summary: Type annotations for boto3.IoT1ClickDevicesService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoT1ClickDevicesService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iot1click-devices"></a>
 
 # mypy-boto3-iot1click-devices
 
 [![PyPI - mypy-boto3-iot1click-devices](https://img.shields.io/pypi/v/mypy-boto3-iot1click-devices.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-devices)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-devices.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-devices)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot1click-devices?color=blue)](https://pypistats.org/packages/mypy-boto3-iot1click-devices)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot1click-devices)](https://pepy.tech/project/mypy-boto3-iot1click-devices)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickDevicesService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
+[boto3.IoT1ClickDevicesService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
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
 [mypy-boto3-iot1click-devices docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,14 +326,15 @@
 ```python
 from mypy_boto3_iot1click_devices.type_defs import (
     ClaimDevicesByClaimCodeRequestRequestTypeDef,
     ClaimDevicesByClaimCodeResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     DeviceDescriptionTypeDef,
     DeviceTypeDef,
+    DeviceMethodOutputTypeDef,
     DeviceMethodTypeDef,
     EmptyResponseMetadataTypeDef,
     FinalizeDeviceClaimRequestRequestTypeDef,
     FinalizeDeviceClaimResponseTypeDef,
     GetDeviceMethodsRequestRequestTypeDef,
     InitiateDeviceClaimRequestRequestTypeDef,
     InitiateDeviceClaimResponseTypeDef,
```

### Comparing `mypy-boto3-iot1click-devices-1.28.0/mypy_boto3_iot1click_devices.egg-info/SOURCES.txt` & `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.0/setup.py` & `mypy-boto3-iot1click-devices-1.28.12/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iot1click-devices",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_iot1click_devices"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoT1ClickDevicesService 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.IoT1ClickDevicesService 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

