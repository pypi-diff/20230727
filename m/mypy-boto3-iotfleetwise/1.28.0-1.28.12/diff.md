# Comparing `tmp/mypy-boto3-iotfleetwise-1.28.0.tar.gz` & `tmp/mypy-boto3-iotfleetwise-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotfleetwise-1.28.0.tar", last modified: Thu Jul  6 20:59:48 2023, max compression
+gzip compressed data, was "mypy-boto3-iotfleetwise-1.28.12.tar", last modified: Thu Jul 27 05:34:49 2023, max compression
```

## Comparing `mypy-boto3-iotfleetwise-1.28.0.tar` & `mypy-boto3-iotfleetwise-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:48.810332 mypy-boto3-iotfleetwise-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:43:51.000000 mypy-boto3-iotfleetwise-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21420 2023-07-06 20:59:48.806331 mypy-boto3-iotfleetwise-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19915 2023-07-06 20:43:51.000000 mypy-boto3-iotfleetwise-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:48.794332 mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-06 20:43:51.000000 mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-06 20:43:51.000000 mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:43:51.000000 mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40870 2023-07-06 20:43:51.000000 mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40800 2023-07-06 20:43:51.000000 mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-07-06 20:43:52.000000 mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-07-06 20:43:52.000000 mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15514 2023-07-06 20:43:51.000000 mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-07-06 20:43:51.000000 mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:43:51.000000 mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    58188 2023-07-06 20:43:53.000000 mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    58088 2023-07-06 20:43:53.000000 mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:43:51.000000 mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:48.806331 mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21420 2023-07-06 20:59:48.000000 mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 20:59:48.000000 mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:48.000000 mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:48.000000 mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:48.000000 mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 20:59:48.000000 mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:48.810332 mypy-boto3-iotfleetwise-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:43:51.000000 mypy-boto3-iotfleetwise-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.928481 mypy-boto3-iotfleetwise-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:05.000000 mypy-boto3-iotfleetwise-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22130 2023-07-27 05:34:49.920481 mypy-boto3-iotfleetwise-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20623 2023-07-27 05:24:05.000000 mypy-boto3-iotfleetwise-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.920481 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-27 05:24:05.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-27 05:24:05.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:24:05.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40870 2023-07-27 05:24:07.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40800 2023-07-27 05:24:05.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-07-27 05:24:07.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-07-27 05:24:07.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15514 2023-07-27 05:24:07.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-07-27 05:24:07.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:05.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    68052 2023-07-27 05:24:08.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67924 2023-07-27 05:24:08.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:05.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.920481 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22130 2023-07-27 05:34:49.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:34:49.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:49.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:49.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:49.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:49.000000 mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:49.928481 mypy-boto3-iotfleetwise-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:24:05.000000 mypy-boto3-iotfleetwise-1.28.12/setup.py
```

### Comparing `mypy-boto3-iotfleetwise-1.28.0/LICENSE` & `mypy-boto3-iotfleetwise-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.0/PKG-INFO` & `mypy-boto3-iotfleetwise-1.28.12/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotfleetwise
-Version: 1.28.0
-Summary: Type annotations for boto3.IoTFleetWise 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTFleetWise 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iotfleetwise"></a>
 
 # mypy-boto3-iotfleetwise
 
 [![PyPI - mypy-boto3-iotfleetwise](https://img.shields.io/pypi/v/mypy-boto3-iotfleetwise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleetwise)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleetwise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotfleetwise?color=blue)](https://pypistats.org/packages/mypy-boto3-iotfleetwise)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotfleetwise)](https://pepy.tech/project/mypy-boto3-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetWise 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
+[boto3.IoTFleetWise 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
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
 [mypy-boto3-iotfleetwise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/).
 
 See how it helps to find and fix potential bugs:
 
@@ -392,38 +392,48 @@
 ### Typed dictionaries
 
 `mypy_boto3_iotfleetwise.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotfleetwise.type_defs import (
+    ActuatorOutputTypeDef,
     ActuatorTypeDef,
     AssociateVehicleFleetRequestRequestTypeDef,
+    AttributeOutputTypeDef,
     AttributeTypeDef,
     CreateVehicleErrorTypeDef,
     CreateVehicleResponseItemTypeDef,
     UpdateVehicleRequestItemTypeDef,
     UpdateVehicleErrorTypeDef,
     UpdateVehicleResponseItemTypeDef,
+    BranchOutputTypeDef,
     BranchTypeDef,
     CampaignSummaryTypeDef,
     CanDbcDefinitionTypeDef,
+    CanInterfaceOutputTypeDef,
     CanInterfaceTypeDef,
+    CanSignalOutputTypeDef,
     CanSignalTypeDef,
+    CloudWatchLogDeliveryOptionsOutputTypeDef,
     CloudWatchLogDeliveryOptionsTypeDef,
+    ConditionBasedCollectionSchemeOutputTypeDef,
+    TimeBasedCollectionSchemeOutputTypeDef,
     ConditionBasedCollectionSchemeTypeDef,
     TimeBasedCollectionSchemeTypeDef,
     SignalInformationTypeDef,
     TagTypeDef,
     CreateCampaignResponseTypeDef,
     CreateDecoderManifestResponseTypeDef,
     CreateFleetResponseTypeDef,
     CreateModelManifestResponseTypeDef,
     CreateSignalCatalogResponseTypeDef,
     CreateVehicleResponseTypeDef,
+    S3ConfigOutputTypeDef,
+    TimestreamConfigOutputTypeDef,
     S3ConfigTypeDef,
     TimestreamConfigTypeDef,
     DecoderManifestSummaryTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteCampaignResponseTypeDef,
     DeleteDecoderManifestRequestRequestTypeDef,
     DeleteDecoderManifestResponseTypeDef,
@@ -435,14 +445,15 @@
     DeleteSignalCatalogResponseTypeDef,
     DeleteVehicleRequestRequestTypeDef,
     DeleteVehicleResponseTypeDef,
     DisassociateVehicleFleetRequestRequestTypeDef,
     FleetSummaryTypeDef,
     FormattedVssTypeDef,
     GetCampaignRequestRequestTypeDef,
+    SignalInformationOutputTypeDef,
     GetDecoderManifestRequestRequestTypeDef,
     GetDecoderManifestResponseTypeDef,
     GetFleetRequestRequestTypeDef,
     GetFleetResponseTypeDef,
     GetModelManifestRequestRequestTypeDef,
     GetModelManifestResponseTypeDef,
     IamRegistrationResponseTypeDef,
@@ -450,14 +461,15 @@
     GetSignalCatalogRequestRequestTypeDef,
     NodeCountsTypeDef,
     GetVehicleRequestRequestTypeDef,
     GetVehicleResponseTypeDef,
     GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
     GetVehicleStatusRequestRequestTypeDef,
     VehicleStatusTypeDef,
+    IamResourcesOutputTypeDef,
     IamResourcesTypeDef,
     ImportDecoderManifestResponseTypeDef,
     ImportSignalCatalogResponseTypeDef,
     ListCampaignsRequestListCampaignsPaginateTypeDef,
     ListCampaignsRequestRequestTypeDef,
     ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
     ListDecoderManifestNetworkInterfacesRequestRequestTypeDef,
@@ -477,25 +489,30 @@
     ModelManifestSummaryTypeDef,
     ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
     ListSignalCatalogNodesRequestRequestTypeDef,
     ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef,
     ListSignalCatalogsRequestRequestTypeDef,
     SignalCatalogSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
     ListVehiclesInFleetRequestRequestTypeDef,
     ListVehiclesInFleetResponseTypeDef,
     ListVehiclesRequestListVehiclesPaginateTypeDef,
     ListVehiclesRequestRequestTypeDef,
     VehicleSummaryTypeDef,
+    ObdInterfaceOutputTypeDef,
     ObdInterfaceTypeDef,
+    SensorOutputTypeDef,
     SensorTypeDef,
+    ObdSignalOutputTypeDef,
     ObdSignalTypeDef,
     PaginatorConfigTypeDef,
     TimestreamResourcesTypeDef,
+    TimestreamResourcesOutputTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignRequestRequestTypeDef,
     UpdateCampaignResponseTypeDef,
     UpdateDecoderManifestResponseTypeDef,
     UpdateFleetRequestRequestTypeDef,
     UpdateFleetResponseTypeDef,
@@ -507,52 +524,57 @@
     BatchCreateVehicleResponseTypeDef,
     BatchUpdateVehicleRequestRequestTypeDef,
     BatchUpdateVehicleResponseTypeDef,
     ListCampaignsResponseTypeDef,
     NetworkFileDefinitionTypeDef,
     GetLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
+    CollectionSchemeOutputTypeDef,
     CollectionSchemeTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateModelManifestRequestRequestTypeDef,
     CreateVehicleRequestItemTypeDef,
     CreateVehicleRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    DataDestinationConfigOutputTypeDef,
     DataDestinationConfigTypeDef,
     ListDecoderManifestsResponseTypeDef,
     ListFleetsResponseTypeDef,
     ImportSignalCatalogRequestRequestTypeDef,
     GetRegisterAccountStatusResponseTypeDef,
     GetSignalCatalogResponseTypeDef,
     GetVehicleStatusResponseTypeDef,
     ListModelManifestsResponseTypeDef,
     ListSignalCatalogsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVehiclesResponseTypeDef,
+    NetworkInterfaceOutputTypeDef,
     NetworkInterfaceTypeDef,
+    NodeOutputTypeDef,
     NodeTypeDef,
+    SignalDecoderOutputTypeDef,
     SignalDecoderTypeDef,
     RegisterAccountRequestRequestTypeDef,
     RegisterAccountResponseTypeDef,
     ImportDecoderManifestRequestRequestTypeDef,
     BatchCreateVehicleRequestRequestTypeDef,
-    CreateCampaignRequestRequestTypeDef,
     GetCampaignResponseTypeDef,
+    CreateCampaignRequestRequestTypeDef,
     ListDecoderManifestNetworkInterfacesResponseTypeDef,
-    CreateSignalCatalogRequestRequestTypeDef,
     ListModelManifestNodesResponseTypeDef,
     ListSignalCatalogNodesResponseTypeDef,
+    CreateSignalCatalogRequestRequestTypeDef,
     UpdateSignalCatalogRequestRequestTypeDef,
-    CreateDecoderManifestRequestRequestTypeDef,
     ListDecoderManifestSignalsResponseTypeDef,
+    CreateDecoderManifestRequestRequestTypeDef,
     UpdateDecoderManifestRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActuatorTypeDef:
+def get_structure() -> ActuatorOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotfleetwise-1.28.0/README.md` & `mypy-boto3-iotfleetwise-1.28.12/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iotfleetwise"></a>
 
 # mypy-boto3-iotfleetwise
 
 [![PyPI - mypy-boto3-iotfleetwise](https://img.shields.io/pypi/v/mypy-boto3-iotfleetwise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleetwise)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleetwise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotfleetwise?color=blue)](https://pypistats.org/packages/mypy-boto3-iotfleetwise)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotfleetwise)](https://pepy.tech/project/mypy-boto3-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetWise 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
+[boto3.IoTFleetWise 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
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
 [mypy-boto3-iotfleetwise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/).
 
 See how it helps to find and fix potential bugs:
 
@@ -360,38 +360,48 @@
 ### Typed dictionaries
 
 `mypy_boto3_iotfleetwise.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotfleetwise.type_defs import (
+    ActuatorOutputTypeDef,
     ActuatorTypeDef,
     AssociateVehicleFleetRequestRequestTypeDef,
+    AttributeOutputTypeDef,
     AttributeTypeDef,
     CreateVehicleErrorTypeDef,
     CreateVehicleResponseItemTypeDef,
     UpdateVehicleRequestItemTypeDef,
     UpdateVehicleErrorTypeDef,
     UpdateVehicleResponseItemTypeDef,
+    BranchOutputTypeDef,
     BranchTypeDef,
     CampaignSummaryTypeDef,
     CanDbcDefinitionTypeDef,
+    CanInterfaceOutputTypeDef,
     CanInterfaceTypeDef,
+    CanSignalOutputTypeDef,
     CanSignalTypeDef,
+    CloudWatchLogDeliveryOptionsOutputTypeDef,
     CloudWatchLogDeliveryOptionsTypeDef,
+    ConditionBasedCollectionSchemeOutputTypeDef,
+    TimeBasedCollectionSchemeOutputTypeDef,
     ConditionBasedCollectionSchemeTypeDef,
     TimeBasedCollectionSchemeTypeDef,
     SignalInformationTypeDef,
     TagTypeDef,
     CreateCampaignResponseTypeDef,
     CreateDecoderManifestResponseTypeDef,
     CreateFleetResponseTypeDef,
     CreateModelManifestResponseTypeDef,
     CreateSignalCatalogResponseTypeDef,
     CreateVehicleResponseTypeDef,
+    S3ConfigOutputTypeDef,
+    TimestreamConfigOutputTypeDef,
     S3ConfigTypeDef,
     TimestreamConfigTypeDef,
     DecoderManifestSummaryTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteCampaignResponseTypeDef,
     DeleteDecoderManifestRequestRequestTypeDef,
     DeleteDecoderManifestResponseTypeDef,
@@ -403,14 +413,15 @@
     DeleteSignalCatalogResponseTypeDef,
     DeleteVehicleRequestRequestTypeDef,
     DeleteVehicleResponseTypeDef,
     DisassociateVehicleFleetRequestRequestTypeDef,
     FleetSummaryTypeDef,
     FormattedVssTypeDef,
     GetCampaignRequestRequestTypeDef,
+    SignalInformationOutputTypeDef,
     GetDecoderManifestRequestRequestTypeDef,
     GetDecoderManifestResponseTypeDef,
     GetFleetRequestRequestTypeDef,
     GetFleetResponseTypeDef,
     GetModelManifestRequestRequestTypeDef,
     GetModelManifestResponseTypeDef,
     IamRegistrationResponseTypeDef,
@@ -418,14 +429,15 @@
     GetSignalCatalogRequestRequestTypeDef,
     NodeCountsTypeDef,
     GetVehicleRequestRequestTypeDef,
     GetVehicleResponseTypeDef,
     GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
     GetVehicleStatusRequestRequestTypeDef,
     VehicleStatusTypeDef,
+    IamResourcesOutputTypeDef,
     IamResourcesTypeDef,
     ImportDecoderManifestResponseTypeDef,
     ImportSignalCatalogResponseTypeDef,
     ListCampaignsRequestListCampaignsPaginateTypeDef,
     ListCampaignsRequestRequestTypeDef,
     ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
     ListDecoderManifestNetworkInterfacesRequestRequestTypeDef,
@@ -445,25 +457,30 @@
     ModelManifestSummaryTypeDef,
     ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
     ListSignalCatalogNodesRequestRequestTypeDef,
     ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef,
     ListSignalCatalogsRequestRequestTypeDef,
     SignalCatalogSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
     ListVehiclesInFleetRequestRequestTypeDef,
     ListVehiclesInFleetResponseTypeDef,
     ListVehiclesRequestListVehiclesPaginateTypeDef,
     ListVehiclesRequestRequestTypeDef,
     VehicleSummaryTypeDef,
+    ObdInterfaceOutputTypeDef,
     ObdInterfaceTypeDef,
+    SensorOutputTypeDef,
     SensorTypeDef,
+    ObdSignalOutputTypeDef,
     ObdSignalTypeDef,
     PaginatorConfigTypeDef,
     TimestreamResourcesTypeDef,
+    TimestreamResourcesOutputTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignRequestRequestTypeDef,
     UpdateCampaignResponseTypeDef,
     UpdateDecoderManifestResponseTypeDef,
     UpdateFleetRequestRequestTypeDef,
     UpdateFleetResponseTypeDef,
@@ -475,52 +492,57 @@
     BatchCreateVehicleResponseTypeDef,
     BatchUpdateVehicleRequestRequestTypeDef,
     BatchUpdateVehicleResponseTypeDef,
     ListCampaignsResponseTypeDef,
     NetworkFileDefinitionTypeDef,
     GetLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
+    CollectionSchemeOutputTypeDef,
     CollectionSchemeTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateModelManifestRequestRequestTypeDef,
     CreateVehicleRequestItemTypeDef,
     CreateVehicleRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    DataDestinationConfigOutputTypeDef,
     DataDestinationConfigTypeDef,
     ListDecoderManifestsResponseTypeDef,
     ListFleetsResponseTypeDef,
     ImportSignalCatalogRequestRequestTypeDef,
     GetRegisterAccountStatusResponseTypeDef,
     GetSignalCatalogResponseTypeDef,
     GetVehicleStatusResponseTypeDef,
     ListModelManifestsResponseTypeDef,
     ListSignalCatalogsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVehiclesResponseTypeDef,
+    NetworkInterfaceOutputTypeDef,
     NetworkInterfaceTypeDef,
+    NodeOutputTypeDef,
     NodeTypeDef,
+    SignalDecoderOutputTypeDef,
     SignalDecoderTypeDef,
     RegisterAccountRequestRequestTypeDef,
     RegisterAccountResponseTypeDef,
     ImportDecoderManifestRequestRequestTypeDef,
     BatchCreateVehicleRequestRequestTypeDef,
-    CreateCampaignRequestRequestTypeDef,
     GetCampaignResponseTypeDef,
+    CreateCampaignRequestRequestTypeDef,
     ListDecoderManifestNetworkInterfacesResponseTypeDef,
-    CreateSignalCatalogRequestRequestTypeDef,
     ListModelManifestNodesResponseTypeDef,
     ListSignalCatalogNodesResponseTypeDef,
+    CreateSignalCatalogRequestRequestTypeDef,
     UpdateSignalCatalogRequestRequestTypeDef,
-    CreateDecoderManifestRequestRequestTypeDef,
     ListDecoderManifestSignalsResponseTypeDef,
+    CreateDecoderManifestRequestRequestTypeDef,
     UpdateDecoderManifestRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActuatorTypeDef:
+def get_structure() -> ActuatorOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/__init__.py` & `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/__init__.pyi` & `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/__main__.py` & `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTFleetWise 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.IoTFleetWise 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise\nOther"
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

### Comparing `mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/client.py` & `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/client.pyi` & `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/literals.py` & `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,14 +236,15 @@
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
@@ -322,26 +323,28 @@
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

### Comparing `mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/literals.pyi` & `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -234,14 +234,15 @@
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
@@ -320,26 +321,28 @@
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

### Comparing `mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/paginator.py` & `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/paginator.pyi` & `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/type_defs.py` & `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/type_defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iotfleetwise service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iotfleetwise.type_defs import ActuatorTypeDef
+    from mypy_boto3_iotfleetwise.type_defs import ActuatorOutputTypeDef
 
-    data: ActuatorTypeDef = {...}
+    data: ActuatorOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -40,38 +40,48 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "ActuatorOutputTypeDef",
     "ActuatorTypeDef",
     "AssociateVehicleFleetRequestRequestTypeDef",
+    "AttributeOutputTypeDef",
     "AttributeTypeDef",
     "CreateVehicleErrorTypeDef",
     "CreateVehicleResponseItemTypeDef",
     "UpdateVehicleRequestItemTypeDef",
     "UpdateVehicleErrorTypeDef",
     "UpdateVehicleResponseItemTypeDef",
+    "BranchOutputTypeDef",
     "BranchTypeDef",
     "CampaignSummaryTypeDef",
     "CanDbcDefinitionTypeDef",
+    "CanInterfaceOutputTypeDef",
     "CanInterfaceTypeDef",
+    "CanSignalOutputTypeDef",
     "CanSignalTypeDef",
+    "CloudWatchLogDeliveryOptionsOutputTypeDef",
     "CloudWatchLogDeliveryOptionsTypeDef",
+    "ConditionBasedCollectionSchemeOutputTypeDef",
+    "TimeBasedCollectionSchemeOutputTypeDef",
     "ConditionBasedCollectionSchemeTypeDef",
     "TimeBasedCollectionSchemeTypeDef",
     "SignalInformationTypeDef",
     "TagTypeDef",
     "CreateCampaignResponseTypeDef",
     "CreateDecoderManifestResponseTypeDef",
     "CreateFleetResponseTypeDef",
     "CreateModelManifestResponseTypeDef",
     "CreateSignalCatalogResponseTypeDef",
     "CreateVehicleResponseTypeDef",
+    "S3ConfigOutputTypeDef",
+    "TimestreamConfigOutputTypeDef",
     "S3ConfigTypeDef",
     "TimestreamConfigTypeDef",
     "DecoderManifestSummaryTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteCampaignResponseTypeDef",
     "DeleteDecoderManifestRequestRequestTypeDef",
     "DeleteDecoderManifestResponseTypeDef",
@@ -83,14 +93,15 @@
     "DeleteSignalCatalogResponseTypeDef",
     "DeleteVehicleRequestRequestTypeDef",
     "DeleteVehicleResponseTypeDef",
     "DisassociateVehicleFleetRequestRequestTypeDef",
     "FleetSummaryTypeDef",
     "FormattedVssTypeDef",
     "GetCampaignRequestRequestTypeDef",
+    "SignalInformationOutputTypeDef",
     "GetDecoderManifestRequestRequestTypeDef",
     "GetDecoderManifestResponseTypeDef",
     "GetFleetRequestRequestTypeDef",
     "GetFleetResponseTypeDef",
     "GetModelManifestRequestRequestTypeDef",
     "GetModelManifestResponseTypeDef",
     "IamRegistrationResponseTypeDef",
@@ -98,14 +109,15 @@
     "GetSignalCatalogRequestRequestTypeDef",
     "NodeCountsTypeDef",
     "GetVehicleRequestRequestTypeDef",
     "GetVehicleResponseTypeDef",
     "GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
     "GetVehicleStatusRequestRequestTypeDef",
     "VehicleStatusTypeDef",
+    "IamResourcesOutputTypeDef",
     "IamResourcesTypeDef",
     "ImportDecoderManifestResponseTypeDef",
     "ImportSignalCatalogResponseTypeDef",
     "ListCampaignsRequestListCampaignsPaginateTypeDef",
     "ListCampaignsRequestRequestTypeDef",
     "ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
     "ListDecoderManifestNetworkInterfacesRequestRequestTypeDef",
@@ -125,25 +137,30 @@
     "ModelManifestSummaryTypeDef",
     "ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
     "ListSignalCatalogNodesRequestRequestTypeDef",
     "ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef",
     "ListSignalCatalogsRequestRequestTypeDef",
     "SignalCatalogSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
     "ListVehiclesInFleetRequestRequestTypeDef",
     "ListVehiclesInFleetResponseTypeDef",
     "ListVehiclesRequestListVehiclesPaginateTypeDef",
     "ListVehiclesRequestRequestTypeDef",
     "VehicleSummaryTypeDef",
+    "ObdInterfaceOutputTypeDef",
     "ObdInterfaceTypeDef",
+    "SensorOutputTypeDef",
     "SensorTypeDef",
+    "ObdSignalOutputTypeDef",
     "ObdSignalTypeDef",
     "PaginatorConfigTypeDef",
     "TimestreamResourcesTypeDef",
+    "TimestreamResourcesOutputTypeDef",
     "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCampaignRequestRequestTypeDef",
     "UpdateCampaignResponseTypeDef",
     "UpdateDecoderManifestResponseTypeDef",
     "UpdateFleetRequestRequestTypeDef",
     "UpdateFleetResponseTypeDef",
@@ -155,50 +172,82 @@
     "BatchCreateVehicleResponseTypeDef",
     "BatchUpdateVehicleRequestRequestTypeDef",
     "BatchUpdateVehicleResponseTypeDef",
     "ListCampaignsResponseTypeDef",
     "NetworkFileDefinitionTypeDef",
     "GetLoggingOptionsResponseTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
+    "CollectionSchemeOutputTypeDef",
     "CollectionSchemeTypeDef",
     "CreateFleetRequestRequestTypeDef",
     "CreateModelManifestRequestRequestTypeDef",
     "CreateVehicleRequestItemTypeDef",
     "CreateVehicleRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "DataDestinationConfigOutputTypeDef",
     "DataDestinationConfigTypeDef",
     "ListDecoderManifestsResponseTypeDef",
     "ListFleetsResponseTypeDef",
     "ImportSignalCatalogRequestRequestTypeDef",
     "GetRegisterAccountStatusResponseTypeDef",
     "GetSignalCatalogResponseTypeDef",
     "GetVehicleStatusResponseTypeDef",
     "ListModelManifestsResponseTypeDef",
     "ListSignalCatalogsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListVehiclesResponseTypeDef",
+    "NetworkInterfaceOutputTypeDef",
     "NetworkInterfaceTypeDef",
+    "NodeOutputTypeDef",
     "NodeTypeDef",
+    "SignalDecoderOutputTypeDef",
     "SignalDecoderTypeDef",
     "RegisterAccountRequestRequestTypeDef",
     "RegisterAccountResponseTypeDef",
     "ImportDecoderManifestRequestRequestTypeDef",
     "BatchCreateVehicleRequestRequestTypeDef",
-    "CreateCampaignRequestRequestTypeDef",
     "GetCampaignResponseTypeDef",
+    "CreateCampaignRequestRequestTypeDef",
     "ListDecoderManifestNetworkInterfacesResponseTypeDef",
-    "CreateSignalCatalogRequestRequestTypeDef",
     "ListModelManifestNodesResponseTypeDef",
     "ListSignalCatalogNodesResponseTypeDef",
+    "CreateSignalCatalogRequestRequestTypeDef",
     "UpdateSignalCatalogRequestRequestTypeDef",
-    "CreateDecoderManifestRequestRequestTypeDef",
     "ListDecoderManifestSignalsResponseTypeDef",
+    "CreateDecoderManifestRequestRequestTypeDef",
     "UpdateDecoderManifestRequestRequestTypeDef",
 )
 
+_RequiredActuatorOutputTypeDef = TypedDict(
+    "_RequiredActuatorOutputTypeDef",
+    {
+        "fullyQualifiedName": str,
+        "dataType": NodeDataTypeType,
+    },
+)
+_OptionalActuatorOutputTypeDef = TypedDict(
+    "_OptionalActuatorOutputTypeDef",
+    {
+        "description": str,
+        "unit": str,
+        "allowedValues": List[str],
+        "min": float,
+        "max": float,
+        "assignedValue": str,
+        "deprecationMessage": str,
+        "comment": str,
+    },
+    total=False,
+)
+
+
+class ActuatorOutputTypeDef(_RequiredActuatorOutputTypeDef, _OptionalActuatorOutputTypeDef):
+    pass
+
+
 _RequiredActuatorTypeDef = TypedDict(
     "_RequiredActuatorTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -226,14 +275,42 @@
     "AssociateVehicleFleetRequestRequestTypeDef",
     {
         "vehicleName": str,
         "fleetId": str,
     },
 )
 
+_RequiredAttributeOutputTypeDef = TypedDict(
+    "_RequiredAttributeOutputTypeDef",
+    {
+        "fullyQualifiedName": str,
+        "dataType": NodeDataTypeType,
+    },
+)
+_OptionalAttributeOutputTypeDef = TypedDict(
+    "_OptionalAttributeOutputTypeDef",
+    {
+        "description": str,
+        "unit": str,
+        "allowedValues": List[str],
+        "min": float,
+        "max": float,
+        "assignedValue": str,
+        "defaultValue": str,
+        "deprecationMessage": str,
+        "comment": str,
+    },
+    total=False,
+)
+
+
+class AttributeOutputTypeDef(_RequiredAttributeOutputTypeDef, _OptionalAttributeOutputTypeDef):
+    pass
+
+
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -317,14 +394,35 @@
     {
         "vehicleName": str,
         "arn": str,
     },
     total=False,
 )
 
+_RequiredBranchOutputTypeDef = TypedDict(
+    "_RequiredBranchOutputTypeDef",
+    {
+        "fullyQualifiedName": str,
+    },
+)
+_OptionalBranchOutputTypeDef = TypedDict(
+    "_OptionalBranchOutputTypeDef",
+    {
+        "description": str,
+        "deprecationMessage": str,
+        "comment": str,
+    },
+    total=False,
+)
+
+
+class BranchOutputTypeDef(_RequiredBranchOutputTypeDef, _OptionalBranchOutputTypeDef):
+    pass
+
+
 _RequiredBranchTypeDef = TypedDict(
     "_RequiredBranchTypeDef",
     {
         "fullyQualifiedName": str,
     },
 )
 _OptionalBranchTypeDef = TypedDict(
@@ -383,14 +481,36 @@
 )
 
 
 class CanDbcDefinitionTypeDef(_RequiredCanDbcDefinitionTypeDef, _OptionalCanDbcDefinitionTypeDef):
     pass
 
 
+_RequiredCanInterfaceOutputTypeDef = TypedDict(
+    "_RequiredCanInterfaceOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCanInterfaceOutputTypeDef = TypedDict(
+    "_OptionalCanInterfaceOutputTypeDef",
+    {
+        "protocolName": str,
+        "protocolVersion": str,
+    },
+    total=False,
+)
+
+
+class CanInterfaceOutputTypeDef(
+    _RequiredCanInterfaceOutputTypeDef, _OptionalCanInterfaceOutputTypeDef
+):
+    pass
+
+
 _RequiredCanInterfaceTypeDef = TypedDict(
     "_RequiredCanInterfaceTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCanInterfaceTypeDef = TypedDict(
@@ -403,14 +523,39 @@
 )
 
 
 class CanInterfaceTypeDef(_RequiredCanInterfaceTypeDef, _OptionalCanInterfaceTypeDef):
     pass
 
 
+_RequiredCanSignalOutputTypeDef = TypedDict(
+    "_RequiredCanSignalOutputTypeDef",
+    {
+        "messageId": int,
+        "isBigEndian": bool,
+        "isSigned": bool,
+        "startBit": int,
+        "offset": float,
+        "factor": float,
+        "length": int,
+    },
+)
+_OptionalCanSignalOutputTypeDef = TypedDict(
+    "_OptionalCanSignalOutputTypeDef",
+    {
+        "name": str,
+    },
+    total=False,
+)
+
+
+class CanSignalOutputTypeDef(_RequiredCanSignalOutputTypeDef, _OptionalCanSignalOutputTypeDef):
+    pass
+
+
 _RequiredCanSignalTypeDef = TypedDict(
     "_RequiredCanSignalTypeDef",
     {
         "messageId": int,
         "isBigEndian": bool,
         "isSigned": bool,
         "startBit": int,
@@ -428,14 +573,36 @@
 )
 
 
 class CanSignalTypeDef(_RequiredCanSignalTypeDef, _OptionalCanSignalTypeDef):
     pass
 
 
+_RequiredCloudWatchLogDeliveryOptionsOutputTypeDef = TypedDict(
+    "_RequiredCloudWatchLogDeliveryOptionsOutputTypeDef",
+    {
+        "logType": LogTypeType,
+    },
+)
+_OptionalCloudWatchLogDeliveryOptionsOutputTypeDef = TypedDict(
+    "_OptionalCloudWatchLogDeliveryOptionsOutputTypeDef",
+    {
+        "logGroupName": str,
+    },
+    total=False,
+)
+
+
+class CloudWatchLogDeliveryOptionsOutputTypeDef(
+    _RequiredCloudWatchLogDeliveryOptionsOutputTypeDef,
+    _OptionalCloudWatchLogDeliveryOptionsOutputTypeDef,
+):
+    pass
+
+
 _RequiredCloudWatchLogDeliveryOptionsTypeDef = TypedDict(
     "_RequiredCloudWatchLogDeliveryOptionsTypeDef",
     {
         "logType": LogTypeType,
     },
 )
 _OptionalCloudWatchLogDeliveryOptionsTypeDef = TypedDict(
@@ -449,14 +616,45 @@
 
 class CloudWatchLogDeliveryOptionsTypeDef(
     _RequiredCloudWatchLogDeliveryOptionsTypeDef, _OptionalCloudWatchLogDeliveryOptionsTypeDef
 ):
     pass
 
 
+_RequiredConditionBasedCollectionSchemeOutputTypeDef = TypedDict(
+    "_RequiredConditionBasedCollectionSchemeOutputTypeDef",
+    {
+        "expression": str,
+    },
+)
+_OptionalConditionBasedCollectionSchemeOutputTypeDef = TypedDict(
+    "_OptionalConditionBasedCollectionSchemeOutputTypeDef",
+    {
+        "minimumTriggerIntervalMs": int,
+        "triggerMode": TriggerModeType,
+        "conditionLanguageVersion": int,
+    },
+    total=False,
+)
+
+
+class ConditionBasedCollectionSchemeOutputTypeDef(
+    _RequiredConditionBasedCollectionSchemeOutputTypeDef,
+    _OptionalConditionBasedCollectionSchemeOutputTypeDef,
+):
+    pass
+
+
+TimeBasedCollectionSchemeOutputTypeDef = TypedDict(
+    "TimeBasedCollectionSchemeOutputTypeDef",
+    {
+        "periodMs": int,
+    },
+)
+
 _RequiredConditionBasedCollectionSchemeTypeDef = TypedDict(
     "_RequiredConditionBasedCollectionSchemeTypeDef",
     {
         "expression": str,
     },
 )
 _OptionalConditionBasedCollectionSchemeTypeDef = TypedDict(
@@ -564,14 +762,43 @@
         "vehicleName": str,
         "arn": str,
         "thingArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredS3ConfigOutputTypeDef = TypedDict(
+    "_RequiredS3ConfigOutputTypeDef",
+    {
+        "bucketArn": str,
+    },
+)
+_OptionalS3ConfigOutputTypeDef = TypedDict(
+    "_OptionalS3ConfigOutputTypeDef",
+    {
+        "dataFormat": DataFormatType,
+        "storageCompressionFormat": StorageCompressionFormatType,
+        "prefix": str,
+    },
+    total=False,
+)
+
+
+class S3ConfigOutputTypeDef(_RequiredS3ConfigOutputTypeDef, _OptionalS3ConfigOutputTypeDef):
+    pass
+
+
+TimestreamConfigOutputTypeDef = TypedDict(
+    "TimestreamConfigOutputTypeDef",
+    {
+        "timestreamTableArn": str,
+        "executionRoleArn": str,
+    },
+)
+
 _RequiredS3ConfigTypeDef = TypedDict(
     "_RequiredS3ConfigTypeDef",
     {
         "bucketArn": str,
     },
 )
 _OptionalS3ConfigTypeDef = TypedDict(
@@ -761,14 +988,36 @@
 GetCampaignRequestRequestTypeDef = TypedDict(
     "GetCampaignRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
+_RequiredSignalInformationOutputTypeDef = TypedDict(
+    "_RequiredSignalInformationOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalSignalInformationOutputTypeDef = TypedDict(
+    "_OptionalSignalInformationOutputTypeDef",
+    {
+        "maxSampleCount": int,
+        "minimumSamplingIntervalMs": int,
+    },
+    total=False,
+)
+
+
+class SignalInformationOutputTypeDef(
+    _RequiredSignalInformationOutputTypeDef, _OptionalSignalInformationOutputTypeDef
+):
+    pass
+
+
 GetDecoderManifestRequestRequestTypeDef = TypedDict(
     "GetDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -964,14 +1213,21 @@
         "campaignName": str,
         "vehicleName": str,
         "status": VehicleStateType,
     },
     total=False,
 )
 
+IamResourcesOutputTypeDef = TypedDict(
+    "IamResourcesOutputTypeDef",
+    {
+        "roleArn": str,
+    },
+)
+
 IamResourcesTypeDef = TypedDict(
     "IamResourcesTypeDef",
     {
         "roleArn": str,
     },
 )
 
@@ -1358,14 +1614,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 _RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef = TypedDict(
     "_RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
     {
         "fleetId": str,
     },
 )
 _OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef = TypedDict(
@@ -1443,14 +1707,40 @@
         "modelManifestArn": str,
         "decoderManifestArn": str,
         "creationTime": datetime,
         "lastModificationTime": datetime,
     },
 )
 
+_RequiredObdInterfaceOutputTypeDef = TypedDict(
+    "_RequiredObdInterfaceOutputTypeDef",
+    {
+        "name": str,
+        "requestMessageId": int,
+    },
+)
+_OptionalObdInterfaceOutputTypeDef = TypedDict(
+    "_OptionalObdInterfaceOutputTypeDef",
+    {
+        "obdStandard": str,
+        "pidRequestIntervalSeconds": int,
+        "dtcRequestIntervalSeconds": int,
+        "useExtendedIds": bool,
+        "hasTransmissionEcu": bool,
+    },
+    total=False,
+)
+
+
+class ObdInterfaceOutputTypeDef(
+    _RequiredObdInterfaceOutputTypeDef, _OptionalObdInterfaceOutputTypeDef
+):
+    pass
+
+
 _RequiredObdInterfaceTypeDef = TypedDict(
     "_RequiredObdInterfaceTypeDef",
     {
         "name": str,
         "requestMessageId": int,
     },
 )
@@ -1467,14 +1757,40 @@
 )
 
 
 class ObdInterfaceTypeDef(_RequiredObdInterfaceTypeDef, _OptionalObdInterfaceTypeDef):
     pass
 
 
+_RequiredSensorOutputTypeDef = TypedDict(
+    "_RequiredSensorOutputTypeDef",
+    {
+        "fullyQualifiedName": str,
+        "dataType": NodeDataTypeType,
+    },
+)
+_OptionalSensorOutputTypeDef = TypedDict(
+    "_OptionalSensorOutputTypeDef",
+    {
+        "description": str,
+        "unit": str,
+        "allowedValues": List[str],
+        "min": float,
+        "max": float,
+        "deprecationMessage": str,
+        "comment": str,
+    },
+    total=False,
+)
+
+
+class SensorOutputTypeDef(_RequiredSensorOutputTypeDef, _OptionalSensorOutputTypeDef):
+    pass
+
+
 _RequiredSensorTypeDef = TypedDict(
     "_RequiredSensorTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -1493,14 +1809,40 @@
 )
 
 
 class SensorTypeDef(_RequiredSensorTypeDef, _OptionalSensorTypeDef):
     pass
 
 
+_RequiredObdSignalOutputTypeDef = TypedDict(
+    "_RequiredObdSignalOutputTypeDef",
+    {
+        "pidResponseLength": int,
+        "serviceMode": int,
+        "pid": int,
+        "scaling": float,
+        "offset": float,
+        "startByte": int,
+        "byteLength": int,
+    },
+)
+_OptionalObdSignalOutputTypeDef = TypedDict(
+    "_OptionalObdSignalOutputTypeDef",
+    {
+        "bitRightShift": int,
+        "bitMaskLength": int,
+    },
+    total=False,
+)
+
+
+class ObdSignalOutputTypeDef(_RequiredObdSignalOutputTypeDef, _OptionalObdSignalOutputTypeDef):
+    pass
+
+
 _RequiredObdSignalTypeDef = TypedDict(
     "_RequiredObdSignalTypeDef",
     {
         "pidResponseLength": int,
         "serviceMode": int,
         "pid": int,
         "scaling": float,
@@ -1537,14 +1879,22 @@
     "TimestreamResourcesTypeDef",
     {
         "timestreamDatabaseName": str,
         "timestreamTableName": str,
     },
 )
 
+TimestreamResourcesOutputTypeDef = TypedDict(
+    "TimestreamResourcesOutputTypeDef",
+    {
+        "timestreamDatabaseName": str,
+        "timestreamTableName": str,
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
@@ -1749,26 +2099,35 @@
     },
     total=False,
 )
 
 GetLoggingOptionsResponseTypeDef = TypedDict(
     "GetLoggingOptionsResponseTypeDef",
     {
-        "cloudWatchLogDelivery": CloudWatchLogDeliveryOptionsTypeDef,
+        "cloudWatchLogDelivery": CloudWatchLogDeliveryOptionsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutLoggingOptionsRequestRequestTypeDef = TypedDict(
     "PutLoggingOptionsRequestRequestTypeDef",
     {
         "cloudWatchLogDelivery": CloudWatchLogDeliveryOptionsTypeDef,
     },
 )
 
+CollectionSchemeOutputTypeDef = TypedDict(
+    "CollectionSchemeOutputTypeDef",
+    {
+        "timeBasedCollectionScheme": TimeBasedCollectionSchemeOutputTypeDef,
+        "conditionBasedCollectionScheme": ConditionBasedCollectionSchemeOutputTypeDef,
+    },
+    total=False,
+)
+
 CollectionSchemeTypeDef = TypedDict(
     "CollectionSchemeTypeDef",
     {
         "timeBasedCollectionScheme": TimeBasedCollectionSchemeTypeDef,
         "conditionBasedCollectionScheme": ConditionBasedCollectionSchemeTypeDef,
     },
     total=False,
@@ -1868,30 +2227,31 @@
 
 class CreateVehicleRequestRequestTypeDef(
     _RequiredCreateVehicleRequestRequestTypeDef, _OptionalCreateVehicleRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+DataDestinationConfigOutputTypeDef = TypedDict(
+    "DataDestinationConfigOutputTypeDef",
+    {
+        "s3Config": S3ConfigOutputTypeDef,
+        "timestreamConfig": TimestreamConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 DataDestinationConfigTypeDef = TypedDict(
     "DataDestinationConfigTypeDef",
     {
         "s3Config": S3ConfigTypeDef,
         "timestreamConfig": TimestreamConfigTypeDef,
     },
     total=False,
@@ -1988,23 +2348,54 @@
     {
         "summaries": List[SignalCatalogSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListVehiclesResponseTypeDef = TypedDict(
     "ListVehiclesResponseTypeDef",
     {
         "vehicleSummaries": List[VehicleSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredNetworkInterfaceOutputTypeDef = TypedDict(
+    "_RequiredNetworkInterfaceOutputTypeDef",
+    {
+        "interfaceId": str,
+        "type": NetworkInterfaceTypeType,
+    },
+)
+_OptionalNetworkInterfaceOutputTypeDef = TypedDict(
+    "_OptionalNetworkInterfaceOutputTypeDef",
+    {
+        "canInterface": CanInterfaceOutputTypeDef,
+        "obdInterface": ObdInterfaceOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class NetworkInterfaceOutputTypeDef(
+    _RequiredNetworkInterfaceOutputTypeDef, _OptionalNetworkInterfaceOutputTypeDef
+):
+    pass
+
+
 _RequiredNetworkInterfaceTypeDef = TypedDict(
     "_RequiredNetworkInterfaceTypeDef",
     {
         "interfaceId": str,
         "type": NetworkInterfaceTypeType,
     },
 )
@@ -2018,25 +2409,60 @@
 )
 
 
 class NetworkInterfaceTypeDef(_RequiredNetworkInterfaceTypeDef, _OptionalNetworkInterfaceTypeDef):
     pass
 
 
+NodeOutputTypeDef = TypedDict(
+    "NodeOutputTypeDef",
+    {
+        "branch": BranchOutputTypeDef,
+        "sensor": SensorOutputTypeDef,
+        "actuator": ActuatorOutputTypeDef,
+        "attribute": AttributeOutputTypeDef,
+    },
+    total=False,
+)
+
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "branch": BranchTypeDef,
         "sensor": SensorTypeDef,
         "actuator": ActuatorTypeDef,
         "attribute": AttributeTypeDef,
     },
     total=False,
 )
 
+_RequiredSignalDecoderOutputTypeDef = TypedDict(
+    "_RequiredSignalDecoderOutputTypeDef",
+    {
+        "fullyQualifiedName": str,
+        "type": SignalDecoderTypeType,
+        "interfaceId": str,
+    },
+)
+_OptionalSignalDecoderOutputTypeDef = TypedDict(
+    "_OptionalSignalDecoderOutputTypeDef",
+    {
+        "canSignal": CanSignalOutputTypeDef,
+        "obdSignal": ObdSignalOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class SignalDecoderOutputTypeDef(
+    _RequiredSignalDecoderOutputTypeDef, _OptionalSignalDecoderOutputTypeDef
+):
+    pass
+
+
 _RequiredSignalDecoderTypeDef = TypedDict(
     "_RequiredSignalDecoderTypeDef",
     {
         "fullyQualifiedName": str,
         "type": SignalDecoderTypeType,
         "interfaceId": str,
     },
@@ -2064,16 +2490,16 @@
     total=False,
 )
 
 RegisterAccountResponseTypeDef = TypedDict(
     "RegisterAccountResponseTypeDef",
     {
         "registerAccountStatus": RegistrationStatusType,
-        "timestreamResources": TimestreamResourcesTypeDef,
-        "iamResources": IamResourcesTypeDef,
+        "timestreamResources": TimestreamResourcesOutputTypeDef,
+        "iamResources": IamResourcesOutputTypeDef,
         "creationTime": datetime,
         "lastModificationTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportDecoderManifestRequestRequestTypeDef = TypedDict(
@@ -2087,14 +2513,40 @@
 BatchCreateVehicleRequestRequestTypeDef = TypedDict(
     "BatchCreateVehicleRequestRequestTypeDef",
     {
         "vehicles": Sequence[CreateVehicleRequestItemTypeDef],
     },
 )
 
+GetCampaignResponseTypeDef = TypedDict(
+    "GetCampaignResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "description": str,
+        "signalCatalogArn": str,
+        "targetArn": str,
+        "status": CampaignStatusType,
+        "startTime": datetime,
+        "expiryTime": datetime,
+        "postTriggerCollectionDuration": int,
+        "diagnosticsMode": DiagnosticsModeType,
+        "spoolingMode": SpoolingModeType,
+        "compression": CompressionType,
+        "priority": int,
+        "signalsToCollect": List[SignalInformationOutputTypeDef],
+        "collectionScheme": CollectionSchemeOutputTypeDef,
+        "dataExtraDimensions": List[str],
+        "creationTime": datetime,
+        "lastModificationTime": datetime,
+        "dataDestinationConfigs": List[DataDestinationConfigOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateCampaignRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCampaignRequestRequestTypeDef",
     {
         "name": str,
         "signalCatalogArn": str,
         "targetArn": str,
         "collectionScheme": CollectionSchemeTypeDef,
@@ -2122,44 +2574,36 @@
 
 class CreateCampaignRequestRequestTypeDef(
     _RequiredCreateCampaignRequestRequestTypeDef, _OptionalCreateCampaignRequestRequestTypeDef
 ):
     pass
 
 
-GetCampaignResponseTypeDef = TypedDict(
-    "GetCampaignResponseTypeDef",
+ListDecoderManifestNetworkInterfacesResponseTypeDef = TypedDict(
+    "ListDecoderManifestNetworkInterfacesResponseTypeDef",
     {
-        "name": str,
-        "arn": str,
-        "description": str,
-        "signalCatalogArn": str,
-        "targetArn": str,
-        "status": CampaignStatusType,
-        "startTime": datetime,
-        "expiryTime": datetime,
-        "postTriggerCollectionDuration": int,
-        "diagnosticsMode": DiagnosticsModeType,
-        "spoolingMode": SpoolingModeType,
-        "compression": CompressionType,
-        "priority": int,
-        "signalsToCollect": List[SignalInformationTypeDef],
-        "collectionScheme": CollectionSchemeTypeDef,
-        "dataExtraDimensions": List[str],
-        "creationTime": datetime,
-        "lastModificationTime": datetime,
-        "dataDestinationConfigs": List[DataDestinationConfigTypeDef],
+        "networkInterfaces": List[NetworkInterfaceOutputTypeDef],
+        "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDecoderManifestNetworkInterfacesResponseTypeDef = TypedDict(
-    "ListDecoderManifestNetworkInterfacesResponseTypeDef",
+ListModelManifestNodesResponseTypeDef = TypedDict(
+    "ListModelManifestNodesResponseTypeDef",
+    {
+        "nodes": List[NodeOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListSignalCatalogNodesResponseTypeDef = TypedDict(
+    "ListSignalCatalogNodesResponseTypeDef",
     {
-        "networkInterfaces": List[NetworkInterfaceTypeDef],
+        "nodes": List[NodeOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateSignalCatalogRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSignalCatalogRequestRequestTypeDef",
@@ -2181,32 +2625,14 @@
 class CreateSignalCatalogRequestRequestTypeDef(
     _RequiredCreateSignalCatalogRequestRequestTypeDef,
     _OptionalCreateSignalCatalogRequestRequestTypeDef,
 ):
     pass
 
 
-ListModelManifestNodesResponseTypeDef = TypedDict(
-    "ListModelManifestNodesResponseTypeDef",
-    {
-        "nodes": List[NodeTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSignalCatalogNodesResponseTypeDef = TypedDict(
-    "ListSignalCatalogNodesResponseTypeDef",
-    {
-        "nodes": List[NodeTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSignalCatalogRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
@@ -2224,14 +2650,23 @@
 class UpdateSignalCatalogRequestRequestTypeDef(
     _RequiredUpdateSignalCatalogRequestRequestTypeDef,
     _OptionalUpdateSignalCatalogRequestRequestTypeDef,
 ):
     pass
 
 
+ListDecoderManifestSignalsResponseTypeDef = TypedDict(
+    "ListDecoderManifestSignalsResponseTypeDef",
+    {
+        "signalDecoders": List[SignalDecoderOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateDecoderManifestRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
         "modelManifestArn": str,
     },
 )
@@ -2250,23 +2685,14 @@
 class CreateDecoderManifestRequestRequestTypeDef(
     _RequiredCreateDecoderManifestRequestRequestTypeDef,
     _OptionalCreateDecoderManifestRequestRequestTypeDef,
 ):
     pass
 
 
-ListDecoderManifestSignalsResponseTypeDef = TypedDict(
-    "ListDecoderManifestSignalsResponseTypeDef",
-    {
-        "signalDecoders": List[SignalDecoderTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateDecoderManifestRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateDecoderManifestRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise/type_defs.pyi` & `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise/type_defs.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iotfleetwise service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iotfleetwise.type_defs import ActuatorTypeDef
+    from mypy_boto3_iotfleetwise.type_defs import ActuatorOutputTypeDef
 
-    data: ActuatorTypeDef = {...}
+    data: ActuatorOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -39,38 +39,48 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "ActuatorOutputTypeDef",
     "ActuatorTypeDef",
     "AssociateVehicleFleetRequestRequestTypeDef",
+    "AttributeOutputTypeDef",
     "AttributeTypeDef",
     "CreateVehicleErrorTypeDef",
     "CreateVehicleResponseItemTypeDef",
     "UpdateVehicleRequestItemTypeDef",
     "UpdateVehicleErrorTypeDef",
     "UpdateVehicleResponseItemTypeDef",
+    "BranchOutputTypeDef",
     "BranchTypeDef",
     "CampaignSummaryTypeDef",
     "CanDbcDefinitionTypeDef",
+    "CanInterfaceOutputTypeDef",
     "CanInterfaceTypeDef",
+    "CanSignalOutputTypeDef",
     "CanSignalTypeDef",
+    "CloudWatchLogDeliveryOptionsOutputTypeDef",
     "CloudWatchLogDeliveryOptionsTypeDef",
+    "ConditionBasedCollectionSchemeOutputTypeDef",
+    "TimeBasedCollectionSchemeOutputTypeDef",
     "ConditionBasedCollectionSchemeTypeDef",
     "TimeBasedCollectionSchemeTypeDef",
     "SignalInformationTypeDef",
     "TagTypeDef",
     "CreateCampaignResponseTypeDef",
     "CreateDecoderManifestResponseTypeDef",
     "CreateFleetResponseTypeDef",
     "CreateModelManifestResponseTypeDef",
     "CreateSignalCatalogResponseTypeDef",
     "CreateVehicleResponseTypeDef",
+    "S3ConfigOutputTypeDef",
+    "TimestreamConfigOutputTypeDef",
     "S3ConfigTypeDef",
     "TimestreamConfigTypeDef",
     "DecoderManifestSummaryTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteCampaignResponseTypeDef",
     "DeleteDecoderManifestRequestRequestTypeDef",
     "DeleteDecoderManifestResponseTypeDef",
@@ -82,14 +92,15 @@
     "DeleteSignalCatalogResponseTypeDef",
     "DeleteVehicleRequestRequestTypeDef",
     "DeleteVehicleResponseTypeDef",
     "DisassociateVehicleFleetRequestRequestTypeDef",
     "FleetSummaryTypeDef",
     "FormattedVssTypeDef",
     "GetCampaignRequestRequestTypeDef",
+    "SignalInformationOutputTypeDef",
     "GetDecoderManifestRequestRequestTypeDef",
     "GetDecoderManifestResponseTypeDef",
     "GetFleetRequestRequestTypeDef",
     "GetFleetResponseTypeDef",
     "GetModelManifestRequestRequestTypeDef",
     "GetModelManifestResponseTypeDef",
     "IamRegistrationResponseTypeDef",
@@ -97,14 +108,15 @@
     "GetSignalCatalogRequestRequestTypeDef",
     "NodeCountsTypeDef",
     "GetVehicleRequestRequestTypeDef",
     "GetVehicleResponseTypeDef",
     "GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
     "GetVehicleStatusRequestRequestTypeDef",
     "VehicleStatusTypeDef",
+    "IamResourcesOutputTypeDef",
     "IamResourcesTypeDef",
     "ImportDecoderManifestResponseTypeDef",
     "ImportSignalCatalogResponseTypeDef",
     "ListCampaignsRequestListCampaignsPaginateTypeDef",
     "ListCampaignsRequestRequestTypeDef",
     "ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
     "ListDecoderManifestNetworkInterfacesRequestRequestTypeDef",
@@ -124,25 +136,30 @@
     "ModelManifestSummaryTypeDef",
     "ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
     "ListSignalCatalogNodesRequestRequestTypeDef",
     "ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef",
     "ListSignalCatalogsRequestRequestTypeDef",
     "SignalCatalogSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
     "ListVehiclesInFleetRequestRequestTypeDef",
     "ListVehiclesInFleetResponseTypeDef",
     "ListVehiclesRequestListVehiclesPaginateTypeDef",
     "ListVehiclesRequestRequestTypeDef",
     "VehicleSummaryTypeDef",
+    "ObdInterfaceOutputTypeDef",
     "ObdInterfaceTypeDef",
+    "SensorOutputTypeDef",
     "SensorTypeDef",
+    "ObdSignalOutputTypeDef",
     "ObdSignalTypeDef",
     "PaginatorConfigTypeDef",
     "TimestreamResourcesTypeDef",
+    "TimestreamResourcesOutputTypeDef",
     "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCampaignRequestRequestTypeDef",
     "UpdateCampaignResponseTypeDef",
     "UpdateDecoderManifestResponseTypeDef",
     "UpdateFleetRequestRequestTypeDef",
     "UpdateFleetResponseTypeDef",
@@ -154,50 +171,80 @@
     "BatchCreateVehicleResponseTypeDef",
     "BatchUpdateVehicleRequestRequestTypeDef",
     "BatchUpdateVehicleResponseTypeDef",
     "ListCampaignsResponseTypeDef",
     "NetworkFileDefinitionTypeDef",
     "GetLoggingOptionsResponseTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
+    "CollectionSchemeOutputTypeDef",
     "CollectionSchemeTypeDef",
     "CreateFleetRequestRequestTypeDef",
     "CreateModelManifestRequestRequestTypeDef",
     "CreateVehicleRequestItemTypeDef",
     "CreateVehicleRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "DataDestinationConfigOutputTypeDef",
     "DataDestinationConfigTypeDef",
     "ListDecoderManifestsResponseTypeDef",
     "ListFleetsResponseTypeDef",
     "ImportSignalCatalogRequestRequestTypeDef",
     "GetRegisterAccountStatusResponseTypeDef",
     "GetSignalCatalogResponseTypeDef",
     "GetVehicleStatusResponseTypeDef",
     "ListModelManifestsResponseTypeDef",
     "ListSignalCatalogsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListVehiclesResponseTypeDef",
+    "NetworkInterfaceOutputTypeDef",
     "NetworkInterfaceTypeDef",
+    "NodeOutputTypeDef",
     "NodeTypeDef",
+    "SignalDecoderOutputTypeDef",
     "SignalDecoderTypeDef",
     "RegisterAccountRequestRequestTypeDef",
     "RegisterAccountResponseTypeDef",
     "ImportDecoderManifestRequestRequestTypeDef",
     "BatchCreateVehicleRequestRequestTypeDef",
-    "CreateCampaignRequestRequestTypeDef",
     "GetCampaignResponseTypeDef",
+    "CreateCampaignRequestRequestTypeDef",
     "ListDecoderManifestNetworkInterfacesResponseTypeDef",
-    "CreateSignalCatalogRequestRequestTypeDef",
     "ListModelManifestNodesResponseTypeDef",
     "ListSignalCatalogNodesResponseTypeDef",
+    "CreateSignalCatalogRequestRequestTypeDef",
     "UpdateSignalCatalogRequestRequestTypeDef",
-    "CreateDecoderManifestRequestRequestTypeDef",
     "ListDecoderManifestSignalsResponseTypeDef",
+    "CreateDecoderManifestRequestRequestTypeDef",
     "UpdateDecoderManifestRequestRequestTypeDef",
 )
 
+_RequiredActuatorOutputTypeDef = TypedDict(
+    "_RequiredActuatorOutputTypeDef",
+    {
+        "fullyQualifiedName": str,
+        "dataType": NodeDataTypeType,
+    },
+)
+_OptionalActuatorOutputTypeDef = TypedDict(
+    "_OptionalActuatorOutputTypeDef",
+    {
+        "description": str,
+        "unit": str,
+        "allowedValues": List[str],
+        "min": float,
+        "max": float,
+        "assignedValue": str,
+        "deprecationMessage": str,
+        "comment": str,
+    },
+    total=False,
+)
+
+class ActuatorOutputTypeDef(_RequiredActuatorOutputTypeDef, _OptionalActuatorOutputTypeDef):
+    pass
+
 _RequiredActuatorTypeDef = TypedDict(
     "_RequiredActuatorTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -223,14 +270,40 @@
     "AssociateVehicleFleetRequestRequestTypeDef",
     {
         "vehicleName": str,
         "fleetId": str,
     },
 )
 
+_RequiredAttributeOutputTypeDef = TypedDict(
+    "_RequiredAttributeOutputTypeDef",
+    {
+        "fullyQualifiedName": str,
+        "dataType": NodeDataTypeType,
+    },
+)
+_OptionalAttributeOutputTypeDef = TypedDict(
+    "_OptionalAttributeOutputTypeDef",
+    {
+        "description": str,
+        "unit": str,
+        "allowedValues": List[str],
+        "min": float,
+        "max": float,
+        "assignedValue": str,
+        "defaultValue": str,
+        "deprecationMessage": str,
+        "comment": str,
+    },
+    total=False,
+)
+
+class AttributeOutputTypeDef(_RequiredAttributeOutputTypeDef, _OptionalAttributeOutputTypeDef):
+    pass
+
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -310,14 +383,33 @@
     {
         "vehicleName": str,
         "arn": str,
     },
     total=False,
 )
 
+_RequiredBranchOutputTypeDef = TypedDict(
+    "_RequiredBranchOutputTypeDef",
+    {
+        "fullyQualifiedName": str,
+    },
+)
+_OptionalBranchOutputTypeDef = TypedDict(
+    "_OptionalBranchOutputTypeDef",
+    {
+        "description": str,
+        "deprecationMessage": str,
+        "comment": str,
+    },
+    total=False,
+)
+
+class BranchOutputTypeDef(_RequiredBranchOutputTypeDef, _OptionalBranchOutputTypeDef):
+    pass
+
 _RequiredBranchTypeDef = TypedDict(
     "_RequiredBranchTypeDef",
     {
         "fullyQualifiedName": str,
     },
 )
 _OptionalBranchTypeDef = TypedDict(
@@ -370,14 +462,34 @@
     },
     total=False,
 )
 
 class CanDbcDefinitionTypeDef(_RequiredCanDbcDefinitionTypeDef, _OptionalCanDbcDefinitionTypeDef):
     pass
 
+_RequiredCanInterfaceOutputTypeDef = TypedDict(
+    "_RequiredCanInterfaceOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCanInterfaceOutputTypeDef = TypedDict(
+    "_OptionalCanInterfaceOutputTypeDef",
+    {
+        "protocolName": str,
+        "protocolVersion": str,
+    },
+    total=False,
+)
+
+class CanInterfaceOutputTypeDef(
+    _RequiredCanInterfaceOutputTypeDef, _OptionalCanInterfaceOutputTypeDef
+):
+    pass
+
 _RequiredCanInterfaceTypeDef = TypedDict(
     "_RequiredCanInterfaceTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCanInterfaceTypeDef = TypedDict(
@@ -388,14 +500,37 @@
     },
     total=False,
 )
 
 class CanInterfaceTypeDef(_RequiredCanInterfaceTypeDef, _OptionalCanInterfaceTypeDef):
     pass
 
+_RequiredCanSignalOutputTypeDef = TypedDict(
+    "_RequiredCanSignalOutputTypeDef",
+    {
+        "messageId": int,
+        "isBigEndian": bool,
+        "isSigned": bool,
+        "startBit": int,
+        "offset": float,
+        "factor": float,
+        "length": int,
+    },
+)
+_OptionalCanSignalOutputTypeDef = TypedDict(
+    "_OptionalCanSignalOutputTypeDef",
+    {
+        "name": str,
+    },
+    total=False,
+)
+
+class CanSignalOutputTypeDef(_RequiredCanSignalOutputTypeDef, _OptionalCanSignalOutputTypeDef):
+    pass
+
 _RequiredCanSignalTypeDef = TypedDict(
     "_RequiredCanSignalTypeDef",
     {
         "messageId": int,
         "isBigEndian": bool,
         "isSigned": bool,
         "startBit": int,
@@ -411,14 +546,34 @@
     },
     total=False,
 )
 
 class CanSignalTypeDef(_RequiredCanSignalTypeDef, _OptionalCanSignalTypeDef):
     pass
 
+_RequiredCloudWatchLogDeliveryOptionsOutputTypeDef = TypedDict(
+    "_RequiredCloudWatchLogDeliveryOptionsOutputTypeDef",
+    {
+        "logType": LogTypeType,
+    },
+)
+_OptionalCloudWatchLogDeliveryOptionsOutputTypeDef = TypedDict(
+    "_OptionalCloudWatchLogDeliveryOptionsOutputTypeDef",
+    {
+        "logGroupName": str,
+    },
+    total=False,
+)
+
+class CloudWatchLogDeliveryOptionsOutputTypeDef(
+    _RequiredCloudWatchLogDeliveryOptionsOutputTypeDef,
+    _OptionalCloudWatchLogDeliveryOptionsOutputTypeDef,
+):
+    pass
+
 _RequiredCloudWatchLogDeliveryOptionsTypeDef = TypedDict(
     "_RequiredCloudWatchLogDeliveryOptionsTypeDef",
     {
         "logType": LogTypeType,
     },
 )
 _OptionalCloudWatchLogDeliveryOptionsTypeDef = TypedDict(
@@ -430,14 +585,43 @@
 )
 
 class CloudWatchLogDeliveryOptionsTypeDef(
     _RequiredCloudWatchLogDeliveryOptionsTypeDef, _OptionalCloudWatchLogDeliveryOptionsTypeDef
 ):
     pass
 
+_RequiredConditionBasedCollectionSchemeOutputTypeDef = TypedDict(
+    "_RequiredConditionBasedCollectionSchemeOutputTypeDef",
+    {
+        "expression": str,
+    },
+)
+_OptionalConditionBasedCollectionSchemeOutputTypeDef = TypedDict(
+    "_OptionalConditionBasedCollectionSchemeOutputTypeDef",
+    {
+        "minimumTriggerIntervalMs": int,
+        "triggerMode": TriggerModeType,
+        "conditionLanguageVersion": int,
+    },
+    total=False,
+)
+
+class ConditionBasedCollectionSchemeOutputTypeDef(
+    _RequiredConditionBasedCollectionSchemeOutputTypeDef,
+    _OptionalConditionBasedCollectionSchemeOutputTypeDef,
+):
+    pass
+
+TimeBasedCollectionSchemeOutputTypeDef = TypedDict(
+    "TimeBasedCollectionSchemeOutputTypeDef",
+    {
+        "periodMs": int,
+    },
+)
+
 _RequiredConditionBasedCollectionSchemeTypeDef = TypedDict(
     "_RequiredConditionBasedCollectionSchemeTypeDef",
     {
         "expression": str,
     },
 )
 _OptionalConditionBasedCollectionSchemeTypeDef = TypedDict(
@@ -541,14 +725,41 @@
         "vehicleName": str,
         "arn": str,
         "thingArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredS3ConfigOutputTypeDef = TypedDict(
+    "_RequiredS3ConfigOutputTypeDef",
+    {
+        "bucketArn": str,
+    },
+)
+_OptionalS3ConfigOutputTypeDef = TypedDict(
+    "_OptionalS3ConfigOutputTypeDef",
+    {
+        "dataFormat": DataFormatType,
+        "storageCompressionFormat": StorageCompressionFormatType,
+        "prefix": str,
+    },
+    total=False,
+)
+
+class S3ConfigOutputTypeDef(_RequiredS3ConfigOutputTypeDef, _OptionalS3ConfigOutputTypeDef):
+    pass
+
+TimestreamConfigOutputTypeDef = TypedDict(
+    "TimestreamConfigOutputTypeDef",
+    {
+        "timestreamTableArn": str,
+        "executionRoleArn": str,
+    },
+)
+
 _RequiredS3ConfigTypeDef = TypedDict(
     "_RequiredS3ConfigTypeDef",
     {
         "bucketArn": str,
     },
 )
 _OptionalS3ConfigTypeDef = TypedDict(
@@ -732,14 +943,34 @@
 GetCampaignRequestRequestTypeDef = TypedDict(
     "GetCampaignRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
+_RequiredSignalInformationOutputTypeDef = TypedDict(
+    "_RequiredSignalInformationOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalSignalInformationOutputTypeDef = TypedDict(
+    "_OptionalSignalInformationOutputTypeDef",
+    {
+        "maxSampleCount": int,
+        "minimumSamplingIntervalMs": int,
+    },
+    total=False,
+)
+
+class SignalInformationOutputTypeDef(
+    _RequiredSignalInformationOutputTypeDef, _OptionalSignalInformationOutputTypeDef
+):
+    pass
+
 GetDecoderManifestRequestRequestTypeDef = TypedDict(
     "GetDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -927,14 +1158,21 @@
         "campaignName": str,
         "vehicleName": str,
         "status": VehicleStateType,
     },
     total=False,
 )
 
+IamResourcesOutputTypeDef = TypedDict(
+    "IamResourcesOutputTypeDef",
+    {
+        "roleArn": str,
+    },
+)
+
 IamResourcesTypeDef = TypedDict(
     "IamResourcesTypeDef",
     {
         "roleArn": str,
     },
 )
 
@@ -1299,14 +1537,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 _RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef = TypedDict(
     "_RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
     {
         "fleetId": str,
     },
 )
 _OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef = TypedDict(
@@ -1380,14 +1626,38 @@
         "modelManifestArn": str,
         "decoderManifestArn": str,
         "creationTime": datetime,
         "lastModificationTime": datetime,
     },
 )
 
+_RequiredObdInterfaceOutputTypeDef = TypedDict(
+    "_RequiredObdInterfaceOutputTypeDef",
+    {
+        "name": str,
+        "requestMessageId": int,
+    },
+)
+_OptionalObdInterfaceOutputTypeDef = TypedDict(
+    "_OptionalObdInterfaceOutputTypeDef",
+    {
+        "obdStandard": str,
+        "pidRequestIntervalSeconds": int,
+        "dtcRequestIntervalSeconds": int,
+        "useExtendedIds": bool,
+        "hasTransmissionEcu": bool,
+    },
+    total=False,
+)
+
+class ObdInterfaceOutputTypeDef(
+    _RequiredObdInterfaceOutputTypeDef, _OptionalObdInterfaceOutputTypeDef
+):
+    pass
+
 _RequiredObdInterfaceTypeDef = TypedDict(
     "_RequiredObdInterfaceTypeDef",
     {
         "name": str,
         "requestMessageId": int,
     },
 )
@@ -1402,14 +1672,38 @@
     },
     total=False,
 )
 
 class ObdInterfaceTypeDef(_RequiredObdInterfaceTypeDef, _OptionalObdInterfaceTypeDef):
     pass
 
+_RequiredSensorOutputTypeDef = TypedDict(
+    "_RequiredSensorOutputTypeDef",
+    {
+        "fullyQualifiedName": str,
+        "dataType": NodeDataTypeType,
+    },
+)
+_OptionalSensorOutputTypeDef = TypedDict(
+    "_OptionalSensorOutputTypeDef",
+    {
+        "description": str,
+        "unit": str,
+        "allowedValues": List[str],
+        "min": float,
+        "max": float,
+        "deprecationMessage": str,
+        "comment": str,
+    },
+    total=False,
+)
+
+class SensorOutputTypeDef(_RequiredSensorOutputTypeDef, _OptionalSensorOutputTypeDef):
+    pass
+
 _RequiredSensorTypeDef = TypedDict(
     "_RequiredSensorTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -1426,14 +1720,38 @@
     },
     total=False,
 )
 
 class SensorTypeDef(_RequiredSensorTypeDef, _OptionalSensorTypeDef):
     pass
 
+_RequiredObdSignalOutputTypeDef = TypedDict(
+    "_RequiredObdSignalOutputTypeDef",
+    {
+        "pidResponseLength": int,
+        "serviceMode": int,
+        "pid": int,
+        "scaling": float,
+        "offset": float,
+        "startByte": int,
+        "byteLength": int,
+    },
+)
+_OptionalObdSignalOutputTypeDef = TypedDict(
+    "_OptionalObdSignalOutputTypeDef",
+    {
+        "bitRightShift": int,
+        "bitMaskLength": int,
+    },
+    total=False,
+)
+
+class ObdSignalOutputTypeDef(_RequiredObdSignalOutputTypeDef, _OptionalObdSignalOutputTypeDef):
+    pass
+
 _RequiredObdSignalTypeDef = TypedDict(
     "_RequiredObdSignalTypeDef",
     {
         "pidResponseLength": int,
         "serviceMode": int,
         "pid": int,
         "scaling": float,
@@ -1468,14 +1786,22 @@
     "TimestreamResourcesTypeDef",
     {
         "timestreamDatabaseName": str,
         "timestreamTableName": str,
     },
 )
 
+TimestreamResourcesOutputTypeDef = TypedDict(
+    "TimestreamResourcesOutputTypeDef",
+    {
+        "timestreamDatabaseName": str,
+        "timestreamTableName": str,
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
@@ -1672,26 +1998,35 @@
     },
     total=False,
 )
 
 GetLoggingOptionsResponseTypeDef = TypedDict(
     "GetLoggingOptionsResponseTypeDef",
     {
-        "cloudWatchLogDelivery": CloudWatchLogDeliveryOptionsTypeDef,
+        "cloudWatchLogDelivery": CloudWatchLogDeliveryOptionsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutLoggingOptionsRequestRequestTypeDef = TypedDict(
     "PutLoggingOptionsRequestRequestTypeDef",
     {
         "cloudWatchLogDelivery": CloudWatchLogDeliveryOptionsTypeDef,
     },
 )
 
+CollectionSchemeOutputTypeDef = TypedDict(
+    "CollectionSchemeOutputTypeDef",
+    {
+        "timeBasedCollectionScheme": TimeBasedCollectionSchemeOutputTypeDef,
+        "conditionBasedCollectionScheme": ConditionBasedCollectionSchemeOutputTypeDef,
+    },
+    total=False,
+)
+
 CollectionSchemeTypeDef = TypedDict(
     "CollectionSchemeTypeDef",
     {
         "timeBasedCollectionScheme": TimeBasedCollectionSchemeTypeDef,
         "conditionBasedCollectionScheme": ConditionBasedCollectionSchemeTypeDef,
     },
     total=False,
@@ -1783,30 +2118,31 @@
 )
 
 class CreateVehicleRequestRequestTypeDef(
     _RequiredCreateVehicleRequestRequestTypeDef, _OptionalCreateVehicleRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+DataDestinationConfigOutputTypeDef = TypedDict(
+    "DataDestinationConfigOutputTypeDef",
+    {
+        "s3Config": S3ConfigOutputTypeDef,
+        "timestreamConfig": TimestreamConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 DataDestinationConfigTypeDef = TypedDict(
     "DataDestinationConfigTypeDef",
     {
         "s3Config": S3ConfigTypeDef,
         "timestreamConfig": TimestreamConfigTypeDef,
     },
     total=False,
@@ -1901,23 +2237,52 @@
     {
         "summaries": List[SignalCatalogSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListVehiclesResponseTypeDef = TypedDict(
     "ListVehiclesResponseTypeDef",
     {
         "vehicleSummaries": List[VehicleSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredNetworkInterfaceOutputTypeDef = TypedDict(
+    "_RequiredNetworkInterfaceOutputTypeDef",
+    {
+        "interfaceId": str,
+        "type": NetworkInterfaceTypeType,
+    },
+)
+_OptionalNetworkInterfaceOutputTypeDef = TypedDict(
+    "_OptionalNetworkInterfaceOutputTypeDef",
+    {
+        "canInterface": CanInterfaceOutputTypeDef,
+        "obdInterface": ObdInterfaceOutputTypeDef,
+    },
+    total=False,
+)
+
+class NetworkInterfaceOutputTypeDef(
+    _RequiredNetworkInterfaceOutputTypeDef, _OptionalNetworkInterfaceOutputTypeDef
+):
+    pass
+
 _RequiredNetworkInterfaceTypeDef = TypedDict(
     "_RequiredNetworkInterfaceTypeDef",
     {
         "interfaceId": str,
         "type": NetworkInterfaceTypeType,
     },
 )
@@ -1929,25 +2294,58 @@
     },
     total=False,
 )
 
 class NetworkInterfaceTypeDef(_RequiredNetworkInterfaceTypeDef, _OptionalNetworkInterfaceTypeDef):
     pass
 
+NodeOutputTypeDef = TypedDict(
+    "NodeOutputTypeDef",
+    {
+        "branch": BranchOutputTypeDef,
+        "sensor": SensorOutputTypeDef,
+        "actuator": ActuatorOutputTypeDef,
+        "attribute": AttributeOutputTypeDef,
+    },
+    total=False,
+)
+
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "branch": BranchTypeDef,
         "sensor": SensorTypeDef,
         "actuator": ActuatorTypeDef,
         "attribute": AttributeTypeDef,
     },
     total=False,
 )
 
+_RequiredSignalDecoderOutputTypeDef = TypedDict(
+    "_RequiredSignalDecoderOutputTypeDef",
+    {
+        "fullyQualifiedName": str,
+        "type": SignalDecoderTypeType,
+        "interfaceId": str,
+    },
+)
+_OptionalSignalDecoderOutputTypeDef = TypedDict(
+    "_OptionalSignalDecoderOutputTypeDef",
+    {
+        "canSignal": CanSignalOutputTypeDef,
+        "obdSignal": ObdSignalOutputTypeDef,
+    },
+    total=False,
+)
+
+class SignalDecoderOutputTypeDef(
+    _RequiredSignalDecoderOutputTypeDef, _OptionalSignalDecoderOutputTypeDef
+):
+    pass
+
 _RequiredSignalDecoderTypeDef = TypedDict(
     "_RequiredSignalDecoderTypeDef",
     {
         "fullyQualifiedName": str,
         "type": SignalDecoderTypeType,
         "interfaceId": str,
     },
@@ -1973,16 +2371,16 @@
     total=False,
 )
 
 RegisterAccountResponseTypeDef = TypedDict(
     "RegisterAccountResponseTypeDef",
     {
         "registerAccountStatus": RegistrationStatusType,
-        "timestreamResources": TimestreamResourcesTypeDef,
-        "iamResources": IamResourcesTypeDef,
+        "timestreamResources": TimestreamResourcesOutputTypeDef,
+        "iamResources": IamResourcesOutputTypeDef,
         "creationTime": datetime,
         "lastModificationTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportDecoderManifestRequestRequestTypeDef = TypedDict(
@@ -1996,14 +2394,40 @@
 BatchCreateVehicleRequestRequestTypeDef = TypedDict(
     "BatchCreateVehicleRequestRequestTypeDef",
     {
         "vehicles": Sequence[CreateVehicleRequestItemTypeDef],
     },
 )
 
+GetCampaignResponseTypeDef = TypedDict(
+    "GetCampaignResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "description": str,
+        "signalCatalogArn": str,
+        "targetArn": str,
+        "status": CampaignStatusType,
+        "startTime": datetime,
+        "expiryTime": datetime,
+        "postTriggerCollectionDuration": int,
+        "diagnosticsMode": DiagnosticsModeType,
+        "spoolingMode": SpoolingModeType,
+        "compression": CompressionType,
+        "priority": int,
+        "signalsToCollect": List[SignalInformationOutputTypeDef],
+        "collectionScheme": CollectionSchemeOutputTypeDef,
+        "dataExtraDimensions": List[str],
+        "creationTime": datetime,
+        "lastModificationTime": datetime,
+        "dataDestinationConfigs": List[DataDestinationConfigOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateCampaignRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCampaignRequestRequestTypeDef",
     {
         "name": str,
         "signalCatalogArn": str,
         "targetArn": str,
         "collectionScheme": CollectionSchemeTypeDef,
@@ -2029,44 +2453,36 @@
 )
 
 class CreateCampaignRequestRequestTypeDef(
     _RequiredCreateCampaignRequestRequestTypeDef, _OptionalCreateCampaignRequestRequestTypeDef
 ):
     pass
 
-GetCampaignResponseTypeDef = TypedDict(
-    "GetCampaignResponseTypeDef",
+ListDecoderManifestNetworkInterfacesResponseTypeDef = TypedDict(
+    "ListDecoderManifestNetworkInterfacesResponseTypeDef",
     {
-        "name": str,
-        "arn": str,
-        "description": str,
-        "signalCatalogArn": str,
-        "targetArn": str,
-        "status": CampaignStatusType,
-        "startTime": datetime,
-        "expiryTime": datetime,
-        "postTriggerCollectionDuration": int,
-        "diagnosticsMode": DiagnosticsModeType,
-        "spoolingMode": SpoolingModeType,
-        "compression": CompressionType,
-        "priority": int,
-        "signalsToCollect": List[SignalInformationTypeDef],
-        "collectionScheme": CollectionSchemeTypeDef,
-        "dataExtraDimensions": List[str],
-        "creationTime": datetime,
-        "lastModificationTime": datetime,
-        "dataDestinationConfigs": List[DataDestinationConfigTypeDef],
+        "networkInterfaces": List[NetworkInterfaceOutputTypeDef],
+        "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDecoderManifestNetworkInterfacesResponseTypeDef = TypedDict(
-    "ListDecoderManifestNetworkInterfacesResponseTypeDef",
+ListModelManifestNodesResponseTypeDef = TypedDict(
+    "ListModelManifestNodesResponseTypeDef",
+    {
+        "nodes": List[NodeOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListSignalCatalogNodesResponseTypeDef = TypedDict(
+    "ListSignalCatalogNodesResponseTypeDef",
     {
-        "networkInterfaces": List[NetworkInterfaceTypeDef],
+        "nodes": List[NodeOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateSignalCatalogRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSignalCatalogRequestRequestTypeDef",
@@ -2086,32 +2502,14 @@
 
 class CreateSignalCatalogRequestRequestTypeDef(
     _RequiredCreateSignalCatalogRequestRequestTypeDef,
     _OptionalCreateSignalCatalogRequestRequestTypeDef,
 ):
     pass
 
-ListModelManifestNodesResponseTypeDef = TypedDict(
-    "ListModelManifestNodesResponseTypeDef",
-    {
-        "nodes": List[NodeTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSignalCatalogNodesResponseTypeDef = TypedDict(
-    "ListSignalCatalogNodesResponseTypeDef",
-    {
-        "nodes": List[NodeTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSignalCatalogRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
@@ -2127,14 +2525,23 @@
 
 class UpdateSignalCatalogRequestRequestTypeDef(
     _RequiredUpdateSignalCatalogRequestRequestTypeDef,
     _OptionalUpdateSignalCatalogRequestRequestTypeDef,
 ):
     pass
 
+ListDecoderManifestSignalsResponseTypeDef = TypedDict(
+    "ListDecoderManifestSignalsResponseTypeDef",
+    {
+        "signalDecoders": List[SignalDecoderOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateDecoderManifestRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
         "modelManifestArn": str,
     },
 )
@@ -2151,23 +2558,14 @@
 
 class CreateDecoderManifestRequestRequestTypeDef(
     _RequiredCreateDecoderManifestRequestRequestTypeDef,
     _OptionalCreateDecoderManifestRequestRequestTypeDef,
 ):
     pass
 
-ListDecoderManifestSignalsResponseTypeDef = TypedDict(
-    "ListDecoderManifestSignalsResponseTypeDef",
-    {
-        "signalDecoders": List[SignalDecoderTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateDecoderManifestRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateDecoderManifestRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise.egg-info/PKG-INFO` & `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotfleetwise
-Version: 1.28.0
-Summary: Type annotations for boto3.IoTFleetWise 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTFleetWise 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iotfleetwise"></a>
 
 # mypy-boto3-iotfleetwise
 
 [![PyPI - mypy-boto3-iotfleetwise](https://img.shields.io/pypi/v/mypy-boto3-iotfleetwise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleetwise)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleetwise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotfleetwise?color=blue)](https://pypistats.org/packages/mypy-boto3-iotfleetwise)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotfleetwise)](https://pepy.tech/project/mypy-boto3-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetWise 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
+[boto3.IoTFleetWise 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
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
 [mypy-boto3-iotfleetwise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/).
 
 See how it helps to find and fix potential bugs:
 
@@ -392,38 +392,48 @@
 ### Typed dictionaries
 
 `mypy_boto3_iotfleetwise.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotfleetwise.type_defs import (
+    ActuatorOutputTypeDef,
     ActuatorTypeDef,
     AssociateVehicleFleetRequestRequestTypeDef,
+    AttributeOutputTypeDef,
     AttributeTypeDef,
     CreateVehicleErrorTypeDef,
     CreateVehicleResponseItemTypeDef,
     UpdateVehicleRequestItemTypeDef,
     UpdateVehicleErrorTypeDef,
     UpdateVehicleResponseItemTypeDef,
+    BranchOutputTypeDef,
     BranchTypeDef,
     CampaignSummaryTypeDef,
     CanDbcDefinitionTypeDef,
+    CanInterfaceOutputTypeDef,
     CanInterfaceTypeDef,
+    CanSignalOutputTypeDef,
     CanSignalTypeDef,
+    CloudWatchLogDeliveryOptionsOutputTypeDef,
     CloudWatchLogDeliveryOptionsTypeDef,
+    ConditionBasedCollectionSchemeOutputTypeDef,
+    TimeBasedCollectionSchemeOutputTypeDef,
     ConditionBasedCollectionSchemeTypeDef,
     TimeBasedCollectionSchemeTypeDef,
     SignalInformationTypeDef,
     TagTypeDef,
     CreateCampaignResponseTypeDef,
     CreateDecoderManifestResponseTypeDef,
     CreateFleetResponseTypeDef,
     CreateModelManifestResponseTypeDef,
     CreateSignalCatalogResponseTypeDef,
     CreateVehicleResponseTypeDef,
+    S3ConfigOutputTypeDef,
+    TimestreamConfigOutputTypeDef,
     S3ConfigTypeDef,
     TimestreamConfigTypeDef,
     DecoderManifestSummaryTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteCampaignResponseTypeDef,
     DeleteDecoderManifestRequestRequestTypeDef,
     DeleteDecoderManifestResponseTypeDef,
@@ -435,14 +445,15 @@
     DeleteSignalCatalogResponseTypeDef,
     DeleteVehicleRequestRequestTypeDef,
     DeleteVehicleResponseTypeDef,
     DisassociateVehicleFleetRequestRequestTypeDef,
     FleetSummaryTypeDef,
     FormattedVssTypeDef,
     GetCampaignRequestRequestTypeDef,
+    SignalInformationOutputTypeDef,
     GetDecoderManifestRequestRequestTypeDef,
     GetDecoderManifestResponseTypeDef,
     GetFleetRequestRequestTypeDef,
     GetFleetResponseTypeDef,
     GetModelManifestRequestRequestTypeDef,
     GetModelManifestResponseTypeDef,
     IamRegistrationResponseTypeDef,
@@ -450,14 +461,15 @@
     GetSignalCatalogRequestRequestTypeDef,
     NodeCountsTypeDef,
     GetVehicleRequestRequestTypeDef,
     GetVehicleResponseTypeDef,
     GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
     GetVehicleStatusRequestRequestTypeDef,
     VehicleStatusTypeDef,
+    IamResourcesOutputTypeDef,
     IamResourcesTypeDef,
     ImportDecoderManifestResponseTypeDef,
     ImportSignalCatalogResponseTypeDef,
     ListCampaignsRequestListCampaignsPaginateTypeDef,
     ListCampaignsRequestRequestTypeDef,
     ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
     ListDecoderManifestNetworkInterfacesRequestRequestTypeDef,
@@ -477,25 +489,30 @@
     ModelManifestSummaryTypeDef,
     ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
     ListSignalCatalogNodesRequestRequestTypeDef,
     ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef,
     ListSignalCatalogsRequestRequestTypeDef,
     SignalCatalogSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
     ListVehiclesInFleetRequestRequestTypeDef,
     ListVehiclesInFleetResponseTypeDef,
     ListVehiclesRequestListVehiclesPaginateTypeDef,
     ListVehiclesRequestRequestTypeDef,
     VehicleSummaryTypeDef,
+    ObdInterfaceOutputTypeDef,
     ObdInterfaceTypeDef,
+    SensorOutputTypeDef,
     SensorTypeDef,
+    ObdSignalOutputTypeDef,
     ObdSignalTypeDef,
     PaginatorConfigTypeDef,
     TimestreamResourcesTypeDef,
+    TimestreamResourcesOutputTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignRequestRequestTypeDef,
     UpdateCampaignResponseTypeDef,
     UpdateDecoderManifestResponseTypeDef,
     UpdateFleetRequestRequestTypeDef,
     UpdateFleetResponseTypeDef,
@@ -507,52 +524,57 @@
     BatchCreateVehicleResponseTypeDef,
     BatchUpdateVehicleRequestRequestTypeDef,
     BatchUpdateVehicleResponseTypeDef,
     ListCampaignsResponseTypeDef,
     NetworkFileDefinitionTypeDef,
     GetLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
+    CollectionSchemeOutputTypeDef,
     CollectionSchemeTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateModelManifestRequestRequestTypeDef,
     CreateVehicleRequestItemTypeDef,
     CreateVehicleRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    DataDestinationConfigOutputTypeDef,
     DataDestinationConfigTypeDef,
     ListDecoderManifestsResponseTypeDef,
     ListFleetsResponseTypeDef,
     ImportSignalCatalogRequestRequestTypeDef,
     GetRegisterAccountStatusResponseTypeDef,
     GetSignalCatalogResponseTypeDef,
     GetVehicleStatusResponseTypeDef,
     ListModelManifestsResponseTypeDef,
     ListSignalCatalogsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVehiclesResponseTypeDef,
+    NetworkInterfaceOutputTypeDef,
     NetworkInterfaceTypeDef,
+    NodeOutputTypeDef,
     NodeTypeDef,
+    SignalDecoderOutputTypeDef,
     SignalDecoderTypeDef,
     RegisterAccountRequestRequestTypeDef,
     RegisterAccountResponseTypeDef,
     ImportDecoderManifestRequestRequestTypeDef,
     BatchCreateVehicleRequestRequestTypeDef,
-    CreateCampaignRequestRequestTypeDef,
     GetCampaignResponseTypeDef,
+    CreateCampaignRequestRequestTypeDef,
     ListDecoderManifestNetworkInterfacesResponseTypeDef,
-    CreateSignalCatalogRequestRequestTypeDef,
     ListModelManifestNodesResponseTypeDef,
     ListSignalCatalogNodesResponseTypeDef,
+    CreateSignalCatalogRequestRequestTypeDef,
     UpdateSignalCatalogRequestRequestTypeDef,
-    CreateDecoderManifestRequestRequestTypeDef,
     ListDecoderManifestSignalsResponseTypeDef,
+    CreateDecoderManifestRequestRequestTypeDef,
     UpdateDecoderManifestRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActuatorTypeDef:
+def get_structure() -> ActuatorOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotfleetwise-1.28.0/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt` & `mypy-boto3-iotfleetwise-1.28.12/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.0/setup.py` & `mypy-boto3-iotfleetwise-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotfleetwise",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_iotfleetwise"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTFleetWise 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.IoTFleetWise 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

