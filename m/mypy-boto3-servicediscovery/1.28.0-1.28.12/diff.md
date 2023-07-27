# Comparing `tmp/mypy-boto3-servicediscovery-1.28.0.tar.gz` & `tmp/mypy-boto3-servicediscovery-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-servicediscovery-1.28.0.tar", last modified: Thu Jul  6 21:00:37 2023, max compression
+gzip compressed data, was "mypy-boto3-servicediscovery-1.28.12.tar", last modified: Thu Jul 27 11:49:38 2023, max compression
```

## Comparing `mypy-boto3-servicediscovery-1.28.0.tar` & `mypy-boto3-servicediscovery-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:37.398431 mypy-boto3-servicediscovery-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:55:45.000000 mypy-boto3-servicediscovery-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-07-06 21:00:37.378430 mypy-boto3-servicediscovery-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15658 2023-07-06 20:55:45.000000 mypy-boto3-servicediscovery-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:37.378430 mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-06 20:55:45.000000 mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-06 20:55:45.000000 mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-06 20:55:45.000000 mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-06 20:55:45.000000 mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22776 2023-07-06 20:55:45.000000 mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10169 2023-07-06 20:55:45.000000 mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-07-06 20:55:45.000000 mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-07-06 20:55:45.000000 mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-07-06 20:55:45.000000 mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:55:45.000000 mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28472 2023-07-06 20:55:46.000000 mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28436 2023-07-06 20:55:46.000000 mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:55:45.000000 mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:37.378430 mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-07-06 21:00:37.000000 mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-06 21:00:37.000000 mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:37.000000 mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:37.000000 mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:37.000000 mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 21:00:37.000000 mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:37.398431 mypy-boto3-servicediscovery-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-06 20:55:44.000000 mypy-boto3-servicediscovery-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.765293 mypy-boto3-servicediscovery-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:47.000000 mypy-boto3-servicediscovery-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17344 2023-07-27 11:49:38.757293 mypy-boto3-servicediscovery-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15821 2023-07-27 11:46:47.000000 mypy-boto3-servicediscovery-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.757293 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-27 11:46:47.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-27 11:46:47.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-27 11:46:47.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-27 11:46:48.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22776 2023-07-27 11:46:48.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-07-27 11:46:48.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-07-27 11:46:48.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-27 11:46:48.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-07-27 11:46:48.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:47.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    30085 2023-07-27 11:46:49.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30045 2023-07-27 11:46:48.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:47.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.757293 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17344 2023-07-27 11:49:38.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-27 11:49:38.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:38.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 11:49:38.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:38.765293 mypy-boto3-servicediscovery-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 11:46:47.000000 mypy-boto3-servicediscovery-1.28.12/setup.py
```

### Comparing `mypy-boto3-servicediscovery-1.28.0/LICENSE` & `mypy-boto3-servicediscovery-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.0/PKG-INFO` & `mypy-boto3-servicediscovery-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicediscovery
-Version: 1.28.0
-Summary: Type annotations for boto3.ServiceDiscovery 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ServiceDiscovery 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-servicediscovery"></a>
 
 # mypy-boto3-servicediscovery
 
 [![PyPI - mypy-boto3-servicediscovery](https://img.shields.io/pypi/v/mypy-boto3-servicediscovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicediscovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicediscovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicediscovery)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-servicediscovery?color=blue)](https://pypistats.org/packages/mypy-boto3-servicediscovery)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicediscovery)](https://pepy.tech/project/mypy-boto3-servicediscovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceDiscovery 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
+[boto3.ServiceDiscovery 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
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
 [mypy-boto3-servicediscovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -348,99 +348,105 @@
 
 `mypy_boto3_servicediscovery.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_servicediscovery.type_defs import (
     TagTypeDef,
-    CreateHttpNamespaceResponseTypeDef,
-    CreatePrivateDnsNamespaceResponseTypeDef,
-    CreatePublicDnsNamespaceResponseTypeDef,
+    ResponseMetadataTypeDef,
     HealthCheckConfigTypeDef,
     HealthCheckCustomConfigTypeDef,
     DeleteNamespaceRequestRequestTypeDef,
-    DeleteNamespaceResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeregisterInstanceRequestRequestTypeDef,
-    DeregisterInstanceResponseTypeDef,
     DiscoverInstancesRequestRequestTypeDef,
     HttpInstanceSummaryTypeDef,
     DnsRecordTypeDef,
-    SOATypeDef,
-    EmptyResponseMetadataTypeDef,
+    DnsRecordOutputTypeDef,
+    SOAOutputTypeDef,
     GetInstanceRequestRequestTypeDef,
     InstanceTypeDef,
     GetInstancesHealthStatusRequestRequestTypeDef,
-    GetInstancesHealthStatusResponseTypeDef,
     GetNamespaceRequestRequestTypeDef,
     GetOperationRequestRequestTypeDef,
     OperationTypeDef,
     GetServiceRequestRequestTypeDef,
+    HealthCheckConfigOutputTypeDef,
+    HealthCheckCustomConfigOutputTypeDef,
     HttpNamespaceChangeTypeDef,
     HttpPropertiesTypeDef,
     InstanceSummaryTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListInstancesRequestRequestTypeDef,
     NamespaceFilterTypeDef,
     OperationFilterTypeDef,
     OperationSummaryTypeDef,
     ServiceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     SOAChangeTypeDef,
+    SOATypeDef,
     RegisterInstanceRequestRequestTypeDef,
-    RegisterInstanceResponseTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateHttpNamespaceResponseTypeDef,
     UpdateInstanceCustomHealthStatusRequestRequestTypeDef,
+    CreateHttpNamespaceRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    CreateHttpNamespaceResponseTypeDef,
+    CreatePrivateDnsNamespaceResponseTypeDef,
+    CreatePublicDnsNamespaceResponseTypeDef,
+    DeleteNamespaceResponseTypeDef,
+    DeregisterInstanceResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetInstancesHealthStatusResponseTypeDef,
+    RegisterInstanceResponseTypeDef,
+    UpdateHttpNamespaceResponseTypeDef,
     UpdatePrivateDnsNamespaceResponseTypeDef,
     UpdatePublicDnsNamespaceResponseTypeDef,
     UpdateServiceResponseTypeDef,
-    CreateHttpNamespaceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     DiscoverInstancesResponseTypeDef,
     DnsConfigChangeTypeDef,
     DnsConfigTypeDef,
+    DnsConfigOutputTypeDef,
     DnsPropertiesTypeDef,
-    PrivateDnsPropertiesMutableTypeDef,
-    PublicDnsPropertiesMutableTypeDef,
     GetInstanceResponseTypeDef,
     GetOperationResponseTypeDef,
     UpdateHttpNamespaceRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
     ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListNamespacesRequestRequestTypeDef,
     ListOperationsRequestListOperationsPaginateTypeDef,
     ListOperationsRequestRequestTypeDef,
     ListOperationsResponseTypeDef,
     ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PrivateDnsPropertiesMutableChangeTypeDef,
     PublicDnsPropertiesMutableChangeTypeDef,
+    PrivateDnsPropertiesMutableTypeDef,
+    PublicDnsPropertiesMutableTypeDef,
     ServiceChangeTypeDef,
     CreateServiceRequestRequestTypeDef,
     ServiceSummaryTypeDef,
     ServiceTypeDef,
     NamespacePropertiesTypeDef,
-    PrivateDnsNamespacePropertiesTypeDef,
-    PublicDnsNamespacePropertiesTypeDef,
     PrivateDnsNamespacePropertiesChangeTypeDef,
     PublicDnsNamespacePropertiesChangeTypeDef,
+    PrivateDnsNamespacePropertiesTypeDef,
+    PublicDnsNamespacePropertiesTypeDef,
     UpdateServiceRequestRequestTypeDef,
     ListServicesResponseTypeDef,
     CreateServiceResponseTypeDef,
     GetServiceResponseTypeDef,
     NamespaceSummaryTypeDef,
     NamespaceTypeDef,
-    CreatePrivateDnsNamespaceRequestRequestTypeDef,
-    CreatePublicDnsNamespaceRequestRequestTypeDef,
     PrivateDnsNamespaceChangeTypeDef,
     PublicDnsNamespaceChangeTypeDef,
+    CreatePrivateDnsNamespaceRequestRequestTypeDef,
+    CreatePublicDnsNamespaceRequestRequestTypeDef,
     ListNamespacesResponseTypeDef,
     GetNamespaceResponseTypeDef,
     UpdatePrivateDnsNamespaceRequestRequestTypeDef,
     UpdatePublicDnsNamespaceRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-servicediscovery-1.28.0/README.md` & `mypy-boto3-servicediscovery-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-servicediscovery"></a>
 
 # mypy-boto3-servicediscovery
 
 [![PyPI - mypy-boto3-servicediscovery](https://img.shields.io/pypi/v/mypy-boto3-servicediscovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicediscovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicediscovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicediscovery)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-servicediscovery?color=blue)](https://pypistats.org/packages/mypy-boto3-servicediscovery)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicediscovery)](https://pepy.tech/project/mypy-boto3-servicediscovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceDiscovery 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
+[boto3.ServiceDiscovery 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
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
 [mypy-boto3-servicediscovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -316,99 +316,105 @@
 
 `mypy_boto3_servicediscovery.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_servicediscovery.type_defs import (
     TagTypeDef,
-    CreateHttpNamespaceResponseTypeDef,
-    CreatePrivateDnsNamespaceResponseTypeDef,
-    CreatePublicDnsNamespaceResponseTypeDef,
+    ResponseMetadataTypeDef,
     HealthCheckConfigTypeDef,
     HealthCheckCustomConfigTypeDef,
     DeleteNamespaceRequestRequestTypeDef,
-    DeleteNamespaceResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeregisterInstanceRequestRequestTypeDef,
-    DeregisterInstanceResponseTypeDef,
     DiscoverInstancesRequestRequestTypeDef,
     HttpInstanceSummaryTypeDef,
     DnsRecordTypeDef,
-    SOATypeDef,
-    EmptyResponseMetadataTypeDef,
+    DnsRecordOutputTypeDef,
+    SOAOutputTypeDef,
     GetInstanceRequestRequestTypeDef,
     InstanceTypeDef,
     GetInstancesHealthStatusRequestRequestTypeDef,
-    GetInstancesHealthStatusResponseTypeDef,
     GetNamespaceRequestRequestTypeDef,
     GetOperationRequestRequestTypeDef,
     OperationTypeDef,
     GetServiceRequestRequestTypeDef,
+    HealthCheckConfigOutputTypeDef,
+    HealthCheckCustomConfigOutputTypeDef,
     HttpNamespaceChangeTypeDef,
     HttpPropertiesTypeDef,
     InstanceSummaryTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListInstancesRequestRequestTypeDef,
     NamespaceFilterTypeDef,
     OperationFilterTypeDef,
     OperationSummaryTypeDef,
     ServiceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     SOAChangeTypeDef,
+    SOATypeDef,
     RegisterInstanceRequestRequestTypeDef,
-    RegisterInstanceResponseTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateHttpNamespaceResponseTypeDef,
     UpdateInstanceCustomHealthStatusRequestRequestTypeDef,
+    CreateHttpNamespaceRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    CreateHttpNamespaceResponseTypeDef,
+    CreatePrivateDnsNamespaceResponseTypeDef,
+    CreatePublicDnsNamespaceResponseTypeDef,
+    DeleteNamespaceResponseTypeDef,
+    DeregisterInstanceResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetInstancesHealthStatusResponseTypeDef,
+    RegisterInstanceResponseTypeDef,
+    UpdateHttpNamespaceResponseTypeDef,
     UpdatePrivateDnsNamespaceResponseTypeDef,
     UpdatePublicDnsNamespaceResponseTypeDef,
     UpdateServiceResponseTypeDef,
-    CreateHttpNamespaceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     DiscoverInstancesResponseTypeDef,
     DnsConfigChangeTypeDef,
     DnsConfigTypeDef,
+    DnsConfigOutputTypeDef,
     DnsPropertiesTypeDef,
-    PrivateDnsPropertiesMutableTypeDef,
-    PublicDnsPropertiesMutableTypeDef,
     GetInstanceResponseTypeDef,
     GetOperationResponseTypeDef,
     UpdateHttpNamespaceRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
     ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListNamespacesRequestRequestTypeDef,
     ListOperationsRequestListOperationsPaginateTypeDef,
     ListOperationsRequestRequestTypeDef,
     ListOperationsResponseTypeDef,
     ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PrivateDnsPropertiesMutableChangeTypeDef,
     PublicDnsPropertiesMutableChangeTypeDef,
+    PrivateDnsPropertiesMutableTypeDef,
+    PublicDnsPropertiesMutableTypeDef,
     ServiceChangeTypeDef,
     CreateServiceRequestRequestTypeDef,
     ServiceSummaryTypeDef,
     ServiceTypeDef,
     NamespacePropertiesTypeDef,
-    PrivateDnsNamespacePropertiesTypeDef,
-    PublicDnsNamespacePropertiesTypeDef,
     PrivateDnsNamespacePropertiesChangeTypeDef,
     PublicDnsNamespacePropertiesChangeTypeDef,
+    PrivateDnsNamespacePropertiesTypeDef,
+    PublicDnsNamespacePropertiesTypeDef,
     UpdateServiceRequestRequestTypeDef,
     ListServicesResponseTypeDef,
     CreateServiceResponseTypeDef,
     GetServiceResponseTypeDef,
     NamespaceSummaryTypeDef,
     NamespaceTypeDef,
-    CreatePrivateDnsNamespaceRequestRequestTypeDef,
-    CreatePublicDnsNamespaceRequestRequestTypeDef,
     PrivateDnsNamespaceChangeTypeDef,
     PublicDnsNamespaceChangeTypeDef,
+    CreatePrivateDnsNamespaceRequestRequestTypeDef,
+    CreatePublicDnsNamespaceRequestRequestTypeDef,
     ListNamespacesResponseTypeDef,
     GetNamespaceResponseTypeDef,
     UpdatePrivateDnsNamespaceRequestRequestTypeDef,
     UpdatePublicDnsNamespaceRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/__init__.py` & `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/__init__.pyi` & `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/__main__.py` & `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ServiceDiscovery 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ServiceDiscovery 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery\nOther"
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

### Comparing `mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/client.py` & `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/client.pyi` & `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/literals.py` & `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,15 @@
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
@@ -277,26 +278,28 @@
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

### Comparing `mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/literals.pyi` & `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,15 @@
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
@@ -275,26 +276,28 @@
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

### Comparing `mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/paginator.py` & `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 class ListInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listinstancespaginator)
     """
 
     def paginate(
-        self, *, ServiceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServiceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listinstancespaginator)
         """
 
 
@@ -79,15 +79,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listnamespacespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[NamespaceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNamespacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListNamespaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listnamespacespaginator)
         """
 
 
@@ -97,15 +97,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listoperationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OperationFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listoperationspaginator)
         """
 
 
@@ -115,13 +115,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listservicespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ServiceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listservicespaginator)
         """
```

### Comparing `mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/paginator.pyi` & `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 class ListInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listinstancespaginator)
     """
 
     def paginate(
-        self, *, ServiceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServiceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listinstancespaginator)
         """
 
 class ListNamespacesPaginator(Paginator):
@@ -75,15 +75,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listnamespacespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[NamespaceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNamespacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListNamespaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listnamespacespaginator)
         """
 
 class ListOperationsPaginator(Paginator):
@@ -92,15 +92,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listoperationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OperationFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listoperationspaginator)
         """
 
 class ListServicesPaginator(Paginator):
@@ -109,13 +109,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listservicespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ServiceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listservicespaginator)
         """
```

### Comparing `mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/type_defs.py` & `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -37,137 +37,129 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
-    "CreateHttpNamespaceResponseTypeDef",
-    "CreatePrivateDnsNamespaceResponseTypeDef",
-    "CreatePublicDnsNamespaceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "HealthCheckConfigTypeDef",
     "HealthCheckCustomConfigTypeDef",
     "DeleteNamespaceRequestRequestTypeDef",
-    "DeleteNamespaceResponseTypeDef",
     "DeleteServiceRequestRequestTypeDef",
     "DeregisterInstanceRequestRequestTypeDef",
-    "DeregisterInstanceResponseTypeDef",
     "DiscoverInstancesRequestRequestTypeDef",
     "HttpInstanceSummaryTypeDef",
     "DnsRecordTypeDef",
-    "SOATypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "DnsRecordOutputTypeDef",
+    "SOAOutputTypeDef",
     "GetInstanceRequestRequestTypeDef",
     "InstanceTypeDef",
     "GetInstancesHealthStatusRequestRequestTypeDef",
-    "GetInstancesHealthStatusResponseTypeDef",
     "GetNamespaceRequestRequestTypeDef",
     "GetOperationRequestRequestTypeDef",
     "OperationTypeDef",
     "GetServiceRequestRequestTypeDef",
+    "HealthCheckConfigOutputTypeDef",
+    "HealthCheckCustomConfigOutputTypeDef",
     "HttpNamespaceChangeTypeDef",
     "HttpPropertiesTypeDef",
     "InstanceSummaryTypeDef",
-    "ListInstancesRequestListInstancesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "NamespaceFilterTypeDef",
     "OperationFilterTypeDef",
     "OperationSummaryTypeDef",
     "ServiceFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
     "SOAChangeTypeDef",
+    "SOATypeDef",
     "RegisterInstanceRequestRequestTypeDef",
-    "RegisterInstanceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateHttpNamespaceResponseTypeDef",
     "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
+    "CreateHttpNamespaceRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "CreateHttpNamespaceResponseTypeDef",
+    "CreatePrivateDnsNamespaceResponseTypeDef",
+    "CreatePublicDnsNamespaceResponseTypeDef",
+    "DeleteNamespaceResponseTypeDef",
+    "DeregisterInstanceResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetInstancesHealthStatusResponseTypeDef",
+    "RegisterInstanceResponseTypeDef",
+    "UpdateHttpNamespaceResponseTypeDef",
     "UpdatePrivateDnsNamespaceResponseTypeDef",
     "UpdatePublicDnsNamespaceResponseTypeDef",
     "UpdateServiceResponseTypeDef",
-    "CreateHttpNamespaceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "DiscoverInstancesResponseTypeDef",
     "DnsConfigChangeTypeDef",
     "DnsConfigTypeDef",
+    "DnsConfigOutputTypeDef",
     "DnsPropertiesTypeDef",
-    "PrivateDnsPropertiesMutableTypeDef",
-    "PublicDnsPropertiesMutableTypeDef",
     "GetInstanceResponseTypeDef",
     "GetOperationResponseTypeDef",
     "UpdateHttpNamespaceRequestRequestTypeDef",
     "ListInstancesResponseTypeDef",
+    "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
     "ListNamespacesRequestRequestTypeDef",
     "ListOperationsRequestListOperationsPaginateTypeDef",
     "ListOperationsRequestRequestTypeDef",
     "ListOperationsResponseTypeDef",
     "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PrivateDnsPropertiesMutableChangeTypeDef",
     "PublicDnsPropertiesMutableChangeTypeDef",
+    "PrivateDnsPropertiesMutableTypeDef",
+    "PublicDnsPropertiesMutableTypeDef",
     "ServiceChangeTypeDef",
     "CreateServiceRequestRequestTypeDef",
     "ServiceSummaryTypeDef",
     "ServiceTypeDef",
     "NamespacePropertiesTypeDef",
-    "PrivateDnsNamespacePropertiesTypeDef",
-    "PublicDnsNamespacePropertiesTypeDef",
     "PrivateDnsNamespacePropertiesChangeTypeDef",
     "PublicDnsNamespacePropertiesChangeTypeDef",
+    "PrivateDnsNamespacePropertiesTypeDef",
+    "PublicDnsNamespacePropertiesTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "ListServicesResponseTypeDef",
     "CreateServiceResponseTypeDef",
     "GetServiceResponseTypeDef",
     "NamespaceSummaryTypeDef",
     "NamespaceTypeDef",
-    "CreatePrivateDnsNamespaceRequestRequestTypeDef",
-    "CreatePublicDnsNamespaceRequestRequestTypeDef",
     "PrivateDnsNamespaceChangeTypeDef",
     "PublicDnsNamespaceChangeTypeDef",
+    "CreatePrivateDnsNamespaceRequestRequestTypeDef",
+    "CreatePublicDnsNamespaceRequestRequestTypeDef",
     "ListNamespacesResponseTypeDef",
     "GetNamespaceResponseTypeDef",
     "UpdatePrivateDnsNamespaceRequestRequestTypeDef",
     "UpdatePublicDnsNamespaceRequestRequestTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateHttpNamespaceResponseTypeDef = TypedDict(
-    "CreateHttpNamespaceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePrivateDnsNamespaceResponseTypeDef = TypedDict(
-    "CreatePrivateDnsNamespaceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePublicDnsNamespaceResponseTypeDef = TypedDict(
-    "CreatePublicDnsNamespaceResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredHealthCheckConfigTypeDef = TypedDict(
     "_RequiredHealthCheckConfigTypeDef",
     {
         "Type": HealthCheckTypeType,
@@ -178,21 +170,19 @@
     {
         "ResourcePath": str,
         "FailureThreshold": int,
     },
     total=False,
 )
 
-
 class HealthCheckConfigTypeDef(
     _RequiredHealthCheckConfigTypeDef, _OptionalHealthCheckConfigTypeDef
 ):
     pass
 
-
 HealthCheckCustomConfigTypeDef = TypedDict(
     "HealthCheckCustomConfigTypeDef",
     {
         "FailureThreshold": int,
     },
     total=False,
 )
@@ -200,22 +190,14 @@
 DeleteNamespaceRequestRequestTypeDef = TypedDict(
     "DeleteNamespaceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-DeleteNamespaceResponseTypeDef = TypedDict(
-    "DeleteNamespaceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteServiceRequestRequestTypeDef = TypedDict(
     "DeleteServiceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -223,22 +205,14 @@
     "DeregisterInstanceRequestRequestTypeDef",
     {
         "ServiceId": str,
         "InstanceId": str,
     },
 )
 
-DeregisterInstanceResponseTypeDef = TypedDict(
-    "DeregisterInstanceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDiscoverInstancesRequestRequestTypeDef = TypedDict(
     "_RequiredDiscoverInstancesRequestRequestTypeDef",
     {
         "NamespaceName": str,
         "ServiceName": str,
     },
 )
@@ -249,21 +223,19 @@
         "QueryParameters": Mapping[str, str],
         "OptionalParameters": Mapping[str, str],
         "HealthStatus": HealthStatusFilterType,
     },
     total=False,
 )
 
-
 class DiscoverInstancesRequestRequestTypeDef(
     _RequiredDiscoverInstancesRequestRequestTypeDef, _OptionalDiscoverInstancesRequestRequestTypeDef
 ):
     pass
 
-
 HttpInstanceSummaryTypeDef = TypedDict(
     "HttpInstanceSummaryTypeDef",
     {
         "InstanceId": str,
         "NamespaceName": str,
         "ServiceName": str,
         "HealthStatus": HealthStatusType,
@@ -276,25 +248,26 @@
     "DnsRecordTypeDef",
     {
         "Type": RecordTypeType,
         "TTL": int,
     },
 )
 
-SOATypeDef = TypedDict(
-    "SOATypeDef",
+DnsRecordOutputTypeDef = TypedDict(
+    "DnsRecordOutputTypeDef",
     {
+        "Type": RecordTypeType,
         "TTL": int,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+SOAOutputTypeDef = TypedDict(
+    "SOAOutputTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TTL": int,
     },
 )
 
 GetInstanceRequestRequestTypeDef = TypedDict(
     "GetInstanceRequestRequestTypeDef",
     {
         "ServiceId": str,
@@ -313,19 +286,17 @@
     {
         "CreatorRequestId": str,
         "Attributes": Dict[str, str],
     },
     total=False,
 )
 
-
 class InstanceTypeDef(_RequiredInstanceTypeDef, _OptionalInstanceTypeDef):
     pass
 
-
 _RequiredGetInstancesHealthStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetInstancesHealthStatusRequestRequestTypeDef",
     {
         "ServiceId": str,
     },
 )
 _OptionalGetInstancesHealthStatusRequestRequestTypeDef = TypedDict(
@@ -334,31 +305,20 @@
         "Instances": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetInstancesHealthStatusRequestRequestTypeDef(
     _RequiredGetInstancesHealthStatusRequestRequestTypeDef,
     _OptionalGetInstancesHealthStatusRequestRequestTypeDef,
 ):
     pass
 
-
-GetInstancesHealthStatusResponseTypeDef = TypedDict(
-    "GetInstancesHealthStatusResponseTypeDef",
-    {
-        "Status": Dict[str, HealthStatusType],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetNamespaceRequestRequestTypeDef = TypedDict(
     "GetNamespaceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -387,14 +347,42 @@
 GetServiceRequestRequestTypeDef = TypedDict(
     "GetServiceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+_RequiredHealthCheckConfigOutputTypeDef = TypedDict(
+    "_RequiredHealthCheckConfigOutputTypeDef",
+    {
+        "Type": HealthCheckTypeType,
+    },
+)
+_OptionalHealthCheckConfigOutputTypeDef = TypedDict(
+    "_OptionalHealthCheckConfigOutputTypeDef",
+    {
+        "ResourcePath": str,
+        "FailureThreshold": int,
+    },
+    total=False,
+)
+
+class HealthCheckConfigOutputTypeDef(
+    _RequiredHealthCheckConfigOutputTypeDef, _OptionalHealthCheckConfigOutputTypeDef
+):
+    pass
+
+HealthCheckCustomConfigOutputTypeDef = TypedDict(
+    "HealthCheckCustomConfigOutputTypeDef",
+    {
+        "FailureThreshold": int,
+    },
+    total=False,
+)
+
 HttpNamespaceChangeTypeDef = TypedDict(
     "HttpNamespaceChangeTypeDef",
     {
         "Description": str,
     },
 )
 
@@ -411,36 +399,24 @@
     {
         "Id": str,
         "Attributes": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "_RequiredListInstancesRequestListInstancesPaginateTypeDef",
-    {
-        "ServiceId": str,
-    },
-)
-_OptionalListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "_OptionalListInstancesRequestListInstancesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListInstancesRequestListInstancesPaginateTypeDef(
-    _RequiredListInstancesRequestListInstancesPaginateTypeDef,
-    _OptionalListInstancesRequestListInstancesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListInstancesRequestRequestTypeDef = TypedDict(
     "_RequiredListInstancesRequestRequestTypeDef",
     {
         "ServiceId": str,
     },
 )
 _OptionalListInstancesRequestRequestTypeDef = TypedDict(
@@ -448,21 +424,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListInstancesRequestRequestTypeDef(
     _RequiredListInstancesRequestRequestTypeDef, _OptionalListInstancesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredNamespaceFilterTypeDef = TypedDict(
     "_RequiredNamespaceFilterTypeDef",
     {
         "Name": NamespaceFilterNameType,
         "Values": Sequence[str],
     },
 )
@@ -470,19 +444,17 @@
     "_OptionalNamespaceFilterTypeDef",
     {
         "Condition": FilterConditionType,
     },
     total=False,
 )
 
-
 class NamespaceFilterTypeDef(_RequiredNamespaceFilterTypeDef, _OptionalNamespaceFilterTypeDef):
     pass
 
-
 _RequiredOperationFilterTypeDef = TypedDict(
     "_RequiredOperationFilterTypeDef",
     {
         "Name": OperationFilterNameType,
         "Values": Sequence[str],
     },
 )
@@ -490,19 +462,17 @@
     "_OptionalOperationFilterTypeDef",
     {
         "Condition": FilterConditionType,
     },
     total=False,
 )
 
-
 class OperationFilterTypeDef(_RequiredOperationFilterTypeDef, _OptionalOperationFilterTypeDef):
     pass
 
-
 OperationSummaryTypeDef = TypedDict(
     "OperationSummaryTypeDef",
     {
         "Id": str,
         "Status": OperationStatusType,
     },
     total=False,
@@ -519,43 +489,46 @@
     "_OptionalServiceFilterTypeDef",
     {
         "Condition": FilterConditionType,
     },
     total=False,
 )
 
-
 class ServiceFilterTypeDef(_RequiredServiceFilterTypeDef, _OptionalServiceFilterTypeDef):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
 SOAChangeTypeDef = TypedDict(
     "SOAChangeTypeDef",
     {
         "TTL": int,
     },
 )
 
+SOATypeDef = TypedDict(
+    "SOATypeDef",
+    {
+        "TTL": int,
+    },
+)
+
 _RequiredRegisterInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterInstanceRequestRequestTypeDef",
     {
         "ServiceId": str,
         "InstanceId": str,
         "Attributes": Mapping[str, str],
     },
@@ -564,134 +537,167 @@
     "_OptionalRegisterInstanceRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
     },
     total=False,
 )
 
-
 class RegisterInstanceRequestRequestTypeDef(
     _RequiredRegisterInstanceRequestRequestTypeDef, _OptionalRegisterInstanceRequestRequestTypeDef
 ):
     pass
 
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "TagKeys": Sequence[str],
+    },
+)
 
-RegisterInstanceResponseTypeDef = TypedDict(
-    "RegisterInstanceResponseTypeDef",
+UpdateInstanceCustomHealthStatusRequestRequestTypeDef = TypedDict(
+    "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ServiceId": str,
+        "InstanceId": str,
+        "Status": CustomHealthStatusType,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateHttpNamespaceRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Name": str,
+    },
+)
+_OptionalCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateHttpNamespaceRequestRequestTypeDef",
+    {
+        "CreatorRequestId": str,
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+class CreateHttpNamespaceRequestRequestTypeDef(
+    _RequiredCreateHttpNamespaceRequestRequestTypeDef,
+    _OptionalCreateHttpNamespaceRequestRequestTypeDef,
+):
+    pass
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
-        "TagKeys": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
-UpdateHttpNamespaceResponseTypeDef = TypedDict(
-    "UpdateHttpNamespaceResponseTypeDef",
+CreateHttpNamespaceResponseTypeDef = TypedDict(
+    "CreateHttpNamespaceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateInstanceCustomHealthStatusRequestRequestTypeDef = TypedDict(
-    "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
+CreatePrivateDnsNamespaceResponseTypeDef = TypedDict(
+    "CreatePrivateDnsNamespaceResponseTypeDef",
     {
-        "ServiceId": str,
-        "InstanceId": str,
-        "Status": CustomHealthStatusType,
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdatePrivateDnsNamespaceResponseTypeDef = TypedDict(
-    "UpdatePrivateDnsNamespaceResponseTypeDef",
+CreatePublicDnsNamespaceResponseTypeDef = TypedDict(
+    "CreatePublicDnsNamespaceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdatePublicDnsNamespaceResponseTypeDef = TypedDict(
-    "UpdatePublicDnsNamespaceResponseTypeDef",
+DeleteNamespaceResponseTypeDef = TypedDict(
+    "DeleteNamespaceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateServiceResponseTypeDef = TypedDict(
-    "UpdateServiceResponseTypeDef",
+DeregisterInstanceResponseTypeDef = TypedDict(
+    "DeregisterInstanceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateHttpNamespaceRequestRequestTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateHttpNamespaceRequestRequestTypeDef",
+
+GetInstancesHealthStatusResponseTypeDef = TypedDict(
+    "GetInstancesHealthStatusResponseTypeDef",
     {
-        "CreatorRequestId": str,
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
+        "Status": Dict[str, HealthStatusType],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+RegisterInstanceResponseTypeDef = TypedDict(
+    "RegisterInstanceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class CreateHttpNamespaceRequestRequestTypeDef(
-    _RequiredCreateHttpNamespaceRequestRequestTypeDef,
-    _OptionalCreateHttpNamespaceRequestRequestTypeDef,
-):
-    pass
+UpdateHttpNamespaceResponseTypeDef = TypedDict(
+    "UpdateHttpNamespaceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+UpdatePrivateDnsNamespaceResponseTypeDef = TypedDict(
+    "UpdatePrivateDnsNamespaceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+UpdatePublicDnsNamespaceResponseTypeDef = TypedDict(
+    "UpdatePublicDnsNamespaceResponseTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+UpdateServiceResponseTypeDef = TypedDict(
+    "UpdateServiceResponseTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DiscoverInstancesResponseTypeDef = TypedDict(
     "DiscoverInstancesResponseTypeDef",
     {
         "Instances": List[HttpInstanceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DnsConfigChangeTypeDef = TypedDict(
     "DnsConfigChangeTypeDef",
     {
         "DnsRecords": Sequence[DnsRecordTypeDef],
@@ -709,55 +715,57 @@
     {
         "NamespaceId": str,
         "RoutingPolicy": RoutingPolicyType,
     },
     total=False,
 )
 
-
 class DnsConfigTypeDef(_RequiredDnsConfigTypeDef, _OptionalDnsConfigTypeDef):
     pass
 
-
-DnsPropertiesTypeDef = TypedDict(
-    "DnsPropertiesTypeDef",
+_RequiredDnsConfigOutputTypeDef = TypedDict(
+    "_RequiredDnsConfigOutputTypeDef",
     {
-        "HostedZoneId": str,
-        "SOA": SOATypeDef,
+        "DnsRecords": List[DnsRecordOutputTypeDef],
     },
-    total=False,
 )
-
-PrivateDnsPropertiesMutableTypeDef = TypedDict(
-    "PrivateDnsPropertiesMutableTypeDef",
+_OptionalDnsConfigOutputTypeDef = TypedDict(
+    "_OptionalDnsConfigOutputTypeDef",
     {
-        "SOA": SOATypeDef,
+        "NamespaceId": str,
+        "RoutingPolicy": RoutingPolicyType,
     },
+    total=False,
 )
 
-PublicDnsPropertiesMutableTypeDef = TypedDict(
-    "PublicDnsPropertiesMutableTypeDef",
+class DnsConfigOutputTypeDef(_RequiredDnsConfigOutputTypeDef, _OptionalDnsConfigOutputTypeDef):
+    pass
+
+DnsPropertiesTypeDef = TypedDict(
+    "DnsPropertiesTypeDef",
     {
-        "SOA": SOATypeDef,
+        "HostedZoneId": str,
+        "SOA": SOAOutputTypeDef,
     },
+    total=False,
 )
 
 GetInstanceResponseTypeDef = TypedDict(
     "GetInstanceResponseTypeDef",
     {
         "Instance": InstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOperationResponseTypeDef = TypedDict(
     "GetOperationResponseTypeDef",
     {
         "Operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateHttpNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateHttpNamespaceRequestRequestTypeDef",
     {
         "Id": str,
@@ -768,36 +776,54 @@
     "_OptionalUpdateHttpNamespaceRequestRequestTypeDef",
     {
         "UpdaterRequestId": str,
     },
     total=False,
 )
 
-
 class UpdateHttpNamespaceRequestRequestTypeDef(
     _RequiredUpdateHttpNamespaceRequestRequestTypeDef,
     _OptionalUpdateHttpNamespaceRequestRequestTypeDef,
 ):
     pass
 
-
 ListInstancesResponseTypeDef = TypedDict(
     "ListInstancesResponseTypeDef",
     {
         "Instances": List[InstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "_RequiredListInstancesRequestListInstancesPaginateTypeDef",
+    {
+        "ServiceId": str,
+    },
+)
+_OptionalListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "_OptionalListInstancesRequestListInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListInstancesRequestListInstancesPaginateTypeDef(
+    _RequiredListInstancesRequestListInstancesPaginateTypeDef,
+    _OptionalListInstancesRequestListInstancesPaginateTypeDef,
+):
+    pass
+
 ListNamespacesRequestListNamespacesPaginateTypeDef = TypedDict(
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
     {
         "Filters": Sequence[NamespaceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListNamespacesRequestRequestTypeDef = TypedDict(
     "ListNamespacesRequestRequestTypeDef",
     {
@@ -808,15 +834,15 @@
     total=False,
 )
 
 ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
     "ListOperationsRequestListOperationsPaginateTypeDef",
     {
         "Filters": Sequence[OperationFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListOperationsRequestRequestTypeDef = TypedDict(
     "ListOperationsRequestRequestTypeDef",
     {
@@ -828,51 +854,73 @@
 )
 
 ListOperationsResponseTypeDef = TypedDict(
     "ListOperationsResponseTypeDef",
     {
         "Operations": List[OperationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServicesRequestListServicesPaginateTypeDef = TypedDict(
     "ListServicesRequestListServicesPaginateTypeDef",
     {
         "Filters": Sequence[ServiceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[ServiceFilterTypeDef],
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PrivateDnsPropertiesMutableChangeTypeDef = TypedDict(
     "PrivateDnsPropertiesMutableChangeTypeDef",
     {
         "SOA": SOAChangeTypeDef,
     },
 )
 
 PublicDnsPropertiesMutableChangeTypeDef = TypedDict(
     "PublicDnsPropertiesMutableChangeTypeDef",
     {
         "SOA": SOAChangeTypeDef,
     },
 )
 
+PrivateDnsPropertiesMutableTypeDef = TypedDict(
+    "PrivateDnsPropertiesMutableTypeDef",
+    {
+        "SOA": SOATypeDef,
+    },
+)
+
+PublicDnsPropertiesMutableTypeDef = TypedDict(
+    "PublicDnsPropertiesMutableTypeDef",
+    {
+        "SOA": SOATypeDef,
+    },
+)
+
 ServiceChangeTypeDef = TypedDict(
     "ServiceChangeTypeDef",
     {
         "Description": str,
         "DnsConfig": DnsConfigChangeTypeDef,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
     },
@@ -896,51 +944,49 @@
         "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
         "Type": Literal["HTTP"],
     },
     total=False,
 )
 
-
 class CreateServiceRequestRequestTypeDef(
     _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
 ):
     pass
 
-
 ServiceSummaryTypeDef = TypedDict(
     "ServiceSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Type": ServiceTypeType,
         "Description": str,
         "InstanceCount": int,
-        "DnsConfig": DnsConfigTypeDef,
-        "HealthCheckConfig": HealthCheckConfigTypeDef,
-        "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
+        "DnsConfig": DnsConfigOutputTypeDef,
+        "HealthCheckConfig": HealthCheckConfigOutputTypeDef,
+        "HealthCheckCustomConfig": HealthCheckCustomConfigOutputTypeDef,
         "CreateDate": datetime,
     },
     total=False,
 )
 
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "NamespaceId": str,
         "Description": str,
         "InstanceCount": int,
-        "DnsConfig": DnsConfigTypeDef,
+        "DnsConfig": DnsConfigOutputTypeDef,
         "Type": ServiceTypeType,
-        "HealthCheckConfig": HealthCheckConfigTypeDef,
-        "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
+        "HealthCheckConfig": HealthCheckConfigOutputTypeDef,
+        "HealthCheckCustomConfig": HealthCheckCustomConfigOutputTypeDef,
         "CreateDate": datetime,
         "CreatorRequestId": str,
     },
     total=False,
 )
 
 NamespacePropertiesTypeDef = TypedDict(
@@ -948,39 +994,39 @@
     {
         "DnsProperties": DnsPropertiesTypeDef,
         "HttpProperties": HttpPropertiesTypeDef,
     },
     total=False,
 )
 
-PrivateDnsNamespacePropertiesTypeDef = TypedDict(
-    "PrivateDnsNamespacePropertiesTypeDef",
+PrivateDnsNamespacePropertiesChangeTypeDef = TypedDict(
+    "PrivateDnsNamespacePropertiesChangeTypeDef",
     {
-        "DnsProperties": PrivateDnsPropertiesMutableTypeDef,
+        "DnsProperties": PrivateDnsPropertiesMutableChangeTypeDef,
     },
 )
 
-PublicDnsNamespacePropertiesTypeDef = TypedDict(
-    "PublicDnsNamespacePropertiesTypeDef",
+PublicDnsNamespacePropertiesChangeTypeDef = TypedDict(
+    "PublicDnsNamespacePropertiesChangeTypeDef",
     {
-        "DnsProperties": PublicDnsPropertiesMutableTypeDef,
+        "DnsProperties": PublicDnsPropertiesMutableChangeTypeDef,
     },
 )
 
-PrivateDnsNamespacePropertiesChangeTypeDef = TypedDict(
-    "PrivateDnsNamespacePropertiesChangeTypeDef",
+PrivateDnsNamespacePropertiesTypeDef = TypedDict(
+    "PrivateDnsNamespacePropertiesTypeDef",
     {
-        "DnsProperties": PrivateDnsPropertiesMutableChangeTypeDef,
+        "DnsProperties": PrivateDnsPropertiesMutableTypeDef,
     },
 )
 
-PublicDnsNamespacePropertiesChangeTypeDef = TypedDict(
-    "PublicDnsNamespacePropertiesChangeTypeDef",
+PublicDnsNamespacePropertiesTypeDef = TypedDict(
+    "PublicDnsNamespacePropertiesTypeDef",
     {
-        "DnsProperties": PublicDnsPropertiesMutableChangeTypeDef,
+        "DnsProperties": PublicDnsPropertiesMutableTypeDef,
     },
 )
 
 UpdateServiceRequestRequestTypeDef = TypedDict(
     "UpdateServiceRequestRequestTypeDef",
     {
         "Id": str,
@@ -989,31 +1035,31 @@
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "Services": List[ServiceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceResponseTypeDef = TypedDict(
     "GetServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NamespaceSummaryTypeDef = TypedDict(
     "NamespaceSummaryTypeDef",
     {
         "Id": str,
@@ -1040,14 +1086,32 @@
         "Properties": NamespacePropertiesTypeDef,
         "CreateDate": datetime,
         "CreatorRequestId": str,
     },
     total=False,
 )
 
+PrivateDnsNamespaceChangeTypeDef = TypedDict(
+    "PrivateDnsNamespaceChangeTypeDef",
+    {
+        "Description": str,
+        "Properties": PrivateDnsNamespacePropertiesChangeTypeDef,
+    },
+    total=False,
+)
+
+PublicDnsNamespaceChangeTypeDef = TypedDict(
+    "PublicDnsNamespaceChangeTypeDef",
+    {
+        "Description": str,
+        "Properties": PublicDnsNamespacePropertiesChangeTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreatePrivateDnsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePrivateDnsNamespaceRequestRequestTypeDef",
     {
         "Name": str,
         "Vpc": str,
     },
 )
@@ -1058,22 +1122,20 @@
         "Description": str,
         "Tags": Sequence[TagTypeDef],
         "Properties": PrivateDnsNamespacePropertiesTypeDef,
     },
     total=False,
 )
 
-
 class CreatePrivateDnsNamespaceRequestRequestTypeDef(
     _RequiredCreatePrivateDnsNamespaceRequestRequestTypeDef,
     _OptionalCreatePrivateDnsNamespaceRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreatePublicDnsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePublicDnsNamespaceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreatePublicDnsNamespaceRequestRequestTypeDef = TypedDict(
@@ -1083,54 +1145,34 @@
         "Description": str,
         "Tags": Sequence[TagTypeDef],
         "Properties": PublicDnsNamespacePropertiesTypeDef,
     },
     total=False,
 )
 
-
 class CreatePublicDnsNamespaceRequestRequestTypeDef(
     _RequiredCreatePublicDnsNamespaceRequestRequestTypeDef,
     _OptionalCreatePublicDnsNamespaceRequestRequestTypeDef,
 ):
     pass
 
-
-PrivateDnsNamespaceChangeTypeDef = TypedDict(
-    "PrivateDnsNamespaceChangeTypeDef",
-    {
-        "Description": str,
-        "Properties": PrivateDnsNamespacePropertiesChangeTypeDef,
-    },
-    total=False,
-)
-
-PublicDnsNamespaceChangeTypeDef = TypedDict(
-    "PublicDnsNamespaceChangeTypeDef",
-    {
-        "Description": str,
-        "Properties": PublicDnsNamespacePropertiesChangeTypeDef,
-    },
-    total=False,
-)
-
 ListNamespacesResponseTypeDef = TypedDict(
     "ListNamespacesResponseTypeDef",
     {
         "Namespaces": List[NamespaceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNamespaceResponseTypeDef = TypedDict(
     "GetNamespaceResponseTypeDef",
     {
         "Namespace": NamespaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdatePrivateDnsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePrivateDnsNamespaceRequestRequestTypeDef",
     {
         "Id": str,
@@ -1141,22 +1183,20 @@
     "_OptionalUpdatePrivateDnsNamespaceRequestRequestTypeDef",
     {
         "UpdaterRequestId": str,
     },
     total=False,
 )
 
-
 class UpdatePrivateDnsNamespaceRequestRequestTypeDef(
     _RequiredUpdatePrivateDnsNamespaceRequestRequestTypeDef,
     _OptionalUpdatePrivateDnsNamespaceRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdatePublicDnsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePublicDnsNamespaceRequestRequestTypeDef",
     {
         "Id": str,
         "Namespace": PublicDnsNamespaceChangeTypeDef,
     },
 )
@@ -1164,13 +1204,12 @@
     "_OptionalUpdatePublicDnsNamespaceRequestRequestTypeDef",
     {
         "UpdaterRequestId": str,
     },
     total=False,
 )
 
-
 class UpdatePublicDnsNamespaceRequestRequestTypeDef(
     _RequiredUpdatePublicDnsNamespaceRequestRequestTypeDef,
     _OptionalUpdatePublicDnsNamespaceRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery/type_defs.pyi` & `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,136 +37,130 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TagTypeDef",
-    "CreateHttpNamespaceResponseTypeDef",
-    "CreatePrivateDnsNamespaceResponseTypeDef",
-    "CreatePublicDnsNamespaceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "HealthCheckConfigTypeDef",
     "HealthCheckCustomConfigTypeDef",
     "DeleteNamespaceRequestRequestTypeDef",
-    "DeleteNamespaceResponseTypeDef",
     "DeleteServiceRequestRequestTypeDef",
     "DeregisterInstanceRequestRequestTypeDef",
-    "DeregisterInstanceResponseTypeDef",
     "DiscoverInstancesRequestRequestTypeDef",
     "HttpInstanceSummaryTypeDef",
     "DnsRecordTypeDef",
-    "SOATypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "DnsRecordOutputTypeDef",
+    "SOAOutputTypeDef",
     "GetInstanceRequestRequestTypeDef",
     "InstanceTypeDef",
     "GetInstancesHealthStatusRequestRequestTypeDef",
-    "GetInstancesHealthStatusResponseTypeDef",
     "GetNamespaceRequestRequestTypeDef",
     "GetOperationRequestRequestTypeDef",
     "OperationTypeDef",
     "GetServiceRequestRequestTypeDef",
+    "HealthCheckConfigOutputTypeDef",
+    "HealthCheckCustomConfigOutputTypeDef",
     "HttpNamespaceChangeTypeDef",
     "HttpPropertiesTypeDef",
     "InstanceSummaryTypeDef",
-    "ListInstancesRequestListInstancesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "NamespaceFilterTypeDef",
     "OperationFilterTypeDef",
     "OperationSummaryTypeDef",
     "ServiceFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
     "SOAChangeTypeDef",
+    "SOATypeDef",
     "RegisterInstanceRequestRequestTypeDef",
-    "RegisterInstanceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateHttpNamespaceResponseTypeDef",
     "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
+    "CreateHttpNamespaceRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "CreateHttpNamespaceResponseTypeDef",
+    "CreatePrivateDnsNamespaceResponseTypeDef",
+    "CreatePublicDnsNamespaceResponseTypeDef",
+    "DeleteNamespaceResponseTypeDef",
+    "DeregisterInstanceResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetInstancesHealthStatusResponseTypeDef",
+    "RegisterInstanceResponseTypeDef",
+    "UpdateHttpNamespaceResponseTypeDef",
     "UpdatePrivateDnsNamespaceResponseTypeDef",
     "UpdatePublicDnsNamespaceResponseTypeDef",
     "UpdateServiceResponseTypeDef",
-    "CreateHttpNamespaceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "DiscoverInstancesResponseTypeDef",
     "DnsConfigChangeTypeDef",
     "DnsConfigTypeDef",
+    "DnsConfigOutputTypeDef",
     "DnsPropertiesTypeDef",
-    "PrivateDnsPropertiesMutableTypeDef",
-    "PublicDnsPropertiesMutableTypeDef",
     "GetInstanceResponseTypeDef",
     "GetOperationResponseTypeDef",
     "UpdateHttpNamespaceRequestRequestTypeDef",
     "ListInstancesResponseTypeDef",
+    "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
     "ListNamespacesRequestRequestTypeDef",
     "ListOperationsRequestListOperationsPaginateTypeDef",
     "ListOperationsRequestRequestTypeDef",
     "ListOperationsResponseTypeDef",
     "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PrivateDnsPropertiesMutableChangeTypeDef",
     "PublicDnsPropertiesMutableChangeTypeDef",
+    "PrivateDnsPropertiesMutableTypeDef",
+    "PublicDnsPropertiesMutableTypeDef",
     "ServiceChangeTypeDef",
     "CreateServiceRequestRequestTypeDef",
     "ServiceSummaryTypeDef",
     "ServiceTypeDef",
     "NamespacePropertiesTypeDef",
-    "PrivateDnsNamespacePropertiesTypeDef",
-    "PublicDnsNamespacePropertiesTypeDef",
     "PrivateDnsNamespacePropertiesChangeTypeDef",
     "PublicDnsNamespacePropertiesChangeTypeDef",
+    "PrivateDnsNamespacePropertiesTypeDef",
+    "PublicDnsNamespacePropertiesTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "ListServicesResponseTypeDef",
     "CreateServiceResponseTypeDef",
     "GetServiceResponseTypeDef",
     "NamespaceSummaryTypeDef",
     "NamespaceTypeDef",
-    "CreatePrivateDnsNamespaceRequestRequestTypeDef",
-    "CreatePublicDnsNamespaceRequestRequestTypeDef",
     "PrivateDnsNamespaceChangeTypeDef",
     "PublicDnsNamespaceChangeTypeDef",
+    "CreatePrivateDnsNamespaceRequestRequestTypeDef",
+    "CreatePublicDnsNamespaceRequestRequestTypeDef",
     "ListNamespacesResponseTypeDef",
     "GetNamespaceResponseTypeDef",
     "UpdatePrivateDnsNamespaceRequestRequestTypeDef",
     "UpdatePublicDnsNamespaceRequestRequestTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateHttpNamespaceResponseTypeDef = TypedDict(
-    "CreateHttpNamespaceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePrivateDnsNamespaceResponseTypeDef = TypedDict(
-    "CreatePrivateDnsNamespaceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePublicDnsNamespaceResponseTypeDef = TypedDict(
-    "CreatePublicDnsNamespaceResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredHealthCheckConfigTypeDef = TypedDict(
     "_RequiredHealthCheckConfigTypeDef",
     {
         "Type": HealthCheckTypeType,
@@ -177,19 +171,21 @@
     {
         "ResourcePath": str,
         "FailureThreshold": int,
     },
     total=False,
 )
 
+
 class HealthCheckConfigTypeDef(
     _RequiredHealthCheckConfigTypeDef, _OptionalHealthCheckConfigTypeDef
 ):
     pass
 
+
 HealthCheckCustomConfigTypeDef = TypedDict(
     "HealthCheckCustomConfigTypeDef",
     {
         "FailureThreshold": int,
     },
     total=False,
 )
@@ -197,22 +193,14 @@
 DeleteNamespaceRequestRequestTypeDef = TypedDict(
     "DeleteNamespaceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-DeleteNamespaceResponseTypeDef = TypedDict(
-    "DeleteNamespaceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteServiceRequestRequestTypeDef = TypedDict(
     "DeleteServiceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -220,22 +208,14 @@
     "DeregisterInstanceRequestRequestTypeDef",
     {
         "ServiceId": str,
         "InstanceId": str,
     },
 )
 
-DeregisterInstanceResponseTypeDef = TypedDict(
-    "DeregisterInstanceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDiscoverInstancesRequestRequestTypeDef = TypedDict(
     "_RequiredDiscoverInstancesRequestRequestTypeDef",
     {
         "NamespaceName": str,
         "ServiceName": str,
     },
 )
@@ -246,19 +226,21 @@
         "QueryParameters": Mapping[str, str],
         "OptionalParameters": Mapping[str, str],
         "HealthStatus": HealthStatusFilterType,
     },
     total=False,
 )
 
+
 class DiscoverInstancesRequestRequestTypeDef(
     _RequiredDiscoverInstancesRequestRequestTypeDef, _OptionalDiscoverInstancesRequestRequestTypeDef
 ):
     pass
 
+
 HttpInstanceSummaryTypeDef = TypedDict(
     "HttpInstanceSummaryTypeDef",
     {
         "InstanceId": str,
         "NamespaceName": str,
         "ServiceName": str,
         "HealthStatus": HealthStatusType,
@@ -271,25 +253,26 @@
     "DnsRecordTypeDef",
     {
         "Type": RecordTypeType,
         "TTL": int,
     },
 )
 
-SOATypeDef = TypedDict(
-    "SOATypeDef",
+DnsRecordOutputTypeDef = TypedDict(
+    "DnsRecordOutputTypeDef",
     {
+        "Type": RecordTypeType,
         "TTL": int,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+SOAOutputTypeDef = TypedDict(
+    "SOAOutputTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TTL": int,
     },
 )
 
 GetInstanceRequestRequestTypeDef = TypedDict(
     "GetInstanceRequestRequestTypeDef",
     {
         "ServiceId": str,
@@ -308,17 +291,19 @@
     {
         "CreatorRequestId": str,
         "Attributes": Dict[str, str],
     },
     total=False,
 )
 
+
 class InstanceTypeDef(_RequiredInstanceTypeDef, _OptionalInstanceTypeDef):
     pass
 
+
 _RequiredGetInstancesHealthStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetInstancesHealthStatusRequestRequestTypeDef",
     {
         "ServiceId": str,
     },
 )
 _OptionalGetInstancesHealthStatusRequestRequestTypeDef = TypedDict(
@@ -327,28 +312,21 @@
         "Instances": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetInstancesHealthStatusRequestRequestTypeDef(
     _RequiredGetInstancesHealthStatusRequestRequestTypeDef,
     _OptionalGetInstancesHealthStatusRequestRequestTypeDef,
 ):
     pass
 
-GetInstancesHealthStatusResponseTypeDef = TypedDict(
-    "GetInstancesHealthStatusResponseTypeDef",
-    {
-        "Status": Dict[str, HealthStatusType],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetNamespaceRequestRequestTypeDef = TypedDict(
     "GetNamespaceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
@@ -378,14 +356,44 @@
 GetServiceRequestRequestTypeDef = TypedDict(
     "GetServiceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+_RequiredHealthCheckConfigOutputTypeDef = TypedDict(
+    "_RequiredHealthCheckConfigOutputTypeDef",
+    {
+        "Type": HealthCheckTypeType,
+    },
+)
+_OptionalHealthCheckConfigOutputTypeDef = TypedDict(
+    "_OptionalHealthCheckConfigOutputTypeDef",
+    {
+        "ResourcePath": str,
+        "FailureThreshold": int,
+    },
+    total=False,
+)
+
+
+class HealthCheckConfigOutputTypeDef(
+    _RequiredHealthCheckConfigOutputTypeDef, _OptionalHealthCheckConfigOutputTypeDef
+):
+    pass
+
+
+HealthCheckCustomConfigOutputTypeDef = TypedDict(
+    "HealthCheckCustomConfigOutputTypeDef",
+    {
+        "FailureThreshold": int,
+    },
+    total=False,
+)
+
 HttpNamespaceChangeTypeDef = TypedDict(
     "HttpNamespaceChangeTypeDef",
     {
         "Description": str,
     },
 )
 
@@ -402,34 +410,24 @@
     {
         "Id": str,
         "Attributes": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "_RequiredListInstancesRequestListInstancesPaginateTypeDef",
-    {
-        "ServiceId": str,
-    },
-)
-_OptionalListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "_OptionalListInstancesRequestListInstancesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListInstancesRequestListInstancesPaginateTypeDef(
-    _RequiredListInstancesRequestListInstancesPaginateTypeDef,
-    _OptionalListInstancesRequestListInstancesPaginateTypeDef,
-):
-    pass
-
 _RequiredListInstancesRequestRequestTypeDef = TypedDict(
     "_RequiredListInstancesRequestRequestTypeDef",
     {
         "ServiceId": str,
     },
 )
 _OptionalListInstancesRequestRequestTypeDef = TypedDict(
@@ -437,19 +435,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListInstancesRequestRequestTypeDef(
     _RequiredListInstancesRequestRequestTypeDef, _OptionalListInstancesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredNamespaceFilterTypeDef = TypedDict(
     "_RequiredNamespaceFilterTypeDef",
     {
         "Name": NamespaceFilterNameType,
         "Values": Sequence[str],
     },
 )
@@ -457,17 +457,19 @@
     "_OptionalNamespaceFilterTypeDef",
     {
         "Condition": FilterConditionType,
     },
     total=False,
 )
 
+
 class NamespaceFilterTypeDef(_RequiredNamespaceFilterTypeDef, _OptionalNamespaceFilterTypeDef):
     pass
 
+
 _RequiredOperationFilterTypeDef = TypedDict(
     "_RequiredOperationFilterTypeDef",
     {
         "Name": OperationFilterNameType,
         "Values": Sequence[str],
     },
 )
@@ -475,17 +477,19 @@
     "_OptionalOperationFilterTypeDef",
     {
         "Condition": FilterConditionType,
     },
     total=False,
 )
 
+
 class OperationFilterTypeDef(_RequiredOperationFilterTypeDef, _OptionalOperationFilterTypeDef):
     pass
 
+
 OperationSummaryTypeDef = TypedDict(
     "OperationSummaryTypeDef",
     {
         "Id": str,
         "Status": OperationStatusType,
     },
     total=False,
@@ -502,41 +506,48 @@
     "_OptionalServiceFilterTypeDef",
     {
         "Condition": FilterConditionType,
     },
     total=False,
 )
 
+
 class ServiceFilterTypeDef(_RequiredServiceFilterTypeDef, _OptionalServiceFilterTypeDef):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
 SOAChangeTypeDef = TypedDict(
     "SOAChangeTypeDef",
     {
         "TTL": int,
     },
 )
 
+SOATypeDef = TypedDict(
+    "SOATypeDef",
+    {
+        "TTL": int,
+    },
+)
+
 _RequiredRegisterInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterInstanceRequestRequestTypeDef",
     {
         "ServiceId": str,
         "InstanceId": str,
         "Attributes": Mapping[str, str],
     },
@@ -545,130 +556,171 @@
     "_OptionalRegisterInstanceRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
     },
     total=False,
 )
 
+
 class RegisterInstanceRequestRequestTypeDef(
     _RequiredRegisterInstanceRequestRequestTypeDef, _OptionalRegisterInstanceRequestRequestTypeDef
 ):
     pass
 
-RegisterInstanceResponseTypeDef = TypedDict(
-    "RegisterInstanceResponseTypeDef",
+
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceARN": str,
+        "TagKeys": Sequence[str],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+UpdateInstanceCustomHealthStatusRequestRequestTypeDef = TypedDict(
+    "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ServiceId": str,
+        "InstanceId": str,
+        "Status": CustomHealthStatusType,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+_RequiredCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateHttpNamespaceRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateHttpNamespaceRequestRequestTypeDef",
+    {
+        "CreatorRequestId": str,
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateHttpNamespaceRequestRequestTypeDef(
+    _RequiredCreateHttpNamespaceRequestRequestTypeDef,
+    _OptionalCreateHttpNamespaceRequestRequestTypeDef,
+):
+    pass
+
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
-        "TagKeys": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
-UpdateHttpNamespaceResponseTypeDef = TypedDict(
-    "UpdateHttpNamespaceResponseTypeDef",
+CreateHttpNamespaceResponseTypeDef = TypedDict(
+    "CreateHttpNamespaceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateInstanceCustomHealthStatusRequestRequestTypeDef = TypedDict(
-    "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
+CreatePrivateDnsNamespaceResponseTypeDef = TypedDict(
+    "CreatePrivateDnsNamespaceResponseTypeDef",
     {
-        "ServiceId": str,
-        "InstanceId": str,
-        "Status": CustomHealthStatusType,
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdatePrivateDnsNamespaceResponseTypeDef = TypedDict(
-    "UpdatePrivateDnsNamespaceResponseTypeDef",
+CreatePublicDnsNamespaceResponseTypeDef = TypedDict(
+    "CreatePublicDnsNamespaceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdatePublicDnsNamespaceResponseTypeDef = TypedDict(
-    "UpdatePublicDnsNamespaceResponseTypeDef",
+DeleteNamespaceResponseTypeDef = TypedDict(
+    "DeleteNamespaceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateServiceResponseTypeDef = TypedDict(
-    "UpdateServiceResponseTypeDef",
+DeregisterInstanceResponseTypeDef = TypedDict(
+    "DeregisterInstanceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateHttpNamespaceRequestRequestTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateHttpNamespaceRequestRequestTypeDef",
+
+GetInstancesHealthStatusResponseTypeDef = TypedDict(
+    "GetInstancesHealthStatusResponseTypeDef",
     {
-        "CreatorRequestId": str,
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
+        "Status": Dict[str, HealthStatusType],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateHttpNamespaceRequestRequestTypeDef(
-    _RequiredCreateHttpNamespaceRequestRequestTypeDef,
-    _OptionalCreateHttpNamespaceRequestRequestTypeDef,
-):
-    pass
+RegisterInstanceResponseTypeDef = TypedDict(
+    "RegisterInstanceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+UpdateHttpNamespaceResponseTypeDef = TypedDict(
+    "UpdateHttpNamespaceResponseTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+UpdatePrivateDnsNamespaceResponseTypeDef = TypedDict(
+    "UpdatePrivateDnsNamespaceResponseTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePublicDnsNamespaceResponseTypeDef = TypedDict(
+    "UpdatePublicDnsNamespaceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateServiceResponseTypeDef = TypedDict(
+    "UpdateServiceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DiscoverInstancesResponseTypeDef = TypedDict(
     "DiscoverInstancesResponseTypeDef",
     {
         "Instances": List[HttpInstanceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DnsConfigChangeTypeDef = TypedDict(
     "DnsConfigChangeTypeDef",
     {
         "DnsRecords": Sequence[DnsRecordTypeDef],
@@ -686,53 +738,61 @@
     {
         "NamespaceId": str,
         "RoutingPolicy": RoutingPolicyType,
     },
     total=False,
 )
 
+
 class DnsConfigTypeDef(_RequiredDnsConfigTypeDef, _OptionalDnsConfigTypeDef):
     pass
 
-DnsPropertiesTypeDef = TypedDict(
-    "DnsPropertiesTypeDef",
+
+_RequiredDnsConfigOutputTypeDef = TypedDict(
+    "_RequiredDnsConfigOutputTypeDef",
     {
-        "HostedZoneId": str,
-        "SOA": SOATypeDef,
+        "DnsRecords": List[DnsRecordOutputTypeDef],
     },
-    total=False,
 )
-
-PrivateDnsPropertiesMutableTypeDef = TypedDict(
-    "PrivateDnsPropertiesMutableTypeDef",
+_OptionalDnsConfigOutputTypeDef = TypedDict(
+    "_OptionalDnsConfigOutputTypeDef",
     {
-        "SOA": SOATypeDef,
+        "NamespaceId": str,
+        "RoutingPolicy": RoutingPolicyType,
     },
+    total=False,
 )
 
-PublicDnsPropertiesMutableTypeDef = TypedDict(
-    "PublicDnsPropertiesMutableTypeDef",
+
+class DnsConfigOutputTypeDef(_RequiredDnsConfigOutputTypeDef, _OptionalDnsConfigOutputTypeDef):
+    pass
+
+
+DnsPropertiesTypeDef = TypedDict(
+    "DnsPropertiesTypeDef",
     {
-        "SOA": SOATypeDef,
+        "HostedZoneId": str,
+        "SOA": SOAOutputTypeDef,
     },
+    total=False,
 )
 
 GetInstanceResponseTypeDef = TypedDict(
     "GetInstanceResponseTypeDef",
     {
         "Instance": InstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOperationResponseTypeDef = TypedDict(
     "GetOperationResponseTypeDef",
     {
         "Operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateHttpNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateHttpNamespaceRequestRequestTypeDef",
     {
         "Id": str,
@@ -743,34 +803,58 @@
     "_OptionalUpdateHttpNamespaceRequestRequestTypeDef",
     {
         "UpdaterRequestId": str,
     },
     total=False,
 )
 
+
 class UpdateHttpNamespaceRequestRequestTypeDef(
     _RequiredUpdateHttpNamespaceRequestRequestTypeDef,
     _OptionalUpdateHttpNamespaceRequestRequestTypeDef,
 ):
     pass
 
+
 ListInstancesResponseTypeDef = TypedDict(
     "ListInstancesResponseTypeDef",
     {
         "Instances": List[InstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "_RequiredListInstancesRequestListInstancesPaginateTypeDef",
+    {
+        "ServiceId": str,
+    },
+)
+_OptionalListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "_OptionalListInstancesRequestListInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+
+class ListInstancesRequestListInstancesPaginateTypeDef(
+    _RequiredListInstancesRequestListInstancesPaginateTypeDef,
+    _OptionalListInstancesRequestListInstancesPaginateTypeDef,
+):
+    pass
+
+
 ListNamespacesRequestListNamespacesPaginateTypeDef = TypedDict(
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
     {
         "Filters": Sequence[NamespaceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListNamespacesRequestRequestTypeDef = TypedDict(
     "ListNamespacesRequestRequestTypeDef",
     {
@@ -781,15 +865,15 @@
     total=False,
 )
 
 ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
     "ListOperationsRequestListOperationsPaginateTypeDef",
     {
         "Filters": Sequence[OperationFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListOperationsRequestRequestTypeDef = TypedDict(
     "ListOperationsRequestRequestTypeDef",
     {
@@ -801,51 +885,73 @@
 )
 
 ListOperationsResponseTypeDef = TypedDict(
     "ListOperationsResponseTypeDef",
     {
         "Operations": List[OperationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServicesRequestListServicesPaginateTypeDef = TypedDict(
     "ListServicesRequestListServicesPaginateTypeDef",
     {
         "Filters": Sequence[ServiceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[ServiceFilterTypeDef],
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PrivateDnsPropertiesMutableChangeTypeDef = TypedDict(
     "PrivateDnsPropertiesMutableChangeTypeDef",
     {
         "SOA": SOAChangeTypeDef,
     },
 )
 
 PublicDnsPropertiesMutableChangeTypeDef = TypedDict(
     "PublicDnsPropertiesMutableChangeTypeDef",
     {
         "SOA": SOAChangeTypeDef,
     },
 )
 
+PrivateDnsPropertiesMutableTypeDef = TypedDict(
+    "PrivateDnsPropertiesMutableTypeDef",
+    {
+        "SOA": SOATypeDef,
+    },
+)
+
+PublicDnsPropertiesMutableTypeDef = TypedDict(
+    "PublicDnsPropertiesMutableTypeDef",
+    {
+        "SOA": SOATypeDef,
+    },
+)
+
 ServiceChangeTypeDef = TypedDict(
     "ServiceChangeTypeDef",
     {
         "Description": str,
         "DnsConfig": DnsConfigChangeTypeDef,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
     },
@@ -869,49 +975,51 @@
         "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
         "Type": Literal["HTTP"],
     },
     total=False,
 )
 
+
 class CreateServiceRequestRequestTypeDef(
     _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
 ):
     pass
 
+
 ServiceSummaryTypeDef = TypedDict(
     "ServiceSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Type": ServiceTypeType,
         "Description": str,
         "InstanceCount": int,
-        "DnsConfig": DnsConfigTypeDef,
-        "HealthCheckConfig": HealthCheckConfigTypeDef,
-        "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
+        "DnsConfig": DnsConfigOutputTypeDef,
+        "HealthCheckConfig": HealthCheckConfigOutputTypeDef,
+        "HealthCheckCustomConfig": HealthCheckCustomConfigOutputTypeDef,
         "CreateDate": datetime,
     },
     total=False,
 )
 
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "NamespaceId": str,
         "Description": str,
         "InstanceCount": int,
-        "DnsConfig": DnsConfigTypeDef,
+        "DnsConfig": DnsConfigOutputTypeDef,
         "Type": ServiceTypeType,
-        "HealthCheckConfig": HealthCheckConfigTypeDef,
-        "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
+        "HealthCheckConfig": HealthCheckConfigOutputTypeDef,
+        "HealthCheckCustomConfig": HealthCheckCustomConfigOutputTypeDef,
         "CreateDate": datetime,
         "CreatorRequestId": str,
     },
     total=False,
 )
 
 NamespacePropertiesTypeDef = TypedDict(
@@ -919,39 +1027,39 @@
     {
         "DnsProperties": DnsPropertiesTypeDef,
         "HttpProperties": HttpPropertiesTypeDef,
     },
     total=False,
 )
 
-PrivateDnsNamespacePropertiesTypeDef = TypedDict(
-    "PrivateDnsNamespacePropertiesTypeDef",
+PrivateDnsNamespacePropertiesChangeTypeDef = TypedDict(
+    "PrivateDnsNamespacePropertiesChangeTypeDef",
     {
-        "DnsProperties": PrivateDnsPropertiesMutableTypeDef,
+        "DnsProperties": PrivateDnsPropertiesMutableChangeTypeDef,
     },
 )
 
-PublicDnsNamespacePropertiesTypeDef = TypedDict(
-    "PublicDnsNamespacePropertiesTypeDef",
+PublicDnsNamespacePropertiesChangeTypeDef = TypedDict(
+    "PublicDnsNamespacePropertiesChangeTypeDef",
     {
-        "DnsProperties": PublicDnsPropertiesMutableTypeDef,
+        "DnsProperties": PublicDnsPropertiesMutableChangeTypeDef,
     },
 )
 
-PrivateDnsNamespacePropertiesChangeTypeDef = TypedDict(
-    "PrivateDnsNamespacePropertiesChangeTypeDef",
+PrivateDnsNamespacePropertiesTypeDef = TypedDict(
+    "PrivateDnsNamespacePropertiesTypeDef",
     {
-        "DnsProperties": PrivateDnsPropertiesMutableChangeTypeDef,
+        "DnsProperties": PrivateDnsPropertiesMutableTypeDef,
     },
 )
 
-PublicDnsNamespacePropertiesChangeTypeDef = TypedDict(
-    "PublicDnsNamespacePropertiesChangeTypeDef",
+PublicDnsNamespacePropertiesTypeDef = TypedDict(
+    "PublicDnsNamespacePropertiesTypeDef",
     {
-        "DnsProperties": PublicDnsPropertiesMutableChangeTypeDef,
+        "DnsProperties": PublicDnsPropertiesMutableTypeDef,
     },
 )
 
 UpdateServiceRequestRequestTypeDef = TypedDict(
     "UpdateServiceRequestRequestTypeDef",
     {
         "Id": str,
@@ -960,31 +1068,31 @@
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "Services": List[ServiceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceResponseTypeDef = TypedDict(
     "GetServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NamespaceSummaryTypeDef = TypedDict(
     "NamespaceSummaryTypeDef",
     {
         "Id": str,
@@ -1011,14 +1119,32 @@
         "Properties": NamespacePropertiesTypeDef,
         "CreateDate": datetime,
         "CreatorRequestId": str,
     },
     total=False,
 )
 
+PrivateDnsNamespaceChangeTypeDef = TypedDict(
+    "PrivateDnsNamespaceChangeTypeDef",
+    {
+        "Description": str,
+        "Properties": PrivateDnsNamespacePropertiesChangeTypeDef,
+    },
+    total=False,
+)
+
+PublicDnsNamespaceChangeTypeDef = TypedDict(
+    "PublicDnsNamespaceChangeTypeDef",
+    {
+        "Description": str,
+        "Properties": PublicDnsNamespacePropertiesChangeTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreatePrivateDnsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePrivateDnsNamespaceRequestRequestTypeDef",
     {
         "Name": str,
         "Vpc": str,
     },
 )
@@ -1029,20 +1155,22 @@
         "Description": str,
         "Tags": Sequence[TagTypeDef],
         "Properties": PrivateDnsNamespacePropertiesTypeDef,
     },
     total=False,
 )
 
+
 class CreatePrivateDnsNamespaceRequestRequestTypeDef(
     _RequiredCreatePrivateDnsNamespaceRequestRequestTypeDef,
     _OptionalCreatePrivateDnsNamespaceRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreatePublicDnsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePublicDnsNamespaceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreatePublicDnsNamespaceRequestRequestTypeDef = TypedDict(
@@ -1052,52 +1180,36 @@
         "Description": str,
         "Tags": Sequence[TagTypeDef],
         "Properties": PublicDnsNamespacePropertiesTypeDef,
     },
     total=False,
 )
 
+
 class CreatePublicDnsNamespaceRequestRequestTypeDef(
     _RequiredCreatePublicDnsNamespaceRequestRequestTypeDef,
     _OptionalCreatePublicDnsNamespaceRequestRequestTypeDef,
 ):
     pass
 
-PrivateDnsNamespaceChangeTypeDef = TypedDict(
-    "PrivateDnsNamespaceChangeTypeDef",
-    {
-        "Description": str,
-        "Properties": PrivateDnsNamespacePropertiesChangeTypeDef,
-    },
-    total=False,
-)
-
-PublicDnsNamespaceChangeTypeDef = TypedDict(
-    "PublicDnsNamespaceChangeTypeDef",
-    {
-        "Description": str,
-        "Properties": PublicDnsNamespacePropertiesChangeTypeDef,
-    },
-    total=False,
-)
 
 ListNamespacesResponseTypeDef = TypedDict(
     "ListNamespacesResponseTypeDef",
     {
         "Namespaces": List[NamespaceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNamespaceResponseTypeDef = TypedDict(
     "GetNamespaceResponseTypeDef",
     {
         "Namespace": NamespaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdatePrivateDnsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePrivateDnsNamespaceRequestRequestTypeDef",
     {
         "Id": str,
@@ -1108,20 +1220,22 @@
     "_OptionalUpdatePrivateDnsNamespaceRequestRequestTypeDef",
     {
         "UpdaterRequestId": str,
     },
     total=False,
 )
 
+
 class UpdatePrivateDnsNamespaceRequestRequestTypeDef(
     _RequiredUpdatePrivateDnsNamespaceRequestRequestTypeDef,
     _OptionalUpdatePrivateDnsNamespaceRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdatePublicDnsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePublicDnsNamespaceRequestRequestTypeDef",
     {
         "Id": str,
         "Namespace": PublicDnsNamespaceChangeTypeDef,
     },
 )
@@ -1129,12 +1243,13 @@
     "_OptionalUpdatePublicDnsNamespaceRequestRequestTypeDef",
     {
         "UpdaterRequestId": str,
     },
     total=False,
 )
 
+
 class UpdatePublicDnsNamespaceRequestRequestTypeDef(
     _RequiredUpdatePublicDnsNamespaceRequestRequestTypeDef,
     _OptionalUpdatePublicDnsNamespaceRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery.egg-info/PKG-INFO` & `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicediscovery
-Version: 1.28.0
-Summary: Type annotations for boto3.ServiceDiscovery 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ServiceDiscovery 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-servicediscovery"></a>
 
 # mypy-boto3-servicediscovery
 
 [![PyPI - mypy-boto3-servicediscovery](https://img.shields.io/pypi/v/mypy-boto3-servicediscovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicediscovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicediscovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicediscovery)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-servicediscovery?color=blue)](https://pypistats.org/packages/mypy-boto3-servicediscovery)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicediscovery)](https://pepy.tech/project/mypy-boto3-servicediscovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceDiscovery 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
+[boto3.ServiceDiscovery 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
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
 [mypy-boto3-servicediscovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -348,99 +348,105 @@
 
 `mypy_boto3_servicediscovery.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_servicediscovery.type_defs import (
     TagTypeDef,
-    CreateHttpNamespaceResponseTypeDef,
-    CreatePrivateDnsNamespaceResponseTypeDef,
-    CreatePublicDnsNamespaceResponseTypeDef,
+    ResponseMetadataTypeDef,
     HealthCheckConfigTypeDef,
     HealthCheckCustomConfigTypeDef,
     DeleteNamespaceRequestRequestTypeDef,
-    DeleteNamespaceResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeregisterInstanceRequestRequestTypeDef,
-    DeregisterInstanceResponseTypeDef,
     DiscoverInstancesRequestRequestTypeDef,
     HttpInstanceSummaryTypeDef,
     DnsRecordTypeDef,
-    SOATypeDef,
-    EmptyResponseMetadataTypeDef,
+    DnsRecordOutputTypeDef,
+    SOAOutputTypeDef,
     GetInstanceRequestRequestTypeDef,
     InstanceTypeDef,
     GetInstancesHealthStatusRequestRequestTypeDef,
-    GetInstancesHealthStatusResponseTypeDef,
     GetNamespaceRequestRequestTypeDef,
     GetOperationRequestRequestTypeDef,
     OperationTypeDef,
     GetServiceRequestRequestTypeDef,
+    HealthCheckConfigOutputTypeDef,
+    HealthCheckCustomConfigOutputTypeDef,
     HttpNamespaceChangeTypeDef,
     HttpPropertiesTypeDef,
     InstanceSummaryTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListInstancesRequestRequestTypeDef,
     NamespaceFilterTypeDef,
     OperationFilterTypeDef,
     OperationSummaryTypeDef,
     ServiceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     SOAChangeTypeDef,
+    SOATypeDef,
     RegisterInstanceRequestRequestTypeDef,
-    RegisterInstanceResponseTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateHttpNamespaceResponseTypeDef,
     UpdateInstanceCustomHealthStatusRequestRequestTypeDef,
+    CreateHttpNamespaceRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    CreateHttpNamespaceResponseTypeDef,
+    CreatePrivateDnsNamespaceResponseTypeDef,
+    CreatePublicDnsNamespaceResponseTypeDef,
+    DeleteNamespaceResponseTypeDef,
+    DeregisterInstanceResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetInstancesHealthStatusResponseTypeDef,
+    RegisterInstanceResponseTypeDef,
+    UpdateHttpNamespaceResponseTypeDef,
     UpdatePrivateDnsNamespaceResponseTypeDef,
     UpdatePublicDnsNamespaceResponseTypeDef,
     UpdateServiceResponseTypeDef,
-    CreateHttpNamespaceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     DiscoverInstancesResponseTypeDef,
     DnsConfigChangeTypeDef,
     DnsConfigTypeDef,
+    DnsConfigOutputTypeDef,
     DnsPropertiesTypeDef,
-    PrivateDnsPropertiesMutableTypeDef,
-    PublicDnsPropertiesMutableTypeDef,
     GetInstanceResponseTypeDef,
     GetOperationResponseTypeDef,
     UpdateHttpNamespaceRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
     ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListNamespacesRequestRequestTypeDef,
     ListOperationsRequestListOperationsPaginateTypeDef,
     ListOperationsRequestRequestTypeDef,
     ListOperationsResponseTypeDef,
     ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PrivateDnsPropertiesMutableChangeTypeDef,
     PublicDnsPropertiesMutableChangeTypeDef,
+    PrivateDnsPropertiesMutableTypeDef,
+    PublicDnsPropertiesMutableTypeDef,
     ServiceChangeTypeDef,
     CreateServiceRequestRequestTypeDef,
     ServiceSummaryTypeDef,
     ServiceTypeDef,
     NamespacePropertiesTypeDef,
-    PrivateDnsNamespacePropertiesTypeDef,
-    PublicDnsNamespacePropertiesTypeDef,
     PrivateDnsNamespacePropertiesChangeTypeDef,
     PublicDnsNamespacePropertiesChangeTypeDef,
+    PrivateDnsNamespacePropertiesTypeDef,
+    PublicDnsNamespacePropertiesTypeDef,
     UpdateServiceRequestRequestTypeDef,
     ListServicesResponseTypeDef,
     CreateServiceResponseTypeDef,
     GetServiceResponseTypeDef,
     NamespaceSummaryTypeDef,
     NamespaceTypeDef,
-    CreatePrivateDnsNamespaceRequestRequestTypeDef,
-    CreatePublicDnsNamespaceRequestRequestTypeDef,
     PrivateDnsNamespaceChangeTypeDef,
     PublicDnsNamespaceChangeTypeDef,
+    CreatePrivateDnsNamespaceRequestRequestTypeDef,
+    CreatePublicDnsNamespaceRequestRequestTypeDef,
     ListNamespacesResponseTypeDef,
     GetNamespaceResponseTypeDef,
     UpdatePrivateDnsNamespaceRequestRequestTypeDef,
     UpdatePublicDnsNamespaceRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-servicediscovery-1.28.0/mypy_boto3_servicediscovery.egg-info/SOURCES.txt` & `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.0/setup.py` & `mypy-boto3-servicediscovery-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-servicediscovery",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_servicediscovery"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ServiceDiscovery 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ServiceDiscovery 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

