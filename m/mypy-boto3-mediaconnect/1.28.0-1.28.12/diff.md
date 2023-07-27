# Comparing `tmp/mypy-boto3-mediaconnect-1.28.0.tar.gz` & `tmp/mypy-boto3-mediaconnect-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediaconnect-1.28.0.tar", last modified: Thu Jul  6 21:00:04 2023, max compression
+gzip compressed data, was "mypy-boto3-mediaconnect-1.28.12.tar", last modified: Thu Jul 27 05:35:00 2023, max compression
```

## Comparing `mypy-boto3-mediaconnect-1.28.0.tar` & `mypy-boto3-mediaconnect-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:04.714364 mypy-boto3-mediaconnect-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:46:40.000000 mypy-boto3-mediaconnect-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22056 2023-07-06 21:00:04.714364 mypy-boto3-mediaconnect-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20551 2023-07-06 20:46:40.000000 mypy-boto3-mediaconnect-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:04.706364 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-06 20:46:40.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-06 20:46:40.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:46:40.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40366 2023-07-06 20:46:41.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40299 2023-07-06 20:46:41.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-07-06 20:46:41.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-07-06 20:46:41.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-07-06 20:46:41.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-06 20:46:41.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:46:40.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    65058 2023-07-06 20:46:45.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    64967 2023-07-06 20:46:42.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:46:40.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-06 20:46:41.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-06 20:46:41.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:04.714364 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22056 2023-07-06 21:00:04.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-06 21:00:04.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:04.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:04.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:04.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 21:00:04.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:04.714364 mypy-boto3-mediaconnect-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:46:40.000000 mypy-boto3-mediaconnect-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.140444 mypy-boto3-mediaconnect-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22212 2023-07-27 05:35:00.140444 mypy-boto3-mediaconnect-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20705 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.136444 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40366 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40299 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-07-27 05:25:56.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-07-27 05:25:56.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    66581 2023-07-27 05:25:57.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66488 2023-07-27 05:25:57.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.140444 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22212 2023-07-27 05:34:59.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-27 05:35:00.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:59.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:59.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:59.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:59.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:00.144444 mypy-boto3-mediaconnect-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/setup.py
```

### Comparing `mypy-boto3-mediaconnect-1.28.0/LICENSE` & `mypy-boto3-mediaconnect-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.28.0/PKG-INFO` & `mypy-boto3-mediaconnect-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediaconnect
-Version: 1.28.0
-Summary: Type annotations for boto3.MediaConnect 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MediaConnect 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mediaconnect"></a>
 
 # mypy-boto3-mediaconnect
 
 [![PyPI - mypy-boto3-mediaconnect](https://img.shields.io/pypi/v/mypy-boto3-mediaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconnect?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconnect)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediaconnect)](https://pepy.tech/project/mypy-boto3-mediaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConnect 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
+[boto3.MediaConnect 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
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
 [mypy-boto3-mediaconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -405,14 +405,15 @@
     AddEgressGatewayBridgeRequestTypeDef,
     VpcInterfaceRequestTypeDef,
     VpcInterfaceTypeDef,
     AddIngressGatewayBridgeRequestTypeDef,
     AddMaintenanceTypeDef,
     EncryptionTypeDef,
     BridgeFlowOutputTypeDef,
+    VpcInterfaceAttachmentOutputTypeDef,
     BridgeNetworkOutputTypeDef,
     BridgeNetworkSourceTypeDef,
     EgressGatewayBridgeTypeDef,
     IngressGatewayBridgeTypeDef,
     MessageDetailTypeDef,
     GatewayNetworkTypeDef,
     DeleteBridgeRequestRequestTypeDef,
@@ -432,18 +433,21 @@
     DescribeOfferingRequestRequestTypeDef,
     DescribeReservationRequestRequestTypeDef,
     InterfaceRequestTypeDef,
     InterfaceTypeDef,
     EmptyResponseMetadataTypeDef,
     EncodingParametersRequestTypeDef,
     EncodingParametersTypeDef,
+    EncryptionOutputTypeDef,
+    SourcePriorityOutputTypeDef,
     SourcePriorityTypeDef,
     MaintenanceTypeDef,
     FmtpRequestTypeDef,
     FmtpTypeDef,
+    GatewayNetworkOutputTypeDef,
     ListBridgesRequestListBridgesPaginateTypeDef,
     ListBridgesRequestRequestTypeDef,
     ListedBridgeTypeDef,
     ListEntitlementsRequestListEntitlementsPaginateTypeDef,
     ListEntitlementsRequestRequestTypeDef,
     ListedEntitlementTypeDef,
     ListFlowsRequestListFlowsPaginateTypeDef,
@@ -492,70 +496,71 @@
     UpdateBridgeStateRequestRequestTypeDef,
     UpdateBridgeStateResponseTypeDef,
     UpdateEncryptionTypeDef,
     UpdateMaintenanceTypeDef,
     UpdateGatewayInstanceRequestRequestTypeDef,
     UpdateGatewayInstanceResponseTypeDef,
     AddBridgeFlowSourceRequestTypeDef,
-    BridgeFlowSourceTypeDef,
-    GatewayBridgeSourceTypeDef,
     SetGatewayBridgeSourceRequestTypeDef,
     UpdateBridgeFlowSourceRequestTypeDef,
     UpdateGatewayBridgeSourceRequestTypeDef,
     AddBridgeOutputRequestTypeDef,
     AddFlowVpcInterfacesRequestRequestTypeDef,
     AddFlowVpcInterfacesResponseTypeDef,
-    EntitlementTypeDef,
     GrantEntitlementRequestTypeDef,
+    BridgeFlowSourceTypeDef,
+    GatewayBridgeSourceTypeDef,
     BridgeOutputTypeDef,
     GatewayInstanceTypeDef,
     CreateGatewayRequestRequestTypeDef,
-    GatewayTypeDef,
     DescribeFlowRequestFlowActiveWaitTypeDef,
     DescribeFlowRequestFlowDeletedWaitTypeDef,
     DescribeFlowRequestFlowStandbyWaitTypeDef,
     DestinationConfigurationRequestTypeDef,
     InputConfigurationRequestTypeDef,
     DestinationConfigurationTypeDef,
     InputConfigurationTypeDef,
+    EntitlementTypeDef,
+    FailoverConfigOutputTypeDef,
     FailoverConfigTypeDef,
     UpdateFailoverConfigTypeDef,
     ListedFlowTypeDef,
     MediaStreamAttributesRequestTypeDef,
     MediaStreamAttributesTypeDef,
+    GatewayTypeDef,
     ListBridgesResponseTypeDef,
     ListEntitlementsResponseTypeDef,
     ListGatewayInstancesResponseTypeDef,
     ListGatewaysResponseTypeDef,
     OfferingTypeDef,
     ReservationTypeDef,
     UpdateBridgeOutputRequestRequestTypeDef,
     UpdateFlowEntitlementRequestRequestTypeDef,
     AddBridgeSourceRequestTypeDef,
-    BridgeSourceTypeDef,
     UpdateBridgeSourceRequestRequestTypeDef,
     AddBridgeOutputsRequestRequestTypeDef,
-    GrantFlowEntitlementsResponseTypeDef,
-    UpdateFlowEntitlementResponseTypeDef,
     GrantFlowEntitlementsRequestRequestTypeDef,
+    BridgeSourceTypeDef,
     AddBridgeOutputsResponseTypeDef,
     UpdateBridgeOutputResponseTypeDef,
     DescribeGatewayInstanceResponseTypeDef,
-    CreateGatewayResponseTypeDef,
-    DescribeGatewayResponseTypeDef,
     MediaStreamOutputConfigurationRequestTypeDef,
     MediaStreamSourceConfigurationRequestTypeDef,
     MediaStreamOutputConfigurationTypeDef,
     MediaStreamSourceConfigurationTypeDef,
+    GrantFlowEntitlementsResponseTypeDef,
+    UpdateFlowEntitlementResponseTypeDef,
     UpdateBridgeRequestRequestTypeDef,
     UpdateFlowRequestRequestTypeDef,
     ListFlowsResponseTypeDef,
     AddMediaStreamRequestTypeDef,
     UpdateFlowMediaStreamRequestRequestTypeDef,
     MediaStreamTypeDef,
+    CreateGatewayResponseTypeDef,
+    DescribeGatewayResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     ListOfferingsResponseTypeDef,
     DescribeReservationResponseTypeDef,
     ListReservationsResponseTypeDef,
     PurchaseOfferingResponseTypeDef,
     AddBridgeSourcesRequestRequestTypeDef,
     CreateBridgeRequestRequestTypeDef,
```

### Comparing `mypy-boto3-mediaconnect-1.28.0/README.md` & `mypy-boto3-mediaconnect-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-mediaconnect"></a>
 
 # mypy-boto3-mediaconnect
 
 [![PyPI - mypy-boto3-mediaconnect](https://img.shields.io/pypi/v/mypy-boto3-mediaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconnect?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconnect)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediaconnect)](https://pepy.tech/project/mypy-boto3-mediaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConnect 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
+[boto3.MediaConnect 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
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
 [mypy-boto3-mediaconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -373,14 +373,15 @@
     AddEgressGatewayBridgeRequestTypeDef,
     VpcInterfaceRequestTypeDef,
     VpcInterfaceTypeDef,
     AddIngressGatewayBridgeRequestTypeDef,
     AddMaintenanceTypeDef,
     EncryptionTypeDef,
     BridgeFlowOutputTypeDef,
+    VpcInterfaceAttachmentOutputTypeDef,
     BridgeNetworkOutputTypeDef,
     BridgeNetworkSourceTypeDef,
     EgressGatewayBridgeTypeDef,
     IngressGatewayBridgeTypeDef,
     MessageDetailTypeDef,
     GatewayNetworkTypeDef,
     DeleteBridgeRequestRequestTypeDef,
@@ -400,18 +401,21 @@
     DescribeOfferingRequestRequestTypeDef,
     DescribeReservationRequestRequestTypeDef,
     InterfaceRequestTypeDef,
     InterfaceTypeDef,
     EmptyResponseMetadataTypeDef,
     EncodingParametersRequestTypeDef,
     EncodingParametersTypeDef,
+    EncryptionOutputTypeDef,
+    SourcePriorityOutputTypeDef,
     SourcePriorityTypeDef,
     MaintenanceTypeDef,
     FmtpRequestTypeDef,
     FmtpTypeDef,
+    GatewayNetworkOutputTypeDef,
     ListBridgesRequestListBridgesPaginateTypeDef,
     ListBridgesRequestRequestTypeDef,
     ListedBridgeTypeDef,
     ListEntitlementsRequestListEntitlementsPaginateTypeDef,
     ListEntitlementsRequestRequestTypeDef,
     ListedEntitlementTypeDef,
     ListFlowsRequestListFlowsPaginateTypeDef,
@@ -460,70 +464,71 @@
     UpdateBridgeStateRequestRequestTypeDef,
     UpdateBridgeStateResponseTypeDef,
     UpdateEncryptionTypeDef,
     UpdateMaintenanceTypeDef,
     UpdateGatewayInstanceRequestRequestTypeDef,
     UpdateGatewayInstanceResponseTypeDef,
     AddBridgeFlowSourceRequestTypeDef,
-    BridgeFlowSourceTypeDef,
-    GatewayBridgeSourceTypeDef,
     SetGatewayBridgeSourceRequestTypeDef,
     UpdateBridgeFlowSourceRequestTypeDef,
     UpdateGatewayBridgeSourceRequestTypeDef,
     AddBridgeOutputRequestTypeDef,
     AddFlowVpcInterfacesRequestRequestTypeDef,
     AddFlowVpcInterfacesResponseTypeDef,
-    EntitlementTypeDef,
     GrantEntitlementRequestTypeDef,
+    BridgeFlowSourceTypeDef,
+    GatewayBridgeSourceTypeDef,
     BridgeOutputTypeDef,
     GatewayInstanceTypeDef,
     CreateGatewayRequestRequestTypeDef,
-    GatewayTypeDef,
     DescribeFlowRequestFlowActiveWaitTypeDef,
     DescribeFlowRequestFlowDeletedWaitTypeDef,
     DescribeFlowRequestFlowStandbyWaitTypeDef,
     DestinationConfigurationRequestTypeDef,
     InputConfigurationRequestTypeDef,
     DestinationConfigurationTypeDef,
     InputConfigurationTypeDef,
+    EntitlementTypeDef,
+    FailoverConfigOutputTypeDef,
     FailoverConfigTypeDef,
     UpdateFailoverConfigTypeDef,
     ListedFlowTypeDef,
     MediaStreamAttributesRequestTypeDef,
     MediaStreamAttributesTypeDef,
+    GatewayTypeDef,
     ListBridgesResponseTypeDef,
     ListEntitlementsResponseTypeDef,
     ListGatewayInstancesResponseTypeDef,
     ListGatewaysResponseTypeDef,
     OfferingTypeDef,
     ReservationTypeDef,
     UpdateBridgeOutputRequestRequestTypeDef,
     UpdateFlowEntitlementRequestRequestTypeDef,
     AddBridgeSourceRequestTypeDef,
-    BridgeSourceTypeDef,
     UpdateBridgeSourceRequestRequestTypeDef,
     AddBridgeOutputsRequestRequestTypeDef,
-    GrantFlowEntitlementsResponseTypeDef,
-    UpdateFlowEntitlementResponseTypeDef,
     GrantFlowEntitlementsRequestRequestTypeDef,
+    BridgeSourceTypeDef,
     AddBridgeOutputsResponseTypeDef,
     UpdateBridgeOutputResponseTypeDef,
     DescribeGatewayInstanceResponseTypeDef,
-    CreateGatewayResponseTypeDef,
-    DescribeGatewayResponseTypeDef,
     MediaStreamOutputConfigurationRequestTypeDef,
     MediaStreamSourceConfigurationRequestTypeDef,
     MediaStreamOutputConfigurationTypeDef,
     MediaStreamSourceConfigurationTypeDef,
+    GrantFlowEntitlementsResponseTypeDef,
+    UpdateFlowEntitlementResponseTypeDef,
     UpdateBridgeRequestRequestTypeDef,
     UpdateFlowRequestRequestTypeDef,
     ListFlowsResponseTypeDef,
     AddMediaStreamRequestTypeDef,
     UpdateFlowMediaStreamRequestRequestTypeDef,
     MediaStreamTypeDef,
+    CreateGatewayResponseTypeDef,
+    DescribeGatewayResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     ListOfferingsResponseTypeDef,
     DescribeReservationResponseTypeDef,
     ListReservationsResponseTypeDef,
     PurchaseOfferingResponseTypeDef,
     AddBridgeSourcesRequestRequestTypeDef,
     CreateBridgeRequestRequestTypeDef,
```

### Comparing `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/__init__.py` & `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/__init__.pyi` & `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/__main__.py` & `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaConnect 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.MediaConnect 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect\nOther"
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

### Comparing `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/client.py` & `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/client.pyi` & `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/literals.py` & `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/literals.pyi`

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
     "AlgorithmType",
     "BridgePlacementType",
     "BridgeStateType",
     "ColorimetryType",
     "ConnectionStatusType",
     "DesiredStateType",
@@ -61,15 +60,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AlgorithmType = Literal["aes128", "aes192", "aes256"]
 BridgePlacementType = Literal["AVAILABLE", "LOCKED"]
 BridgeStateType = Literal[
     "ACTIVE",
     "CREATING",
     "DELETED",
     "DELETING",
@@ -255,14 +253,15 @@
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
@@ -341,26 +340,28 @@
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
@@ -515,14 +516,15 @@
 ]
 WaiterName = Literal["flow_active", "flow_deleted", "flow_standby"]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
+    "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
```

### Comparing `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/literals.pyi` & `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/literals.py`

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
     "AlgorithmType",
     "BridgePlacementType",
     "BridgeStateType",
     "ColorimetryType",
     "ConnectionStatusType",
     "DesiredStateType",
@@ -60,14 +61,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 AlgorithmType = Literal["aes128", "aes192", "aes256"]
 BridgePlacementType = Literal["AVAILABLE", "LOCKED"]
 BridgeStateType = Literal[
     "ACTIVE",
     "CREATING",
     "DELETED",
     "DELETING",
@@ -253,14 +255,15 @@
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
@@ -339,26 +342,28 @@
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
@@ -513,14 +518,15 @@
 ]
 WaiterName = Literal["flow_active", "flow_deleted", "flow_standby"]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
+    "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
```

### Comparing `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/paginator.py` & `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/paginator.pyi` & `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/type_defs.py` & `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     "AddEgressGatewayBridgeRequestTypeDef",
     "VpcInterfaceRequestTypeDef",
     "VpcInterfaceTypeDef",
     "AddIngressGatewayBridgeRequestTypeDef",
     "AddMaintenanceTypeDef",
     "EncryptionTypeDef",
     "BridgeFlowOutputTypeDef",
+    "VpcInterfaceAttachmentOutputTypeDef",
     "BridgeNetworkOutputTypeDef",
     "BridgeNetworkSourceTypeDef",
     "EgressGatewayBridgeTypeDef",
     "IngressGatewayBridgeTypeDef",
     "MessageDetailTypeDef",
     "GatewayNetworkTypeDef",
     "DeleteBridgeRequestRequestTypeDef",
@@ -85,18 +86,21 @@
     "DescribeOfferingRequestRequestTypeDef",
     "DescribeReservationRequestRequestTypeDef",
     "InterfaceRequestTypeDef",
     "InterfaceTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EncodingParametersRequestTypeDef",
     "EncodingParametersTypeDef",
+    "EncryptionOutputTypeDef",
+    "SourcePriorityOutputTypeDef",
     "SourcePriorityTypeDef",
     "MaintenanceTypeDef",
     "FmtpRequestTypeDef",
     "FmtpTypeDef",
+    "GatewayNetworkOutputTypeDef",
     "ListBridgesRequestListBridgesPaginateTypeDef",
     "ListBridgesRequestRequestTypeDef",
     "ListedBridgeTypeDef",
     "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
     "ListEntitlementsRequestRequestTypeDef",
     "ListedEntitlementTypeDef",
     "ListFlowsRequestListFlowsPaginateTypeDef",
@@ -145,70 +149,71 @@
     "UpdateBridgeStateRequestRequestTypeDef",
     "UpdateBridgeStateResponseTypeDef",
     "UpdateEncryptionTypeDef",
     "UpdateMaintenanceTypeDef",
     "UpdateGatewayInstanceRequestRequestTypeDef",
     "UpdateGatewayInstanceResponseTypeDef",
     "AddBridgeFlowSourceRequestTypeDef",
-    "BridgeFlowSourceTypeDef",
-    "GatewayBridgeSourceTypeDef",
     "SetGatewayBridgeSourceRequestTypeDef",
     "UpdateBridgeFlowSourceRequestTypeDef",
     "UpdateGatewayBridgeSourceRequestTypeDef",
     "AddBridgeOutputRequestTypeDef",
     "AddFlowVpcInterfacesRequestRequestTypeDef",
     "AddFlowVpcInterfacesResponseTypeDef",
-    "EntitlementTypeDef",
     "GrantEntitlementRequestTypeDef",
+    "BridgeFlowSourceTypeDef",
+    "GatewayBridgeSourceTypeDef",
     "BridgeOutputTypeDef",
     "GatewayInstanceTypeDef",
     "CreateGatewayRequestRequestTypeDef",
-    "GatewayTypeDef",
     "DescribeFlowRequestFlowActiveWaitTypeDef",
     "DescribeFlowRequestFlowDeletedWaitTypeDef",
     "DescribeFlowRequestFlowStandbyWaitTypeDef",
     "DestinationConfigurationRequestTypeDef",
     "InputConfigurationRequestTypeDef",
     "DestinationConfigurationTypeDef",
     "InputConfigurationTypeDef",
+    "EntitlementTypeDef",
+    "FailoverConfigOutputTypeDef",
     "FailoverConfigTypeDef",
     "UpdateFailoverConfigTypeDef",
     "ListedFlowTypeDef",
     "MediaStreamAttributesRequestTypeDef",
     "MediaStreamAttributesTypeDef",
+    "GatewayTypeDef",
     "ListBridgesResponseTypeDef",
     "ListEntitlementsResponseTypeDef",
     "ListGatewayInstancesResponseTypeDef",
     "ListGatewaysResponseTypeDef",
     "OfferingTypeDef",
     "ReservationTypeDef",
     "UpdateBridgeOutputRequestRequestTypeDef",
     "UpdateFlowEntitlementRequestRequestTypeDef",
     "AddBridgeSourceRequestTypeDef",
-    "BridgeSourceTypeDef",
     "UpdateBridgeSourceRequestRequestTypeDef",
     "AddBridgeOutputsRequestRequestTypeDef",
-    "GrantFlowEntitlementsResponseTypeDef",
-    "UpdateFlowEntitlementResponseTypeDef",
     "GrantFlowEntitlementsRequestRequestTypeDef",
+    "BridgeSourceTypeDef",
     "AddBridgeOutputsResponseTypeDef",
     "UpdateBridgeOutputResponseTypeDef",
     "DescribeGatewayInstanceResponseTypeDef",
-    "CreateGatewayResponseTypeDef",
-    "DescribeGatewayResponseTypeDef",
     "MediaStreamOutputConfigurationRequestTypeDef",
     "MediaStreamSourceConfigurationRequestTypeDef",
     "MediaStreamOutputConfigurationTypeDef",
     "MediaStreamSourceConfigurationTypeDef",
+    "GrantFlowEntitlementsResponseTypeDef",
+    "UpdateFlowEntitlementResponseTypeDef",
     "UpdateBridgeRequestRequestTypeDef",
     "UpdateFlowRequestRequestTypeDef",
     "ListFlowsResponseTypeDef",
     "AddMediaStreamRequestTypeDef",
     "UpdateFlowMediaStreamRequestRequestTypeDef",
     "MediaStreamTypeDef",
+    "CreateGatewayResponseTypeDef",
+    "DescribeGatewayResponseTypeDef",
     "DescribeOfferingResponseTypeDef",
     "ListOfferingsResponseTypeDef",
     "DescribeReservationResponseTypeDef",
     "ListReservationsResponseTypeDef",
     "PurchaseOfferingResponseTypeDef",
     "AddBridgeSourcesRequestRequestTypeDef",
     "CreateBridgeRequestRequestTypeDef",
@@ -361,14 +366,22 @@
     {
         "FlowArn": str,
         "FlowSourceArn": str,
         "Name": str,
     },
 )
 
+VpcInterfaceAttachmentOutputTypeDef = TypedDict(
+    "VpcInterfaceAttachmentOutputTypeDef",
+    {
+        "VpcInterfaceName": str,
+    },
+    total=False,
+)
+
 BridgeNetworkOutputTypeDef = TypedDict(
     "BridgeNetworkOutputTypeDef",
     {
         "IpAddress": str,
         "Name": str,
         "NetworkName": str,
         "Port": int,
@@ -627,14 +640,48 @@
     "EncodingParametersTypeDef",
     {
         "CompressionFactor": float,
         "EncoderProfile": EncoderProfileType,
     },
 )
 
+_RequiredEncryptionOutputTypeDef = TypedDict(
+    "_RequiredEncryptionOutputTypeDef",
+    {
+        "RoleArn": str,
+    },
+)
+_OptionalEncryptionOutputTypeDef = TypedDict(
+    "_OptionalEncryptionOutputTypeDef",
+    {
+        "Algorithm": AlgorithmType,
+        "ConstantInitializationVector": str,
+        "DeviceId": str,
+        "KeyType": KeyTypeType,
+        "Region": str,
+        "ResourceId": str,
+        "SecretArn": str,
+        "Url": str,
+    },
+    total=False,
+)
+
+
+class EncryptionOutputTypeDef(_RequiredEncryptionOutputTypeDef, _OptionalEncryptionOutputTypeDef):
+    pass
+
+
+SourcePriorityOutputTypeDef = TypedDict(
+    "SourcePriorityOutputTypeDef",
+    {
+        "PrimarySource": str,
+    },
+    total=False,
+)
+
 SourcePriorityTypeDef = TypedDict(
     "SourcePriorityTypeDef",
     {
         "PrimarySource": str,
     },
     total=False,
 )
@@ -674,14 +721,22 @@
         "Range": RangeType,
         "ScanMode": ScanModeType,
         "Tcs": TcsType,
     },
     total=False,
 )
 
+GatewayNetworkOutputTypeDef = TypedDict(
+    "GatewayNetworkOutputTypeDef",
+    {
+        "CidrBlock": str,
+        "Name": str,
+    },
+)
+
 ListBridgesRequestListBridgesPaginateTypeDef = TypedDict(
     "ListBridgesRequestListBridgesPaginateTypeDef",
     {
         "FilterArn": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1262,56 +1317,14 @@
 
 class AddBridgeFlowSourceRequestTypeDef(
     _RequiredAddBridgeFlowSourceRequestTypeDef, _OptionalAddBridgeFlowSourceRequestTypeDef
 ):
     pass
 
 
-_RequiredBridgeFlowSourceTypeDef = TypedDict(
-    "_RequiredBridgeFlowSourceTypeDef",
-    {
-        "FlowArn": str,
-        "Name": str,
-    },
-)
-_OptionalBridgeFlowSourceTypeDef = TypedDict(
-    "_OptionalBridgeFlowSourceTypeDef",
-    {
-        "FlowVpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
-        "OutputArn": str,
-    },
-    total=False,
-)
-
-
-class BridgeFlowSourceTypeDef(_RequiredBridgeFlowSourceTypeDef, _OptionalBridgeFlowSourceTypeDef):
-    pass
-
-
-_RequiredGatewayBridgeSourceTypeDef = TypedDict(
-    "_RequiredGatewayBridgeSourceTypeDef",
-    {
-        "BridgeArn": str,
-    },
-)
-_OptionalGatewayBridgeSourceTypeDef = TypedDict(
-    "_OptionalGatewayBridgeSourceTypeDef",
-    {
-        "VpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
-    },
-    total=False,
-)
-
-
-class GatewayBridgeSourceTypeDef(
-    _RequiredGatewayBridgeSourceTypeDef, _OptionalGatewayBridgeSourceTypeDef
-):
-    pass
-
-
 _RequiredSetGatewayBridgeSourceRequestTypeDef = TypedDict(
     "_RequiredSetGatewayBridgeSourceRequestTypeDef",
     {
         "BridgeArn": str,
     },
 )
 _OptionalSetGatewayBridgeSourceRequestTypeDef = TypedDict(
@@ -1368,59 +1381,77 @@
     {
         "FlowArn": str,
         "VpcInterfaces": List[VpcInterfaceTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredEntitlementTypeDef = TypedDict(
-    "_RequiredEntitlementTypeDef",
+_RequiredGrantEntitlementRequestTypeDef = TypedDict(
+    "_RequiredGrantEntitlementRequestTypeDef",
     {
-        "EntitlementArn": str,
-        "Name": str,
-        "Subscribers": List[str],
+        "Subscribers": Sequence[str],
     },
 )
-_OptionalEntitlementTypeDef = TypedDict(
-    "_OptionalEntitlementTypeDef",
+_OptionalGrantEntitlementRequestTypeDef = TypedDict(
+    "_OptionalGrantEntitlementRequestTypeDef",
     {
         "DataTransferSubscriberFeePercent": int,
         "Description": str,
         "Encryption": EncryptionTypeDef,
         "EntitlementStatus": EntitlementStatusType,
+        "Name": str,
     },
     total=False,
 )
 
 
-class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
+class GrantEntitlementRequestTypeDef(
+    _RequiredGrantEntitlementRequestTypeDef, _OptionalGrantEntitlementRequestTypeDef
+):
     pass
 
 
-_RequiredGrantEntitlementRequestTypeDef = TypedDict(
-    "_RequiredGrantEntitlementRequestTypeDef",
+_RequiredBridgeFlowSourceTypeDef = TypedDict(
+    "_RequiredBridgeFlowSourceTypeDef",
     {
-        "Subscribers": Sequence[str],
+        "FlowArn": str,
+        "Name": str,
     },
 )
-_OptionalGrantEntitlementRequestTypeDef = TypedDict(
-    "_OptionalGrantEntitlementRequestTypeDef",
+_OptionalBridgeFlowSourceTypeDef = TypedDict(
+    "_OptionalBridgeFlowSourceTypeDef",
     {
-        "DataTransferSubscriberFeePercent": int,
-        "Description": str,
-        "Encryption": EncryptionTypeDef,
-        "EntitlementStatus": EntitlementStatusType,
-        "Name": str,
+        "FlowVpcInterfaceAttachment": VpcInterfaceAttachmentOutputTypeDef,
+        "OutputArn": str,
     },
     total=False,
 )
 
 
-class GrantEntitlementRequestTypeDef(
-    _RequiredGrantEntitlementRequestTypeDef, _OptionalGrantEntitlementRequestTypeDef
+class BridgeFlowSourceTypeDef(_RequiredBridgeFlowSourceTypeDef, _OptionalBridgeFlowSourceTypeDef):
+    pass
+
+
+_RequiredGatewayBridgeSourceTypeDef = TypedDict(
+    "_RequiredGatewayBridgeSourceTypeDef",
+    {
+        "BridgeArn": str,
+    },
+)
+_OptionalGatewayBridgeSourceTypeDef = TypedDict(
+    "_OptionalGatewayBridgeSourceTypeDef",
+    {
+        "VpcInterfaceAttachment": VpcInterfaceAttachmentOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class GatewayBridgeSourceTypeDef(
+    _RequiredGatewayBridgeSourceTypeDef, _OptionalGatewayBridgeSourceTypeDef
 ):
     pass
 
 
 BridgeOutputTypeDef = TypedDict(
     "BridgeOutputTypeDef",
     {
@@ -1460,37 +1491,14 @@
     {
         "EgressCidrBlocks": Sequence[str],
         "Name": str,
         "Networks": Sequence[GatewayNetworkTypeDef],
     },
 )
 
-_RequiredGatewayTypeDef = TypedDict(
-    "_RequiredGatewayTypeDef",
-    {
-        "EgressCidrBlocks": List[str],
-        "GatewayArn": str,
-        "Name": str,
-        "Networks": List[GatewayNetworkTypeDef],
-    },
-)
-_OptionalGatewayTypeDef = TypedDict(
-    "_OptionalGatewayTypeDef",
-    {
-        "GatewayMessages": List[MessageDetailTypeDef],
-        "GatewayState": GatewayStateType,
-    },
-    total=False,
-)
-
-
-class GatewayTypeDef(_RequiredGatewayTypeDef, _OptionalGatewayTypeDef):
-    pass
-
-
 _RequiredDescribeFlowRequestFlowActiveWaitTypeDef = TypedDict(
     "_RequiredDescribeFlowRequestFlowActiveWaitTypeDef",
     {
         "FlowArn": str,
     },
 )
 _OptionalDescribeFlowRequestFlowActiveWaitTypeDef = TypedDict(
@@ -1585,14 +1593,49 @@
     {
         "InputIp": str,
         "InputPort": int,
         "Interface": InterfaceTypeDef,
     },
 )
 
+_RequiredEntitlementTypeDef = TypedDict(
+    "_RequiredEntitlementTypeDef",
+    {
+        "EntitlementArn": str,
+        "Name": str,
+        "Subscribers": List[str],
+    },
+)
+_OptionalEntitlementTypeDef = TypedDict(
+    "_OptionalEntitlementTypeDef",
+    {
+        "DataTransferSubscriberFeePercent": int,
+        "Description": str,
+        "Encryption": EncryptionOutputTypeDef,
+        "EntitlementStatus": EntitlementStatusType,
+    },
+    total=False,
+)
+
+
+class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
+    pass
+
+
+FailoverConfigOutputTypeDef = TypedDict(
+    "FailoverConfigOutputTypeDef",
+    {
+        "FailoverMode": FailoverModeType,
+        "RecoveryWindow": int,
+        "SourcePriority": SourcePriorityOutputTypeDef,
+        "State": StateType,
+    },
+    total=False,
+)
+
 FailoverConfigTypeDef = TypedDict(
     "FailoverConfigTypeDef",
     {
         "FailoverMode": FailoverModeType,
         "RecoveryWindow": int,
         "SourcePriority": SourcePriorityTypeDef,
         "State": StateType,
@@ -1661,14 +1704,37 @@
 
 class MediaStreamAttributesTypeDef(
     _RequiredMediaStreamAttributesTypeDef, _OptionalMediaStreamAttributesTypeDef
 ):
     pass
 
 
+_RequiredGatewayTypeDef = TypedDict(
+    "_RequiredGatewayTypeDef",
+    {
+        "EgressCidrBlocks": List[str],
+        "GatewayArn": str,
+        "Name": str,
+        "Networks": List[GatewayNetworkOutputTypeDef],
+    },
+)
+_OptionalGatewayTypeDef = TypedDict(
+    "_OptionalGatewayTypeDef",
+    {
+        "GatewayMessages": List[MessageDetailTypeDef],
+        "GatewayState": GatewayStateType,
+    },
+    total=False,
+)
+
+
+class GatewayTypeDef(_RequiredGatewayTypeDef, _OptionalGatewayTypeDef):
+    pass
+
+
 ListBridgesResponseTypeDef = TypedDict(
     "ListBridgesResponseTypeDef",
     {
         "Bridges": List[ListedBridgeTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1788,23 +1854,14 @@
     {
         "FlowSource": AddBridgeFlowSourceRequestTypeDef,
         "NetworkSource": AddBridgeNetworkSourceRequestTypeDef,
     },
     total=False,
 )
 
-BridgeSourceTypeDef = TypedDict(
-    "BridgeSourceTypeDef",
-    {
-        "FlowSource": BridgeFlowSourceTypeDef,
-        "NetworkSource": BridgeNetworkSourceTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateBridgeSourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBridgeSourceRequestRequestTypeDef",
     {
         "BridgeArn": str,
         "SourceName": str,
     },
 )
@@ -1829,38 +1886,29 @@
     "AddBridgeOutputsRequestRequestTypeDef",
     {
         "BridgeArn": str,
         "Outputs": Sequence[AddBridgeOutputRequestTypeDef],
     },
 )
 
-GrantFlowEntitlementsResponseTypeDef = TypedDict(
-    "GrantFlowEntitlementsResponseTypeDef",
-    {
-        "Entitlements": List[EntitlementTypeDef],
-        "FlowArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateFlowEntitlementResponseTypeDef = TypedDict(
-    "UpdateFlowEntitlementResponseTypeDef",
+GrantFlowEntitlementsRequestRequestTypeDef = TypedDict(
+    "GrantFlowEntitlementsRequestRequestTypeDef",
     {
-        "Entitlement": EntitlementTypeDef,
+        "Entitlements": Sequence[GrantEntitlementRequestTypeDef],
         "FlowArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GrantFlowEntitlementsRequestRequestTypeDef = TypedDict(
-    "GrantFlowEntitlementsRequestRequestTypeDef",
+BridgeSourceTypeDef = TypedDict(
+    "BridgeSourceTypeDef",
     {
-        "Entitlements": Sequence[GrantEntitlementRequestTypeDef],
-        "FlowArn": str,
+        "FlowSource": BridgeFlowSourceTypeDef,
+        "NetworkSource": BridgeNetworkSourceTypeDef,
     },
+    total=False,
 )
 
 AddBridgeOutputsResponseTypeDef = TypedDict(
     "AddBridgeOutputsResponseTypeDef",
     {
         "BridgeArn": str,
         "Outputs": List[BridgeOutputTypeDef],
@@ -1881,30 +1929,14 @@
     "DescribeGatewayInstanceResponseTypeDef",
     {
         "GatewayInstance": GatewayInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateGatewayResponseTypeDef = TypedDict(
-    "CreateGatewayResponseTypeDef",
-    {
-        "Gateway": GatewayTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeGatewayResponseTypeDef = TypedDict(
-    "DescribeGatewayResponseTypeDef",
-    {
-        "Gateway": GatewayTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredMediaStreamOutputConfigurationRequestTypeDef = TypedDict(
     "_RequiredMediaStreamOutputConfigurationRequestTypeDef",
     {
         "EncodingName": EncodingNameType,
         "MediaStreamName": str,
     },
 )
@@ -1989,14 +2021,32 @@
 
 class MediaStreamSourceConfigurationTypeDef(
     _RequiredMediaStreamSourceConfigurationTypeDef, _OptionalMediaStreamSourceConfigurationTypeDef
 ):
     pass
 
 
+GrantFlowEntitlementsResponseTypeDef = TypedDict(
+    "GrantFlowEntitlementsResponseTypeDef",
+    {
+        "Entitlements": List[EntitlementTypeDef],
+        "FlowArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateFlowEntitlementResponseTypeDef = TypedDict(
+    "UpdateFlowEntitlementResponseTypeDef",
+    {
+        "Entitlement": EntitlementTypeDef,
+        "FlowArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateBridgeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBridgeRequestRequestTypeDef",
     {
         "BridgeArn": str,
     },
 )
 _OptionalUpdateBridgeRequestRequestTypeDef = TypedDict(
@@ -2121,14 +2171,30 @@
 )
 
 
 class MediaStreamTypeDef(_RequiredMediaStreamTypeDef, _OptionalMediaStreamTypeDef):
     pass
 
 
+CreateGatewayResponseTypeDef = TypedDict(
+    "CreateGatewayResponseTypeDef",
+    {
+        "Gateway": GatewayTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeGatewayResponseTypeDef = TypedDict(
+    "DescribeGatewayResponseTypeDef",
+    {
+        "Gateway": GatewayTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeOfferingResponseTypeDef = TypedDict(
     "DescribeOfferingResponseTypeDef",
     {
         "Offering": OfferingTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2222,15 +2288,15 @@
 _OptionalBridgeTypeDef = TypedDict(
     "_OptionalBridgeTypeDef",
     {
         "BridgeMessages": List[MessageDetailTypeDef],
         "EgressGatewayBridge": EgressGatewayBridgeTypeDef,
         "IngressGatewayBridge": IngressGatewayBridgeTypeDef,
         "Outputs": List[BridgeOutputTypeDef],
-        "SourceFailoverConfig": FailoverConfigTypeDef,
+        "SourceFailoverConfig": FailoverConfigOutputTypeDef,
         "Sources": List[BridgeSourceTypeDef],
     },
     total=False,
 )
 
 
 class BridgeTypeDef(_RequiredBridgeTypeDef, _OptionalBridgeTypeDef):
@@ -2388,22 +2454,22 @@
 )
 _OptionalOutputTypeDef = TypedDict(
     "_OptionalOutputTypeDef",
     {
         "DataTransferSubscriberFeePercent": int,
         "Description": str,
         "Destination": str,
-        "Encryption": EncryptionTypeDef,
+        "Encryption": EncryptionOutputTypeDef,
         "EntitlementArn": str,
         "ListenerAddress": str,
         "MediaLiveInputArn": str,
         "MediaStreamOutputConfigurations": List[MediaStreamOutputConfigurationTypeDef],
         "Port": int,
         "Transport": TransportTypeDef,
-        "VpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
+        "VpcInterfaceAttachment": VpcInterfaceAttachmentOutputTypeDef,
         "BridgeArn": str,
         "BridgePorts": List[int],
     },
     total=False,
 )
 
 
@@ -2418,15 +2484,15 @@
         "SourceArn": str,
     },
 )
 _OptionalSourceTypeDef = TypedDict(
     "_OptionalSourceTypeDef",
     {
         "DataTransferSubscriberFeePercent": int,
-        "Decryption": EncryptionTypeDef,
+        "Decryption": EncryptionOutputTypeDef,
         "Description": str,
         "EntitlementArn": str,
         "IngestIp": str,
         "IngestPort": int,
         "MediaStreamSourceConfigurations": List[MediaStreamSourceConfigurationTypeDef],
         "SenderControlPort": int,
         "SenderIpAddress": str,
@@ -2579,15 +2645,15 @@
 )
 _OptionalFlowTypeDef = TypedDict(
     "_OptionalFlowTypeDef",
     {
         "Description": str,
         "EgressIp": str,
         "MediaStreams": List[MediaStreamTypeDef],
-        "SourceFailoverConfig": FailoverConfigTypeDef,
+        "SourceFailoverConfig": FailoverConfigOutputTypeDef,
         "Sources": List[SourceTypeDef],
         "VpcInterfaces": List[VpcInterfaceTypeDef],
         "Maintenance": MaintenanceTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/type_defs.pyi` & `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     "AddEgressGatewayBridgeRequestTypeDef",
     "VpcInterfaceRequestTypeDef",
     "VpcInterfaceTypeDef",
     "AddIngressGatewayBridgeRequestTypeDef",
     "AddMaintenanceTypeDef",
     "EncryptionTypeDef",
     "BridgeFlowOutputTypeDef",
+    "VpcInterfaceAttachmentOutputTypeDef",
     "BridgeNetworkOutputTypeDef",
     "BridgeNetworkSourceTypeDef",
     "EgressGatewayBridgeTypeDef",
     "IngressGatewayBridgeTypeDef",
     "MessageDetailTypeDef",
     "GatewayNetworkTypeDef",
     "DeleteBridgeRequestRequestTypeDef",
@@ -84,18 +85,21 @@
     "DescribeOfferingRequestRequestTypeDef",
     "DescribeReservationRequestRequestTypeDef",
     "InterfaceRequestTypeDef",
     "InterfaceTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EncodingParametersRequestTypeDef",
     "EncodingParametersTypeDef",
+    "EncryptionOutputTypeDef",
+    "SourcePriorityOutputTypeDef",
     "SourcePriorityTypeDef",
     "MaintenanceTypeDef",
     "FmtpRequestTypeDef",
     "FmtpTypeDef",
+    "GatewayNetworkOutputTypeDef",
     "ListBridgesRequestListBridgesPaginateTypeDef",
     "ListBridgesRequestRequestTypeDef",
     "ListedBridgeTypeDef",
     "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
     "ListEntitlementsRequestRequestTypeDef",
     "ListedEntitlementTypeDef",
     "ListFlowsRequestListFlowsPaginateTypeDef",
@@ -144,70 +148,71 @@
     "UpdateBridgeStateRequestRequestTypeDef",
     "UpdateBridgeStateResponseTypeDef",
     "UpdateEncryptionTypeDef",
     "UpdateMaintenanceTypeDef",
     "UpdateGatewayInstanceRequestRequestTypeDef",
     "UpdateGatewayInstanceResponseTypeDef",
     "AddBridgeFlowSourceRequestTypeDef",
-    "BridgeFlowSourceTypeDef",
-    "GatewayBridgeSourceTypeDef",
     "SetGatewayBridgeSourceRequestTypeDef",
     "UpdateBridgeFlowSourceRequestTypeDef",
     "UpdateGatewayBridgeSourceRequestTypeDef",
     "AddBridgeOutputRequestTypeDef",
     "AddFlowVpcInterfacesRequestRequestTypeDef",
     "AddFlowVpcInterfacesResponseTypeDef",
-    "EntitlementTypeDef",
     "GrantEntitlementRequestTypeDef",
+    "BridgeFlowSourceTypeDef",
+    "GatewayBridgeSourceTypeDef",
     "BridgeOutputTypeDef",
     "GatewayInstanceTypeDef",
     "CreateGatewayRequestRequestTypeDef",
-    "GatewayTypeDef",
     "DescribeFlowRequestFlowActiveWaitTypeDef",
     "DescribeFlowRequestFlowDeletedWaitTypeDef",
     "DescribeFlowRequestFlowStandbyWaitTypeDef",
     "DestinationConfigurationRequestTypeDef",
     "InputConfigurationRequestTypeDef",
     "DestinationConfigurationTypeDef",
     "InputConfigurationTypeDef",
+    "EntitlementTypeDef",
+    "FailoverConfigOutputTypeDef",
     "FailoverConfigTypeDef",
     "UpdateFailoverConfigTypeDef",
     "ListedFlowTypeDef",
     "MediaStreamAttributesRequestTypeDef",
     "MediaStreamAttributesTypeDef",
+    "GatewayTypeDef",
     "ListBridgesResponseTypeDef",
     "ListEntitlementsResponseTypeDef",
     "ListGatewayInstancesResponseTypeDef",
     "ListGatewaysResponseTypeDef",
     "OfferingTypeDef",
     "ReservationTypeDef",
     "UpdateBridgeOutputRequestRequestTypeDef",
     "UpdateFlowEntitlementRequestRequestTypeDef",
     "AddBridgeSourceRequestTypeDef",
-    "BridgeSourceTypeDef",
     "UpdateBridgeSourceRequestRequestTypeDef",
     "AddBridgeOutputsRequestRequestTypeDef",
-    "GrantFlowEntitlementsResponseTypeDef",
-    "UpdateFlowEntitlementResponseTypeDef",
     "GrantFlowEntitlementsRequestRequestTypeDef",
+    "BridgeSourceTypeDef",
     "AddBridgeOutputsResponseTypeDef",
     "UpdateBridgeOutputResponseTypeDef",
     "DescribeGatewayInstanceResponseTypeDef",
-    "CreateGatewayResponseTypeDef",
-    "DescribeGatewayResponseTypeDef",
     "MediaStreamOutputConfigurationRequestTypeDef",
     "MediaStreamSourceConfigurationRequestTypeDef",
     "MediaStreamOutputConfigurationTypeDef",
     "MediaStreamSourceConfigurationTypeDef",
+    "GrantFlowEntitlementsResponseTypeDef",
+    "UpdateFlowEntitlementResponseTypeDef",
     "UpdateBridgeRequestRequestTypeDef",
     "UpdateFlowRequestRequestTypeDef",
     "ListFlowsResponseTypeDef",
     "AddMediaStreamRequestTypeDef",
     "UpdateFlowMediaStreamRequestRequestTypeDef",
     "MediaStreamTypeDef",
+    "CreateGatewayResponseTypeDef",
+    "DescribeGatewayResponseTypeDef",
     "DescribeOfferingResponseTypeDef",
     "ListOfferingsResponseTypeDef",
     "DescribeReservationResponseTypeDef",
     "ListReservationsResponseTypeDef",
     "PurchaseOfferingResponseTypeDef",
     "AddBridgeSourcesRequestRequestTypeDef",
     "CreateBridgeRequestRequestTypeDef",
@@ -356,14 +361,22 @@
     {
         "FlowArn": str,
         "FlowSourceArn": str,
         "Name": str,
     },
 )
 
+VpcInterfaceAttachmentOutputTypeDef = TypedDict(
+    "VpcInterfaceAttachmentOutputTypeDef",
+    {
+        "VpcInterfaceName": str,
+    },
+    total=False,
+)
+
 BridgeNetworkOutputTypeDef = TypedDict(
     "BridgeNetworkOutputTypeDef",
     {
         "IpAddress": str,
         "Name": str,
         "NetworkName": str,
         "Port": int,
@@ -614,14 +627,46 @@
     "EncodingParametersTypeDef",
     {
         "CompressionFactor": float,
         "EncoderProfile": EncoderProfileType,
     },
 )
 
+_RequiredEncryptionOutputTypeDef = TypedDict(
+    "_RequiredEncryptionOutputTypeDef",
+    {
+        "RoleArn": str,
+    },
+)
+_OptionalEncryptionOutputTypeDef = TypedDict(
+    "_OptionalEncryptionOutputTypeDef",
+    {
+        "Algorithm": AlgorithmType,
+        "ConstantInitializationVector": str,
+        "DeviceId": str,
+        "KeyType": KeyTypeType,
+        "Region": str,
+        "ResourceId": str,
+        "SecretArn": str,
+        "Url": str,
+    },
+    total=False,
+)
+
+class EncryptionOutputTypeDef(_RequiredEncryptionOutputTypeDef, _OptionalEncryptionOutputTypeDef):
+    pass
+
+SourcePriorityOutputTypeDef = TypedDict(
+    "SourcePriorityOutputTypeDef",
+    {
+        "PrimarySource": str,
+    },
+    total=False,
+)
+
 SourcePriorityTypeDef = TypedDict(
     "SourcePriorityTypeDef",
     {
         "PrimarySource": str,
     },
     total=False,
 )
@@ -661,14 +706,22 @@
         "Range": RangeType,
         "ScanMode": ScanModeType,
         "Tcs": TcsType,
     },
     total=False,
 )
 
+GatewayNetworkOutputTypeDef = TypedDict(
+    "GatewayNetworkOutputTypeDef",
+    {
+        "CidrBlock": str,
+        "Name": str,
+    },
+)
+
 ListBridgesRequestListBridgesPaginateTypeDef = TypedDict(
     "ListBridgesRequestListBridgesPaginateTypeDef",
     {
         "FilterArn": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1237,52 +1290,14 @@
 )
 
 class AddBridgeFlowSourceRequestTypeDef(
     _RequiredAddBridgeFlowSourceRequestTypeDef, _OptionalAddBridgeFlowSourceRequestTypeDef
 ):
     pass
 
-_RequiredBridgeFlowSourceTypeDef = TypedDict(
-    "_RequiredBridgeFlowSourceTypeDef",
-    {
-        "FlowArn": str,
-        "Name": str,
-    },
-)
-_OptionalBridgeFlowSourceTypeDef = TypedDict(
-    "_OptionalBridgeFlowSourceTypeDef",
-    {
-        "FlowVpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
-        "OutputArn": str,
-    },
-    total=False,
-)
-
-class BridgeFlowSourceTypeDef(_RequiredBridgeFlowSourceTypeDef, _OptionalBridgeFlowSourceTypeDef):
-    pass
-
-_RequiredGatewayBridgeSourceTypeDef = TypedDict(
-    "_RequiredGatewayBridgeSourceTypeDef",
-    {
-        "BridgeArn": str,
-    },
-)
-_OptionalGatewayBridgeSourceTypeDef = TypedDict(
-    "_OptionalGatewayBridgeSourceTypeDef",
-    {
-        "VpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
-    },
-    total=False,
-)
-
-class GatewayBridgeSourceTypeDef(
-    _RequiredGatewayBridgeSourceTypeDef, _OptionalGatewayBridgeSourceTypeDef
-):
-    pass
-
 _RequiredSetGatewayBridgeSourceRequestTypeDef = TypedDict(
     "_RequiredSetGatewayBridgeSourceRequestTypeDef",
     {
         "BridgeArn": str,
     },
 )
 _OptionalSetGatewayBridgeSourceRequestTypeDef = TypedDict(
@@ -1337,56 +1352,72 @@
     {
         "FlowArn": str,
         "VpcInterfaces": List[VpcInterfaceTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredEntitlementTypeDef = TypedDict(
-    "_RequiredEntitlementTypeDef",
+_RequiredGrantEntitlementRequestTypeDef = TypedDict(
+    "_RequiredGrantEntitlementRequestTypeDef",
     {
-        "EntitlementArn": str,
-        "Name": str,
-        "Subscribers": List[str],
+        "Subscribers": Sequence[str],
     },
 )
-_OptionalEntitlementTypeDef = TypedDict(
-    "_OptionalEntitlementTypeDef",
+_OptionalGrantEntitlementRequestTypeDef = TypedDict(
+    "_OptionalGrantEntitlementRequestTypeDef",
     {
         "DataTransferSubscriberFeePercent": int,
         "Description": str,
         "Encryption": EncryptionTypeDef,
         "EntitlementStatus": EntitlementStatusType,
+        "Name": str,
     },
     total=False,
 )
 
-class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
+class GrantEntitlementRequestTypeDef(
+    _RequiredGrantEntitlementRequestTypeDef, _OptionalGrantEntitlementRequestTypeDef
+):
     pass
 
-_RequiredGrantEntitlementRequestTypeDef = TypedDict(
-    "_RequiredGrantEntitlementRequestTypeDef",
+_RequiredBridgeFlowSourceTypeDef = TypedDict(
+    "_RequiredBridgeFlowSourceTypeDef",
     {
-        "Subscribers": Sequence[str],
+        "FlowArn": str,
+        "Name": str,
     },
 )
-_OptionalGrantEntitlementRequestTypeDef = TypedDict(
-    "_OptionalGrantEntitlementRequestTypeDef",
+_OptionalBridgeFlowSourceTypeDef = TypedDict(
+    "_OptionalBridgeFlowSourceTypeDef",
     {
-        "DataTransferSubscriberFeePercent": int,
-        "Description": str,
-        "Encryption": EncryptionTypeDef,
-        "EntitlementStatus": EntitlementStatusType,
-        "Name": str,
+        "FlowVpcInterfaceAttachment": VpcInterfaceAttachmentOutputTypeDef,
+        "OutputArn": str,
     },
     total=False,
 )
 
-class GrantEntitlementRequestTypeDef(
-    _RequiredGrantEntitlementRequestTypeDef, _OptionalGrantEntitlementRequestTypeDef
+class BridgeFlowSourceTypeDef(_RequiredBridgeFlowSourceTypeDef, _OptionalBridgeFlowSourceTypeDef):
+    pass
+
+_RequiredGatewayBridgeSourceTypeDef = TypedDict(
+    "_RequiredGatewayBridgeSourceTypeDef",
+    {
+        "BridgeArn": str,
+    },
+)
+_OptionalGatewayBridgeSourceTypeDef = TypedDict(
+    "_OptionalGatewayBridgeSourceTypeDef",
+    {
+        "VpcInterfaceAttachment": VpcInterfaceAttachmentOutputTypeDef,
+    },
+    total=False,
+)
+
+class GatewayBridgeSourceTypeDef(
+    _RequiredGatewayBridgeSourceTypeDef, _OptionalGatewayBridgeSourceTypeDef
 ):
     pass
 
 BridgeOutputTypeDef = TypedDict(
     "BridgeOutputTypeDef",
     {
         "FlowOutput": BridgeFlowOutputTypeDef,
@@ -1423,35 +1454,14 @@
     {
         "EgressCidrBlocks": Sequence[str],
         "Name": str,
         "Networks": Sequence[GatewayNetworkTypeDef],
     },
 )
 
-_RequiredGatewayTypeDef = TypedDict(
-    "_RequiredGatewayTypeDef",
-    {
-        "EgressCidrBlocks": List[str],
-        "GatewayArn": str,
-        "Name": str,
-        "Networks": List[GatewayNetworkTypeDef],
-    },
-)
-_OptionalGatewayTypeDef = TypedDict(
-    "_OptionalGatewayTypeDef",
-    {
-        "GatewayMessages": List[MessageDetailTypeDef],
-        "GatewayState": GatewayStateType,
-    },
-    total=False,
-)
-
-class GatewayTypeDef(_RequiredGatewayTypeDef, _OptionalGatewayTypeDef):
-    pass
-
 _RequiredDescribeFlowRequestFlowActiveWaitTypeDef = TypedDict(
     "_RequiredDescribeFlowRequestFlowActiveWaitTypeDef",
     {
         "FlowArn": str,
     },
 )
 _OptionalDescribeFlowRequestFlowActiveWaitTypeDef = TypedDict(
@@ -1540,14 +1550,47 @@
     {
         "InputIp": str,
         "InputPort": int,
         "Interface": InterfaceTypeDef,
     },
 )
 
+_RequiredEntitlementTypeDef = TypedDict(
+    "_RequiredEntitlementTypeDef",
+    {
+        "EntitlementArn": str,
+        "Name": str,
+        "Subscribers": List[str],
+    },
+)
+_OptionalEntitlementTypeDef = TypedDict(
+    "_OptionalEntitlementTypeDef",
+    {
+        "DataTransferSubscriberFeePercent": int,
+        "Description": str,
+        "Encryption": EncryptionOutputTypeDef,
+        "EntitlementStatus": EntitlementStatusType,
+    },
+    total=False,
+)
+
+class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
+    pass
+
+FailoverConfigOutputTypeDef = TypedDict(
+    "FailoverConfigOutputTypeDef",
+    {
+        "FailoverMode": FailoverModeType,
+        "RecoveryWindow": int,
+        "SourcePriority": SourcePriorityOutputTypeDef,
+        "State": StateType,
+    },
+    total=False,
+)
+
 FailoverConfigTypeDef = TypedDict(
     "FailoverConfigTypeDef",
     {
         "FailoverMode": FailoverModeType,
         "RecoveryWindow": int,
         "SourcePriority": SourcePriorityTypeDef,
         "State": StateType,
@@ -1612,14 +1655,35 @@
 )
 
 class MediaStreamAttributesTypeDef(
     _RequiredMediaStreamAttributesTypeDef, _OptionalMediaStreamAttributesTypeDef
 ):
     pass
 
+_RequiredGatewayTypeDef = TypedDict(
+    "_RequiredGatewayTypeDef",
+    {
+        "EgressCidrBlocks": List[str],
+        "GatewayArn": str,
+        "Name": str,
+        "Networks": List[GatewayNetworkOutputTypeDef],
+    },
+)
+_OptionalGatewayTypeDef = TypedDict(
+    "_OptionalGatewayTypeDef",
+    {
+        "GatewayMessages": List[MessageDetailTypeDef],
+        "GatewayState": GatewayStateType,
+    },
+    total=False,
+)
+
+class GatewayTypeDef(_RequiredGatewayTypeDef, _OptionalGatewayTypeDef):
+    pass
+
 ListBridgesResponseTypeDef = TypedDict(
     "ListBridgesResponseTypeDef",
     {
         "Bridges": List[ListedBridgeTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1735,23 +1799,14 @@
     {
         "FlowSource": AddBridgeFlowSourceRequestTypeDef,
         "NetworkSource": AddBridgeNetworkSourceRequestTypeDef,
     },
     total=False,
 )
 
-BridgeSourceTypeDef = TypedDict(
-    "BridgeSourceTypeDef",
-    {
-        "FlowSource": BridgeFlowSourceTypeDef,
-        "NetworkSource": BridgeNetworkSourceTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateBridgeSourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBridgeSourceRequestRequestTypeDef",
     {
         "BridgeArn": str,
         "SourceName": str,
     },
 )
@@ -1774,38 +1829,29 @@
     "AddBridgeOutputsRequestRequestTypeDef",
     {
         "BridgeArn": str,
         "Outputs": Sequence[AddBridgeOutputRequestTypeDef],
     },
 )
 
-GrantFlowEntitlementsResponseTypeDef = TypedDict(
-    "GrantFlowEntitlementsResponseTypeDef",
-    {
-        "Entitlements": List[EntitlementTypeDef],
-        "FlowArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateFlowEntitlementResponseTypeDef = TypedDict(
-    "UpdateFlowEntitlementResponseTypeDef",
+GrantFlowEntitlementsRequestRequestTypeDef = TypedDict(
+    "GrantFlowEntitlementsRequestRequestTypeDef",
     {
-        "Entitlement": EntitlementTypeDef,
+        "Entitlements": Sequence[GrantEntitlementRequestTypeDef],
         "FlowArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GrantFlowEntitlementsRequestRequestTypeDef = TypedDict(
-    "GrantFlowEntitlementsRequestRequestTypeDef",
+BridgeSourceTypeDef = TypedDict(
+    "BridgeSourceTypeDef",
     {
-        "Entitlements": Sequence[GrantEntitlementRequestTypeDef],
-        "FlowArn": str,
+        "FlowSource": BridgeFlowSourceTypeDef,
+        "NetworkSource": BridgeNetworkSourceTypeDef,
     },
+    total=False,
 )
 
 AddBridgeOutputsResponseTypeDef = TypedDict(
     "AddBridgeOutputsResponseTypeDef",
     {
         "BridgeArn": str,
         "Outputs": List[BridgeOutputTypeDef],
@@ -1826,30 +1872,14 @@
     "DescribeGatewayInstanceResponseTypeDef",
     {
         "GatewayInstance": GatewayInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateGatewayResponseTypeDef = TypedDict(
-    "CreateGatewayResponseTypeDef",
-    {
-        "Gateway": GatewayTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeGatewayResponseTypeDef = TypedDict(
-    "DescribeGatewayResponseTypeDef",
-    {
-        "Gateway": GatewayTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredMediaStreamOutputConfigurationRequestTypeDef = TypedDict(
     "_RequiredMediaStreamOutputConfigurationRequestTypeDef",
     {
         "EncodingName": EncodingNameType,
         "MediaStreamName": str,
     },
 )
@@ -1926,14 +1956,32 @@
 )
 
 class MediaStreamSourceConfigurationTypeDef(
     _RequiredMediaStreamSourceConfigurationTypeDef, _OptionalMediaStreamSourceConfigurationTypeDef
 ):
     pass
 
+GrantFlowEntitlementsResponseTypeDef = TypedDict(
+    "GrantFlowEntitlementsResponseTypeDef",
+    {
+        "Entitlements": List[EntitlementTypeDef],
+        "FlowArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateFlowEntitlementResponseTypeDef = TypedDict(
+    "UpdateFlowEntitlementResponseTypeDef",
+    {
+        "Entitlement": EntitlementTypeDef,
+        "FlowArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateBridgeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBridgeRequestRequestTypeDef",
     {
         "BridgeArn": str,
     },
 )
 _OptionalUpdateBridgeRequestRequestTypeDef = TypedDict(
@@ -2048,14 +2096,30 @@
     },
     total=False,
 )
 
 class MediaStreamTypeDef(_RequiredMediaStreamTypeDef, _OptionalMediaStreamTypeDef):
     pass
 
+CreateGatewayResponseTypeDef = TypedDict(
+    "CreateGatewayResponseTypeDef",
+    {
+        "Gateway": GatewayTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeGatewayResponseTypeDef = TypedDict(
+    "DescribeGatewayResponseTypeDef",
+    {
+        "Gateway": GatewayTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeOfferingResponseTypeDef = TypedDict(
     "DescribeOfferingResponseTypeDef",
     {
         "Offering": OfferingTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2147,15 +2211,15 @@
 _OptionalBridgeTypeDef = TypedDict(
     "_OptionalBridgeTypeDef",
     {
         "BridgeMessages": List[MessageDetailTypeDef],
         "EgressGatewayBridge": EgressGatewayBridgeTypeDef,
         "IngressGatewayBridge": IngressGatewayBridgeTypeDef,
         "Outputs": List[BridgeOutputTypeDef],
-        "SourceFailoverConfig": FailoverConfigTypeDef,
+        "SourceFailoverConfig": FailoverConfigOutputTypeDef,
         "Sources": List[BridgeSourceTypeDef],
     },
     total=False,
 )
 
 class BridgeTypeDef(_RequiredBridgeTypeDef, _OptionalBridgeTypeDef):
     pass
@@ -2305,22 +2369,22 @@
 )
 _OptionalOutputTypeDef = TypedDict(
     "_OptionalOutputTypeDef",
     {
         "DataTransferSubscriberFeePercent": int,
         "Description": str,
         "Destination": str,
-        "Encryption": EncryptionTypeDef,
+        "Encryption": EncryptionOutputTypeDef,
         "EntitlementArn": str,
         "ListenerAddress": str,
         "MediaLiveInputArn": str,
         "MediaStreamOutputConfigurations": List[MediaStreamOutputConfigurationTypeDef],
         "Port": int,
         "Transport": TransportTypeDef,
-        "VpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
+        "VpcInterfaceAttachment": VpcInterfaceAttachmentOutputTypeDef,
         "BridgeArn": str,
         "BridgePorts": List[int],
     },
     total=False,
 )
 
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
@@ -2333,15 +2397,15 @@
         "SourceArn": str,
     },
 )
 _OptionalSourceTypeDef = TypedDict(
     "_OptionalSourceTypeDef",
     {
         "DataTransferSubscriberFeePercent": int,
-        "Decryption": EncryptionTypeDef,
+        "Decryption": EncryptionOutputTypeDef,
         "Description": str,
         "EntitlementArn": str,
         "IngestIp": str,
         "IngestPort": int,
         "MediaStreamSourceConfigurations": List[MediaStreamSourceConfigurationTypeDef],
         "SenderControlPort": int,
         "SenderIpAddress": str,
@@ -2490,15 +2554,15 @@
 )
 _OptionalFlowTypeDef = TypedDict(
     "_OptionalFlowTypeDef",
     {
         "Description": str,
         "EgressIp": str,
         "MediaStreams": List[MediaStreamTypeDef],
-        "SourceFailoverConfig": FailoverConfigTypeDef,
+        "SourceFailoverConfig": FailoverConfigOutputTypeDef,
         "Sources": List[SourceTypeDef],
         "VpcInterfaces": List[VpcInterfaceTypeDef],
         "Maintenance": MaintenanceTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/waiter.py` & `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/waiter.pyi` & `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect.egg-info/PKG-INFO` & `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediaconnect
-Version: 1.28.0
-Summary: Type annotations for boto3.MediaConnect 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MediaConnect 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mediaconnect"></a>
 
 # mypy-boto3-mediaconnect
 
 [![PyPI - mypy-boto3-mediaconnect](https://img.shields.io/pypi/v/mypy-boto3-mediaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconnect?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconnect)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediaconnect)](https://pepy.tech/project/mypy-boto3-mediaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConnect 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
+[boto3.MediaConnect 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
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
 [mypy-boto3-mediaconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -405,14 +405,15 @@
     AddEgressGatewayBridgeRequestTypeDef,
     VpcInterfaceRequestTypeDef,
     VpcInterfaceTypeDef,
     AddIngressGatewayBridgeRequestTypeDef,
     AddMaintenanceTypeDef,
     EncryptionTypeDef,
     BridgeFlowOutputTypeDef,
+    VpcInterfaceAttachmentOutputTypeDef,
     BridgeNetworkOutputTypeDef,
     BridgeNetworkSourceTypeDef,
     EgressGatewayBridgeTypeDef,
     IngressGatewayBridgeTypeDef,
     MessageDetailTypeDef,
     GatewayNetworkTypeDef,
     DeleteBridgeRequestRequestTypeDef,
@@ -432,18 +433,21 @@
     DescribeOfferingRequestRequestTypeDef,
     DescribeReservationRequestRequestTypeDef,
     InterfaceRequestTypeDef,
     InterfaceTypeDef,
     EmptyResponseMetadataTypeDef,
     EncodingParametersRequestTypeDef,
     EncodingParametersTypeDef,
+    EncryptionOutputTypeDef,
+    SourcePriorityOutputTypeDef,
     SourcePriorityTypeDef,
     MaintenanceTypeDef,
     FmtpRequestTypeDef,
     FmtpTypeDef,
+    GatewayNetworkOutputTypeDef,
     ListBridgesRequestListBridgesPaginateTypeDef,
     ListBridgesRequestRequestTypeDef,
     ListedBridgeTypeDef,
     ListEntitlementsRequestListEntitlementsPaginateTypeDef,
     ListEntitlementsRequestRequestTypeDef,
     ListedEntitlementTypeDef,
     ListFlowsRequestListFlowsPaginateTypeDef,
@@ -492,70 +496,71 @@
     UpdateBridgeStateRequestRequestTypeDef,
     UpdateBridgeStateResponseTypeDef,
     UpdateEncryptionTypeDef,
     UpdateMaintenanceTypeDef,
     UpdateGatewayInstanceRequestRequestTypeDef,
     UpdateGatewayInstanceResponseTypeDef,
     AddBridgeFlowSourceRequestTypeDef,
-    BridgeFlowSourceTypeDef,
-    GatewayBridgeSourceTypeDef,
     SetGatewayBridgeSourceRequestTypeDef,
     UpdateBridgeFlowSourceRequestTypeDef,
     UpdateGatewayBridgeSourceRequestTypeDef,
     AddBridgeOutputRequestTypeDef,
     AddFlowVpcInterfacesRequestRequestTypeDef,
     AddFlowVpcInterfacesResponseTypeDef,
-    EntitlementTypeDef,
     GrantEntitlementRequestTypeDef,
+    BridgeFlowSourceTypeDef,
+    GatewayBridgeSourceTypeDef,
     BridgeOutputTypeDef,
     GatewayInstanceTypeDef,
     CreateGatewayRequestRequestTypeDef,
-    GatewayTypeDef,
     DescribeFlowRequestFlowActiveWaitTypeDef,
     DescribeFlowRequestFlowDeletedWaitTypeDef,
     DescribeFlowRequestFlowStandbyWaitTypeDef,
     DestinationConfigurationRequestTypeDef,
     InputConfigurationRequestTypeDef,
     DestinationConfigurationTypeDef,
     InputConfigurationTypeDef,
+    EntitlementTypeDef,
+    FailoverConfigOutputTypeDef,
     FailoverConfigTypeDef,
     UpdateFailoverConfigTypeDef,
     ListedFlowTypeDef,
     MediaStreamAttributesRequestTypeDef,
     MediaStreamAttributesTypeDef,
+    GatewayTypeDef,
     ListBridgesResponseTypeDef,
     ListEntitlementsResponseTypeDef,
     ListGatewayInstancesResponseTypeDef,
     ListGatewaysResponseTypeDef,
     OfferingTypeDef,
     ReservationTypeDef,
     UpdateBridgeOutputRequestRequestTypeDef,
     UpdateFlowEntitlementRequestRequestTypeDef,
     AddBridgeSourceRequestTypeDef,
-    BridgeSourceTypeDef,
     UpdateBridgeSourceRequestRequestTypeDef,
     AddBridgeOutputsRequestRequestTypeDef,
-    GrantFlowEntitlementsResponseTypeDef,
-    UpdateFlowEntitlementResponseTypeDef,
     GrantFlowEntitlementsRequestRequestTypeDef,
+    BridgeSourceTypeDef,
     AddBridgeOutputsResponseTypeDef,
     UpdateBridgeOutputResponseTypeDef,
     DescribeGatewayInstanceResponseTypeDef,
-    CreateGatewayResponseTypeDef,
-    DescribeGatewayResponseTypeDef,
     MediaStreamOutputConfigurationRequestTypeDef,
     MediaStreamSourceConfigurationRequestTypeDef,
     MediaStreamOutputConfigurationTypeDef,
     MediaStreamSourceConfigurationTypeDef,
+    GrantFlowEntitlementsResponseTypeDef,
+    UpdateFlowEntitlementResponseTypeDef,
     UpdateBridgeRequestRequestTypeDef,
     UpdateFlowRequestRequestTypeDef,
     ListFlowsResponseTypeDef,
     AddMediaStreamRequestTypeDef,
     UpdateFlowMediaStreamRequestRequestTypeDef,
     MediaStreamTypeDef,
+    CreateGatewayResponseTypeDef,
+    DescribeGatewayResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     ListOfferingsResponseTypeDef,
     DescribeReservationResponseTypeDef,
     ListReservationsResponseTypeDef,
     PurchaseOfferingResponseTypeDef,
     AddBridgeSourcesRequestRequestTypeDef,
     CreateBridgeRequestRequestTypeDef,
```

### Comparing `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect.egg-info/SOURCES.txt` & `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.28.0/setup.py` & `mypy-boto3-mediaconnect-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediaconnect",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_mediaconnect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaConnect 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.MediaConnect 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

