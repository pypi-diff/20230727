# Comparing `tmp/mypy-boto3-groundstation-1.28.0.tar.gz` & `tmp/mypy-boto3-groundstation-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-groundstation-1.28.0.tar", last modified: Thu Jul  6 20:59:40 2023, max compression
+gzip compressed data, was "mypy-boto3-groundstation-1.28.12.tar", last modified: Thu Jul 27 05:34:45 2023, max compression
```

## Comparing `mypy-boto3-groundstation-1.28.0.tar` & `mypy-boto3-groundstation-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:40.914315 mypy-boto3-groundstation-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:42:23.000000 mypy-boto3-groundstation-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19266 2023-07-06 20:59:40.914315 mypy-boto3-groundstation-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17757 2023-07-06 20:42:23.000000 mypy-boto3-groundstation-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:40.906315 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-06 20:42:23.000000 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-06 20:42:23.000000 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-06 20:42:23.000000 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26848 2023-07-06 20:42:23.000000 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26800 2023-07-06 20:42:23.000000 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-07-06 20:42:24.000000 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10897 2023-07-06 20:42:24.000000 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-07-06 20:42:23.000000 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-07-06 20:42:23.000000 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:42:23.000000 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40185 2023-07-06 20:42:25.000000 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40136 2023-07-06 20:42:24.000000 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:42:23.000000 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-06 20:42:23.000000 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-06 20:42:23.000000 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:40.914315 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19266 2023-07-06 20:59:40.000000 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-06 20:59:40.000000 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:40.000000 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:40.000000 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:40.000000 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 20:59:40.000000 mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:40.914315 mypy-boto3-groundstation-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-06 20:42:23.000000 mypy-boto3-groundstation-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:45.144498 mypy-boto3-groundstation-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20170 2023-07-27 05:34:45.140498 mypy-boto3-groundstation-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18659 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:45.132498 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26848 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26800 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-27 05:23:11.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-27 05:23:11.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-07-27 05:23:10.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    48959 2023-07-27 05:23:12.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48894 2023-07-27 05:23:11.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-27 05:23:10.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-27 05:23:10.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:45.140498 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20170 2023-07-27 05:34:44.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-27 05:34:44.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:44.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:44.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:44.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 05:34:44.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:45.144498 mypy-boto3-groundstation-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/setup.py
```

### Comparing `mypy-boto3-groundstation-1.28.0/LICENSE` & `mypy-boto3-groundstation-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.0/PKG-INFO` & `mypy-boto3-groundstation-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-groundstation
-Version: 1.28.0
-Summary: Type annotations for boto3.GroundStation 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.GroundStation 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-groundstation"></a>
 
 # mypy-boto3-groundstation
 
 [![PyPI - mypy-boto3-groundstation](https://img.shields.io/pypi/v/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-groundstation?color=blue)](https://pypistats.org/packages/mypy-boto3-groundstation)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-groundstation)](https://pepy.tech/project/mypy-boto3-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GroundStation 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[boto3.GroundStation 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
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
 [mypy-boto3-groundstation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -387,55 +387,68 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_groundstation.type_defs import (
     ComponentVersionTypeDef,
     AggregateStatusTypeDef,
     AntennaDemodDecodeDetailsTypeDef,
+    DecodeConfigOutputTypeDef,
+    DemodulationConfigOutputTypeDef,
     DecodeConfigTypeDef,
     DemodulationConfigTypeDef,
+    EirpOutputTypeDef,
     EirpTypeDef,
     CancelContactRequestRequestTypeDef,
     ComponentStatusDataTypeDef,
     S3RecordingDetailsTypeDef,
     ConfigIdResponseTypeDef,
     ConfigListItemTypeDef,
+    DataflowEndpointConfigOutputTypeDef,
+    S3RecordingConfigOutputTypeDef,
+    TrackingConfigOutputTypeDef,
+    UplinkEchoConfigOutputTypeDef,
     DataflowEndpointConfigTypeDef,
     S3RecordingConfigTypeDef,
     TrackingConfigTypeDef,
     UplinkEchoConfigTypeDef,
+    SocketAddressOutputTypeDef,
     SocketAddressTypeDef,
     ElevationTypeDef,
     ContactIdResponseTypeDef,
     KmsKeyTypeDef,
     DataflowEndpointGroupIdResponseTypeDef,
     DataflowEndpointListItemTypeDef,
     DeleteConfigRequestRequestTypeDef,
     DeleteDataflowEndpointGroupRequestRequestTypeDef,
     DeleteEphemerisRequestRequestTypeDef,
     DeleteMissionProfileRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeContactRequestRequestTypeDef,
     DescribeEphemerisRequestRequestTypeDef,
     DiscoveryDataTypeDef,
+    SecurityDetailsOutputTypeDef,
     SecurityDetailsTypeDef,
-    S3ObjectTypeDef,
+    S3ObjectOutputTypeDef,
     EphemerisIdResponseTypeDef,
     EphemerisMetaDataTypeDef,
+    FrequencyBandwidthOutputTypeDef,
     FrequencyBandwidthTypeDef,
+    FrequencyOutputTypeDef,
     FrequencyTypeDef,
     GetAgentConfigurationRequestRequestTypeDef,
     GetAgentConfigurationResponseTypeDef,
     GetConfigRequestRequestTypeDef,
     GetDataflowEndpointGroupRequestRequestTypeDef,
     GetMinuteUsageRequestRequestTypeDef,
     GetMinuteUsageResponseTypeDef,
     GetMissionProfileRequestRequestTypeDef,
+    KmsKeyOutputTypeDef,
     GetSatelliteRequestRequestTypeDef,
     GroundStationDataTypeDef,
+    IntegerRangeOutputTypeDef,
     IntegerRangeTypeDef,
     ListConfigsRequestListConfigsPaginateTypeDef,
     ListConfigsRequestRequestTypeDef,
     ListContactsRequestListContactsPaginateTypeDef,
     ListContactsRequestRequestTypeDef,
     ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef,
     ListDataflowEndpointGroupsRequestRequestTypeDef,
@@ -447,67 +460,80 @@
     ListMissionProfilesRequestRequestTypeDef,
     MissionProfileListItemTypeDef,
     ListSatellitesRequestListSatellitesPaginateTypeDef,
     ListSatellitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     MissionProfileIdResponseTypeDef,
+    S3ObjectTypeDef,
     PaginatorConfigTypeDef,
     RegisterAgentResponseTypeDef,
     ReserveContactRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TimeRangeTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgentStatusResponseTypeDef,
     UpdateEphemerisRequestRequestTypeDef,
     AgentDetailsTypeDef,
     UpdateAgentStatusRequestRequestTypeDef,
     ListConfigsResponseTypeDef,
+    ConnectionDetailsOutputTypeDef,
+    DataflowEndpointOutputTypeDef,
     ConnectionDetailsTypeDef,
     DataflowEndpointTypeDef,
     ContactDataTypeDef,
     CreateMissionProfileRequestRequestTypeDef,
-    GetMissionProfileResponseTypeDef,
     UpdateMissionProfileRequestRequestTypeDef,
     ListDataflowEndpointGroupsResponseTypeDef,
     DescribeContactRequestContactScheduledWaitTypeDef,
     EphemerisDescriptionTypeDef,
     EphemerisItemTypeDef,
-    OEMEphemerisTypeDef,
     GetSatelliteResponseTypeDef,
     SatelliteListItemTypeDef,
+    SpectrumConfigOutputTypeDef,
+    UplinkSpectrumConfigOutputTypeDef,
     SpectrumConfigTypeDef,
     UplinkSpectrumConfigTypeDef,
+    GetMissionProfileResponseTypeDef,
     ListGroundStationsResponseTypeDef,
+    RangedSocketAddressOutputTypeDef,
     RangedSocketAddressTypeDef,
     ListMissionProfilesResponseTypeDef,
+    OEMEphemerisTypeDef,
     TLEDataTypeDef,
     RegisterAgentRequestRequestTypeDef,
     ListContactsResponseTypeDef,
     EphemerisTypeDescriptionTypeDef,
     ListEphemeridesResponseTypeDef,
     ListSatellitesResponseTypeDef,
+    AntennaDownlinkConfigOutputTypeDef,
+    AntennaDownlinkDemodDecodeConfigOutputTypeDef,
+    AntennaUplinkConfigOutputTypeDef,
     AntennaDownlinkConfigTypeDef,
     AntennaDownlinkDemodDecodeConfigTypeDef,
     AntennaUplinkConfigTypeDef,
+    RangedConnectionDetailsOutputTypeDef,
     RangedConnectionDetailsTypeDef,
     TLEEphemerisTypeDef,
     DescribeEphemerisResponseTypeDef,
+    ConfigTypeDataOutputTypeDef,
     ConfigTypeDataTypeDef,
+    AwsGroundStationAgentEndpointOutputTypeDef,
     AwsGroundStationAgentEndpointTypeDef,
     EphemerisDataTypeDef,
-    CreateConfigRequestRequestTypeDef,
     GetConfigResponseTypeDef,
+    CreateConfigRequestRequestTypeDef,
     UpdateConfigRequestRequestTypeDef,
+    EndpointDetailsOutputTypeDef,
     EndpointDetailsTypeDef,
     CreateEphemerisRequestRequestTypeDef,
     ConfigDetailsTypeDef,
-    CreateDataflowEndpointGroupRequestRequestTypeDef,
     GetDataflowEndpointGroupResponseTypeDef,
+    CreateDataflowEndpointGroupRequestRequestTypeDef,
     DestinationTypeDef,
     SourceTypeDef,
     DataflowDetailTypeDef,
     DescribeContactResponseTypeDef,
 )
```

### Comparing `mypy-boto3-groundstation-1.28.0/README.md` & `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-groundstation
+Version: 1.28.12
+Summary: Type annotations for boto3.GroundStation 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 groundstation type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-groundstation"></a>
 
 # mypy-boto3-groundstation
 
 [![PyPI - mypy-boto3-groundstation](https://img.shields.io/pypi/v/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-groundstation?color=blue)](https://pypistats.org/packages/mypy-boto3-groundstation)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-groundstation)](https://pepy.tech/project/mypy-boto3-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GroundStation 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[boto3.GroundStation 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
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
 [mypy-boto3-groundstation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -355,55 +387,68 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_groundstation.type_defs import (
     ComponentVersionTypeDef,
     AggregateStatusTypeDef,
     AntennaDemodDecodeDetailsTypeDef,
+    DecodeConfigOutputTypeDef,
+    DemodulationConfigOutputTypeDef,
     DecodeConfigTypeDef,
     DemodulationConfigTypeDef,
+    EirpOutputTypeDef,
     EirpTypeDef,
     CancelContactRequestRequestTypeDef,
     ComponentStatusDataTypeDef,
     S3RecordingDetailsTypeDef,
     ConfigIdResponseTypeDef,
     ConfigListItemTypeDef,
+    DataflowEndpointConfigOutputTypeDef,
+    S3RecordingConfigOutputTypeDef,
+    TrackingConfigOutputTypeDef,
+    UplinkEchoConfigOutputTypeDef,
     DataflowEndpointConfigTypeDef,
     S3RecordingConfigTypeDef,
     TrackingConfigTypeDef,
     UplinkEchoConfigTypeDef,
+    SocketAddressOutputTypeDef,
     SocketAddressTypeDef,
     ElevationTypeDef,
     ContactIdResponseTypeDef,
     KmsKeyTypeDef,
     DataflowEndpointGroupIdResponseTypeDef,
     DataflowEndpointListItemTypeDef,
     DeleteConfigRequestRequestTypeDef,
     DeleteDataflowEndpointGroupRequestRequestTypeDef,
     DeleteEphemerisRequestRequestTypeDef,
     DeleteMissionProfileRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeContactRequestRequestTypeDef,
     DescribeEphemerisRequestRequestTypeDef,
     DiscoveryDataTypeDef,
+    SecurityDetailsOutputTypeDef,
     SecurityDetailsTypeDef,
-    S3ObjectTypeDef,
+    S3ObjectOutputTypeDef,
     EphemerisIdResponseTypeDef,
     EphemerisMetaDataTypeDef,
+    FrequencyBandwidthOutputTypeDef,
     FrequencyBandwidthTypeDef,
+    FrequencyOutputTypeDef,
     FrequencyTypeDef,
     GetAgentConfigurationRequestRequestTypeDef,
     GetAgentConfigurationResponseTypeDef,
     GetConfigRequestRequestTypeDef,
     GetDataflowEndpointGroupRequestRequestTypeDef,
     GetMinuteUsageRequestRequestTypeDef,
     GetMinuteUsageResponseTypeDef,
     GetMissionProfileRequestRequestTypeDef,
+    KmsKeyOutputTypeDef,
     GetSatelliteRequestRequestTypeDef,
     GroundStationDataTypeDef,
+    IntegerRangeOutputTypeDef,
     IntegerRangeTypeDef,
     ListConfigsRequestListConfigsPaginateTypeDef,
     ListConfigsRequestRequestTypeDef,
     ListContactsRequestListContactsPaginateTypeDef,
     ListContactsRequestRequestTypeDef,
     ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef,
     ListDataflowEndpointGroupsRequestRequestTypeDef,
@@ -415,67 +460,80 @@
     ListMissionProfilesRequestRequestTypeDef,
     MissionProfileListItemTypeDef,
     ListSatellitesRequestListSatellitesPaginateTypeDef,
     ListSatellitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     MissionProfileIdResponseTypeDef,
+    S3ObjectTypeDef,
     PaginatorConfigTypeDef,
     RegisterAgentResponseTypeDef,
     ReserveContactRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TimeRangeTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgentStatusResponseTypeDef,
     UpdateEphemerisRequestRequestTypeDef,
     AgentDetailsTypeDef,
     UpdateAgentStatusRequestRequestTypeDef,
     ListConfigsResponseTypeDef,
+    ConnectionDetailsOutputTypeDef,
+    DataflowEndpointOutputTypeDef,
     ConnectionDetailsTypeDef,
     DataflowEndpointTypeDef,
     ContactDataTypeDef,
     CreateMissionProfileRequestRequestTypeDef,
-    GetMissionProfileResponseTypeDef,
     UpdateMissionProfileRequestRequestTypeDef,
     ListDataflowEndpointGroupsResponseTypeDef,
     DescribeContactRequestContactScheduledWaitTypeDef,
     EphemerisDescriptionTypeDef,
     EphemerisItemTypeDef,
-    OEMEphemerisTypeDef,
     GetSatelliteResponseTypeDef,
     SatelliteListItemTypeDef,
+    SpectrumConfigOutputTypeDef,
+    UplinkSpectrumConfigOutputTypeDef,
     SpectrumConfigTypeDef,
     UplinkSpectrumConfigTypeDef,
+    GetMissionProfileResponseTypeDef,
     ListGroundStationsResponseTypeDef,
+    RangedSocketAddressOutputTypeDef,
     RangedSocketAddressTypeDef,
     ListMissionProfilesResponseTypeDef,
+    OEMEphemerisTypeDef,
     TLEDataTypeDef,
     RegisterAgentRequestRequestTypeDef,
     ListContactsResponseTypeDef,
     EphemerisTypeDescriptionTypeDef,
     ListEphemeridesResponseTypeDef,
     ListSatellitesResponseTypeDef,
+    AntennaDownlinkConfigOutputTypeDef,
+    AntennaDownlinkDemodDecodeConfigOutputTypeDef,
+    AntennaUplinkConfigOutputTypeDef,
     AntennaDownlinkConfigTypeDef,
     AntennaDownlinkDemodDecodeConfigTypeDef,
     AntennaUplinkConfigTypeDef,
+    RangedConnectionDetailsOutputTypeDef,
     RangedConnectionDetailsTypeDef,
     TLEEphemerisTypeDef,
     DescribeEphemerisResponseTypeDef,
+    ConfigTypeDataOutputTypeDef,
     ConfigTypeDataTypeDef,
+    AwsGroundStationAgentEndpointOutputTypeDef,
     AwsGroundStationAgentEndpointTypeDef,
     EphemerisDataTypeDef,
-    CreateConfigRequestRequestTypeDef,
     GetConfigResponseTypeDef,
+    CreateConfigRequestRequestTypeDef,
     UpdateConfigRequestRequestTypeDef,
+    EndpointDetailsOutputTypeDef,
     EndpointDetailsTypeDef,
     CreateEphemerisRequestRequestTypeDef,
     ConfigDetailsTypeDef,
-    CreateDataflowEndpointGroupRequestRequestTypeDef,
     GetDataflowEndpointGroupResponseTypeDef,
+    CreateDataflowEndpointGroupRequestRequestTypeDef,
     DestinationTypeDef,
     SourceTypeDef,
     DataflowDetailTypeDef,
     DescribeContactResponseTypeDef,
 )
```

### Comparing `mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/__init__.py` & `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/__init__.pyi` & `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/__main__.py` & `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GroundStation 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.GroundStation 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation\nOther"
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

### Comparing `mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/client.py` & `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/client.pyi` & `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/literals.py` & `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,14 +229,15 @@
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
@@ -315,26 +316,28 @@
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

### Comparing `mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/literals.pyi` & `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -227,14 +227,15 @@
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
@@ -313,26 +314,28 @@
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

### Comparing `mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/paginator.py` & `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/paginator.pyi` & `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/type_defs.py` & `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -38,60 +38,72 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ComponentVersionTypeDef",
     "AggregateStatusTypeDef",
     "AntennaDemodDecodeDetailsTypeDef",
+    "DecodeConfigOutputTypeDef",
+    "DemodulationConfigOutputTypeDef",
     "DecodeConfigTypeDef",
     "DemodulationConfigTypeDef",
+    "EirpOutputTypeDef",
     "EirpTypeDef",
     "CancelContactRequestRequestTypeDef",
     "ComponentStatusDataTypeDef",
     "S3RecordingDetailsTypeDef",
     "ConfigIdResponseTypeDef",
     "ConfigListItemTypeDef",
+    "DataflowEndpointConfigOutputTypeDef",
+    "S3RecordingConfigOutputTypeDef",
+    "TrackingConfigOutputTypeDef",
+    "UplinkEchoConfigOutputTypeDef",
     "DataflowEndpointConfigTypeDef",
     "S3RecordingConfigTypeDef",
     "TrackingConfigTypeDef",
     "UplinkEchoConfigTypeDef",
+    "SocketAddressOutputTypeDef",
     "SocketAddressTypeDef",
     "ElevationTypeDef",
     "ContactIdResponseTypeDef",
     "KmsKeyTypeDef",
     "DataflowEndpointGroupIdResponseTypeDef",
     "DataflowEndpointListItemTypeDef",
     "DeleteConfigRequestRequestTypeDef",
     "DeleteDataflowEndpointGroupRequestRequestTypeDef",
     "DeleteEphemerisRequestRequestTypeDef",
     "DeleteMissionProfileRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeContactRequestRequestTypeDef",
     "DescribeEphemerisRequestRequestTypeDef",
     "DiscoveryDataTypeDef",
+    "SecurityDetailsOutputTypeDef",
     "SecurityDetailsTypeDef",
-    "S3ObjectTypeDef",
+    "S3ObjectOutputTypeDef",
     "EphemerisIdResponseTypeDef",
     "EphemerisMetaDataTypeDef",
+    "FrequencyBandwidthOutputTypeDef",
     "FrequencyBandwidthTypeDef",
+    "FrequencyOutputTypeDef",
     "FrequencyTypeDef",
     "GetAgentConfigurationRequestRequestTypeDef",
     "GetAgentConfigurationResponseTypeDef",
     "GetConfigRequestRequestTypeDef",
     "GetDataflowEndpointGroupRequestRequestTypeDef",
     "GetMinuteUsageRequestRequestTypeDef",
     "GetMinuteUsageResponseTypeDef",
     "GetMissionProfileRequestRequestTypeDef",
+    "KmsKeyOutputTypeDef",
     "GetSatelliteRequestRequestTypeDef",
     "GroundStationDataTypeDef",
+    "IntegerRangeOutputTypeDef",
     "IntegerRangeTypeDef",
     "ListConfigsRequestListConfigsPaginateTypeDef",
     "ListConfigsRequestRequestTypeDef",
     "ListContactsRequestListContactsPaginateTypeDef",
     "ListContactsRequestRequestTypeDef",
     "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
     "ListDataflowEndpointGroupsRequestRequestTypeDef",
@@ -103,67 +115,80 @@
     "ListMissionProfilesRequestRequestTypeDef",
     "MissionProfileListItemTypeDef",
     "ListSatellitesRequestListSatellitesPaginateTypeDef",
     "ListSatellitesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "MissionProfileIdResponseTypeDef",
+    "S3ObjectTypeDef",
     "PaginatorConfigTypeDef",
     "RegisterAgentResponseTypeDef",
     "ReserveContactRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TimeRangeTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAgentStatusResponseTypeDef",
     "UpdateEphemerisRequestRequestTypeDef",
     "AgentDetailsTypeDef",
     "UpdateAgentStatusRequestRequestTypeDef",
     "ListConfigsResponseTypeDef",
+    "ConnectionDetailsOutputTypeDef",
+    "DataflowEndpointOutputTypeDef",
     "ConnectionDetailsTypeDef",
     "DataflowEndpointTypeDef",
     "ContactDataTypeDef",
     "CreateMissionProfileRequestRequestTypeDef",
-    "GetMissionProfileResponseTypeDef",
     "UpdateMissionProfileRequestRequestTypeDef",
     "ListDataflowEndpointGroupsResponseTypeDef",
     "DescribeContactRequestContactScheduledWaitTypeDef",
     "EphemerisDescriptionTypeDef",
     "EphemerisItemTypeDef",
-    "OEMEphemerisTypeDef",
     "GetSatelliteResponseTypeDef",
     "SatelliteListItemTypeDef",
+    "SpectrumConfigOutputTypeDef",
+    "UplinkSpectrumConfigOutputTypeDef",
     "SpectrumConfigTypeDef",
     "UplinkSpectrumConfigTypeDef",
+    "GetMissionProfileResponseTypeDef",
     "ListGroundStationsResponseTypeDef",
+    "RangedSocketAddressOutputTypeDef",
     "RangedSocketAddressTypeDef",
     "ListMissionProfilesResponseTypeDef",
+    "OEMEphemerisTypeDef",
     "TLEDataTypeDef",
     "RegisterAgentRequestRequestTypeDef",
     "ListContactsResponseTypeDef",
     "EphemerisTypeDescriptionTypeDef",
     "ListEphemeridesResponseTypeDef",
     "ListSatellitesResponseTypeDef",
+    "AntennaDownlinkConfigOutputTypeDef",
+    "AntennaDownlinkDemodDecodeConfigOutputTypeDef",
+    "AntennaUplinkConfigOutputTypeDef",
     "AntennaDownlinkConfigTypeDef",
     "AntennaDownlinkDemodDecodeConfigTypeDef",
     "AntennaUplinkConfigTypeDef",
+    "RangedConnectionDetailsOutputTypeDef",
     "RangedConnectionDetailsTypeDef",
     "TLEEphemerisTypeDef",
     "DescribeEphemerisResponseTypeDef",
+    "ConfigTypeDataOutputTypeDef",
     "ConfigTypeDataTypeDef",
+    "AwsGroundStationAgentEndpointOutputTypeDef",
     "AwsGroundStationAgentEndpointTypeDef",
     "EphemerisDataTypeDef",
-    "CreateConfigRequestRequestTypeDef",
     "GetConfigResponseTypeDef",
+    "CreateConfigRequestRequestTypeDef",
     "UpdateConfigRequestRequestTypeDef",
+    "EndpointDetailsOutputTypeDef",
     "EndpointDetailsTypeDef",
     "CreateEphemerisRequestRequestTypeDef",
     "ConfigDetailsTypeDef",
-    "CreateDataflowEndpointGroupRequestRequestTypeDef",
     "GetDataflowEndpointGroupResponseTypeDef",
+    "CreateDataflowEndpointGroupRequestRequestTypeDef",
     "DestinationTypeDef",
     "SourceTypeDef",
     "DataflowDetailTypeDef",
     "DescribeContactResponseTypeDef",
 )
 
 ComponentVersionTypeDef = TypedDict(
@@ -184,41 +209,61 @@
     "_OptionalAggregateStatusTypeDef",
     {
         "signatureMap": Mapping[str, bool],
     },
     total=False,
 )
 
-
 class AggregateStatusTypeDef(_RequiredAggregateStatusTypeDef, _OptionalAggregateStatusTypeDef):
     pass
 
-
 AntennaDemodDecodeDetailsTypeDef = TypedDict(
     "AntennaDemodDecodeDetailsTypeDef",
     {
         "outputNode": str,
     },
     total=False,
 )
 
+DecodeConfigOutputTypeDef = TypedDict(
+    "DecodeConfigOutputTypeDef",
+    {
+        "unvalidatedJSON": str,
+    },
+)
+
+DemodulationConfigOutputTypeDef = TypedDict(
+    "DemodulationConfigOutputTypeDef",
+    {
+        "unvalidatedJSON": str,
+    },
+)
+
 DecodeConfigTypeDef = TypedDict(
     "DecodeConfigTypeDef",
     {
         "unvalidatedJSON": str,
     },
 )
 
 DemodulationConfigTypeDef = TypedDict(
     "DemodulationConfigTypeDef",
     {
         "unvalidatedJSON": str,
     },
 )
 
+EirpOutputTypeDef = TypedDict(
+    "EirpOutputTypeDef",
+    {
+        "units": Literal["dBW"],
+        "value": float,
+    },
+)
+
 EirpTypeDef = TypedDict(
     "EirpTypeDef",
     {
         "units": Literal["dBW"],
         "value": float,
     },
 )
@@ -245,21 +290,19 @@
         "bytesReceived": int,
         "bytesSent": int,
         "packetsDropped": int,
     },
     total=False,
 )
 
-
 class ComponentStatusDataTypeDef(
     _RequiredComponentStatusDataTypeDef, _OptionalComponentStatusDataTypeDef
 ):
     pass
 
-
 S3RecordingDetailsTypeDef = TypedDict(
     "S3RecordingDetailsTypeDef",
     {
         "bucketArn": str,
         "keyTemplate": str,
     },
     total=False,
@@ -282,35 +325,87 @@
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "name": str,
     },
     total=False,
 )
 
+_RequiredDataflowEndpointConfigOutputTypeDef = TypedDict(
+    "_RequiredDataflowEndpointConfigOutputTypeDef",
+    {
+        "dataflowEndpointName": str,
+    },
+)
+_OptionalDataflowEndpointConfigOutputTypeDef = TypedDict(
+    "_OptionalDataflowEndpointConfigOutputTypeDef",
+    {
+        "dataflowEndpointRegion": str,
+    },
+    total=False,
+)
+
+class DataflowEndpointConfigOutputTypeDef(
+    _RequiredDataflowEndpointConfigOutputTypeDef, _OptionalDataflowEndpointConfigOutputTypeDef
+):
+    pass
+
+_RequiredS3RecordingConfigOutputTypeDef = TypedDict(
+    "_RequiredS3RecordingConfigOutputTypeDef",
+    {
+        "bucketArn": str,
+        "roleArn": str,
+    },
+)
+_OptionalS3RecordingConfigOutputTypeDef = TypedDict(
+    "_OptionalS3RecordingConfigOutputTypeDef",
+    {
+        "prefix": str,
+    },
+    total=False,
+)
+
+class S3RecordingConfigOutputTypeDef(
+    _RequiredS3RecordingConfigOutputTypeDef, _OptionalS3RecordingConfigOutputTypeDef
+):
+    pass
+
+TrackingConfigOutputTypeDef = TypedDict(
+    "TrackingConfigOutputTypeDef",
+    {
+        "autotrack": CriticalityType,
+    },
+)
+
+UplinkEchoConfigOutputTypeDef = TypedDict(
+    "UplinkEchoConfigOutputTypeDef",
+    {
+        "antennaUplinkConfigArn": str,
+        "enabled": bool,
+    },
+)
+
 _RequiredDataflowEndpointConfigTypeDef = TypedDict(
     "_RequiredDataflowEndpointConfigTypeDef",
     {
         "dataflowEndpointName": str,
     },
 )
 _OptionalDataflowEndpointConfigTypeDef = TypedDict(
     "_OptionalDataflowEndpointConfigTypeDef",
     {
         "dataflowEndpointRegion": str,
     },
     total=False,
 )
 
-
 class DataflowEndpointConfigTypeDef(
     _RequiredDataflowEndpointConfigTypeDef, _OptionalDataflowEndpointConfigTypeDef
 ):
     pass
 
-
 _RequiredS3RecordingConfigTypeDef = TypedDict(
     "_RequiredS3RecordingConfigTypeDef",
     {
         "bucketArn": str,
         "roleArn": str,
     },
 )
@@ -318,21 +413,19 @@
     "_OptionalS3RecordingConfigTypeDef",
     {
         "prefix": str,
     },
     total=False,
 )
 
-
 class S3RecordingConfigTypeDef(
     _RequiredS3RecordingConfigTypeDef, _OptionalS3RecordingConfigTypeDef
 ):
     pass
 
-
 TrackingConfigTypeDef = TypedDict(
     "TrackingConfigTypeDef",
     {
         "autotrack": CriticalityType,
     },
 )
 
@@ -340,14 +433,22 @@
     "UplinkEchoConfigTypeDef",
     {
         "antennaUplinkConfigArn": str,
         "enabled": bool,
     },
 )
 
+SocketAddressOutputTypeDef = TypedDict(
+    "SocketAddressOutputTypeDef",
+    {
+        "name": str,
+        "port": int,
+    },
+)
+
 SocketAddressTypeDef = TypedDict(
     "SocketAddressTypeDef",
     {
         "name": str,
         "port": int,
     },
 )
@@ -451,25 +552,34 @@
     {
         "capabilityArns": Sequence[str],
         "privateIpAddresses": Sequence[str],
         "publicIpAddresses": Sequence[str],
     },
 )
 
+SecurityDetailsOutputTypeDef = TypedDict(
+    "SecurityDetailsOutputTypeDef",
+    {
+        "roleArn": str,
+        "securityGroupIds": List[str],
+        "subnetIds": List[str],
+    },
+)
+
 SecurityDetailsTypeDef = TypedDict(
     "SecurityDetailsTypeDef",
     {
         "roleArn": str,
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
     },
 )
 
-S3ObjectTypeDef = TypedDict(
-    "S3ObjectTypeDef",
+S3ObjectOutputTypeDef = TypedDict(
+    "S3ObjectOutputTypeDef",
     {
         "bucket": str,
         "key": str,
         "version": str,
     },
     total=False,
 )
@@ -494,29 +604,43 @@
         "ephemerisId": str,
         "epoch": datetime,
         "name": str,
     },
     total=False,
 )
 
-
 class EphemerisMetaDataTypeDef(
     _RequiredEphemerisMetaDataTypeDef, _OptionalEphemerisMetaDataTypeDef
 ):
     pass
 
+FrequencyBandwidthOutputTypeDef = TypedDict(
+    "FrequencyBandwidthOutputTypeDef",
+    {
+        "units": BandwidthUnitsType,
+        "value": float,
+    },
+)
 
 FrequencyBandwidthTypeDef = TypedDict(
     "FrequencyBandwidthTypeDef",
     {
         "units": BandwidthUnitsType,
         "value": float,
     },
 )
 
+FrequencyOutputTypeDef = TypedDict(
+    "FrequencyOutputTypeDef",
+    {
+        "units": FrequencyUnitsType,
+        "value": float,
+    },
+)
+
 FrequencyTypeDef = TypedDict(
     "FrequencyTypeDef",
     {
         "units": FrequencyUnitsType,
         "value": float,
     },
 )
@@ -575,14 +699,23 @@
 GetMissionProfileRequestRequestTypeDef = TypedDict(
     "GetMissionProfileRequestRequestTypeDef",
     {
         "missionProfileId": str,
     },
 )
 
+KmsKeyOutputTypeDef = TypedDict(
+    "KmsKeyOutputTypeDef",
+    {
+        "kmsAliasArn": str,
+        "kmsKeyArn": str,
+    },
+    total=False,
+)
+
 GetSatelliteRequestRequestTypeDef = TypedDict(
     "GetSatelliteRequestRequestTypeDef",
     {
         "satelliteId": str,
     },
 )
 
@@ -592,14 +725,22 @@
         "groundStationId": str,
         "groundStationName": str,
         "region": str,
     },
     total=False,
 )
 
+IntegerRangeOutputTypeDef = TypedDict(
+    "IntegerRangeOutputTypeDef",
+    {
+        "maximum": int,
+        "minimum": int,
+    },
+)
+
 IntegerRangeTypeDef = TypedDict(
     "IntegerRangeTypeDef",
     {
         "maximum": int,
         "minimum": int,
     },
 )
@@ -636,22 +777,20 @@
         "missionProfileArn": str,
         "satelliteArn": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListContactsRequestListContactsPaginateTypeDef(
     _RequiredListContactsRequestListContactsPaginateTypeDef,
     _OptionalListContactsRequestListContactsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListContactsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactsRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "startTime": Union[datetime, str],
         "statusList": Sequence[ContactStatusType],
     },
@@ -664,21 +803,19 @@
         "missionProfileArn": str,
         "nextToken": str,
         "satelliteArn": str,
     },
     total=False,
 )
 
-
 class ListContactsRequestRequestTypeDef(
     _RequiredListContactsRequestRequestTypeDef, _OptionalListContactsRequestRequestTypeDef
 ):
     pass
 
-
 ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef = TypedDict(
     "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -705,22 +842,20 @@
     {
         "statusList": Sequence[EphemerisStatusType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListEphemeridesRequestListEphemeridesPaginateTypeDef(
     _RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef,
     _OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListEphemeridesRequestRequestTypeDef = TypedDict(
     "_RequiredListEphemeridesRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "satelliteId": str,
         "startTime": Union[datetime, str],
     },
@@ -731,21 +866,19 @@
         "maxResults": int,
         "nextToken": str,
         "statusList": Sequence[EphemerisStatusType],
     },
     total=False,
 )
 
-
 class ListEphemeridesRequestRequestTypeDef(
     _RequiredListEphemeridesRequestRequestTypeDef, _OptionalListEphemeridesRequestRequestTypeDef
 ):
     pass
 
-
 ListGroundStationsRequestListGroundStationsPaginateTypeDef = TypedDict(
     "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
     {
         "satelliteId": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -825,14 +958,24 @@
     "MissionProfileIdResponseTypeDef",
     {
         "missionProfileId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+S3ObjectTypeDef = TypedDict(
+    "S3ObjectTypeDef",
+    {
+        "bucket": str,
+        "key": str,
+        "version": str,
+    },
+    total=False,
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -861,21 +1004,19 @@
     "_OptionalReserveContactRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class ReserveContactRequestRequestTypeDef(
     _RequiredReserveContactRequestRequestTypeDef, _OptionalReserveContactRequestRequestTypeDef
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
@@ -927,21 +1068,19 @@
     {
         "name": str,
         "priority": int,
     },
     total=False,
 )
 
-
 class UpdateEphemerisRequestRequestTypeDef(
     _RequiredUpdateEphemerisRequestRequestTypeDef, _OptionalUpdateEphemerisRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredAgentDetailsTypeDef = TypedDict(
     "_RequiredAgentDetailsTypeDef",
     {
         "agentVersion": str,
         "componentVersions": Sequence[ComponentVersionTypeDef],
         "instanceId": str,
         "instanceType": str,
@@ -952,19 +1091,17 @@
     {
         "agentCpuCores": Sequence[int],
         "reservedCpuCores": Sequence[int],
     },
     total=False,
 )
 
-
 class AgentDetailsTypeDef(_RequiredAgentDetailsTypeDef, _OptionalAgentDetailsTypeDef):
     pass
 
-
 UpdateAgentStatusRequestRequestTypeDef = TypedDict(
     "UpdateAgentStatusRequestRequestTypeDef",
     {
         "agentId": str,
         "aggregateStatus": AggregateStatusTypeDef,
         "componentStatuses": Sequence[ComponentStatusDataTypeDef],
         "taskId": str,
@@ -976,35 +1113,63 @@
     {
         "configList": List[ConfigListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredConnectionDetailsOutputTypeDef = TypedDict(
+    "_RequiredConnectionDetailsOutputTypeDef",
+    {
+        "socketAddress": SocketAddressOutputTypeDef,
+    },
+)
+_OptionalConnectionDetailsOutputTypeDef = TypedDict(
+    "_OptionalConnectionDetailsOutputTypeDef",
+    {
+        "mtu": int,
+    },
+    total=False,
+)
+
+class ConnectionDetailsOutputTypeDef(
+    _RequiredConnectionDetailsOutputTypeDef, _OptionalConnectionDetailsOutputTypeDef
+):
+    pass
+
+DataflowEndpointOutputTypeDef = TypedDict(
+    "DataflowEndpointOutputTypeDef",
+    {
+        "address": SocketAddressOutputTypeDef,
+        "mtu": int,
+        "name": str,
+        "status": EndpointStatusType,
+    },
+    total=False,
+)
+
 _RequiredConnectionDetailsTypeDef = TypedDict(
     "_RequiredConnectionDetailsTypeDef",
     {
         "socketAddress": SocketAddressTypeDef,
     },
 )
 _OptionalConnectionDetailsTypeDef = TypedDict(
     "_OptionalConnectionDetailsTypeDef",
     {
         "mtu": int,
     },
     total=False,
 )
 
-
 class ConnectionDetailsTypeDef(
     _RequiredConnectionDetailsTypeDef, _OptionalConnectionDetailsTypeDef
 ):
     pass
 
-
 DataflowEndpointTypeDef = TypedDict(
     "DataflowEndpointTypeDef",
     {
         "address": SocketAddressTypeDef,
         "mtu": int,
         "name": str,
         "status": EndpointStatusType,
@@ -1049,41 +1214,20 @@
         "streamsKmsKey": KmsKeyTypeDef,
         "streamsKmsRole": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateMissionProfileRequestRequestTypeDef(
     _RequiredCreateMissionProfileRequestRequestTypeDef,
     _OptionalCreateMissionProfileRequestRequestTypeDef,
 ):
     pass
 
-
-GetMissionProfileResponseTypeDef = TypedDict(
-    "GetMissionProfileResponseTypeDef",
-    {
-        "contactPostPassDurationSeconds": int,
-        "contactPrePassDurationSeconds": int,
-        "dataflowEdges": List[List[str]],
-        "minimumViableContactDurationSeconds": int,
-        "missionProfileArn": str,
-        "missionProfileId": str,
-        "name": str,
-        "region": str,
-        "streamsKmsKey": KmsKeyTypeDef,
-        "streamsKmsRole": str,
-        "tags": Dict[str, str],
-        "trackingConfigArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateMissionProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMissionProfileRequestRequestTypeDef",
     {
         "missionProfileId": str,
     },
 )
 _OptionalUpdateMissionProfileRequestRequestTypeDef = TypedDict(
@@ -1097,22 +1241,20 @@
         "streamsKmsKey": KmsKeyTypeDef,
         "streamsKmsRole": str,
         "trackingConfigArn": str,
     },
     total=False,
 )
 
-
 class UpdateMissionProfileRequestRequestTypeDef(
     _RequiredUpdateMissionProfileRequestRequestTypeDef,
     _OptionalUpdateMissionProfileRequestRequestTypeDef,
 ):
     pass
 
-
 ListDataflowEndpointGroupsResponseTypeDef = TypedDict(
     "ListDataflowEndpointGroupsResponseTypeDef",
     {
         "dataflowEndpointGroupList": List[DataflowEndpointListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1128,54 +1270,43 @@
     "_OptionalDescribeContactRequestContactScheduledWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeContactRequestContactScheduledWaitTypeDef(
     _RequiredDescribeContactRequestContactScheduledWaitTypeDef,
     _OptionalDescribeContactRequestContactScheduledWaitTypeDef,
 ):
     pass
 
-
 EphemerisDescriptionTypeDef = TypedDict(
     "EphemerisDescriptionTypeDef",
     {
         "ephemerisData": str,
-        "sourceS3Object": S3ObjectTypeDef,
+        "sourceS3Object": S3ObjectOutputTypeDef,
     },
     total=False,
 )
 
 EphemerisItemTypeDef = TypedDict(
     "EphemerisItemTypeDef",
     {
         "creationTime": datetime,
         "enabled": bool,
         "ephemerisId": str,
         "name": str,
         "priority": int,
-        "sourceS3Object": S3ObjectTypeDef,
+        "sourceS3Object": S3ObjectOutputTypeDef,
         "status": EphemerisStatusType,
     },
     total=False,
 )
 
-OEMEphemerisTypeDef = TypedDict(
-    "OEMEphemerisTypeDef",
-    {
-        "oemData": str,
-        "s3Object": S3ObjectTypeDef,
-    },
-    total=False,
-)
-
 GetSatelliteResponseTypeDef = TypedDict(
     "GetSatelliteResponseTypeDef",
     {
         "currentEphemeris": EphemerisMetaDataTypeDef,
         "groundStations": List[str],
         "noradSatelliteID": int,
         "satelliteArn": str,
@@ -1192,14 +1323,53 @@
         "noradSatelliteID": int,
         "satelliteArn": str,
         "satelliteId": str,
     },
     total=False,
 )
 
+_RequiredSpectrumConfigOutputTypeDef = TypedDict(
+    "_RequiredSpectrumConfigOutputTypeDef",
+    {
+        "bandwidth": FrequencyBandwidthOutputTypeDef,
+        "centerFrequency": FrequencyOutputTypeDef,
+    },
+)
+_OptionalSpectrumConfigOutputTypeDef = TypedDict(
+    "_OptionalSpectrumConfigOutputTypeDef",
+    {
+        "polarization": PolarizationType,
+    },
+    total=False,
+)
+
+class SpectrumConfigOutputTypeDef(
+    _RequiredSpectrumConfigOutputTypeDef, _OptionalSpectrumConfigOutputTypeDef
+):
+    pass
+
+_RequiredUplinkSpectrumConfigOutputTypeDef = TypedDict(
+    "_RequiredUplinkSpectrumConfigOutputTypeDef",
+    {
+        "centerFrequency": FrequencyOutputTypeDef,
+    },
+)
+_OptionalUplinkSpectrumConfigOutputTypeDef = TypedDict(
+    "_OptionalUplinkSpectrumConfigOutputTypeDef",
+    {
+        "polarization": PolarizationType,
+    },
+    total=False,
+)
+
+class UplinkSpectrumConfigOutputTypeDef(
+    _RequiredUplinkSpectrumConfigOutputTypeDef, _OptionalUplinkSpectrumConfigOutputTypeDef
+):
+    pass
+
 _RequiredSpectrumConfigTypeDef = TypedDict(
     "_RequiredSpectrumConfigTypeDef",
     {
         "bandwidth": FrequencyBandwidthTypeDef,
         "centerFrequency": FrequencyTypeDef,
     },
 )
@@ -1207,49 +1377,72 @@
     "_OptionalSpectrumConfigTypeDef",
     {
         "polarization": PolarizationType,
     },
     total=False,
 )
 
-
 class SpectrumConfigTypeDef(_RequiredSpectrumConfigTypeDef, _OptionalSpectrumConfigTypeDef):
     pass
 
-
 _RequiredUplinkSpectrumConfigTypeDef = TypedDict(
     "_RequiredUplinkSpectrumConfigTypeDef",
     {
         "centerFrequency": FrequencyTypeDef,
     },
 )
 _OptionalUplinkSpectrumConfigTypeDef = TypedDict(
     "_OptionalUplinkSpectrumConfigTypeDef",
     {
         "polarization": PolarizationType,
     },
     total=False,
 )
 
-
 class UplinkSpectrumConfigTypeDef(
     _RequiredUplinkSpectrumConfigTypeDef, _OptionalUplinkSpectrumConfigTypeDef
 ):
     pass
 
+GetMissionProfileResponseTypeDef = TypedDict(
+    "GetMissionProfileResponseTypeDef",
+    {
+        "contactPostPassDurationSeconds": int,
+        "contactPrePassDurationSeconds": int,
+        "dataflowEdges": List[List[str]],
+        "minimumViableContactDurationSeconds": int,
+        "missionProfileArn": str,
+        "missionProfileId": str,
+        "name": str,
+        "region": str,
+        "streamsKmsKey": KmsKeyOutputTypeDef,
+        "streamsKmsRole": str,
+        "tags": Dict[str, str],
+        "trackingConfigArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 ListGroundStationsResponseTypeDef = TypedDict(
     "ListGroundStationsResponseTypeDef",
     {
         "groundStationList": List[GroundStationDataTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RangedSocketAddressOutputTypeDef = TypedDict(
+    "RangedSocketAddressOutputTypeDef",
+    {
+        "name": str,
+        "portRange": IntegerRangeOutputTypeDef,
+    },
+)
+
 RangedSocketAddressTypeDef = TypedDict(
     "RangedSocketAddressTypeDef",
     {
         "name": str,
         "portRange": IntegerRangeTypeDef,
     },
 )
@@ -1259,14 +1452,23 @@
     {
         "missionProfileList": List[MissionProfileListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+OEMEphemerisTypeDef = TypedDict(
+    "OEMEphemerisTypeDef",
+    {
+        "oemData": str,
+        "s3Object": S3ObjectTypeDef,
+    },
+    total=False,
+)
+
 TLEDataTypeDef = TypedDict(
     "TLEDataTypeDef",
     {
         "tleLine1": str,
         "tleLine2": str,
         "validTimeRange": TimeRangeTypeDef,
     },
@@ -1312,14 +1514,50 @@
     {
         "nextToken": str,
         "satellites": List[SatelliteListItemTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AntennaDownlinkConfigOutputTypeDef = TypedDict(
+    "AntennaDownlinkConfigOutputTypeDef",
+    {
+        "spectrumConfig": SpectrumConfigOutputTypeDef,
+    },
+)
+
+AntennaDownlinkDemodDecodeConfigOutputTypeDef = TypedDict(
+    "AntennaDownlinkDemodDecodeConfigOutputTypeDef",
+    {
+        "decodeConfig": DecodeConfigOutputTypeDef,
+        "demodulationConfig": DemodulationConfigOutputTypeDef,
+        "spectrumConfig": SpectrumConfigOutputTypeDef,
+    },
+)
+
+_RequiredAntennaUplinkConfigOutputTypeDef = TypedDict(
+    "_RequiredAntennaUplinkConfigOutputTypeDef",
+    {
+        "spectrumConfig": UplinkSpectrumConfigOutputTypeDef,
+        "targetEirp": EirpOutputTypeDef,
+    },
+)
+_OptionalAntennaUplinkConfigOutputTypeDef = TypedDict(
+    "_OptionalAntennaUplinkConfigOutputTypeDef",
+    {
+        "transmitDisabled": bool,
+    },
+    total=False,
+)
+
+class AntennaUplinkConfigOutputTypeDef(
+    _RequiredAntennaUplinkConfigOutputTypeDef, _OptionalAntennaUplinkConfigOutputTypeDef
+):
+    pass
+
 AntennaDownlinkConfigTypeDef = TypedDict(
     "AntennaDownlinkConfigTypeDef",
     {
         "spectrumConfig": SpectrumConfigTypeDef,
     },
 )
 
@@ -1343,20 +1581,37 @@
     "_OptionalAntennaUplinkConfigTypeDef",
     {
         "transmitDisabled": bool,
     },
     total=False,
 )
 
-
 class AntennaUplinkConfigTypeDef(
     _RequiredAntennaUplinkConfigTypeDef, _OptionalAntennaUplinkConfigTypeDef
 ):
     pass
 
+_RequiredRangedConnectionDetailsOutputTypeDef = TypedDict(
+    "_RequiredRangedConnectionDetailsOutputTypeDef",
+    {
+        "socketAddress": RangedSocketAddressOutputTypeDef,
+    },
+)
+_OptionalRangedConnectionDetailsOutputTypeDef = TypedDict(
+    "_OptionalRangedConnectionDetailsOutputTypeDef",
+    {
+        "mtu": int,
+    },
+    total=False,
+)
+
+class RangedConnectionDetailsOutputTypeDef(
+    _RequiredRangedConnectionDetailsOutputTypeDef, _OptionalRangedConnectionDetailsOutputTypeDef
+):
+    pass
 
 _RequiredRangedConnectionDetailsTypeDef = TypedDict(
     "_RequiredRangedConnectionDetailsTypeDef",
     {
         "socketAddress": RangedSocketAddressTypeDef,
     },
 )
@@ -1364,21 +1619,19 @@
     "_OptionalRangedConnectionDetailsTypeDef",
     {
         "mtu": int,
     },
     total=False,
 )
 
-
 class RangedConnectionDetailsTypeDef(
     _RequiredRangedConnectionDetailsTypeDef, _OptionalRangedConnectionDetailsTypeDef
 ):
     pass
 
-
 TLEEphemerisTypeDef = TypedDict(
     "TLEEphemerisTypeDef",
     {
         "s3Object": S3ObjectTypeDef,
         "tleData": Sequence[TLEDataTypeDef],
     },
     total=False,
@@ -1397,28 +1650,65 @@
         "status": EphemerisStatusType,
         "suppliedData": EphemerisTypeDescriptionTypeDef,
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ConfigTypeDataOutputTypeDef = TypedDict(
+    "ConfigTypeDataOutputTypeDef",
+    {
+        "antennaDownlinkConfig": AntennaDownlinkConfigOutputTypeDef,
+        "antennaDownlinkDemodDecodeConfig": AntennaDownlinkDemodDecodeConfigOutputTypeDef,
+        "antennaUplinkConfig": AntennaUplinkConfigOutputTypeDef,
+        "dataflowEndpointConfig": DataflowEndpointConfigOutputTypeDef,
+        "s3RecordingConfig": S3RecordingConfigOutputTypeDef,
+        "trackingConfig": TrackingConfigOutputTypeDef,
+        "uplinkEchoConfig": UplinkEchoConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 ConfigTypeDataTypeDef = TypedDict(
     "ConfigTypeDataTypeDef",
     {
         "antennaDownlinkConfig": AntennaDownlinkConfigTypeDef,
         "antennaDownlinkDemodDecodeConfig": AntennaDownlinkDemodDecodeConfigTypeDef,
         "antennaUplinkConfig": AntennaUplinkConfigTypeDef,
         "dataflowEndpointConfig": DataflowEndpointConfigTypeDef,
         "s3RecordingConfig": S3RecordingConfigTypeDef,
         "trackingConfig": TrackingConfigTypeDef,
         "uplinkEchoConfig": UplinkEchoConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredAwsGroundStationAgentEndpointOutputTypeDef = TypedDict(
+    "_RequiredAwsGroundStationAgentEndpointOutputTypeDef",
+    {
+        "egressAddress": ConnectionDetailsOutputTypeDef,
+        "ingressAddress": RangedConnectionDetailsOutputTypeDef,
+        "name": str,
+    },
+)
+_OptionalAwsGroundStationAgentEndpointOutputTypeDef = TypedDict(
+    "_OptionalAwsGroundStationAgentEndpointOutputTypeDef",
+    {
+        "agentStatus": AgentStatusType,
+        "auditResults": AuditResultsType,
+    },
+    total=False,
+)
+
+class AwsGroundStationAgentEndpointOutputTypeDef(
+    _RequiredAwsGroundStationAgentEndpointOutputTypeDef,
+    _OptionalAwsGroundStationAgentEndpointOutputTypeDef,
+):
+    pass
+
 _RequiredAwsGroundStationAgentEndpointTypeDef = TypedDict(
     "_RequiredAwsGroundStationAgentEndpointTypeDef",
     {
         "egressAddress": ConnectionDetailsTypeDef,
         "ingressAddress": RangedConnectionDetailsTypeDef,
         "name": str,
     },
@@ -1428,30 +1718,41 @@
     {
         "agentStatus": AgentStatusType,
         "auditResults": AuditResultsType,
     },
     total=False,
 )
 
-
 class AwsGroundStationAgentEndpointTypeDef(
     _RequiredAwsGroundStationAgentEndpointTypeDef, _OptionalAwsGroundStationAgentEndpointTypeDef
 ):
     pass
 
-
 EphemerisDataTypeDef = TypedDict(
     "EphemerisDataTypeDef",
     {
         "oem": OEMEphemerisTypeDef,
         "tle": TLEEphemerisTypeDef,
     },
     total=False,
 )
 
+GetConfigResponseTypeDef = TypedDict(
+    "GetConfigResponseTypeDef",
+    {
+        "configArn": str,
+        "configData": ConfigTypeDataOutputTypeDef,
+        "configId": str,
+        "configType": ConfigCapabilityTypeType,
+        "name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigRequestRequestTypeDef",
     {
         "configData": ConfigTypeDataTypeDef,
         "name": str,
     },
 )
@@ -1459,42 +1760,39 @@
     "_OptionalCreateConfigRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateConfigRequestRequestTypeDef(
     _RequiredCreateConfigRequestRequestTypeDef, _OptionalCreateConfigRequestRequestTypeDef
 ):
     pass
 
-
-GetConfigResponseTypeDef = TypedDict(
-    "GetConfigResponseTypeDef",
+UpdateConfigRequestRequestTypeDef = TypedDict(
+    "UpdateConfigRequestRequestTypeDef",
     {
-        "configArn": str,
         "configData": ConfigTypeDataTypeDef,
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateConfigRequestRequestTypeDef = TypedDict(
-    "UpdateConfigRequestRequestTypeDef",
+EndpointDetailsOutputTypeDef = TypedDict(
+    "EndpointDetailsOutputTypeDef",
     {
-        "configData": ConfigTypeDataTypeDef,
-        "configId": str,
-        "configType": ConfigCapabilityTypeType,
-        "name": str,
+        "awsGroundStationAgentEndpoint": AwsGroundStationAgentEndpointOutputTypeDef,
+        "endpoint": DataflowEndpointOutputTypeDef,
+        "healthReasons": List[CapabilityHealthReasonType],
+        "healthStatus": CapabilityHealthType,
+        "securityDetails": SecurityDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 EndpointDetailsTypeDef = TypedDict(
     "EndpointDetailsTypeDef",
     {
         "awsGroundStationAgentEndpoint": AwsGroundStationAgentEndpointTypeDef,
         "endpoint": DataflowEndpointTypeDef,
@@ -1521,31 +1819,42 @@
         "kmsKeyArn": str,
         "priority": int,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateEphemerisRequestRequestTypeDef(
     _RequiredCreateEphemerisRequestRequestTypeDef, _OptionalCreateEphemerisRequestRequestTypeDef
 ):
     pass
 
-
 ConfigDetailsTypeDef = TypedDict(
     "ConfigDetailsTypeDef",
     {
         "antennaDemodDecodeDetails": AntennaDemodDecodeDetailsTypeDef,
-        "endpointDetails": EndpointDetailsTypeDef,
+        "endpointDetails": EndpointDetailsOutputTypeDef,
         "s3RecordingDetails": S3RecordingDetailsTypeDef,
     },
     total=False,
 )
 
+GetDataflowEndpointGroupResponseTypeDef = TypedDict(
+    "GetDataflowEndpointGroupResponseTypeDef",
+    {
+        "contactPostPassDurationSeconds": int,
+        "contactPrePassDurationSeconds": int,
+        "dataflowEndpointGroupArn": str,
+        "dataflowEndpointGroupId": str,
+        "endpointsDetails": List[EndpointDetailsOutputTypeDef],
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef",
     {
         "endpointDetails": Sequence[EndpointDetailsTypeDef],
     },
 )
 _OptionalCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
@@ -1554,35 +1863,20 @@
         "contactPostPassDurationSeconds": int,
         "contactPrePassDurationSeconds": int,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateDataflowEndpointGroupRequestRequestTypeDef(
     _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef,
     _OptionalCreateDataflowEndpointGroupRequestRequestTypeDef,
 ):
     pass
 
-
-GetDataflowEndpointGroupResponseTypeDef = TypedDict(
-    "GetDataflowEndpointGroupResponseTypeDef",
-    {
-        "contactPostPassDurationSeconds": int,
-        "contactPrePassDurationSeconds": int,
-        "dataflowEndpointGroupArn": str,
-        "dataflowEndpointGroupId": str,
-        "endpointsDetails": List[EndpointDetailsTypeDef],
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "configDetails": ConfigDetailsTypeDef,
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "dataflowDestinationRegion": str,
```

### Comparing `mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/type_defs.pyi` & `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/type_defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,59 +38,73 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ComponentVersionTypeDef",
     "AggregateStatusTypeDef",
     "AntennaDemodDecodeDetailsTypeDef",
+    "DecodeConfigOutputTypeDef",
+    "DemodulationConfigOutputTypeDef",
     "DecodeConfigTypeDef",
     "DemodulationConfigTypeDef",
+    "EirpOutputTypeDef",
     "EirpTypeDef",
     "CancelContactRequestRequestTypeDef",
     "ComponentStatusDataTypeDef",
     "S3RecordingDetailsTypeDef",
     "ConfigIdResponseTypeDef",
     "ConfigListItemTypeDef",
+    "DataflowEndpointConfigOutputTypeDef",
+    "S3RecordingConfigOutputTypeDef",
+    "TrackingConfigOutputTypeDef",
+    "UplinkEchoConfigOutputTypeDef",
     "DataflowEndpointConfigTypeDef",
     "S3RecordingConfigTypeDef",
     "TrackingConfigTypeDef",
     "UplinkEchoConfigTypeDef",
+    "SocketAddressOutputTypeDef",
     "SocketAddressTypeDef",
     "ElevationTypeDef",
     "ContactIdResponseTypeDef",
     "KmsKeyTypeDef",
     "DataflowEndpointGroupIdResponseTypeDef",
     "DataflowEndpointListItemTypeDef",
     "DeleteConfigRequestRequestTypeDef",
     "DeleteDataflowEndpointGroupRequestRequestTypeDef",
     "DeleteEphemerisRequestRequestTypeDef",
     "DeleteMissionProfileRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeContactRequestRequestTypeDef",
     "DescribeEphemerisRequestRequestTypeDef",
     "DiscoveryDataTypeDef",
+    "SecurityDetailsOutputTypeDef",
     "SecurityDetailsTypeDef",
-    "S3ObjectTypeDef",
+    "S3ObjectOutputTypeDef",
     "EphemerisIdResponseTypeDef",
     "EphemerisMetaDataTypeDef",
+    "FrequencyBandwidthOutputTypeDef",
     "FrequencyBandwidthTypeDef",
+    "FrequencyOutputTypeDef",
     "FrequencyTypeDef",
     "GetAgentConfigurationRequestRequestTypeDef",
     "GetAgentConfigurationResponseTypeDef",
     "GetConfigRequestRequestTypeDef",
     "GetDataflowEndpointGroupRequestRequestTypeDef",
     "GetMinuteUsageRequestRequestTypeDef",
     "GetMinuteUsageResponseTypeDef",
     "GetMissionProfileRequestRequestTypeDef",
+    "KmsKeyOutputTypeDef",
     "GetSatelliteRequestRequestTypeDef",
     "GroundStationDataTypeDef",
+    "IntegerRangeOutputTypeDef",
     "IntegerRangeTypeDef",
     "ListConfigsRequestListConfigsPaginateTypeDef",
     "ListConfigsRequestRequestTypeDef",
     "ListContactsRequestListContactsPaginateTypeDef",
     "ListContactsRequestRequestTypeDef",
     "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
     "ListDataflowEndpointGroupsRequestRequestTypeDef",
@@ -102,67 +116,80 @@
     "ListMissionProfilesRequestRequestTypeDef",
     "MissionProfileListItemTypeDef",
     "ListSatellitesRequestListSatellitesPaginateTypeDef",
     "ListSatellitesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "MissionProfileIdResponseTypeDef",
+    "S3ObjectTypeDef",
     "PaginatorConfigTypeDef",
     "RegisterAgentResponseTypeDef",
     "ReserveContactRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TimeRangeTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAgentStatusResponseTypeDef",
     "UpdateEphemerisRequestRequestTypeDef",
     "AgentDetailsTypeDef",
     "UpdateAgentStatusRequestRequestTypeDef",
     "ListConfigsResponseTypeDef",
+    "ConnectionDetailsOutputTypeDef",
+    "DataflowEndpointOutputTypeDef",
     "ConnectionDetailsTypeDef",
     "DataflowEndpointTypeDef",
     "ContactDataTypeDef",
     "CreateMissionProfileRequestRequestTypeDef",
-    "GetMissionProfileResponseTypeDef",
     "UpdateMissionProfileRequestRequestTypeDef",
     "ListDataflowEndpointGroupsResponseTypeDef",
     "DescribeContactRequestContactScheduledWaitTypeDef",
     "EphemerisDescriptionTypeDef",
     "EphemerisItemTypeDef",
-    "OEMEphemerisTypeDef",
     "GetSatelliteResponseTypeDef",
     "SatelliteListItemTypeDef",
+    "SpectrumConfigOutputTypeDef",
+    "UplinkSpectrumConfigOutputTypeDef",
     "SpectrumConfigTypeDef",
     "UplinkSpectrumConfigTypeDef",
+    "GetMissionProfileResponseTypeDef",
     "ListGroundStationsResponseTypeDef",
+    "RangedSocketAddressOutputTypeDef",
     "RangedSocketAddressTypeDef",
     "ListMissionProfilesResponseTypeDef",
+    "OEMEphemerisTypeDef",
     "TLEDataTypeDef",
     "RegisterAgentRequestRequestTypeDef",
     "ListContactsResponseTypeDef",
     "EphemerisTypeDescriptionTypeDef",
     "ListEphemeridesResponseTypeDef",
     "ListSatellitesResponseTypeDef",
+    "AntennaDownlinkConfigOutputTypeDef",
+    "AntennaDownlinkDemodDecodeConfigOutputTypeDef",
+    "AntennaUplinkConfigOutputTypeDef",
     "AntennaDownlinkConfigTypeDef",
     "AntennaDownlinkDemodDecodeConfigTypeDef",
     "AntennaUplinkConfigTypeDef",
+    "RangedConnectionDetailsOutputTypeDef",
     "RangedConnectionDetailsTypeDef",
     "TLEEphemerisTypeDef",
     "DescribeEphemerisResponseTypeDef",
+    "ConfigTypeDataOutputTypeDef",
     "ConfigTypeDataTypeDef",
+    "AwsGroundStationAgentEndpointOutputTypeDef",
     "AwsGroundStationAgentEndpointTypeDef",
     "EphemerisDataTypeDef",
-    "CreateConfigRequestRequestTypeDef",
     "GetConfigResponseTypeDef",
+    "CreateConfigRequestRequestTypeDef",
     "UpdateConfigRequestRequestTypeDef",
+    "EndpointDetailsOutputTypeDef",
     "EndpointDetailsTypeDef",
     "CreateEphemerisRequestRequestTypeDef",
     "ConfigDetailsTypeDef",
-    "CreateDataflowEndpointGroupRequestRequestTypeDef",
     "GetDataflowEndpointGroupResponseTypeDef",
+    "CreateDataflowEndpointGroupRequestRequestTypeDef",
     "DestinationTypeDef",
     "SourceTypeDef",
     "DataflowDetailTypeDef",
     "DescribeContactResponseTypeDef",
 )
 
 ComponentVersionTypeDef = TypedDict(
@@ -183,39 +210,63 @@
     "_OptionalAggregateStatusTypeDef",
     {
         "signatureMap": Mapping[str, bool],
     },
     total=False,
 )
 
+
 class AggregateStatusTypeDef(_RequiredAggregateStatusTypeDef, _OptionalAggregateStatusTypeDef):
     pass
 
+
 AntennaDemodDecodeDetailsTypeDef = TypedDict(
     "AntennaDemodDecodeDetailsTypeDef",
     {
         "outputNode": str,
     },
     total=False,
 )
 
+DecodeConfigOutputTypeDef = TypedDict(
+    "DecodeConfigOutputTypeDef",
+    {
+        "unvalidatedJSON": str,
+    },
+)
+
+DemodulationConfigOutputTypeDef = TypedDict(
+    "DemodulationConfigOutputTypeDef",
+    {
+        "unvalidatedJSON": str,
+    },
+)
+
 DecodeConfigTypeDef = TypedDict(
     "DecodeConfigTypeDef",
     {
         "unvalidatedJSON": str,
     },
 )
 
 DemodulationConfigTypeDef = TypedDict(
     "DemodulationConfigTypeDef",
     {
         "unvalidatedJSON": str,
     },
 )
 
+EirpOutputTypeDef = TypedDict(
+    "EirpOutputTypeDef",
+    {
+        "units": Literal["dBW"],
+        "value": float,
+    },
+)
+
 EirpTypeDef = TypedDict(
     "EirpTypeDef",
     {
         "units": Literal["dBW"],
         "value": float,
     },
 )
@@ -242,19 +293,21 @@
         "bytesReceived": int,
         "bytesSent": int,
         "packetsDropped": int,
     },
     total=False,
 )
 
+
 class ComponentStatusDataTypeDef(
     _RequiredComponentStatusDataTypeDef, _OptionalComponentStatusDataTypeDef
 ):
     pass
 
+
 S3RecordingDetailsTypeDef = TypedDict(
     "S3RecordingDetailsTypeDef",
     {
         "bucketArn": str,
         "keyTemplate": str,
     },
     total=False,
@@ -277,33 +330,93 @@
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "name": str,
     },
     total=False,
 )
 
+_RequiredDataflowEndpointConfigOutputTypeDef = TypedDict(
+    "_RequiredDataflowEndpointConfigOutputTypeDef",
+    {
+        "dataflowEndpointName": str,
+    },
+)
+_OptionalDataflowEndpointConfigOutputTypeDef = TypedDict(
+    "_OptionalDataflowEndpointConfigOutputTypeDef",
+    {
+        "dataflowEndpointRegion": str,
+    },
+    total=False,
+)
+
+
+class DataflowEndpointConfigOutputTypeDef(
+    _RequiredDataflowEndpointConfigOutputTypeDef, _OptionalDataflowEndpointConfigOutputTypeDef
+):
+    pass
+
+
+_RequiredS3RecordingConfigOutputTypeDef = TypedDict(
+    "_RequiredS3RecordingConfigOutputTypeDef",
+    {
+        "bucketArn": str,
+        "roleArn": str,
+    },
+)
+_OptionalS3RecordingConfigOutputTypeDef = TypedDict(
+    "_OptionalS3RecordingConfigOutputTypeDef",
+    {
+        "prefix": str,
+    },
+    total=False,
+)
+
+
+class S3RecordingConfigOutputTypeDef(
+    _RequiredS3RecordingConfigOutputTypeDef, _OptionalS3RecordingConfigOutputTypeDef
+):
+    pass
+
+
+TrackingConfigOutputTypeDef = TypedDict(
+    "TrackingConfigOutputTypeDef",
+    {
+        "autotrack": CriticalityType,
+    },
+)
+
+UplinkEchoConfigOutputTypeDef = TypedDict(
+    "UplinkEchoConfigOutputTypeDef",
+    {
+        "antennaUplinkConfigArn": str,
+        "enabled": bool,
+    },
+)
+
 _RequiredDataflowEndpointConfigTypeDef = TypedDict(
     "_RequiredDataflowEndpointConfigTypeDef",
     {
         "dataflowEndpointName": str,
     },
 )
 _OptionalDataflowEndpointConfigTypeDef = TypedDict(
     "_OptionalDataflowEndpointConfigTypeDef",
     {
         "dataflowEndpointRegion": str,
     },
     total=False,
 )
 
+
 class DataflowEndpointConfigTypeDef(
     _RequiredDataflowEndpointConfigTypeDef, _OptionalDataflowEndpointConfigTypeDef
 ):
     pass
 
+
 _RequiredS3RecordingConfigTypeDef = TypedDict(
     "_RequiredS3RecordingConfigTypeDef",
     {
         "bucketArn": str,
         "roleArn": str,
     },
 )
@@ -311,19 +424,21 @@
     "_OptionalS3RecordingConfigTypeDef",
     {
         "prefix": str,
     },
     total=False,
 )
 
+
 class S3RecordingConfigTypeDef(
     _RequiredS3RecordingConfigTypeDef, _OptionalS3RecordingConfigTypeDef
 ):
     pass
 
+
 TrackingConfigTypeDef = TypedDict(
     "TrackingConfigTypeDef",
     {
         "autotrack": CriticalityType,
     },
 )
 
@@ -331,14 +446,22 @@
     "UplinkEchoConfigTypeDef",
     {
         "antennaUplinkConfigArn": str,
         "enabled": bool,
     },
 )
 
+SocketAddressOutputTypeDef = TypedDict(
+    "SocketAddressOutputTypeDef",
+    {
+        "name": str,
+        "port": int,
+    },
+)
+
 SocketAddressTypeDef = TypedDict(
     "SocketAddressTypeDef",
     {
         "name": str,
         "port": int,
     },
 )
@@ -442,25 +565,34 @@
     {
         "capabilityArns": Sequence[str],
         "privateIpAddresses": Sequence[str],
         "publicIpAddresses": Sequence[str],
     },
 )
 
+SecurityDetailsOutputTypeDef = TypedDict(
+    "SecurityDetailsOutputTypeDef",
+    {
+        "roleArn": str,
+        "securityGroupIds": List[str],
+        "subnetIds": List[str],
+    },
+)
+
 SecurityDetailsTypeDef = TypedDict(
     "SecurityDetailsTypeDef",
     {
         "roleArn": str,
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
     },
 )
 
-S3ObjectTypeDef = TypedDict(
-    "S3ObjectTypeDef",
+S3ObjectOutputTypeDef = TypedDict(
+    "S3ObjectOutputTypeDef",
     {
         "bucket": str,
         "key": str,
         "version": str,
     },
     total=False,
 )
@@ -485,27 +617,45 @@
         "ephemerisId": str,
         "epoch": datetime,
         "name": str,
     },
     total=False,
 )
 
+
 class EphemerisMetaDataTypeDef(
     _RequiredEphemerisMetaDataTypeDef, _OptionalEphemerisMetaDataTypeDef
 ):
     pass
 
+
+FrequencyBandwidthOutputTypeDef = TypedDict(
+    "FrequencyBandwidthOutputTypeDef",
+    {
+        "units": BandwidthUnitsType,
+        "value": float,
+    },
+)
+
 FrequencyBandwidthTypeDef = TypedDict(
     "FrequencyBandwidthTypeDef",
     {
         "units": BandwidthUnitsType,
         "value": float,
     },
 )
 
+FrequencyOutputTypeDef = TypedDict(
+    "FrequencyOutputTypeDef",
+    {
+        "units": FrequencyUnitsType,
+        "value": float,
+    },
+)
+
 FrequencyTypeDef = TypedDict(
     "FrequencyTypeDef",
     {
         "units": FrequencyUnitsType,
         "value": float,
     },
 )
@@ -564,14 +714,23 @@
 GetMissionProfileRequestRequestTypeDef = TypedDict(
     "GetMissionProfileRequestRequestTypeDef",
     {
         "missionProfileId": str,
     },
 )
 
+KmsKeyOutputTypeDef = TypedDict(
+    "KmsKeyOutputTypeDef",
+    {
+        "kmsAliasArn": str,
+        "kmsKeyArn": str,
+    },
+    total=False,
+)
+
 GetSatelliteRequestRequestTypeDef = TypedDict(
     "GetSatelliteRequestRequestTypeDef",
     {
         "satelliteId": str,
     },
 )
 
@@ -581,14 +740,22 @@
         "groundStationId": str,
         "groundStationName": str,
         "region": str,
     },
     total=False,
 )
 
+IntegerRangeOutputTypeDef = TypedDict(
+    "IntegerRangeOutputTypeDef",
+    {
+        "maximum": int,
+        "minimum": int,
+    },
+)
+
 IntegerRangeTypeDef = TypedDict(
     "IntegerRangeTypeDef",
     {
         "maximum": int,
         "minimum": int,
     },
 )
@@ -625,20 +792,22 @@
         "missionProfileArn": str,
         "satelliteArn": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListContactsRequestListContactsPaginateTypeDef(
     _RequiredListContactsRequestListContactsPaginateTypeDef,
     _OptionalListContactsRequestListContactsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListContactsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactsRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "startTime": Union[datetime, str],
         "statusList": Sequence[ContactStatusType],
     },
@@ -651,19 +820,21 @@
         "missionProfileArn": str,
         "nextToken": str,
         "satelliteArn": str,
     },
     total=False,
 )
 
+
 class ListContactsRequestRequestTypeDef(
     _RequiredListContactsRequestRequestTypeDef, _OptionalListContactsRequestRequestTypeDef
 ):
     pass
 
+
 ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef = TypedDict(
     "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -690,20 +861,22 @@
     {
         "statusList": Sequence[EphemerisStatusType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListEphemeridesRequestListEphemeridesPaginateTypeDef(
     _RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef,
     _OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListEphemeridesRequestRequestTypeDef = TypedDict(
     "_RequiredListEphemeridesRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "satelliteId": str,
         "startTime": Union[datetime, str],
     },
@@ -714,19 +887,21 @@
         "maxResults": int,
         "nextToken": str,
         "statusList": Sequence[EphemerisStatusType],
     },
     total=False,
 )
 
+
 class ListEphemeridesRequestRequestTypeDef(
     _RequiredListEphemeridesRequestRequestTypeDef, _OptionalListEphemeridesRequestRequestTypeDef
 ):
     pass
 
+
 ListGroundStationsRequestListGroundStationsPaginateTypeDef = TypedDict(
     "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
     {
         "satelliteId": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -806,14 +981,24 @@
     "MissionProfileIdResponseTypeDef",
     {
         "missionProfileId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+S3ObjectTypeDef = TypedDict(
+    "S3ObjectTypeDef",
+    {
+        "bucket": str,
+        "key": str,
+        "version": str,
+    },
+    total=False,
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -842,19 +1027,21 @@
     "_OptionalReserveContactRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class ReserveContactRequestRequestTypeDef(
     _RequiredReserveContactRequestRequestTypeDef, _OptionalReserveContactRequestRequestTypeDef
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
@@ -906,19 +1093,21 @@
     {
         "name": str,
         "priority": int,
     },
     total=False,
 )
 
+
 class UpdateEphemerisRequestRequestTypeDef(
     _RequiredUpdateEphemerisRequestRequestTypeDef, _OptionalUpdateEphemerisRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredAgentDetailsTypeDef = TypedDict(
     "_RequiredAgentDetailsTypeDef",
     {
         "agentVersion": str,
         "componentVersions": Sequence[ComponentVersionTypeDef],
         "instanceId": str,
         "instanceType": str,
@@ -929,17 +1118,19 @@
     {
         "agentCpuCores": Sequence[int],
         "reservedCpuCores": Sequence[int],
     },
     total=False,
 )
 
+
 class AgentDetailsTypeDef(_RequiredAgentDetailsTypeDef, _OptionalAgentDetailsTypeDef):
     pass
 
+
 UpdateAgentStatusRequestRequestTypeDef = TypedDict(
     "UpdateAgentStatusRequestRequestTypeDef",
     {
         "agentId": str,
         "aggregateStatus": AggregateStatusTypeDef,
         "componentStatuses": Sequence[ComponentStatusDataTypeDef],
         "taskId": str,
@@ -951,33 +1142,67 @@
     {
         "configList": List[ConfigListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredConnectionDetailsOutputTypeDef = TypedDict(
+    "_RequiredConnectionDetailsOutputTypeDef",
+    {
+        "socketAddress": SocketAddressOutputTypeDef,
+    },
+)
+_OptionalConnectionDetailsOutputTypeDef = TypedDict(
+    "_OptionalConnectionDetailsOutputTypeDef",
+    {
+        "mtu": int,
+    },
+    total=False,
+)
+
+
+class ConnectionDetailsOutputTypeDef(
+    _RequiredConnectionDetailsOutputTypeDef, _OptionalConnectionDetailsOutputTypeDef
+):
+    pass
+
+
+DataflowEndpointOutputTypeDef = TypedDict(
+    "DataflowEndpointOutputTypeDef",
+    {
+        "address": SocketAddressOutputTypeDef,
+        "mtu": int,
+        "name": str,
+        "status": EndpointStatusType,
+    },
+    total=False,
+)
+
 _RequiredConnectionDetailsTypeDef = TypedDict(
     "_RequiredConnectionDetailsTypeDef",
     {
         "socketAddress": SocketAddressTypeDef,
     },
 )
 _OptionalConnectionDetailsTypeDef = TypedDict(
     "_OptionalConnectionDetailsTypeDef",
     {
         "mtu": int,
     },
     total=False,
 )
 
+
 class ConnectionDetailsTypeDef(
     _RequiredConnectionDetailsTypeDef, _OptionalConnectionDetailsTypeDef
 ):
     pass
 
+
 DataflowEndpointTypeDef = TypedDict(
     "DataflowEndpointTypeDef",
     {
         "address": SocketAddressTypeDef,
         "mtu": int,
         "name": str,
         "status": EndpointStatusType,
@@ -1022,38 +1247,21 @@
         "streamsKmsKey": KmsKeyTypeDef,
         "streamsKmsRole": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateMissionProfileRequestRequestTypeDef(
     _RequiredCreateMissionProfileRequestRequestTypeDef,
     _OptionalCreateMissionProfileRequestRequestTypeDef,
 ):
     pass
 
-GetMissionProfileResponseTypeDef = TypedDict(
-    "GetMissionProfileResponseTypeDef",
-    {
-        "contactPostPassDurationSeconds": int,
-        "contactPrePassDurationSeconds": int,
-        "dataflowEdges": List[List[str]],
-        "minimumViableContactDurationSeconds": int,
-        "missionProfileArn": str,
-        "missionProfileId": str,
-        "name": str,
-        "region": str,
-        "streamsKmsKey": KmsKeyTypeDef,
-        "streamsKmsRole": str,
-        "tags": Dict[str, str],
-        "trackingConfigArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateMissionProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMissionProfileRequestRequestTypeDef",
     {
         "missionProfileId": str,
     },
 )
@@ -1068,20 +1276,22 @@
         "streamsKmsKey": KmsKeyTypeDef,
         "streamsKmsRole": str,
         "trackingConfigArn": str,
     },
     total=False,
 )
 
+
 class UpdateMissionProfileRequestRequestTypeDef(
     _RequiredUpdateMissionProfileRequestRequestTypeDef,
     _OptionalUpdateMissionProfileRequestRequestTypeDef,
 ):
     pass
 
+
 ListDataflowEndpointGroupsResponseTypeDef = TypedDict(
     "ListDataflowEndpointGroupsResponseTypeDef",
     {
         "dataflowEndpointGroupList": List[DataflowEndpointListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1097,52 +1307,45 @@
     "_OptionalDescribeContactRequestContactScheduledWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeContactRequestContactScheduledWaitTypeDef(
     _RequiredDescribeContactRequestContactScheduledWaitTypeDef,
     _OptionalDescribeContactRequestContactScheduledWaitTypeDef,
 ):
     pass
 
+
 EphemerisDescriptionTypeDef = TypedDict(
     "EphemerisDescriptionTypeDef",
     {
         "ephemerisData": str,
-        "sourceS3Object": S3ObjectTypeDef,
+        "sourceS3Object": S3ObjectOutputTypeDef,
     },
     total=False,
 )
 
 EphemerisItemTypeDef = TypedDict(
     "EphemerisItemTypeDef",
     {
         "creationTime": datetime,
         "enabled": bool,
         "ephemerisId": str,
         "name": str,
         "priority": int,
-        "sourceS3Object": S3ObjectTypeDef,
+        "sourceS3Object": S3ObjectOutputTypeDef,
         "status": EphemerisStatusType,
     },
     total=False,
 )
 
-OEMEphemerisTypeDef = TypedDict(
-    "OEMEphemerisTypeDef",
-    {
-        "oemData": str,
-        "s3Object": S3ObjectTypeDef,
-    },
-    total=False,
-)
-
 GetSatelliteResponseTypeDef = TypedDict(
     "GetSatelliteResponseTypeDef",
     {
         "currentEphemeris": EphemerisMetaDataTypeDef,
         "groundStations": List[str],
         "noradSatelliteID": int,
         "satelliteArn": str,
@@ -1159,14 +1362,57 @@
         "noradSatelliteID": int,
         "satelliteArn": str,
         "satelliteId": str,
     },
     total=False,
 )
 
+_RequiredSpectrumConfigOutputTypeDef = TypedDict(
+    "_RequiredSpectrumConfigOutputTypeDef",
+    {
+        "bandwidth": FrequencyBandwidthOutputTypeDef,
+        "centerFrequency": FrequencyOutputTypeDef,
+    },
+)
+_OptionalSpectrumConfigOutputTypeDef = TypedDict(
+    "_OptionalSpectrumConfigOutputTypeDef",
+    {
+        "polarization": PolarizationType,
+    },
+    total=False,
+)
+
+
+class SpectrumConfigOutputTypeDef(
+    _RequiredSpectrumConfigOutputTypeDef, _OptionalSpectrumConfigOutputTypeDef
+):
+    pass
+
+
+_RequiredUplinkSpectrumConfigOutputTypeDef = TypedDict(
+    "_RequiredUplinkSpectrumConfigOutputTypeDef",
+    {
+        "centerFrequency": FrequencyOutputTypeDef,
+    },
+)
+_OptionalUplinkSpectrumConfigOutputTypeDef = TypedDict(
+    "_OptionalUplinkSpectrumConfigOutputTypeDef",
+    {
+        "polarization": PolarizationType,
+    },
+    total=False,
+)
+
+
+class UplinkSpectrumConfigOutputTypeDef(
+    _RequiredUplinkSpectrumConfigOutputTypeDef, _OptionalUplinkSpectrumConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredSpectrumConfigTypeDef = TypedDict(
     "_RequiredSpectrumConfigTypeDef",
     {
         "bandwidth": FrequencyBandwidthTypeDef,
         "centerFrequency": FrequencyTypeDef,
     },
 )
@@ -1174,45 +1420,76 @@
     "_OptionalSpectrumConfigTypeDef",
     {
         "polarization": PolarizationType,
     },
     total=False,
 )
 
+
 class SpectrumConfigTypeDef(_RequiredSpectrumConfigTypeDef, _OptionalSpectrumConfigTypeDef):
     pass
 
+
 _RequiredUplinkSpectrumConfigTypeDef = TypedDict(
     "_RequiredUplinkSpectrumConfigTypeDef",
     {
         "centerFrequency": FrequencyTypeDef,
     },
 )
 _OptionalUplinkSpectrumConfigTypeDef = TypedDict(
     "_OptionalUplinkSpectrumConfigTypeDef",
     {
         "polarization": PolarizationType,
     },
     total=False,
 )
 
+
 class UplinkSpectrumConfigTypeDef(
     _RequiredUplinkSpectrumConfigTypeDef, _OptionalUplinkSpectrumConfigTypeDef
 ):
     pass
 
+
+GetMissionProfileResponseTypeDef = TypedDict(
+    "GetMissionProfileResponseTypeDef",
+    {
+        "contactPostPassDurationSeconds": int,
+        "contactPrePassDurationSeconds": int,
+        "dataflowEdges": List[List[str]],
+        "minimumViableContactDurationSeconds": int,
+        "missionProfileArn": str,
+        "missionProfileId": str,
+        "name": str,
+        "region": str,
+        "streamsKmsKey": KmsKeyOutputTypeDef,
+        "streamsKmsRole": str,
+        "tags": Dict[str, str],
+        "trackingConfigArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListGroundStationsResponseTypeDef = TypedDict(
     "ListGroundStationsResponseTypeDef",
     {
         "groundStationList": List[GroundStationDataTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RangedSocketAddressOutputTypeDef = TypedDict(
+    "RangedSocketAddressOutputTypeDef",
+    {
+        "name": str,
+        "portRange": IntegerRangeOutputTypeDef,
+    },
+)
+
 RangedSocketAddressTypeDef = TypedDict(
     "RangedSocketAddressTypeDef",
     {
         "name": str,
         "portRange": IntegerRangeTypeDef,
     },
 )
@@ -1222,14 +1499,23 @@
     {
         "missionProfileList": List[MissionProfileListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+OEMEphemerisTypeDef = TypedDict(
+    "OEMEphemerisTypeDef",
+    {
+        "oemData": str,
+        "s3Object": S3ObjectTypeDef,
+    },
+    total=False,
+)
+
 TLEDataTypeDef = TypedDict(
     "TLEDataTypeDef",
     {
         "tleLine1": str,
         "tleLine2": str,
         "validTimeRange": TimeRangeTypeDef,
     },
@@ -1275,14 +1561,52 @@
     {
         "nextToken": str,
         "satellites": List[SatelliteListItemTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AntennaDownlinkConfigOutputTypeDef = TypedDict(
+    "AntennaDownlinkConfigOutputTypeDef",
+    {
+        "spectrumConfig": SpectrumConfigOutputTypeDef,
+    },
+)
+
+AntennaDownlinkDemodDecodeConfigOutputTypeDef = TypedDict(
+    "AntennaDownlinkDemodDecodeConfigOutputTypeDef",
+    {
+        "decodeConfig": DecodeConfigOutputTypeDef,
+        "demodulationConfig": DemodulationConfigOutputTypeDef,
+        "spectrumConfig": SpectrumConfigOutputTypeDef,
+    },
+)
+
+_RequiredAntennaUplinkConfigOutputTypeDef = TypedDict(
+    "_RequiredAntennaUplinkConfigOutputTypeDef",
+    {
+        "spectrumConfig": UplinkSpectrumConfigOutputTypeDef,
+        "targetEirp": EirpOutputTypeDef,
+    },
+)
+_OptionalAntennaUplinkConfigOutputTypeDef = TypedDict(
+    "_OptionalAntennaUplinkConfigOutputTypeDef",
+    {
+        "transmitDisabled": bool,
+    },
+    total=False,
+)
+
+
+class AntennaUplinkConfigOutputTypeDef(
+    _RequiredAntennaUplinkConfigOutputTypeDef, _OptionalAntennaUplinkConfigOutputTypeDef
+):
+    pass
+
+
 AntennaDownlinkConfigTypeDef = TypedDict(
     "AntennaDownlinkConfigTypeDef",
     {
         "spectrumConfig": SpectrumConfigTypeDef,
     },
 )
 
@@ -1306,38 +1630,63 @@
     "_OptionalAntennaUplinkConfigTypeDef",
     {
         "transmitDisabled": bool,
     },
     total=False,
 )
 
+
 class AntennaUplinkConfigTypeDef(
     _RequiredAntennaUplinkConfigTypeDef, _OptionalAntennaUplinkConfigTypeDef
 ):
     pass
 
+
+_RequiredRangedConnectionDetailsOutputTypeDef = TypedDict(
+    "_RequiredRangedConnectionDetailsOutputTypeDef",
+    {
+        "socketAddress": RangedSocketAddressOutputTypeDef,
+    },
+)
+_OptionalRangedConnectionDetailsOutputTypeDef = TypedDict(
+    "_OptionalRangedConnectionDetailsOutputTypeDef",
+    {
+        "mtu": int,
+    },
+    total=False,
+)
+
+
+class RangedConnectionDetailsOutputTypeDef(
+    _RequiredRangedConnectionDetailsOutputTypeDef, _OptionalRangedConnectionDetailsOutputTypeDef
+):
+    pass
+
+
 _RequiredRangedConnectionDetailsTypeDef = TypedDict(
     "_RequiredRangedConnectionDetailsTypeDef",
     {
         "socketAddress": RangedSocketAddressTypeDef,
     },
 )
 _OptionalRangedConnectionDetailsTypeDef = TypedDict(
     "_OptionalRangedConnectionDetailsTypeDef",
     {
         "mtu": int,
     },
     total=False,
 )
 
+
 class RangedConnectionDetailsTypeDef(
     _RequiredRangedConnectionDetailsTypeDef, _OptionalRangedConnectionDetailsTypeDef
 ):
     pass
 
+
 TLEEphemerisTypeDef = TypedDict(
     "TLEEphemerisTypeDef",
     {
         "s3Object": S3ObjectTypeDef,
         "tleData": Sequence[TLEDataTypeDef],
     },
     total=False,
@@ -1356,28 +1705,67 @@
         "status": EphemerisStatusType,
         "suppliedData": EphemerisTypeDescriptionTypeDef,
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ConfigTypeDataOutputTypeDef = TypedDict(
+    "ConfigTypeDataOutputTypeDef",
+    {
+        "antennaDownlinkConfig": AntennaDownlinkConfigOutputTypeDef,
+        "antennaDownlinkDemodDecodeConfig": AntennaDownlinkDemodDecodeConfigOutputTypeDef,
+        "antennaUplinkConfig": AntennaUplinkConfigOutputTypeDef,
+        "dataflowEndpointConfig": DataflowEndpointConfigOutputTypeDef,
+        "s3RecordingConfig": S3RecordingConfigOutputTypeDef,
+        "trackingConfig": TrackingConfigOutputTypeDef,
+        "uplinkEchoConfig": UplinkEchoConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 ConfigTypeDataTypeDef = TypedDict(
     "ConfigTypeDataTypeDef",
     {
         "antennaDownlinkConfig": AntennaDownlinkConfigTypeDef,
         "antennaDownlinkDemodDecodeConfig": AntennaDownlinkDemodDecodeConfigTypeDef,
         "antennaUplinkConfig": AntennaUplinkConfigTypeDef,
         "dataflowEndpointConfig": DataflowEndpointConfigTypeDef,
         "s3RecordingConfig": S3RecordingConfigTypeDef,
         "trackingConfig": TrackingConfigTypeDef,
         "uplinkEchoConfig": UplinkEchoConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredAwsGroundStationAgentEndpointOutputTypeDef = TypedDict(
+    "_RequiredAwsGroundStationAgentEndpointOutputTypeDef",
+    {
+        "egressAddress": ConnectionDetailsOutputTypeDef,
+        "ingressAddress": RangedConnectionDetailsOutputTypeDef,
+        "name": str,
+    },
+)
+_OptionalAwsGroundStationAgentEndpointOutputTypeDef = TypedDict(
+    "_OptionalAwsGroundStationAgentEndpointOutputTypeDef",
+    {
+        "agentStatus": AgentStatusType,
+        "auditResults": AuditResultsType,
+    },
+    total=False,
+)
+
+
+class AwsGroundStationAgentEndpointOutputTypeDef(
+    _RequiredAwsGroundStationAgentEndpointOutputTypeDef,
+    _OptionalAwsGroundStationAgentEndpointOutputTypeDef,
+):
+    pass
+
+
 _RequiredAwsGroundStationAgentEndpointTypeDef = TypedDict(
     "_RequiredAwsGroundStationAgentEndpointTypeDef",
     {
         "egressAddress": ConnectionDetailsTypeDef,
         "ingressAddress": RangedConnectionDetailsTypeDef,
         "name": str,
     },
@@ -1387,28 +1775,43 @@
     {
         "agentStatus": AgentStatusType,
         "auditResults": AuditResultsType,
     },
     total=False,
 )
 
+
 class AwsGroundStationAgentEndpointTypeDef(
     _RequiredAwsGroundStationAgentEndpointTypeDef, _OptionalAwsGroundStationAgentEndpointTypeDef
 ):
     pass
 
+
 EphemerisDataTypeDef = TypedDict(
     "EphemerisDataTypeDef",
     {
         "oem": OEMEphemerisTypeDef,
         "tle": TLEEphemerisTypeDef,
     },
     total=False,
 )
 
+GetConfigResponseTypeDef = TypedDict(
+    "GetConfigResponseTypeDef",
+    {
+        "configArn": str,
+        "configData": ConfigTypeDataOutputTypeDef,
+        "configId": str,
+        "configType": ConfigCapabilityTypeType,
+        "name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigRequestRequestTypeDef",
     {
         "configData": ConfigTypeDataTypeDef,
         "name": str,
     },
 )
@@ -1416,40 +1819,41 @@
     "_OptionalCreateConfigRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateConfigRequestRequestTypeDef(
     _RequiredCreateConfigRequestRequestTypeDef, _OptionalCreateConfigRequestRequestTypeDef
 ):
     pass
 
-GetConfigResponseTypeDef = TypedDict(
-    "GetConfigResponseTypeDef",
+
+UpdateConfigRequestRequestTypeDef = TypedDict(
+    "UpdateConfigRequestRequestTypeDef",
     {
-        "configArn": str,
         "configData": ConfigTypeDataTypeDef,
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateConfigRequestRequestTypeDef = TypedDict(
-    "UpdateConfigRequestRequestTypeDef",
+EndpointDetailsOutputTypeDef = TypedDict(
+    "EndpointDetailsOutputTypeDef",
     {
-        "configData": ConfigTypeDataTypeDef,
-        "configId": str,
-        "configType": ConfigCapabilityTypeType,
-        "name": str,
+        "awsGroundStationAgentEndpoint": AwsGroundStationAgentEndpointOutputTypeDef,
+        "endpoint": DataflowEndpointOutputTypeDef,
+        "healthReasons": List[CapabilityHealthReasonType],
+        "healthStatus": CapabilityHealthType,
+        "securityDetails": SecurityDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 EndpointDetailsTypeDef = TypedDict(
     "EndpointDetailsTypeDef",
     {
         "awsGroundStationAgentEndpoint": AwsGroundStationAgentEndpointTypeDef,
         "endpoint": DataflowEndpointTypeDef,
@@ -1476,29 +1880,44 @@
         "kmsKeyArn": str,
         "priority": int,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateEphemerisRequestRequestTypeDef(
     _RequiredCreateEphemerisRequestRequestTypeDef, _OptionalCreateEphemerisRequestRequestTypeDef
 ):
     pass
 
+
 ConfigDetailsTypeDef = TypedDict(
     "ConfigDetailsTypeDef",
     {
         "antennaDemodDecodeDetails": AntennaDemodDecodeDetailsTypeDef,
-        "endpointDetails": EndpointDetailsTypeDef,
+        "endpointDetails": EndpointDetailsOutputTypeDef,
         "s3RecordingDetails": S3RecordingDetailsTypeDef,
     },
     total=False,
 )
 
+GetDataflowEndpointGroupResponseTypeDef = TypedDict(
+    "GetDataflowEndpointGroupResponseTypeDef",
+    {
+        "contactPostPassDurationSeconds": int,
+        "contactPrePassDurationSeconds": int,
+        "dataflowEndpointGroupArn": str,
+        "dataflowEndpointGroupId": str,
+        "endpointsDetails": List[EndpointDetailsOutputTypeDef],
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef",
     {
         "endpointDetails": Sequence[EndpointDetailsTypeDef],
     },
 )
 _OptionalCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
@@ -1507,32 +1926,21 @@
         "contactPostPassDurationSeconds": int,
         "contactPrePassDurationSeconds": int,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateDataflowEndpointGroupRequestRequestTypeDef(
     _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef,
     _OptionalCreateDataflowEndpointGroupRequestRequestTypeDef,
 ):
     pass
 
-GetDataflowEndpointGroupResponseTypeDef = TypedDict(
-    "GetDataflowEndpointGroupResponseTypeDef",
-    {
-        "contactPostPassDurationSeconds": int,
-        "contactPrePassDurationSeconds": int,
-        "dataflowEndpointGroupArn": str,
-        "dataflowEndpointGroupId": str,
-        "endpointsDetails": List[EndpointDetailsTypeDef],
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "configDetails": ConfigDetailsTypeDef,
         "configId": str,
         "configType": ConfigCapabilityTypeType,
```

### Comparing `mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/waiter.py` & `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation/waiter.pyi` & `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation.egg-info/PKG-INFO` & `mypy-boto3-groundstation-1.28.12/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-groundstation
-Version: 1.28.0
-Summary: Type annotations for boto3.GroundStation 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 groundstation type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-groundstation"></a>
 
 # mypy-boto3-groundstation
 
 [![PyPI - mypy-boto3-groundstation](https://img.shields.io/pypi/v/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-groundstation?color=blue)](https://pypistats.org/packages/mypy-boto3-groundstation)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-groundstation)](https://pepy.tech/project/mypy-boto3-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GroundStation 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[boto3.GroundStation 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
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
 [mypy-boto3-groundstation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -387,55 +355,68 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_groundstation.type_defs import (
     ComponentVersionTypeDef,
     AggregateStatusTypeDef,
     AntennaDemodDecodeDetailsTypeDef,
+    DecodeConfigOutputTypeDef,
+    DemodulationConfigOutputTypeDef,
     DecodeConfigTypeDef,
     DemodulationConfigTypeDef,
+    EirpOutputTypeDef,
     EirpTypeDef,
     CancelContactRequestRequestTypeDef,
     ComponentStatusDataTypeDef,
     S3RecordingDetailsTypeDef,
     ConfigIdResponseTypeDef,
     ConfigListItemTypeDef,
+    DataflowEndpointConfigOutputTypeDef,
+    S3RecordingConfigOutputTypeDef,
+    TrackingConfigOutputTypeDef,
+    UplinkEchoConfigOutputTypeDef,
     DataflowEndpointConfigTypeDef,
     S3RecordingConfigTypeDef,
     TrackingConfigTypeDef,
     UplinkEchoConfigTypeDef,
+    SocketAddressOutputTypeDef,
     SocketAddressTypeDef,
     ElevationTypeDef,
     ContactIdResponseTypeDef,
     KmsKeyTypeDef,
     DataflowEndpointGroupIdResponseTypeDef,
     DataflowEndpointListItemTypeDef,
     DeleteConfigRequestRequestTypeDef,
     DeleteDataflowEndpointGroupRequestRequestTypeDef,
     DeleteEphemerisRequestRequestTypeDef,
     DeleteMissionProfileRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeContactRequestRequestTypeDef,
     DescribeEphemerisRequestRequestTypeDef,
     DiscoveryDataTypeDef,
+    SecurityDetailsOutputTypeDef,
     SecurityDetailsTypeDef,
-    S3ObjectTypeDef,
+    S3ObjectOutputTypeDef,
     EphemerisIdResponseTypeDef,
     EphemerisMetaDataTypeDef,
+    FrequencyBandwidthOutputTypeDef,
     FrequencyBandwidthTypeDef,
+    FrequencyOutputTypeDef,
     FrequencyTypeDef,
     GetAgentConfigurationRequestRequestTypeDef,
     GetAgentConfigurationResponseTypeDef,
     GetConfigRequestRequestTypeDef,
     GetDataflowEndpointGroupRequestRequestTypeDef,
     GetMinuteUsageRequestRequestTypeDef,
     GetMinuteUsageResponseTypeDef,
     GetMissionProfileRequestRequestTypeDef,
+    KmsKeyOutputTypeDef,
     GetSatelliteRequestRequestTypeDef,
     GroundStationDataTypeDef,
+    IntegerRangeOutputTypeDef,
     IntegerRangeTypeDef,
     ListConfigsRequestListConfigsPaginateTypeDef,
     ListConfigsRequestRequestTypeDef,
     ListContactsRequestListContactsPaginateTypeDef,
     ListContactsRequestRequestTypeDef,
     ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef,
     ListDataflowEndpointGroupsRequestRequestTypeDef,
@@ -447,67 +428,80 @@
     ListMissionProfilesRequestRequestTypeDef,
     MissionProfileListItemTypeDef,
     ListSatellitesRequestListSatellitesPaginateTypeDef,
     ListSatellitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     MissionProfileIdResponseTypeDef,
+    S3ObjectTypeDef,
     PaginatorConfigTypeDef,
     RegisterAgentResponseTypeDef,
     ReserveContactRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TimeRangeTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgentStatusResponseTypeDef,
     UpdateEphemerisRequestRequestTypeDef,
     AgentDetailsTypeDef,
     UpdateAgentStatusRequestRequestTypeDef,
     ListConfigsResponseTypeDef,
+    ConnectionDetailsOutputTypeDef,
+    DataflowEndpointOutputTypeDef,
     ConnectionDetailsTypeDef,
     DataflowEndpointTypeDef,
     ContactDataTypeDef,
     CreateMissionProfileRequestRequestTypeDef,
-    GetMissionProfileResponseTypeDef,
     UpdateMissionProfileRequestRequestTypeDef,
     ListDataflowEndpointGroupsResponseTypeDef,
     DescribeContactRequestContactScheduledWaitTypeDef,
     EphemerisDescriptionTypeDef,
     EphemerisItemTypeDef,
-    OEMEphemerisTypeDef,
     GetSatelliteResponseTypeDef,
     SatelliteListItemTypeDef,
+    SpectrumConfigOutputTypeDef,
+    UplinkSpectrumConfigOutputTypeDef,
     SpectrumConfigTypeDef,
     UplinkSpectrumConfigTypeDef,
+    GetMissionProfileResponseTypeDef,
     ListGroundStationsResponseTypeDef,
+    RangedSocketAddressOutputTypeDef,
     RangedSocketAddressTypeDef,
     ListMissionProfilesResponseTypeDef,
+    OEMEphemerisTypeDef,
     TLEDataTypeDef,
     RegisterAgentRequestRequestTypeDef,
     ListContactsResponseTypeDef,
     EphemerisTypeDescriptionTypeDef,
     ListEphemeridesResponseTypeDef,
     ListSatellitesResponseTypeDef,
+    AntennaDownlinkConfigOutputTypeDef,
+    AntennaDownlinkDemodDecodeConfigOutputTypeDef,
+    AntennaUplinkConfigOutputTypeDef,
     AntennaDownlinkConfigTypeDef,
     AntennaDownlinkDemodDecodeConfigTypeDef,
     AntennaUplinkConfigTypeDef,
+    RangedConnectionDetailsOutputTypeDef,
     RangedConnectionDetailsTypeDef,
     TLEEphemerisTypeDef,
     DescribeEphemerisResponseTypeDef,
+    ConfigTypeDataOutputTypeDef,
     ConfigTypeDataTypeDef,
+    AwsGroundStationAgentEndpointOutputTypeDef,
     AwsGroundStationAgentEndpointTypeDef,
     EphemerisDataTypeDef,
-    CreateConfigRequestRequestTypeDef,
     GetConfigResponseTypeDef,
+    CreateConfigRequestRequestTypeDef,
     UpdateConfigRequestRequestTypeDef,
+    EndpointDetailsOutputTypeDef,
     EndpointDetailsTypeDef,
     CreateEphemerisRequestRequestTypeDef,
     ConfigDetailsTypeDef,
-    CreateDataflowEndpointGroupRequestRequestTypeDef,
     GetDataflowEndpointGroupResponseTypeDef,
+    CreateDataflowEndpointGroupRequestRequestTypeDef,
     DestinationTypeDef,
     SourceTypeDef,
     DataflowDetailTypeDef,
     DescribeContactResponseTypeDef,
 )
```

### Comparing `mypy-boto3-groundstation-1.28.0/mypy_boto3_groundstation.egg-info/SOURCES.txt` & `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.0/setup.py` & `mypy-boto3-groundstation-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-groundstation",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_groundstation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GroundStation 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.GroundStation 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

