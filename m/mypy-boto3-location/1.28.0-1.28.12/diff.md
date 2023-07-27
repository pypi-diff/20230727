# Comparing `tmp/mypy-boto3-location-1.28.0.tar.gz` & `tmp/mypy-boto3-location-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-location-1.28.0.tar", last modified: Thu Jul  6 21:00:01 2023, max compression
+gzip compressed data, was "mypy-boto3-location-1.28.12.tar", last modified: Thu Jul 27 05:34:57 2023, max compression
```

## Comparing `mypy-boto3-location-1.28.0.tar` & `mypy-boto3-location-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:01.026357 mypy-boto3-location-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:46:01.000000 mypy-boto3-location-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21053 2023-07-06 21:00:01.026357 mypy-boto3-location-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19557 2023-07-06 20:46:01.000000 mypy-boto3-location-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:01.026357 mypy-boto3-location-1.28.0/mypy_boto3_location/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-06 20:46:01.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-06 20:46:01.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-06 20:46:01.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45543 2023-07-06 20:46:02.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    45468 2023-07-06 20:46:02.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10278 2023-07-06 20:46:02.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-07-06 20:46:02.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-07-06 20:46:02.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11798 2023-07-06 20:46:02.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:46:01.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    65082 2023-07-06 20:46:04.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    64971 2023-07-06 20:46:03.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:46:01.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:01.026357 mypy-boto3-location-1.28.0/mypy_boto3_location.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21053 2023-07-06 21:00:00.000000 mypy-boto3-location-1.28.0/mypy_boto3_location.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 21:00:00.000000 mypy-boto3-location-1.28.0/mypy_boto3_location.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:00.000000 mypy-boto3-location-1.28.0/mypy_boto3_location.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:00.000000 mypy-boto3-location-1.28.0/mypy_boto3_location.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:00.000000 mypy-boto3-location-1.28.0/mypy_boto3_location.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:00:00.000000 mypy-boto3-location-1.28.0/mypy_boto3_location.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:01.026357 mypy-boto3-location-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 20:46:01.000000 mypy-boto3-location-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.476454 mypy-boto3-location-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:30.000000 mypy-boto3-location-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21251 2023-07-27 05:34:57.476454 mypy-boto3-location-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19753 2023-07-27 05:25:30.000000 mypy-boto3-location-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.476454 mypy-boto3-location-1.28.12/mypy_boto3_location/
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-27 05:25:30.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-27 05:25:30.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-27 05:25:30.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45543 2023-07-27 05:25:31.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45468 2023-07-27 05:25:31.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-07-27 05:25:31.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-07-27 05:25:31.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-07-27 05:25:31.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11798 2023-07-27 05:25:31.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:30.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    66915 2023-07-27 05:25:32.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66800 2023-07-27 05:25:32.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:30.000000 mypy-boto3-location-1.28.12/mypy_boto3_location/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.476454 mypy-boto3-location-1.28.12/mypy_boto3_location.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21251 2023-07-27 05:34:57.000000 mypy-boto3-location-1.28.12/mypy_boto3_location.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 05:34:57.000000 mypy-boto3-location-1.28.12/mypy_boto3_location.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-location-1.28.12/mypy_boto3_location.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-location-1.28.12/mypy_boto3_location.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:57.000000 mypy-boto3-location-1.28.12/mypy_boto3_location.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 05:34:57.000000 mypy-boto3-location-1.28.12/mypy_boto3_location.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:57.476454 mypy-boto3-location-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:25:30.000000 mypy-boto3-location-1.28.12/setup.py
```

### Comparing `mypy-boto3-location-1.28.0/LICENSE` & `mypy-boto3-location-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.0/PKG-INFO` & `mypy-boto3-location-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-location
-Version: 1.28.0
-Summary: Type annotations for boto3.LocationService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.LocationService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-location"></a>
 
 # mypy-boto3-location
 
 [![PyPI - mypy-boto3-location](https://img.shields.io/pypi/v/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-location?color=blue)](https://pypistats.org/packages/mypy-boto3-location)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-location)](https://pepy.tech/project/mypy-boto3-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LocationService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[boto3.LocationService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
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
 [mypy-boto3-location docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,53 +368,58 @@
 
 `mypy_boto3_location.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_location.type_defs import (
     ApiKeyFilterTypeDef,
+    ApiKeyRestrictionsOutputTypeDef,
     ApiKeyRestrictionsTypeDef,
     AssociateTrackerConsumerRequestRequestTypeDef,
     BatchItemErrorTypeDef,
     BatchDeleteDevicePositionHistoryRequestRequestTypeDef,
     BatchDeleteGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionRequestRequestTypeDef,
     BatchPutGeofenceSuccessTypeDef,
     CalculateRouteCarModeOptionsTypeDef,
     CalculateRouteMatrixSummaryTypeDef,
     CalculateRouteSummaryTypeDef,
     TruckDimensionsTypeDef,
     TruckWeightTypeDef,
+    CircleOutputTypeDef,
     CircleTypeDef,
     CreateGeofenceCollectionRequestRequestTypeDef,
     CreateGeofenceCollectionResponseTypeDef,
     CreateKeyResponseTypeDef,
     MapConfigurationTypeDef,
     CreateMapResponseTypeDef,
     DataSourceConfigurationTypeDef,
     CreatePlaceIndexResponseTypeDef,
     CreateRouteCalculatorRequestRequestTypeDef,
     CreateRouteCalculatorResponseTypeDef,
     CreateTrackerRequestRequestTypeDef,
     CreateTrackerResponseTypeDef,
+    DataSourceConfigurationOutputTypeDef,
     DeleteGeofenceCollectionRequestRequestTypeDef,
     DeleteKeyRequestRequestTypeDef,
     DeleteMapRequestRequestTypeDef,
     DeletePlaceIndexRequestRequestTypeDef,
     DeleteRouteCalculatorRequestRequestTypeDef,
     DeleteTrackerRequestRequestTypeDef,
     DescribeGeofenceCollectionRequestRequestTypeDef,
     DescribeGeofenceCollectionResponseTypeDef,
     DescribeKeyRequestRequestTypeDef,
     DescribeMapRequestRequestTypeDef,
+    MapConfigurationOutputTypeDef,
     DescribePlaceIndexRequestRequestTypeDef,
     DescribeRouteCalculatorRequestRequestTypeDef,
     DescribeRouteCalculatorResponseTypeDef,
     DescribeTrackerRequestRequestTypeDef,
     DescribeTrackerResponseTypeDef,
+    PositionalAccuracyOutputTypeDef,
     PositionalAccuracyTypeDef,
     DisassociateTrackerConsumerRequestRequestTypeDef,
     GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
     GetDevicePositionHistoryRequestRequestTypeDef,
     GetDevicePositionRequestRequestTypeDef,
     GetGeofenceRequestRequestTypeDef,
     GetMapGlyphsRequestRequestTypeDef,
@@ -475,35 +480,36 @@
     UpdatePlaceIndexResponseTypeDef,
     UpdateRouteCalculatorRequestRequestTypeDef,
     UpdateRouteCalculatorResponseTypeDef,
     UpdateTrackerRequestRequestTypeDef,
     UpdateTrackerResponseTypeDef,
     ListKeysRequestListKeysPaginateTypeDef,
     ListKeysRequestRequestTypeDef,
-    CreateKeyRequestRequestTypeDef,
     DescribeKeyResponseTypeDef,
     ListKeysResponseEntryTypeDef,
+    CreateKeyRequestRequestTypeDef,
     UpdateKeyRequestRequestTypeDef,
     BatchDeleteDevicePositionHistoryErrorTypeDef,
     BatchDeleteGeofenceErrorTypeDef,
     BatchEvaluateGeofencesErrorTypeDef,
     BatchGetDevicePositionErrorTypeDef,
     BatchPutGeofenceErrorTypeDef,
     BatchUpdateDevicePositionErrorTypeDef,
     CalculateRouteTruckModeOptionsTypeDef,
+    GeofenceGeometryOutputTypeDef,
     GeofenceGeometryTypeDef,
     CreateMapRequestRequestTypeDef,
-    DescribeMapResponseTypeDef,
     CreatePlaceIndexRequestRequestTypeDef,
-    DescribePlaceIndexResponseTypeDef,
     UpdatePlaceIndexRequestRequestTypeDef,
+    DescribePlaceIndexResponseTypeDef,
+    DescribeMapResponseTypeDef,
     DevicePositionTypeDef,
-    DevicePositionUpdateTypeDef,
     GetDevicePositionResponseTypeDef,
     ListDevicePositionsResponseEntryTypeDef,
+    DevicePositionUpdateTypeDef,
     LegTypeDef,
     ListGeofenceCollectionsResponseTypeDef,
     ListMapsResponseTypeDef,
     ListPlaceIndexesResponseTypeDef,
     ListRouteCalculatorsResponseTypeDef,
     ListTrackersResponseTypeDef,
     UpdateMapRequestRequestTypeDef,
@@ -514,30 +520,30 @@
     BatchDeleteDevicePositionHistoryResponseTypeDef,
     BatchDeleteGeofenceResponseTypeDef,
     BatchEvaluateGeofencesResponseTypeDef,
     BatchPutGeofenceResponseTypeDef,
     BatchUpdateDevicePositionResponseTypeDef,
     CalculateRouteMatrixRequestRequestTypeDef,
     CalculateRouteRequestRequestTypeDef,
-    BatchPutGeofenceRequestEntryTypeDef,
     GetGeofenceResponseTypeDef,
     ListGeofenceResponseEntryTypeDef,
+    BatchPutGeofenceRequestEntryTypeDef,
     PutGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionResponseTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
+    ListDevicePositionsResponseTypeDef,
     BatchEvaluateGeofencesRequestRequestTypeDef,
     BatchUpdateDevicePositionRequestRequestTypeDef,
-    ListDevicePositionsResponseTypeDef,
     CalculateRouteResponseTypeDef,
     GetPlaceResponseTypeDef,
     SearchForPositionResultTypeDef,
     SearchForTextResultTypeDef,
     CalculateRouteMatrixResponseTypeDef,
-    BatchPutGeofenceRequestRequestTypeDef,
     ListGeofencesResponseTypeDef,
+    BatchPutGeofenceRequestRequestTypeDef,
     SearchPlaceIndexForPositionResponseTypeDef,
     SearchPlaceIndexForTextResponseTypeDef,
 )
 
 
 def get_structure() -> ApiKeyFilterTypeDef:
     return {...}
```

### Comparing `mypy-boto3-location-1.28.0/README.md` & `mypy-boto3-location-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-location"></a>
 
 # mypy-boto3-location
 
 [![PyPI - mypy-boto3-location](https://img.shields.io/pypi/v/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-location?color=blue)](https://pypistats.org/packages/mypy-boto3-location)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-location)](https://pepy.tech/project/mypy-boto3-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LocationService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[boto3.LocationService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
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
 [mypy-boto3-location docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,53 +336,58 @@
 
 `mypy_boto3_location.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_location.type_defs import (
     ApiKeyFilterTypeDef,
+    ApiKeyRestrictionsOutputTypeDef,
     ApiKeyRestrictionsTypeDef,
     AssociateTrackerConsumerRequestRequestTypeDef,
     BatchItemErrorTypeDef,
     BatchDeleteDevicePositionHistoryRequestRequestTypeDef,
     BatchDeleteGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionRequestRequestTypeDef,
     BatchPutGeofenceSuccessTypeDef,
     CalculateRouteCarModeOptionsTypeDef,
     CalculateRouteMatrixSummaryTypeDef,
     CalculateRouteSummaryTypeDef,
     TruckDimensionsTypeDef,
     TruckWeightTypeDef,
+    CircleOutputTypeDef,
     CircleTypeDef,
     CreateGeofenceCollectionRequestRequestTypeDef,
     CreateGeofenceCollectionResponseTypeDef,
     CreateKeyResponseTypeDef,
     MapConfigurationTypeDef,
     CreateMapResponseTypeDef,
     DataSourceConfigurationTypeDef,
     CreatePlaceIndexResponseTypeDef,
     CreateRouteCalculatorRequestRequestTypeDef,
     CreateRouteCalculatorResponseTypeDef,
     CreateTrackerRequestRequestTypeDef,
     CreateTrackerResponseTypeDef,
+    DataSourceConfigurationOutputTypeDef,
     DeleteGeofenceCollectionRequestRequestTypeDef,
     DeleteKeyRequestRequestTypeDef,
     DeleteMapRequestRequestTypeDef,
     DeletePlaceIndexRequestRequestTypeDef,
     DeleteRouteCalculatorRequestRequestTypeDef,
     DeleteTrackerRequestRequestTypeDef,
     DescribeGeofenceCollectionRequestRequestTypeDef,
     DescribeGeofenceCollectionResponseTypeDef,
     DescribeKeyRequestRequestTypeDef,
     DescribeMapRequestRequestTypeDef,
+    MapConfigurationOutputTypeDef,
     DescribePlaceIndexRequestRequestTypeDef,
     DescribeRouteCalculatorRequestRequestTypeDef,
     DescribeRouteCalculatorResponseTypeDef,
     DescribeTrackerRequestRequestTypeDef,
     DescribeTrackerResponseTypeDef,
+    PositionalAccuracyOutputTypeDef,
     PositionalAccuracyTypeDef,
     DisassociateTrackerConsumerRequestRequestTypeDef,
     GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
     GetDevicePositionHistoryRequestRequestTypeDef,
     GetDevicePositionRequestRequestTypeDef,
     GetGeofenceRequestRequestTypeDef,
     GetMapGlyphsRequestRequestTypeDef,
@@ -443,35 +448,36 @@
     UpdatePlaceIndexResponseTypeDef,
     UpdateRouteCalculatorRequestRequestTypeDef,
     UpdateRouteCalculatorResponseTypeDef,
     UpdateTrackerRequestRequestTypeDef,
     UpdateTrackerResponseTypeDef,
     ListKeysRequestListKeysPaginateTypeDef,
     ListKeysRequestRequestTypeDef,
-    CreateKeyRequestRequestTypeDef,
     DescribeKeyResponseTypeDef,
     ListKeysResponseEntryTypeDef,
+    CreateKeyRequestRequestTypeDef,
     UpdateKeyRequestRequestTypeDef,
     BatchDeleteDevicePositionHistoryErrorTypeDef,
     BatchDeleteGeofenceErrorTypeDef,
     BatchEvaluateGeofencesErrorTypeDef,
     BatchGetDevicePositionErrorTypeDef,
     BatchPutGeofenceErrorTypeDef,
     BatchUpdateDevicePositionErrorTypeDef,
     CalculateRouteTruckModeOptionsTypeDef,
+    GeofenceGeometryOutputTypeDef,
     GeofenceGeometryTypeDef,
     CreateMapRequestRequestTypeDef,
-    DescribeMapResponseTypeDef,
     CreatePlaceIndexRequestRequestTypeDef,
-    DescribePlaceIndexResponseTypeDef,
     UpdatePlaceIndexRequestRequestTypeDef,
+    DescribePlaceIndexResponseTypeDef,
+    DescribeMapResponseTypeDef,
     DevicePositionTypeDef,
-    DevicePositionUpdateTypeDef,
     GetDevicePositionResponseTypeDef,
     ListDevicePositionsResponseEntryTypeDef,
+    DevicePositionUpdateTypeDef,
     LegTypeDef,
     ListGeofenceCollectionsResponseTypeDef,
     ListMapsResponseTypeDef,
     ListPlaceIndexesResponseTypeDef,
     ListRouteCalculatorsResponseTypeDef,
     ListTrackersResponseTypeDef,
     UpdateMapRequestRequestTypeDef,
@@ -482,30 +488,30 @@
     BatchDeleteDevicePositionHistoryResponseTypeDef,
     BatchDeleteGeofenceResponseTypeDef,
     BatchEvaluateGeofencesResponseTypeDef,
     BatchPutGeofenceResponseTypeDef,
     BatchUpdateDevicePositionResponseTypeDef,
     CalculateRouteMatrixRequestRequestTypeDef,
     CalculateRouteRequestRequestTypeDef,
-    BatchPutGeofenceRequestEntryTypeDef,
     GetGeofenceResponseTypeDef,
     ListGeofenceResponseEntryTypeDef,
+    BatchPutGeofenceRequestEntryTypeDef,
     PutGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionResponseTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
+    ListDevicePositionsResponseTypeDef,
     BatchEvaluateGeofencesRequestRequestTypeDef,
     BatchUpdateDevicePositionRequestRequestTypeDef,
-    ListDevicePositionsResponseTypeDef,
     CalculateRouteResponseTypeDef,
     GetPlaceResponseTypeDef,
     SearchForPositionResultTypeDef,
     SearchForTextResultTypeDef,
     CalculateRouteMatrixResponseTypeDef,
-    BatchPutGeofenceRequestRequestTypeDef,
     ListGeofencesResponseTypeDef,
+    BatchPutGeofenceRequestRequestTypeDef,
     SearchPlaceIndexForPositionResponseTypeDef,
     SearchPlaceIndexForTextResponseTypeDef,
 )
 
 
 def get_structure() -> ApiKeyFilterTypeDef:
     return {...}
```

### Comparing `mypy-boto3-location-1.28.0/mypy_boto3_location/__init__.py` & `mypy-boto3-location-1.28.12/mypy_boto3_location/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.0/mypy_boto3_location/__init__.pyi` & `mypy-boto3-location-1.28.12/mypy_boto3_location/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.0/mypy_boto3_location/__main__.py` & `mypy-boto3-location-1.28.12/mypy_boto3_location/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LocationService 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.LocationService 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService\nOther"
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

### Comparing `mypy-boto3-location-1.28.0/mypy_boto3_location/client.py` & `mypy-boto3-location-1.28.12/mypy_boto3_location/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.0/mypy_boto3_location/client.pyi` & `mypy-boto3-location-1.28.12/mypy_boto3_location/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.0/mypy_boto3_location/literals.py` & `mypy-boto3-location-1.28.12/mypy_boto3_location/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -198,14 +198,15 @@
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
@@ -284,26 +285,28 @@
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

### Comparing `mypy-boto3-location-1.28.0/mypy_boto3_location/literals.pyi` & `mypy-boto3-location-1.28.12/mypy_boto3_location/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -196,14 +196,15 @@
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
@@ -282,26 +283,28 @@
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

### Comparing `mypy-boto3-location-1.28.0/mypy_boto3_location/paginator.py` & `mypy-boto3-location-1.28.12/mypy_boto3_location/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.0/mypy_boto3_location/paginator.pyi` & `mypy-boto3-location-1.28.12/mypy_boto3_location/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.0/mypy_boto3_location/type_defs.py` & `mypy-boto3-location-1.28.12/mypy_boto3_location/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,53 +34,58 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ApiKeyFilterTypeDef",
+    "ApiKeyRestrictionsOutputTypeDef",
     "ApiKeyRestrictionsTypeDef",
     "AssociateTrackerConsumerRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
     "BatchDeleteDevicePositionHistoryRequestRequestTypeDef",
     "BatchDeleteGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionRequestRequestTypeDef",
     "BatchPutGeofenceSuccessTypeDef",
     "CalculateRouteCarModeOptionsTypeDef",
     "CalculateRouteMatrixSummaryTypeDef",
     "CalculateRouteSummaryTypeDef",
     "TruckDimensionsTypeDef",
     "TruckWeightTypeDef",
+    "CircleOutputTypeDef",
     "CircleTypeDef",
     "CreateGeofenceCollectionRequestRequestTypeDef",
     "CreateGeofenceCollectionResponseTypeDef",
     "CreateKeyResponseTypeDef",
     "MapConfigurationTypeDef",
     "CreateMapResponseTypeDef",
     "DataSourceConfigurationTypeDef",
     "CreatePlaceIndexResponseTypeDef",
     "CreateRouteCalculatorRequestRequestTypeDef",
     "CreateRouteCalculatorResponseTypeDef",
     "CreateTrackerRequestRequestTypeDef",
     "CreateTrackerResponseTypeDef",
+    "DataSourceConfigurationOutputTypeDef",
     "DeleteGeofenceCollectionRequestRequestTypeDef",
     "DeleteKeyRequestRequestTypeDef",
     "DeleteMapRequestRequestTypeDef",
     "DeletePlaceIndexRequestRequestTypeDef",
     "DeleteRouteCalculatorRequestRequestTypeDef",
     "DeleteTrackerRequestRequestTypeDef",
     "DescribeGeofenceCollectionRequestRequestTypeDef",
     "DescribeGeofenceCollectionResponseTypeDef",
     "DescribeKeyRequestRequestTypeDef",
     "DescribeMapRequestRequestTypeDef",
+    "MapConfigurationOutputTypeDef",
     "DescribePlaceIndexRequestRequestTypeDef",
     "DescribeRouteCalculatorRequestRequestTypeDef",
     "DescribeRouteCalculatorResponseTypeDef",
     "DescribeTrackerRequestRequestTypeDef",
     "DescribeTrackerResponseTypeDef",
+    "PositionalAccuracyOutputTypeDef",
     "PositionalAccuracyTypeDef",
     "DisassociateTrackerConsumerRequestRequestTypeDef",
     "GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
     "GetDevicePositionHistoryRequestRequestTypeDef",
     "GetDevicePositionRequestRequestTypeDef",
     "GetGeofenceRequestRequestTypeDef",
     "GetMapGlyphsRequestRequestTypeDef",
@@ -141,35 +146,36 @@
     "UpdatePlaceIndexResponseTypeDef",
     "UpdateRouteCalculatorRequestRequestTypeDef",
     "UpdateRouteCalculatorResponseTypeDef",
     "UpdateTrackerRequestRequestTypeDef",
     "UpdateTrackerResponseTypeDef",
     "ListKeysRequestListKeysPaginateTypeDef",
     "ListKeysRequestRequestTypeDef",
-    "CreateKeyRequestRequestTypeDef",
     "DescribeKeyResponseTypeDef",
     "ListKeysResponseEntryTypeDef",
+    "CreateKeyRequestRequestTypeDef",
     "UpdateKeyRequestRequestTypeDef",
     "BatchDeleteDevicePositionHistoryErrorTypeDef",
     "BatchDeleteGeofenceErrorTypeDef",
     "BatchEvaluateGeofencesErrorTypeDef",
     "BatchGetDevicePositionErrorTypeDef",
     "BatchPutGeofenceErrorTypeDef",
     "BatchUpdateDevicePositionErrorTypeDef",
     "CalculateRouteTruckModeOptionsTypeDef",
+    "GeofenceGeometryOutputTypeDef",
     "GeofenceGeometryTypeDef",
     "CreateMapRequestRequestTypeDef",
-    "DescribeMapResponseTypeDef",
     "CreatePlaceIndexRequestRequestTypeDef",
-    "DescribePlaceIndexResponseTypeDef",
     "UpdatePlaceIndexRequestRequestTypeDef",
+    "DescribePlaceIndexResponseTypeDef",
+    "DescribeMapResponseTypeDef",
     "DevicePositionTypeDef",
-    "DevicePositionUpdateTypeDef",
     "GetDevicePositionResponseTypeDef",
     "ListDevicePositionsResponseEntryTypeDef",
+    "DevicePositionUpdateTypeDef",
     "LegTypeDef",
     "ListGeofenceCollectionsResponseTypeDef",
     "ListMapsResponseTypeDef",
     "ListPlaceIndexesResponseTypeDef",
     "ListRouteCalculatorsResponseTypeDef",
     "ListTrackersResponseTypeDef",
     "UpdateMapRequestRequestTypeDef",
@@ -180,42 +186,64 @@
     "BatchDeleteDevicePositionHistoryResponseTypeDef",
     "BatchDeleteGeofenceResponseTypeDef",
     "BatchEvaluateGeofencesResponseTypeDef",
     "BatchPutGeofenceResponseTypeDef",
     "BatchUpdateDevicePositionResponseTypeDef",
     "CalculateRouteMatrixRequestRequestTypeDef",
     "CalculateRouteRequestRequestTypeDef",
-    "BatchPutGeofenceRequestEntryTypeDef",
     "GetGeofenceResponseTypeDef",
     "ListGeofenceResponseEntryTypeDef",
+    "BatchPutGeofenceRequestEntryTypeDef",
     "PutGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionResponseTypeDef",
     "GetDevicePositionHistoryResponseTypeDef",
+    "ListDevicePositionsResponseTypeDef",
     "BatchEvaluateGeofencesRequestRequestTypeDef",
     "BatchUpdateDevicePositionRequestRequestTypeDef",
-    "ListDevicePositionsResponseTypeDef",
     "CalculateRouteResponseTypeDef",
     "GetPlaceResponseTypeDef",
     "SearchForPositionResultTypeDef",
     "SearchForTextResultTypeDef",
     "CalculateRouteMatrixResponseTypeDef",
-    "BatchPutGeofenceRequestRequestTypeDef",
     "ListGeofencesResponseTypeDef",
+    "BatchPutGeofenceRequestRequestTypeDef",
     "SearchPlaceIndexForPositionResponseTypeDef",
     "SearchPlaceIndexForTextResponseTypeDef",
 )
 
 ApiKeyFilterTypeDef = TypedDict(
     "ApiKeyFilterTypeDef",
     {
         "KeyStatus": StatusType,
     },
     total=False,
 )
 
+_RequiredApiKeyRestrictionsOutputTypeDef = TypedDict(
+    "_RequiredApiKeyRestrictionsOutputTypeDef",
+    {
+        "AllowActions": List[str],
+        "AllowResources": List[str],
+    },
+)
+_OptionalApiKeyRestrictionsOutputTypeDef = TypedDict(
+    "_OptionalApiKeyRestrictionsOutputTypeDef",
+    {
+        "AllowReferers": List[str],
+    },
+    total=False,
+)
+
+
+class ApiKeyRestrictionsOutputTypeDef(
+    _RequiredApiKeyRestrictionsOutputTypeDef, _OptionalApiKeyRestrictionsOutputTypeDef
+):
+    pass
+
+
 _RequiredApiKeyRestrictionsTypeDef = TypedDict(
     "_RequiredApiKeyRestrictionsTypeDef",
     {
         "AllowActions": Sequence[str],
         "AllowResources": Sequence[str],
     },
 )
@@ -330,14 +358,22 @@
     {
         "Total": float,
         "Unit": VehicleWeightUnitType,
     },
     total=False,
 )
 
+CircleOutputTypeDef = TypedDict(
+    "CircleOutputTypeDef",
+    {
+        "Center": List[float],
+        "Radius": float,
+    },
+)
+
 CircleTypeDef = TypedDict(
     "CircleTypeDef",
     {
         "Center": Sequence[float],
         "Radius": float,
     },
 )
@@ -504,14 +540,22 @@
         "CreateTime": datetime,
         "TrackerArn": str,
         "TrackerName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DataSourceConfigurationOutputTypeDef = TypedDict(
+    "DataSourceConfigurationOutputTypeDef",
+    {
+        "IntendedUse": IntendedUseType,
+    },
+    total=False,
+)
+
 DeleteGeofenceCollectionRequestRequestTypeDef = TypedDict(
     "DeleteGeofenceCollectionRequestRequestTypeDef",
     {
         "CollectionName": str,
     },
 )
 
@@ -583,14 +627,35 @@
 DescribeMapRequestRequestTypeDef = TypedDict(
     "DescribeMapRequestRequestTypeDef",
     {
         "MapName": str,
     },
 )
 
+_RequiredMapConfigurationOutputTypeDef = TypedDict(
+    "_RequiredMapConfigurationOutputTypeDef",
+    {
+        "Style": str,
+    },
+)
+_OptionalMapConfigurationOutputTypeDef = TypedDict(
+    "_OptionalMapConfigurationOutputTypeDef",
+    {
+        "PoliticalView": str,
+    },
+    total=False,
+)
+
+
+class MapConfigurationOutputTypeDef(
+    _RequiredMapConfigurationOutputTypeDef, _OptionalMapConfigurationOutputTypeDef
+):
+    pass
+
+
 DescribePlaceIndexRequestRequestTypeDef = TypedDict(
     "DescribePlaceIndexRequestRequestTypeDef",
     {
         "IndexName": str,
     },
 )
 
@@ -637,14 +702,21 @@
         "TrackerArn": str,
         "TrackerName": str,
         "UpdateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PositionalAccuracyOutputTypeDef = TypedDict(
+    "PositionalAccuracyOutputTypeDef",
+    {
+        "Horizontal": float,
+    },
+)
+
 PositionalAccuracyTypeDef = TypedDict(
     "PositionalAccuracyTypeDef",
     {
         "Horizontal": float,
     },
 )
 
@@ -1713,62 +1785,37 @@
         "Filter": ApiKeyFilterTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredCreateKeyRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKeyRequestRequestTypeDef",
-    {
-        "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsTypeDef,
-    },
-)
-_OptionalCreateKeyRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKeyRequestRequestTypeDef",
-    {
-        "Description": str,
-        "ExpireTime": Union[datetime, str],
-        "NoExpiry": bool,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateKeyRequestRequestTypeDef(
-    _RequiredCreateKeyRequestRequestTypeDef, _OptionalCreateKeyRequestRequestTypeDef
-):
-    pass
-
-
 DescribeKeyResponseTypeDef = TypedDict(
     "DescribeKeyResponseTypeDef",
     {
         "CreateTime": datetime,
         "Description": str,
         "ExpireTime": datetime,
         "Key": str,
         "KeyArn": str,
         "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsTypeDef,
+        "Restrictions": ApiKeyRestrictionsOutputTypeDef,
         "Tags": Dict[str, str],
         "UpdateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListKeysResponseEntryTypeDef = TypedDict(
     "_RequiredListKeysResponseEntryTypeDef",
     {
         "CreateTime": datetime,
         "ExpireTime": datetime,
         "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsTypeDef,
+        "Restrictions": ApiKeyRestrictionsOutputTypeDef,
         "UpdateTime": datetime,
     },
 )
 _OptionalListKeysResponseEntryTypeDef = TypedDict(
     "_OptionalListKeysResponseEntryTypeDef",
     {
         "Description": str,
@@ -1779,14 +1826,39 @@
 
 class ListKeysResponseEntryTypeDef(
     _RequiredListKeysResponseEntryTypeDef, _OptionalListKeysResponseEntryTypeDef
 ):
     pass
 
 
+_RequiredCreateKeyRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKeyRequestRequestTypeDef",
+    {
+        "KeyName": str,
+        "Restrictions": ApiKeyRestrictionsTypeDef,
+    },
+)
+_OptionalCreateKeyRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKeyRequestRequestTypeDef",
+    {
+        "Description": str,
+        "ExpireTime": Union[datetime, str],
+        "NoExpiry": bool,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateKeyRequestRequestTypeDef(
+    _RequiredCreateKeyRequestRequestTypeDef, _OptionalCreateKeyRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredUpdateKeyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKeyRequestRequestTypeDef",
     {
         "KeyName": str,
     },
 )
 _OptionalUpdateKeyRequestRequestTypeDef = TypedDict(
@@ -1865,14 +1937,23 @@
         "AvoidTolls": bool,
         "Dimensions": TruckDimensionsTypeDef,
         "Weight": TruckWeightTypeDef,
     },
     total=False,
 )
 
+GeofenceGeometryOutputTypeDef = TypedDict(
+    "GeofenceGeometryOutputTypeDef",
+    {
+        "Circle": CircleOutputTypeDef,
+        "Polygon": List[List[List[float]]],
+    },
+    total=False,
+)
+
 GeofenceGeometryTypeDef = TypedDict(
     "GeofenceGeometryTypeDef",
     {
         "Circle": CircleTypeDef,
         "Polygon": Sequence[Sequence[Sequence[float]]],
     },
     total=False,
@@ -1898,30 +1979,14 @@
 
 class CreateMapRequestRequestTypeDef(
     _RequiredCreateMapRequestRequestTypeDef, _OptionalCreateMapRequestRequestTypeDef
 ):
     pass
 
 
-DescribeMapResponseTypeDef = TypedDict(
-    "DescribeMapResponseTypeDef",
-    {
-        "Configuration": MapConfigurationTypeDef,
-        "CreateTime": datetime,
-        "DataSource": str,
-        "Description": str,
-        "MapArn": str,
-        "MapName": str,
-        "PricingPlan": PricingPlanType,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePlaceIndexRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePlaceIndexRequestRequestTypeDef",
     {
         "DataSource": str,
         "IndexName": str,
     },
 )
@@ -1939,30 +2004,14 @@
 
 class CreatePlaceIndexRequestRequestTypeDef(
     _RequiredCreatePlaceIndexRequestRequestTypeDef, _OptionalCreatePlaceIndexRequestRequestTypeDef
 ):
     pass
 
 
-DescribePlaceIndexResponseTypeDef = TypedDict(
-    "DescribePlaceIndexResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "DataSource": str,
-        "DataSourceConfiguration": DataSourceConfigurationTypeDef,
-        "Description": str,
-        "IndexArn": str,
-        "IndexName": str,
-        "PricingPlan": PricingPlanType,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePlaceIndexRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePlaceIndexRequestRequestTypeDef",
     {
         "IndexName": str,
     },
 )
 _OptionalUpdatePlaceIndexRequestRequestTypeDef = TypedDict(
@@ -1978,65 +2027,73 @@
 
 class UpdatePlaceIndexRequestRequestTypeDef(
     _RequiredUpdatePlaceIndexRequestRequestTypeDef, _OptionalUpdatePlaceIndexRequestRequestTypeDef
 ):
     pass
 
 
+DescribePlaceIndexResponseTypeDef = TypedDict(
+    "DescribePlaceIndexResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "DataSource": str,
+        "DataSourceConfiguration": DataSourceConfigurationOutputTypeDef,
+        "Description": str,
+        "IndexArn": str,
+        "IndexName": str,
+        "PricingPlan": PricingPlanType,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeMapResponseTypeDef = TypedDict(
+    "DescribeMapResponseTypeDef",
+    {
+        "Configuration": MapConfigurationOutputTypeDef,
+        "CreateTime": datetime,
+        "DataSource": str,
+        "Description": str,
+        "MapArn": str,
+        "MapName": str,
+        "PricingPlan": PricingPlanType,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDevicePositionTypeDef = TypedDict(
     "_RequiredDevicePositionTypeDef",
     {
         "Position": List[float],
         "ReceivedTime": datetime,
         "SampleTime": datetime,
     },
 )
 _OptionalDevicePositionTypeDef = TypedDict(
     "_OptionalDevicePositionTypeDef",
     {
-        "Accuracy": PositionalAccuracyTypeDef,
+        "Accuracy": PositionalAccuracyOutputTypeDef,
         "DeviceId": str,
         "PositionProperties": Dict[str, str],
     },
     total=False,
 )
 
 
 class DevicePositionTypeDef(_RequiredDevicePositionTypeDef, _OptionalDevicePositionTypeDef):
     pass
 
 
-_RequiredDevicePositionUpdateTypeDef = TypedDict(
-    "_RequiredDevicePositionUpdateTypeDef",
-    {
-        "DeviceId": str,
-        "Position": Sequence[float],
-        "SampleTime": Union[datetime, str],
-    },
-)
-_OptionalDevicePositionUpdateTypeDef = TypedDict(
-    "_OptionalDevicePositionUpdateTypeDef",
-    {
-        "Accuracy": PositionalAccuracyTypeDef,
-        "PositionProperties": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class DevicePositionUpdateTypeDef(
-    _RequiredDevicePositionUpdateTypeDef, _OptionalDevicePositionUpdateTypeDef
-):
-    pass
-
-
 GetDevicePositionResponseTypeDef = TypedDict(
     "GetDevicePositionResponseTypeDef",
     {
-        "Accuracy": PositionalAccuracyTypeDef,
+        "Accuracy": PositionalAccuracyOutputTypeDef,
         "DeviceId": str,
         "Position": List[float],
         "PositionProperties": Dict[str, str],
         "ReceivedTime": datetime,
         "SampleTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2049,28 +2106,52 @@
         "Position": List[float],
         "SampleTime": datetime,
     },
 )
 _OptionalListDevicePositionsResponseEntryTypeDef = TypedDict(
     "_OptionalListDevicePositionsResponseEntryTypeDef",
     {
-        "Accuracy": PositionalAccuracyTypeDef,
+        "Accuracy": PositionalAccuracyOutputTypeDef,
         "PositionProperties": Dict[str, str],
     },
     total=False,
 )
 
 
 class ListDevicePositionsResponseEntryTypeDef(
     _RequiredListDevicePositionsResponseEntryTypeDef,
     _OptionalListDevicePositionsResponseEntryTypeDef,
 ):
     pass
 
 
+_RequiredDevicePositionUpdateTypeDef = TypedDict(
+    "_RequiredDevicePositionUpdateTypeDef",
+    {
+        "DeviceId": str,
+        "Position": Sequence[float],
+        "SampleTime": Union[datetime, str],
+    },
+)
+_OptionalDevicePositionUpdateTypeDef = TypedDict(
+    "_OptionalDevicePositionUpdateTypeDef",
+    {
+        "Accuracy": PositionalAccuracyTypeDef,
+        "PositionProperties": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class DevicePositionUpdateTypeDef(
+    _RequiredDevicePositionUpdateTypeDef, _OptionalDevicePositionUpdateTypeDef
+):
+    pass
+
+
 _RequiredLegTypeDef = TypedDict(
     "_RequiredLegTypeDef",
     {
         "Distance": float,
         "DurationSeconds": float,
         "EndPosition": List[float],
         "StartPosition": List[float],
@@ -2317,55 +2398,33 @@
 
 class CalculateRouteRequestRequestTypeDef(
     _RequiredCalculateRouteRequestRequestTypeDef, _OptionalCalculateRouteRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredBatchPutGeofenceRequestEntryTypeDef = TypedDict(
-    "_RequiredBatchPutGeofenceRequestEntryTypeDef",
-    {
-        "GeofenceId": str,
-        "Geometry": GeofenceGeometryTypeDef,
-    },
-)
-_OptionalBatchPutGeofenceRequestEntryTypeDef = TypedDict(
-    "_OptionalBatchPutGeofenceRequestEntryTypeDef",
-    {
-        "GeofenceProperties": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class BatchPutGeofenceRequestEntryTypeDef(
-    _RequiredBatchPutGeofenceRequestEntryTypeDef, _OptionalBatchPutGeofenceRequestEntryTypeDef
-):
-    pass
-
-
 GetGeofenceResponseTypeDef = TypedDict(
     "GetGeofenceResponseTypeDef",
     {
         "CreateTime": datetime,
         "GeofenceId": str,
         "GeofenceProperties": Dict[str, str],
-        "Geometry": GeofenceGeometryTypeDef,
+        "Geometry": GeofenceGeometryOutputTypeDef,
         "Status": str,
         "UpdateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListGeofenceResponseEntryTypeDef = TypedDict(
     "_RequiredListGeofenceResponseEntryTypeDef",
     {
         "CreateTime": datetime,
         "GeofenceId": str,
-        "Geometry": GeofenceGeometryTypeDef,
+        "Geometry": GeofenceGeometryOutputTypeDef,
         "Status": str,
         "UpdateTime": datetime,
     },
 )
 _OptionalListGeofenceResponseEntryTypeDef = TypedDict(
     "_OptionalListGeofenceResponseEntryTypeDef",
     {
@@ -2377,14 +2436,36 @@
 
 class ListGeofenceResponseEntryTypeDef(
     _RequiredListGeofenceResponseEntryTypeDef, _OptionalListGeofenceResponseEntryTypeDef
 ):
     pass
 
 
+_RequiredBatchPutGeofenceRequestEntryTypeDef = TypedDict(
+    "_RequiredBatchPutGeofenceRequestEntryTypeDef",
+    {
+        "GeofenceId": str,
+        "Geometry": GeofenceGeometryTypeDef,
+    },
+)
+_OptionalBatchPutGeofenceRequestEntryTypeDef = TypedDict(
+    "_OptionalBatchPutGeofenceRequestEntryTypeDef",
+    {
+        "GeofenceProperties": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class BatchPutGeofenceRequestEntryTypeDef(
+    _RequiredBatchPutGeofenceRequestEntryTypeDef, _OptionalBatchPutGeofenceRequestEntryTypeDef
+):
+    pass
+
+
 _RequiredPutGeofenceRequestRequestTypeDef = TypedDict(
     "_RequiredPutGeofenceRequestRequestTypeDef",
     {
         "CollectionName": str,
         "GeofenceId": str,
         "Geometry": GeofenceGeometryTypeDef,
     },
@@ -2418,14 +2499,23 @@
     {
         "DevicePositions": List[DevicePositionTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListDevicePositionsResponseTypeDef = TypedDict(
+    "ListDevicePositionsResponseTypeDef",
+    {
+        "Entries": List[ListDevicePositionsResponseEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BatchEvaluateGeofencesRequestRequestTypeDef = TypedDict(
     "BatchEvaluateGeofencesRequestRequestTypeDef",
     {
         "CollectionName": str,
         "DevicePositionUpdates": Sequence[DevicePositionUpdateTypeDef],
     },
 )
@@ -2434,23 +2524,14 @@
     "BatchUpdateDevicePositionRequestRequestTypeDef",
     {
         "TrackerName": str,
         "Updates": Sequence[DevicePositionUpdateTypeDef],
     },
 )
 
-ListDevicePositionsResponseTypeDef = TypedDict(
-    "ListDevicePositionsResponseTypeDef",
-    {
-        "Entries": List[ListDevicePositionsResponseEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CalculateRouteResponseTypeDef = TypedDict(
     "CalculateRouteResponseTypeDef",
     {
         "Legs": List[LegTypeDef],
         "Summary": CalculateRouteSummaryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2516,31 +2597,31 @@
         "SnappedDeparturePositions": List[List[float]],
         "SnappedDestinationPositions": List[List[float]],
         "Summary": CalculateRouteMatrixSummaryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-BatchPutGeofenceRequestRequestTypeDef = TypedDict(
-    "BatchPutGeofenceRequestRequestTypeDef",
-    {
-        "CollectionName": str,
-        "Entries": Sequence[BatchPutGeofenceRequestEntryTypeDef],
-    },
-)
-
 ListGeofencesResponseTypeDef = TypedDict(
     "ListGeofencesResponseTypeDef",
     {
         "Entries": List[ListGeofenceResponseEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+BatchPutGeofenceRequestRequestTypeDef = TypedDict(
+    "BatchPutGeofenceRequestRequestTypeDef",
+    {
+        "CollectionName": str,
+        "Entries": Sequence[BatchPutGeofenceRequestEntryTypeDef],
+    },
+)
+
 SearchPlaceIndexForPositionResponseTypeDef = TypedDict(
     "SearchPlaceIndexForPositionResponseTypeDef",
     {
         "Results": List[SearchForPositionResultTypeDef],
         "Summary": SearchPlaceIndexForPositionSummaryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-location-1.28.0/mypy_boto3_location/type_defs.pyi` & `mypy-boto3-location-1.28.12/mypy_boto3_location/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -33,53 +33,58 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ApiKeyFilterTypeDef",
+    "ApiKeyRestrictionsOutputTypeDef",
     "ApiKeyRestrictionsTypeDef",
     "AssociateTrackerConsumerRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
     "BatchDeleteDevicePositionHistoryRequestRequestTypeDef",
     "BatchDeleteGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionRequestRequestTypeDef",
     "BatchPutGeofenceSuccessTypeDef",
     "CalculateRouteCarModeOptionsTypeDef",
     "CalculateRouteMatrixSummaryTypeDef",
     "CalculateRouteSummaryTypeDef",
     "TruckDimensionsTypeDef",
     "TruckWeightTypeDef",
+    "CircleOutputTypeDef",
     "CircleTypeDef",
     "CreateGeofenceCollectionRequestRequestTypeDef",
     "CreateGeofenceCollectionResponseTypeDef",
     "CreateKeyResponseTypeDef",
     "MapConfigurationTypeDef",
     "CreateMapResponseTypeDef",
     "DataSourceConfigurationTypeDef",
     "CreatePlaceIndexResponseTypeDef",
     "CreateRouteCalculatorRequestRequestTypeDef",
     "CreateRouteCalculatorResponseTypeDef",
     "CreateTrackerRequestRequestTypeDef",
     "CreateTrackerResponseTypeDef",
+    "DataSourceConfigurationOutputTypeDef",
     "DeleteGeofenceCollectionRequestRequestTypeDef",
     "DeleteKeyRequestRequestTypeDef",
     "DeleteMapRequestRequestTypeDef",
     "DeletePlaceIndexRequestRequestTypeDef",
     "DeleteRouteCalculatorRequestRequestTypeDef",
     "DeleteTrackerRequestRequestTypeDef",
     "DescribeGeofenceCollectionRequestRequestTypeDef",
     "DescribeGeofenceCollectionResponseTypeDef",
     "DescribeKeyRequestRequestTypeDef",
     "DescribeMapRequestRequestTypeDef",
+    "MapConfigurationOutputTypeDef",
     "DescribePlaceIndexRequestRequestTypeDef",
     "DescribeRouteCalculatorRequestRequestTypeDef",
     "DescribeRouteCalculatorResponseTypeDef",
     "DescribeTrackerRequestRequestTypeDef",
     "DescribeTrackerResponseTypeDef",
+    "PositionalAccuracyOutputTypeDef",
     "PositionalAccuracyTypeDef",
     "DisassociateTrackerConsumerRequestRequestTypeDef",
     "GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
     "GetDevicePositionHistoryRequestRequestTypeDef",
     "GetDevicePositionRequestRequestTypeDef",
     "GetGeofenceRequestRequestTypeDef",
     "GetMapGlyphsRequestRequestTypeDef",
@@ -140,35 +145,36 @@
     "UpdatePlaceIndexResponseTypeDef",
     "UpdateRouteCalculatorRequestRequestTypeDef",
     "UpdateRouteCalculatorResponseTypeDef",
     "UpdateTrackerRequestRequestTypeDef",
     "UpdateTrackerResponseTypeDef",
     "ListKeysRequestListKeysPaginateTypeDef",
     "ListKeysRequestRequestTypeDef",
-    "CreateKeyRequestRequestTypeDef",
     "DescribeKeyResponseTypeDef",
     "ListKeysResponseEntryTypeDef",
+    "CreateKeyRequestRequestTypeDef",
     "UpdateKeyRequestRequestTypeDef",
     "BatchDeleteDevicePositionHistoryErrorTypeDef",
     "BatchDeleteGeofenceErrorTypeDef",
     "BatchEvaluateGeofencesErrorTypeDef",
     "BatchGetDevicePositionErrorTypeDef",
     "BatchPutGeofenceErrorTypeDef",
     "BatchUpdateDevicePositionErrorTypeDef",
     "CalculateRouteTruckModeOptionsTypeDef",
+    "GeofenceGeometryOutputTypeDef",
     "GeofenceGeometryTypeDef",
     "CreateMapRequestRequestTypeDef",
-    "DescribeMapResponseTypeDef",
     "CreatePlaceIndexRequestRequestTypeDef",
-    "DescribePlaceIndexResponseTypeDef",
     "UpdatePlaceIndexRequestRequestTypeDef",
+    "DescribePlaceIndexResponseTypeDef",
+    "DescribeMapResponseTypeDef",
     "DevicePositionTypeDef",
-    "DevicePositionUpdateTypeDef",
     "GetDevicePositionResponseTypeDef",
     "ListDevicePositionsResponseEntryTypeDef",
+    "DevicePositionUpdateTypeDef",
     "LegTypeDef",
     "ListGeofenceCollectionsResponseTypeDef",
     "ListMapsResponseTypeDef",
     "ListPlaceIndexesResponseTypeDef",
     "ListRouteCalculatorsResponseTypeDef",
     "ListTrackersResponseTypeDef",
     "UpdateMapRequestRequestTypeDef",
@@ -179,42 +185,62 @@
     "BatchDeleteDevicePositionHistoryResponseTypeDef",
     "BatchDeleteGeofenceResponseTypeDef",
     "BatchEvaluateGeofencesResponseTypeDef",
     "BatchPutGeofenceResponseTypeDef",
     "BatchUpdateDevicePositionResponseTypeDef",
     "CalculateRouteMatrixRequestRequestTypeDef",
     "CalculateRouteRequestRequestTypeDef",
-    "BatchPutGeofenceRequestEntryTypeDef",
     "GetGeofenceResponseTypeDef",
     "ListGeofenceResponseEntryTypeDef",
+    "BatchPutGeofenceRequestEntryTypeDef",
     "PutGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionResponseTypeDef",
     "GetDevicePositionHistoryResponseTypeDef",
+    "ListDevicePositionsResponseTypeDef",
     "BatchEvaluateGeofencesRequestRequestTypeDef",
     "BatchUpdateDevicePositionRequestRequestTypeDef",
-    "ListDevicePositionsResponseTypeDef",
     "CalculateRouteResponseTypeDef",
     "GetPlaceResponseTypeDef",
     "SearchForPositionResultTypeDef",
     "SearchForTextResultTypeDef",
     "CalculateRouteMatrixResponseTypeDef",
-    "BatchPutGeofenceRequestRequestTypeDef",
     "ListGeofencesResponseTypeDef",
+    "BatchPutGeofenceRequestRequestTypeDef",
     "SearchPlaceIndexForPositionResponseTypeDef",
     "SearchPlaceIndexForTextResponseTypeDef",
 )
 
 ApiKeyFilterTypeDef = TypedDict(
     "ApiKeyFilterTypeDef",
     {
         "KeyStatus": StatusType,
     },
     total=False,
 )
 
+_RequiredApiKeyRestrictionsOutputTypeDef = TypedDict(
+    "_RequiredApiKeyRestrictionsOutputTypeDef",
+    {
+        "AllowActions": List[str],
+        "AllowResources": List[str],
+    },
+)
+_OptionalApiKeyRestrictionsOutputTypeDef = TypedDict(
+    "_OptionalApiKeyRestrictionsOutputTypeDef",
+    {
+        "AllowReferers": List[str],
+    },
+    total=False,
+)
+
+class ApiKeyRestrictionsOutputTypeDef(
+    _RequiredApiKeyRestrictionsOutputTypeDef, _OptionalApiKeyRestrictionsOutputTypeDef
+):
+    pass
+
 _RequiredApiKeyRestrictionsTypeDef = TypedDict(
     "_RequiredApiKeyRestrictionsTypeDef",
     {
         "AllowActions": Sequence[str],
         "AllowResources": Sequence[str],
     },
 )
@@ -327,14 +353,22 @@
     {
         "Total": float,
         "Unit": VehicleWeightUnitType,
     },
     total=False,
 )
 
+CircleOutputTypeDef = TypedDict(
+    "CircleOutputTypeDef",
+    {
+        "Center": List[float],
+        "Radius": float,
+    },
+)
+
 CircleTypeDef = TypedDict(
     "CircleTypeDef",
     {
         "Center": Sequence[float],
         "Radius": float,
     },
 )
@@ -493,14 +527,22 @@
         "CreateTime": datetime,
         "TrackerArn": str,
         "TrackerName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DataSourceConfigurationOutputTypeDef = TypedDict(
+    "DataSourceConfigurationOutputTypeDef",
+    {
+        "IntendedUse": IntendedUseType,
+    },
+    total=False,
+)
+
 DeleteGeofenceCollectionRequestRequestTypeDef = TypedDict(
     "DeleteGeofenceCollectionRequestRequestTypeDef",
     {
         "CollectionName": str,
     },
 )
 
@@ -572,14 +614,33 @@
 DescribeMapRequestRequestTypeDef = TypedDict(
     "DescribeMapRequestRequestTypeDef",
     {
         "MapName": str,
     },
 )
 
+_RequiredMapConfigurationOutputTypeDef = TypedDict(
+    "_RequiredMapConfigurationOutputTypeDef",
+    {
+        "Style": str,
+    },
+)
+_OptionalMapConfigurationOutputTypeDef = TypedDict(
+    "_OptionalMapConfigurationOutputTypeDef",
+    {
+        "PoliticalView": str,
+    },
+    total=False,
+)
+
+class MapConfigurationOutputTypeDef(
+    _RequiredMapConfigurationOutputTypeDef, _OptionalMapConfigurationOutputTypeDef
+):
+    pass
+
 DescribePlaceIndexRequestRequestTypeDef = TypedDict(
     "DescribePlaceIndexRequestRequestTypeDef",
     {
         "IndexName": str,
     },
 )
 
@@ -626,14 +687,21 @@
         "TrackerArn": str,
         "TrackerName": str,
         "UpdateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PositionalAccuracyOutputTypeDef = TypedDict(
+    "PositionalAccuracyOutputTypeDef",
+    {
+        "Horizontal": float,
+    },
+)
+
 PositionalAccuracyTypeDef = TypedDict(
     "PositionalAccuracyTypeDef",
     {
         "Horizontal": float,
     },
 )
 
@@ -1640,60 +1708,37 @@
         "Filter": ApiKeyFilterTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredCreateKeyRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKeyRequestRequestTypeDef",
-    {
-        "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsTypeDef,
-    },
-)
-_OptionalCreateKeyRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKeyRequestRequestTypeDef",
-    {
-        "Description": str,
-        "ExpireTime": Union[datetime, str],
-        "NoExpiry": bool,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateKeyRequestRequestTypeDef(
-    _RequiredCreateKeyRequestRequestTypeDef, _OptionalCreateKeyRequestRequestTypeDef
-):
-    pass
-
 DescribeKeyResponseTypeDef = TypedDict(
     "DescribeKeyResponseTypeDef",
     {
         "CreateTime": datetime,
         "Description": str,
         "ExpireTime": datetime,
         "Key": str,
         "KeyArn": str,
         "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsTypeDef,
+        "Restrictions": ApiKeyRestrictionsOutputTypeDef,
         "Tags": Dict[str, str],
         "UpdateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListKeysResponseEntryTypeDef = TypedDict(
     "_RequiredListKeysResponseEntryTypeDef",
     {
         "CreateTime": datetime,
         "ExpireTime": datetime,
         "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsTypeDef,
+        "Restrictions": ApiKeyRestrictionsOutputTypeDef,
         "UpdateTime": datetime,
     },
 )
 _OptionalListKeysResponseEntryTypeDef = TypedDict(
     "_OptionalListKeysResponseEntryTypeDef",
     {
         "Description": str,
@@ -1702,14 +1747,37 @@
 )
 
 class ListKeysResponseEntryTypeDef(
     _RequiredListKeysResponseEntryTypeDef, _OptionalListKeysResponseEntryTypeDef
 ):
     pass
 
+_RequiredCreateKeyRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKeyRequestRequestTypeDef",
+    {
+        "KeyName": str,
+        "Restrictions": ApiKeyRestrictionsTypeDef,
+    },
+)
+_OptionalCreateKeyRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKeyRequestRequestTypeDef",
+    {
+        "Description": str,
+        "ExpireTime": Union[datetime, str],
+        "NoExpiry": bool,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateKeyRequestRequestTypeDef(
+    _RequiredCreateKeyRequestRequestTypeDef, _OptionalCreateKeyRequestRequestTypeDef
+):
+    pass
+
 _RequiredUpdateKeyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKeyRequestRequestTypeDef",
     {
         "KeyName": str,
     },
 )
 _OptionalUpdateKeyRequestRequestTypeDef = TypedDict(
@@ -1786,14 +1854,23 @@
         "AvoidTolls": bool,
         "Dimensions": TruckDimensionsTypeDef,
         "Weight": TruckWeightTypeDef,
     },
     total=False,
 )
 
+GeofenceGeometryOutputTypeDef = TypedDict(
+    "GeofenceGeometryOutputTypeDef",
+    {
+        "Circle": CircleOutputTypeDef,
+        "Polygon": List[List[List[float]]],
+    },
+    total=False,
+)
+
 GeofenceGeometryTypeDef = TypedDict(
     "GeofenceGeometryTypeDef",
     {
         "Circle": CircleTypeDef,
         "Polygon": Sequence[Sequence[Sequence[float]]],
     },
     total=False,
@@ -1817,30 +1894,14 @@
 )
 
 class CreateMapRequestRequestTypeDef(
     _RequiredCreateMapRequestRequestTypeDef, _OptionalCreateMapRequestRequestTypeDef
 ):
     pass
 
-DescribeMapResponseTypeDef = TypedDict(
-    "DescribeMapResponseTypeDef",
-    {
-        "Configuration": MapConfigurationTypeDef,
-        "CreateTime": datetime,
-        "DataSource": str,
-        "Description": str,
-        "MapArn": str,
-        "MapName": str,
-        "PricingPlan": PricingPlanType,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePlaceIndexRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePlaceIndexRequestRequestTypeDef",
     {
         "DataSource": str,
         "IndexName": str,
     },
 )
@@ -1856,30 +1917,14 @@
 )
 
 class CreatePlaceIndexRequestRequestTypeDef(
     _RequiredCreatePlaceIndexRequestRequestTypeDef, _OptionalCreatePlaceIndexRequestRequestTypeDef
 ):
     pass
 
-DescribePlaceIndexResponseTypeDef = TypedDict(
-    "DescribePlaceIndexResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "DataSource": str,
-        "DataSourceConfiguration": DataSourceConfigurationTypeDef,
-        "Description": str,
-        "IndexArn": str,
-        "IndexName": str,
-        "PricingPlan": PricingPlanType,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePlaceIndexRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePlaceIndexRequestRequestTypeDef",
     {
         "IndexName": str,
     },
 )
 _OptionalUpdatePlaceIndexRequestRequestTypeDef = TypedDict(
@@ -1893,61 +1938,71 @@
 )
 
 class UpdatePlaceIndexRequestRequestTypeDef(
     _RequiredUpdatePlaceIndexRequestRequestTypeDef, _OptionalUpdatePlaceIndexRequestRequestTypeDef
 ):
     pass
 
+DescribePlaceIndexResponseTypeDef = TypedDict(
+    "DescribePlaceIndexResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "DataSource": str,
+        "DataSourceConfiguration": DataSourceConfigurationOutputTypeDef,
+        "Description": str,
+        "IndexArn": str,
+        "IndexName": str,
+        "PricingPlan": PricingPlanType,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeMapResponseTypeDef = TypedDict(
+    "DescribeMapResponseTypeDef",
+    {
+        "Configuration": MapConfigurationOutputTypeDef,
+        "CreateTime": datetime,
+        "DataSource": str,
+        "Description": str,
+        "MapArn": str,
+        "MapName": str,
+        "PricingPlan": PricingPlanType,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDevicePositionTypeDef = TypedDict(
     "_RequiredDevicePositionTypeDef",
     {
         "Position": List[float],
         "ReceivedTime": datetime,
         "SampleTime": datetime,
     },
 )
 _OptionalDevicePositionTypeDef = TypedDict(
     "_OptionalDevicePositionTypeDef",
     {
-        "Accuracy": PositionalAccuracyTypeDef,
+        "Accuracy": PositionalAccuracyOutputTypeDef,
         "DeviceId": str,
         "PositionProperties": Dict[str, str],
     },
     total=False,
 )
 
 class DevicePositionTypeDef(_RequiredDevicePositionTypeDef, _OptionalDevicePositionTypeDef):
     pass
 
-_RequiredDevicePositionUpdateTypeDef = TypedDict(
-    "_RequiredDevicePositionUpdateTypeDef",
-    {
-        "DeviceId": str,
-        "Position": Sequence[float],
-        "SampleTime": Union[datetime, str],
-    },
-)
-_OptionalDevicePositionUpdateTypeDef = TypedDict(
-    "_OptionalDevicePositionUpdateTypeDef",
-    {
-        "Accuracy": PositionalAccuracyTypeDef,
-        "PositionProperties": Mapping[str, str],
-    },
-    total=False,
-)
-
-class DevicePositionUpdateTypeDef(
-    _RequiredDevicePositionUpdateTypeDef, _OptionalDevicePositionUpdateTypeDef
-):
-    pass
-
 GetDevicePositionResponseTypeDef = TypedDict(
     "GetDevicePositionResponseTypeDef",
     {
-        "Accuracy": PositionalAccuracyTypeDef,
+        "Accuracy": PositionalAccuracyOutputTypeDef,
         "DeviceId": str,
         "Position": List[float],
         "PositionProperties": Dict[str, str],
         "ReceivedTime": datetime,
         "SampleTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1960,26 +2015,48 @@
         "Position": List[float],
         "SampleTime": datetime,
     },
 )
 _OptionalListDevicePositionsResponseEntryTypeDef = TypedDict(
     "_OptionalListDevicePositionsResponseEntryTypeDef",
     {
-        "Accuracy": PositionalAccuracyTypeDef,
+        "Accuracy": PositionalAccuracyOutputTypeDef,
         "PositionProperties": Dict[str, str],
     },
     total=False,
 )
 
 class ListDevicePositionsResponseEntryTypeDef(
     _RequiredListDevicePositionsResponseEntryTypeDef,
     _OptionalListDevicePositionsResponseEntryTypeDef,
 ):
     pass
 
+_RequiredDevicePositionUpdateTypeDef = TypedDict(
+    "_RequiredDevicePositionUpdateTypeDef",
+    {
+        "DeviceId": str,
+        "Position": Sequence[float],
+        "SampleTime": Union[datetime, str],
+    },
+)
+_OptionalDevicePositionUpdateTypeDef = TypedDict(
+    "_OptionalDevicePositionUpdateTypeDef",
+    {
+        "Accuracy": PositionalAccuracyTypeDef,
+        "PositionProperties": Mapping[str, str],
+    },
+    total=False,
+)
+
+class DevicePositionUpdateTypeDef(
+    _RequiredDevicePositionUpdateTypeDef, _OptionalDevicePositionUpdateTypeDef
+):
+    pass
+
 _RequiredLegTypeDef = TypedDict(
     "_RequiredLegTypeDef",
     {
         "Distance": float,
         "DurationSeconds": float,
         "EndPosition": List[float],
         "StartPosition": List[float],
@@ -2216,53 +2293,33 @@
 )
 
 class CalculateRouteRequestRequestTypeDef(
     _RequiredCalculateRouteRequestRequestTypeDef, _OptionalCalculateRouteRequestRequestTypeDef
 ):
     pass
 
-_RequiredBatchPutGeofenceRequestEntryTypeDef = TypedDict(
-    "_RequiredBatchPutGeofenceRequestEntryTypeDef",
-    {
-        "GeofenceId": str,
-        "Geometry": GeofenceGeometryTypeDef,
-    },
-)
-_OptionalBatchPutGeofenceRequestEntryTypeDef = TypedDict(
-    "_OptionalBatchPutGeofenceRequestEntryTypeDef",
-    {
-        "GeofenceProperties": Mapping[str, str],
-    },
-    total=False,
-)
-
-class BatchPutGeofenceRequestEntryTypeDef(
-    _RequiredBatchPutGeofenceRequestEntryTypeDef, _OptionalBatchPutGeofenceRequestEntryTypeDef
-):
-    pass
-
 GetGeofenceResponseTypeDef = TypedDict(
     "GetGeofenceResponseTypeDef",
     {
         "CreateTime": datetime,
         "GeofenceId": str,
         "GeofenceProperties": Dict[str, str],
-        "Geometry": GeofenceGeometryTypeDef,
+        "Geometry": GeofenceGeometryOutputTypeDef,
         "Status": str,
         "UpdateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListGeofenceResponseEntryTypeDef = TypedDict(
     "_RequiredListGeofenceResponseEntryTypeDef",
     {
         "CreateTime": datetime,
         "GeofenceId": str,
-        "Geometry": GeofenceGeometryTypeDef,
+        "Geometry": GeofenceGeometryOutputTypeDef,
         "Status": str,
         "UpdateTime": datetime,
     },
 )
 _OptionalListGeofenceResponseEntryTypeDef = TypedDict(
     "_OptionalListGeofenceResponseEntryTypeDef",
     {
@@ -2272,14 +2329,34 @@
 )
 
 class ListGeofenceResponseEntryTypeDef(
     _RequiredListGeofenceResponseEntryTypeDef, _OptionalListGeofenceResponseEntryTypeDef
 ):
     pass
 
+_RequiredBatchPutGeofenceRequestEntryTypeDef = TypedDict(
+    "_RequiredBatchPutGeofenceRequestEntryTypeDef",
+    {
+        "GeofenceId": str,
+        "Geometry": GeofenceGeometryTypeDef,
+    },
+)
+_OptionalBatchPutGeofenceRequestEntryTypeDef = TypedDict(
+    "_OptionalBatchPutGeofenceRequestEntryTypeDef",
+    {
+        "GeofenceProperties": Mapping[str, str],
+    },
+    total=False,
+)
+
+class BatchPutGeofenceRequestEntryTypeDef(
+    _RequiredBatchPutGeofenceRequestEntryTypeDef, _OptionalBatchPutGeofenceRequestEntryTypeDef
+):
+    pass
+
 _RequiredPutGeofenceRequestRequestTypeDef = TypedDict(
     "_RequiredPutGeofenceRequestRequestTypeDef",
     {
         "CollectionName": str,
         "GeofenceId": str,
         "Geometry": GeofenceGeometryTypeDef,
     },
@@ -2311,14 +2388,23 @@
     {
         "DevicePositions": List[DevicePositionTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListDevicePositionsResponseTypeDef = TypedDict(
+    "ListDevicePositionsResponseTypeDef",
+    {
+        "Entries": List[ListDevicePositionsResponseEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BatchEvaluateGeofencesRequestRequestTypeDef = TypedDict(
     "BatchEvaluateGeofencesRequestRequestTypeDef",
     {
         "CollectionName": str,
         "DevicePositionUpdates": Sequence[DevicePositionUpdateTypeDef],
     },
 )
@@ -2327,23 +2413,14 @@
     "BatchUpdateDevicePositionRequestRequestTypeDef",
     {
         "TrackerName": str,
         "Updates": Sequence[DevicePositionUpdateTypeDef],
     },
 )
 
-ListDevicePositionsResponseTypeDef = TypedDict(
-    "ListDevicePositionsResponseTypeDef",
-    {
-        "Entries": List[ListDevicePositionsResponseEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CalculateRouteResponseTypeDef = TypedDict(
     "CalculateRouteResponseTypeDef",
     {
         "Legs": List[LegTypeDef],
         "Summary": CalculateRouteSummaryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2405,31 +2482,31 @@
         "SnappedDeparturePositions": List[List[float]],
         "SnappedDestinationPositions": List[List[float]],
         "Summary": CalculateRouteMatrixSummaryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-BatchPutGeofenceRequestRequestTypeDef = TypedDict(
-    "BatchPutGeofenceRequestRequestTypeDef",
-    {
-        "CollectionName": str,
-        "Entries": Sequence[BatchPutGeofenceRequestEntryTypeDef],
-    },
-)
-
 ListGeofencesResponseTypeDef = TypedDict(
     "ListGeofencesResponseTypeDef",
     {
         "Entries": List[ListGeofenceResponseEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+BatchPutGeofenceRequestRequestTypeDef = TypedDict(
+    "BatchPutGeofenceRequestRequestTypeDef",
+    {
+        "CollectionName": str,
+        "Entries": Sequence[BatchPutGeofenceRequestEntryTypeDef],
+    },
+)
+
 SearchPlaceIndexForPositionResponseTypeDef = TypedDict(
     "SearchPlaceIndexForPositionResponseTypeDef",
     {
         "Results": List[SearchForPositionResultTypeDef],
         "Summary": SearchPlaceIndexForPositionSummaryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-location-1.28.0/mypy_boto3_location.egg-info/PKG-INFO` & `mypy-boto3-location-1.28.12/mypy_boto3_location.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-location
-Version: 1.28.0
-Summary: Type annotations for boto3.LocationService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.LocationService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-location"></a>
 
 # mypy-boto3-location
 
 [![PyPI - mypy-boto3-location](https://img.shields.io/pypi/v/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-location?color=blue)](https://pypistats.org/packages/mypy-boto3-location)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-location)](https://pepy.tech/project/mypy-boto3-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LocationService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[boto3.LocationService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
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
 [mypy-boto3-location docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,53 +368,58 @@
 
 `mypy_boto3_location.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_location.type_defs import (
     ApiKeyFilterTypeDef,
+    ApiKeyRestrictionsOutputTypeDef,
     ApiKeyRestrictionsTypeDef,
     AssociateTrackerConsumerRequestRequestTypeDef,
     BatchItemErrorTypeDef,
     BatchDeleteDevicePositionHistoryRequestRequestTypeDef,
     BatchDeleteGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionRequestRequestTypeDef,
     BatchPutGeofenceSuccessTypeDef,
     CalculateRouteCarModeOptionsTypeDef,
     CalculateRouteMatrixSummaryTypeDef,
     CalculateRouteSummaryTypeDef,
     TruckDimensionsTypeDef,
     TruckWeightTypeDef,
+    CircleOutputTypeDef,
     CircleTypeDef,
     CreateGeofenceCollectionRequestRequestTypeDef,
     CreateGeofenceCollectionResponseTypeDef,
     CreateKeyResponseTypeDef,
     MapConfigurationTypeDef,
     CreateMapResponseTypeDef,
     DataSourceConfigurationTypeDef,
     CreatePlaceIndexResponseTypeDef,
     CreateRouteCalculatorRequestRequestTypeDef,
     CreateRouteCalculatorResponseTypeDef,
     CreateTrackerRequestRequestTypeDef,
     CreateTrackerResponseTypeDef,
+    DataSourceConfigurationOutputTypeDef,
     DeleteGeofenceCollectionRequestRequestTypeDef,
     DeleteKeyRequestRequestTypeDef,
     DeleteMapRequestRequestTypeDef,
     DeletePlaceIndexRequestRequestTypeDef,
     DeleteRouteCalculatorRequestRequestTypeDef,
     DeleteTrackerRequestRequestTypeDef,
     DescribeGeofenceCollectionRequestRequestTypeDef,
     DescribeGeofenceCollectionResponseTypeDef,
     DescribeKeyRequestRequestTypeDef,
     DescribeMapRequestRequestTypeDef,
+    MapConfigurationOutputTypeDef,
     DescribePlaceIndexRequestRequestTypeDef,
     DescribeRouteCalculatorRequestRequestTypeDef,
     DescribeRouteCalculatorResponseTypeDef,
     DescribeTrackerRequestRequestTypeDef,
     DescribeTrackerResponseTypeDef,
+    PositionalAccuracyOutputTypeDef,
     PositionalAccuracyTypeDef,
     DisassociateTrackerConsumerRequestRequestTypeDef,
     GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
     GetDevicePositionHistoryRequestRequestTypeDef,
     GetDevicePositionRequestRequestTypeDef,
     GetGeofenceRequestRequestTypeDef,
     GetMapGlyphsRequestRequestTypeDef,
@@ -475,35 +480,36 @@
     UpdatePlaceIndexResponseTypeDef,
     UpdateRouteCalculatorRequestRequestTypeDef,
     UpdateRouteCalculatorResponseTypeDef,
     UpdateTrackerRequestRequestTypeDef,
     UpdateTrackerResponseTypeDef,
     ListKeysRequestListKeysPaginateTypeDef,
     ListKeysRequestRequestTypeDef,
-    CreateKeyRequestRequestTypeDef,
     DescribeKeyResponseTypeDef,
     ListKeysResponseEntryTypeDef,
+    CreateKeyRequestRequestTypeDef,
     UpdateKeyRequestRequestTypeDef,
     BatchDeleteDevicePositionHistoryErrorTypeDef,
     BatchDeleteGeofenceErrorTypeDef,
     BatchEvaluateGeofencesErrorTypeDef,
     BatchGetDevicePositionErrorTypeDef,
     BatchPutGeofenceErrorTypeDef,
     BatchUpdateDevicePositionErrorTypeDef,
     CalculateRouteTruckModeOptionsTypeDef,
+    GeofenceGeometryOutputTypeDef,
     GeofenceGeometryTypeDef,
     CreateMapRequestRequestTypeDef,
-    DescribeMapResponseTypeDef,
     CreatePlaceIndexRequestRequestTypeDef,
-    DescribePlaceIndexResponseTypeDef,
     UpdatePlaceIndexRequestRequestTypeDef,
+    DescribePlaceIndexResponseTypeDef,
+    DescribeMapResponseTypeDef,
     DevicePositionTypeDef,
-    DevicePositionUpdateTypeDef,
     GetDevicePositionResponseTypeDef,
     ListDevicePositionsResponseEntryTypeDef,
+    DevicePositionUpdateTypeDef,
     LegTypeDef,
     ListGeofenceCollectionsResponseTypeDef,
     ListMapsResponseTypeDef,
     ListPlaceIndexesResponseTypeDef,
     ListRouteCalculatorsResponseTypeDef,
     ListTrackersResponseTypeDef,
     UpdateMapRequestRequestTypeDef,
@@ -514,30 +520,30 @@
     BatchDeleteDevicePositionHistoryResponseTypeDef,
     BatchDeleteGeofenceResponseTypeDef,
     BatchEvaluateGeofencesResponseTypeDef,
     BatchPutGeofenceResponseTypeDef,
     BatchUpdateDevicePositionResponseTypeDef,
     CalculateRouteMatrixRequestRequestTypeDef,
     CalculateRouteRequestRequestTypeDef,
-    BatchPutGeofenceRequestEntryTypeDef,
     GetGeofenceResponseTypeDef,
     ListGeofenceResponseEntryTypeDef,
+    BatchPutGeofenceRequestEntryTypeDef,
     PutGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionResponseTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
+    ListDevicePositionsResponseTypeDef,
     BatchEvaluateGeofencesRequestRequestTypeDef,
     BatchUpdateDevicePositionRequestRequestTypeDef,
-    ListDevicePositionsResponseTypeDef,
     CalculateRouteResponseTypeDef,
     GetPlaceResponseTypeDef,
     SearchForPositionResultTypeDef,
     SearchForTextResultTypeDef,
     CalculateRouteMatrixResponseTypeDef,
-    BatchPutGeofenceRequestRequestTypeDef,
     ListGeofencesResponseTypeDef,
+    BatchPutGeofenceRequestRequestTypeDef,
     SearchPlaceIndexForPositionResponseTypeDef,
     SearchPlaceIndexForTextResponseTypeDef,
 )
 
 
 def get_structure() -> ApiKeyFilterTypeDef:
     return {...}
```

### Comparing `mypy-boto3-location-1.28.0/mypy_boto3_location.egg-info/SOURCES.txt` & `mypy-boto3-location-1.28.12/mypy_boto3_location.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.0/setup.py` & `mypy-boto3-location-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-location",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_location"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LocationService 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.LocationService 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

