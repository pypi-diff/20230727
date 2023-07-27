# Comparing `tmp/mypy-boto3-iotwireless-1.28.0.tar.gz` & `tmp/mypy-boto3-iotwireless-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotwireless-1.28.0.tar", last modified: Thu Jul  6 20:59:51 2023, max compression
+gzip compressed data, was "mypy-boto3-iotwireless-1.28.12.tar", last modified: Thu Jul 27 05:34:51 2023, max compression
```

## Comparing `mypy-boto3-iotwireless-1.28.0.tar` & `mypy-boto3-iotwireless-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:51.082336 mypy-boto3-iotwireless-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:44:12.000000 mypy-boto3-iotwireless-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25383 2023-07-06 20:59:51.078336 mypy-boto3-iotwireless-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23882 2023-07-06 20:44:12.000000 mypy-boto3-iotwireless-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:51.066336 mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-06 20:44:12.000000 mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-06 20:44:12.000000 mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-06 20:44:12.000000 mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72150 2023-07-06 20:44:13.000000 mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    72034 2023-07-06 20:44:12.000000 mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-07-06 20:44:13.000000 mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-06 20:44:13.000000 mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:44:12.000000 mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    97139 2023-07-06 20:44:16.000000 mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    97050 2023-07-06 20:44:14.000000 mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:44:12.000000 mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:51.078336 mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25383 2023-07-06 20:59:50.000000 mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-06 20:59:50.000000 mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:50.000000 mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:50.000000 mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:50.000000 mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 20:59:50.000000 mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:51.082336 mypy-boto3-iotwireless-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-06 20:44:12.000000 mypy-boto3-iotwireless-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.420476 mypy-boto3-iotwireless-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:19.000000 mypy-boto3-iotwireless-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27301 2023-07-27 05:34:51.420476 mypy-boto3-iotwireless-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25798 2023-07-27 05:24:19.000000 mypy-boto3-iotwireless-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.408475 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-27 05:24:19.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-27 05:24:19.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-27 05:24:19.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72150 2023-07-27 05:24:20.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72034 2023-07-27 05:24:19.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-07-27 05:24:20.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-07-27 05:24:20.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:19.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   110665 2023-07-27 05:24:22.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110572 2023-07-27 05:24:21.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:19.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.420476 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27301 2023-07-27 05:34:51.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-27 05:34:51.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:51.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 05:34:51.000000 mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:51.420476 mypy-boto3-iotwireless-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 05:24:19.000000 mypy-boto3-iotwireless-1.28.12/setup.py
```

### Comparing `mypy-boto3-iotwireless-1.28.0/LICENSE` & `mypy-boto3-iotwireless-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.28.0/PKG-INFO` & `mypy-boto3-iotwireless-1.28.12/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotwireless
-Version: 1.28.0
-Summary: Type annotations for boto3.IoTWireless 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTWireless 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iotwireless"></a>
 
 # mypy-boto3-iotwireless
 
 [![PyPI - mypy-boto3-iotwireless](https://img.shields.io/pypi/v/mypy-boto3-iotwireless.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotwireless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotwireless.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotwireless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotwireless?color=blue)](https://pypistats.org/packages/mypy-boto3-iotwireless)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotwireless)](https://pepy.tech/project/mypy-boto3-iotwireless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTWireless 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
+[boto3.IoTWireless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
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
 [mypy-boto3-iotwireless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -335,33 +335,40 @@
 ### Typed dictionaries
 
 `mypy_boto3_iotwireless.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotwireless.type_defs import (
+    SessionKeysAbpV10XOutputTypeDef,
     SessionKeysAbpV10XTypeDef,
+    SessionKeysAbpV11OutputTypeDef,
     SessionKeysAbpV11TypeDef,
     AccuracyTypeDef,
+    ApplicationConfigOutputTypeDef,
     ApplicationConfigTypeDef,
     SidewalkAccountInfoTypeDef,
     TagTypeDef,
+    SidewalkAccountInfoOutputTypeDef,
     AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef,
     AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef,
     AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     AssociateWirelessDeviceWithThingRequestRequestTypeDef,
     AssociateWirelessGatewayWithCertificateRequestRequestTypeDef,
     AssociateWirelessGatewayWithCertificateResponseTypeDef,
     AssociateWirelessGatewayWithThingRequestRequestTypeDef,
+    BeaconingOutputTypeDef,
     BeaconingTypeDef,
     CancelMulticastGroupSessionRequestRequestTypeDef,
     CdmaLocalIdTypeDef,
     CdmaNmrObjTypeDef,
     CertificateListTypeDef,
+    LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef,
     LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef,
+    LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef,
     LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef,
     CreateDestinationResponseTypeDef,
     LoRaWANDeviceProfileTypeDef,
     CreateDeviceProfileResponseTypeDef,
     LoRaWANFuotaTaskTypeDef,
     CreateFuotaTaskResponseTypeDef,
     LoRaWANMulticastTypeDef,
@@ -388,36 +395,42 @@
     DeleteWirelessDeviceRequestRequestTypeDef,
     DeleteWirelessGatewayRequestRequestTypeDef,
     DeleteWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     DeleteWirelessGatewayTaskRequestRequestTypeDef,
     DeregisterWirelessDeviceRequestRequestTypeDef,
     DestinationsTypeDef,
     DeviceProfileTypeDef,
+    SidewalkEventNotificationConfigurationsOutputTypeDef,
     SidewalkEventNotificationConfigurationsTypeDef,
+    SidewalkResourceTypeEventConfigurationOutputTypeDef,
     SidewalkResourceTypeEventConfigurationTypeDef,
     DisassociateAwsAccountFromPartnerAccountRequestRequestTypeDef,
     DisassociateMulticastGroupFromFuotaTaskRequestRequestTypeDef,
     DisassociateWirelessDeviceFromFuotaTaskRequestRequestTypeDef,
     DisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
     DisassociateWirelessDeviceFromThingRequestRequestTypeDef,
     DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef,
     DisassociateWirelessGatewayFromThingRequestRequestTypeDef,
+    PositioningOutputTypeDef,
     PositioningTypeDef,
     FuotaTaskTypeDef,
+    GatewayListItemOutputTypeDef,
     GatewayListItemTypeDef,
     GetDestinationRequestRequestTypeDef,
     GetDestinationResponseTypeDef,
     GetDeviceProfileRequestRequestTypeDef,
+    LoRaWANDeviceProfileOutputTypeDef,
     GetFuotaTaskRequestRequestTypeDef,
     LoRaWANFuotaTaskGetInfoTypeDef,
     GetMulticastGroupRequestRequestTypeDef,
     LoRaWANMulticastGetTypeDef,
     GetMulticastGroupSessionRequestRequestTypeDef,
-    LoRaWANMulticastSessionTypeDef,
+    LoRaWANMulticastSessionOutputTypeDef,
     GetNetworkAnalyzerConfigurationRequestRequestTypeDef,
+    TraceContentOutputTypeDef,
     GetPartnerAccountRequestRequestTypeDef,
     SidewalkAccountInfoWithFingerprintTypeDef,
     GetPositionConfigurationRequestRequestTypeDef,
     GnssTypeDef,
     IpTypeDef,
     WiFiAccessPointTypeDef,
     GetPositionEstimateResponseTypeDef,
@@ -444,15 +457,17 @@
     GetWirelessGatewayStatisticsResponseTypeDef,
     GetWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     GetWirelessGatewayTaskRequestRequestTypeDef,
     GetWirelessGatewayTaskResponseTypeDef,
     GlobalIdentityTypeDef,
     GsmLocalIdTypeDef,
     ImportedSidewalkDeviceTypeDef,
+    LoRaWANJoinEventNotificationConfigurationsOutputTypeDef,
     LoRaWANJoinEventNotificationConfigurationsTypeDef,
+    LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef,
     LoRaWANJoinResourceTypeEventConfigurationTypeDef,
     ListDestinationsRequestRequestTypeDef,
     ListDeviceProfilesRequestRequestTypeDef,
     ListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef,
     ListEventConfigurationsRequestRequestTypeDef,
     ListFuotaTasksRequestRequestTypeDef,
     ListMulticastGroupsByFuotaTaskRequestRequestTypeDef,
@@ -463,24 +478,29 @@
     NetworkAnalyzerConfigurationsTypeDef,
     ListPartnerAccountsRequestRequestTypeDef,
     ListPositionConfigurationsRequestRequestTypeDef,
     ListQueuedMessagesRequestRequestTypeDef,
     ListServiceProfilesRequestRequestTypeDef,
     ServiceProfileTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListWirelessDeviceImportTasksRequestRequestTypeDef,
     ListWirelessDevicesRequestRequestTypeDef,
     ListWirelessGatewayTaskDefinitionsRequestRequestTypeDef,
     ListWirelessGatewaysRequestRequestTypeDef,
     LoRaWANGatewayMetadataTypeDef,
+    OtaaV10XOutputTypeDef,
+    OtaaV11OutputTypeDef,
     OtaaV10XTypeDef,
     OtaaV11TypeDef,
+    LoRaWANGatewayVersionOutputTypeDef,
     LoRaWANGatewayVersionTypeDef,
     LoRaWANListDeviceTypeDef,
     LoRaWANMulticastMetadataTypeDef,
+    LoRaWANMulticastSessionTypeDef,
     LoRaWANStartFuotaTaskTypeDef,
     UpdateAbpV10XTypeDef,
     UpdateAbpV11TypeDef,
     LteLocalIdTypeDef,
     LteNmrObjTypeDef,
     SemtechGnssConfigurationTypeDef,
     SemtechGnssDetailTypeDef,
@@ -503,135 +523,158 @@
     UntagResourceRequestRequestTypeDef,
     UpdateDestinationRequestRequestTypeDef,
     UpdatePositionRequestRequestTypeDef,
     UpdateResourcePositionRequestRequestTypeDef,
     UpdateWirelessGatewayRequestRequestTypeDef,
     WcdmaLocalIdTypeDef,
     WcdmaNmrObjTypeDef,
+    WirelessDeviceEventLogOptionOutputTypeDef,
     WirelessDeviceEventLogOptionTypeDef,
+    WirelessGatewayEventLogOptionOutputTypeDef,
     WirelessGatewayEventLogOptionTypeDef,
+    AbpV10XOutputTypeDef,
     AbpV10XTypeDef,
+    AbpV11OutputTypeDef,
     AbpV11TypeDef,
     GetPositionResponseTypeDef,
-    AssociateAwsAccountWithPartnerAccountResponseTypeDef,
     AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef,
     CreateDestinationRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    AssociateAwsAccountWithPartnerAccountResponseTypeDef,
+    LoRaWANGatewayOutputTypeDef,
     LoRaWANGatewayTypeDef,
     CdmaObjTypeDef,
     SidewalkDeviceTypeDef,
     SidewalkListDeviceTypeDef,
+    ConnectionStatusEventConfigurationOutputTypeDef,
     ConnectionStatusEventConfigurationTypeDef,
+    ConnectionStatusResourceTypeEventConfigurationOutputTypeDef,
     ConnectionStatusResourceTypeEventConfigurationTypeDef,
     CreateDeviceProfileRequestRequestTypeDef,
     CreateFuotaTaskRequestRequestTypeDef,
     UpdateFuotaTaskRequestRequestTypeDef,
     CreateMulticastGroupRequestRequestTypeDef,
     UpdateMulticastGroupRequestRequestTypeDef,
     CreateNetworkAnalyzerConfigurationRequestRequestTypeDef,
-    GetNetworkAnalyzerConfigurationResponseTypeDef,
     UpdateNetworkAnalyzerConfigurationRequestRequestTypeDef,
     CreateServiceProfileRequestRequestTypeDef,
     SidewalkGetDeviceProfileTypeDef,
     ListDestinationsResponseTypeDef,
     ListDeviceProfilesResponseTypeDef,
+    DeviceRegistrationStateEventConfigurationOutputTypeDef,
+    MessageDeliveryStatusEventConfigurationOutputTypeDef,
+    ProximityEventConfigurationOutputTypeDef,
     DeviceRegistrationStateEventConfigurationTypeDef,
     MessageDeliveryStatusEventConfigurationTypeDef,
     ProximityEventConfigurationTypeDef,
+    DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef,
+    MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef,
+    ProximityResourceTypeEventConfigurationOutputTypeDef,
     DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,
     MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
     ProximityResourceTypeEventConfigurationTypeDef,
+    FPortsOutputTypeDef,
     FPortsTypeDef,
     UpdateFPortsTypeDef,
     ListFuotaTasksResponseTypeDef,
+    ParticipatingGatewaysOutputTypeDef,
     ParticipatingGatewaysTypeDef,
     GetFuotaTaskResponseTypeDef,
     GetMulticastGroupResponseTypeDef,
     GetMulticastGroupSessionResponseTypeDef,
-    StartMulticastGroupSessionRequestRequestTypeDef,
+    GetNetworkAnalyzerConfigurationResponseTypeDef,
     GetPartnerAccountResponseTypeDef,
     ListPartnerAccountsResponseTypeDef,
     GetServiceProfileResponseTypeDef,
     GetWirelessDeviceImportTaskResponseTypeDef,
     WirelessDeviceImportTaskTypeDef,
     GsmNmrObjTypeDef,
     ImportedWirelessDeviceTypeDef,
+    JoinEventConfigurationOutputTypeDef,
     JoinEventConfigurationTypeDef,
+    JoinResourceTypeEventConfigurationOutputTypeDef,
     JoinResourceTypeEventConfigurationTypeDef,
     ListMulticastGroupsByFuotaTaskResponseTypeDef,
     ListMulticastGroupsResponseTypeDef,
     ListNetworkAnalyzerConfigurationsResponseTypeDef,
     ListServiceProfilesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     LoRaWANDeviceMetadataTypeDef,
     LoRaWANGatewayCurrentVersionTypeDef,
-    LoRaWANUpdateGatewayTaskCreateTypeDef,
+    LoRaWANUpdateGatewayTaskCreateOutputTypeDef,
     LoRaWANUpdateGatewayTaskEntryTypeDef,
+    LoRaWANUpdateGatewayTaskCreateTypeDef,
     MulticastWirelessMetadataTypeDef,
+    StartMulticastGroupSessionRequestRequestTypeDef,
     StartFuotaTaskRequestRequestTypeDef,
     LteObjTypeDef,
     PositionSolverConfigurationsTypeDef,
     PositionSolverDetailsTypeDef,
     StartSingleWirelessDeviceImportTaskRequestRequestTypeDef,
     StartWirelessDeviceImportTaskRequestRequestTypeDef,
     UpdatePartnerAccountRequestRequestTypeDef,
     UpdateWirelessDeviceImportTaskRequestRequestTypeDef,
     TdscdmaObjTypeDef,
     WcdmaObjTypeDef,
+    WirelessDeviceLogOptionOutputTypeDef,
     WirelessDeviceLogOptionTypeDef,
+    WirelessGatewayLogOptionOutputTypeDef,
     WirelessGatewayLogOptionTypeDef,
-    CreateWirelessGatewayRequestRequestTypeDef,
     GetWirelessGatewayResponseTypeDef,
     WirelessGatewayStatisticsTypeDef,
+    CreateWirelessGatewayRequestRequestTypeDef,
     WirelessDeviceStatisticsTypeDef,
     GetDeviceProfileResponseTypeDef,
+    LoRaWANDeviceOutputTypeDef,
     LoRaWANDeviceTypeDef,
     LoRaWANUpdateDeviceTypeDef,
+    LoRaWANSendDataToDeviceOutputTypeDef,
     LoRaWANSendDataToDeviceTypeDef,
     ListWirelessDeviceImportTasksResponseTypeDef,
     GsmObjTypeDef,
     ListDevicesForWirelessDeviceImportTaskResponseTypeDef,
     EventNotificationItemConfigurationsTypeDef,
     GetResourceEventConfigurationResponseTypeDef,
     UpdateResourceEventConfigurationRequestRequestTypeDef,
     GetEventConfigurationByResourceTypesResponseTypeDef,
     UpdateEventConfigurationByResourceTypesRequestRequestTypeDef,
     GetWirelessDeviceStatisticsResponseTypeDef,
     GetWirelessGatewayFirmwareInformationResponseTypeDef,
-    UpdateWirelessGatewayTaskCreateTypeDef,
+    UpdateWirelessGatewayTaskCreateOutputTypeDef,
     UpdateWirelessGatewayTaskEntryTypeDef,
+    UpdateWirelessGatewayTaskCreateTypeDef,
     SendDataToMulticastGroupRequestRequestTypeDef,
     PutPositionConfigurationRequestRequestTypeDef,
     GetPositionConfigurationResponseTypeDef,
     PositionConfigurationItemTypeDef,
     GetLogLevelsByResourceTypesResponseTypeDef,
     UpdateLogLevelsByResourceTypesRequestRequestTypeDef,
     ListWirelessGatewaysResponseTypeDef,
     ListWirelessDevicesResponseTypeDef,
-    CreateWirelessDeviceRequestRequestTypeDef,
     GetWirelessDeviceResponseTypeDef,
+    CreateWirelessDeviceRequestRequestTypeDef,
     UpdateWirelessDeviceRequestRequestTypeDef,
     DownlinkQueueMessageTypeDef,
     WirelessMetadataTypeDef,
     CellTowersTypeDef,
     EventConfigurationItemTypeDef,
-    CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     GetWirelessGatewayTaskDefinitionResponseTypeDef,
     ListWirelessGatewayTaskDefinitionsResponseTypeDef,
+    CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     ListPositionConfigurationsResponseTypeDef,
     ListQueuedMessagesResponseTypeDef,
     SendDataToWirelessDeviceRequestRequestTypeDef,
     GetPositionEstimateRequestRequestTypeDef,
     ListEventConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> SessionKeysAbpV10XTypeDef:
+def get_structure() -> SessionKeysAbpV10XOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotwireless-1.28.0/README.md` & `mypy-boto3-iotwireless-1.28.12/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iotwireless"></a>
 
 # mypy-boto3-iotwireless
 
 [![PyPI - mypy-boto3-iotwireless](https://img.shields.io/pypi/v/mypy-boto3-iotwireless.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotwireless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotwireless.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotwireless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotwireless?color=blue)](https://pypistats.org/packages/mypy-boto3-iotwireless)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotwireless)](https://pepy.tech/project/mypy-boto3-iotwireless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTWireless 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
+[boto3.IoTWireless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
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
 [mypy-boto3-iotwireless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,33 +303,40 @@
 ### Typed dictionaries
 
 `mypy_boto3_iotwireless.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotwireless.type_defs import (
+    SessionKeysAbpV10XOutputTypeDef,
     SessionKeysAbpV10XTypeDef,
+    SessionKeysAbpV11OutputTypeDef,
     SessionKeysAbpV11TypeDef,
     AccuracyTypeDef,
+    ApplicationConfigOutputTypeDef,
     ApplicationConfigTypeDef,
     SidewalkAccountInfoTypeDef,
     TagTypeDef,
+    SidewalkAccountInfoOutputTypeDef,
     AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef,
     AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef,
     AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     AssociateWirelessDeviceWithThingRequestRequestTypeDef,
     AssociateWirelessGatewayWithCertificateRequestRequestTypeDef,
     AssociateWirelessGatewayWithCertificateResponseTypeDef,
     AssociateWirelessGatewayWithThingRequestRequestTypeDef,
+    BeaconingOutputTypeDef,
     BeaconingTypeDef,
     CancelMulticastGroupSessionRequestRequestTypeDef,
     CdmaLocalIdTypeDef,
     CdmaNmrObjTypeDef,
     CertificateListTypeDef,
+    LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef,
     LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef,
+    LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef,
     LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef,
     CreateDestinationResponseTypeDef,
     LoRaWANDeviceProfileTypeDef,
     CreateDeviceProfileResponseTypeDef,
     LoRaWANFuotaTaskTypeDef,
     CreateFuotaTaskResponseTypeDef,
     LoRaWANMulticastTypeDef,
@@ -356,36 +363,42 @@
     DeleteWirelessDeviceRequestRequestTypeDef,
     DeleteWirelessGatewayRequestRequestTypeDef,
     DeleteWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     DeleteWirelessGatewayTaskRequestRequestTypeDef,
     DeregisterWirelessDeviceRequestRequestTypeDef,
     DestinationsTypeDef,
     DeviceProfileTypeDef,
+    SidewalkEventNotificationConfigurationsOutputTypeDef,
     SidewalkEventNotificationConfigurationsTypeDef,
+    SidewalkResourceTypeEventConfigurationOutputTypeDef,
     SidewalkResourceTypeEventConfigurationTypeDef,
     DisassociateAwsAccountFromPartnerAccountRequestRequestTypeDef,
     DisassociateMulticastGroupFromFuotaTaskRequestRequestTypeDef,
     DisassociateWirelessDeviceFromFuotaTaskRequestRequestTypeDef,
     DisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
     DisassociateWirelessDeviceFromThingRequestRequestTypeDef,
     DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef,
     DisassociateWirelessGatewayFromThingRequestRequestTypeDef,
+    PositioningOutputTypeDef,
     PositioningTypeDef,
     FuotaTaskTypeDef,
+    GatewayListItemOutputTypeDef,
     GatewayListItemTypeDef,
     GetDestinationRequestRequestTypeDef,
     GetDestinationResponseTypeDef,
     GetDeviceProfileRequestRequestTypeDef,
+    LoRaWANDeviceProfileOutputTypeDef,
     GetFuotaTaskRequestRequestTypeDef,
     LoRaWANFuotaTaskGetInfoTypeDef,
     GetMulticastGroupRequestRequestTypeDef,
     LoRaWANMulticastGetTypeDef,
     GetMulticastGroupSessionRequestRequestTypeDef,
-    LoRaWANMulticastSessionTypeDef,
+    LoRaWANMulticastSessionOutputTypeDef,
     GetNetworkAnalyzerConfigurationRequestRequestTypeDef,
+    TraceContentOutputTypeDef,
     GetPartnerAccountRequestRequestTypeDef,
     SidewalkAccountInfoWithFingerprintTypeDef,
     GetPositionConfigurationRequestRequestTypeDef,
     GnssTypeDef,
     IpTypeDef,
     WiFiAccessPointTypeDef,
     GetPositionEstimateResponseTypeDef,
@@ -412,15 +425,17 @@
     GetWirelessGatewayStatisticsResponseTypeDef,
     GetWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     GetWirelessGatewayTaskRequestRequestTypeDef,
     GetWirelessGatewayTaskResponseTypeDef,
     GlobalIdentityTypeDef,
     GsmLocalIdTypeDef,
     ImportedSidewalkDeviceTypeDef,
+    LoRaWANJoinEventNotificationConfigurationsOutputTypeDef,
     LoRaWANJoinEventNotificationConfigurationsTypeDef,
+    LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef,
     LoRaWANJoinResourceTypeEventConfigurationTypeDef,
     ListDestinationsRequestRequestTypeDef,
     ListDeviceProfilesRequestRequestTypeDef,
     ListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef,
     ListEventConfigurationsRequestRequestTypeDef,
     ListFuotaTasksRequestRequestTypeDef,
     ListMulticastGroupsByFuotaTaskRequestRequestTypeDef,
@@ -431,24 +446,29 @@
     NetworkAnalyzerConfigurationsTypeDef,
     ListPartnerAccountsRequestRequestTypeDef,
     ListPositionConfigurationsRequestRequestTypeDef,
     ListQueuedMessagesRequestRequestTypeDef,
     ListServiceProfilesRequestRequestTypeDef,
     ServiceProfileTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListWirelessDeviceImportTasksRequestRequestTypeDef,
     ListWirelessDevicesRequestRequestTypeDef,
     ListWirelessGatewayTaskDefinitionsRequestRequestTypeDef,
     ListWirelessGatewaysRequestRequestTypeDef,
     LoRaWANGatewayMetadataTypeDef,
+    OtaaV10XOutputTypeDef,
+    OtaaV11OutputTypeDef,
     OtaaV10XTypeDef,
     OtaaV11TypeDef,
+    LoRaWANGatewayVersionOutputTypeDef,
     LoRaWANGatewayVersionTypeDef,
     LoRaWANListDeviceTypeDef,
     LoRaWANMulticastMetadataTypeDef,
+    LoRaWANMulticastSessionTypeDef,
     LoRaWANStartFuotaTaskTypeDef,
     UpdateAbpV10XTypeDef,
     UpdateAbpV11TypeDef,
     LteLocalIdTypeDef,
     LteNmrObjTypeDef,
     SemtechGnssConfigurationTypeDef,
     SemtechGnssDetailTypeDef,
@@ -471,135 +491,158 @@
     UntagResourceRequestRequestTypeDef,
     UpdateDestinationRequestRequestTypeDef,
     UpdatePositionRequestRequestTypeDef,
     UpdateResourcePositionRequestRequestTypeDef,
     UpdateWirelessGatewayRequestRequestTypeDef,
     WcdmaLocalIdTypeDef,
     WcdmaNmrObjTypeDef,
+    WirelessDeviceEventLogOptionOutputTypeDef,
     WirelessDeviceEventLogOptionTypeDef,
+    WirelessGatewayEventLogOptionOutputTypeDef,
     WirelessGatewayEventLogOptionTypeDef,
+    AbpV10XOutputTypeDef,
     AbpV10XTypeDef,
+    AbpV11OutputTypeDef,
     AbpV11TypeDef,
     GetPositionResponseTypeDef,
-    AssociateAwsAccountWithPartnerAccountResponseTypeDef,
     AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef,
     CreateDestinationRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    AssociateAwsAccountWithPartnerAccountResponseTypeDef,
+    LoRaWANGatewayOutputTypeDef,
     LoRaWANGatewayTypeDef,
     CdmaObjTypeDef,
     SidewalkDeviceTypeDef,
     SidewalkListDeviceTypeDef,
+    ConnectionStatusEventConfigurationOutputTypeDef,
     ConnectionStatusEventConfigurationTypeDef,
+    ConnectionStatusResourceTypeEventConfigurationOutputTypeDef,
     ConnectionStatusResourceTypeEventConfigurationTypeDef,
     CreateDeviceProfileRequestRequestTypeDef,
     CreateFuotaTaskRequestRequestTypeDef,
     UpdateFuotaTaskRequestRequestTypeDef,
     CreateMulticastGroupRequestRequestTypeDef,
     UpdateMulticastGroupRequestRequestTypeDef,
     CreateNetworkAnalyzerConfigurationRequestRequestTypeDef,
-    GetNetworkAnalyzerConfigurationResponseTypeDef,
     UpdateNetworkAnalyzerConfigurationRequestRequestTypeDef,
     CreateServiceProfileRequestRequestTypeDef,
     SidewalkGetDeviceProfileTypeDef,
     ListDestinationsResponseTypeDef,
     ListDeviceProfilesResponseTypeDef,
+    DeviceRegistrationStateEventConfigurationOutputTypeDef,
+    MessageDeliveryStatusEventConfigurationOutputTypeDef,
+    ProximityEventConfigurationOutputTypeDef,
     DeviceRegistrationStateEventConfigurationTypeDef,
     MessageDeliveryStatusEventConfigurationTypeDef,
     ProximityEventConfigurationTypeDef,
+    DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef,
+    MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef,
+    ProximityResourceTypeEventConfigurationOutputTypeDef,
     DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,
     MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
     ProximityResourceTypeEventConfigurationTypeDef,
+    FPortsOutputTypeDef,
     FPortsTypeDef,
     UpdateFPortsTypeDef,
     ListFuotaTasksResponseTypeDef,
+    ParticipatingGatewaysOutputTypeDef,
     ParticipatingGatewaysTypeDef,
     GetFuotaTaskResponseTypeDef,
     GetMulticastGroupResponseTypeDef,
     GetMulticastGroupSessionResponseTypeDef,
-    StartMulticastGroupSessionRequestRequestTypeDef,
+    GetNetworkAnalyzerConfigurationResponseTypeDef,
     GetPartnerAccountResponseTypeDef,
     ListPartnerAccountsResponseTypeDef,
     GetServiceProfileResponseTypeDef,
     GetWirelessDeviceImportTaskResponseTypeDef,
     WirelessDeviceImportTaskTypeDef,
     GsmNmrObjTypeDef,
     ImportedWirelessDeviceTypeDef,
+    JoinEventConfigurationOutputTypeDef,
     JoinEventConfigurationTypeDef,
+    JoinResourceTypeEventConfigurationOutputTypeDef,
     JoinResourceTypeEventConfigurationTypeDef,
     ListMulticastGroupsByFuotaTaskResponseTypeDef,
     ListMulticastGroupsResponseTypeDef,
     ListNetworkAnalyzerConfigurationsResponseTypeDef,
     ListServiceProfilesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     LoRaWANDeviceMetadataTypeDef,
     LoRaWANGatewayCurrentVersionTypeDef,
-    LoRaWANUpdateGatewayTaskCreateTypeDef,
+    LoRaWANUpdateGatewayTaskCreateOutputTypeDef,
     LoRaWANUpdateGatewayTaskEntryTypeDef,
+    LoRaWANUpdateGatewayTaskCreateTypeDef,
     MulticastWirelessMetadataTypeDef,
+    StartMulticastGroupSessionRequestRequestTypeDef,
     StartFuotaTaskRequestRequestTypeDef,
     LteObjTypeDef,
     PositionSolverConfigurationsTypeDef,
     PositionSolverDetailsTypeDef,
     StartSingleWirelessDeviceImportTaskRequestRequestTypeDef,
     StartWirelessDeviceImportTaskRequestRequestTypeDef,
     UpdatePartnerAccountRequestRequestTypeDef,
     UpdateWirelessDeviceImportTaskRequestRequestTypeDef,
     TdscdmaObjTypeDef,
     WcdmaObjTypeDef,
+    WirelessDeviceLogOptionOutputTypeDef,
     WirelessDeviceLogOptionTypeDef,
+    WirelessGatewayLogOptionOutputTypeDef,
     WirelessGatewayLogOptionTypeDef,
-    CreateWirelessGatewayRequestRequestTypeDef,
     GetWirelessGatewayResponseTypeDef,
     WirelessGatewayStatisticsTypeDef,
+    CreateWirelessGatewayRequestRequestTypeDef,
     WirelessDeviceStatisticsTypeDef,
     GetDeviceProfileResponseTypeDef,
+    LoRaWANDeviceOutputTypeDef,
     LoRaWANDeviceTypeDef,
     LoRaWANUpdateDeviceTypeDef,
+    LoRaWANSendDataToDeviceOutputTypeDef,
     LoRaWANSendDataToDeviceTypeDef,
     ListWirelessDeviceImportTasksResponseTypeDef,
     GsmObjTypeDef,
     ListDevicesForWirelessDeviceImportTaskResponseTypeDef,
     EventNotificationItemConfigurationsTypeDef,
     GetResourceEventConfigurationResponseTypeDef,
     UpdateResourceEventConfigurationRequestRequestTypeDef,
     GetEventConfigurationByResourceTypesResponseTypeDef,
     UpdateEventConfigurationByResourceTypesRequestRequestTypeDef,
     GetWirelessDeviceStatisticsResponseTypeDef,
     GetWirelessGatewayFirmwareInformationResponseTypeDef,
-    UpdateWirelessGatewayTaskCreateTypeDef,
+    UpdateWirelessGatewayTaskCreateOutputTypeDef,
     UpdateWirelessGatewayTaskEntryTypeDef,
+    UpdateWirelessGatewayTaskCreateTypeDef,
     SendDataToMulticastGroupRequestRequestTypeDef,
     PutPositionConfigurationRequestRequestTypeDef,
     GetPositionConfigurationResponseTypeDef,
     PositionConfigurationItemTypeDef,
     GetLogLevelsByResourceTypesResponseTypeDef,
     UpdateLogLevelsByResourceTypesRequestRequestTypeDef,
     ListWirelessGatewaysResponseTypeDef,
     ListWirelessDevicesResponseTypeDef,
-    CreateWirelessDeviceRequestRequestTypeDef,
     GetWirelessDeviceResponseTypeDef,
+    CreateWirelessDeviceRequestRequestTypeDef,
     UpdateWirelessDeviceRequestRequestTypeDef,
     DownlinkQueueMessageTypeDef,
     WirelessMetadataTypeDef,
     CellTowersTypeDef,
     EventConfigurationItemTypeDef,
-    CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     GetWirelessGatewayTaskDefinitionResponseTypeDef,
     ListWirelessGatewayTaskDefinitionsResponseTypeDef,
+    CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     ListPositionConfigurationsResponseTypeDef,
     ListQueuedMessagesResponseTypeDef,
     SendDataToWirelessDeviceRequestRequestTypeDef,
     GetPositionEstimateRequestRequestTypeDef,
     ListEventConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> SessionKeysAbpV10XTypeDef:
+def get_structure() -> SessionKeysAbpV10XOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless/__main__.py` & `mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTWireless 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.IoTWireless 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless\nOther"
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

### Comparing `mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless/client.py` & `mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless/client.pyi` & `mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless/literals.py` & `mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,14 +266,15 @@
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
@@ -352,26 +353,28 @@
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

### Comparing `mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless/literals.pyi` & `mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -264,14 +264,15 @@
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
@@ -350,26 +351,28 @@
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

### Comparing `mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless/type_defs.py` & `mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iotwireless service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iotwireless.type_defs import SessionKeysAbpV10XTypeDef
+    from mypy_boto3_iotwireless.type_defs import SessionKeysAbpV10XOutputTypeDef
 
-    data: SessionKeysAbpV10XTypeDef = {...}
+    data: SessionKeysAbpV10XOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -58,35 +58,41 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "SessionKeysAbpV10XOutputTypeDef",
     "SessionKeysAbpV10XTypeDef",
+    "SessionKeysAbpV11OutputTypeDef",
     "SessionKeysAbpV11TypeDef",
     "AccuracyTypeDef",
+    "ApplicationConfigOutputTypeDef",
     "ApplicationConfigTypeDef",
     "SidewalkAccountInfoTypeDef",
     "TagTypeDef",
+    "SidewalkAccountInfoOutputTypeDef",
     "AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef",
     "AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef",
     "AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     "AssociateWirelessDeviceWithThingRequestRequestTypeDef",
     "AssociateWirelessGatewayWithCertificateRequestRequestTypeDef",
     "AssociateWirelessGatewayWithCertificateResponseTypeDef",
     "AssociateWirelessGatewayWithThingRequestRequestTypeDef",
+    "BeaconingOutputTypeDef",
     "BeaconingTypeDef",
     "CancelMulticastGroupSessionRequestRequestTypeDef",
     "CdmaLocalIdTypeDef",
     "CdmaNmrObjTypeDef",
     "CertificateListTypeDef",
+    "LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef",
     "LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef",
+    "LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef",
     "LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef",
     "CreateDestinationResponseTypeDef",
     "LoRaWANDeviceProfileTypeDef",
     "CreateDeviceProfileResponseTypeDef",
     "LoRaWANFuotaTaskTypeDef",
     "CreateFuotaTaskResponseTypeDef",
     "LoRaWANMulticastTypeDef",
@@ -113,36 +119,42 @@
     "DeleteWirelessDeviceRequestRequestTypeDef",
     "DeleteWirelessGatewayRequestRequestTypeDef",
     "DeleteWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "DeleteWirelessGatewayTaskRequestRequestTypeDef",
     "DeregisterWirelessDeviceRequestRequestTypeDef",
     "DestinationsTypeDef",
     "DeviceProfileTypeDef",
+    "SidewalkEventNotificationConfigurationsOutputTypeDef",
     "SidewalkEventNotificationConfigurationsTypeDef",
+    "SidewalkResourceTypeEventConfigurationOutputTypeDef",
     "SidewalkResourceTypeEventConfigurationTypeDef",
     "DisassociateAwsAccountFromPartnerAccountRequestRequestTypeDef",
     "DisassociateMulticastGroupFromFuotaTaskRequestRequestTypeDef",
     "DisassociateWirelessDeviceFromFuotaTaskRequestRequestTypeDef",
     "DisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef",
     "DisassociateWirelessDeviceFromThingRequestRequestTypeDef",
     "DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef",
     "DisassociateWirelessGatewayFromThingRequestRequestTypeDef",
+    "PositioningOutputTypeDef",
     "PositioningTypeDef",
     "FuotaTaskTypeDef",
+    "GatewayListItemOutputTypeDef",
     "GatewayListItemTypeDef",
     "GetDestinationRequestRequestTypeDef",
     "GetDestinationResponseTypeDef",
     "GetDeviceProfileRequestRequestTypeDef",
+    "LoRaWANDeviceProfileOutputTypeDef",
     "GetFuotaTaskRequestRequestTypeDef",
     "LoRaWANFuotaTaskGetInfoTypeDef",
     "GetMulticastGroupRequestRequestTypeDef",
     "LoRaWANMulticastGetTypeDef",
     "GetMulticastGroupSessionRequestRequestTypeDef",
-    "LoRaWANMulticastSessionTypeDef",
+    "LoRaWANMulticastSessionOutputTypeDef",
     "GetNetworkAnalyzerConfigurationRequestRequestTypeDef",
+    "TraceContentOutputTypeDef",
     "GetPartnerAccountRequestRequestTypeDef",
     "SidewalkAccountInfoWithFingerprintTypeDef",
     "GetPositionConfigurationRequestRequestTypeDef",
     "GnssTypeDef",
     "IpTypeDef",
     "WiFiAccessPointTypeDef",
     "GetPositionEstimateResponseTypeDef",
@@ -169,15 +181,17 @@
     "GetWirelessGatewayStatisticsResponseTypeDef",
     "GetWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "GetWirelessGatewayTaskRequestRequestTypeDef",
     "GetWirelessGatewayTaskResponseTypeDef",
     "GlobalIdentityTypeDef",
     "GsmLocalIdTypeDef",
     "ImportedSidewalkDeviceTypeDef",
+    "LoRaWANJoinEventNotificationConfigurationsOutputTypeDef",
     "LoRaWANJoinEventNotificationConfigurationsTypeDef",
+    "LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef",
     "LoRaWANJoinResourceTypeEventConfigurationTypeDef",
     "ListDestinationsRequestRequestTypeDef",
     "ListDeviceProfilesRequestRequestTypeDef",
     "ListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef",
     "ListEventConfigurationsRequestRequestTypeDef",
     "ListFuotaTasksRequestRequestTypeDef",
     "ListMulticastGroupsByFuotaTaskRequestRequestTypeDef",
@@ -188,24 +202,29 @@
     "NetworkAnalyzerConfigurationsTypeDef",
     "ListPartnerAccountsRequestRequestTypeDef",
     "ListPositionConfigurationsRequestRequestTypeDef",
     "ListQueuedMessagesRequestRequestTypeDef",
     "ListServiceProfilesRequestRequestTypeDef",
     "ServiceProfileTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListWirelessDeviceImportTasksRequestRequestTypeDef",
     "ListWirelessDevicesRequestRequestTypeDef",
     "ListWirelessGatewayTaskDefinitionsRequestRequestTypeDef",
     "ListWirelessGatewaysRequestRequestTypeDef",
     "LoRaWANGatewayMetadataTypeDef",
+    "OtaaV10XOutputTypeDef",
+    "OtaaV11OutputTypeDef",
     "OtaaV10XTypeDef",
     "OtaaV11TypeDef",
+    "LoRaWANGatewayVersionOutputTypeDef",
     "LoRaWANGatewayVersionTypeDef",
     "LoRaWANListDeviceTypeDef",
     "LoRaWANMulticastMetadataTypeDef",
+    "LoRaWANMulticastSessionTypeDef",
     "LoRaWANStartFuotaTaskTypeDef",
     "UpdateAbpV10XTypeDef",
     "UpdateAbpV11TypeDef",
     "LteLocalIdTypeDef",
     "LteNmrObjTypeDef",
     "SemtechGnssConfigurationTypeDef",
     "SemtechGnssDetailTypeDef",
@@ -228,142 +247,185 @@
     "UntagResourceRequestRequestTypeDef",
     "UpdateDestinationRequestRequestTypeDef",
     "UpdatePositionRequestRequestTypeDef",
     "UpdateResourcePositionRequestRequestTypeDef",
     "UpdateWirelessGatewayRequestRequestTypeDef",
     "WcdmaLocalIdTypeDef",
     "WcdmaNmrObjTypeDef",
+    "WirelessDeviceEventLogOptionOutputTypeDef",
     "WirelessDeviceEventLogOptionTypeDef",
+    "WirelessGatewayEventLogOptionOutputTypeDef",
     "WirelessGatewayEventLogOptionTypeDef",
+    "AbpV10XOutputTypeDef",
     "AbpV10XTypeDef",
+    "AbpV11OutputTypeDef",
     "AbpV11TypeDef",
     "GetPositionResponseTypeDef",
-    "AssociateAwsAccountWithPartnerAccountResponseTypeDef",
     "AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef",
     "CreateDestinationRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     "StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "AssociateAwsAccountWithPartnerAccountResponseTypeDef",
+    "LoRaWANGatewayOutputTypeDef",
     "LoRaWANGatewayTypeDef",
     "CdmaObjTypeDef",
     "SidewalkDeviceTypeDef",
     "SidewalkListDeviceTypeDef",
+    "ConnectionStatusEventConfigurationOutputTypeDef",
     "ConnectionStatusEventConfigurationTypeDef",
+    "ConnectionStatusResourceTypeEventConfigurationOutputTypeDef",
     "ConnectionStatusResourceTypeEventConfigurationTypeDef",
     "CreateDeviceProfileRequestRequestTypeDef",
     "CreateFuotaTaskRequestRequestTypeDef",
     "UpdateFuotaTaskRequestRequestTypeDef",
     "CreateMulticastGroupRequestRequestTypeDef",
     "UpdateMulticastGroupRequestRequestTypeDef",
     "CreateNetworkAnalyzerConfigurationRequestRequestTypeDef",
-    "GetNetworkAnalyzerConfigurationResponseTypeDef",
     "UpdateNetworkAnalyzerConfigurationRequestRequestTypeDef",
     "CreateServiceProfileRequestRequestTypeDef",
     "SidewalkGetDeviceProfileTypeDef",
     "ListDestinationsResponseTypeDef",
     "ListDeviceProfilesResponseTypeDef",
+    "DeviceRegistrationStateEventConfigurationOutputTypeDef",
+    "MessageDeliveryStatusEventConfigurationOutputTypeDef",
+    "ProximityEventConfigurationOutputTypeDef",
     "DeviceRegistrationStateEventConfigurationTypeDef",
     "MessageDeliveryStatusEventConfigurationTypeDef",
     "ProximityEventConfigurationTypeDef",
+    "DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef",
+    "MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef",
+    "ProximityResourceTypeEventConfigurationOutputTypeDef",
     "DeviceRegistrationStateResourceTypeEventConfigurationTypeDef",
     "MessageDeliveryStatusResourceTypeEventConfigurationTypeDef",
     "ProximityResourceTypeEventConfigurationTypeDef",
+    "FPortsOutputTypeDef",
     "FPortsTypeDef",
     "UpdateFPortsTypeDef",
     "ListFuotaTasksResponseTypeDef",
+    "ParticipatingGatewaysOutputTypeDef",
     "ParticipatingGatewaysTypeDef",
     "GetFuotaTaskResponseTypeDef",
     "GetMulticastGroupResponseTypeDef",
     "GetMulticastGroupSessionResponseTypeDef",
-    "StartMulticastGroupSessionRequestRequestTypeDef",
+    "GetNetworkAnalyzerConfigurationResponseTypeDef",
     "GetPartnerAccountResponseTypeDef",
     "ListPartnerAccountsResponseTypeDef",
     "GetServiceProfileResponseTypeDef",
     "GetWirelessDeviceImportTaskResponseTypeDef",
     "WirelessDeviceImportTaskTypeDef",
     "GsmNmrObjTypeDef",
     "ImportedWirelessDeviceTypeDef",
+    "JoinEventConfigurationOutputTypeDef",
     "JoinEventConfigurationTypeDef",
+    "JoinResourceTypeEventConfigurationOutputTypeDef",
     "JoinResourceTypeEventConfigurationTypeDef",
     "ListMulticastGroupsByFuotaTaskResponseTypeDef",
     "ListMulticastGroupsResponseTypeDef",
     "ListNetworkAnalyzerConfigurationsResponseTypeDef",
     "ListServiceProfilesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "LoRaWANDeviceMetadataTypeDef",
     "LoRaWANGatewayCurrentVersionTypeDef",
-    "LoRaWANUpdateGatewayTaskCreateTypeDef",
+    "LoRaWANUpdateGatewayTaskCreateOutputTypeDef",
     "LoRaWANUpdateGatewayTaskEntryTypeDef",
+    "LoRaWANUpdateGatewayTaskCreateTypeDef",
     "MulticastWirelessMetadataTypeDef",
+    "StartMulticastGroupSessionRequestRequestTypeDef",
     "StartFuotaTaskRequestRequestTypeDef",
     "LteObjTypeDef",
     "PositionSolverConfigurationsTypeDef",
     "PositionSolverDetailsTypeDef",
     "StartSingleWirelessDeviceImportTaskRequestRequestTypeDef",
     "StartWirelessDeviceImportTaskRequestRequestTypeDef",
     "UpdatePartnerAccountRequestRequestTypeDef",
     "UpdateWirelessDeviceImportTaskRequestRequestTypeDef",
     "TdscdmaObjTypeDef",
     "WcdmaObjTypeDef",
+    "WirelessDeviceLogOptionOutputTypeDef",
     "WirelessDeviceLogOptionTypeDef",
+    "WirelessGatewayLogOptionOutputTypeDef",
     "WirelessGatewayLogOptionTypeDef",
-    "CreateWirelessGatewayRequestRequestTypeDef",
     "GetWirelessGatewayResponseTypeDef",
     "WirelessGatewayStatisticsTypeDef",
+    "CreateWirelessGatewayRequestRequestTypeDef",
     "WirelessDeviceStatisticsTypeDef",
     "GetDeviceProfileResponseTypeDef",
+    "LoRaWANDeviceOutputTypeDef",
     "LoRaWANDeviceTypeDef",
     "LoRaWANUpdateDeviceTypeDef",
+    "LoRaWANSendDataToDeviceOutputTypeDef",
     "LoRaWANSendDataToDeviceTypeDef",
     "ListWirelessDeviceImportTasksResponseTypeDef",
     "GsmObjTypeDef",
     "ListDevicesForWirelessDeviceImportTaskResponseTypeDef",
     "EventNotificationItemConfigurationsTypeDef",
     "GetResourceEventConfigurationResponseTypeDef",
     "UpdateResourceEventConfigurationRequestRequestTypeDef",
     "GetEventConfigurationByResourceTypesResponseTypeDef",
     "UpdateEventConfigurationByResourceTypesRequestRequestTypeDef",
     "GetWirelessDeviceStatisticsResponseTypeDef",
     "GetWirelessGatewayFirmwareInformationResponseTypeDef",
-    "UpdateWirelessGatewayTaskCreateTypeDef",
+    "UpdateWirelessGatewayTaskCreateOutputTypeDef",
     "UpdateWirelessGatewayTaskEntryTypeDef",
+    "UpdateWirelessGatewayTaskCreateTypeDef",
     "SendDataToMulticastGroupRequestRequestTypeDef",
     "PutPositionConfigurationRequestRequestTypeDef",
     "GetPositionConfigurationResponseTypeDef",
     "PositionConfigurationItemTypeDef",
     "GetLogLevelsByResourceTypesResponseTypeDef",
     "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
     "ListWirelessGatewaysResponseTypeDef",
     "ListWirelessDevicesResponseTypeDef",
-    "CreateWirelessDeviceRequestRequestTypeDef",
     "GetWirelessDeviceResponseTypeDef",
+    "CreateWirelessDeviceRequestRequestTypeDef",
     "UpdateWirelessDeviceRequestRequestTypeDef",
     "DownlinkQueueMessageTypeDef",
     "WirelessMetadataTypeDef",
     "CellTowersTypeDef",
     "EventConfigurationItemTypeDef",
-    "CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "GetWirelessGatewayTaskDefinitionResponseTypeDef",
     "ListWirelessGatewayTaskDefinitionsResponseTypeDef",
+    "CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "ListPositionConfigurationsResponseTypeDef",
     "ListQueuedMessagesResponseTypeDef",
     "SendDataToWirelessDeviceRequestRequestTypeDef",
     "GetPositionEstimateRequestRequestTypeDef",
     "ListEventConfigurationsResponseTypeDef",
 )
 
+SessionKeysAbpV10XOutputTypeDef = TypedDict(
+    "SessionKeysAbpV10XOutputTypeDef",
+    {
+        "NwkSKey": str,
+        "AppSKey": str,
+    },
+    total=False,
+)
+
 SessionKeysAbpV10XTypeDef = TypedDict(
     "SessionKeysAbpV10XTypeDef",
     {
         "NwkSKey": str,
         "AppSKey": str,
     },
     total=False,
 )
 
+SessionKeysAbpV11OutputTypeDef = TypedDict(
+    "SessionKeysAbpV11OutputTypeDef",
+    {
+        "FNwkSIntKey": str,
+        "SNwkSIntKey": str,
+        "NwkSEncKey": str,
+        "AppSKey": str,
+    },
+    total=False,
+)
+
 SessionKeysAbpV11TypeDef = TypedDict(
     "SessionKeysAbpV11TypeDef",
     {
         "FNwkSIntKey": str,
         "SNwkSIntKey": str,
         "NwkSEncKey": str,
         "AppSKey": str,
@@ -376,14 +438,24 @@
     {
         "HorizontalAccuracy": float,
         "VerticalAccuracy": float,
     },
     total=False,
 )
 
+ApplicationConfigOutputTypeDef = TypedDict(
+    "ApplicationConfigOutputTypeDef",
+    {
+        "FPort": int,
+        "Type": Literal["SemtechGeolocation"],
+        "DestinationName": str,
+    },
+    total=False,
+)
+
 ApplicationConfigTypeDef = TypedDict(
     "ApplicationConfigTypeDef",
     {
         "FPort": int,
         "Type": Literal["SemtechGeolocation"],
         "DestinationName": str,
     },
@@ -403,14 +475,23 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+SidewalkAccountInfoOutputTypeDef = TypedDict(
+    "SidewalkAccountInfoOutputTypeDef",
+    {
+        "AmazonId": str,
+        "AppServerPrivateKey": str,
+    },
+    total=False,
+)
+
 AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef = TypedDict(
     "AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef",
     {
         "Id": str,
         "MulticastGroupId": str,
     },
 )
@@ -459,14 +540,23 @@
     "AssociateWirelessGatewayWithThingRequestRequestTypeDef",
     {
         "Id": str,
         "ThingArn": str,
     },
 )
 
+BeaconingOutputTypeDef = TypedDict(
+    "BeaconingOutputTypeDef",
+    {
+        "DataRate": int,
+        "Frequencies": List[int],
+    },
+    total=False,
+)
+
 BeaconingTypeDef = TypedDict(
     "BeaconingTypeDef",
     {
         "DataRate": int,
         "Frequencies": Sequence[int],
     },
     total=False,
@@ -499,35 +589,49 @@
     {
         "PilotPower": int,
         "BaseStationId": int,
     },
     total=False,
 )
 
-
 class CdmaNmrObjTypeDef(_RequiredCdmaNmrObjTypeDef, _OptionalCdmaNmrObjTypeDef):
     pass
 
-
 CertificateListTypeDef = TypedDict(
     "CertificateListTypeDef",
     {
         "SigningAlg": SigningAlgType,
         "Value": str,
     },
 )
 
+LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef = TypedDict(
+    "LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef",
+    {
+        "GatewayEuiEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
 LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef = TypedDict(
     "LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef",
     {
         "GatewayEuiEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
+LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef = TypedDict(
+    "LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef",
+    {
+        "WirelessGatewayEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
 LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef = TypedDict(
     "LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef",
     {
         "WirelessGatewayEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
@@ -716,21 +820,19 @@
         "FactorySupport": bool,
         "ApId": str,
         "DeviceTypeId": str,
     },
     total=False,
 )
 
-
 class DakCertificateMetadataTypeDef(
     _RequiredDakCertificateMetadataTypeDef, _OptionalDakCertificateMetadataTypeDef
 ):
     pass
 
-
 DeleteDestinationRequestRequestTypeDef = TypedDict(
     "DeleteDestinationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -773,22 +875,20 @@
     "_OptionalDeleteQueuedMessagesRequestRequestTypeDef",
     {
         "WirelessDeviceType": WirelessDeviceTypeType,
     },
     total=False,
 )
 
-
 class DeleteQueuedMessagesRequestRequestTypeDef(
     _RequiredDeleteQueuedMessagesRequestRequestTypeDef,
     _OptionalDeleteQueuedMessagesRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteServiceProfileRequestRequestTypeDef = TypedDict(
     "DeleteServiceProfileRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -837,22 +937,20 @@
     "_OptionalDeregisterWirelessDeviceRequestRequestTypeDef",
     {
         "WirelessDeviceType": WirelessDeviceTypeType,
     },
     total=False,
 )
 
-
 class DeregisterWirelessDeviceRequestRequestTypeDef(
     _RequiredDeregisterWirelessDeviceRequestRequestTypeDef,
     _OptionalDeregisterWirelessDeviceRequestRequestTypeDef,
 ):
     pass
 
-
 DestinationsTypeDef = TypedDict(
     "DestinationsTypeDef",
     {
         "Arn": str,
         "Name": str,
         "ExpressionType": ExpressionTypeType,
         "Expression": str,
@@ -868,22 +966,38 @@
         "Arn": str,
         "Name": str,
         "Id": str,
     },
     total=False,
 )
 
+SidewalkEventNotificationConfigurationsOutputTypeDef = TypedDict(
+    "SidewalkEventNotificationConfigurationsOutputTypeDef",
+    {
+        "AmazonIdEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
 SidewalkEventNotificationConfigurationsTypeDef = TypedDict(
     "SidewalkEventNotificationConfigurationsTypeDef",
     {
         "AmazonIdEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
+SidewalkResourceTypeEventConfigurationOutputTypeDef = TypedDict(
+    "SidewalkResourceTypeEventConfigurationOutputTypeDef",
+    {
+        "WirelessDeviceEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
 SidewalkResourceTypeEventConfigurationTypeDef = TypedDict(
     "SidewalkResourceTypeEventConfigurationTypeDef",
     {
         "WirelessDeviceEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
@@ -937,14 +1051,24 @@
 DisassociateWirelessGatewayFromThingRequestRequestTypeDef = TypedDict(
     "DisassociateWirelessGatewayFromThingRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+PositioningOutputTypeDef = TypedDict(
+    "PositioningOutputTypeDef",
+    {
+        "ClockSync": int,
+        "Stream": int,
+        "Gnss": int,
+    },
+    total=False,
+)
+
 PositioningTypeDef = TypedDict(
     "PositioningTypeDef",
     {
         "ClockSync": int,
         "Stream": int,
         "Gnss": int,
     },
@@ -957,14 +1081,22 @@
         "Id": str,
         "Arn": str,
         "Name": str,
     },
     total=False,
 )
 
+GatewayListItemOutputTypeDef = TypedDict(
+    "GatewayListItemOutputTypeDef",
+    {
+        "GatewayId": str,
+        "DownlinkFrequency": int,
+    },
+)
+
 GatewayListItemTypeDef = TypedDict(
     "GatewayListItemTypeDef",
     {
         "GatewayId": str,
         "DownlinkFrequency": int,
     },
 )
@@ -992,14 +1124,40 @@
 GetDeviceProfileRequestRequestTypeDef = TypedDict(
     "GetDeviceProfileRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+LoRaWANDeviceProfileOutputTypeDef = TypedDict(
+    "LoRaWANDeviceProfileOutputTypeDef",
+    {
+        "SupportsClassB": bool,
+        "ClassBTimeout": int,
+        "PingSlotPeriod": int,
+        "PingSlotDr": int,
+        "PingSlotFreq": int,
+        "SupportsClassC": bool,
+        "ClassCTimeout": int,
+        "MacVersion": str,
+        "RegParamsRevision": str,
+        "RxDelay1": int,
+        "RxDrOffset1": int,
+        "RxDataRate2": int,
+        "RxFreq2": int,
+        "FactoryPresetFreqsList": List[int],
+        "MaxEirp": int,
+        "MaxDutyCycle": int,
+        "RfRegion": str,
+        "SupportsJoin": bool,
+        "Supports32BitFCnt": bool,
+    },
+    total=False,
+)
+
 GetFuotaTaskRequestRequestTypeDef = TypedDict(
     "GetFuotaTaskRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1033,16 +1191,16 @@
 GetMulticastGroupSessionRequestRequestTypeDef = TypedDict(
     "GetMulticastGroupSessionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-LoRaWANMulticastSessionTypeDef = TypedDict(
-    "LoRaWANMulticastSessionTypeDef",
+LoRaWANMulticastSessionOutputTypeDef = TypedDict(
+    "LoRaWANMulticastSessionOutputTypeDef",
     {
         "DlDr": int,
         "DlFreq": int,
         "SessionStartTime": datetime,
         "SessionTimeout": int,
         "PingSlotPeriod": int,
     },
@@ -1052,14 +1210,24 @@
 GetNetworkAnalyzerConfigurationRequestRequestTypeDef = TypedDict(
     "GetNetworkAnalyzerConfigurationRequestRequestTypeDef",
     {
         "ConfigurationName": str,
     },
 )
 
+TraceContentOutputTypeDef = TypedDict(
+    "TraceContentOutputTypeDef",
+    {
+        "WirelessDeviceFrameInfo": WirelessDeviceFrameInfoType,
+        "LogLevel": LogLevelType,
+        "MulticastFrameInfo": MulticastFrameInfoType,
+    },
+    total=False,
+)
+
 GetPartnerAccountRequestRequestTypeDef = TypedDict(
     "GetPartnerAccountRequestRequestTypeDef",
     {
         "PartnerAccountId": str,
         "PartnerType": Literal["Sidewalk"],
     },
 )
@@ -1096,19 +1264,17 @@
         "AssistPosition": Sequence[float],
         "AssistAltitude": float,
         "Use2DSolver": bool,
     },
     total=False,
 )
 
-
 class GnssTypeDef(_RequiredGnssTypeDef, _OptionalGnssTypeDef):
     pass
 
-
 IpTypeDef = TypedDict(
     "IpTypeDef",
     {
         "IpAddress": str,
     },
 )
 
@@ -1147,22 +1313,20 @@
     "_OptionalGetResourceEventConfigurationRequestRequestTypeDef",
     {
         "PartnerType": Literal["Sidewalk"],
     },
     total=False,
 )
 
-
 class GetResourceEventConfigurationRequestRequestTypeDef(
     _RequiredGetResourceEventConfigurationRequestRequestTypeDef,
     _OptionalGetResourceEventConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 GetResourceLogLevelRequestRequestTypeDef = TypedDict(
     "GetResourceLogLevelRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": str,
     },
 )
@@ -1381,22 +1545,38 @@
         "OnboardingStatus": OnboardStatusType,
         "OnboardingStatusReason": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
+LoRaWANJoinEventNotificationConfigurationsOutputTypeDef = TypedDict(
+    "LoRaWANJoinEventNotificationConfigurationsOutputTypeDef",
+    {
+        "DevEuiEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
 LoRaWANJoinEventNotificationConfigurationsTypeDef = TypedDict(
     "LoRaWANJoinEventNotificationConfigurationsTypeDef",
     {
         "DevEuiEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
+LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef = TypedDict(
+    "LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef",
+    {
+        "WirelessDeviceEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
 LoRaWANJoinResourceTypeEventConfigurationTypeDef = TypedDict(
     "LoRaWANJoinResourceTypeEventConfigurationTypeDef",
     {
         "WirelessDeviceEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
@@ -1432,22 +1612,20 @@
         "MaxResults": int,
         "NextToken": str,
         "Status": OnboardStatusType,
     },
     total=False,
 )
 
-
 class ListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef(
     _RequiredListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef,
     _OptionalListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListEventConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListEventConfigurationsRequestRequestTypeDef",
     {
         "ResourceType": EventNotificationResourceTypeType,
     },
 )
 _OptionalListEventConfigurationsRequestRequestTypeDef = TypedDict(
@@ -1455,22 +1633,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListEventConfigurationsRequestRequestTypeDef(
     _RequiredListEventConfigurationsRequestRequestTypeDef,
     _OptionalListEventConfigurationsRequestRequestTypeDef,
 ):
     pass
 
-
 ListFuotaTasksRequestRequestTypeDef = TypedDict(
     "ListFuotaTasksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1487,22 +1663,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListMulticastGroupsByFuotaTaskRequestRequestTypeDef(
     _RequiredListMulticastGroupsByFuotaTaskRequestRequestTypeDef,
     _OptionalListMulticastGroupsByFuotaTaskRequestRequestTypeDef,
 ):
     pass
 
-
 MulticastGroupByFuotaTaskTypeDef = TypedDict(
     "MulticastGroupByFuotaTaskTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
@@ -1575,22 +1749,20 @@
         "NextToken": str,
         "MaxResults": int,
         "WirelessDeviceType": WirelessDeviceTypeType,
     },
     total=False,
 )
 
-
 class ListQueuedMessagesRequestRequestTypeDef(
     _RequiredListQueuedMessagesRequestRequestTypeDef,
     _OptionalListQueuedMessagesRequestRequestTypeDef,
 ):
     pass
 
-
 ListServiceProfilesRequestRequestTypeDef = TypedDict(
     "ListServiceProfilesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1609,14 +1781,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 ListWirelessDeviceImportTasksRequestRequestTypeDef = TypedDict(
     "ListWirelessDeviceImportTasksRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1662,14 +1842,34 @@
         "GatewayEui": str,
         "Snr": float,
         "Rssi": float,
     },
     total=False,
 )
 
+OtaaV10XOutputTypeDef = TypedDict(
+    "OtaaV10XOutputTypeDef",
+    {
+        "AppKey": str,
+        "AppEui": str,
+        "GenAppKey": str,
+    },
+    total=False,
+)
+
+OtaaV11OutputTypeDef = TypedDict(
+    "OtaaV11OutputTypeDef",
+    {
+        "AppKey": str,
+        "NwkKey": str,
+        "JoinEui": str,
+    },
+    total=False,
+)
+
 OtaaV10XTypeDef = TypedDict(
     "OtaaV10XTypeDef",
     {
         "AppKey": str,
         "AppEui": str,
         "GenAppKey": str,
     },
@@ -1682,14 +1882,24 @@
         "AppKey": str,
         "NwkKey": str,
         "JoinEui": str,
     },
     total=False,
 )
 
+LoRaWANGatewayVersionOutputTypeDef = TypedDict(
+    "LoRaWANGatewayVersionOutputTypeDef",
+    {
+        "PackageVersion": str,
+        "Model": str,
+        "Station": str,
+    },
+    total=False,
+)
+
 LoRaWANGatewayVersionTypeDef = TypedDict(
     "LoRaWANGatewayVersionTypeDef",
     {
         "PackageVersion": str,
         "Model": str,
         "Station": str,
     },
@@ -1708,14 +1918,26 @@
     "LoRaWANMulticastMetadataTypeDef",
     {
         "FPort": int,
     },
     total=False,
 )
 
+LoRaWANMulticastSessionTypeDef = TypedDict(
+    "LoRaWANMulticastSessionTypeDef",
+    {
+        "DlDr": int,
+        "DlFreq": int,
+        "SessionStartTime": Union[datetime, str],
+        "SessionTimeout": int,
+        "PingSlotPeriod": int,
+    },
+    total=False,
+)
+
 LoRaWANStartFuotaTaskTypeDef = TypedDict(
     "LoRaWANStartFuotaTaskTypeDef",
     {
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
@@ -1757,19 +1979,17 @@
     {
         "Rsrp": int,
         "Rsrq": float,
     },
     total=False,
 )
 
-
 class LteNmrObjTypeDef(_RequiredLteNmrObjTypeDef, _OptionalLteNmrObjTypeDef):
     pass
 
-
 SemtechGnssConfigurationTypeDef = TypedDict(
     "SemtechGnssConfigurationTypeDef",
     {
         "Status": PositionConfigurationStatusType,
         "Fec": PositionConfigurationFecType,
     },
 )
@@ -1911,19 +2131,17 @@
         "UtranCid": int,
         "Rscp": int,
         "PathLoss": int,
     },
     total=False,
 )
 
-
 class TdscdmaNmrObjTypeDef(_RequiredTdscdmaNmrObjTypeDef, _OptionalTdscdmaNmrObjTypeDef):
     pass
 
-
 TestWirelessDeviceRequestRequestTypeDef = TypedDict(
     "TestWirelessDeviceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1956,21 +2174,19 @@
         "Expression": str,
         "Description": str,
         "RoleArn": str,
     },
     total=False,
 )
 
-
 class UpdateDestinationRequestRequestTypeDef(
     _RequiredUpdateDestinationRequestRequestTypeDef, _OptionalUpdateDestinationRequestRequestTypeDef
 ):
     pass
 
-
 UpdatePositionRequestRequestTypeDef = TypedDict(
     "UpdatePositionRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": PositionResourceTypeType,
         "Position": Sequence[float],
     },
@@ -1987,22 +2203,20 @@
     "_OptionalUpdateResourcePositionRequestRequestTypeDef",
     {
         "GeoJsonPayload": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
-
 class UpdateResourcePositionRequestRequestTypeDef(
     _RequiredUpdateResourcePositionRequestRequestTypeDef,
     _OptionalUpdateResourcePositionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateWirelessGatewayRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWirelessGatewayRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateWirelessGatewayRequestRequestTypeDef = TypedDict(
@@ -2013,22 +2227,20 @@
         "JoinEuiFilters": Sequence[Sequence[str]],
         "NetIdFilters": Sequence[str],
         "MaxEirp": float,
     },
     total=False,
 )
 
-
 class UpdateWirelessGatewayRequestRequestTypeDef(
     _RequiredUpdateWirelessGatewayRequestRequestTypeDef,
     _OptionalUpdateWirelessGatewayRequestRequestTypeDef,
 ):
     pass
 
-
 WcdmaLocalIdTypeDef = TypedDict(
     "WcdmaLocalIdTypeDef",
     {
         "Uarfcndl": int,
         "Psc": int,
     },
 )
@@ -2046,45 +2258,79 @@
     {
         "Rscp": int,
         "PathLoss": int,
     },
     total=False,
 )
 
-
 class WcdmaNmrObjTypeDef(_RequiredWcdmaNmrObjTypeDef, _OptionalWcdmaNmrObjTypeDef):
     pass
 
+WirelessDeviceEventLogOptionOutputTypeDef = TypedDict(
+    "WirelessDeviceEventLogOptionOutputTypeDef",
+    {
+        "Event": WirelessDeviceEventType,
+        "LogLevel": LogLevelType,
+    },
+)
 
 WirelessDeviceEventLogOptionTypeDef = TypedDict(
     "WirelessDeviceEventLogOptionTypeDef",
     {
         "Event": WirelessDeviceEventType,
         "LogLevel": LogLevelType,
     },
 )
 
+WirelessGatewayEventLogOptionOutputTypeDef = TypedDict(
+    "WirelessGatewayEventLogOptionOutputTypeDef",
+    {
+        "Event": WirelessGatewayEventType,
+        "LogLevel": LogLevelType,
+    },
+)
+
 WirelessGatewayEventLogOptionTypeDef = TypedDict(
     "WirelessGatewayEventLogOptionTypeDef",
     {
         "Event": WirelessGatewayEventType,
         "LogLevel": LogLevelType,
     },
 )
 
+AbpV10XOutputTypeDef = TypedDict(
+    "AbpV10XOutputTypeDef",
+    {
+        "DevAddr": str,
+        "SessionKeys": SessionKeysAbpV10XOutputTypeDef,
+        "FCntStart": int,
+    },
+    total=False,
+)
+
 AbpV10XTypeDef = TypedDict(
     "AbpV10XTypeDef",
     {
         "DevAddr": str,
         "SessionKeys": SessionKeysAbpV10XTypeDef,
         "FCntStart": int,
     },
     total=False,
 )
 
+AbpV11OutputTypeDef = TypedDict(
+    "AbpV11OutputTypeDef",
+    {
+        "DevAddr": str,
+        "SessionKeys": SessionKeysAbpV11OutputTypeDef,
+        "FCntStart": int,
+    },
+    total=False,
+)
+
 AbpV11TypeDef = TypedDict(
     "AbpV11TypeDef",
     {
         "DevAddr": str,
         "SessionKeys": SessionKeysAbpV11TypeDef,
         "FCntStart": int,
     },
@@ -2100,23 +2346,14 @@
         "SolverProvider": Literal["Semtech"],
         "SolverVersion": str,
         "Timestamp": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AssociateAwsAccountWithPartnerAccountResponseTypeDef = TypedDict(
-    "AssociateAwsAccountWithPartnerAccountResponseTypeDef",
-    {
-        "Sidewalk": SidewalkAccountInfoTypeDef,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef",
     {
         "Sidewalk": SidewalkAccountInfoTypeDef,
     },
 )
 _OptionalAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef = TypedDict(
@@ -2124,22 +2361,20 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef(
     _RequiredAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef,
     _OptionalAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDestinationRequestRequestTypeDef",
     {
         "Name": str,
         "ExpressionType": ExpressionTypeType,
         "Expression": str,
         "RoleArn": str,
@@ -2151,29 +2386,19 @@
         "Description": str,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class CreateDestinationRequestRequestTypeDef(
     _RequiredCreateDestinationRequestRequestTypeDef, _OptionalCreateDestinationRequestRequestTypeDef
 ):
     pass
 
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef = TypedDict(
     "_RequiredStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef = TypedDict(
@@ -2181,22 +2406,20 @@
     {
         "QueryString": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef(
     _RequiredStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     _OptionalStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef = TypedDict(
     "_RequiredStartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalStartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef = TypedDict(
@@ -2204,30 +2427,51 @@
     {
         "QueryString": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef(
     _RequiredStartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
     _OptionalStartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+AssociateAwsAccountWithPartnerAccountResponseTypeDef = TypedDict(
+    "AssociateAwsAccountWithPartnerAccountResponseTypeDef",
+    {
+        "Sidewalk": SidewalkAccountInfoOutputTypeDef,
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+LoRaWANGatewayOutputTypeDef = TypedDict(
+    "LoRaWANGatewayOutputTypeDef",
+    {
+        "GatewayEui": str,
+        "RfRegion": str,
+        "JoinEuiFilters": List[List[str]],
+        "NetIdFilters": List[str],
+        "SubBands": List[int],
+        "Beaconing": BeaconingOutputTypeDef,
+        "MaxEirp": float,
+    },
+    total=False,
+)
+
 LoRaWANGatewayTypeDef = TypedDict(
     "LoRaWANGatewayTypeDef",
     {
         "GatewayEui": str,
         "RfRegion": str,
         "JoinEuiFilters": Sequence[Sequence[str]],
         "NetIdFilters": Sequence[str],
@@ -2255,19 +2499,17 @@
         "BaseLat": float,
         "BaseLng": float,
         "CdmaNmr": Sequence[CdmaNmrObjTypeDef],
     },
     total=False,
 )
 
-
 class CdmaObjTypeDef(_RequiredCdmaObjTypeDef, _OptionalCdmaObjTypeDef):
     pass
 
-
 SidewalkDeviceTypeDef = TypedDict(
     "SidewalkDeviceTypeDef",
     {
         "AmazonId": str,
         "SidewalkId": str,
         "SidewalkManufacturingSn": str,
         "DeviceCertificates": List[CertificateListTypeDef],
@@ -2288,23 +2530,40 @@
         "DeviceCertificates": List[CertificateListTypeDef],
         "DeviceProfileId": str,
         "Status": WirelessDeviceSidewalkStatusType,
     },
     total=False,
 )
 
+ConnectionStatusEventConfigurationOutputTypeDef = TypedDict(
+    "ConnectionStatusEventConfigurationOutputTypeDef",
+    {
+        "LoRaWAN": LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef,
+        "WirelessGatewayIdEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
 ConnectionStatusEventConfigurationTypeDef = TypedDict(
     "ConnectionStatusEventConfigurationTypeDef",
     {
         "LoRaWAN": LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef,
         "WirelessGatewayIdEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
+ConnectionStatusResourceTypeEventConfigurationOutputTypeDef = TypedDict(
+    "ConnectionStatusResourceTypeEventConfigurationOutputTypeDef",
+    {
+        "LoRaWAN": LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ConnectionStatusResourceTypeEventConfigurationTypeDef = TypedDict(
     "ConnectionStatusResourceTypeEventConfigurationTypeDef",
     {
         "LoRaWAN": LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef,
     },
     total=False,
 )
@@ -2339,21 +2598,19 @@
         "RedundancyPercent": int,
         "FragmentSizeBytes": int,
         "FragmentIntervalMS": int,
     },
     total=False,
 )
 
-
 class CreateFuotaTaskRequestRequestTypeDef(
     _RequiredCreateFuotaTaskRequestRequestTypeDef, _OptionalCreateFuotaTaskRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateFuotaTaskRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFuotaTaskRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateFuotaTaskRequestRequestTypeDef = TypedDict(
@@ -2367,21 +2624,19 @@
         "RedundancyPercent": int,
         "FragmentSizeBytes": int,
         "FragmentIntervalMS": int,
     },
     total=False,
 )
 
-
 class UpdateFuotaTaskRequestRequestTypeDef(
     _RequiredUpdateFuotaTaskRequestRequestTypeDef, _OptionalUpdateFuotaTaskRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateMulticastGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMulticastGroupRequestRequestTypeDef",
     {
         "LoRaWAN": LoRaWANMulticastTypeDef,
     },
 )
 _OptionalCreateMulticastGroupRequestRequestTypeDef = TypedDict(
@@ -2391,22 +2646,20 @@
         "Description": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMulticastGroupRequestRequestTypeDef(
     _RequiredCreateMulticastGroupRequestRequestTypeDef,
     _OptionalCreateMulticastGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateMulticastGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMulticastGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateMulticastGroupRequestRequestTypeDef = TypedDict(
@@ -2415,22 +2668,20 @@
         "Name": str,
         "Description": str,
         "LoRaWAN": LoRaWANMulticastTypeDef,
     },
     total=False,
 )
 
-
 class UpdateMulticastGroupRequestRequestTypeDef(
     _RequiredUpdateMulticastGroupRequestRequestTypeDef,
     _OptionalUpdateMulticastGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateNetworkAnalyzerConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNetworkAnalyzerConfigurationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateNetworkAnalyzerConfigurationRequestRequestTypeDef = TypedDict(
@@ -2443,36 +2694,20 @@
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
         "MulticastGroups": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateNetworkAnalyzerConfigurationRequestRequestTypeDef(
     _RequiredCreateNetworkAnalyzerConfigurationRequestRequestTypeDef,
     _OptionalCreateNetworkAnalyzerConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
-GetNetworkAnalyzerConfigurationResponseTypeDef = TypedDict(
-    "GetNetworkAnalyzerConfigurationResponseTypeDef",
-    {
-        "TraceContent": TraceContentTypeDef,
-        "WirelessDevices": List[str],
-        "WirelessGateways": List[str],
-        "Description": str,
-        "Arn": str,
-        "Name": str,
-        "MulticastGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef",
     {
         "ConfigurationName": str,
     },
 )
 _OptionalUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef = TypedDict(
@@ -2486,22 +2721,20 @@
         "Description": str,
         "MulticastGroupsToAdd": Sequence[str],
         "MulticastGroupsToRemove": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateNetworkAnalyzerConfigurationRequestRequestTypeDef(
     _RequiredUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef,
     _OptionalUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 CreateServiceProfileRequestRequestTypeDef = TypedDict(
     "CreateServiceProfileRequestRequestTypeDef",
     {
         "Name": str,
         "LoRaWAN": LoRaWANServiceProfileTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
@@ -2533,14 +2766,41 @@
     {
         "NextToken": str,
         "DeviceProfileList": List[DeviceProfileTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DeviceRegistrationStateEventConfigurationOutputTypeDef = TypedDict(
+    "DeviceRegistrationStateEventConfigurationOutputTypeDef",
+    {
+        "Sidewalk": SidewalkEventNotificationConfigurationsOutputTypeDef,
+        "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
+MessageDeliveryStatusEventConfigurationOutputTypeDef = TypedDict(
+    "MessageDeliveryStatusEventConfigurationOutputTypeDef",
+    {
+        "Sidewalk": SidewalkEventNotificationConfigurationsOutputTypeDef,
+        "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
+ProximityEventConfigurationOutputTypeDef = TypedDict(
+    "ProximityEventConfigurationOutputTypeDef",
+    {
+        "Sidewalk": SidewalkEventNotificationConfigurationsOutputTypeDef,
+        "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
 DeviceRegistrationStateEventConfigurationTypeDef = TypedDict(
     "DeviceRegistrationStateEventConfigurationTypeDef",
     {
         "Sidewalk": SidewalkEventNotificationConfigurationsTypeDef,
         "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
@@ -2560,14 +2820,38 @@
     {
         "Sidewalk": SidewalkEventNotificationConfigurationsTypeDef,
         "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
+DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef = TypedDict(
+    "DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef",
+    {
+        "Sidewalk": SidewalkResourceTypeEventConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef = TypedDict(
+    "MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef",
+    {
+        "Sidewalk": SidewalkResourceTypeEventConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+ProximityResourceTypeEventConfigurationOutputTypeDef = TypedDict(
+    "ProximityResourceTypeEventConfigurationOutputTypeDef",
+    {
+        "Sidewalk": SidewalkResourceTypeEventConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 DeviceRegistrationStateResourceTypeEventConfigurationTypeDef = TypedDict(
     "DeviceRegistrationStateResourceTypeEventConfigurationTypeDef",
     {
         "Sidewalk": SidewalkResourceTypeEventConfigurationTypeDef,
     },
     total=False,
 )
@@ -2584,14 +2868,26 @@
     "ProximityResourceTypeEventConfigurationTypeDef",
     {
         "Sidewalk": SidewalkResourceTypeEventConfigurationTypeDef,
     },
     total=False,
 )
 
+FPortsOutputTypeDef = TypedDict(
+    "FPortsOutputTypeDef",
+    {
+        "Fuota": int,
+        "Multicast": int,
+        "ClockSync": int,
+        "Positioning": PositioningOutputTypeDef,
+        "Applications": List[ApplicationConfigOutputTypeDef],
+    },
+    total=False,
+)
+
 FPortsTypeDef = TypedDict(
     "FPortsTypeDef",
     {
         "Fuota": int,
         "Multicast": int,
         "ClockSync": int,
         "Positioning": PositioningTypeDef,
@@ -2614,19 +2910,28 @@
     {
         "NextToken": str,
         "FuotaTaskList": List[FuotaTaskTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ParticipatingGatewaysOutputTypeDef = TypedDict(
+    "ParticipatingGatewaysOutputTypeDef",
+    {
+        "DownlinkMode": DownlinkModeType,
+        "GatewayList": List[GatewayListItemOutputTypeDef],
+        "TransmissionInterval": int,
+    },
+)
+
 ParticipatingGatewaysTypeDef = TypedDict(
     "ParticipatingGatewaysTypeDef",
     {
         "DownlinkMode": DownlinkModeType,
-        "GatewayList": List[GatewayListItemTypeDef],
+        "GatewayList": Sequence[GatewayListItemTypeDef],
         "TransmissionInterval": int,
     },
 )
 
 GetFuotaTaskResponseTypeDef = TypedDict(
     "GetFuotaTaskResponseTypeDef",
     {
@@ -2659,24 +2964,30 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMulticastGroupSessionResponseTypeDef = TypedDict(
     "GetMulticastGroupSessionResponseTypeDef",
     {
-        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
+        "LoRaWAN": LoRaWANMulticastSessionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartMulticastGroupSessionRequestRequestTypeDef = TypedDict(
-    "StartMulticastGroupSessionRequestRequestTypeDef",
+GetNetworkAnalyzerConfigurationResponseTypeDef = TypedDict(
+    "GetNetworkAnalyzerConfigurationResponseTypeDef",
     {
-        "Id": str,
-        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
+        "TraceContent": TraceContentOutputTypeDef,
+        "WirelessDevices": List[str],
+        "WirelessGateways": List[str],
+        "Description": str,
+        "Arn": str,
+        "Name": str,
+        "MulticastGroups": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPartnerAccountResponseTypeDef = TypedDict(
     "GetPartnerAccountResponseTypeDef",
     {
         "Sidewalk": SidewalkAccountInfoWithFingerprintTypeDef,
@@ -2753,36 +3064,51 @@
     {
         "RxLevel": int,
         "GlobalIdentity": GlobalIdentityTypeDef,
     },
     total=False,
 )
 
-
 class GsmNmrObjTypeDef(_RequiredGsmNmrObjTypeDef, _OptionalGsmNmrObjTypeDef):
     pass
 
-
 ImportedWirelessDeviceTypeDef = TypedDict(
     "ImportedWirelessDeviceTypeDef",
     {
         "Sidewalk": ImportedSidewalkDeviceTypeDef,
     },
     total=False,
 )
 
+JoinEventConfigurationOutputTypeDef = TypedDict(
+    "JoinEventConfigurationOutputTypeDef",
+    {
+        "LoRaWAN": LoRaWANJoinEventNotificationConfigurationsOutputTypeDef,
+        "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
 JoinEventConfigurationTypeDef = TypedDict(
     "JoinEventConfigurationTypeDef",
     {
         "LoRaWAN": LoRaWANJoinEventNotificationConfigurationsTypeDef,
         "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
+JoinResourceTypeEventConfigurationOutputTypeDef = TypedDict(
+    "JoinResourceTypeEventConfigurationOutputTypeDef",
+    {
+        "LoRaWAN": LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 JoinResourceTypeEventConfigurationTypeDef = TypedDict(
     "JoinResourceTypeEventConfigurationTypeDef",
     {
         "LoRaWAN": LoRaWANJoinResourceTypeEventConfigurationTypeDef,
     },
     total=False,
 )
@@ -2819,14 +3145,22 @@
     {
         "NextToken": str,
         "ServiceProfileList": List[ServiceProfileTypeDef],
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
 LoRaWANDeviceMetadataTypeDef = TypedDict(
     "LoRaWANDeviceMetadataTypeDef",
     {
         "DevEui": str,
         "FPort": int,
         "DataRate": int,
         "Frequency": int,
@@ -2835,68 +3169,85 @@
     },
     total=False,
 )
 
 LoRaWANGatewayCurrentVersionTypeDef = TypedDict(
     "LoRaWANGatewayCurrentVersionTypeDef",
     {
-        "CurrentVersion": LoRaWANGatewayVersionTypeDef,
+        "CurrentVersion": LoRaWANGatewayVersionOutputTypeDef,
     },
     total=False,
 )
 
-LoRaWANUpdateGatewayTaskCreateTypeDef = TypedDict(
-    "LoRaWANUpdateGatewayTaskCreateTypeDef",
+LoRaWANUpdateGatewayTaskCreateOutputTypeDef = TypedDict(
+    "LoRaWANUpdateGatewayTaskCreateOutputTypeDef",
     {
         "UpdateSignature": str,
         "SigKeyCrc": int,
-        "CurrentVersion": LoRaWANGatewayVersionTypeDef,
-        "UpdateVersion": LoRaWANGatewayVersionTypeDef,
+        "CurrentVersion": LoRaWANGatewayVersionOutputTypeDef,
+        "UpdateVersion": LoRaWANGatewayVersionOutputTypeDef,
     },
     total=False,
 )
 
 LoRaWANUpdateGatewayTaskEntryTypeDef = TypedDict(
     "LoRaWANUpdateGatewayTaskEntryTypeDef",
     {
+        "CurrentVersion": LoRaWANGatewayVersionOutputTypeDef,
+        "UpdateVersion": LoRaWANGatewayVersionOutputTypeDef,
+    },
+    total=False,
+)
+
+LoRaWANUpdateGatewayTaskCreateTypeDef = TypedDict(
+    "LoRaWANUpdateGatewayTaskCreateTypeDef",
+    {
+        "UpdateSignature": str,
+        "SigKeyCrc": int,
         "CurrentVersion": LoRaWANGatewayVersionTypeDef,
         "UpdateVersion": LoRaWANGatewayVersionTypeDef,
     },
     total=False,
 )
 
 MulticastWirelessMetadataTypeDef = TypedDict(
     "MulticastWirelessMetadataTypeDef",
     {
         "LoRaWAN": LoRaWANMulticastMetadataTypeDef,
     },
     total=False,
 )
 
+StartMulticastGroupSessionRequestRequestTypeDef = TypedDict(
+    "StartMulticastGroupSessionRequestRequestTypeDef",
+    {
+        "Id": str,
+        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
+    },
+)
+
 _RequiredStartFuotaTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartFuotaTaskRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalStartFuotaTaskRequestRequestTypeDef = TypedDict(
     "_OptionalStartFuotaTaskRequestRequestTypeDef",
     {
         "LoRaWAN": LoRaWANStartFuotaTaskTypeDef,
     },
     total=False,
 )
 
-
 class StartFuotaTaskRequestRequestTypeDef(
     _RequiredStartFuotaTaskRequestRequestTypeDef, _OptionalStartFuotaTaskRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredLteObjTypeDef = TypedDict(
     "_RequiredLteObjTypeDef",
     {
         "Mcc": int,
         "Mnc": int,
         "EutranCid": int,
     },
@@ -2911,19 +3262,17 @@
         "Rsrq": float,
         "NrCapable": bool,
         "LteNmr": Sequence[LteNmrObjTypeDef],
     },
     total=False,
 )
 
-
 class LteObjTypeDef(_RequiredLteObjTypeDef, _OptionalLteObjTypeDef):
     pass
 
-
 PositionSolverConfigurationsTypeDef = TypedDict(
     "PositionSolverConfigurationsTypeDef",
     {
         "SemtechGnss": SemtechGnssConfigurationTypeDef,
     },
     total=False,
 )
@@ -2949,22 +3298,20 @@
         "ClientRequestToken": str,
         "DeviceName": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartSingleWirelessDeviceImportTaskRequestRequestTypeDef(
     _RequiredStartSingleWirelessDeviceImportTaskRequestRequestTypeDef,
     _OptionalStartSingleWirelessDeviceImportTaskRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartWirelessDeviceImportTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartWirelessDeviceImportTaskRequestRequestTypeDef",
     {
         "DestinationName": str,
         "Sidewalk": SidewalkStartImportInfoTypeDef,
     },
 )
@@ -2973,22 +3320,20 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartWirelessDeviceImportTaskRequestRequestTypeDef(
     _RequiredStartWirelessDeviceImportTaskRequestRequestTypeDef,
     _OptionalStartWirelessDeviceImportTaskRequestRequestTypeDef,
 ):
     pass
 
-
 UpdatePartnerAccountRequestRequestTypeDef = TypedDict(
     "UpdatePartnerAccountRequestRequestTypeDef",
     {
         "Sidewalk": SidewalkUpdateAccountTypeDef,
         "PartnerAccountId": str,
         "PartnerType": Literal["Sidewalk"],
     },
@@ -3019,19 +3364,17 @@
         "Rscp": int,
         "PathLoss": int,
         "TdscdmaNmr": Sequence[TdscdmaNmrObjTypeDef],
     },
     total=False,
 )
 
-
 class TdscdmaObjTypeDef(_RequiredTdscdmaObjTypeDef, _OptionalTdscdmaObjTypeDef):
     pass
 
-
 _RequiredWcdmaObjTypeDef = TypedDict(
     "_RequiredWcdmaObjTypeDef",
     {
         "Mcc": int,
         "Mnc": int,
         "UtranCid": int,
     },
@@ -3044,115 +3387,147 @@
         "Rscp": int,
         "PathLoss": int,
         "WcdmaNmr": Sequence[WcdmaNmrObjTypeDef],
     },
     total=False,
 )
 
-
 class WcdmaObjTypeDef(_RequiredWcdmaObjTypeDef, _OptionalWcdmaObjTypeDef):
     pass
 
+_RequiredWirelessDeviceLogOptionOutputTypeDef = TypedDict(
+    "_RequiredWirelessDeviceLogOptionOutputTypeDef",
+    {
+        "Type": WirelessDeviceTypeType,
+        "LogLevel": LogLevelType,
+    },
+)
+_OptionalWirelessDeviceLogOptionOutputTypeDef = TypedDict(
+    "_OptionalWirelessDeviceLogOptionOutputTypeDef",
+    {
+        "Events": List[WirelessDeviceEventLogOptionOutputTypeDef],
+    },
+    total=False,
+)
+
+class WirelessDeviceLogOptionOutputTypeDef(
+    _RequiredWirelessDeviceLogOptionOutputTypeDef, _OptionalWirelessDeviceLogOptionOutputTypeDef
+):
+    pass
 
 _RequiredWirelessDeviceLogOptionTypeDef = TypedDict(
     "_RequiredWirelessDeviceLogOptionTypeDef",
     {
         "Type": WirelessDeviceTypeType,
         "LogLevel": LogLevelType,
     },
 )
 _OptionalWirelessDeviceLogOptionTypeDef = TypedDict(
     "_OptionalWirelessDeviceLogOptionTypeDef",
     {
-        "Events": List[WirelessDeviceEventLogOptionTypeDef],
+        "Events": Sequence[WirelessDeviceEventLogOptionTypeDef],
     },
     total=False,
 )
 
-
 class WirelessDeviceLogOptionTypeDef(
     _RequiredWirelessDeviceLogOptionTypeDef, _OptionalWirelessDeviceLogOptionTypeDef
 ):
     pass
 
-
-_RequiredWirelessGatewayLogOptionTypeDef = TypedDict(
-    "_RequiredWirelessGatewayLogOptionTypeDef",
+_RequiredWirelessGatewayLogOptionOutputTypeDef = TypedDict(
+    "_RequiredWirelessGatewayLogOptionOutputTypeDef",
     {
         "Type": Literal["LoRaWAN"],
         "LogLevel": LogLevelType,
     },
 )
-_OptionalWirelessGatewayLogOptionTypeDef = TypedDict(
-    "_OptionalWirelessGatewayLogOptionTypeDef",
+_OptionalWirelessGatewayLogOptionOutputTypeDef = TypedDict(
+    "_OptionalWirelessGatewayLogOptionOutputTypeDef",
     {
-        "Events": List[WirelessGatewayEventLogOptionTypeDef],
+        "Events": List[WirelessGatewayEventLogOptionOutputTypeDef],
     },
     total=False,
 )
 
-
-class WirelessGatewayLogOptionTypeDef(
-    _RequiredWirelessGatewayLogOptionTypeDef, _OptionalWirelessGatewayLogOptionTypeDef
+class WirelessGatewayLogOptionOutputTypeDef(
+    _RequiredWirelessGatewayLogOptionOutputTypeDef, _OptionalWirelessGatewayLogOptionOutputTypeDef
 ):
     pass
 
-
-_RequiredCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWirelessGatewayRequestRequestTypeDef",
+_RequiredWirelessGatewayLogOptionTypeDef = TypedDict(
+    "_RequiredWirelessGatewayLogOptionTypeDef",
     {
-        "LoRaWAN": LoRaWANGatewayTypeDef,
+        "Type": Literal["LoRaWAN"],
+        "LogLevel": LogLevelType,
     },
 )
-_OptionalCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWirelessGatewayRequestRequestTypeDef",
+_OptionalWirelessGatewayLogOptionTypeDef = TypedDict(
+    "_OptionalWirelessGatewayLogOptionTypeDef",
     {
-        "Name": str,
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
-        "ClientRequestToken": str,
+        "Events": Sequence[WirelessGatewayEventLogOptionTypeDef],
     },
     total=False,
 )
 
-
-class CreateWirelessGatewayRequestRequestTypeDef(
-    _RequiredCreateWirelessGatewayRequestRequestTypeDef,
-    _OptionalCreateWirelessGatewayRequestRequestTypeDef,
+class WirelessGatewayLogOptionTypeDef(
+    _RequiredWirelessGatewayLogOptionTypeDef, _OptionalWirelessGatewayLogOptionTypeDef
 ):
     pass
 
-
 GetWirelessGatewayResponseTypeDef = TypedDict(
     "GetWirelessGatewayResponseTypeDef",
     {
         "Name": str,
         "Id": str,
         "Description": str,
-        "LoRaWAN": LoRaWANGatewayTypeDef,
+        "LoRaWAN": LoRaWANGatewayOutputTypeDef,
         "Arn": str,
         "ThingName": str,
         "ThingArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WirelessGatewayStatisticsTypeDef = TypedDict(
     "WirelessGatewayStatisticsTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
-        "LoRaWAN": LoRaWANGatewayTypeDef,
+        "LoRaWAN": LoRaWANGatewayOutputTypeDef,
         "LastUplinkReceivedAt": str,
     },
     total=False,
 )
 
+_RequiredCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWirelessGatewayRequestRequestTypeDef",
+    {
+        "LoRaWAN": LoRaWANGatewayTypeDef,
+    },
+)
+_OptionalCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWirelessGatewayRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+class CreateWirelessGatewayRequestRequestTypeDef(
+    _RequiredCreateWirelessGatewayRequestRequestTypeDef,
+    _OptionalCreateWirelessGatewayRequestRequestTypeDef,
+):
+    pass
+
 WirelessDeviceStatisticsTypeDef = TypedDict(
     "WirelessDeviceStatisticsTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Type": WirelessDeviceTypeType,
         "Name": str,
@@ -3169,20 +3544,35 @@
 
 GetDeviceProfileResponseTypeDef = TypedDict(
     "GetDeviceProfileResponseTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Id": str,
-        "LoRaWAN": LoRaWANDeviceProfileTypeDef,
+        "LoRaWAN": LoRaWANDeviceProfileOutputTypeDef,
         "Sidewalk": SidewalkGetDeviceProfileTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LoRaWANDeviceOutputTypeDef = TypedDict(
+    "LoRaWANDeviceOutputTypeDef",
+    {
+        "DevEui": str,
+        "DeviceProfileId": str,
+        "ServiceProfileId": str,
+        "OtaaV1_1": OtaaV11OutputTypeDef,
+        "OtaaV1_0_x": OtaaV10XOutputTypeDef,
+        "AbpV1_1": AbpV11OutputTypeDef,
+        "AbpV1_0_x": AbpV10XOutputTypeDef,
+        "FPorts": FPortsOutputTypeDef,
+    },
+    total=False,
+)
+
 LoRaWANDeviceTypeDef = TypedDict(
     "LoRaWANDeviceTypeDef",
     {
         "DevEui": str,
         "DeviceProfileId": str,
         "ServiceProfileId": str,
         "OtaaV1_1": OtaaV11TypeDef,
@@ -3202,14 +3592,23 @@
         "AbpV1_1": UpdateAbpV11TypeDef,
         "AbpV1_0_x": UpdateAbpV10XTypeDef,
         "FPorts": UpdateFPortsTypeDef,
     },
     total=False,
 )
 
+LoRaWANSendDataToDeviceOutputTypeDef = TypedDict(
+    "LoRaWANSendDataToDeviceOutputTypeDef",
+    {
+        "FPort": int,
+        "ParticipatingGateways": ParticipatingGatewaysOutputTypeDef,
+    },
+    total=False,
+)
+
 LoRaWANSendDataToDeviceTypeDef = TypedDict(
     "LoRaWANSendDataToDeviceTypeDef",
     {
         "FPort": int,
         "ParticipatingGateways": ParticipatingGatewaysTypeDef,
     },
     total=False,
@@ -3240,49 +3639,47 @@
         "GsmTimingAdvance": int,
         "RxLevel": int,
         "GsmNmr": Sequence[GsmNmrObjTypeDef],
     },
     total=False,
 )
 
-
 class GsmObjTypeDef(_RequiredGsmObjTypeDef, _OptionalGsmObjTypeDef):
     pass
 
-
 ListDevicesForWirelessDeviceImportTaskResponseTypeDef = TypedDict(
     "ListDevicesForWirelessDeviceImportTaskResponseTypeDef",
     {
         "NextToken": str,
         "DestinationName": str,
         "ImportedWirelessDeviceList": List[ImportedWirelessDeviceTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventNotificationItemConfigurationsTypeDef = TypedDict(
     "EventNotificationItemConfigurationsTypeDef",
     {
-        "DeviceRegistrationState": DeviceRegistrationStateEventConfigurationTypeDef,
-        "Proximity": ProximityEventConfigurationTypeDef,
-        "Join": JoinEventConfigurationTypeDef,
-        "ConnectionStatus": ConnectionStatusEventConfigurationTypeDef,
-        "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationTypeDef,
+        "DeviceRegistrationState": DeviceRegistrationStateEventConfigurationOutputTypeDef,
+        "Proximity": ProximityEventConfigurationOutputTypeDef,
+        "Join": JoinEventConfigurationOutputTypeDef,
+        "ConnectionStatus": ConnectionStatusEventConfigurationOutputTypeDef,
+        "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 GetResourceEventConfigurationResponseTypeDef = TypedDict(
     "GetResourceEventConfigurationResponseTypeDef",
     {
-        "DeviceRegistrationState": DeviceRegistrationStateEventConfigurationTypeDef,
-        "Proximity": ProximityEventConfigurationTypeDef,
-        "Join": JoinEventConfigurationTypeDef,
-        "ConnectionStatus": ConnectionStatusEventConfigurationTypeDef,
-        "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationTypeDef,
+        "DeviceRegistrationState": DeviceRegistrationStateEventConfigurationOutputTypeDef,
+        "Proximity": ProximityEventConfigurationOutputTypeDef,
+        "Join": JoinEventConfigurationOutputTypeDef,
+        "ConnectionStatus": ConnectionStatusEventConfigurationOutputTypeDef,
+        "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateResourceEventConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceEventConfigurationRequestRequestTypeDef",
     {
@@ -3299,30 +3696,30 @@
         "Join": JoinEventConfigurationTypeDef,
         "ConnectionStatus": ConnectionStatusEventConfigurationTypeDef,
         "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateResourceEventConfigurationRequestRequestTypeDef(
     _RequiredUpdateResourceEventConfigurationRequestRequestTypeDef,
     _OptionalUpdateResourceEventConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 GetEventConfigurationByResourceTypesResponseTypeDef = TypedDict(
     "GetEventConfigurationByResourceTypesResponseTypeDef",
     {
-        "DeviceRegistrationState": DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,
-        "Proximity": ProximityResourceTypeEventConfigurationTypeDef,
-        "Join": JoinResourceTypeEventConfigurationTypeDef,
-        "ConnectionStatus": ConnectionStatusResourceTypeEventConfigurationTypeDef,
-        "MessageDeliveryStatus": MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
+        "DeviceRegistrationState": (
+            DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef
+        ),
+        "Proximity": ProximityResourceTypeEventConfigurationOutputTypeDef,
+        "Join": JoinResourceTypeEventConfigurationOutputTypeDef,
+        "ConnectionStatus": ConnectionStatusResourceTypeEventConfigurationOutputTypeDef,
+        "MessageDeliveryStatus": MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEventConfigurationByResourceTypesRequestRequestTypeDef = TypedDict(
     "UpdateEventConfigurationByResourceTypesRequestRequestTypeDef",
     {
@@ -3350,34 +3747,44 @@
     "GetWirelessGatewayFirmwareInformationResponseTypeDef",
     {
         "LoRaWAN": LoRaWANGatewayCurrentVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateWirelessGatewayTaskCreateTypeDef = TypedDict(
-    "UpdateWirelessGatewayTaskCreateTypeDef",
+UpdateWirelessGatewayTaskCreateOutputTypeDef = TypedDict(
+    "UpdateWirelessGatewayTaskCreateOutputTypeDef",
     {
         "UpdateDataSource": str,
         "UpdateDataRole": str,
-        "LoRaWAN": LoRaWANUpdateGatewayTaskCreateTypeDef,
+        "LoRaWAN": LoRaWANUpdateGatewayTaskCreateOutputTypeDef,
     },
     total=False,
 )
 
 UpdateWirelessGatewayTaskEntryTypeDef = TypedDict(
     "UpdateWirelessGatewayTaskEntryTypeDef",
     {
         "Id": str,
         "LoRaWAN": LoRaWANUpdateGatewayTaskEntryTypeDef,
         "Arn": str,
     },
     total=False,
 )
 
+UpdateWirelessGatewayTaskCreateTypeDef = TypedDict(
+    "UpdateWirelessGatewayTaskCreateTypeDef",
+    {
+        "UpdateDataSource": str,
+        "UpdateDataRole": str,
+        "LoRaWAN": LoRaWANUpdateGatewayTaskCreateTypeDef,
+    },
+    total=False,
+)
+
 SendDataToMulticastGroupRequestRequestTypeDef = TypedDict(
     "SendDataToMulticastGroupRequestRequestTypeDef",
     {
         "Id": str,
         "PayloadData": str,
         "WirelessMetadata": MulticastWirelessMetadataTypeDef,
     },
@@ -3395,22 +3802,20 @@
     {
         "Solvers": PositionSolverConfigurationsTypeDef,
         "Destination": str,
     },
     total=False,
 )
 
-
 class PutPositionConfigurationRequestRequestTypeDef(
     _RequiredPutPositionConfigurationRequestRequestTypeDef,
     _OptionalPutPositionConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 GetPositionConfigurationResponseTypeDef = TypedDict(
     "GetPositionConfigurationResponseTypeDef",
     {
         "Solvers": PositionSolverDetailsTypeDef,
         "Destination": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -3427,16 +3832,16 @@
     total=False,
 )
 
 GetLogLevelsByResourceTypesResponseTypeDef = TypedDict(
     "GetLogLevelsByResourceTypesResponseTypeDef",
     {
         "DefaultLogLevel": LogLevelType,
-        "WirelessGatewayLogOptions": List[WirelessGatewayLogOptionTypeDef],
-        "WirelessDeviceLogOptions": List[WirelessDeviceLogOptionTypeDef],
+        "WirelessGatewayLogOptions": List[WirelessGatewayLogOptionOutputTypeDef],
+        "WirelessDeviceLogOptions": List[WirelessDeviceLogOptionOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateLogLevelsByResourceTypesRequestRequestTypeDef = TypedDict(
     "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
     {
@@ -3461,14 +3866,32 @@
     {
         "NextToken": str,
         "WirelessDeviceList": List[WirelessDeviceStatisticsTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+GetWirelessDeviceResponseTypeDef = TypedDict(
+    "GetWirelessDeviceResponseTypeDef",
+    {
+        "Type": WirelessDeviceTypeType,
+        "Name": str,
+        "Description": str,
+        "DestinationName": str,
+        "Id": str,
+        "Arn": str,
+        "ThingName": str,
+        "ThingArn": str,
+        "LoRaWAN": LoRaWANDeviceOutputTypeDef,
+        "Sidewalk": SidewalkDeviceTypeDef,
+        "Positioning": PositioningConfigStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateWirelessDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWirelessDeviceRequestRequestTypeDef",
     {
         "Type": WirelessDeviceTypeType,
         "DestinationName": str,
     },
 )
@@ -3482,40 +3905,20 @@
         "Tags": Sequence[TagTypeDef],
         "Positioning": PositioningConfigStatusType,
         "Sidewalk": SidewalkCreateWirelessDeviceTypeDef,
     },
     total=False,
 )
 
-
 class CreateWirelessDeviceRequestRequestTypeDef(
     _RequiredCreateWirelessDeviceRequestRequestTypeDef,
     _OptionalCreateWirelessDeviceRequestRequestTypeDef,
 ):
     pass
 
-
-GetWirelessDeviceResponseTypeDef = TypedDict(
-    "GetWirelessDeviceResponseTypeDef",
-    {
-        "Type": WirelessDeviceTypeType,
-        "Name": str,
-        "Description": str,
-        "DestinationName": str,
-        "Id": str,
-        "Arn": str,
-        "ThingName": str,
-        "ThingArn": str,
-        "LoRaWAN": LoRaWANDeviceTypeDef,
-        "Sidewalk": SidewalkDeviceTypeDef,
-        "Positioning": PositioningConfigStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateWirelessDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWirelessDeviceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateWirelessDeviceRequestRequestTypeDef = TypedDict(
@@ -3526,29 +3929,27 @@
         "Description": str,
         "LoRaWAN": LoRaWANUpdateDeviceTypeDef,
         "Positioning": PositioningConfigStatusType,
     },
     total=False,
 )
 
-
 class UpdateWirelessDeviceRequestRequestTypeDef(
     _RequiredUpdateWirelessDeviceRequestRequestTypeDef,
     _OptionalUpdateWirelessDeviceRequestRequestTypeDef,
 ):
     pass
 
-
 DownlinkQueueMessageTypeDef = TypedDict(
     "DownlinkQueueMessageTypeDef",
     {
         "MessageId": str,
         "TransmitMode": int,
         "ReceivedAt": str,
-        "LoRaWAN": LoRaWANSendDataToDeviceTypeDef,
+        "LoRaWAN": LoRaWANSendDataToDeviceOutputTypeDef,
     },
     total=False,
 )
 
 WirelessMetadataTypeDef = TypedDict(
     "WirelessMetadataTypeDef",
     {
@@ -3577,14 +3978,34 @@
         "IdentifierType": IdentifierTypeType,
         "PartnerType": Literal["Sidewalk"],
         "Events": EventNotificationItemConfigurationsTypeDef,
     },
     total=False,
 )
 
+GetWirelessGatewayTaskDefinitionResponseTypeDef = TypedDict(
+    "GetWirelessGatewayTaskDefinitionResponseTypeDef",
+    {
+        "AutoCreateTasks": bool,
+        "Name": str,
+        "Update": UpdateWirelessGatewayTaskCreateOutputTypeDef,
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListWirelessGatewayTaskDefinitionsResponseTypeDef = TypedDict(
+    "ListWirelessGatewayTaskDefinitionsResponseTypeDef",
+    {
+        "NextToken": str,
+        "TaskDefinitions": List[UpdateWirelessGatewayTaskEntryTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     {
         "AutoCreateTasks": bool,
     },
 )
 _OptionalCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef = TypedDict(
@@ -3594,42 +4015,20 @@
         "Update": UpdateWirelessGatewayTaskCreateTypeDef,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef(
     _RequiredCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     _OptionalCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
-GetWirelessGatewayTaskDefinitionResponseTypeDef = TypedDict(
-    "GetWirelessGatewayTaskDefinitionResponseTypeDef",
-    {
-        "AutoCreateTasks": bool,
-        "Name": str,
-        "Update": UpdateWirelessGatewayTaskCreateTypeDef,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListWirelessGatewayTaskDefinitionsResponseTypeDef = TypedDict(
-    "ListWirelessGatewayTaskDefinitionsResponseTypeDef",
-    {
-        "NextToken": str,
-        "TaskDefinitions": List[UpdateWirelessGatewayTaskEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListPositionConfigurationsResponseTypeDef = TypedDict(
     "ListPositionConfigurationsResponseTypeDef",
     {
         "PositionConfigurationList": List[PositionConfigurationItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -3656,22 +4055,20 @@
     "_OptionalSendDataToWirelessDeviceRequestRequestTypeDef",
     {
         "WirelessMetadata": WirelessMetadataTypeDef,
     },
     total=False,
 )
 
-
 class SendDataToWirelessDeviceRequestRequestTypeDef(
     _RequiredSendDataToWirelessDeviceRequestRequestTypeDef,
     _OptionalSendDataToWirelessDeviceRequestRequestTypeDef,
 ):
     pass
 
-
 GetPositionEstimateRequestRequestTypeDef = TypedDict(
     "GetPositionEstimateRequestRequestTypeDef",
     {
         "WiFiAccessPoints": Sequence[WiFiAccessPointTypeDef],
         "CellTowers": CellTowersTypeDef,
         "Ip": IpTypeDef,
         "Gnss": GnssTypeDef,
```

### Comparing `mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless/type_defs.pyi` & `mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless/type_defs.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iotwireless service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iotwireless.type_defs import SessionKeysAbpV10XTypeDef
+    from mypy_boto3_iotwireless.type_defs import SessionKeysAbpV10XOutputTypeDef
 
-    data: SessionKeysAbpV10XTypeDef = {...}
+    data: SessionKeysAbpV10XOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -58,34 +58,42 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "SessionKeysAbpV10XOutputTypeDef",
     "SessionKeysAbpV10XTypeDef",
+    "SessionKeysAbpV11OutputTypeDef",
     "SessionKeysAbpV11TypeDef",
     "AccuracyTypeDef",
+    "ApplicationConfigOutputTypeDef",
     "ApplicationConfigTypeDef",
     "SidewalkAccountInfoTypeDef",
     "TagTypeDef",
+    "SidewalkAccountInfoOutputTypeDef",
     "AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef",
     "AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef",
     "AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     "AssociateWirelessDeviceWithThingRequestRequestTypeDef",
     "AssociateWirelessGatewayWithCertificateRequestRequestTypeDef",
     "AssociateWirelessGatewayWithCertificateResponseTypeDef",
     "AssociateWirelessGatewayWithThingRequestRequestTypeDef",
+    "BeaconingOutputTypeDef",
     "BeaconingTypeDef",
     "CancelMulticastGroupSessionRequestRequestTypeDef",
     "CdmaLocalIdTypeDef",
     "CdmaNmrObjTypeDef",
     "CertificateListTypeDef",
+    "LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef",
     "LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef",
+    "LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef",
     "LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef",
     "CreateDestinationResponseTypeDef",
     "LoRaWANDeviceProfileTypeDef",
     "CreateDeviceProfileResponseTypeDef",
     "LoRaWANFuotaTaskTypeDef",
     "CreateFuotaTaskResponseTypeDef",
     "LoRaWANMulticastTypeDef",
@@ -112,36 +120,42 @@
     "DeleteWirelessDeviceRequestRequestTypeDef",
     "DeleteWirelessGatewayRequestRequestTypeDef",
     "DeleteWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "DeleteWirelessGatewayTaskRequestRequestTypeDef",
     "DeregisterWirelessDeviceRequestRequestTypeDef",
     "DestinationsTypeDef",
     "DeviceProfileTypeDef",
+    "SidewalkEventNotificationConfigurationsOutputTypeDef",
     "SidewalkEventNotificationConfigurationsTypeDef",
+    "SidewalkResourceTypeEventConfigurationOutputTypeDef",
     "SidewalkResourceTypeEventConfigurationTypeDef",
     "DisassociateAwsAccountFromPartnerAccountRequestRequestTypeDef",
     "DisassociateMulticastGroupFromFuotaTaskRequestRequestTypeDef",
     "DisassociateWirelessDeviceFromFuotaTaskRequestRequestTypeDef",
     "DisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef",
     "DisassociateWirelessDeviceFromThingRequestRequestTypeDef",
     "DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef",
     "DisassociateWirelessGatewayFromThingRequestRequestTypeDef",
+    "PositioningOutputTypeDef",
     "PositioningTypeDef",
     "FuotaTaskTypeDef",
+    "GatewayListItemOutputTypeDef",
     "GatewayListItemTypeDef",
     "GetDestinationRequestRequestTypeDef",
     "GetDestinationResponseTypeDef",
     "GetDeviceProfileRequestRequestTypeDef",
+    "LoRaWANDeviceProfileOutputTypeDef",
     "GetFuotaTaskRequestRequestTypeDef",
     "LoRaWANFuotaTaskGetInfoTypeDef",
     "GetMulticastGroupRequestRequestTypeDef",
     "LoRaWANMulticastGetTypeDef",
     "GetMulticastGroupSessionRequestRequestTypeDef",
-    "LoRaWANMulticastSessionTypeDef",
+    "LoRaWANMulticastSessionOutputTypeDef",
     "GetNetworkAnalyzerConfigurationRequestRequestTypeDef",
+    "TraceContentOutputTypeDef",
     "GetPartnerAccountRequestRequestTypeDef",
     "SidewalkAccountInfoWithFingerprintTypeDef",
     "GetPositionConfigurationRequestRequestTypeDef",
     "GnssTypeDef",
     "IpTypeDef",
     "WiFiAccessPointTypeDef",
     "GetPositionEstimateResponseTypeDef",
@@ -168,15 +182,17 @@
     "GetWirelessGatewayStatisticsResponseTypeDef",
     "GetWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "GetWirelessGatewayTaskRequestRequestTypeDef",
     "GetWirelessGatewayTaskResponseTypeDef",
     "GlobalIdentityTypeDef",
     "GsmLocalIdTypeDef",
     "ImportedSidewalkDeviceTypeDef",
+    "LoRaWANJoinEventNotificationConfigurationsOutputTypeDef",
     "LoRaWANJoinEventNotificationConfigurationsTypeDef",
+    "LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef",
     "LoRaWANJoinResourceTypeEventConfigurationTypeDef",
     "ListDestinationsRequestRequestTypeDef",
     "ListDeviceProfilesRequestRequestTypeDef",
     "ListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef",
     "ListEventConfigurationsRequestRequestTypeDef",
     "ListFuotaTasksRequestRequestTypeDef",
     "ListMulticastGroupsByFuotaTaskRequestRequestTypeDef",
@@ -187,24 +203,29 @@
     "NetworkAnalyzerConfigurationsTypeDef",
     "ListPartnerAccountsRequestRequestTypeDef",
     "ListPositionConfigurationsRequestRequestTypeDef",
     "ListQueuedMessagesRequestRequestTypeDef",
     "ListServiceProfilesRequestRequestTypeDef",
     "ServiceProfileTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListWirelessDeviceImportTasksRequestRequestTypeDef",
     "ListWirelessDevicesRequestRequestTypeDef",
     "ListWirelessGatewayTaskDefinitionsRequestRequestTypeDef",
     "ListWirelessGatewaysRequestRequestTypeDef",
     "LoRaWANGatewayMetadataTypeDef",
+    "OtaaV10XOutputTypeDef",
+    "OtaaV11OutputTypeDef",
     "OtaaV10XTypeDef",
     "OtaaV11TypeDef",
+    "LoRaWANGatewayVersionOutputTypeDef",
     "LoRaWANGatewayVersionTypeDef",
     "LoRaWANListDeviceTypeDef",
     "LoRaWANMulticastMetadataTypeDef",
+    "LoRaWANMulticastSessionTypeDef",
     "LoRaWANStartFuotaTaskTypeDef",
     "UpdateAbpV10XTypeDef",
     "UpdateAbpV11TypeDef",
     "LteLocalIdTypeDef",
     "LteNmrObjTypeDef",
     "SemtechGnssConfigurationTypeDef",
     "SemtechGnssDetailTypeDef",
@@ -227,142 +248,185 @@
     "UntagResourceRequestRequestTypeDef",
     "UpdateDestinationRequestRequestTypeDef",
     "UpdatePositionRequestRequestTypeDef",
     "UpdateResourcePositionRequestRequestTypeDef",
     "UpdateWirelessGatewayRequestRequestTypeDef",
     "WcdmaLocalIdTypeDef",
     "WcdmaNmrObjTypeDef",
+    "WirelessDeviceEventLogOptionOutputTypeDef",
     "WirelessDeviceEventLogOptionTypeDef",
+    "WirelessGatewayEventLogOptionOutputTypeDef",
     "WirelessGatewayEventLogOptionTypeDef",
+    "AbpV10XOutputTypeDef",
     "AbpV10XTypeDef",
+    "AbpV11OutputTypeDef",
     "AbpV11TypeDef",
     "GetPositionResponseTypeDef",
-    "AssociateAwsAccountWithPartnerAccountResponseTypeDef",
     "AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef",
     "CreateDestinationRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     "StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "AssociateAwsAccountWithPartnerAccountResponseTypeDef",
+    "LoRaWANGatewayOutputTypeDef",
     "LoRaWANGatewayTypeDef",
     "CdmaObjTypeDef",
     "SidewalkDeviceTypeDef",
     "SidewalkListDeviceTypeDef",
+    "ConnectionStatusEventConfigurationOutputTypeDef",
     "ConnectionStatusEventConfigurationTypeDef",
+    "ConnectionStatusResourceTypeEventConfigurationOutputTypeDef",
     "ConnectionStatusResourceTypeEventConfigurationTypeDef",
     "CreateDeviceProfileRequestRequestTypeDef",
     "CreateFuotaTaskRequestRequestTypeDef",
     "UpdateFuotaTaskRequestRequestTypeDef",
     "CreateMulticastGroupRequestRequestTypeDef",
     "UpdateMulticastGroupRequestRequestTypeDef",
     "CreateNetworkAnalyzerConfigurationRequestRequestTypeDef",
-    "GetNetworkAnalyzerConfigurationResponseTypeDef",
     "UpdateNetworkAnalyzerConfigurationRequestRequestTypeDef",
     "CreateServiceProfileRequestRequestTypeDef",
     "SidewalkGetDeviceProfileTypeDef",
     "ListDestinationsResponseTypeDef",
     "ListDeviceProfilesResponseTypeDef",
+    "DeviceRegistrationStateEventConfigurationOutputTypeDef",
+    "MessageDeliveryStatusEventConfigurationOutputTypeDef",
+    "ProximityEventConfigurationOutputTypeDef",
     "DeviceRegistrationStateEventConfigurationTypeDef",
     "MessageDeliveryStatusEventConfigurationTypeDef",
     "ProximityEventConfigurationTypeDef",
+    "DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef",
+    "MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef",
+    "ProximityResourceTypeEventConfigurationOutputTypeDef",
     "DeviceRegistrationStateResourceTypeEventConfigurationTypeDef",
     "MessageDeliveryStatusResourceTypeEventConfigurationTypeDef",
     "ProximityResourceTypeEventConfigurationTypeDef",
+    "FPortsOutputTypeDef",
     "FPortsTypeDef",
     "UpdateFPortsTypeDef",
     "ListFuotaTasksResponseTypeDef",
+    "ParticipatingGatewaysOutputTypeDef",
     "ParticipatingGatewaysTypeDef",
     "GetFuotaTaskResponseTypeDef",
     "GetMulticastGroupResponseTypeDef",
     "GetMulticastGroupSessionResponseTypeDef",
-    "StartMulticastGroupSessionRequestRequestTypeDef",
+    "GetNetworkAnalyzerConfigurationResponseTypeDef",
     "GetPartnerAccountResponseTypeDef",
     "ListPartnerAccountsResponseTypeDef",
     "GetServiceProfileResponseTypeDef",
     "GetWirelessDeviceImportTaskResponseTypeDef",
     "WirelessDeviceImportTaskTypeDef",
     "GsmNmrObjTypeDef",
     "ImportedWirelessDeviceTypeDef",
+    "JoinEventConfigurationOutputTypeDef",
     "JoinEventConfigurationTypeDef",
+    "JoinResourceTypeEventConfigurationOutputTypeDef",
     "JoinResourceTypeEventConfigurationTypeDef",
     "ListMulticastGroupsByFuotaTaskResponseTypeDef",
     "ListMulticastGroupsResponseTypeDef",
     "ListNetworkAnalyzerConfigurationsResponseTypeDef",
     "ListServiceProfilesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "LoRaWANDeviceMetadataTypeDef",
     "LoRaWANGatewayCurrentVersionTypeDef",
-    "LoRaWANUpdateGatewayTaskCreateTypeDef",
+    "LoRaWANUpdateGatewayTaskCreateOutputTypeDef",
     "LoRaWANUpdateGatewayTaskEntryTypeDef",
+    "LoRaWANUpdateGatewayTaskCreateTypeDef",
     "MulticastWirelessMetadataTypeDef",
+    "StartMulticastGroupSessionRequestRequestTypeDef",
     "StartFuotaTaskRequestRequestTypeDef",
     "LteObjTypeDef",
     "PositionSolverConfigurationsTypeDef",
     "PositionSolverDetailsTypeDef",
     "StartSingleWirelessDeviceImportTaskRequestRequestTypeDef",
     "StartWirelessDeviceImportTaskRequestRequestTypeDef",
     "UpdatePartnerAccountRequestRequestTypeDef",
     "UpdateWirelessDeviceImportTaskRequestRequestTypeDef",
     "TdscdmaObjTypeDef",
     "WcdmaObjTypeDef",
+    "WirelessDeviceLogOptionOutputTypeDef",
     "WirelessDeviceLogOptionTypeDef",
+    "WirelessGatewayLogOptionOutputTypeDef",
     "WirelessGatewayLogOptionTypeDef",
-    "CreateWirelessGatewayRequestRequestTypeDef",
     "GetWirelessGatewayResponseTypeDef",
     "WirelessGatewayStatisticsTypeDef",
+    "CreateWirelessGatewayRequestRequestTypeDef",
     "WirelessDeviceStatisticsTypeDef",
     "GetDeviceProfileResponseTypeDef",
+    "LoRaWANDeviceOutputTypeDef",
     "LoRaWANDeviceTypeDef",
     "LoRaWANUpdateDeviceTypeDef",
+    "LoRaWANSendDataToDeviceOutputTypeDef",
     "LoRaWANSendDataToDeviceTypeDef",
     "ListWirelessDeviceImportTasksResponseTypeDef",
     "GsmObjTypeDef",
     "ListDevicesForWirelessDeviceImportTaskResponseTypeDef",
     "EventNotificationItemConfigurationsTypeDef",
     "GetResourceEventConfigurationResponseTypeDef",
     "UpdateResourceEventConfigurationRequestRequestTypeDef",
     "GetEventConfigurationByResourceTypesResponseTypeDef",
     "UpdateEventConfigurationByResourceTypesRequestRequestTypeDef",
     "GetWirelessDeviceStatisticsResponseTypeDef",
     "GetWirelessGatewayFirmwareInformationResponseTypeDef",
-    "UpdateWirelessGatewayTaskCreateTypeDef",
+    "UpdateWirelessGatewayTaskCreateOutputTypeDef",
     "UpdateWirelessGatewayTaskEntryTypeDef",
+    "UpdateWirelessGatewayTaskCreateTypeDef",
     "SendDataToMulticastGroupRequestRequestTypeDef",
     "PutPositionConfigurationRequestRequestTypeDef",
     "GetPositionConfigurationResponseTypeDef",
     "PositionConfigurationItemTypeDef",
     "GetLogLevelsByResourceTypesResponseTypeDef",
     "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
     "ListWirelessGatewaysResponseTypeDef",
     "ListWirelessDevicesResponseTypeDef",
-    "CreateWirelessDeviceRequestRequestTypeDef",
     "GetWirelessDeviceResponseTypeDef",
+    "CreateWirelessDeviceRequestRequestTypeDef",
     "UpdateWirelessDeviceRequestRequestTypeDef",
     "DownlinkQueueMessageTypeDef",
     "WirelessMetadataTypeDef",
     "CellTowersTypeDef",
     "EventConfigurationItemTypeDef",
-    "CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "GetWirelessGatewayTaskDefinitionResponseTypeDef",
     "ListWirelessGatewayTaskDefinitionsResponseTypeDef",
+    "CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "ListPositionConfigurationsResponseTypeDef",
     "ListQueuedMessagesResponseTypeDef",
     "SendDataToWirelessDeviceRequestRequestTypeDef",
     "GetPositionEstimateRequestRequestTypeDef",
     "ListEventConfigurationsResponseTypeDef",
 )
 
+SessionKeysAbpV10XOutputTypeDef = TypedDict(
+    "SessionKeysAbpV10XOutputTypeDef",
+    {
+        "NwkSKey": str,
+        "AppSKey": str,
+    },
+    total=False,
+)
+
 SessionKeysAbpV10XTypeDef = TypedDict(
     "SessionKeysAbpV10XTypeDef",
     {
         "NwkSKey": str,
         "AppSKey": str,
     },
     total=False,
 )
 
+SessionKeysAbpV11OutputTypeDef = TypedDict(
+    "SessionKeysAbpV11OutputTypeDef",
+    {
+        "FNwkSIntKey": str,
+        "SNwkSIntKey": str,
+        "NwkSEncKey": str,
+        "AppSKey": str,
+    },
+    total=False,
+)
+
 SessionKeysAbpV11TypeDef = TypedDict(
     "SessionKeysAbpV11TypeDef",
     {
         "FNwkSIntKey": str,
         "SNwkSIntKey": str,
         "NwkSEncKey": str,
         "AppSKey": str,
@@ -375,14 +439,24 @@
     {
         "HorizontalAccuracy": float,
         "VerticalAccuracy": float,
     },
     total=False,
 )
 
+ApplicationConfigOutputTypeDef = TypedDict(
+    "ApplicationConfigOutputTypeDef",
+    {
+        "FPort": int,
+        "Type": Literal["SemtechGeolocation"],
+        "DestinationName": str,
+    },
+    total=False,
+)
+
 ApplicationConfigTypeDef = TypedDict(
     "ApplicationConfigTypeDef",
     {
         "FPort": int,
         "Type": Literal["SemtechGeolocation"],
         "DestinationName": str,
     },
@@ -402,14 +476,23 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+SidewalkAccountInfoOutputTypeDef = TypedDict(
+    "SidewalkAccountInfoOutputTypeDef",
+    {
+        "AmazonId": str,
+        "AppServerPrivateKey": str,
+    },
+    total=False,
+)
+
 AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef = TypedDict(
     "AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef",
     {
         "Id": str,
         "MulticastGroupId": str,
     },
 )
@@ -458,14 +541,23 @@
     "AssociateWirelessGatewayWithThingRequestRequestTypeDef",
     {
         "Id": str,
         "ThingArn": str,
     },
 )
 
+BeaconingOutputTypeDef = TypedDict(
+    "BeaconingOutputTypeDef",
+    {
+        "DataRate": int,
+        "Frequencies": List[int],
+    },
+    total=False,
+)
+
 BeaconingTypeDef = TypedDict(
     "BeaconingTypeDef",
     {
         "DataRate": int,
         "Frequencies": Sequence[int],
     },
     total=False,
@@ -498,33 +590,51 @@
     {
         "PilotPower": int,
         "BaseStationId": int,
     },
     total=False,
 )
 
+
 class CdmaNmrObjTypeDef(_RequiredCdmaNmrObjTypeDef, _OptionalCdmaNmrObjTypeDef):
     pass
 
+
 CertificateListTypeDef = TypedDict(
     "CertificateListTypeDef",
     {
         "SigningAlg": SigningAlgType,
         "Value": str,
     },
 )
 
+LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef = TypedDict(
+    "LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef",
+    {
+        "GatewayEuiEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
 LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef = TypedDict(
     "LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef",
     {
         "GatewayEuiEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
+LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef = TypedDict(
+    "LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef",
+    {
+        "WirelessGatewayEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
 LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef = TypedDict(
     "LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef",
     {
         "WirelessGatewayEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
@@ -713,19 +823,21 @@
         "FactorySupport": bool,
         "ApId": str,
         "DeviceTypeId": str,
     },
     total=False,
 )
 
+
 class DakCertificateMetadataTypeDef(
     _RequiredDakCertificateMetadataTypeDef, _OptionalDakCertificateMetadataTypeDef
 ):
     pass
 
+
 DeleteDestinationRequestRequestTypeDef = TypedDict(
     "DeleteDestinationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -768,20 +880,22 @@
     "_OptionalDeleteQueuedMessagesRequestRequestTypeDef",
     {
         "WirelessDeviceType": WirelessDeviceTypeType,
     },
     total=False,
 )
 
+
 class DeleteQueuedMessagesRequestRequestTypeDef(
     _RequiredDeleteQueuedMessagesRequestRequestTypeDef,
     _OptionalDeleteQueuedMessagesRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteServiceProfileRequestRequestTypeDef = TypedDict(
     "DeleteServiceProfileRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -830,20 +944,22 @@
     "_OptionalDeregisterWirelessDeviceRequestRequestTypeDef",
     {
         "WirelessDeviceType": WirelessDeviceTypeType,
     },
     total=False,
 )
 
+
 class DeregisterWirelessDeviceRequestRequestTypeDef(
     _RequiredDeregisterWirelessDeviceRequestRequestTypeDef,
     _OptionalDeregisterWirelessDeviceRequestRequestTypeDef,
 ):
     pass
 
+
 DestinationsTypeDef = TypedDict(
     "DestinationsTypeDef",
     {
         "Arn": str,
         "Name": str,
         "ExpressionType": ExpressionTypeType,
         "Expression": str,
@@ -859,22 +975,38 @@
         "Arn": str,
         "Name": str,
         "Id": str,
     },
     total=False,
 )
 
+SidewalkEventNotificationConfigurationsOutputTypeDef = TypedDict(
+    "SidewalkEventNotificationConfigurationsOutputTypeDef",
+    {
+        "AmazonIdEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
 SidewalkEventNotificationConfigurationsTypeDef = TypedDict(
     "SidewalkEventNotificationConfigurationsTypeDef",
     {
         "AmazonIdEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
+SidewalkResourceTypeEventConfigurationOutputTypeDef = TypedDict(
+    "SidewalkResourceTypeEventConfigurationOutputTypeDef",
+    {
+        "WirelessDeviceEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
 SidewalkResourceTypeEventConfigurationTypeDef = TypedDict(
     "SidewalkResourceTypeEventConfigurationTypeDef",
     {
         "WirelessDeviceEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
@@ -928,14 +1060,24 @@
 DisassociateWirelessGatewayFromThingRequestRequestTypeDef = TypedDict(
     "DisassociateWirelessGatewayFromThingRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+PositioningOutputTypeDef = TypedDict(
+    "PositioningOutputTypeDef",
+    {
+        "ClockSync": int,
+        "Stream": int,
+        "Gnss": int,
+    },
+    total=False,
+)
+
 PositioningTypeDef = TypedDict(
     "PositioningTypeDef",
     {
         "ClockSync": int,
         "Stream": int,
         "Gnss": int,
     },
@@ -948,14 +1090,22 @@
         "Id": str,
         "Arn": str,
         "Name": str,
     },
     total=False,
 )
 
+GatewayListItemOutputTypeDef = TypedDict(
+    "GatewayListItemOutputTypeDef",
+    {
+        "GatewayId": str,
+        "DownlinkFrequency": int,
+    },
+)
+
 GatewayListItemTypeDef = TypedDict(
     "GatewayListItemTypeDef",
     {
         "GatewayId": str,
         "DownlinkFrequency": int,
     },
 )
@@ -983,14 +1133,40 @@
 GetDeviceProfileRequestRequestTypeDef = TypedDict(
     "GetDeviceProfileRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+LoRaWANDeviceProfileOutputTypeDef = TypedDict(
+    "LoRaWANDeviceProfileOutputTypeDef",
+    {
+        "SupportsClassB": bool,
+        "ClassBTimeout": int,
+        "PingSlotPeriod": int,
+        "PingSlotDr": int,
+        "PingSlotFreq": int,
+        "SupportsClassC": bool,
+        "ClassCTimeout": int,
+        "MacVersion": str,
+        "RegParamsRevision": str,
+        "RxDelay1": int,
+        "RxDrOffset1": int,
+        "RxDataRate2": int,
+        "RxFreq2": int,
+        "FactoryPresetFreqsList": List[int],
+        "MaxEirp": int,
+        "MaxDutyCycle": int,
+        "RfRegion": str,
+        "SupportsJoin": bool,
+        "Supports32BitFCnt": bool,
+    },
+    total=False,
+)
+
 GetFuotaTaskRequestRequestTypeDef = TypedDict(
     "GetFuotaTaskRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1024,16 +1200,16 @@
 GetMulticastGroupSessionRequestRequestTypeDef = TypedDict(
     "GetMulticastGroupSessionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-LoRaWANMulticastSessionTypeDef = TypedDict(
-    "LoRaWANMulticastSessionTypeDef",
+LoRaWANMulticastSessionOutputTypeDef = TypedDict(
+    "LoRaWANMulticastSessionOutputTypeDef",
     {
         "DlDr": int,
         "DlFreq": int,
         "SessionStartTime": datetime,
         "SessionTimeout": int,
         "PingSlotPeriod": int,
     },
@@ -1043,14 +1219,24 @@
 GetNetworkAnalyzerConfigurationRequestRequestTypeDef = TypedDict(
     "GetNetworkAnalyzerConfigurationRequestRequestTypeDef",
     {
         "ConfigurationName": str,
     },
 )
 
+TraceContentOutputTypeDef = TypedDict(
+    "TraceContentOutputTypeDef",
+    {
+        "WirelessDeviceFrameInfo": WirelessDeviceFrameInfoType,
+        "LogLevel": LogLevelType,
+        "MulticastFrameInfo": MulticastFrameInfoType,
+    },
+    total=False,
+)
+
 GetPartnerAccountRequestRequestTypeDef = TypedDict(
     "GetPartnerAccountRequestRequestTypeDef",
     {
         "PartnerAccountId": str,
         "PartnerType": Literal["Sidewalk"],
     },
 )
@@ -1087,17 +1273,19 @@
         "AssistPosition": Sequence[float],
         "AssistAltitude": float,
         "Use2DSolver": bool,
     },
     total=False,
 )
 
+
 class GnssTypeDef(_RequiredGnssTypeDef, _OptionalGnssTypeDef):
     pass
 
+
 IpTypeDef = TypedDict(
     "IpTypeDef",
     {
         "IpAddress": str,
     },
 )
 
@@ -1136,20 +1324,22 @@
     "_OptionalGetResourceEventConfigurationRequestRequestTypeDef",
     {
         "PartnerType": Literal["Sidewalk"],
     },
     total=False,
 )
 
+
 class GetResourceEventConfigurationRequestRequestTypeDef(
     _RequiredGetResourceEventConfigurationRequestRequestTypeDef,
     _OptionalGetResourceEventConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 GetResourceLogLevelRequestRequestTypeDef = TypedDict(
     "GetResourceLogLevelRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": str,
     },
 )
@@ -1368,22 +1558,38 @@
         "OnboardingStatus": OnboardStatusType,
         "OnboardingStatusReason": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
+LoRaWANJoinEventNotificationConfigurationsOutputTypeDef = TypedDict(
+    "LoRaWANJoinEventNotificationConfigurationsOutputTypeDef",
+    {
+        "DevEuiEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
 LoRaWANJoinEventNotificationConfigurationsTypeDef = TypedDict(
     "LoRaWANJoinEventNotificationConfigurationsTypeDef",
     {
         "DevEuiEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
+LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef = TypedDict(
+    "LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef",
+    {
+        "WirelessDeviceEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
 LoRaWANJoinResourceTypeEventConfigurationTypeDef = TypedDict(
     "LoRaWANJoinResourceTypeEventConfigurationTypeDef",
     {
         "WirelessDeviceEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
@@ -1419,20 +1625,22 @@
         "MaxResults": int,
         "NextToken": str,
         "Status": OnboardStatusType,
     },
     total=False,
 )
 
+
 class ListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef(
     _RequiredListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef,
     _OptionalListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListEventConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListEventConfigurationsRequestRequestTypeDef",
     {
         "ResourceType": EventNotificationResourceTypeType,
     },
 )
 _OptionalListEventConfigurationsRequestRequestTypeDef = TypedDict(
@@ -1440,20 +1648,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListEventConfigurationsRequestRequestTypeDef(
     _RequiredListEventConfigurationsRequestRequestTypeDef,
     _OptionalListEventConfigurationsRequestRequestTypeDef,
 ):
     pass
 
+
 ListFuotaTasksRequestRequestTypeDef = TypedDict(
     "ListFuotaTasksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1470,20 +1680,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListMulticastGroupsByFuotaTaskRequestRequestTypeDef(
     _RequiredListMulticastGroupsByFuotaTaskRequestRequestTypeDef,
     _OptionalListMulticastGroupsByFuotaTaskRequestRequestTypeDef,
 ):
     pass
 
+
 MulticastGroupByFuotaTaskTypeDef = TypedDict(
     "MulticastGroupByFuotaTaskTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
@@ -1556,20 +1768,22 @@
         "NextToken": str,
         "MaxResults": int,
         "WirelessDeviceType": WirelessDeviceTypeType,
     },
     total=False,
 )
 
+
 class ListQueuedMessagesRequestRequestTypeDef(
     _RequiredListQueuedMessagesRequestRequestTypeDef,
     _OptionalListQueuedMessagesRequestRequestTypeDef,
 ):
     pass
 
+
 ListServiceProfilesRequestRequestTypeDef = TypedDict(
     "ListServiceProfilesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1588,14 +1802,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 ListWirelessDeviceImportTasksRequestRequestTypeDef = TypedDict(
     "ListWirelessDeviceImportTasksRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1641,14 +1863,34 @@
         "GatewayEui": str,
         "Snr": float,
         "Rssi": float,
     },
     total=False,
 )
 
+OtaaV10XOutputTypeDef = TypedDict(
+    "OtaaV10XOutputTypeDef",
+    {
+        "AppKey": str,
+        "AppEui": str,
+        "GenAppKey": str,
+    },
+    total=False,
+)
+
+OtaaV11OutputTypeDef = TypedDict(
+    "OtaaV11OutputTypeDef",
+    {
+        "AppKey": str,
+        "NwkKey": str,
+        "JoinEui": str,
+    },
+    total=False,
+)
+
 OtaaV10XTypeDef = TypedDict(
     "OtaaV10XTypeDef",
     {
         "AppKey": str,
         "AppEui": str,
         "GenAppKey": str,
     },
@@ -1661,14 +1903,24 @@
         "AppKey": str,
         "NwkKey": str,
         "JoinEui": str,
     },
     total=False,
 )
 
+LoRaWANGatewayVersionOutputTypeDef = TypedDict(
+    "LoRaWANGatewayVersionOutputTypeDef",
+    {
+        "PackageVersion": str,
+        "Model": str,
+        "Station": str,
+    },
+    total=False,
+)
+
 LoRaWANGatewayVersionTypeDef = TypedDict(
     "LoRaWANGatewayVersionTypeDef",
     {
         "PackageVersion": str,
         "Model": str,
         "Station": str,
     },
@@ -1687,14 +1939,26 @@
     "LoRaWANMulticastMetadataTypeDef",
     {
         "FPort": int,
     },
     total=False,
 )
 
+LoRaWANMulticastSessionTypeDef = TypedDict(
+    "LoRaWANMulticastSessionTypeDef",
+    {
+        "DlDr": int,
+        "DlFreq": int,
+        "SessionStartTime": Union[datetime, str],
+        "SessionTimeout": int,
+        "PingSlotPeriod": int,
+    },
+    total=False,
+)
+
 LoRaWANStartFuotaTaskTypeDef = TypedDict(
     "LoRaWANStartFuotaTaskTypeDef",
     {
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
@@ -1736,17 +2000,19 @@
     {
         "Rsrp": int,
         "Rsrq": float,
     },
     total=False,
 )
 
+
 class LteNmrObjTypeDef(_RequiredLteNmrObjTypeDef, _OptionalLteNmrObjTypeDef):
     pass
 
+
 SemtechGnssConfigurationTypeDef = TypedDict(
     "SemtechGnssConfigurationTypeDef",
     {
         "Status": PositionConfigurationStatusType,
         "Fec": PositionConfigurationFecType,
     },
 )
@@ -1888,17 +2154,19 @@
         "UtranCid": int,
         "Rscp": int,
         "PathLoss": int,
     },
     total=False,
 )
 
+
 class TdscdmaNmrObjTypeDef(_RequiredTdscdmaNmrObjTypeDef, _OptionalTdscdmaNmrObjTypeDef):
     pass
 
+
 TestWirelessDeviceRequestRequestTypeDef = TypedDict(
     "TestWirelessDeviceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1931,19 +2199,21 @@
         "Expression": str,
         "Description": str,
         "RoleArn": str,
     },
     total=False,
 )
 
+
 class UpdateDestinationRequestRequestTypeDef(
     _RequiredUpdateDestinationRequestRequestTypeDef, _OptionalUpdateDestinationRequestRequestTypeDef
 ):
     pass
 
+
 UpdatePositionRequestRequestTypeDef = TypedDict(
     "UpdatePositionRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": PositionResourceTypeType,
         "Position": Sequence[float],
     },
@@ -1960,20 +2230,22 @@
     "_OptionalUpdateResourcePositionRequestRequestTypeDef",
     {
         "GeoJsonPayload": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
+
 class UpdateResourcePositionRequestRequestTypeDef(
     _RequiredUpdateResourcePositionRequestRequestTypeDef,
     _OptionalUpdateResourcePositionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateWirelessGatewayRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWirelessGatewayRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateWirelessGatewayRequestRequestTypeDef = TypedDict(
@@ -1984,20 +2256,22 @@
         "JoinEuiFilters": Sequence[Sequence[str]],
         "NetIdFilters": Sequence[str],
         "MaxEirp": float,
     },
     total=False,
 )
 
+
 class UpdateWirelessGatewayRequestRequestTypeDef(
     _RequiredUpdateWirelessGatewayRequestRequestTypeDef,
     _OptionalUpdateWirelessGatewayRequestRequestTypeDef,
 ):
     pass
 
+
 WcdmaLocalIdTypeDef = TypedDict(
     "WcdmaLocalIdTypeDef",
     {
         "Uarfcndl": int,
         "Psc": int,
     },
 )
@@ -2015,43 +2289,81 @@
     {
         "Rscp": int,
         "PathLoss": int,
     },
     total=False,
 )
 
+
 class WcdmaNmrObjTypeDef(_RequiredWcdmaNmrObjTypeDef, _OptionalWcdmaNmrObjTypeDef):
     pass
 
+
+WirelessDeviceEventLogOptionOutputTypeDef = TypedDict(
+    "WirelessDeviceEventLogOptionOutputTypeDef",
+    {
+        "Event": WirelessDeviceEventType,
+        "LogLevel": LogLevelType,
+    },
+)
+
 WirelessDeviceEventLogOptionTypeDef = TypedDict(
     "WirelessDeviceEventLogOptionTypeDef",
     {
         "Event": WirelessDeviceEventType,
         "LogLevel": LogLevelType,
     },
 )
 
+WirelessGatewayEventLogOptionOutputTypeDef = TypedDict(
+    "WirelessGatewayEventLogOptionOutputTypeDef",
+    {
+        "Event": WirelessGatewayEventType,
+        "LogLevel": LogLevelType,
+    },
+)
+
 WirelessGatewayEventLogOptionTypeDef = TypedDict(
     "WirelessGatewayEventLogOptionTypeDef",
     {
         "Event": WirelessGatewayEventType,
         "LogLevel": LogLevelType,
     },
 )
 
+AbpV10XOutputTypeDef = TypedDict(
+    "AbpV10XOutputTypeDef",
+    {
+        "DevAddr": str,
+        "SessionKeys": SessionKeysAbpV10XOutputTypeDef,
+        "FCntStart": int,
+    },
+    total=False,
+)
+
 AbpV10XTypeDef = TypedDict(
     "AbpV10XTypeDef",
     {
         "DevAddr": str,
         "SessionKeys": SessionKeysAbpV10XTypeDef,
         "FCntStart": int,
     },
     total=False,
 )
 
+AbpV11OutputTypeDef = TypedDict(
+    "AbpV11OutputTypeDef",
+    {
+        "DevAddr": str,
+        "SessionKeys": SessionKeysAbpV11OutputTypeDef,
+        "FCntStart": int,
+    },
+    total=False,
+)
+
 AbpV11TypeDef = TypedDict(
     "AbpV11TypeDef",
     {
         "DevAddr": str,
         "SessionKeys": SessionKeysAbpV11TypeDef,
         "FCntStart": int,
     },
@@ -2067,23 +2379,14 @@
         "SolverProvider": Literal["Semtech"],
         "SolverVersion": str,
         "Timestamp": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AssociateAwsAccountWithPartnerAccountResponseTypeDef = TypedDict(
-    "AssociateAwsAccountWithPartnerAccountResponseTypeDef",
-    {
-        "Sidewalk": SidewalkAccountInfoTypeDef,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef",
     {
         "Sidewalk": SidewalkAccountInfoTypeDef,
     },
 )
 _OptionalAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef = TypedDict(
@@ -2091,20 +2394,22 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef(
     _RequiredAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef,
     _OptionalAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDestinationRequestRequestTypeDef",
     {
         "Name": str,
         "ExpressionType": ExpressionTypeType,
         "Expression": str,
         "RoleArn": str,
@@ -2116,26 +2421,20 @@
         "Description": str,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class CreateDestinationRequestRequestTypeDef(
     _RequiredCreateDestinationRequestRequestTypeDef, _OptionalCreateDestinationRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef = TypedDict(
     "_RequiredStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
@@ -2144,20 +2443,22 @@
     {
         "QueryString": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef(
     _RequiredStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     _OptionalStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef = TypedDict(
     "_RequiredStartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalStartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef = TypedDict(
@@ -2165,28 +2466,53 @@
     {
         "QueryString": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef(
     _RequiredStartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
     _OptionalStartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+AssociateAwsAccountWithPartnerAccountResponseTypeDef = TypedDict(
+    "AssociateAwsAccountWithPartnerAccountResponseTypeDef",
+    {
+        "Sidewalk": SidewalkAccountInfoOutputTypeDef,
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+LoRaWANGatewayOutputTypeDef = TypedDict(
+    "LoRaWANGatewayOutputTypeDef",
+    {
+        "GatewayEui": str,
+        "RfRegion": str,
+        "JoinEuiFilters": List[List[str]],
+        "NetIdFilters": List[str],
+        "SubBands": List[int],
+        "Beaconing": BeaconingOutputTypeDef,
+        "MaxEirp": float,
+    },
+    total=False,
+)
+
 LoRaWANGatewayTypeDef = TypedDict(
     "LoRaWANGatewayTypeDef",
     {
         "GatewayEui": str,
         "RfRegion": str,
         "JoinEuiFilters": Sequence[Sequence[str]],
         "NetIdFilters": Sequence[str],
@@ -2214,17 +2540,19 @@
         "BaseLat": float,
         "BaseLng": float,
         "CdmaNmr": Sequence[CdmaNmrObjTypeDef],
     },
     total=False,
 )
 
+
 class CdmaObjTypeDef(_RequiredCdmaObjTypeDef, _OptionalCdmaObjTypeDef):
     pass
 
+
 SidewalkDeviceTypeDef = TypedDict(
     "SidewalkDeviceTypeDef",
     {
         "AmazonId": str,
         "SidewalkId": str,
         "SidewalkManufacturingSn": str,
         "DeviceCertificates": List[CertificateListTypeDef],
@@ -2245,23 +2573,40 @@
         "DeviceCertificates": List[CertificateListTypeDef],
         "DeviceProfileId": str,
         "Status": WirelessDeviceSidewalkStatusType,
     },
     total=False,
 )
 
+ConnectionStatusEventConfigurationOutputTypeDef = TypedDict(
+    "ConnectionStatusEventConfigurationOutputTypeDef",
+    {
+        "LoRaWAN": LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef,
+        "WirelessGatewayIdEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
 ConnectionStatusEventConfigurationTypeDef = TypedDict(
     "ConnectionStatusEventConfigurationTypeDef",
     {
         "LoRaWAN": LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef,
         "WirelessGatewayIdEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
+ConnectionStatusResourceTypeEventConfigurationOutputTypeDef = TypedDict(
+    "ConnectionStatusResourceTypeEventConfigurationOutputTypeDef",
+    {
+        "LoRaWAN": LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ConnectionStatusResourceTypeEventConfigurationTypeDef = TypedDict(
     "ConnectionStatusResourceTypeEventConfigurationTypeDef",
     {
         "LoRaWAN": LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef,
     },
     total=False,
 )
@@ -2296,19 +2641,21 @@
         "RedundancyPercent": int,
         "FragmentSizeBytes": int,
         "FragmentIntervalMS": int,
     },
     total=False,
 )
 
+
 class CreateFuotaTaskRequestRequestTypeDef(
     _RequiredCreateFuotaTaskRequestRequestTypeDef, _OptionalCreateFuotaTaskRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateFuotaTaskRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFuotaTaskRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateFuotaTaskRequestRequestTypeDef = TypedDict(
@@ -2322,19 +2669,21 @@
         "RedundancyPercent": int,
         "FragmentSizeBytes": int,
         "FragmentIntervalMS": int,
     },
     total=False,
 )
 
+
 class UpdateFuotaTaskRequestRequestTypeDef(
     _RequiredUpdateFuotaTaskRequestRequestTypeDef, _OptionalUpdateFuotaTaskRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateMulticastGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMulticastGroupRequestRequestTypeDef",
     {
         "LoRaWAN": LoRaWANMulticastTypeDef,
     },
 )
 _OptionalCreateMulticastGroupRequestRequestTypeDef = TypedDict(
@@ -2344,20 +2693,22 @@
         "Description": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMulticastGroupRequestRequestTypeDef(
     _RequiredCreateMulticastGroupRequestRequestTypeDef,
     _OptionalCreateMulticastGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateMulticastGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMulticastGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateMulticastGroupRequestRequestTypeDef = TypedDict(
@@ -2366,20 +2717,22 @@
         "Name": str,
         "Description": str,
         "LoRaWAN": LoRaWANMulticastTypeDef,
     },
     total=False,
 )
 
+
 class UpdateMulticastGroupRequestRequestTypeDef(
     _RequiredUpdateMulticastGroupRequestRequestTypeDef,
     _OptionalUpdateMulticastGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateNetworkAnalyzerConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNetworkAnalyzerConfigurationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateNetworkAnalyzerConfigurationRequestRequestTypeDef = TypedDict(
@@ -2392,33 +2745,21 @@
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
         "MulticastGroups": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateNetworkAnalyzerConfigurationRequestRequestTypeDef(
     _RequiredCreateNetworkAnalyzerConfigurationRequestRequestTypeDef,
     _OptionalCreateNetworkAnalyzerConfigurationRequestRequestTypeDef,
 ):
     pass
 
-GetNetworkAnalyzerConfigurationResponseTypeDef = TypedDict(
-    "GetNetworkAnalyzerConfigurationResponseTypeDef",
-    {
-        "TraceContent": TraceContentTypeDef,
-        "WirelessDevices": List[str],
-        "WirelessGateways": List[str],
-        "Description": str,
-        "Arn": str,
-        "Name": str,
-        "MulticastGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef",
     {
         "ConfigurationName": str,
     },
 )
@@ -2433,20 +2774,22 @@
         "Description": str,
         "MulticastGroupsToAdd": Sequence[str],
         "MulticastGroupsToRemove": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateNetworkAnalyzerConfigurationRequestRequestTypeDef(
     _RequiredUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef,
     _OptionalUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 CreateServiceProfileRequestRequestTypeDef = TypedDict(
     "CreateServiceProfileRequestRequestTypeDef",
     {
         "Name": str,
         "LoRaWAN": LoRaWANServiceProfileTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
@@ -2478,14 +2821,41 @@
     {
         "NextToken": str,
         "DeviceProfileList": List[DeviceProfileTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DeviceRegistrationStateEventConfigurationOutputTypeDef = TypedDict(
+    "DeviceRegistrationStateEventConfigurationOutputTypeDef",
+    {
+        "Sidewalk": SidewalkEventNotificationConfigurationsOutputTypeDef,
+        "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
+MessageDeliveryStatusEventConfigurationOutputTypeDef = TypedDict(
+    "MessageDeliveryStatusEventConfigurationOutputTypeDef",
+    {
+        "Sidewalk": SidewalkEventNotificationConfigurationsOutputTypeDef,
+        "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
+ProximityEventConfigurationOutputTypeDef = TypedDict(
+    "ProximityEventConfigurationOutputTypeDef",
+    {
+        "Sidewalk": SidewalkEventNotificationConfigurationsOutputTypeDef,
+        "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
 DeviceRegistrationStateEventConfigurationTypeDef = TypedDict(
     "DeviceRegistrationStateEventConfigurationTypeDef",
     {
         "Sidewalk": SidewalkEventNotificationConfigurationsTypeDef,
         "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
@@ -2505,14 +2875,38 @@
     {
         "Sidewalk": SidewalkEventNotificationConfigurationsTypeDef,
         "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
+DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef = TypedDict(
+    "DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef",
+    {
+        "Sidewalk": SidewalkResourceTypeEventConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef = TypedDict(
+    "MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef",
+    {
+        "Sidewalk": SidewalkResourceTypeEventConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+ProximityResourceTypeEventConfigurationOutputTypeDef = TypedDict(
+    "ProximityResourceTypeEventConfigurationOutputTypeDef",
+    {
+        "Sidewalk": SidewalkResourceTypeEventConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 DeviceRegistrationStateResourceTypeEventConfigurationTypeDef = TypedDict(
     "DeviceRegistrationStateResourceTypeEventConfigurationTypeDef",
     {
         "Sidewalk": SidewalkResourceTypeEventConfigurationTypeDef,
     },
     total=False,
 )
@@ -2529,14 +2923,26 @@
     "ProximityResourceTypeEventConfigurationTypeDef",
     {
         "Sidewalk": SidewalkResourceTypeEventConfigurationTypeDef,
     },
     total=False,
 )
 
+FPortsOutputTypeDef = TypedDict(
+    "FPortsOutputTypeDef",
+    {
+        "Fuota": int,
+        "Multicast": int,
+        "ClockSync": int,
+        "Positioning": PositioningOutputTypeDef,
+        "Applications": List[ApplicationConfigOutputTypeDef],
+    },
+    total=False,
+)
+
 FPortsTypeDef = TypedDict(
     "FPortsTypeDef",
     {
         "Fuota": int,
         "Multicast": int,
         "ClockSync": int,
         "Positioning": PositioningTypeDef,
@@ -2559,19 +2965,28 @@
     {
         "NextToken": str,
         "FuotaTaskList": List[FuotaTaskTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ParticipatingGatewaysOutputTypeDef = TypedDict(
+    "ParticipatingGatewaysOutputTypeDef",
+    {
+        "DownlinkMode": DownlinkModeType,
+        "GatewayList": List[GatewayListItemOutputTypeDef],
+        "TransmissionInterval": int,
+    },
+)
+
 ParticipatingGatewaysTypeDef = TypedDict(
     "ParticipatingGatewaysTypeDef",
     {
         "DownlinkMode": DownlinkModeType,
-        "GatewayList": List[GatewayListItemTypeDef],
+        "GatewayList": Sequence[GatewayListItemTypeDef],
         "TransmissionInterval": int,
     },
 )
 
 GetFuotaTaskResponseTypeDef = TypedDict(
     "GetFuotaTaskResponseTypeDef",
     {
@@ -2604,24 +3019,30 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMulticastGroupSessionResponseTypeDef = TypedDict(
     "GetMulticastGroupSessionResponseTypeDef",
     {
-        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
+        "LoRaWAN": LoRaWANMulticastSessionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartMulticastGroupSessionRequestRequestTypeDef = TypedDict(
-    "StartMulticastGroupSessionRequestRequestTypeDef",
+GetNetworkAnalyzerConfigurationResponseTypeDef = TypedDict(
+    "GetNetworkAnalyzerConfigurationResponseTypeDef",
     {
-        "Id": str,
-        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
+        "TraceContent": TraceContentOutputTypeDef,
+        "WirelessDevices": List[str],
+        "WirelessGateways": List[str],
+        "Description": str,
+        "Arn": str,
+        "Name": str,
+        "MulticastGroups": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPartnerAccountResponseTypeDef = TypedDict(
     "GetPartnerAccountResponseTypeDef",
     {
         "Sidewalk": SidewalkAccountInfoWithFingerprintTypeDef,
@@ -2698,34 +3119,53 @@
     {
         "RxLevel": int,
         "GlobalIdentity": GlobalIdentityTypeDef,
     },
     total=False,
 )
 
+
 class GsmNmrObjTypeDef(_RequiredGsmNmrObjTypeDef, _OptionalGsmNmrObjTypeDef):
     pass
 
+
 ImportedWirelessDeviceTypeDef = TypedDict(
     "ImportedWirelessDeviceTypeDef",
     {
         "Sidewalk": ImportedSidewalkDeviceTypeDef,
     },
     total=False,
 )
 
+JoinEventConfigurationOutputTypeDef = TypedDict(
+    "JoinEventConfigurationOutputTypeDef",
+    {
+        "LoRaWAN": LoRaWANJoinEventNotificationConfigurationsOutputTypeDef,
+        "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
+    },
+    total=False,
+)
+
 JoinEventConfigurationTypeDef = TypedDict(
     "JoinEventConfigurationTypeDef",
     {
         "LoRaWAN": LoRaWANJoinEventNotificationConfigurationsTypeDef,
         "WirelessDeviceIdEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
+JoinResourceTypeEventConfigurationOutputTypeDef = TypedDict(
+    "JoinResourceTypeEventConfigurationOutputTypeDef",
+    {
+        "LoRaWAN": LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 JoinResourceTypeEventConfigurationTypeDef = TypedDict(
     "JoinResourceTypeEventConfigurationTypeDef",
     {
         "LoRaWAN": LoRaWANJoinResourceTypeEventConfigurationTypeDef,
     },
     total=False,
 )
@@ -2762,14 +3202,22 @@
     {
         "NextToken": str,
         "ServiceProfileList": List[ServiceProfileTypeDef],
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
 LoRaWANDeviceMetadataTypeDef = TypedDict(
     "LoRaWANDeviceMetadataTypeDef",
     {
         "DevEui": str,
         "FPort": int,
         "DataRate": int,
         "Frequency": int,
@@ -2778,66 +3226,87 @@
     },
     total=False,
 )
 
 LoRaWANGatewayCurrentVersionTypeDef = TypedDict(
     "LoRaWANGatewayCurrentVersionTypeDef",
     {
-        "CurrentVersion": LoRaWANGatewayVersionTypeDef,
+        "CurrentVersion": LoRaWANGatewayVersionOutputTypeDef,
     },
     total=False,
 )
 
-LoRaWANUpdateGatewayTaskCreateTypeDef = TypedDict(
-    "LoRaWANUpdateGatewayTaskCreateTypeDef",
+LoRaWANUpdateGatewayTaskCreateOutputTypeDef = TypedDict(
+    "LoRaWANUpdateGatewayTaskCreateOutputTypeDef",
     {
         "UpdateSignature": str,
         "SigKeyCrc": int,
-        "CurrentVersion": LoRaWANGatewayVersionTypeDef,
-        "UpdateVersion": LoRaWANGatewayVersionTypeDef,
+        "CurrentVersion": LoRaWANGatewayVersionOutputTypeDef,
+        "UpdateVersion": LoRaWANGatewayVersionOutputTypeDef,
     },
     total=False,
 )
 
 LoRaWANUpdateGatewayTaskEntryTypeDef = TypedDict(
     "LoRaWANUpdateGatewayTaskEntryTypeDef",
     {
+        "CurrentVersion": LoRaWANGatewayVersionOutputTypeDef,
+        "UpdateVersion": LoRaWANGatewayVersionOutputTypeDef,
+    },
+    total=False,
+)
+
+LoRaWANUpdateGatewayTaskCreateTypeDef = TypedDict(
+    "LoRaWANUpdateGatewayTaskCreateTypeDef",
+    {
+        "UpdateSignature": str,
+        "SigKeyCrc": int,
         "CurrentVersion": LoRaWANGatewayVersionTypeDef,
         "UpdateVersion": LoRaWANGatewayVersionTypeDef,
     },
     total=False,
 )
 
 MulticastWirelessMetadataTypeDef = TypedDict(
     "MulticastWirelessMetadataTypeDef",
     {
         "LoRaWAN": LoRaWANMulticastMetadataTypeDef,
     },
     total=False,
 )
 
+StartMulticastGroupSessionRequestRequestTypeDef = TypedDict(
+    "StartMulticastGroupSessionRequestRequestTypeDef",
+    {
+        "Id": str,
+        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
+    },
+)
+
 _RequiredStartFuotaTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartFuotaTaskRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalStartFuotaTaskRequestRequestTypeDef = TypedDict(
     "_OptionalStartFuotaTaskRequestRequestTypeDef",
     {
         "LoRaWAN": LoRaWANStartFuotaTaskTypeDef,
     },
     total=False,
 )
 
+
 class StartFuotaTaskRequestRequestTypeDef(
     _RequiredStartFuotaTaskRequestRequestTypeDef, _OptionalStartFuotaTaskRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredLteObjTypeDef = TypedDict(
     "_RequiredLteObjTypeDef",
     {
         "Mcc": int,
         "Mnc": int,
         "EutranCid": int,
     },
@@ -2852,17 +3321,19 @@
         "Rsrq": float,
         "NrCapable": bool,
         "LteNmr": Sequence[LteNmrObjTypeDef],
     },
     total=False,
 )
 
+
 class LteObjTypeDef(_RequiredLteObjTypeDef, _OptionalLteObjTypeDef):
     pass
 
+
 PositionSolverConfigurationsTypeDef = TypedDict(
     "PositionSolverConfigurationsTypeDef",
     {
         "SemtechGnss": SemtechGnssConfigurationTypeDef,
     },
     total=False,
 )
@@ -2888,20 +3359,22 @@
         "ClientRequestToken": str,
         "DeviceName": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartSingleWirelessDeviceImportTaskRequestRequestTypeDef(
     _RequiredStartSingleWirelessDeviceImportTaskRequestRequestTypeDef,
     _OptionalStartSingleWirelessDeviceImportTaskRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartWirelessDeviceImportTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartWirelessDeviceImportTaskRequestRequestTypeDef",
     {
         "DestinationName": str,
         "Sidewalk": SidewalkStartImportInfoTypeDef,
     },
 )
@@ -2910,20 +3383,22 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartWirelessDeviceImportTaskRequestRequestTypeDef(
     _RequiredStartWirelessDeviceImportTaskRequestRequestTypeDef,
     _OptionalStartWirelessDeviceImportTaskRequestRequestTypeDef,
 ):
     pass
 
+
 UpdatePartnerAccountRequestRequestTypeDef = TypedDict(
     "UpdatePartnerAccountRequestRequestTypeDef",
     {
         "Sidewalk": SidewalkUpdateAccountTypeDef,
         "PartnerAccountId": str,
         "PartnerType": Literal["Sidewalk"],
     },
@@ -2954,17 +3429,19 @@
         "Rscp": int,
         "PathLoss": int,
         "TdscdmaNmr": Sequence[TdscdmaNmrObjTypeDef],
     },
     total=False,
 )
 
+
 class TdscdmaObjTypeDef(_RequiredTdscdmaObjTypeDef, _OptionalTdscdmaObjTypeDef):
     pass
 
+
 _RequiredWcdmaObjTypeDef = TypedDict(
     "_RequiredWcdmaObjTypeDef",
     {
         "Mcc": int,
         "Mnc": int,
         "UtranCid": int,
     },
@@ -2977,107 +3454,159 @@
         "Rscp": int,
         "PathLoss": int,
         "WcdmaNmr": Sequence[WcdmaNmrObjTypeDef],
     },
     total=False,
 )
 
+
 class WcdmaObjTypeDef(_RequiredWcdmaObjTypeDef, _OptionalWcdmaObjTypeDef):
     pass
 
+
+_RequiredWirelessDeviceLogOptionOutputTypeDef = TypedDict(
+    "_RequiredWirelessDeviceLogOptionOutputTypeDef",
+    {
+        "Type": WirelessDeviceTypeType,
+        "LogLevel": LogLevelType,
+    },
+)
+_OptionalWirelessDeviceLogOptionOutputTypeDef = TypedDict(
+    "_OptionalWirelessDeviceLogOptionOutputTypeDef",
+    {
+        "Events": List[WirelessDeviceEventLogOptionOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class WirelessDeviceLogOptionOutputTypeDef(
+    _RequiredWirelessDeviceLogOptionOutputTypeDef, _OptionalWirelessDeviceLogOptionOutputTypeDef
+):
+    pass
+
+
 _RequiredWirelessDeviceLogOptionTypeDef = TypedDict(
     "_RequiredWirelessDeviceLogOptionTypeDef",
     {
         "Type": WirelessDeviceTypeType,
         "LogLevel": LogLevelType,
     },
 )
 _OptionalWirelessDeviceLogOptionTypeDef = TypedDict(
     "_OptionalWirelessDeviceLogOptionTypeDef",
     {
-        "Events": List[WirelessDeviceEventLogOptionTypeDef],
+        "Events": Sequence[WirelessDeviceEventLogOptionTypeDef],
     },
     total=False,
 )
 
+
 class WirelessDeviceLogOptionTypeDef(
     _RequiredWirelessDeviceLogOptionTypeDef, _OptionalWirelessDeviceLogOptionTypeDef
 ):
     pass
 
-_RequiredWirelessGatewayLogOptionTypeDef = TypedDict(
-    "_RequiredWirelessGatewayLogOptionTypeDef",
+
+_RequiredWirelessGatewayLogOptionOutputTypeDef = TypedDict(
+    "_RequiredWirelessGatewayLogOptionOutputTypeDef",
     {
         "Type": Literal["LoRaWAN"],
         "LogLevel": LogLevelType,
     },
 )
-_OptionalWirelessGatewayLogOptionTypeDef = TypedDict(
-    "_OptionalWirelessGatewayLogOptionTypeDef",
+_OptionalWirelessGatewayLogOptionOutputTypeDef = TypedDict(
+    "_OptionalWirelessGatewayLogOptionOutputTypeDef",
     {
-        "Events": List[WirelessGatewayEventLogOptionTypeDef],
+        "Events": List[WirelessGatewayEventLogOptionOutputTypeDef],
     },
     total=False,
 )
 
-class WirelessGatewayLogOptionTypeDef(
-    _RequiredWirelessGatewayLogOptionTypeDef, _OptionalWirelessGatewayLogOptionTypeDef
+
+class WirelessGatewayLogOptionOutputTypeDef(
+    _RequiredWirelessGatewayLogOptionOutputTypeDef, _OptionalWirelessGatewayLogOptionOutputTypeDef
 ):
     pass
 
-_RequiredCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWirelessGatewayRequestRequestTypeDef",
+
+_RequiredWirelessGatewayLogOptionTypeDef = TypedDict(
+    "_RequiredWirelessGatewayLogOptionTypeDef",
     {
-        "LoRaWAN": LoRaWANGatewayTypeDef,
+        "Type": Literal["LoRaWAN"],
+        "LogLevel": LogLevelType,
     },
 )
-_OptionalCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWirelessGatewayRequestRequestTypeDef",
+_OptionalWirelessGatewayLogOptionTypeDef = TypedDict(
+    "_OptionalWirelessGatewayLogOptionTypeDef",
     {
-        "Name": str,
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
-        "ClientRequestToken": str,
+        "Events": Sequence[WirelessGatewayEventLogOptionTypeDef],
     },
     total=False,
 )
 
-class CreateWirelessGatewayRequestRequestTypeDef(
-    _RequiredCreateWirelessGatewayRequestRequestTypeDef,
-    _OptionalCreateWirelessGatewayRequestRequestTypeDef,
+
+class WirelessGatewayLogOptionTypeDef(
+    _RequiredWirelessGatewayLogOptionTypeDef, _OptionalWirelessGatewayLogOptionTypeDef
 ):
     pass
 
+
 GetWirelessGatewayResponseTypeDef = TypedDict(
     "GetWirelessGatewayResponseTypeDef",
     {
         "Name": str,
         "Id": str,
         "Description": str,
-        "LoRaWAN": LoRaWANGatewayTypeDef,
+        "LoRaWAN": LoRaWANGatewayOutputTypeDef,
         "Arn": str,
         "ThingName": str,
         "ThingArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WirelessGatewayStatisticsTypeDef = TypedDict(
     "WirelessGatewayStatisticsTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
-        "LoRaWAN": LoRaWANGatewayTypeDef,
+        "LoRaWAN": LoRaWANGatewayOutputTypeDef,
         "LastUplinkReceivedAt": str,
     },
     total=False,
 )
 
+_RequiredCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWirelessGatewayRequestRequestTypeDef",
+    {
+        "LoRaWAN": LoRaWANGatewayTypeDef,
+    },
+)
+_OptionalCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWirelessGatewayRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class CreateWirelessGatewayRequestRequestTypeDef(
+    _RequiredCreateWirelessGatewayRequestRequestTypeDef,
+    _OptionalCreateWirelessGatewayRequestRequestTypeDef,
+):
+    pass
+
+
 WirelessDeviceStatisticsTypeDef = TypedDict(
     "WirelessDeviceStatisticsTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Type": WirelessDeviceTypeType,
         "Name": str,
@@ -3094,20 +3623,35 @@
 
 GetDeviceProfileResponseTypeDef = TypedDict(
     "GetDeviceProfileResponseTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Id": str,
-        "LoRaWAN": LoRaWANDeviceProfileTypeDef,
+        "LoRaWAN": LoRaWANDeviceProfileOutputTypeDef,
         "Sidewalk": SidewalkGetDeviceProfileTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LoRaWANDeviceOutputTypeDef = TypedDict(
+    "LoRaWANDeviceOutputTypeDef",
+    {
+        "DevEui": str,
+        "DeviceProfileId": str,
+        "ServiceProfileId": str,
+        "OtaaV1_1": OtaaV11OutputTypeDef,
+        "OtaaV1_0_x": OtaaV10XOutputTypeDef,
+        "AbpV1_1": AbpV11OutputTypeDef,
+        "AbpV1_0_x": AbpV10XOutputTypeDef,
+        "FPorts": FPortsOutputTypeDef,
+    },
+    total=False,
+)
+
 LoRaWANDeviceTypeDef = TypedDict(
     "LoRaWANDeviceTypeDef",
     {
         "DevEui": str,
         "DeviceProfileId": str,
         "ServiceProfileId": str,
         "OtaaV1_1": OtaaV11TypeDef,
@@ -3127,14 +3671,23 @@
         "AbpV1_1": UpdateAbpV11TypeDef,
         "AbpV1_0_x": UpdateAbpV10XTypeDef,
         "FPorts": UpdateFPortsTypeDef,
     },
     total=False,
 )
 
+LoRaWANSendDataToDeviceOutputTypeDef = TypedDict(
+    "LoRaWANSendDataToDeviceOutputTypeDef",
+    {
+        "FPort": int,
+        "ParticipatingGateways": ParticipatingGatewaysOutputTypeDef,
+    },
+    total=False,
+)
+
 LoRaWANSendDataToDeviceTypeDef = TypedDict(
     "LoRaWANSendDataToDeviceTypeDef",
     {
         "FPort": int,
         "ParticipatingGateways": ParticipatingGatewaysTypeDef,
     },
     total=False,
@@ -3165,47 +3718,49 @@
         "GsmTimingAdvance": int,
         "RxLevel": int,
         "GsmNmr": Sequence[GsmNmrObjTypeDef],
     },
     total=False,
 )
 
+
 class GsmObjTypeDef(_RequiredGsmObjTypeDef, _OptionalGsmObjTypeDef):
     pass
 
+
 ListDevicesForWirelessDeviceImportTaskResponseTypeDef = TypedDict(
     "ListDevicesForWirelessDeviceImportTaskResponseTypeDef",
     {
         "NextToken": str,
         "DestinationName": str,
         "ImportedWirelessDeviceList": List[ImportedWirelessDeviceTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventNotificationItemConfigurationsTypeDef = TypedDict(
     "EventNotificationItemConfigurationsTypeDef",
     {
-        "DeviceRegistrationState": DeviceRegistrationStateEventConfigurationTypeDef,
-        "Proximity": ProximityEventConfigurationTypeDef,
-        "Join": JoinEventConfigurationTypeDef,
-        "ConnectionStatus": ConnectionStatusEventConfigurationTypeDef,
-        "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationTypeDef,
+        "DeviceRegistrationState": DeviceRegistrationStateEventConfigurationOutputTypeDef,
+        "Proximity": ProximityEventConfigurationOutputTypeDef,
+        "Join": JoinEventConfigurationOutputTypeDef,
+        "ConnectionStatus": ConnectionStatusEventConfigurationOutputTypeDef,
+        "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 GetResourceEventConfigurationResponseTypeDef = TypedDict(
     "GetResourceEventConfigurationResponseTypeDef",
     {
-        "DeviceRegistrationState": DeviceRegistrationStateEventConfigurationTypeDef,
-        "Proximity": ProximityEventConfigurationTypeDef,
-        "Join": JoinEventConfigurationTypeDef,
-        "ConnectionStatus": ConnectionStatusEventConfigurationTypeDef,
-        "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationTypeDef,
+        "DeviceRegistrationState": DeviceRegistrationStateEventConfigurationOutputTypeDef,
+        "Proximity": ProximityEventConfigurationOutputTypeDef,
+        "Join": JoinEventConfigurationOutputTypeDef,
+        "ConnectionStatus": ConnectionStatusEventConfigurationOutputTypeDef,
+        "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateResourceEventConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceEventConfigurationRequestRequestTypeDef",
     {
@@ -3222,28 +3777,32 @@
         "Join": JoinEventConfigurationTypeDef,
         "ConnectionStatus": ConnectionStatusEventConfigurationTypeDef,
         "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateResourceEventConfigurationRequestRequestTypeDef(
     _RequiredUpdateResourceEventConfigurationRequestRequestTypeDef,
     _OptionalUpdateResourceEventConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 GetEventConfigurationByResourceTypesResponseTypeDef = TypedDict(
     "GetEventConfigurationByResourceTypesResponseTypeDef",
     {
-        "DeviceRegistrationState": DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,
-        "Proximity": ProximityResourceTypeEventConfigurationTypeDef,
-        "Join": JoinResourceTypeEventConfigurationTypeDef,
-        "ConnectionStatus": ConnectionStatusResourceTypeEventConfigurationTypeDef,
-        "MessageDeliveryStatus": MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
+        "DeviceRegistrationState": (
+            DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef
+        ),
+        "Proximity": ProximityResourceTypeEventConfigurationOutputTypeDef,
+        "Join": JoinResourceTypeEventConfigurationOutputTypeDef,
+        "ConnectionStatus": ConnectionStatusResourceTypeEventConfigurationOutputTypeDef,
+        "MessageDeliveryStatus": MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEventConfigurationByResourceTypesRequestRequestTypeDef = TypedDict(
     "UpdateEventConfigurationByResourceTypesRequestRequestTypeDef",
     {
@@ -3271,34 +3830,44 @@
     "GetWirelessGatewayFirmwareInformationResponseTypeDef",
     {
         "LoRaWAN": LoRaWANGatewayCurrentVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateWirelessGatewayTaskCreateTypeDef = TypedDict(
-    "UpdateWirelessGatewayTaskCreateTypeDef",
+UpdateWirelessGatewayTaskCreateOutputTypeDef = TypedDict(
+    "UpdateWirelessGatewayTaskCreateOutputTypeDef",
     {
         "UpdateDataSource": str,
         "UpdateDataRole": str,
-        "LoRaWAN": LoRaWANUpdateGatewayTaskCreateTypeDef,
+        "LoRaWAN": LoRaWANUpdateGatewayTaskCreateOutputTypeDef,
     },
     total=False,
 )
 
 UpdateWirelessGatewayTaskEntryTypeDef = TypedDict(
     "UpdateWirelessGatewayTaskEntryTypeDef",
     {
         "Id": str,
         "LoRaWAN": LoRaWANUpdateGatewayTaskEntryTypeDef,
         "Arn": str,
     },
     total=False,
 )
 
+UpdateWirelessGatewayTaskCreateTypeDef = TypedDict(
+    "UpdateWirelessGatewayTaskCreateTypeDef",
+    {
+        "UpdateDataSource": str,
+        "UpdateDataRole": str,
+        "LoRaWAN": LoRaWANUpdateGatewayTaskCreateTypeDef,
+    },
+    total=False,
+)
+
 SendDataToMulticastGroupRequestRequestTypeDef = TypedDict(
     "SendDataToMulticastGroupRequestRequestTypeDef",
     {
         "Id": str,
         "PayloadData": str,
         "WirelessMetadata": MulticastWirelessMetadataTypeDef,
     },
@@ -3316,20 +3885,22 @@
     {
         "Solvers": PositionSolverConfigurationsTypeDef,
         "Destination": str,
     },
     total=False,
 )
 
+
 class PutPositionConfigurationRequestRequestTypeDef(
     _RequiredPutPositionConfigurationRequestRequestTypeDef,
     _OptionalPutPositionConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 GetPositionConfigurationResponseTypeDef = TypedDict(
     "GetPositionConfigurationResponseTypeDef",
     {
         "Solvers": PositionSolverDetailsTypeDef,
         "Destination": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -3346,16 +3917,16 @@
     total=False,
 )
 
 GetLogLevelsByResourceTypesResponseTypeDef = TypedDict(
     "GetLogLevelsByResourceTypesResponseTypeDef",
     {
         "DefaultLogLevel": LogLevelType,
-        "WirelessGatewayLogOptions": List[WirelessGatewayLogOptionTypeDef],
-        "WirelessDeviceLogOptions": List[WirelessDeviceLogOptionTypeDef],
+        "WirelessGatewayLogOptions": List[WirelessGatewayLogOptionOutputTypeDef],
+        "WirelessDeviceLogOptions": List[WirelessDeviceLogOptionOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateLogLevelsByResourceTypesRequestRequestTypeDef = TypedDict(
     "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
     {
@@ -3380,14 +3951,32 @@
     {
         "NextToken": str,
         "WirelessDeviceList": List[WirelessDeviceStatisticsTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+GetWirelessDeviceResponseTypeDef = TypedDict(
+    "GetWirelessDeviceResponseTypeDef",
+    {
+        "Type": WirelessDeviceTypeType,
+        "Name": str,
+        "Description": str,
+        "DestinationName": str,
+        "Id": str,
+        "Arn": str,
+        "ThingName": str,
+        "ThingArn": str,
+        "LoRaWAN": LoRaWANDeviceOutputTypeDef,
+        "Sidewalk": SidewalkDeviceTypeDef,
+        "Positioning": PositioningConfigStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateWirelessDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWirelessDeviceRequestRequestTypeDef",
     {
         "Type": WirelessDeviceTypeType,
         "DestinationName": str,
     },
 )
@@ -3401,37 +3990,21 @@
         "Tags": Sequence[TagTypeDef],
         "Positioning": PositioningConfigStatusType,
         "Sidewalk": SidewalkCreateWirelessDeviceTypeDef,
     },
     total=False,
 )
 
+
 class CreateWirelessDeviceRequestRequestTypeDef(
     _RequiredCreateWirelessDeviceRequestRequestTypeDef,
     _OptionalCreateWirelessDeviceRequestRequestTypeDef,
 ):
     pass
 
-GetWirelessDeviceResponseTypeDef = TypedDict(
-    "GetWirelessDeviceResponseTypeDef",
-    {
-        "Type": WirelessDeviceTypeType,
-        "Name": str,
-        "Description": str,
-        "DestinationName": str,
-        "Id": str,
-        "Arn": str,
-        "ThingName": str,
-        "ThingArn": str,
-        "LoRaWAN": LoRaWANDeviceTypeDef,
-        "Sidewalk": SidewalkDeviceTypeDef,
-        "Positioning": PositioningConfigStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateWirelessDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWirelessDeviceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
@@ -3443,27 +4016,29 @@
         "Description": str,
         "LoRaWAN": LoRaWANUpdateDeviceTypeDef,
         "Positioning": PositioningConfigStatusType,
     },
     total=False,
 )
 
+
 class UpdateWirelessDeviceRequestRequestTypeDef(
     _RequiredUpdateWirelessDeviceRequestRequestTypeDef,
     _OptionalUpdateWirelessDeviceRequestRequestTypeDef,
 ):
     pass
 
+
 DownlinkQueueMessageTypeDef = TypedDict(
     "DownlinkQueueMessageTypeDef",
     {
         "MessageId": str,
         "TransmitMode": int,
         "ReceivedAt": str,
-        "LoRaWAN": LoRaWANSendDataToDeviceTypeDef,
+        "LoRaWAN": LoRaWANSendDataToDeviceOutputTypeDef,
     },
     total=False,
 )
 
 WirelessMetadataTypeDef = TypedDict(
     "WirelessMetadataTypeDef",
     {
@@ -3492,14 +4067,34 @@
         "IdentifierType": IdentifierTypeType,
         "PartnerType": Literal["Sidewalk"],
         "Events": EventNotificationItemConfigurationsTypeDef,
     },
     total=False,
 )
 
+GetWirelessGatewayTaskDefinitionResponseTypeDef = TypedDict(
+    "GetWirelessGatewayTaskDefinitionResponseTypeDef",
+    {
+        "AutoCreateTasks": bool,
+        "Name": str,
+        "Update": UpdateWirelessGatewayTaskCreateOutputTypeDef,
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListWirelessGatewayTaskDefinitionsResponseTypeDef = TypedDict(
+    "ListWirelessGatewayTaskDefinitionsResponseTypeDef",
+    {
+        "NextToken": str,
+        "TaskDefinitions": List[UpdateWirelessGatewayTaskEntryTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     {
         "AutoCreateTasks": bool,
     },
 )
 _OptionalCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef = TypedDict(
@@ -3509,39 +4104,21 @@
         "Update": UpdateWirelessGatewayTaskCreateTypeDef,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef(
     _RequiredCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     _OptionalCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
 ):
     pass
 
-GetWirelessGatewayTaskDefinitionResponseTypeDef = TypedDict(
-    "GetWirelessGatewayTaskDefinitionResponseTypeDef",
-    {
-        "AutoCreateTasks": bool,
-        "Name": str,
-        "Update": UpdateWirelessGatewayTaskCreateTypeDef,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListWirelessGatewayTaskDefinitionsResponseTypeDef = TypedDict(
-    "ListWirelessGatewayTaskDefinitionsResponseTypeDef",
-    {
-        "NextToken": str,
-        "TaskDefinitions": List[UpdateWirelessGatewayTaskEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ListPositionConfigurationsResponseTypeDef = TypedDict(
     "ListPositionConfigurationsResponseTypeDef",
     {
         "PositionConfigurationList": List[PositionConfigurationItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -3569,20 +4146,22 @@
     "_OptionalSendDataToWirelessDeviceRequestRequestTypeDef",
     {
         "WirelessMetadata": WirelessMetadataTypeDef,
     },
     total=False,
 )
 
+
 class SendDataToWirelessDeviceRequestRequestTypeDef(
     _RequiredSendDataToWirelessDeviceRequestRequestTypeDef,
     _OptionalSendDataToWirelessDeviceRequestRequestTypeDef,
 ):
     pass
 
+
 GetPositionEstimateRequestRequestTypeDef = TypedDict(
     "GetPositionEstimateRequestRequestTypeDef",
     {
         "WiFiAccessPoints": Sequence[WiFiAccessPointTypeDef],
         "CellTowers": CellTowersTypeDef,
         "Ip": IpTypeDef,
         "Gnss": GnssTypeDef,
```

### Comparing `mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless.egg-info/PKG-INFO` & `mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotwireless
-Version: 1.28.0
-Summary: Type annotations for boto3.IoTWireless 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTWireless 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iotwireless"></a>
 
 # mypy-boto3-iotwireless
 
 [![PyPI - mypy-boto3-iotwireless](https://img.shields.io/pypi/v/mypy-boto3-iotwireless.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotwireless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotwireless.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotwireless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotwireless?color=blue)](https://pypistats.org/packages/mypy-boto3-iotwireless)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotwireless)](https://pepy.tech/project/mypy-boto3-iotwireless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTWireless 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
+[boto3.IoTWireless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
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
 [mypy-boto3-iotwireless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -335,33 +335,40 @@
 ### Typed dictionaries
 
 `mypy_boto3_iotwireless.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotwireless.type_defs import (
+    SessionKeysAbpV10XOutputTypeDef,
     SessionKeysAbpV10XTypeDef,
+    SessionKeysAbpV11OutputTypeDef,
     SessionKeysAbpV11TypeDef,
     AccuracyTypeDef,
+    ApplicationConfigOutputTypeDef,
     ApplicationConfigTypeDef,
     SidewalkAccountInfoTypeDef,
     TagTypeDef,
+    SidewalkAccountInfoOutputTypeDef,
     AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef,
     AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef,
     AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     AssociateWirelessDeviceWithThingRequestRequestTypeDef,
     AssociateWirelessGatewayWithCertificateRequestRequestTypeDef,
     AssociateWirelessGatewayWithCertificateResponseTypeDef,
     AssociateWirelessGatewayWithThingRequestRequestTypeDef,
+    BeaconingOutputTypeDef,
     BeaconingTypeDef,
     CancelMulticastGroupSessionRequestRequestTypeDef,
     CdmaLocalIdTypeDef,
     CdmaNmrObjTypeDef,
     CertificateListTypeDef,
+    LoRaWANConnectionStatusEventNotificationConfigurationsOutputTypeDef,
     LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef,
+    LoRaWANConnectionStatusResourceTypeEventConfigurationOutputTypeDef,
     LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef,
     CreateDestinationResponseTypeDef,
     LoRaWANDeviceProfileTypeDef,
     CreateDeviceProfileResponseTypeDef,
     LoRaWANFuotaTaskTypeDef,
     CreateFuotaTaskResponseTypeDef,
     LoRaWANMulticastTypeDef,
@@ -388,36 +395,42 @@
     DeleteWirelessDeviceRequestRequestTypeDef,
     DeleteWirelessGatewayRequestRequestTypeDef,
     DeleteWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     DeleteWirelessGatewayTaskRequestRequestTypeDef,
     DeregisterWirelessDeviceRequestRequestTypeDef,
     DestinationsTypeDef,
     DeviceProfileTypeDef,
+    SidewalkEventNotificationConfigurationsOutputTypeDef,
     SidewalkEventNotificationConfigurationsTypeDef,
+    SidewalkResourceTypeEventConfigurationOutputTypeDef,
     SidewalkResourceTypeEventConfigurationTypeDef,
     DisassociateAwsAccountFromPartnerAccountRequestRequestTypeDef,
     DisassociateMulticastGroupFromFuotaTaskRequestRequestTypeDef,
     DisassociateWirelessDeviceFromFuotaTaskRequestRequestTypeDef,
     DisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
     DisassociateWirelessDeviceFromThingRequestRequestTypeDef,
     DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef,
     DisassociateWirelessGatewayFromThingRequestRequestTypeDef,
+    PositioningOutputTypeDef,
     PositioningTypeDef,
     FuotaTaskTypeDef,
+    GatewayListItemOutputTypeDef,
     GatewayListItemTypeDef,
     GetDestinationRequestRequestTypeDef,
     GetDestinationResponseTypeDef,
     GetDeviceProfileRequestRequestTypeDef,
+    LoRaWANDeviceProfileOutputTypeDef,
     GetFuotaTaskRequestRequestTypeDef,
     LoRaWANFuotaTaskGetInfoTypeDef,
     GetMulticastGroupRequestRequestTypeDef,
     LoRaWANMulticastGetTypeDef,
     GetMulticastGroupSessionRequestRequestTypeDef,
-    LoRaWANMulticastSessionTypeDef,
+    LoRaWANMulticastSessionOutputTypeDef,
     GetNetworkAnalyzerConfigurationRequestRequestTypeDef,
+    TraceContentOutputTypeDef,
     GetPartnerAccountRequestRequestTypeDef,
     SidewalkAccountInfoWithFingerprintTypeDef,
     GetPositionConfigurationRequestRequestTypeDef,
     GnssTypeDef,
     IpTypeDef,
     WiFiAccessPointTypeDef,
     GetPositionEstimateResponseTypeDef,
@@ -444,15 +457,17 @@
     GetWirelessGatewayStatisticsResponseTypeDef,
     GetWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     GetWirelessGatewayTaskRequestRequestTypeDef,
     GetWirelessGatewayTaskResponseTypeDef,
     GlobalIdentityTypeDef,
     GsmLocalIdTypeDef,
     ImportedSidewalkDeviceTypeDef,
+    LoRaWANJoinEventNotificationConfigurationsOutputTypeDef,
     LoRaWANJoinEventNotificationConfigurationsTypeDef,
+    LoRaWANJoinResourceTypeEventConfigurationOutputTypeDef,
     LoRaWANJoinResourceTypeEventConfigurationTypeDef,
     ListDestinationsRequestRequestTypeDef,
     ListDeviceProfilesRequestRequestTypeDef,
     ListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef,
     ListEventConfigurationsRequestRequestTypeDef,
     ListFuotaTasksRequestRequestTypeDef,
     ListMulticastGroupsByFuotaTaskRequestRequestTypeDef,
@@ -463,24 +478,29 @@
     NetworkAnalyzerConfigurationsTypeDef,
     ListPartnerAccountsRequestRequestTypeDef,
     ListPositionConfigurationsRequestRequestTypeDef,
     ListQueuedMessagesRequestRequestTypeDef,
     ListServiceProfilesRequestRequestTypeDef,
     ServiceProfileTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListWirelessDeviceImportTasksRequestRequestTypeDef,
     ListWirelessDevicesRequestRequestTypeDef,
     ListWirelessGatewayTaskDefinitionsRequestRequestTypeDef,
     ListWirelessGatewaysRequestRequestTypeDef,
     LoRaWANGatewayMetadataTypeDef,
+    OtaaV10XOutputTypeDef,
+    OtaaV11OutputTypeDef,
     OtaaV10XTypeDef,
     OtaaV11TypeDef,
+    LoRaWANGatewayVersionOutputTypeDef,
     LoRaWANGatewayVersionTypeDef,
     LoRaWANListDeviceTypeDef,
     LoRaWANMulticastMetadataTypeDef,
+    LoRaWANMulticastSessionTypeDef,
     LoRaWANStartFuotaTaskTypeDef,
     UpdateAbpV10XTypeDef,
     UpdateAbpV11TypeDef,
     LteLocalIdTypeDef,
     LteNmrObjTypeDef,
     SemtechGnssConfigurationTypeDef,
     SemtechGnssDetailTypeDef,
@@ -503,135 +523,158 @@
     UntagResourceRequestRequestTypeDef,
     UpdateDestinationRequestRequestTypeDef,
     UpdatePositionRequestRequestTypeDef,
     UpdateResourcePositionRequestRequestTypeDef,
     UpdateWirelessGatewayRequestRequestTypeDef,
     WcdmaLocalIdTypeDef,
     WcdmaNmrObjTypeDef,
+    WirelessDeviceEventLogOptionOutputTypeDef,
     WirelessDeviceEventLogOptionTypeDef,
+    WirelessGatewayEventLogOptionOutputTypeDef,
     WirelessGatewayEventLogOptionTypeDef,
+    AbpV10XOutputTypeDef,
     AbpV10XTypeDef,
+    AbpV11OutputTypeDef,
     AbpV11TypeDef,
     GetPositionResponseTypeDef,
-    AssociateAwsAccountWithPartnerAccountResponseTypeDef,
     AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef,
     CreateDestinationRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    AssociateAwsAccountWithPartnerAccountResponseTypeDef,
+    LoRaWANGatewayOutputTypeDef,
     LoRaWANGatewayTypeDef,
     CdmaObjTypeDef,
     SidewalkDeviceTypeDef,
     SidewalkListDeviceTypeDef,
+    ConnectionStatusEventConfigurationOutputTypeDef,
     ConnectionStatusEventConfigurationTypeDef,
+    ConnectionStatusResourceTypeEventConfigurationOutputTypeDef,
     ConnectionStatusResourceTypeEventConfigurationTypeDef,
     CreateDeviceProfileRequestRequestTypeDef,
     CreateFuotaTaskRequestRequestTypeDef,
     UpdateFuotaTaskRequestRequestTypeDef,
     CreateMulticastGroupRequestRequestTypeDef,
     UpdateMulticastGroupRequestRequestTypeDef,
     CreateNetworkAnalyzerConfigurationRequestRequestTypeDef,
-    GetNetworkAnalyzerConfigurationResponseTypeDef,
     UpdateNetworkAnalyzerConfigurationRequestRequestTypeDef,
     CreateServiceProfileRequestRequestTypeDef,
     SidewalkGetDeviceProfileTypeDef,
     ListDestinationsResponseTypeDef,
     ListDeviceProfilesResponseTypeDef,
+    DeviceRegistrationStateEventConfigurationOutputTypeDef,
+    MessageDeliveryStatusEventConfigurationOutputTypeDef,
+    ProximityEventConfigurationOutputTypeDef,
     DeviceRegistrationStateEventConfigurationTypeDef,
     MessageDeliveryStatusEventConfigurationTypeDef,
     ProximityEventConfigurationTypeDef,
+    DeviceRegistrationStateResourceTypeEventConfigurationOutputTypeDef,
+    MessageDeliveryStatusResourceTypeEventConfigurationOutputTypeDef,
+    ProximityResourceTypeEventConfigurationOutputTypeDef,
     DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,
     MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
     ProximityResourceTypeEventConfigurationTypeDef,
+    FPortsOutputTypeDef,
     FPortsTypeDef,
     UpdateFPortsTypeDef,
     ListFuotaTasksResponseTypeDef,
+    ParticipatingGatewaysOutputTypeDef,
     ParticipatingGatewaysTypeDef,
     GetFuotaTaskResponseTypeDef,
     GetMulticastGroupResponseTypeDef,
     GetMulticastGroupSessionResponseTypeDef,
-    StartMulticastGroupSessionRequestRequestTypeDef,
+    GetNetworkAnalyzerConfigurationResponseTypeDef,
     GetPartnerAccountResponseTypeDef,
     ListPartnerAccountsResponseTypeDef,
     GetServiceProfileResponseTypeDef,
     GetWirelessDeviceImportTaskResponseTypeDef,
     WirelessDeviceImportTaskTypeDef,
     GsmNmrObjTypeDef,
     ImportedWirelessDeviceTypeDef,
+    JoinEventConfigurationOutputTypeDef,
     JoinEventConfigurationTypeDef,
+    JoinResourceTypeEventConfigurationOutputTypeDef,
     JoinResourceTypeEventConfigurationTypeDef,
     ListMulticastGroupsByFuotaTaskResponseTypeDef,
     ListMulticastGroupsResponseTypeDef,
     ListNetworkAnalyzerConfigurationsResponseTypeDef,
     ListServiceProfilesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     LoRaWANDeviceMetadataTypeDef,
     LoRaWANGatewayCurrentVersionTypeDef,
-    LoRaWANUpdateGatewayTaskCreateTypeDef,
+    LoRaWANUpdateGatewayTaskCreateOutputTypeDef,
     LoRaWANUpdateGatewayTaskEntryTypeDef,
+    LoRaWANUpdateGatewayTaskCreateTypeDef,
     MulticastWirelessMetadataTypeDef,
+    StartMulticastGroupSessionRequestRequestTypeDef,
     StartFuotaTaskRequestRequestTypeDef,
     LteObjTypeDef,
     PositionSolverConfigurationsTypeDef,
     PositionSolverDetailsTypeDef,
     StartSingleWirelessDeviceImportTaskRequestRequestTypeDef,
     StartWirelessDeviceImportTaskRequestRequestTypeDef,
     UpdatePartnerAccountRequestRequestTypeDef,
     UpdateWirelessDeviceImportTaskRequestRequestTypeDef,
     TdscdmaObjTypeDef,
     WcdmaObjTypeDef,
+    WirelessDeviceLogOptionOutputTypeDef,
     WirelessDeviceLogOptionTypeDef,
+    WirelessGatewayLogOptionOutputTypeDef,
     WirelessGatewayLogOptionTypeDef,
-    CreateWirelessGatewayRequestRequestTypeDef,
     GetWirelessGatewayResponseTypeDef,
     WirelessGatewayStatisticsTypeDef,
+    CreateWirelessGatewayRequestRequestTypeDef,
     WirelessDeviceStatisticsTypeDef,
     GetDeviceProfileResponseTypeDef,
+    LoRaWANDeviceOutputTypeDef,
     LoRaWANDeviceTypeDef,
     LoRaWANUpdateDeviceTypeDef,
+    LoRaWANSendDataToDeviceOutputTypeDef,
     LoRaWANSendDataToDeviceTypeDef,
     ListWirelessDeviceImportTasksResponseTypeDef,
     GsmObjTypeDef,
     ListDevicesForWirelessDeviceImportTaskResponseTypeDef,
     EventNotificationItemConfigurationsTypeDef,
     GetResourceEventConfigurationResponseTypeDef,
     UpdateResourceEventConfigurationRequestRequestTypeDef,
     GetEventConfigurationByResourceTypesResponseTypeDef,
     UpdateEventConfigurationByResourceTypesRequestRequestTypeDef,
     GetWirelessDeviceStatisticsResponseTypeDef,
     GetWirelessGatewayFirmwareInformationResponseTypeDef,
-    UpdateWirelessGatewayTaskCreateTypeDef,
+    UpdateWirelessGatewayTaskCreateOutputTypeDef,
     UpdateWirelessGatewayTaskEntryTypeDef,
+    UpdateWirelessGatewayTaskCreateTypeDef,
     SendDataToMulticastGroupRequestRequestTypeDef,
     PutPositionConfigurationRequestRequestTypeDef,
     GetPositionConfigurationResponseTypeDef,
     PositionConfigurationItemTypeDef,
     GetLogLevelsByResourceTypesResponseTypeDef,
     UpdateLogLevelsByResourceTypesRequestRequestTypeDef,
     ListWirelessGatewaysResponseTypeDef,
     ListWirelessDevicesResponseTypeDef,
-    CreateWirelessDeviceRequestRequestTypeDef,
     GetWirelessDeviceResponseTypeDef,
+    CreateWirelessDeviceRequestRequestTypeDef,
     UpdateWirelessDeviceRequestRequestTypeDef,
     DownlinkQueueMessageTypeDef,
     WirelessMetadataTypeDef,
     CellTowersTypeDef,
     EventConfigurationItemTypeDef,
-    CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     GetWirelessGatewayTaskDefinitionResponseTypeDef,
     ListWirelessGatewayTaskDefinitionsResponseTypeDef,
+    CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     ListPositionConfigurationsResponseTypeDef,
     ListQueuedMessagesResponseTypeDef,
     SendDataToWirelessDeviceRequestRequestTypeDef,
     GetPositionEstimateRequestRequestTypeDef,
     ListEventConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> SessionKeysAbpV10XTypeDef:
+def get_structure() -> SessionKeysAbpV10XOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotwireless-1.28.0/mypy_boto3_iotwireless.egg-info/SOURCES.txt` & `mypy-boto3-iotwireless-1.28.12/mypy_boto3_iotwireless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.28.0/setup.py` & `mypy-boto3-iotwireless-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotwireless",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_iotwireless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTWireless 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.IoTWireless 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

