# Comparing `tmp/mypy-boto3-globalaccelerator-1.28.0.tar.gz` & `tmp/mypy-boto3-globalaccelerator-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-globalaccelerator-1.28.0.tar", last modified: Thu Jul  6 20:59:40 2023, max compression
+gzip compressed data, was "mypy-boto3-globalaccelerator-1.28.12.tar", last modified: Thu Jul 27 05:34:44 2023, max compression
```

## Comparing `mypy-boto3-globalaccelerator-1.28.0.tar` & `mypy-boto3-globalaccelerator-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:40.042313 mypy-boto3-globalaccelerator-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:41:48.000000 mypy-boto3-globalaccelerator-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-06 20:59:40.042313 mypy-boto3-globalaccelerator-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18976 2023-07-06 20:41:48.000000 mypy-boto3-globalaccelerator-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:40.026313 mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-06 20:41:48.000000 mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-06 20:41:48.000000 mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-06 20:41:48.000000 mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41373 2023-07-06 20:41:48.000000 mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41309 2023-07-06 20:41:48.000000 mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-06 20:41:49.000000 mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-06 20:41:49.000000 mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-07-06 20:41:49.000000 mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-06 20:41:49.000000 mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:41:48.000000 mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    44730 2023-07-06 20:41:52.000000 mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44681 2023-07-06 20:41:49.000000 mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:41:48.000000 mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:40.042313 mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-06 20:59:39.000000 mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-06 20:59:39.000000 mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:39.000000 mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:39.000000 mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:39.000000 mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 20:59:39.000000 mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:40.042313 mypy-boto3-globalaccelerator-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-06 20:41:48.000000 mypy-boto3-globalaccelerator-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.156501 mypy-boto3-globalaccelerator-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20569 2023-07-27 05:34:44.148501 mypy-boto3-globalaccelerator-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19042 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.148501 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41373 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41309 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    45263 2023-07-27 05:22:47.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45214 2023-07-27 05:22:47.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.148501 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20569 2023-07-27 05:34:43.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-27 05:34:44.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:43.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:43.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:43.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:43.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:44.156501 mypy-boto3-globalaccelerator-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/setup.py
```

### Comparing `mypy-boto3-globalaccelerator-1.28.0/LICENSE` & `mypy-boto3-globalaccelerator-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-globalaccelerator-1.28.0/PKG-INFO` & `mypy-boto3-globalaccelerator-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-globalaccelerator
-Version: 1.28.0
-Summary: Type annotations for boto3.GlobalAccelerator 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.GlobalAccelerator 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-globalaccelerator"></a>
 
 # mypy-boto3-globalaccelerator
 
 [![PyPI - mypy-boto3-globalaccelerator](https://img.shields.io/pypi/v/mypy-boto3-globalaccelerator.svg?color=blue)](https://pypi.org/project/mypy-boto3-globalaccelerator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-globalaccelerator.svg?color=blue)](https://pypi.org/project/mypy-boto3-globalaccelerator)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-globalaccelerator?color=blue)](https://pypistats.org/packages/mypy-boto3-globalaccelerator)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-globalaccelerator)](https://pepy.tech/project/mypy-boto3-globalaccelerator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GlobalAccelerator 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
+[boto3.GlobalAccelerator 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
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
 [mypy-boto3-globalaccelerator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/).
 
 See how it helps to find and fix potential bugs:
 
@@ -380,14 +380,15 @@
     CidrAuthorizationContextTypeDef,
     TagTypeDef,
     CustomRoutingDestinationConfigurationTypeDef,
     PortRangeTypeDef,
     PortOverrideTypeDef,
     CustomRoutingAcceleratorAttributesTypeDef,
     CustomRoutingDestinationDescriptionTypeDef,
+    PortRangeOutputTypeDef,
     DeleteAcceleratorRequestRequestTypeDef,
     DeleteCustomRoutingAcceleratorRequestRequestTypeDef,
     DeleteCustomRoutingEndpointGroupRequestRequestTypeDef,
     DeleteCustomRoutingListenerRequestRequestTypeDef,
     DeleteEndpointGroupRequestRequestTypeDef,
     DeleteListenerRequestRequestTypeDef,
     DenyCustomRoutingTrafficRequestRequestTypeDef,
@@ -398,14 +399,15 @@
     DescribeCustomRoutingAcceleratorRequestRequestTypeDef,
     DescribeCustomRoutingEndpointGroupRequestRequestTypeDef,
     DescribeCustomRoutingListenerRequestRequestTypeDef,
     DescribeEndpointGroupRequestRequestTypeDef,
     DescribeListenerRequestRequestTypeDef,
     SocketAddressTypeDef,
     EmptyResponseMetadataTypeDef,
+    PortOverrideOutputTypeDef,
     EndpointIdentifierTypeDef,
     ListAcceleratorsRequestListAcceleratorsPaginateTypeDef,
     ListAcceleratorsRequestRequestTypeDef,
     ListByoipCidrsRequestListByoipCidrsPaginateTypeDef,
     ListByoipCidrsRequestRequestTypeDef,
     ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef,
     ListCustomRoutingAcceleratorsRequestRequestTypeDef,
@@ -417,14 +419,15 @@
     ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
     ListCustomRoutingPortMappingsRequestRequestTypeDef,
     ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
     ListEndpointGroupsRequestRequestTypeDef,
     ListListenersRequestListListenersPaginateTypeDef,
     ListListenersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
     RemoveCustomRoutingEndpointsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAcceleratorAttributesRequestRequestTypeDef,
     UpdateAcceleratorRequestRequestTypeDef,
     UpdateCustomRoutingAcceleratorAttributesRequestRequestTypeDef,
@@ -438,62 +441,62 @@
     AddCustomRoutingEndpointsResponseTypeDef,
     AddEndpointsRequestRequestTypeDef,
     AddEndpointsResponseTypeDef,
     ByoipCidrTypeDef,
     ProvisionByoipCidrRequestRequestTypeDef,
     CreateAcceleratorRequestRequestTypeDef,
     CreateCustomRoutingAcceleratorRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateCustomRoutingEndpointGroupRequestRequestTypeDef,
     CreateCustomRoutingListenerRequestRequestTypeDef,
     CreateListenerRequestRequestTypeDef,
-    CustomRoutingListenerTypeDef,
-    ListenerTypeDef,
     UpdateCustomRoutingListenerRequestRequestTypeDef,
     UpdateListenerRequestRequestTypeDef,
     CreateEndpointGroupRequestRequestTypeDef,
-    EndpointGroupTypeDef,
     UpdateEndpointGroupRequestRequestTypeDef,
     DescribeCustomRoutingAcceleratorAttributesResponseTypeDef,
     UpdateCustomRoutingAcceleratorAttributesResponseTypeDef,
     CustomRoutingEndpointGroupTypeDef,
+    CustomRoutingListenerTypeDef,
+    ListenerTypeDef,
     DestinationPortMappingTypeDef,
     PortMappingTypeDef,
+    EndpointGroupTypeDef,
     RemoveEndpointsRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateAcceleratorResponseTypeDef,
     DescribeAcceleratorResponseTypeDef,
     ListAcceleratorsResponseTypeDef,
     UpdateAcceleratorResponseTypeDef,
     CreateCustomRoutingAcceleratorResponseTypeDef,
     DescribeCustomRoutingAcceleratorResponseTypeDef,
     ListCustomRoutingAcceleratorsResponseTypeDef,
     UpdateCustomRoutingAcceleratorResponseTypeDef,
     AdvertiseByoipCidrResponseTypeDef,
     DeprovisionByoipCidrResponseTypeDef,
     ListByoipCidrsResponseTypeDef,
     ProvisionByoipCidrResponseTypeDef,
     WithdrawByoipCidrResponseTypeDef,
+    CreateCustomRoutingEndpointGroupResponseTypeDef,
+    DescribeCustomRoutingEndpointGroupResponseTypeDef,
+    ListCustomRoutingEndpointGroupsResponseTypeDef,
     CreateCustomRoutingListenerResponseTypeDef,
     DescribeCustomRoutingListenerResponseTypeDef,
     ListCustomRoutingListenersResponseTypeDef,
     UpdateCustomRoutingListenerResponseTypeDef,
     CreateListenerResponseTypeDef,
     DescribeListenerResponseTypeDef,
     ListListenersResponseTypeDef,
     UpdateListenerResponseTypeDef,
+    ListCustomRoutingPortMappingsByDestinationResponseTypeDef,
+    ListCustomRoutingPortMappingsResponseTypeDef,
     CreateEndpointGroupResponseTypeDef,
     DescribeEndpointGroupResponseTypeDef,
     ListEndpointGroupsResponseTypeDef,
     UpdateEndpointGroupResponseTypeDef,
-    CreateCustomRoutingEndpointGroupResponseTypeDef,
-    DescribeCustomRoutingEndpointGroupResponseTypeDef,
-    ListCustomRoutingEndpointGroupsResponseTypeDef,
-    ListCustomRoutingPortMappingsByDestinationResponseTypeDef,
-    ListCustomRoutingPortMappingsResponseTypeDef,
 )
 
 
 def get_structure() -> AcceleratorAttributesTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-globalaccelerator-1.28.0/README.md` & `mypy-boto3-globalaccelerator-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-globalaccelerator"></a>
 
 # mypy-boto3-globalaccelerator
 
 [![PyPI - mypy-boto3-globalaccelerator](https://img.shields.io/pypi/v/mypy-boto3-globalaccelerator.svg?color=blue)](https://pypi.org/project/mypy-boto3-globalaccelerator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-globalaccelerator.svg?color=blue)](https://pypi.org/project/mypy-boto3-globalaccelerator)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-globalaccelerator?color=blue)](https://pypistats.org/packages/mypy-boto3-globalaccelerator)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-globalaccelerator)](https://pepy.tech/project/mypy-boto3-globalaccelerator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GlobalAccelerator 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
+[boto3.GlobalAccelerator 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
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
 [mypy-boto3-globalaccelerator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/).
 
 See how it helps to find and fix potential bugs:
 
@@ -348,14 +348,15 @@
     CidrAuthorizationContextTypeDef,
     TagTypeDef,
     CustomRoutingDestinationConfigurationTypeDef,
     PortRangeTypeDef,
     PortOverrideTypeDef,
     CustomRoutingAcceleratorAttributesTypeDef,
     CustomRoutingDestinationDescriptionTypeDef,
+    PortRangeOutputTypeDef,
     DeleteAcceleratorRequestRequestTypeDef,
     DeleteCustomRoutingAcceleratorRequestRequestTypeDef,
     DeleteCustomRoutingEndpointGroupRequestRequestTypeDef,
     DeleteCustomRoutingListenerRequestRequestTypeDef,
     DeleteEndpointGroupRequestRequestTypeDef,
     DeleteListenerRequestRequestTypeDef,
     DenyCustomRoutingTrafficRequestRequestTypeDef,
@@ -366,14 +367,15 @@
     DescribeCustomRoutingAcceleratorRequestRequestTypeDef,
     DescribeCustomRoutingEndpointGroupRequestRequestTypeDef,
     DescribeCustomRoutingListenerRequestRequestTypeDef,
     DescribeEndpointGroupRequestRequestTypeDef,
     DescribeListenerRequestRequestTypeDef,
     SocketAddressTypeDef,
     EmptyResponseMetadataTypeDef,
+    PortOverrideOutputTypeDef,
     EndpointIdentifierTypeDef,
     ListAcceleratorsRequestListAcceleratorsPaginateTypeDef,
     ListAcceleratorsRequestRequestTypeDef,
     ListByoipCidrsRequestListByoipCidrsPaginateTypeDef,
     ListByoipCidrsRequestRequestTypeDef,
     ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef,
     ListCustomRoutingAcceleratorsRequestRequestTypeDef,
@@ -385,14 +387,15 @@
     ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
     ListCustomRoutingPortMappingsRequestRequestTypeDef,
     ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
     ListEndpointGroupsRequestRequestTypeDef,
     ListListenersRequestListListenersPaginateTypeDef,
     ListListenersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
     RemoveCustomRoutingEndpointsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAcceleratorAttributesRequestRequestTypeDef,
     UpdateAcceleratorRequestRequestTypeDef,
     UpdateCustomRoutingAcceleratorAttributesRequestRequestTypeDef,
@@ -406,62 +409,62 @@
     AddCustomRoutingEndpointsResponseTypeDef,
     AddEndpointsRequestRequestTypeDef,
     AddEndpointsResponseTypeDef,
     ByoipCidrTypeDef,
     ProvisionByoipCidrRequestRequestTypeDef,
     CreateAcceleratorRequestRequestTypeDef,
     CreateCustomRoutingAcceleratorRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateCustomRoutingEndpointGroupRequestRequestTypeDef,
     CreateCustomRoutingListenerRequestRequestTypeDef,
     CreateListenerRequestRequestTypeDef,
-    CustomRoutingListenerTypeDef,
-    ListenerTypeDef,
     UpdateCustomRoutingListenerRequestRequestTypeDef,
     UpdateListenerRequestRequestTypeDef,
     CreateEndpointGroupRequestRequestTypeDef,
-    EndpointGroupTypeDef,
     UpdateEndpointGroupRequestRequestTypeDef,
     DescribeCustomRoutingAcceleratorAttributesResponseTypeDef,
     UpdateCustomRoutingAcceleratorAttributesResponseTypeDef,
     CustomRoutingEndpointGroupTypeDef,
+    CustomRoutingListenerTypeDef,
+    ListenerTypeDef,
     DestinationPortMappingTypeDef,
     PortMappingTypeDef,
+    EndpointGroupTypeDef,
     RemoveEndpointsRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateAcceleratorResponseTypeDef,
     DescribeAcceleratorResponseTypeDef,
     ListAcceleratorsResponseTypeDef,
     UpdateAcceleratorResponseTypeDef,
     CreateCustomRoutingAcceleratorResponseTypeDef,
     DescribeCustomRoutingAcceleratorResponseTypeDef,
     ListCustomRoutingAcceleratorsResponseTypeDef,
     UpdateCustomRoutingAcceleratorResponseTypeDef,
     AdvertiseByoipCidrResponseTypeDef,
     DeprovisionByoipCidrResponseTypeDef,
     ListByoipCidrsResponseTypeDef,
     ProvisionByoipCidrResponseTypeDef,
     WithdrawByoipCidrResponseTypeDef,
+    CreateCustomRoutingEndpointGroupResponseTypeDef,
+    DescribeCustomRoutingEndpointGroupResponseTypeDef,
+    ListCustomRoutingEndpointGroupsResponseTypeDef,
     CreateCustomRoutingListenerResponseTypeDef,
     DescribeCustomRoutingListenerResponseTypeDef,
     ListCustomRoutingListenersResponseTypeDef,
     UpdateCustomRoutingListenerResponseTypeDef,
     CreateListenerResponseTypeDef,
     DescribeListenerResponseTypeDef,
     ListListenersResponseTypeDef,
     UpdateListenerResponseTypeDef,
+    ListCustomRoutingPortMappingsByDestinationResponseTypeDef,
+    ListCustomRoutingPortMappingsResponseTypeDef,
     CreateEndpointGroupResponseTypeDef,
     DescribeEndpointGroupResponseTypeDef,
     ListEndpointGroupsResponseTypeDef,
     UpdateEndpointGroupResponseTypeDef,
-    CreateCustomRoutingEndpointGroupResponseTypeDef,
-    DescribeCustomRoutingEndpointGroupResponseTypeDef,
-    ListCustomRoutingEndpointGroupsResponseTypeDef,
-    ListCustomRoutingPortMappingsByDestinationResponseTypeDef,
-    ListCustomRoutingPortMappingsResponseTypeDef,
 )
 
 
 def get_structure() -> AcceleratorAttributesTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/__init__.py` & `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/__init__.pyi` & `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/__main__.py` & `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GlobalAccelerator 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.GlobalAccelerator 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator\nOther"
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

### Comparing `mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/client.py` & `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/client.pyi` & `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/literals.py` & `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AcceleratorStatusType",
     "ByoipCidrStateType",
     "ClientAffinityType",
     "CustomRoutingAcceleratorStatusType",
     "CustomRoutingDestinationTrafficStateType",
     "CustomRoutingProtocolType",
@@ -41,15 +40,14 @@
     "ProtocolType",
     "GlobalAcceleratorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AcceleratorStatusType = Literal["DEPLOYED", "IN_PROGRESS"]
 ByoipCidrStateType = Literal[
     "ADVERTISING",
     "DEPROVISIONED",
     "FAILED_ADVERTISING",
     "FAILED_DEPROVISION",
     "FAILED_PROVISION",
@@ -195,14 +193,15 @@
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
@@ -281,26 +280,28 @@
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

### Comparing `mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/literals.pyi` & `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/literals.py`

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
     "AcceleratorStatusType",
     "ByoipCidrStateType",
     "ClientAffinityType",
     "CustomRoutingAcceleratorStatusType",
     "CustomRoutingDestinationTrafficStateType",
     "CustomRoutingProtocolType",
@@ -40,14 +41,15 @@
     "ProtocolType",
     "GlobalAcceleratorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
+
 AcceleratorStatusType = Literal["DEPLOYED", "IN_PROGRESS"]
 ByoipCidrStateType = Literal[
     "ADVERTISING",
     "DEPROVISIONED",
     "FAILED_ADVERTISING",
     "FAILED_DEPROVISION",
     "FAILED_PROVISION",
@@ -193,14 +195,15 @@
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
@@ -279,26 +282,28 @@
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

### Comparing `mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/paginator.py` & `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/paginator.pyi` & `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/type_defs.py` & `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     "CidrAuthorizationContextTypeDef",
     "TagTypeDef",
     "CustomRoutingDestinationConfigurationTypeDef",
     "PortRangeTypeDef",
     "PortOverrideTypeDef",
     "CustomRoutingAcceleratorAttributesTypeDef",
     "CustomRoutingDestinationDescriptionTypeDef",
+    "PortRangeOutputTypeDef",
     "DeleteAcceleratorRequestRequestTypeDef",
     "DeleteCustomRoutingAcceleratorRequestRequestTypeDef",
     "DeleteCustomRoutingEndpointGroupRequestRequestTypeDef",
     "DeleteCustomRoutingListenerRequestRequestTypeDef",
     "DeleteEndpointGroupRequestRequestTypeDef",
     "DeleteListenerRequestRequestTypeDef",
     "DenyCustomRoutingTrafficRequestRequestTypeDef",
@@ -67,14 +68,15 @@
     "DescribeCustomRoutingAcceleratorRequestRequestTypeDef",
     "DescribeCustomRoutingEndpointGroupRequestRequestTypeDef",
     "DescribeCustomRoutingListenerRequestRequestTypeDef",
     "DescribeEndpointGroupRequestRequestTypeDef",
     "DescribeListenerRequestRequestTypeDef",
     "SocketAddressTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "PortOverrideOutputTypeDef",
     "EndpointIdentifierTypeDef",
     "ListAcceleratorsRequestListAcceleratorsPaginateTypeDef",
     "ListAcceleratorsRequestRequestTypeDef",
     "ListByoipCidrsRequestListByoipCidrsPaginateTypeDef",
     "ListByoipCidrsRequestRequestTypeDef",
     "ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef",
     "ListCustomRoutingAcceleratorsRequestRequestTypeDef",
@@ -86,14 +88,15 @@
     "ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
     "ListCustomRoutingPortMappingsRequestRequestTypeDef",
     "ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
     "ListEndpointGroupsRequestRequestTypeDef",
     "ListListenersRequestListListenersPaginateTypeDef",
     "ListListenersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "PaginatorConfigTypeDef",
     "RemoveCustomRoutingEndpointsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAcceleratorAttributesRequestRequestTypeDef",
     "UpdateAcceleratorRequestRequestTypeDef",
     "UpdateCustomRoutingAcceleratorAttributesRequestRequestTypeDef",
@@ -107,62 +110,62 @@
     "AddCustomRoutingEndpointsResponseTypeDef",
     "AddEndpointsRequestRequestTypeDef",
     "AddEndpointsResponseTypeDef",
     "ByoipCidrTypeDef",
     "ProvisionByoipCidrRequestRequestTypeDef",
     "CreateAcceleratorRequestRequestTypeDef",
     "CreateCustomRoutingAcceleratorRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateCustomRoutingEndpointGroupRequestRequestTypeDef",
     "CreateCustomRoutingListenerRequestRequestTypeDef",
     "CreateListenerRequestRequestTypeDef",
-    "CustomRoutingListenerTypeDef",
-    "ListenerTypeDef",
     "UpdateCustomRoutingListenerRequestRequestTypeDef",
     "UpdateListenerRequestRequestTypeDef",
     "CreateEndpointGroupRequestRequestTypeDef",
-    "EndpointGroupTypeDef",
     "UpdateEndpointGroupRequestRequestTypeDef",
     "DescribeCustomRoutingAcceleratorAttributesResponseTypeDef",
     "UpdateCustomRoutingAcceleratorAttributesResponseTypeDef",
     "CustomRoutingEndpointGroupTypeDef",
+    "CustomRoutingListenerTypeDef",
+    "ListenerTypeDef",
     "DestinationPortMappingTypeDef",
     "PortMappingTypeDef",
+    "EndpointGroupTypeDef",
     "RemoveEndpointsRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateAcceleratorResponseTypeDef",
     "DescribeAcceleratorResponseTypeDef",
     "ListAcceleratorsResponseTypeDef",
     "UpdateAcceleratorResponseTypeDef",
     "CreateCustomRoutingAcceleratorResponseTypeDef",
     "DescribeCustomRoutingAcceleratorResponseTypeDef",
     "ListCustomRoutingAcceleratorsResponseTypeDef",
     "UpdateCustomRoutingAcceleratorResponseTypeDef",
     "AdvertiseByoipCidrResponseTypeDef",
     "DeprovisionByoipCidrResponseTypeDef",
     "ListByoipCidrsResponseTypeDef",
     "ProvisionByoipCidrResponseTypeDef",
     "WithdrawByoipCidrResponseTypeDef",
+    "CreateCustomRoutingEndpointGroupResponseTypeDef",
+    "DescribeCustomRoutingEndpointGroupResponseTypeDef",
+    "ListCustomRoutingEndpointGroupsResponseTypeDef",
     "CreateCustomRoutingListenerResponseTypeDef",
     "DescribeCustomRoutingListenerResponseTypeDef",
     "ListCustomRoutingListenersResponseTypeDef",
     "UpdateCustomRoutingListenerResponseTypeDef",
     "CreateListenerResponseTypeDef",
     "DescribeListenerResponseTypeDef",
     "ListListenersResponseTypeDef",
     "UpdateListenerResponseTypeDef",
+    "ListCustomRoutingPortMappingsByDestinationResponseTypeDef",
+    "ListCustomRoutingPortMappingsResponseTypeDef",
     "CreateEndpointGroupResponseTypeDef",
     "DescribeEndpointGroupResponseTypeDef",
     "ListEndpointGroupsResponseTypeDef",
     "UpdateEndpointGroupResponseTypeDef",
-    "CreateCustomRoutingEndpointGroupResponseTypeDef",
-    "DescribeCustomRoutingEndpointGroupResponseTypeDef",
-    "ListCustomRoutingEndpointGroupsResponseTypeDef",
-    "ListCustomRoutingPortMappingsByDestinationResponseTypeDef",
-    "ListCustomRoutingPortMappingsResponseTypeDef",
 )
 
 AcceleratorAttributesTypeDef = TypedDict(
     "AcceleratorAttributesTypeDef",
     {
         "FlowLogsEnabled": bool,
         "FlowLogsS3Bucket": str,
@@ -328,14 +331,23 @@
         "FromPort": int,
         "ToPort": int,
         "Protocols": List[ProtocolType],
     },
     total=False,
 )
 
+PortRangeOutputTypeDef = TypedDict(
+    "PortRangeOutputTypeDef",
+    {
+        "FromPort": int,
+        "ToPort": int,
+    },
+    total=False,
+)
+
 DeleteAcceleratorRequestRequestTypeDef = TypedDict(
     "DeleteAcceleratorRequestRequestTypeDef",
     {
         "AcceleratorArn": str,
     },
 )
 
@@ -474,14 +486,23 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PortOverrideOutputTypeDef = TypedDict(
+    "PortOverrideOutputTypeDef",
+    {
+        "ListenerPort": int,
+        "EndpointPort": int,
+    },
+    total=False,
+)
+
 _RequiredEndpointIdentifierTypeDef = TypedDict(
     "_RequiredEndpointIdentifierTypeDef",
     {
         "EndpointId": str,
     },
 )
 _OptionalEndpointIdentifierTypeDef = TypedDict(
@@ -808,14 +829,22 @@
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
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1100,22 +1129,14 @@
 class CreateCustomRoutingAcceleratorRequestRequestTypeDef(
     _RequiredCreateCustomRoutingAcceleratorRequestRequestTypeDef,
     _OptionalCreateCustomRoutingAcceleratorRequestRequestTypeDef,
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
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1159,34 +1180,14 @@
 
 class CreateListenerRequestRequestTypeDef(
     _RequiredCreateListenerRequestRequestTypeDef, _OptionalCreateListenerRequestRequestTypeDef
 ):
     pass
 
 
-CustomRoutingListenerTypeDef = TypedDict(
-    "CustomRoutingListenerTypeDef",
-    {
-        "ListenerArn": str,
-        "PortRanges": List[PortRangeTypeDef],
-    },
-    total=False,
-)
-
-ListenerTypeDef = TypedDict(
-    "ListenerTypeDef",
-    {
-        "ListenerArn": str,
-        "PortRanges": List[PortRangeTypeDef],
-        "Protocol": ProtocolType,
-        "ClientAffinity": ClientAffinityType,
-    },
-    total=False,
-)
-
 UpdateCustomRoutingListenerRequestRequestTypeDef = TypedDict(
     "UpdateCustomRoutingListenerRequestRequestTypeDef",
     {
         "ListenerArn": str,
         "PortRanges": Sequence[PortRangeTypeDef],
     },
 )
@@ -1241,31 +1242,14 @@
 class CreateEndpointGroupRequestRequestTypeDef(
     _RequiredCreateEndpointGroupRequestRequestTypeDef,
     _OptionalCreateEndpointGroupRequestRequestTypeDef,
 ):
     pass
 
 
-EndpointGroupTypeDef = TypedDict(
-    "EndpointGroupTypeDef",
-    {
-        "EndpointGroupArn": str,
-        "EndpointGroupRegion": str,
-        "EndpointDescriptions": List[EndpointDescriptionTypeDef],
-        "TrafficDialPercentage": float,
-        "HealthCheckPort": int,
-        "HealthCheckProtocol": HealthCheckProtocolType,
-        "HealthCheckPath": str,
-        "HealthCheckIntervalSeconds": int,
-        "ThresholdCount": int,
-        "PortOverrides": List[PortOverrideTypeDef],
-    },
-    total=False,
-)
-
 _RequiredUpdateEndpointGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEndpointGroupRequestRequestTypeDef",
     {
         "EndpointGroupArn": str,
     },
 )
 _OptionalUpdateEndpointGroupRequestRequestTypeDef = TypedDict(
@@ -1314,14 +1298,34 @@
         "EndpointGroupRegion": str,
         "DestinationDescriptions": List[CustomRoutingDestinationDescriptionTypeDef],
         "EndpointDescriptions": List[CustomRoutingEndpointDescriptionTypeDef],
     },
     total=False,
 )
 
+CustomRoutingListenerTypeDef = TypedDict(
+    "CustomRoutingListenerTypeDef",
+    {
+        "ListenerArn": str,
+        "PortRanges": List[PortRangeOutputTypeDef],
+    },
+    total=False,
+)
+
+ListenerTypeDef = TypedDict(
+    "ListenerTypeDef",
+    {
+        "ListenerArn": str,
+        "PortRanges": List[PortRangeOutputTypeDef],
+        "Protocol": ProtocolType,
+        "ClientAffinity": ClientAffinityType,
+    },
+    total=False,
+)
+
 DestinationPortMappingTypeDef = TypedDict(
     "DestinationPortMappingTypeDef",
     {
         "AcceleratorArn": str,
         "AcceleratorSocketAddresses": List[SocketAddressTypeDef],
         "EndpointGroupArn": str,
         "EndpointId": str,
@@ -1342,22 +1346,47 @@
         "DestinationSocketAddress": SocketAddressTypeDef,
         "Protocols": List[CustomRoutingProtocolType],
         "DestinationTrafficState": CustomRoutingDestinationTrafficStateType,
     },
     total=False,
 )
 
+EndpointGroupTypeDef = TypedDict(
+    "EndpointGroupTypeDef",
+    {
+        "EndpointGroupArn": str,
+        "EndpointGroupRegion": str,
+        "EndpointDescriptions": List[EndpointDescriptionTypeDef],
+        "TrafficDialPercentage": float,
+        "HealthCheckPort": int,
+        "HealthCheckProtocol": HealthCheckProtocolType,
+        "HealthCheckPath": str,
+        "HealthCheckIntervalSeconds": int,
+        "ThresholdCount": int,
+        "PortOverrides": List[PortOverrideOutputTypeDef],
+    },
+    total=False,
+)
+
 RemoveEndpointsRequestRequestTypeDef = TypedDict(
     "RemoveEndpointsRequestRequestTypeDef",
     {
         "EndpointIdentifiers": Sequence[EndpointIdentifierTypeDef],
         "EndpointGroupArn": str,
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
 CreateAcceleratorResponseTypeDef = TypedDict(
     "CreateAcceleratorResponseTypeDef",
     {
         "Accelerator": AcceleratorTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1457,14 +1486,39 @@
     "WithdrawByoipCidrResponseTypeDef",
     {
         "ByoipCidr": ByoipCidrTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateCustomRoutingEndpointGroupResponseTypeDef = TypedDict(
+    "CreateCustomRoutingEndpointGroupResponseTypeDef",
+    {
+        "EndpointGroup": CustomRoutingEndpointGroupTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeCustomRoutingEndpointGroupResponseTypeDef = TypedDict(
+    "DescribeCustomRoutingEndpointGroupResponseTypeDef",
+    {
+        "EndpointGroup": CustomRoutingEndpointGroupTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListCustomRoutingEndpointGroupsResponseTypeDef = TypedDict(
+    "ListCustomRoutingEndpointGroupsResponseTypeDef",
+    {
+        "EndpointGroups": List[CustomRoutingEndpointGroupTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateCustomRoutingListenerResponseTypeDef = TypedDict(
     "CreateCustomRoutingListenerResponseTypeDef",
     {
         "Listener": CustomRoutingListenerTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1523,82 +1577,57 @@
     "UpdateListenerResponseTypeDef",
     {
         "Listener": ListenerTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEndpointGroupResponseTypeDef = TypedDict(
-    "CreateEndpointGroupResponseTypeDef",
-    {
-        "EndpointGroup": EndpointGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeEndpointGroupResponseTypeDef = TypedDict(
-    "DescribeEndpointGroupResponseTypeDef",
+ListCustomRoutingPortMappingsByDestinationResponseTypeDef = TypedDict(
+    "ListCustomRoutingPortMappingsByDestinationResponseTypeDef",
     {
-        "EndpointGroup": EndpointGroupTypeDef,
+        "DestinationPortMappings": List[DestinationPortMappingTypeDef],
+        "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEndpointGroupsResponseTypeDef = TypedDict(
-    "ListEndpointGroupsResponseTypeDef",
+ListCustomRoutingPortMappingsResponseTypeDef = TypedDict(
+    "ListCustomRoutingPortMappingsResponseTypeDef",
     {
-        "EndpointGroups": List[EndpointGroupTypeDef],
+        "PortMappings": List[PortMappingTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateEndpointGroupResponseTypeDef = TypedDict(
-    "UpdateEndpointGroupResponseTypeDef",
+CreateEndpointGroupResponseTypeDef = TypedDict(
+    "CreateEndpointGroupResponseTypeDef",
     {
         "EndpointGroup": EndpointGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateCustomRoutingEndpointGroupResponseTypeDef = TypedDict(
-    "CreateCustomRoutingEndpointGroupResponseTypeDef",
-    {
-        "EndpointGroup": CustomRoutingEndpointGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeCustomRoutingEndpointGroupResponseTypeDef = TypedDict(
-    "DescribeCustomRoutingEndpointGroupResponseTypeDef",
-    {
-        "EndpointGroup": CustomRoutingEndpointGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCustomRoutingEndpointGroupsResponseTypeDef = TypedDict(
-    "ListCustomRoutingEndpointGroupsResponseTypeDef",
+DescribeEndpointGroupResponseTypeDef = TypedDict(
+    "DescribeEndpointGroupResponseTypeDef",
     {
-        "EndpointGroups": List[CustomRoutingEndpointGroupTypeDef],
-        "NextToken": str,
+        "EndpointGroup": EndpointGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListCustomRoutingPortMappingsByDestinationResponseTypeDef = TypedDict(
-    "ListCustomRoutingPortMappingsByDestinationResponseTypeDef",
+ListEndpointGroupsResponseTypeDef = TypedDict(
+    "ListEndpointGroupsResponseTypeDef",
     {
-        "DestinationPortMappings": List[DestinationPortMappingTypeDef],
+        "EndpointGroups": List[EndpointGroupTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListCustomRoutingPortMappingsResponseTypeDef = TypedDict(
-    "ListCustomRoutingPortMappingsResponseTypeDef",
+UpdateEndpointGroupResponseTypeDef = TypedDict(
+    "UpdateEndpointGroupResponseTypeDef",
     {
-        "PortMappings": List[PortMappingTypeDef],
-        "NextToken": str,
+        "EndpointGroup": EndpointGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator/type_defs.pyi` & `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     "CidrAuthorizationContextTypeDef",
     "TagTypeDef",
     "CustomRoutingDestinationConfigurationTypeDef",
     "PortRangeTypeDef",
     "PortOverrideTypeDef",
     "CustomRoutingAcceleratorAttributesTypeDef",
     "CustomRoutingDestinationDescriptionTypeDef",
+    "PortRangeOutputTypeDef",
     "DeleteAcceleratorRequestRequestTypeDef",
     "DeleteCustomRoutingAcceleratorRequestRequestTypeDef",
     "DeleteCustomRoutingEndpointGroupRequestRequestTypeDef",
     "DeleteCustomRoutingListenerRequestRequestTypeDef",
     "DeleteEndpointGroupRequestRequestTypeDef",
     "DeleteListenerRequestRequestTypeDef",
     "DenyCustomRoutingTrafficRequestRequestTypeDef",
@@ -66,14 +67,15 @@
     "DescribeCustomRoutingAcceleratorRequestRequestTypeDef",
     "DescribeCustomRoutingEndpointGroupRequestRequestTypeDef",
     "DescribeCustomRoutingListenerRequestRequestTypeDef",
     "DescribeEndpointGroupRequestRequestTypeDef",
     "DescribeListenerRequestRequestTypeDef",
     "SocketAddressTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "PortOverrideOutputTypeDef",
     "EndpointIdentifierTypeDef",
     "ListAcceleratorsRequestListAcceleratorsPaginateTypeDef",
     "ListAcceleratorsRequestRequestTypeDef",
     "ListByoipCidrsRequestListByoipCidrsPaginateTypeDef",
     "ListByoipCidrsRequestRequestTypeDef",
     "ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef",
     "ListCustomRoutingAcceleratorsRequestRequestTypeDef",
@@ -85,14 +87,15 @@
     "ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
     "ListCustomRoutingPortMappingsRequestRequestTypeDef",
     "ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
     "ListEndpointGroupsRequestRequestTypeDef",
     "ListListenersRequestListListenersPaginateTypeDef",
     "ListListenersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "PaginatorConfigTypeDef",
     "RemoveCustomRoutingEndpointsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAcceleratorAttributesRequestRequestTypeDef",
     "UpdateAcceleratorRequestRequestTypeDef",
     "UpdateCustomRoutingAcceleratorAttributesRequestRequestTypeDef",
@@ -106,62 +109,62 @@
     "AddCustomRoutingEndpointsResponseTypeDef",
     "AddEndpointsRequestRequestTypeDef",
     "AddEndpointsResponseTypeDef",
     "ByoipCidrTypeDef",
     "ProvisionByoipCidrRequestRequestTypeDef",
     "CreateAcceleratorRequestRequestTypeDef",
     "CreateCustomRoutingAcceleratorRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateCustomRoutingEndpointGroupRequestRequestTypeDef",
     "CreateCustomRoutingListenerRequestRequestTypeDef",
     "CreateListenerRequestRequestTypeDef",
-    "CustomRoutingListenerTypeDef",
-    "ListenerTypeDef",
     "UpdateCustomRoutingListenerRequestRequestTypeDef",
     "UpdateListenerRequestRequestTypeDef",
     "CreateEndpointGroupRequestRequestTypeDef",
-    "EndpointGroupTypeDef",
     "UpdateEndpointGroupRequestRequestTypeDef",
     "DescribeCustomRoutingAcceleratorAttributesResponseTypeDef",
     "UpdateCustomRoutingAcceleratorAttributesResponseTypeDef",
     "CustomRoutingEndpointGroupTypeDef",
+    "CustomRoutingListenerTypeDef",
+    "ListenerTypeDef",
     "DestinationPortMappingTypeDef",
     "PortMappingTypeDef",
+    "EndpointGroupTypeDef",
     "RemoveEndpointsRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateAcceleratorResponseTypeDef",
     "DescribeAcceleratorResponseTypeDef",
     "ListAcceleratorsResponseTypeDef",
     "UpdateAcceleratorResponseTypeDef",
     "CreateCustomRoutingAcceleratorResponseTypeDef",
     "DescribeCustomRoutingAcceleratorResponseTypeDef",
     "ListCustomRoutingAcceleratorsResponseTypeDef",
     "UpdateCustomRoutingAcceleratorResponseTypeDef",
     "AdvertiseByoipCidrResponseTypeDef",
     "DeprovisionByoipCidrResponseTypeDef",
     "ListByoipCidrsResponseTypeDef",
     "ProvisionByoipCidrResponseTypeDef",
     "WithdrawByoipCidrResponseTypeDef",
+    "CreateCustomRoutingEndpointGroupResponseTypeDef",
+    "DescribeCustomRoutingEndpointGroupResponseTypeDef",
+    "ListCustomRoutingEndpointGroupsResponseTypeDef",
     "CreateCustomRoutingListenerResponseTypeDef",
     "DescribeCustomRoutingListenerResponseTypeDef",
     "ListCustomRoutingListenersResponseTypeDef",
     "UpdateCustomRoutingListenerResponseTypeDef",
     "CreateListenerResponseTypeDef",
     "DescribeListenerResponseTypeDef",
     "ListListenersResponseTypeDef",
     "UpdateListenerResponseTypeDef",
+    "ListCustomRoutingPortMappingsByDestinationResponseTypeDef",
+    "ListCustomRoutingPortMappingsResponseTypeDef",
     "CreateEndpointGroupResponseTypeDef",
     "DescribeEndpointGroupResponseTypeDef",
     "ListEndpointGroupsResponseTypeDef",
     "UpdateEndpointGroupResponseTypeDef",
-    "CreateCustomRoutingEndpointGroupResponseTypeDef",
-    "DescribeCustomRoutingEndpointGroupResponseTypeDef",
-    "ListCustomRoutingEndpointGroupsResponseTypeDef",
-    "ListCustomRoutingPortMappingsByDestinationResponseTypeDef",
-    "ListCustomRoutingPortMappingsResponseTypeDef",
 )
 
 AcceleratorAttributesTypeDef = TypedDict(
     "AcceleratorAttributesTypeDef",
     {
         "FlowLogsEnabled": bool,
         "FlowLogsS3Bucket": str,
@@ -325,14 +328,23 @@
         "FromPort": int,
         "ToPort": int,
         "Protocols": List[ProtocolType],
     },
     total=False,
 )
 
+PortRangeOutputTypeDef = TypedDict(
+    "PortRangeOutputTypeDef",
+    {
+        "FromPort": int,
+        "ToPort": int,
+    },
+    total=False,
+)
+
 DeleteAcceleratorRequestRequestTypeDef = TypedDict(
     "DeleteAcceleratorRequestRequestTypeDef",
     {
         "AcceleratorArn": str,
     },
 )
 
@@ -469,14 +481,23 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PortOverrideOutputTypeDef = TypedDict(
+    "PortOverrideOutputTypeDef",
+    {
+        "ListenerPort": int,
+        "EndpointPort": int,
+    },
+    total=False,
+)
+
 _RequiredEndpointIdentifierTypeDef = TypedDict(
     "_RequiredEndpointIdentifierTypeDef",
     {
         "EndpointId": str,
     },
 )
 _OptionalEndpointIdentifierTypeDef = TypedDict(
@@ -779,14 +800,22 @@
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
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1059,22 +1088,14 @@
 
 class CreateCustomRoutingAcceleratorRequestRequestTypeDef(
     _RequiredCreateCustomRoutingAcceleratorRequestRequestTypeDef,
     _OptionalCreateCustomRoutingAcceleratorRequestRequestTypeDef,
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
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1116,34 +1137,14 @@
 )
 
 class CreateListenerRequestRequestTypeDef(
     _RequiredCreateListenerRequestRequestTypeDef, _OptionalCreateListenerRequestRequestTypeDef
 ):
     pass
 
-CustomRoutingListenerTypeDef = TypedDict(
-    "CustomRoutingListenerTypeDef",
-    {
-        "ListenerArn": str,
-        "PortRanges": List[PortRangeTypeDef],
-    },
-    total=False,
-)
-
-ListenerTypeDef = TypedDict(
-    "ListenerTypeDef",
-    {
-        "ListenerArn": str,
-        "PortRanges": List[PortRangeTypeDef],
-        "Protocol": ProtocolType,
-        "ClientAffinity": ClientAffinityType,
-    },
-    total=False,
-)
-
 UpdateCustomRoutingListenerRequestRequestTypeDef = TypedDict(
     "UpdateCustomRoutingListenerRequestRequestTypeDef",
     {
         "ListenerArn": str,
         "PortRanges": Sequence[PortRangeTypeDef],
     },
 )
@@ -1194,31 +1195,14 @@
 
 class CreateEndpointGroupRequestRequestTypeDef(
     _RequiredCreateEndpointGroupRequestRequestTypeDef,
     _OptionalCreateEndpointGroupRequestRequestTypeDef,
 ):
     pass
 
-EndpointGroupTypeDef = TypedDict(
-    "EndpointGroupTypeDef",
-    {
-        "EndpointGroupArn": str,
-        "EndpointGroupRegion": str,
-        "EndpointDescriptions": List[EndpointDescriptionTypeDef],
-        "TrafficDialPercentage": float,
-        "HealthCheckPort": int,
-        "HealthCheckProtocol": HealthCheckProtocolType,
-        "HealthCheckPath": str,
-        "HealthCheckIntervalSeconds": int,
-        "ThresholdCount": int,
-        "PortOverrides": List[PortOverrideTypeDef],
-    },
-    total=False,
-)
-
 _RequiredUpdateEndpointGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEndpointGroupRequestRequestTypeDef",
     {
         "EndpointGroupArn": str,
     },
 )
 _OptionalUpdateEndpointGroupRequestRequestTypeDef = TypedDict(
@@ -1265,14 +1249,34 @@
         "EndpointGroupRegion": str,
         "DestinationDescriptions": List[CustomRoutingDestinationDescriptionTypeDef],
         "EndpointDescriptions": List[CustomRoutingEndpointDescriptionTypeDef],
     },
     total=False,
 )
 
+CustomRoutingListenerTypeDef = TypedDict(
+    "CustomRoutingListenerTypeDef",
+    {
+        "ListenerArn": str,
+        "PortRanges": List[PortRangeOutputTypeDef],
+    },
+    total=False,
+)
+
+ListenerTypeDef = TypedDict(
+    "ListenerTypeDef",
+    {
+        "ListenerArn": str,
+        "PortRanges": List[PortRangeOutputTypeDef],
+        "Protocol": ProtocolType,
+        "ClientAffinity": ClientAffinityType,
+    },
+    total=False,
+)
+
 DestinationPortMappingTypeDef = TypedDict(
     "DestinationPortMappingTypeDef",
     {
         "AcceleratorArn": str,
         "AcceleratorSocketAddresses": List[SocketAddressTypeDef],
         "EndpointGroupArn": str,
         "EndpointId": str,
@@ -1293,22 +1297,47 @@
         "DestinationSocketAddress": SocketAddressTypeDef,
         "Protocols": List[CustomRoutingProtocolType],
         "DestinationTrafficState": CustomRoutingDestinationTrafficStateType,
     },
     total=False,
 )
 
+EndpointGroupTypeDef = TypedDict(
+    "EndpointGroupTypeDef",
+    {
+        "EndpointGroupArn": str,
+        "EndpointGroupRegion": str,
+        "EndpointDescriptions": List[EndpointDescriptionTypeDef],
+        "TrafficDialPercentage": float,
+        "HealthCheckPort": int,
+        "HealthCheckProtocol": HealthCheckProtocolType,
+        "HealthCheckPath": str,
+        "HealthCheckIntervalSeconds": int,
+        "ThresholdCount": int,
+        "PortOverrides": List[PortOverrideOutputTypeDef],
+    },
+    total=False,
+)
+
 RemoveEndpointsRequestRequestTypeDef = TypedDict(
     "RemoveEndpointsRequestRequestTypeDef",
     {
         "EndpointIdentifiers": Sequence[EndpointIdentifierTypeDef],
         "EndpointGroupArn": str,
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
 CreateAcceleratorResponseTypeDef = TypedDict(
     "CreateAcceleratorResponseTypeDef",
     {
         "Accelerator": AcceleratorTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1408,14 +1437,39 @@
     "WithdrawByoipCidrResponseTypeDef",
     {
         "ByoipCidr": ByoipCidrTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateCustomRoutingEndpointGroupResponseTypeDef = TypedDict(
+    "CreateCustomRoutingEndpointGroupResponseTypeDef",
+    {
+        "EndpointGroup": CustomRoutingEndpointGroupTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeCustomRoutingEndpointGroupResponseTypeDef = TypedDict(
+    "DescribeCustomRoutingEndpointGroupResponseTypeDef",
+    {
+        "EndpointGroup": CustomRoutingEndpointGroupTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListCustomRoutingEndpointGroupsResponseTypeDef = TypedDict(
+    "ListCustomRoutingEndpointGroupsResponseTypeDef",
+    {
+        "EndpointGroups": List[CustomRoutingEndpointGroupTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateCustomRoutingListenerResponseTypeDef = TypedDict(
     "CreateCustomRoutingListenerResponseTypeDef",
     {
         "Listener": CustomRoutingListenerTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1474,82 +1528,57 @@
     "UpdateListenerResponseTypeDef",
     {
         "Listener": ListenerTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateEndpointGroupResponseTypeDef = TypedDict(
-    "CreateEndpointGroupResponseTypeDef",
-    {
-        "EndpointGroup": EndpointGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeEndpointGroupResponseTypeDef = TypedDict(
-    "DescribeEndpointGroupResponseTypeDef",
+ListCustomRoutingPortMappingsByDestinationResponseTypeDef = TypedDict(
+    "ListCustomRoutingPortMappingsByDestinationResponseTypeDef",
     {
-        "EndpointGroup": EndpointGroupTypeDef,
+        "DestinationPortMappings": List[DestinationPortMappingTypeDef],
+        "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListEndpointGroupsResponseTypeDef = TypedDict(
-    "ListEndpointGroupsResponseTypeDef",
+ListCustomRoutingPortMappingsResponseTypeDef = TypedDict(
+    "ListCustomRoutingPortMappingsResponseTypeDef",
     {
-        "EndpointGroups": List[EndpointGroupTypeDef],
+        "PortMappings": List[PortMappingTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateEndpointGroupResponseTypeDef = TypedDict(
-    "UpdateEndpointGroupResponseTypeDef",
+CreateEndpointGroupResponseTypeDef = TypedDict(
+    "CreateEndpointGroupResponseTypeDef",
     {
         "EndpointGroup": EndpointGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateCustomRoutingEndpointGroupResponseTypeDef = TypedDict(
-    "CreateCustomRoutingEndpointGroupResponseTypeDef",
-    {
-        "EndpointGroup": CustomRoutingEndpointGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeCustomRoutingEndpointGroupResponseTypeDef = TypedDict(
-    "DescribeCustomRoutingEndpointGroupResponseTypeDef",
-    {
-        "EndpointGroup": CustomRoutingEndpointGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCustomRoutingEndpointGroupsResponseTypeDef = TypedDict(
-    "ListCustomRoutingEndpointGroupsResponseTypeDef",
+DescribeEndpointGroupResponseTypeDef = TypedDict(
+    "DescribeEndpointGroupResponseTypeDef",
     {
-        "EndpointGroups": List[CustomRoutingEndpointGroupTypeDef],
-        "NextToken": str,
+        "EndpointGroup": EndpointGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListCustomRoutingPortMappingsByDestinationResponseTypeDef = TypedDict(
-    "ListCustomRoutingPortMappingsByDestinationResponseTypeDef",
+ListEndpointGroupsResponseTypeDef = TypedDict(
+    "ListEndpointGroupsResponseTypeDef",
     {
-        "DestinationPortMappings": List[DestinationPortMappingTypeDef],
+        "EndpointGroups": List[EndpointGroupTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListCustomRoutingPortMappingsResponseTypeDef = TypedDict(
-    "ListCustomRoutingPortMappingsResponseTypeDef",
+UpdateEndpointGroupResponseTypeDef = TypedDict(
+    "UpdateEndpointGroupResponseTypeDef",
     {
-        "PortMappings": List[PortMappingTypeDef],
-        "NextToken": str,
+        "EndpointGroup": EndpointGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator.egg-info/PKG-INFO` & `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-globalaccelerator
-Version: 1.28.0
-Summary: Type annotations for boto3.GlobalAccelerator 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.GlobalAccelerator 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-globalaccelerator"></a>
 
 # mypy-boto3-globalaccelerator
 
 [![PyPI - mypy-boto3-globalaccelerator](https://img.shields.io/pypi/v/mypy-boto3-globalaccelerator.svg?color=blue)](https://pypi.org/project/mypy-boto3-globalaccelerator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-globalaccelerator.svg?color=blue)](https://pypi.org/project/mypy-boto3-globalaccelerator)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-globalaccelerator?color=blue)](https://pypistats.org/packages/mypy-boto3-globalaccelerator)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-globalaccelerator)](https://pepy.tech/project/mypy-boto3-globalaccelerator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GlobalAccelerator 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
+[boto3.GlobalAccelerator 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
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
 [mypy-boto3-globalaccelerator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/).
 
 See how it helps to find and fix potential bugs:
 
@@ -380,14 +380,15 @@
     CidrAuthorizationContextTypeDef,
     TagTypeDef,
     CustomRoutingDestinationConfigurationTypeDef,
     PortRangeTypeDef,
     PortOverrideTypeDef,
     CustomRoutingAcceleratorAttributesTypeDef,
     CustomRoutingDestinationDescriptionTypeDef,
+    PortRangeOutputTypeDef,
     DeleteAcceleratorRequestRequestTypeDef,
     DeleteCustomRoutingAcceleratorRequestRequestTypeDef,
     DeleteCustomRoutingEndpointGroupRequestRequestTypeDef,
     DeleteCustomRoutingListenerRequestRequestTypeDef,
     DeleteEndpointGroupRequestRequestTypeDef,
     DeleteListenerRequestRequestTypeDef,
     DenyCustomRoutingTrafficRequestRequestTypeDef,
@@ -398,14 +399,15 @@
     DescribeCustomRoutingAcceleratorRequestRequestTypeDef,
     DescribeCustomRoutingEndpointGroupRequestRequestTypeDef,
     DescribeCustomRoutingListenerRequestRequestTypeDef,
     DescribeEndpointGroupRequestRequestTypeDef,
     DescribeListenerRequestRequestTypeDef,
     SocketAddressTypeDef,
     EmptyResponseMetadataTypeDef,
+    PortOverrideOutputTypeDef,
     EndpointIdentifierTypeDef,
     ListAcceleratorsRequestListAcceleratorsPaginateTypeDef,
     ListAcceleratorsRequestRequestTypeDef,
     ListByoipCidrsRequestListByoipCidrsPaginateTypeDef,
     ListByoipCidrsRequestRequestTypeDef,
     ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef,
     ListCustomRoutingAcceleratorsRequestRequestTypeDef,
@@ -417,14 +419,15 @@
     ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
     ListCustomRoutingPortMappingsRequestRequestTypeDef,
     ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
     ListEndpointGroupsRequestRequestTypeDef,
     ListListenersRequestListListenersPaginateTypeDef,
     ListListenersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
     RemoveCustomRoutingEndpointsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAcceleratorAttributesRequestRequestTypeDef,
     UpdateAcceleratorRequestRequestTypeDef,
     UpdateCustomRoutingAcceleratorAttributesRequestRequestTypeDef,
@@ -438,62 +441,62 @@
     AddCustomRoutingEndpointsResponseTypeDef,
     AddEndpointsRequestRequestTypeDef,
     AddEndpointsResponseTypeDef,
     ByoipCidrTypeDef,
     ProvisionByoipCidrRequestRequestTypeDef,
     CreateAcceleratorRequestRequestTypeDef,
     CreateCustomRoutingAcceleratorRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateCustomRoutingEndpointGroupRequestRequestTypeDef,
     CreateCustomRoutingListenerRequestRequestTypeDef,
     CreateListenerRequestRequestTypeDef,
-    CustomRoutingListenerTypeDef,
-    ListenerTypeDef,
     UpdateCustomRoutingListenerRequestRequestTypeDef,
     UpdateListenerRequestRequestTypeDef,
     CreateEndpointGroupRequestRequestTypeDef,
-    EndpointGroupTypeDef,
     UpdateEndpointGroupRequestRequestTypeDef,
     DescribeCustomRoutingAcceleratorAttributesResponseTypeDef,
     UpdateCustomRoutingAcceleratorAttributesResponseTypeDef,
     CustomRoutingEndpointGroupTypeDef,
+    CustomRoutingListenerTypeDef,
+    ListenerTypeDef,
     DestinationPortMappingTypeDef,
     PortMappingTypeDef,
+    EndpointGroupTypeDef,
     RemoveEndpointsRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateAcceleratorResponseTypeDef,
     DescribeAcceleratorResponseTypeDef,
     ListAcceleratorsResponseTypeDef,
     UpdateAcceleratorResponseTypeDef,
     CreateCustomRoutingAcceleratorResponseTypeDef,
     DescribeCustomRoutingAcceleratorResponseTypeDef,
     ListCustomRoutingAcceleratorsResponseTypeDef,
     UpdateCustomRoutingAcceleratorResponseTypeDef,
     AdvertiseByoipCidrResponseTypeDef,
     DeprovisionByoipCidrResponseTypeDef,
     ListByoipCidrsResponseTypeDef,
     ProvisionByoipCidrResponseTypeDef,
     WithdrawByoipCidrResponseTypeDef,
+    CreateCustomRoutingEndpointGroupResponseTypeDef,
+    DescribeCustomRoutingEndpointGroupResponseTypeDef,
+    ListCustomRoutingEndpointGroupsResponseTypeDef,
     CreateCustomRoutingListenerResponseTypeDef,
     DescribeCustomRoutingListenerResponseTypeDef,
     ListCustomRoutingListenersResponseTypeDef,
     UpdateCustomRoutingListenerResponseTypeDef,
     CreateListenerResponseTypeDef,
     DescribeListenerResponseTypeDef,
     ListListenersResponseTypeDef,
     UpdateListenerResponseTypeDef,
+    ListCustomRoutingPortMappingsByDestinationResponseTypeDef,
+    ListCustomRoutingPortMappingsResponseTypeDef,
     CreateEndpointGroupResponseTypeDef,
     DescribeEndpointGroupResponseTypeDef,
     ListEndpointGroupsResponseTypeDef,
     UpdateEndpointGroupResponseTypeDef,
-    CreateCustomRoutingEndpointGroupResponseTypeDef,
-    DescribeCustomRoutingEndpointGroupResponseTypeDef,
-    ListCustomRoutingEndpointGroupsResponseTypeDef,
-    ListCustomRoutingPortMappingsByDestinationResponseTypeDef,
-    ListCustomRoutingPortMappingsResponseTypeDef,
 )
 
 
 def get_structure() -> AcceleratorAttributesTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-globalaccelerator-1.28.0/mypy_boto3_globalaccelerator.egg-info/SOURCES.txt` & `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-globalaccelerator-1.28.0/setup.py` & `mypy-boto3-globalaccelerator-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-globalaccelerator",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_globalaccelerator"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GlobalAccelerator 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.GlobalAccelerator 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

