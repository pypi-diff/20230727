# Comparing `tmp/mypy-boto3-appmesh-1.28.0.tar.gz` & `tmp/mypy-boto3-appmesh-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appmesh-1.28.0.tar", last modified: Thu Jul  6 20:58:58 2023, max compression
+gzip compressed data, was "mypy-boto3-appmesh-1.28.12.tar", last modified: Thu Jul 27 05:34:18 2023, max compression
```

## Comparing `mypy-boto3-appmesh-1.28.0.tar` & `mypy-boto3-appmesh-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.750221 mypy-boto3-appmesh-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:33:28.000000 mypy-boto3-appmesh-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22431 2023-07-06 20:58:58.746221 mypy-boto3-appmesh-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20946 2023-07-06 20:33:28.000000 mypy-boto3-appmesh-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.742220 mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-06 20:33:28.000000 mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-06 20:33:28.000000 mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 20:33:28.000000 mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30229 2023-07-06 20:33:28.000000 mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30176 2023-07-06 20:33:28.000000 mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-07-06 20:33:28.000000 mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-07-06 20:33:28.000000 mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-07-06 20:33:28.000000 mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-07-06 20:33:28.000000 mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:33:28.000000 mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    80486 2023-07-06 20:33:32.000000 mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    80335 2023-07-06 20:33:31.000000 mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:33:28.000000 mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.746221 mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22431 2023-07-06 20:58:58.000000 mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-06 20:58:58.000000 mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:58.000000 mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:58.000000 mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:58:58.000000 mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 20:58:58.000000 mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:58:58.750221 mypy-boto3-appmesh-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-06 20:33:28.000000 mypy-boto3-appmesh-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.500577 mypy-boto3-appmesh-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27313 2023-07-27 05:34:18.500577 mypy-boto3-appmesh-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25826 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.496577 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30229 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30176 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   122164 2023-07-27 05:17:31.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121945 2023-07-27 05:17:30.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.500577 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27313 2023-07-27 05:34:18.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-27 05:34:18.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:18.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:34:18.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:18.500577 mypy-boto3-appmesh-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/setup.py
```

### Comparing `mypy-boto3-appmesh-1.28.0/LICENSE` & `mypy-boto3-appmesh-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.0/PKG-INFO` & `mypy-boto3-appmesh-1.28.12/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appmesh
-Version: 1.28.0
-Summary: Type annotations for boto3.AppMesh 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AppMesh 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-appmesh"></a>
 
 # mypy-boto3-appmesh
 
 [![PyPI - mypy-boto3-appmesh](https://img.shields.io/pypi/v/mypy-boto3-appmesh.svg?color=blue)](https://pypi.org/project/mypy-boto3-appmesh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appmesh.svg?color=blue)](https://pypi.org/project/mypy-boto3-appmesh)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appmesh?color=blue)](https://pypistats.org/packages/mypy-boto3-appmesh)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appmesh)](https://pepy.tech/project/mypy-boto3-appmesh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppMesh 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
+[boto3.AppMesh 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
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
 [mypy-boto3-appmesh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,15 +371,18 @@
 ### Typed dictionaries
 
 `mypy_boto3_appmesh.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appmesh.type_defs import (
+    AwsCloudMapInstanceAttributeOutputTypeDef,
     AwsCloudMapInstanceAttributeTypeDef,
+    ListenerTlsFileCertificateOutputTypeDef,
+    ListenerTlsSdsCertificateOutputTypeDef,
     ListenerTlsFileCertificateTypeDef,
     ListenerTlsSdsCertificateTypeDef,
     TagRefTypeDef,
     DeleteGatewayRouteInputRequestTypeDef,
     DeleteMeshInputRequestTypeDef,
     DeleteRouteInputRequestTypeDef,
     DeleteVirtualGatewayInputRequestTypeDef,
@@ -389,226 +392,343 @@
     DescribeGatewayRouteInputRequestTypeDef,
     DescribeMeshInputRequestTypeDef,
     DescribeRouteInputRequestTypeDef,
     DescribeVirtualGatewayInputRequestTypeDef,
     DescribeVirtualNodeInputRequestTypeDef,
     DescribeVirtualRouterInputRequestTypeDef,
     DescribeVirtualServiceInputRequestTypeDef,
+    DnsServiceDiscoveryOutputTypeDef,
     DnsServiceDiscoveryTypeDef,
+    DurationOutputTypeDef,
     DurationTypeDef,
+    EgressFilterOutputTypeDef,
     EgressFilterTypeDef,
     GatewayRouteStatusTypeDef,
     ResourceMetadataTypeDef,
+    GatewayRouteHostnameMatchOutputTypeDef,
     GatewayRouteHostnameMatchTypeDef,
+    GatewayRouteHostnameRewriteOutputTypeDef,
     GatewayRouteHostnameRewriteTypeDef,
     GatewayRouteRefTypeDef,
+    GatewayRouteVirtualServiceOutputTypeDef,
     GatewayRouteVirtualServiceTypeDef,
+    MatchRangeOutputTypeDef,
     MatchRangeTypeDef,
+    WeightedTargetOutputTypeDef,
     WeightedTargetTypeDef,
+    HealthCheckPolicyOutputTypeDef,
     HealthCheckPolicyTypeDef,
+    HttpPathMatchOutputTypeDef,
     HttpPathMatchTypeDef,
+    HttpGatewayRoutePathRewriteOutputTypeDef,
     HttpGatewayRoutePathRewriteTypeDef,
+    HttpGatewayRoutePrefixRewriteOutputTypeDef,
     HttpGatewayRoutePrefixRewriteTypeDef,
+    QueryParameterMatchOutputTypeDef,
     QueryParameterMatchTypeDef,
+    JsonFormatRefOutputTypeDef,
     JsonFormatRefTypeDef,
     ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
     ListGatewayRoutesInputRequestTypeDef,
     ListMeshesInputListMeshesPaginateTypeDef,
     ListMeshesInputRequestTypeDef,
     MeshRefTypeDef,
     ListRoutesInputListRoutesPaginateTypeDef,
     ListRoutesInputRequestTypeDef,
     RouteRefTypeDef,
     ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    TagRefOutputTypeDef,
     ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
     ListVirtualGatewaysInputRequestTypeDef,
     VirtualGatewayRefTypeDef,
     ListVirtualNodesInputListVirtualNodesPaginateTypeDef,
     ListVirtualNodesInputRequestTypeDef,
     VirtualNodeRefTypeDef,
     ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
     ListVirtualRoutersInputRequestTypeDef,
     VirtualRouterRefTypeDef,
     ListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     ListVirtualServicesInputRequestTypeDef,
     VirtualServiceRefTypeDef,
+    PortMappingOutputTypeDef,
+    ListenerTlsAcmCertificateOutputTypeDef,
     ListenerTlsAcmCertificateTypeDef,
+    TlsValidationContextFileTrustOutputTypeDef,
+    TlsValidationContextSdsTrustOutputTypeDef,
     TlsValidationContextFileTrustTypeDef,
     TlsValidationContextSdsTrustTypeDef,
     PortMappingTypeDef,
     MeshStatusTypeDef,
+    MeshServiceDiscoveryOutputTypeDef,
     MeshServiceDiscoveryTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     RouteStatusTypeDef,
+    SubjectAlternativeNameMatchersOutputTypeDef,
     SubjectAlternativeNameMatchersTypeDef,
+    TcpRouteMatchOutputTypeDef,
     TcpRouteMatchTypeDef,
+    TlsValidationContextAcmTrustOutputTypeDef,
     TlsValidationContextAcmTrustTypeDef,
     UntagResourceInputRequestTypeDef,
+    VirtualGatewayListenerTlsFileCertificateOutputTypeDef,
+    VirtualGatewayListenerTlsSdsCertificateOutputTypeDef,
     VirtualGatewayListenerTlsFileCertificateTypeDef,
     VirtualGatewayListenerTlsSdsCertificateTypeDef,
+    VirtualGatewayGrpcConnectionPoolOutputTypeDef,
+    VirtualGatewayHttp2ConnectionPoolOutputTypeDef,
+    VirtualGatewayHttpConnectionPoolOutputTypeDef,
     VirtualGatewayGrpcConnectionPoolTypeDef,
     VirtualGatewayHttp2ConnectionPoolTypeDef,
     VirtualGatewayHttpConnectionPoolTypeDef,
     VirtualGatewayStatusTypeDef,
+    VirtualGatewayHealthCheckPolicyOutputTypeDef,
     VirtualGatewayHealthCheckPolicyTypeDef,
+    VirtualGatewayPortMappingOutputTypeDef,
+    VirtualGatewayListenerTlsAcmCertificateOutputTypeDef,
     VirtualGatewayListenerTlsAcmCertificateTypeDef,
+    VirtualGatewayTlsValidationContextFileTrustOutputTypeDef,
+    VirtualGatewayTlsValidationContextSdsTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextFileTrustTypeDef,
     VirtualGatewayTlsValidationContextSdsTrustTypeDef,
     VirtualGatewayPortMappingTypeDef,
+    VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextAcmTrustTypeDef,
+    VirtualNodeGrpcConnectionPoolOutputTypeDef,
+    VirtualNodeHttp2ConnectionPoolOutputTypeDef,
+    VirtualNodeHttpConnectionPoolOutputTypeDef,
+    VirtualNodeTcpConnectionPoolOutputTypeDef,
     VirtualNodeGrpcConnectionPoolTypeDef,
     VirtualNodeHttp2ConnectionPoolTypeDef,
     VirtualNodeHttpConnectionPoolTypeDef,
     VirtualNodeTcpConnectionPoolTypeDef,
     VirtualNodeStatusTypeDef,
+    VirtualNodeServiceProviderOutputTypeDef,
     VirtualNodeServiceProviderTypeDef,
     VirtualRouterStatusTypeDef,
+    VirtualRouterServiceProviderOutputTypeDef,
     VirtualRouterServiceProviderTypeDef,
     VirtualServiceStatusTypeDef,
+    AwsCloudMapServiceDiscoveryOutputTypeDef,
     AwsCloudMapServiceDiscoveryTypeDef,
+    ClientTlsCertificateOutputTypeDef,
     ClientTlsCertificateTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    GrpcRetryPolicyOutputTypeDef,
+    GrpcTimeoutOutputTypeDef,
+    HttpRetryPolicyOutputTypeDef,
+    HttpTimeoutOutputTypeDef,
+    OutlierDetectionOutputTypeDef,
+    TcpTimeoutOutputTypeDef,
     GrpcRetryPolicyTypeDef,
     GrpcTimeoutTypeDef,
     HttpRetryPolicyTypeDef,
     HttpTimeoutTypeDef,
     OutlierDetectionTypeDef,
     TcpTimeoutTypeDef,
+    GrpcGatewayRouteRewriteOutputTypeDef,
     GrpcGatewayRouteRewriteTypeDef,
     ListGatewayRoutesOutputTypeDef,
+    GatewayRouteTargetOutputTypeDef,
     GatewayRouteTargetTypeDef,
+    GrpcMetadataMatchMethodOutputTypeDef,
+    GrpcRouteMetadataMatchMethodOutputTypeDef,
+    HeaderMatchMethodOutputTypeDef,
     GrpcMetadataMatchMethodTypeDef,
     GrpcRouteMetadataMatchMethodTypeDef,
     HeaderMatchMethodTypeDef,
+    GrpcRouteActionOutputTypeDef,
+    HttpRouteActionOutputTypeDef,
+    TcpRouteActionOutputTypeDef,
     GrpcRouteActionTypeDef,
     HttpRouteActionTypeDef,
     TcpRouteActionTypeDef,
+    HttpGatewayRouteRewriteOutputTypeDef,
     HttpGatewayRouteRewriteTypeDef,
+    HttpQueryParameterOutputTypeDef,
     HttpQueryParameterTypeDef,
+    LoggingFormatOutputTypeDef,
     LoggingFormatTypeDef,
     ListMeshesOutputTypeDef,
     ListRoutesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListVirtualGatewaysOutputTypeDef,
     ListVirtualNodesOutputTypeDef,
     ListVirtualRoutersOutputTypeDef,
     ListVirtualServicesOutputTypeDef,
+    VirtualRouterListenerOutputTypeDef,
+    ListenerTlsCertificateOutputTypeDef,
     ListenerTlsCertificateTypeDef,
+    ListenerTlsValidationContextTrustOutputTypeDef,
     ListenerTlsValidationContextTrustTypeDef,
     VirtualRouterListenerTypeDef,
+    MeshSpecOutputTypeDef,
     MeshSpecTypeDef,
+    SubjectAlternativeNamesOutputTypeDef,
     SubjectAlternativeNamesTypeDef,
+    TlsValidationContextTrustOutputTypeDef,
     TlsValidationContextTrustTypeDef,
+    VirtualGatewayClientTlsCertificateOutputTypeDef,
     VirtualGatewayClientTlsCertificateTypeDef,
+    VirtualGatewayConnectionPoolOutputTypeDef,
     VirtualGatewayConnectionPoolTypeDef,
+    VirtualGatewayListenerTlsCertificateOutputTypeDef,
     VirtualGatewayListenerTlsCertificateTypeDef,
+    VirtualGatewayListenerTlsValidationContextTrustOutputTypeDef,
     VirtualGatewayListenerTlsValidationContextTrustTypeDef,
+    VirtualGatewayTlsValidationContextTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextTrustTypeDef,
+    VirtualNodeConnectionPoolOutputTypeDef,
     VirtualNodeConnectionPoolTypeDef,
+    VirtualServiceProviderOutputTypeDef,
     VirtualServiceProviderTypeDef,
+    ServiceDiscoveryOutputTypeDef,
     ServiceDiscoveryTypeDef,
+    ListenerTimeoutOutputTypeDef,
     ListenerTimeoutTypeDef,
+    GrpcGatewayRouteActionOutputTypeDef,
     GrpcGatewayRouteActionTypeDef,
+    GrpcGatewayRouteMetadataOutputTypeDef,
+    GrpcRouteMetadataOutputTypeDef,
+    HttpGatewayRouteHeaderOutputTypeDef,
+    HttpRouteHeaderOutputTypeDef,
     GrpcGatewayRouteMetadataTypeDef,
     GrpcRouteMetadataTypeDef,
     HttpGatewayRouteHeaderTypeDef,
     HttpRouteHeaderTypeDef,
+    TcpRouteOutputTypeDef,
     TcpRouteTypeDef,
+    HttpGatewayRouteActionOutputTypeDef,
     HttpGatewayRouteActionTypeDef,
+    FileAccessLogOutputTypeDef,
+    VirtualGatewayFileAccessLogOutputTypeDef,
     FileAccessLogTypeDef,
     VirtualGatewayFileAccessLogTypeDef,
+    VirtualRouterSpecOutputTypeDef,
     VirtualRouterSpecTypeDef,
-    CreateMeshInputRequestTypeDef,
     MeshDataTypeDef,
+    CreateMeshInputRequestTypeDef,
     UpdateMeshInputRequestTypeDef,
+    ListenerTlsValidationContextOutputTypeDef,
     ListenerTlsValidationContextTypeDef,
+    TlsValidationContextOutputTypeDef,
     TlsValidationContextTypeDef,
+    VirtualGatewayListenerTlsValidationContextOutputTypeDef,
     VirtualGatewayListenerTlsValidationContextTypeDef,
+    VirtualGatewayTlsValidationContextOutputTypeDef,
     VirtualGatewayTlsValidationContextTypeDef,
+    VirtualServiceSpecOutputTypeDef,
     VirtualServiceSpecTypeDef,
+    GrpcGatewayRouteMatchOutputTypeDef,
+    GrpcRouteMatchOutputTypeDef,
+    HttpGatewayRouteMatchOutputTypeDef,
+    HttpRouteMatchOutputTypeDef,
     GrpcGatewayRouteMatchTypeDef,
     GrpcRouteMatchTypeDef,
     HttpGatewayRouteMatchTypeDef,
     HttpRouteMatchTypeDef,
+    AccessLogOutputTypeDef,
+    VirtualGatewayAccessLogOutputTypeDef,
     AccessLogTypeDef,
     VirtualGatewayAccessLogTypeDef,
+    VirtualRouterDataTypeDef,
     CreateVirtualRouterInputRequestTypeDef,
     UpdateVirtualRouterInputRequestTypeDef,
-    VirtualRouterDataTypeDef,
     CreateMeshOutputTypeDef,
     DeleteMeshOutputTypeDef,
     DescribeMeshOutputTypeDef,
     UpdateMeshOutputTypeDef,
+    ListenerTlsOutputTypeDef,
     ListenerTlsTypeDef,
+    ClientPolicyTlsOutputTypeDef,
     ClientPolicyTlsTypeDef,
+    VirtualGatewayListenerTlsOutputTypeDef,
     VirtualGatewayListenerTlsTypeDef,
+    VirtualGatewayClientPolicyTlsOutputTypeDef,
     VirtualGatewayClientPolicyTlsTypeDef,
+    VirtualServiceDataTypeDef,
     CreateVirtualServiceInputRequestTypeDef,
     UpdateVirtualServiceInputRequestTypeDef,
-    VirtualServiceDataTypeDef,
+    GrpcGatewayRouteOutputTypeDef,
+    GrpcRouteOutputTypeDef,
+    HttpGatewayRouteOutputTypeDef,
+    HttpRouteOutputTypeDef,
     GrpcGatewayRouteTypeDef,
     GrpcRouteTypeDef,
     HttpGatewayRouteTypeDef,
     HttpRouteTypeDef,
+    LoggingOutputTypeDef,
+    VirtualGatewayLoggingOutputTypeDef,
     LoggingTypeDef,
     VirtualGatewayLoggingTypeDef,
     CreateVirtualRouterOutputTypeDef,
     DeleteVirtualRouterOutputTypeDef,
     DescribeVirtualRouterOutputTypeDef,
     UpdateVirtualRouterOutputTypeDef,
+    ListenerOutputTypeDef,
     ListenerTypeDef,
+    ClientPolicyOutputTypeDef,
     ClientPolicyTypeDef,
+    VirtualGatewayListenerOutputTypeDef,
     VirtualGatewayListenerTypeDef,
+    VirtualGatewayClientPolicyOutputTypeDef,
     VirtualGatewayClientPolicyTypeDef,
     CreateVirtualServiceOutputTypeDef,
     DeleteVirtualServiceOutputTypeDef,
     DescribeVirtualServiceOutputTypeDef,
     UpdateVirtualServiceOutputTypeDef,
+    GatewayRouteSpecOutputTypeDef,
+    RouteSpecOutputTypeDef,
     GatewayRouteSpecTypeDef,
     RouteSpecTypeDef,
+    BackendDefaultsOutputTypeDef,
+    VirtualServiceBackendOutputTypeDef,
     BackendDefaultsTypeDef,
     VirtualServiceBackendTypeDef,
+    VirtualGatewayBackendDefaultsOutputTypeDef,
     VirtualGatewayBackendDefaultsTypeDef,
-    CreateGatewayRouteInputRequestTypeDef,
     GatewayRouteDataTypeDef,
+    RouteDataTypeDef,
+    CreateGatewayRouteInputRequestTypeDef,
     UpdateGatewayRouteInputRequestTypeDef,
     CreateRouteInputRequestTypeDef,
-    RouteDataTypeDef,
     UpdateRouteInputRequestTypeDef,
+    BackendOutputTypeDef,
     BackendTypeDef,
+    VirtualGatewaySpecOutputTypeDef,
     VirtualGatewaySpecTypeDef,
     CreateGatewayRouteOutputTypeDef,
     DeleteGatewayRouteOutputTypeDef,
     DescribeGatewayRouteOutputTypeDef,
     UpdateGatewayRouteOutputTypeDef,
     CreateRouteOutputTypeDef,
     DeleteRouteOutputTypeDef,
     DescribeRouteOutputTypeDef,
     UpdateRouteOutputTypeDef,
+    VirtualNodeSpecOutputTypeDef,
     VirtualNodeSpecTypeDef,
+    VirtualGatewayDataTypeDef,
     CreateVirtualGatewayInputRequestTypeDef,
     UpdateVirtualGatewayInputRequestTypeDef,
-    VirtualGatewayDataTypeDef,
+    VirtualNodeDataTypeDef,
     CreateVirtualNodeInputRequestTypeDef,
     UpdateVirtualNodeInputRequestTypeDef,
-    VirtualNodeDataTypeDef,
     CreateVirtualGatewayOutputTypeDef,
     DeleteVirtualGatewayOutputTypeDef,
     DescribeVirtualGatewayOutputTypeDef,
     UpdateVirtualGatewayOutputTypeDef,
     CreateVirtualNodeOutputTypeDef,
     DeleteVirtualNodeOutputTypeDef,
     DescribeVirtualNodeOutputTypeDef,
     UpdateVirtualNodeOutputTypeDef,
 )
 
 
-def get_structure() -> AwsCloudMapInstanceAttributeTypeDef:
+def get_structure() -> AwsCloudMapInstanceAttributeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appmesh-1.28.0/README.md` & `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-appmesh
+Version: 1.28.12
+Summary: Type annotations for boto3.AppMesh 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 appmesh type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-appmesh"></a>
 
 # mypy-boto3-appmesh
 
 [![PyPI - mypy-boto3-appmesh](https://img.shields.io/pypi/v/mypy-boto3-appmesh.svg?color=blue)](https://pypi.org/project/mypy-boto3-appmesh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appmesh.svg?color=blue)](https://pypi.org/project/mypy-boto3-appmesh)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appmesh?color=blue)](https://pypistats.org/packages/mypy-boto3-appmesh)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appmesh)](https://pepy.tech/project/mypy-boto3-appmesh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppMesh 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
+[boto3.AppMesh 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
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
 [mypy-boto3-appmesh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,15 +371,18 @@
 ### Typed dictionaries
 
 `mypy_boto3_appmesh.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appmesh.type_defs import (
+    AwsCloudMapInstanceAttributeOutputTypeDef,
     AwsCloudMapInstanceAttributeTypeDef,
+    ListenerTlsFileCertificateOutputTypeDef,
+    ListenerTlsSdsCertificateOutputTypeDef,
     ListenerTlsFileCertificateTypeDef,
     ListenerTlsSdsCertificateTypeDef,
     TagRefTypeDef,
     DeleteGatewayRouteInputRequestTypeDef,
     DeleteMeshInputRequestTypeDef,
     DeleteRouteInputRequestTypeDef,
     DeleteVirtualGatewayInputRequestTypeDef,
@@ -357,226 +392,343 @@
     DescribeGatewayRouteInputRequestTypeDef,
     DescribeMeshInputRequestTypeDef,
     DescribeRouteInputRequestTypeDef,
     DescribeVirtualGatewayInputRequestTypeDef,
     DescribeVirtualNodeInputRequestTypeDef,
     DescribeVirtualRouterInputRequestTypeDef,
     DescribeVirtualServiceInputRequestTypeDef,
+    DnsServiceDiscoveryOutputTypeDef,
     DnsServiceDiscoveryTypeDef,
+    DurationOutputTypeDef,
     DurationTypeDef,
+    EgressFilterOutputTypeDef,
     EgressFilterTypeDef,
     GatewayRouteStatusTypeDef,
     ResourceMetadataTypeDef,
+    GatewayRouteHostnameMatchOutputTypeDef,
     GatewayRouteHostnameMatchTypeDef,
+    GatewayRouteHostnameRewriteOutputTypeDef,
     GatewayRouteHostnameRewriteTypeDef,
     GatewayRouteRefTypeDef,
+    GatewayRouteVirtualServiceOutputTypeDef,
     GatewayRouteVirtualServiceTypeDef,
+    MatchRangeOutputTypeDef,
     MatchRangeTypeDef,
+    WeightedTargetOutputTypeDef,
     WeightedTargetTypeDef,
+    HealthCheckPolicyOutputTypeDef,
     HealthCheckPolicyTypeDef,
+    HttpPathMatchOutputTypeDef,
     HttpPathMatchTypeDef,
+    HttpGatewayRoutePathRewriteOutputTypeDef,
     HttpGatewayRoutePathRewriteTypeDef,
+    HttpGatewayRoutePrefixRewriteOutputTypeDef,
     HttpGatewayRoutePrefixRewriteTypeDef,
+    QueryParameterMatchOutputTypeDef,
     QueryParameterMatchTypeDef,
+    JsonFormatRefOutputTypeDef,
     JsonFormatRefTypeDef,
     ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
     ListGatewayRoutesInputRequestTypeDef,
     ListMeshesInputListMeshesPaginateTypeDef,
     ListMeshesInputRequestTypeDef,
     MeshRefTypeDef,
     ListRoutesInputListRoutesPaginateTypeDef,
     ListRoutesInputRequestTypeDef,
     RouteRefTypeDef,
     ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    TagRefOutputTypeDef,
     ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
     ListVirtualGatewaysInputRequestTypeDef,
     VirtualGatewayRefTypeDef,
     ListVirtualNodesInputListVirtualNodesPaginateTypeDef,
     ListVirtualNodesInputRequestTypeDef,
     VirtualNodeRefTypeDef,
     ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
     ListVirtualRoutersInputRequestTypeDef,
     VirtualRouterRefTypeDef,
     ListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     ListVirtualServicesInputRequestTypeDef,
     VirtualServiceRefTypeDef,
+    PortMappingOutputTypeDef,
+    ListenerTlsAcmCertificateOutputTypeDef,
     ListenerTlsAcmCertificateTypeDef,
+    TlsValidationContextFileTrustOutputTypeDef,
+    TlsValidationContextSdsTrustOutputTypeDef,
     TlsValidationContextFileTrustTypeDef,
     TlsValidationContextSdsTrustTypeDef,
     PortMappingTypeDef,
     MeshStatusTypeDef,
+    MeshServiceDiscoveryOutputTypeDef,
     MeshServiceDiscoveryTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     RouteStatusTypeDef,
+    SubjectAlternativeNameMatchersOutputTypeDef,
     SubjectAlternativeNameMatchersTypeDef,
+    TcpRouteMatchOutputTypeDef,
     TcpRouteMatchTypeDef,
+    TlsValidationContextAcmTrustOutputTypeDef,
     TlsValidationContextAcmTrustTypeDef,
     UntagResourceInputRequestTypeDef,
+    VirtualGatewayListenerTlsFileCertificateOutputTypeDef,
+    VirtualGatewayListenerTlsSdsCertificateOutputTypeDef,
     VirtualGatewayListenerTlsFileCertificateTypeDef,
     VirtualGatewayListenerTlsSdsCertificateTypeDef,
+    VirtualGatewayGrpcConnectionPoolOutputTypeDef,
+    VirtualGatewayHttp2ConnectionPoolOutputTypeDef,
+    VirtualGatewayHttpConnectionPoolOutputTypeDef,
     VirtualGatewayGrpcConnectionPoolTypeDef,
     VirtualGatewayHttp2ConnectionPoolTypeDef,
     VirtualGatewayHttpConnectionPoolTypeDef,
     VirtualGatewayStatusTypeDef,
+    VirtualGatewayHealthCheckPolicyOutputTypeDef,
     VirtualGatewayHealthCheckPolicyTypeDef,
+    VirtualGatewayPortMappingOutputTypeDef,
+    VirtualGatewayListenerTlsAcmCertificateOutputTypeDef,
     VirtualGatewayListenerTlsAcmCertificateTypeDef,
+    VirtualGatewayTlsValidationContextFileTrustOutputTypeDef,
+    VirtualGatewayTlsValidationContextSdsTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextFileTrustTypeDef,
     VirtualGatewayTlsValidationContextSdsTrustTypeDef,
     VirtualGatewayPortMappingTypeDef,
+    VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextAcmTrustTypeDef,
+    VirtualNodeGrpcConnectionPoolOutputTypeDef,
+    VirtualNodeHttp2ConnectionPoolOutputTypeDef,
+    VirtualNodeHttpConnectionPoolOutputTypeDef,
+    VirtualNodeTcpConnectionPoolOutputTypeDef,
     VirtualNodeGrpcConnectionPoolTypeDef,
     VirtualNodeHttp2ConnectionPoolTypeDef,
     VirtualNodeHttpConnectionPoolTypeDef,
     VirtualNodeTcpConnectionPoolTypeDef,
     VirtualNodeStatusTypeDef,
+    VirtualNodeServiceProviderOutputTypeDef,
     VirtualNodeServiceProviderTypeDef,
     VirtualRouterStatusTypeDef,
+    VirtualRouterServiceProviderOutputTypeDef,
     VirtualRouterServiceProviderTypeDef,
     VirtualServiceStatusTypeDef,
+    AwsCloudMapServiceDiscoveryOutputTypeDef,
     AwsCloudMapServiceDiscoveryTypeDef,
+    ClientTlsCertificateOutputTypeDef,
     ClientTlsCertificateTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    GrpcRetryPolicyOutputTypeDef,
+    GrpcTimeoutOutputTypeDef,
+    HttpRetryPolicyOutputTypeDef,
+    HttpTimeoutOutputTypeDef,
+    OutlierDetectionOutputTypeDef,
+    TcpTimeoutOutputTypeDef,
     GrpcRetryPolicyTypeDef,
     GrpcTimeoutTypeDef,
     HttpRetryPolicyTypeDef,
     HttpTimeoutTypeDef,
     OutlierDetectionTypeDef,
     TcpTimeoutTypeDef,
+    GrpcGatewayRouteRewriteOutputTypeDef,
     GrpcGatewayRouteRewriteTypeDef,
     ListGatewayRoutesOutputTypeDef,
+    GatewayRouteTargetOutputTypeDef,
     GatewayRouteTargetTypeDef,
+    GrpcMetadataMatchMethodOutputTypeDef,
+    GrpcRouteMetadataMatchMethodOutputTypeDef,
+    HeaderMatchMethodOutputTypeDef,
     GrpcMetadataMatchMethodTypeDef,
     GrpcRouteMetadataMatchMethodTypeDef,
     HeaderMatchMethodTypeDef,
+    GrpcRouteActionOutputTypeDef,
+    HttpRouteActionOutputTypeDef,
+    TcpRouteActionOutputTypeDef,
     GrpcRouteActionTypeDef,
     HttpRouteActionTypeDef,
     TcpRouteActionTypeDef,
+    HttpGatewayRouteRewriteOutputTypeDef,
     HttpGatewayRouteRewriteTypeDef,
+    HttpQueryParameterOutputTypeDef,
     HttpQueryParameterTypeDef,
+    LoggingFormatOutputTypeDef,
     LoggingFormatTypeDef,
     ListMeshesOutputTypeDef,
     ListRoutesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListVirtualGatewaysOutputTypeDef,
     ListVirtualNodesOutputTypeDef,
     ListVirtualRoutersOutputTypeDef,
     ListVirtualServicesOutputTypeDef,
+    VirtualRouterListenerOutputTypeDef,
+    ListenerTlsCertificateOutputTypeDef,
     ListenerTlsCertificateTypeDef,
+    ListenerTlsValidationContextTrustOutputTypeDef,
     ListenerTlsValidationContextTrustTypeDef,
     VirtualRouterListenerTypeDef,
+    MeshSpecOutputTypeDef,
     MeshSpecTypeDef,
+    SubjectAlternativeNamesOutputTypeDef,
     SubjectAlternativeNamesTypeDef,
+    TlsValidationContextTrustOutputTypeDef,
     TlsValidationContextTrustTypeDef,
+    VirtualGatewayClientTlsCertificateOutputTypeDef,
     VirtualGatewayClientTlsCertificateTypeDef,
+    VirtualGatewayConnectionPoolOutputTypeDef,
     VirtualGatewayConnectionPoolTypeDef,
+    VirtualGatewayListenerTlsCertificateOutputTypeDef,
     VirtualGatewayListenerTlsCertificateTypeDef,
+    VirtualGatewayListenerTlsValidationContextTrustOutputTypeDef,
     VirtualGatewayListenerTlsValidationContextTrustTypeDef,
+    VirtualGatewayTlsValidationContextTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextTrustTypeDef,
+    VirtualNodeConnectionPoolOutputTypeDef,
     VirtualNodeConnectionPoolTypeDef,
+    VirtualServiceProviderOutputTypeDef,
     VirtualServiceProviderTypeDef,
+    ServiceDiscoveryOutputTypeDef,
     ServiceDiscoveryTypeDef,
+    ListenerTimeoutOutputTypeDef,
     ListenerTimeoutTypeDef,
+    GrpcGatewayRouteActionOutputTypeDef,
     GrpcGatewayRouteActionTypeDef,
+    GrpcGatewayRouteMetadataOutputTypeDef,
+    GrpcRouteMetadataOutputTypeDef,
+    HttpGatewayRouteHeaderOutputTypeDef,
+    HttpRouteHeaderOutputTypeDef,
     GrpcGatewayRouteMetadataTypeDef,
     GrpcRouteMetadataTypeDef,
     HttpGatewayRouteHeaderTypeDef,
     HttpRouteHeaderTypeDef,
+    TcpRouteOutputTypeDef,
     TcpRouteTypeDef,
+    HttpGatewayRouteActionOutputTypeDef,
     HttpGatewayRouteActionTypeDef,
+    FileAccessLogOutputTypeDef,
+    VirtualGatewayFileAccessLogOutputTypeDef,
     FileAccessLogTypeDef,
     VirtualGatewayFileAccessLogTypeDef,
+    VirtualRouterSpecOutputTypeDef,
     VirtualRouterSpecTypeDef,
-    CreateMeshInputRequestTypeDef,
     MeshDataTypeDef,
+    CreateMeshInputRequestTypeDef,
     UpdateMeshInputRequestTypeDef,
+    ListenerTlsValidationContextOutputTypeDef,
     ListenerTlsValidationContextTypeDef,
+    TlsValidationContextOutputTypeDef,
     TlsValidationContextTypeDef,
+    VirtualGatewayListenerTlsValidationContextOutputTypeDef,
     VirtualGatewayListenerTlsValidationContextTypeDef,
+    VirtualGatewayTlsValidationContextOutputTypeDef,
     VirtualGatewayTlsValidationContextTypeDef,
+    VirtualServiceSpecOutputTypeDef,
     VirtualServiceSpecTypeDef,
+    GrpcGatewayRouteMatchOutputTypeDef,
+    GrpcRouteMatchOutputTypeDef,
+    HttpGatewayRouteMatchOutputTypeDef,
+    HttpRouteMatchOutputTypeDef,
     GrpcGatewayRouteMatchTypeDef,
     GrpcRouteMatchTypeDef,
     HttpGatewayRouteMatchTypeDef,
     HttpRouteMatchTypeDef,
+    AccessLogOutputTypeDef,
+    VirtualGatewayAccessLogOutputTypeDef,
     AccessLogTypeDef,
     VirtualGatewayAccessLogTypeDef,
+    VirtualRouterDataTypeDef,
     CreateVirtualRouterInputRequestTypeDef,
     UpdateVirtualRouterInputRequestTypeDef,
-    VirtualRouterDataTypeDef,
     CreateMeshOutputTypeDef,
     DeleteMeshOutputTypeDef,
     DescribeMeshOutputTypeDef,
     UpdateMeshOutputTypeDef,
+    ListenerTlsOutputTypeDef,
     ListenerTlsTypeDef,
+    ClientPolicyTlsOutputTypeDef,
     ClientPolicyTlsTypeDef,
+    VirtualGatewayListenerTlsOutputTypeDef,
     VirtualGatewayListenerTlsTypeDef,
+    VirtualGatewayClientPolicyTlsOutputTypeDef,
     VirtualGatewayClientPolicyTlsTypeDef,
+    VirtualServiceDataTypeDef,
     CreateVirtualServiceInputRequestTypeDef,
     UpdateVirtualServiceInputRequestTypeDef,
-    VirtualServiceDataTypeDef,
+    GrpcGatewayRouteOutputTypeDef,
+    GrpcRouteOutputTypeDef,
+    HttpGatewayRouteOutputTypeDef,
+    HttpRouteOutputTypeDef,
     GrpcGatewayRouteTypeDef,
     GrpcRouteTypeDef,
     HttpGatewayRouteTypeDef,
     HttpRouteTypeDef,
+    LoggingOutputTypeDef,
+    VirtualGatewayLoggingOutputTypeDef,
     LoggingTypeDef,
     VirtualGatewayLoggingTypeDef,
     CreateVirtualRouterOutputTypeDef,
     DeleteVirtualRouterOutputTypeDef,
     DescribeVirtualRouterOutputTypeDef,
     UpdateVirtualRouterOutputTypeDef,
+    ListenerOutputTypeDef,
     ListenerTypeDef,
+    ClientPolicyOutputTypeDef,
     ClientPolicyTypeDef,
+    VirtualGatewayListenerOutputTypeDef,
     VirtualGatewayListenerTypeDef,
+    VirtualGatewayClientPolicyOutputTypeDef,
     VirtualGatewayClientPolicyTypeDef,
     CreateVirtualServiceOutputTypeDef,
     DeleteVirtualServiceOutputTypeDef,
     DescribeVirtualServiceOutputTypeDef,
     UpdateVirtualServiceOutputTypeDef,
+    GatewayRouteSpecOutputTypeDef,
+    RouteSpecOutputTypeDef,
     GatewayRouteSpecTypeDef,
     RouteSpecTypeDef,
+    BackendDefaultsOutputTypeDef,
+    VirtualServiceBackendOutputTypeDef,
     BackendDefaultsTypeDef,
     VirtualServiceBackendTypeDef,
+    VirtualGatewayBackendDefaultsOutputTypeDef,
     VirtualGatewayBackendDefaultsTypeDef,
-    CreateGatewayRouteInputRequestTypeDef,
     GatewayRouteDataTypeDef,
+    RouteDataTypeDef,
+    CreateGatewayRouteInputRequestTypeDef,
     UpdateGatewayRouteInputRequestTypeDef,
     CreateRouteInputRequestTypeDef,
-    RouteDataTypeDef,
     UpdateRouteInputRequestTypeDef,
+    BackendOutputTypeDef,
     BackendTypeDef,
+    VirtualGatewaySpecOutputTypeDef,
     VirtualGatewaySpecTypeDef,
     CreateGatewayRouteOutputTypeDef,
     DeleteGatewayRouteOutputTypeDef,
     DescribeGatewayRouteOutputTypeDef,
     UpdateGatewayRouteOutputTypeDef,
     CreateRouteOutputTypeDef,
     DeleteRouteOutputTypeDef,
     DescribeRouteOutputTypeDef,
     UpdateRouteOutputTypeDef,
+    VirtualNodeSpecOutputTypeDef,
     VirtualNodeSpecTypeDef,
+    VirtualGatewayDataTypeDef,
     CreateVirtualGatewayInputRequestTypeDef,
     UpdateVirtualGatewayInputRequestTypeDef,
-    VirtualGatewayDataTypeDef,
+    VirtualNodeDataTypeDef,
     CreateVirtualNodeInputRequestTypeDef,
     UpdateVirtualNodeInputRequestTypeDef,
-    VirtualNodeDataTypeDef,
     CreateVirtualGatewayOutputTypeDef,
     DeleteVirtualGatewayOutputTypeDef,
     DescribeVirtualGatewayOutputTypeDef,
     UpdateVirtualGatewayOutputTypeDef,
     CreateVirtualNodeOutputTypeDef,
     DeleteVirtualNodeOutputTypeDef,
     DescribeVirtualNodeOutputTypeDef,
     UpdateVirtualNodeOutputTypeDef,
 )
 
 
-def get_structure() -> AwsCloudMapInstanceAttributeTypeDef:
+def get_structure() -> AwsCloudMapInstanceAttributeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/__init__.py` & `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/__init__.pyi` & `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/__main__.py` & `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppMesh 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.AppMesh 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh\nOther"
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

### Comparing `mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/client.py` & `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/client.pyi` & `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/literals.py` & `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,15 @@
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
@@ -290,26 +291,28 @@
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

### Comparing `mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/literals.pyi` & `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -202,14 +202,15 @@
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
@@ -288,26 +289,28 @@
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

### Comparing `mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/paginator.py` & `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/paginator.pyi` & `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh/type_defs.py` & `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/type_defs.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for appmesh service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_appmesh.type_defs import AwsCloudMapInstanceAttributeTypeDef
+    from mypy_boto3_appmesh.type_defs import AwsCloudMapInstanceAttributeOutputTypeDef
 
-    data: AwsCloudMapInstanceAttributeTypeDef = {...}
+    data: AwsCloudMapInstanceAttributeOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -42,17 +42,19 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "AwsCloudMapInstanceAttributeOutputTypeDef",
     "AwsCloudMapInstanceAttributeTypeDef",
+    "ListenerTlsFileCertificateOutputTypeDef",
+    "ListenerTlsSdsCertificateOutputTypeDef",
     "ListenerTlsFileCertificateTypeDef",
     "ListenerTlsSdsCertificateTypeDef",
     "TagRefTypeDef",
     "DeleteGatewayRouteInputRequestTypeDef",
     "DeleteMeshInputRequestTypeDef",
     "DeleteRouteInputRequestTypeDef",
     "DeleteVirtualGatewayInputRequestTypeDef",
@@ -62,232 +64,372 @@
     "DescribeGatewayRouteInputRequestTypeDef",
     "DescribeMeshInputRequestTypeDef",
     "DescribeRouteInputRequestTypeDef",
     "DescribeVirtualGatewayInputRequestTypeDef",
     "DescribeVirtualNodeInputRequestTypeDef",
     "DescribeVirtualRouterInputRequestTypeDef",
     "DescribeVirtualServiceInputRequestTypeDef",
+    "DnsServiceDiscoveryOutputTypeDef",
     "DnsServiceDiscoveryTypeDef",
+    "DurationOutputTypeDef",
     "DurationTypeDef",
+    "EgressFilterOutputTypeDef",
     "EgressFilterTypeDef",
     "GatewayRouteStatusTypeDef",
     "ResourceMetadataTypeDef",
+    "GatewayRouteHostnameMatchOutputTypeDef",
     "GatewayRouteHostnameMatchTypeDef",
+    "GatewayRouteHostnameRewriteOutputTypeDef",
     "GatewayRouteHostnameRewriteTypeDef",
     "GatewayRouteRefTypeDef",
+    "GatewayRouteVirtualServiceOutputTypeDef",
     "GatewayRouteVirtualServiceTypeDef",
+    "MatchRangeOutputTypeDef",
     "MatchRangeTypeDef",
+    "WeightedTargetOutputTypeDef",
     "WeightedTargetTypeDef",
+    "HealthCheckPolicyOutputTypeDef",
     "HealthCheckPolicyTypeDef",
+    "HttpPathMatchOutputTypeDef",
     "HttpPathMatchTypeDef",
+    "HttpGatewayRoutePathRewriteOutputTypeDef",
     "HttpGatewayRoutePathRewriteTypeDef",
+    "HttpGatewayRoutePrefixRewriteOutputTypeDef",
     "HttpGatewayRoutePrefixRewriteTypeDef",
+    "QueryParameterMatchOutputTypeDef",
     "QueryParameterMatchTypeDef",
+    "JsonFormatRefOutputTypeDef",
     "JsonFormatRefTypeDef",
     "ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
     "ListGatewayRoutesInputRequestTypeDef",
     "ListMeshesInputListMeshesPaginateTypeDef",
     "ListMeshesInputRequestTypeDef",
     "MeshRefTypeDef",
     "ListRoutesInputListRoutesPaginateTypeDef",
     "ListRoutesInputRequestTypeDef",
     "RouteRefTypeDef",
     "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "TagRefOutputTypeDef",
     "ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
     "ListVirtualGatewaysInputRequestTypeDef",
     "VirtualGatewayRefTypeDef",
     "ListVirtualNodesInputListVirtualNodesPaginateTypeDef",
     "ListVirtualNodesInputRequestTypeDef",
     "VirtualNodeRefTypeDef",
     "ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
     "ListVirtualRoutersInputRequestTypeDef",
     "VirtualRouterRefTypeDef",
     "ListVirtualServicesInputListVirtualServicesPaginateTypeDef",
     "ListVirtualServicesInputRequestTypeDef",
     "VirtualServiceRefTypeDef",
+    "PortMappingOutputTypeDef",
+    "ListenerTlsAcmCertificateOutputTypeDef",
     "ListenerTlsAcmCertificateTypeDef",
+    "TlsValidationContextFileTrustOutputTypeDef",
+    "TlsValidationContextSdsTrustOutputTypeDef",
     "TlsValidationContextFileTrustTypeDef",
     "TlsValidationContextSdsTrustTypeDef",
     "PortMappingTypeDef",
     "MeshStatusTypeDef",
+    "MeshServiceDiscoveryOutputTypeDef",
     "MeshServiceDiscoveryTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "RouteStatusTypeDef",
+    "SubjectAlternativeNameMatchersOutputTypeDef",
     "SubjectAlternativeNameMatchersTypeDef",
+    "TcpRouteMatchOutputTypeDef",
     "TcpRouteMatchTypeDef",
+    "TlsValidationContextAcmTrustOutputTypeDef",
     "TlsValidationContextAcmTrustTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "VirtualGatewayListenerTlsFileCertificateOutputTypeDef",
+    "VirtualGatewayListenerTlsSdsCertificateOutputTypeDef",
     "VirtualGatewayListenerTlsFileCertificateTypeDef",
     "VirtualGatewayListenerTlsSdsCertificateTypeDef",
+    "VirtualGatewayGrpcConnectionPoolOutputTypeDef",
+    "VirtualGatewayHttp2ConnectionPoolOutputTypeDef",
+    "VirtualGatewayHttpConnectionPoolOutputTypeDef",
     "VirtualGatewayGrpcConnectionPoolTypeDef",
     "VirtualGatewayHttp2ConnectionPoolTypeDef",
     "VirtualGatewayHttpConnectionPoolTypeDef",
     "VirtualGatewayStatusTypeDef",
+    "VirtualGatewayHealthCheckPolicyOutputTypeDef",
     "VirtualGatewayHealthCheckPolicyTypeDef",
+    "VirtualGatewayPortMappingOutputTypeDef",
+    "VirtualGatewayListenerTlsAcmCertificateOutputTypeDef",
     "VirtualGatewayListenerTlsAcmCertificateTypeDef",
+    "VirtualGatewayTlsValidationContextFileTrustOutputTypeDef",
+    "VirtualGatewayTlsValidationContextSdsTrustOutputTypeDef",
     "VirtualGatewayTlsValidationContextFileTrustTypeDef",
     "VirtualGatewayTlsValidationContextSdsTrustTypeDef",
     "VirtualGatewayPortMappingTypeDef",
+    "VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef",
     "VirtualGatewayTlsValidationContextAcmTrustTypeDef",
+    "VirtualNodeGrpcConnectionPoolOutputTypeDef",
+    "VirtualNodeHttp2ConnectionPoolOutputTypeDef",
+    "VirtualNodeHttpConnectionPoolOutputTypeDef",
+    "VirtualNodeTcpConnectionPoolOutputTypeDef",
     "VirtualNodeGrpcConnectionPoolTypeDef",
     "VirtualNodeHttp2ConnectionPoolTypeDef",
     "VirtualNodeHttpConnectionPoolTypeDef",
     "VirtualNodeTcpConnectionPoolTypeDef",
     "VirtualNodeStatusTypeDef",
+    "VirtualNodeServiceProviderOutputTypeDef",
     "VirtualNodeServiceProviderTypeDef",
     "VirtualRouterStatusTypeDef",
+    "VirtualRouterServiceProviderOutputTypeDef",
     "VirtualRouterServiceProviderTypeDef",
     "VirtualServiceStatusTypeDef",
+    "AwsCloudMapServiceDiscoveryOutputTypeDef",
     "AwsCloudMapServiceDiscoveryTypeDef",
+    "ClientTlsCertificateOutputTypeDef",
     "ClientTlsCertificateTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
+    "GrpcRetryPolicyOutputTypeDef",
+    "GrpcTimeoutOutputTypeDef",
+    "HttpRetryPolicyOutputTypeDef",
+    "HttpTimeoutOutputTypeDef",
+    "OutlierDetectionOutputTypeDef",
+    "TcpTimeoutOutputTypeDef",
     "GrpcRetryPolicyTypeDef",
     "GrpcTimeoutTypeDef",
     "HttpRetryPolicyTypeDef",
     "HttpTimeoutTypeDef",
     "OutlierDetectionTypeDef",
     "TcpTimeoutTypeDef",
+    "GrpcGatewayRouteRewriteOutputTypeDef",
     "GrpcGatewayRouteRewriteTypeDef",
     "ListGatewayRoutesOutputTypeDef",
+    "GatewayRouteTargetOutputTypeDef",
     "GatewayRouteTargetTypeDef",
+    "GrpcMetadataMatchMethodOutputTypeDef",
+    "GrpcRouteMetadataMatchMethodOutputTypeDef",
+    "HeaderMatchMethodOutputTypeDef",
     "GrpcMetadataMatchMethodTypeDef",
     "GrpcRouteMetadataMatchMethodTypeDef",
     "HeaderMatchMethodTypeDef",
+    "GrpcRouteActionOutputTypeDef",
+    "HttpRouteActionOutputTypeDef",
+    "TcpRouteActionOutputTypeDef",
     "GrpcRouteActionTypeDef",
     "HttpRouteActionTypeDef",
     "TcpRouteActionTypeDef",
+    "HttpGatewayRouteRewriteOutputTypeDef",
     "HttpGatewayRouteRewriteTypeDef",
+    "HttpQueryParameterOutputTypeDef",
     "HttpQueryParameterTypeDef",
+    "LoggingFormatOutputTypeDef",
     "LoggingFormatTypeDef",
     "ListMeshesOutputTypeDef",
     "ListRoutesOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "ListVirtualGatewaysOutputTypeDef",
     "ListVirtualNodesOutputTypeDef",
     "ListVirtualRoutersOutputTypeDef",
     "ListVirtualServicesOutputTypeDef",
+    "VirtualRouterListenerOutputTypeDef",
+    "ListenerTlsCertificateOutputTypeDef",
     "ListenerTlsCertificateTypeDef",
+    "ListenerTlsValidationContextTrustOutputTypeDef",
     "ListenerTlsValidationContextTrustTypeDef",
     "VirtualRouterListenerTypeDef",
+    "MeshSpecOutputTypeDef",
     "MeshSpecTypeDef",
+    "SubjectAlternativeNamesOutputTypeDef",
     "SubjectAlternativeNamesTypeDef",
+    "TlsValidationContextTrustOutputTypeDef",
     "TlsValidationContextTrustTypeDef",
+    "VirtualGatewayClientTlsCertificateOutputTypeDef",
     "VirtualGatewayClientTlsCertificateTypeDef",
+    "VirtualGatewayConnectionPoolOutputTypeDef",
     "VirtualGatewayConnectionPoolTypeDef",
+    "VirtualGatewayListenerTlsCertificateOutputTypeDef",
     "VirtualGatewayListenerTlsCertificateTypeDef",
+    "VirtualGatewayListenerTlsValidationContextTrustOutputTypeDef",
     "VirtualGatewayListenerTlsValidationContextTrustTypeDef",
+    "VirtualGatewayTlsValidationContextTrustOutputTypeDef",
     "VirtualGatewayTlsValidationContextTrustTypeDef",
+    "VirtualNodeConnectionPoolOutputTypeDef",
     "VirtualNodeConnectionPoolTypeDef",
+    "VirtualServiceProviderOutputTypeDef",
     "VirtualServiceProviderTypeDef",
+    "ServiceDiscoveryOutputTypeDef",
     "ServiceDiscoveryTypeDef",
+    "ListenerTimeoutOutputTypeDef",
     "ListenerTimeoutTypeDef",
+    "GrpcGatewayRouteActionOutputTypeDef",
     "GrpcGatewayRouteActionTypeDef",
+    "GrpcGatewayRouteMetadataOutputTypeDef",
+    "GrpcRouteMetadataOutputTypeDef",
+    "HttpGatewayRouteHeaderOutputTypeDef",
+    "HttpRouteHeaderOutputTypeDef",
     "GrpcGatewayRouteMetadataTypeDef",
     "GrpcRouteMetadataTypeDef",
     "HttpGatewayRouteHeaderTypeDef",
     "HttpRouteHeaderTypeDef",
+    "TcpRouteOutputTypeDef",
     "TcpRouteTypeDef",
+    "HttpGatewayRouteActionOutputTypeDef",
     "HttpGatewayRouteActionTypeDef",
+    "FileAccessLogOutputTypeDef",
+    "VirtualGatewayFileAccessLogOutputTypeDef",
     "FileAccessLogTypeDef",
     "VirtualGatewayFileAccessLogTypeDef",
+    "VirtualRouterSpecOutputTypeDef",
     "VirtualRouterSpecTypeDef",
-    "CreateMeshInputRequestTypeDef",
     "MeshDataTypeDef",
+    "CreateMeshInputRequestTypeDef",
     "UpdateMeshInputRequestTypeDef",
+    "ListenerTlsValidationContextOutputTypeDef",
     "ListenerTlsValidationContextTypeDef",
+    "TlsValidationContextOutputTypeDef",
     "TlsValidationContextTypeDef",
+    "VirtualGatewayListenerTlsValidationContextOutputTypeDef",
     "VirtualGatewayListenerTlsValidationContextTypeDef",
+    "VirtualGatewayTlsValidationContextOutputTypeDef",
     "VirtualGatewayTlsValidationContextTypeDef",
+    "VirtualServiceSpecOutputTypeDef",
     "VirtualServiceSpecTypeDef",
+    "GrpcGatewayRouteMatchOutputTypeDef",
+    "GrpcRouteMatchOutputTypeDef",
+    "HttpGatewayRouteMatchOutputTypeDef",
+    "HttpRouteMatchOutputTypeDef",
     "GrpcGatewayRouteMatchTypeDef",
     "GrpcRouteMatchTypeDef",
     "HttpGatewayRouteMatchTypeDef",
     "HttpRouteMatchTypeDef",
+    "AccessLogOutputTypeDef",
+    "VirtualGatewayAccessLogOutputTypeDef",
     "AccessLogTypeDef",
     "VirtualGatewayAccessLogTypeDef",
+    "VirtualRouterDataTypeDef",
     "CreateVirtualRouterInputRequestTypeDef",
     "UpdateVirtualRouterInputRequestTypeDef",
-    "VirtualRouterDataTypeDef",
     "CreateMeshOutputTypeDef",
     "DeleteMeshOutputTypeDef",
     "DescribeMeshOutputTypeDef",
     "UpdateMeshOutputTypeDef",
+    "ListenerTlsOutputTypeDef",
     "ListenerTlsTypeDef",
+    "ClientPolicyTlsOutputTypeDef",
     "ClientPolicyTlsTypeDef",
+    "VirtualGatewayListenerTlsOutputTypeDef",
     "VirtualGatewayListenerTlsTypeDef",
+    "VirtualGatewayClientPolicyTlsOutputTypeDef",
     "VirtualGatewayClientPolicyTlsTypeDef",
+    "VirtualServiceDataTypeDef",
     "CreateVirtualServiceInputRequestTypeDef",
     "UpdateVirtualServiceInputRequestTypeDef",
-    "VirtualServiceDataTypeDef",
+    "GrpcGatewayRouteOutputTypeDef",
+    "GrpcRouteOutputTypeDef",
+    "HttpGatewayRouteOutputTypeDef",
+    "HttpRouteOutputTypeDef",
     "GrpcGatewayRouteTypeDef",
     "GrpcRouteTypeDef",
     "HttpGatewayRouteTypeDef",
     "HttpRouteTypeDef",
+    "LoggingOutputTypeDef",
+    "VirtualGatewayLoggingOutputTypeDef",
     "LoggingTypeDef",
     "VirtualGatewayLoggingTypeDef",
     "CreateVirtualRouterOutputTypeDef",
     "DeleteVirtualRouterOutputTypeDef",
     "DescribeVirtualRouterOutputTypeDef",
     "UpdateVirtualRouterOutputTypeDef",
+    "ListenerOutputTypeDef",
     "ListenerTypeDef",
+    "ClientPolicyOutputTypeDef",
     "ClientPolicyTypeDef",
+    "VirtualGatewayListenerOutputTypeDef",
     "VirtualGatewayListenerTypeDef",
+    "VirtualGatewayClientPolicyOutputTypeDef",
     "VirtualGatewayClientPolicyTypeDef",
     "CreateVirtualServiceOutputTypeDef",
     "DeleteVirtualServiceOutputTypeDef",
     "DescribeVirtualServiceOutputTypeDef",
     "UpdateVirtualServiceOutputTypeDef",
+    "GatewayRouteSpecOutputTypeDef",
+    "RouteSpecOutputTypeDef",
     "GatewayRouteSpecTypeDef",
     "RouteSpecTypeDef",
+    "BackendDefaultsOutputTypeDef",
+    "VirtualServiceBackendOutputTypeDef",
     "BackendDefaultsTypeDef",
     "VirtualServiceBackendTypeDef",
+    "VirtualGatewayBackendDefaultsOutputTypeDef",
     "VirtualGatewayBackendDefaultsTypeDef",
-    "CreateGatewayRouteInputRequestTypeDef",
     "GatewayRouteDataTypeDef",
+    "RouteDataTypeDef",
+    "CreateGatewayRouteInputRequestTypeDef",
     "UpdateGatewayRouteInputRequestTypeDef",
     "CreateRouteInputRequestTypeDef",
-    "RouteDataTypeDef",
     "UpdateRouteInputRequestTypeDef",
+    "BackendOutputTypeDef",
     "BackendTypeDef",
+    "VirtualGatewaySpecOutputTypeDef",
     "VirtualGatewaySpecTypeDef",
     "CreateGatewayRouteOutputTypeDef",
     "DeleteGatewayRouteOutputTypeDef",
     "DescribeGatewayRouteOutputTypeDef",
     "UpdateGatewayRouteOutputTypeDef",
     "CreateRouteOutputTypeDef",
     "DeleteRouteOutputTypeDef",
     "DescribeRouteOutputTypeDef",
     "UpdateRouteOutputTypeDef",
+    "VirtualNodeSpecOutputTypeDef",
     "VirtualNodeSpecTypeDef",
+    "VirtualGatewayDataTypeDef",
     "CreateVirtualGatewayInputRequestTypeDef",
     "UpdateVirtualGatewayInputRequestTypeDef",
-    "VirtualGatewayDataTypeDef",
+    "VirtualNodeDataTypeDef",
     "CreateVirtualNodeInputRequestTypeDef",
     "UpdateVirtualNodeInputRequestTypeDef",
-    "VirtualNodeDataTypeDef",
     "CreateVirtualGatewayOutputTypeDef",
     "DeleteVirtualGatewayOutputTypeDef",
     "DescribeVirtualGatewayOutputTypeDef",
     "UpdateVirtualGatewayOutputTypeDef",
     "CreateVirtualNodeOutputTypeDef",
     "DeleteVirtualNodeOutputTypeDef",
     "DescribeVirtualNodeOutputTypeDef",
     "UpdateVirtualNodeOutputTypeDef",
 )
 
+AwsCloudMapInstanceAttributeOutputTypeDef = TypedDict(
+    "AwsCloudMapInstanceAttributeOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 AwsCloudMapInstanceAttributeTypeDef = TypedDict(
     "AwsCloudMapInstanceAttributeTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
+ListenerTlsFileCertificateOutputTypeDef = TypedDict(
+    "ListenerTlsFileCertificateOutputTypeDef",
+    {
+        "certificateChain": str,
+        "privateKey": str,
+    },
+)
+
+ListenerTlsSdsCertificateOutputTypeDef = TypedDict(
+    "ListenerTlsSdsCertificateOutputTypeDef",
+    {
+        "secretName": str,
+    },
+)
+
 ListenerTlsFileCertificateTypeDef = TypedDict(
     "ListenerTlsFileCertificateTypeDef",
     {
         "certificateChain": str,
         "privateKey": str,
     },
 )
@@ -319,21 +461,19 @@
     "_OptionalDeleteGatewayRouteInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DeleteGatewayRouteInputRequestTypeDef(
     _RequiredDeleteGatewayRouteInputRequestTypeDef, _OptionalDeleteGatewayRouteInputRequestTypeDef
 ):
     pass
 
-
 DeleteMeshInputRequestTypeDef = TypedDict(
     "DeleteMeshInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 
@@ -349,21 +489,19 @@
     "_OptionalDeleteRouteInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DeleteRouteInputRequestTypeDef(
     _RequiredDeleteRouteInputRequestTypeDef, _OptionalDeleteRouteInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteVirtualGatewayInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVirtualGatewayInputRequestTypeDef",
     {
         "meshName": str,
         "virtualGatewayName": str,
     },
 )
@@ -371,22 +509,20 @@
     "_OptionalDeleteVirtualGatewayInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DeleteVirtualGatewayInputRequestTypeDef(
     _RequiredDeleteVirtualGatewayInputRequestTypeDef,
     _OptionalDeleteVirtualGatewayInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteVirtualNodeInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVirtualNodeInputRequestTypeDef",
     {
         "meshName": str,
         "virtualNodeName": str,
     },
 )
@@ -394,21 +530,19 @@
     "_OptionalDeleteVirtualNodeInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DeleteVirtualNodeInputRequestTypeDef(
     _RequiredDeleteVirtualNodeInputRequestTypeDef, _OptionalDeleteVirtualNodeInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteVirtualRouterInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVirtualRouterInputRequestTypeDef",
     {
         "meshName": str,
         "virtualRouterName": str,
     },
 )
@@ -416,21 +550,19 @@
     "_OptionalDeleteVirtualRouterInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DeleteVirtualRouterInputRequestTypeDef(
     _RequiredDeleteVirtualRouterInputRequestTypeDef, _OptionalDeleteVirtualRouterInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteVirtualServiceInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVirtualServiceInputRequestTypeDef",
     {
         "meshName": str,
         "virtualServiceName": str,
     },
 )
@@ -438,22 +570,20 @@
     "_OptionalDeleteVirtualServiceInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DeleteVirtualServiceInputRequestTypeDef(
     _RequiredDeleteVirtualServiceInputRequestTypeDef,
     _OptionalDeleteVirtualServiceInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredDescribeGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "virtualGatewayName": str,
     },
@@ -462,43 +592,39 @@
     "_OptionalDescribeGatewayRouteInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DescribeGatewayRouteInputRequestTypeDef(
     _RequiredDescribeGatewayRouteInputRequestTypeDef,
     _OptionalDescribeGatewayRouteInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMeshInputRequestTypeDef = TypedDict(
     "_RequiredDescribeMeshInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalDescribeMeshInputRequestTypeDef = TypedDict(
     "_OptionalDescribeMeshInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DescribeMeshInputRequestTypeDef(
     _RequiredDescribeMeshInputRequestTypeDef, _OptionalDescribeMeshInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeRouteInputRequestTypeDef = TypedDict(
     "_RequiredDescribeRouteInputRequestTypeDef",
     {
         "meshName": str,
         "routeName": str,
         "virtualRouterName": str,
     },
@@ -507,21 +633,19 @@
     "_OptionalDescribeRouteInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DescribeRouteInputRequestTypeDef(
     _RequiredDescribeRouteInputRequestTypeDef, _OptionalDescribeRouteInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeVirtualGatewayInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVirtualGatewayInputRequestTypeDef",
     {
         "meshName": str,
         "virtualGatewayName": str,
     },
 )
@@ -529,22 +653,20 @@
     "_OptionalDescribeVirtualGatewayInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DescribeVirtualGatewayInputRequestTypeDef(
     _RequiredDescribeVirtualGatewayInputRequestTypeDef,
     _OptionalDescribeVirtualGatewayInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeVirtualNodeInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVirtualNodeInputRequestTypeDef",
     {
         "meshName": str,
         "virtualNodeName": str,
     },
 )
@@ -552,21 +674,19 @@
     "_OptionalDescribeVirtualNodeInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DescribeVirtualNodeInputRequestTypeDef(
     _RequiredDescribeVirtualNodeInputRequestTypeDef, _OptionalDescribeVirtualNodeInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeVirtualRouterInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVirtualRouterInputRequestTypeDef",
     {
         "meshName": str,
         "virtualRouterName": str,
     },
 )
@@ -574,22 +694,20 @@
     "_OptionalDescribeVirtualRouterInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DescribeVirtualRouterInputRequestTypeDef(
     _RequiredDescribeVirtualRouterInputRequestTypeDef,
     _OptionalDescribeVirtualRouterInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeVirtualServiceInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVirtualServiceInputRequestTypeDef",
     {
         "meshName": str,
         "virtualServiceName": str,
     },
 )
@@ -597,21 +715,39 @@
     "_OptionalDescribeVirtualServiceInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DescribeVirtualServiceInputRequestTypeDef(
     _RequiredDescribeVirtualServiceInputRequestTypeDef,
     _OptionalDescribeVirtualServiceInputRequestTypeDef,
 ):
     pass
 
+_RequiredDnsServiceDiscoveryOutputTypeDef = TypedDict(
+    "_RequiredDnsServiceDiscoveryOutputTypeDef",
+    {
+        "hostname": str,
+    },
+)
+_OptionalDnsServiceDiscoveryOutputTypeDef = TypedDict(
+    "_OptionalDnsServiceDiscoveryOutputTypeDef",
+    {
+        "ipPreference": IpPreferenceType,
+        "responseType": DnsResponseTypeType,
+    },
+    total=False,
+)
+
+class DnsServiceDiscoveryOutputTypeDef(
+    _RequiredDnsServiceDiscoveryOutputTypeDef, _OptionalDnsServiceDiscoveryOutputTypeDef
+):
+    pass
 
 _RequiredDnsServiceDiscoveryTypeDef = TypedDict(
     "_RequiredDnsServiceDiscoveryTypeDef",
     {
         "hostname": str,
     },
 )
@@ -620,30 +756,44 @@
     {
         "ipPreference": IpPreferenceType,
         "responseType": DnsResponseTypeType,
     },
     total=False,
 )
 
-
 class DnsServiceDiscoveryTypeDef(
     _RequiredDnsServiceDiscoveryTypeDef, _OptionalDnsServiceDiscoveryTypeDef
 ):
     pass
 
+DurationOutputTypeDef = TypedDict(
+    "DurationOutputTypeDef",
+    {
+        "unit": DurationUnitType,
+        "value": int,
+    },
+    total=False,
+)
 
 DurationTypeDef = TypedDict(
     "DurationTypeDef",
     {
         "unit": DurationUnitType,
         "value": int,
     },
     total=False,
 )
 
+EgressFilterOutputTypeDef = TypedDict(
+    "EgressFilterOutputTypeDef",
+    {
+        "type": EgressFilterTypeType,
+    },
+)
+
 EgressFilterTypeDef = TypedDict(
     "EgressFilterTypeDef",
     {
         "type": EgressFilterTypeType,
     },
 )
 
@@ -663,23 +813,40 @@
         "meshOwner": str,
         "resourceOwner": str,
         "uid": str,
         "version": int,
     },
 )
 
+GatewayRouteHostnameMatchOutputTypeDef = TypedDict(
+    "GatewayRouteHostnameMatchOutputTypeDef",
+    {
+        "exact": str,
+        "suffix": str,
+    },
+    total=False,
+)
+
 GatewayRouteHostnameMatchTypeDef = TypedDict(
     "GatewayRouteHostnameMatchTypeDef",
     {
         "exact": str,
         "suffix": str,
     },
     total=False,
 )
 
+GatewayRouteHostnameRewriteOutputTypeDef = TypedDict(
+    "GatewayRouteHostnameRewriteOutputTypeDef",
+    {
+        "defaultTargetHostname": DefaultGatewayRouteRewriteType,
+    },
+    total=False,
+)
+
 GatewayRouteHostnameRewriteTypeDef = TypedDict(
     "GatewayRouteHostnameRewriteTypeDef",
     {
         "defaultTargetHostname": DefaultGatewayRouteRewriteType,
     },
     total=False,
 )
@@ -695,29 +862,64 @@
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualGatewayName": str,
     },
 )
 
+GatewayRouteVirtualServiceOutputTypeDef = TypedDict(
+    "GatewayRouteVirtualServiceOutputTypeDef",
+    {
+        "virtualServiceName": str,
+    },
+)
+
 GatewayRouteVirtualServiceTypeDef = TypedDict(
     "GatewayRouteVirtualServiceTypeDef",
     {
         "virtualServiceName": str,
     },
 )
 
+MatchRangeOutputTypeDef = TypedDict(
+    "MatchRangeOutputTypeDef",
+    {
+        "end": int,
+        "start": int,
+    },
+)
+
 MatchRangeTypeDef = TypedDict(
     "MatchRangeTypeDef",
     {
         "end": int,
         "start": int,
     },
 )
 
+_RequiredWeightedTargetOutputTypeDef = TypedDict(
+    "_RequiredWeightedTargetOutputTypeDef",
+    {
+        "virtualNode": str,
+        "weight": int,
+    },
+)
+_OptionalWeightedTargetOutputTypeDef = TypedDict(
+    "_OptionalWeightedTargetOutputTypeDef",
+    {
+        "port": int,
+    },
+    total=False,
+)
+
+class WeightedTargetOutputTypeDef(
+    _RequiredWeightedTargetOutputTypeDef, _OptionalWeightedTargetOutputTypeDef
+):
+    pass
+
 _RequiredWeightedTargetTypeDef = TypedDict(
     "_RequiredWeightedTargetTypeDef",
     {
         "virtualNode": str,
         "weight": int,
     },
 )
@@ -725,18 +927,40 @@
     "_OptionalWeightedTargetTypeDef",
     {
         "port": int,
     },
     total=False,
 )
 
-
 class WeightedTargetTypeDef(_RequiredWeightedTargetTypeDef, _OptionalWeightedTargetTypeDef):
     pass
 
+_RequiredHealthCheckPolicyOutputTypeDef = TypedDict(
+    "_RequiredHealthCheckPolicyOutputTypeDef",
+    {
+        "healthyThreshold": int,
+        "intervalMillis": int,
+        "protocol": PortProtocolType,
+        "timeoutMillis": int,
+        "unhealthyThreshold": int,
+    },
+)
+_OptionalHealthCheckPolicyOutputTypeDef = TypedDict(
+    "_OptionalHealthCheckPolicyOutputTypeDef",
+    {
+        "path": str,
+        "port": int,
+    },
+    total=False,
+)
+
+class HealthCheckPolicyOutputTypeDef(
+    _RequiredHealthCheckPolicyOutputTypeDef, _OptionalHealthCheckPolicyOutputTypeDef
+):
+    pass
 
 _RequiredHealthCheckPolicyTypeDef = TypedDict(
     "_RequiredHealthCheckPolicyTypeDef",
     {
         "healthyThreshold": int,
         "intervalMillis": int,
         "protocol": PortProtocolType,
@@ -749,55 +973,95 @@
     {
         "path": str,
         "port": int,
     },
     total=False,
 )
 
-
 class HealthCheckPolicyTypeDef(
     _RequiredHealthCheckPolicyTypeDef, _OptionalHealthCheckPolicyTypeDef
 ):
     pass
 
+HttpPathMatchOutputTypeDef = TypedDict(
+    "HttpPathMatchOutputTypeDef",
+    {
+        "exact": str,
+        "regex": str,
+    },
+    total=False,
+)
 
 HttpPathMatchTypeDef = TypedDict(
     "HttpPathMatchTypeDef",
     {
         "exact": str,
         "regex": str,
     },
     total=False,
 )
 
+HttpGatewayRoutePathRewriteOutputTypeDef = TypedDict(
+    "HttpGatewayRoutePathRewriteOutputTypeDef",
+    {
+        "exact": str,
+    },
+    total=False,
+)
+
 HttpGatewayRoutePathRewriteTypeDef = TypedDict(
     "HttpGatewayRoutePathRewriteTypeDef",
     {
         "exact": str,
     },
     total=False,
 )
 
+HttpGatewayRoutePrefixRewriteOutputTypeDef = TypedDict(
+    "HttpGatewayRoutePrefixRewriteOutputTypeDef",
+    {
+        "defaultPrefix": DefaultGatewayRouteRewriteType,
+        "value": str,
+    },
+    total=False,
+)
+
 HttpGatewayRoutePrefixRewriteTypeDef = TypedDict(
     "HttpGatewayRoutePrefixRewriteTypeDef",
     {
         "defaultPrefix": DefaultGatewayRouteRewriteType,
         "value": str,
     },
     total=False,
 )
 
+QueryParameterMatchOutputTypeDef = TypedDict(
+    "QueryParameterMatchOutputTypeDef",
+    {
+        "exact": str,
+    },
+    total=False,
+)
+
 QueryParameterMatchTypeDef = TypedDict(
     "QueryParameterMatchTypeDef",
     {
         "exact": str,
     },
     total=False,
 )
 
+JsonFormatRefOutputTypeDef = TypedDict(
+    "JsonFormatRefOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 JsonFormatRefTypeDef = TypedDict(
     "JsonFormatRefTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -814,22 +1078,20 @@
     {
         "meshOwner": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef(
     _RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
     _OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListGatewayRoutesInputRequestTypeDef = TypedDict(
     "_RequiredListGatewayRoutesInputRequestTypeDef",
     {
         "meshName": str,
         "virtualGatewayName": str,
     },
 )
@@ -839,21 +1101,19 @@
         "limit": int,
         "meshOwner": str,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListGatewayRoutesInputRequestTypeDef(
     _RequiredListGatewayRoutesInputRequestTypeDef, _OptionalListGatewayRoutesInputRequestTypeDef
 ):
     pass
 
-
 ListMeshesInputListMeshesPaginateTypeDef = TypedDict(
     "ListMeshesInputListMeshesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -892,22 +1152,20 @@
     {
         "meshOwner": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListRoutesInputListRoutesPaginateTypeDef(
     _RequiredListRoutesInputListRoutesPaginateTypeDef,
     _OptionalListRoutesInputListRoutesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListRoutesInputRequestTypeDef = TypedDict(
     "_RequiredListRoutesInputRequestTypeDef",
     {
         "meshName": str,
         "virtualRouterName": str,
     },
 )
@@ -917,21 +1175,19 @@
         "limit": int,
         "meshOwner": str,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListRoutesInputRequestTypeDef(
     _RequiredListRoutesInputRequestTypeDef, _OptionalListRoutesInputRequestTypeDef
 ):
     pass
 
-
 RouteRefTypeDef = TypedDict(
     "RouteRefTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "meshName": str,
@@ -953,22 +1209,20 @@
     "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
 ):
     pass
 
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -976,20 +1230,26 @@
     {
         "limit": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
+TagRefOutputTypeDef = TypedDict(
+    "TagRefOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
 
 _RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
     "_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
     {
         "meshName": str,
     },
 )
@@ -998,22 +1258,20 @@
     {
         "meshOwner": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef(
     _RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
     _OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListVirtualGatewaysInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualGatewaysInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualGatewaysInputRequestTypeDef = TypedDict(
@@ -1022,21 +1280,19 @@
         "limit": int,
         "meshOwner": str,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListVirtualGatewaysInputRequestTypeDef(
     _RequiredListVirtualGatewaysInputRequestTypeDef, _OptionalListVirtualGatewaysInputRequestTypeDef
 ):
     pass
 
-
 VirtualGatewayRefTypeDef = TypedDict(
     "VirtualGatewayRefTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "meshName": str,
@@ -1058,22 +1314,20 @@
     {
         "meshOwner": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListVirtualNodesInputListVirtualNodesPaginateTypeDef(
     _RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef,
     _OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListVirtualNodesInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualNodesInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualNodesInputRequestTypeDef = TypedDict(
@@ -1082,21 +1336,19 @@
         "limit": int,
         "meshOwner": str,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListVirtualNodesInputRequestTypeDef(
     _RequiredListVirtualNodesInputRequestTypeDef, _OptionalListVirtualNodesInputRequestTypeDef
 ):
     pass
 
-
 VirtualNodeRefTypeDef = TypedDict(
     "VirtualNodeRefTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "meshName": str,
@@ -1118,22 +1370,20 @@
     {
         "meshOwner": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef(
     _RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
     _OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListVirtualRoutersInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualRoutersInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualRoutersInputRequestTypeDef = TypedDict(
@@ -1142,21 +1392,19 @@
         "limit": int,
         "meshOwner": str,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListVirtualRoutersInputRequestTypeDef(
     _RequiredListVirtualRoutersInputRequestTypeDef, _OptionalListVirtualRoutersInputRequestTypeDef
 ):
     pass
 
-
 VirtualRouterRefTypeDef = TypedDict(
     "VirtualRouterRefTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "meshName": str,
@@ -1178,22 +1426,20 @@
     {
         "meshOwner": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListVirtualServicesInputListVirtualServicesPaginateTypeDef(
     _RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     _OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListVirtualServicesInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualServicesInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualServicesInputRequestTypeDef = TypedDict(
@@ -1202,42 +1448,69 @@
         "limit": int,
         "meshOwner": str,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListVirtualServicesInputRequestTypeDef(
     _RequiredListVirtualServicesInputRequestTypeDef, _OptionalListVirtualServicesInputRequestTypeDef
 ):
     pass
 
-
 VirtualServiceRefTypeDef = TypedDict(
     "VirtualServiceRefTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "meshName": str,
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualServiceName": str,
     },
 )
 
+PortMappingOutputTypeDef = TypedDict(
+    "PortMappingOutputTypeDef",
+    {
+        "port": int,
+        "protocol": PortProtocolType,
+    },
+)
+
+ListenerTlsAcmCertificateOutputTypeDef = TypedDict(
+    "ListenerTlsAcmCertificateOutputTypeDef",
+    {
+        "certificateArn": str,
+    },
+)
+
 ListenerTlsAcmCertificateTypeDef = TypedDict(
     "ListenerTlsAcmCertificateTypeDef",
     {
         "certificateArn": str,
     },
 )
 
+TlsValidationContextFileTrustOutputTypeDef = TypedDict(
+    "TlsValidationContextFileTrustOutputTypeDef",
+    {
+        "certificateChain": str,
+    },
+)
+
+TlsValidationContextSdsTrustOutputTypeDef = TypedDict(
+    "TlsValidationContextSdsTrustOutputTypeDef",
+    {
+        "secretName": str,
+    },
+)
+
 TlsValidationContextFileTrustTypeDef = TypedDict(
     "TlsValidationContextFileTrustTypeDef",
     {
         "certificateChain": str,
     },
 )
 
@@ -1260,14 +1533,22 @@
     "MeshStatusTypeDef",
     {
         "status": MeshStatusCodeType,
     },
     total=False,
 )
 
+MeshServiceDiscoveryOutputTypeDef = TypedDict(
+    "MeshServiceDiscoveryOutputTypeDef",
+    {
+        "ipPreference": IpPreferenceType,
+    },
+    total=False,
+)
+
 MeshServiceDiscoveryTypeDef = TypedDict(
     "MeshServiceDiscoveryTypeDef",
     {
         "ipPreference": IpPreferenceType,
     },
     total=False,
 )
@@ -1296,29 +1577,51 @@
 RouteStatusTypeDef = TypedDict(
     "RouteStatusTypeDef",
     {
         "status": RouteStatusCodeType,
     },
 )
 
+SubjectAlternativeNameMatchersOutputTypeDef = TypedDict(
+    "SubjectAlternativeNameMatchersOutputTypeDef",
+    {
+        "exact": List[str],
+    },
+)
+
 SubjectAlternativeNameMatchersTypeDef = TypedDict(
     "SubjectAlternativeNameMatchersTypeDef",
     {
         "exact": Sequence[str],
     },
 )
 
+TcpRouteMatchOutputTypeDef = TypedDict(
+    "TcpRouteMatchOutputTypeDef",
+    {
+        "port": int,
+    },
+    total=False,
+)
+
 TcpRouteMatchTypeDef = TypedDict(
     "TcpRouteMatchTypeDef",
     {
         "port": int,
     },
     total=False,
 )
 
+TlsValidationContextAcmTrustOutputTypeDef = TypedDict(
+    "TlsValidationContextAcmTrustOutputTypeDef",
+    {
+        "certificateAuthorityArns": List[str],
+    },
+)
+
 TlsValidationContextAcmTrustTypeDef = TypedDict(
     "TlsValidationContextAcmTrustTypeDef",
     {
         "certificateAuthorityArns": Sequence[str],
     },
 )
 
@@ -1326,14 +1629,29 @@
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+VirtualGatewayListenerTlsFileCertificateOutputTypeDef = TypedDict(
+    "VirtualGatewayListenerTlsFileCertificateOutputTypeDef",
+    {
+        "certificateChain": str,
+        "privateKey": str,
+    },
+)
+
+VirtualGatewayListenerTlsSdsCertificateOutputTypeDef = TypedDict(
+    "VirtualGatewayListenerTlsSdsCertificateOutputTypeDef",
+    {
+        "secretName": str,
+    },
+)
+
 VirtualGatewayListenerTlsFileCertificateTypeDef = TypedDict(
     "VirtualGatewayListenerTlsFileCertificateTypeDef",
     {
         "certificateChain": str,
         "privateKey": str,
     },
 )
@@ -1341,14 +1659,48 @@
 VirtualGatewayListenerTlsSdsCertificateTypeDef = TypedDict(
     "VirtualGatewayListenerTlsSdsCertificateTypeDef",
     {
         "secretName": str,
     },
 )
 
+VirtualGatewayGrpcConnectionPoolOutputTypeDef = TypedDict(
+    "VirtualGatewayGrpcConnectionPoolOutputTypeDef",
+    {
+        "maxRequests": int,
+    },
+)
+
+VirtualGatewayHttp2ConnectionPoolOutputTypeDef = TypedDict(
+    "VirtualGatewayHttp2ConnectionPoolOutputTypeDef",
+    {
+        "maxRequests": int,
+    },
+)
+
+_RequiredVirtualGatewayHttpConnectionPoolOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewayHttpConnectionPoolOutputTypeDef",
+    {
+        "maxConnections": int,
+    },
+)
+_OptionalVirtualGatewayHttpConnectionPoolOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewayHttpConnectionPoolOutputTypeDef",
+    {
+        "maxPendingRequests": int,
+    },
+    total=False,
+)
+
+class VirtualGatewayHttpConnectionPoolOutputTypeDef(
+    _RequiredVirtualGatewayHttpConnectionPoolOutputTypeDef,
+    _OptionalVirtualGatewayHttpConnectionPoolOutputTypeDef,
+):
+    pass
+
 VirtualGatewayGrpcConnectionPoolTypeDef = TypedDict(
     "VirtualGatewayGrpcConnectionPoolTypeDef",
     {
         "maxRequests": int,
     },
 )
 
@@ -1369,29 +1721,52 @@
     "_OptionalVirtualGatewayHttpConnectionPoolTypeDef",
     {
         "maxPendingRequests": int,
     },
     total=False,
 )
 
-
 class VirtualGatewayHttpConnectionPoolTypeDef(
     _RequiredVirtualGatewayHttpConnectionPoolTypeDef,
     _OptionalVirtualGatewayHttpConnectionPoolTypeDef,
 ):
     pass
 
-
 VirtualGatewayStatusTypeDef = TypedDict(
     "VirtualGatewayStatusTypeDef",
     {
         "status": VirtualGatewayStatusCodeType,
     },
 )
 
+_RequiredVirtualGatewayHealthCheckPolicyOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewayHealthCheckPolicyOutputTypeDef",
+    {
+        "healthyThreshold": int,
+        "intervalMillis": int,
+        "protocol": VirtualGatewayPortProtocolType,
+        "timeoutMillis": int,
+        "unhealthyThreshold": int,
+    },
+)
+_OptionalVirtualGatewayHealthCheckPolicyOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewayHealthCheckPolicyOutputTypeDef",
+    {
+        "path": str,
+        "port": int,
+    },
+    total=False,
+)
+
+class VirtualGatewayHealthCheckPolicyOutputTypeDef(
+    _RequiredVirtualGatewayHealthCheckPolicyOutputTypeDef,
+    _OptionalVirtualGatewayHealthCheckPolicyOutputTypeDef,
+):
+    pass
+
 _RequiredVirtualGatewayHealthCheckPolicyTypeDef = TypedDict(
     "_RequiredVirtualGatewayHealthCheckPolicyTypeDef",
     {
         "healthyThreshold": int,
         "intervalMillis": int,
         "protocol": VirtualGatewayPortProtocolType,
         "timeoutMillis": int,
@@ -1403,28 +1778,55 @@
     {
         "path": str,
         "port": int,
     },
     total=False,
 )
 
-
 class VirtualGatewayHealthCheckPolicyTypeDef(
     _RequiredVirtualGatewayHealthCheckPolicyTypeDef, _OptionalVirtualGatewayHealthCheckPolicyTypeDef
 ):
     pass
 
+VirtualGatewayPortMappingOutputTypeDef = TypedDict(
+    "VirtualGatewayPortMappingOutputTypeDef",
+    {
+        "port": int,
+        "protocol": VirtualGatewayPortProtocolType,
+    },
+)
+
+VirtualGatewayListenerTlsAcmCertificateOutputTypeDef = TypedDict(
+    "VirtualGatewayListenerTlsAcmCertificateOutputTypeDef",
+    {
+        "certificateArn": str,
+    },
+)
 
 VirtualGatewayListenerTlsAcmCertificateTypeDef = TypedDict(
     "VirtualGatewayListenerTlsAcmCertificateTypeDef",
     {
         "certificateArn": str,
     },
 )
 
+VirtualGatewayTlsValidationContextFileTrustOutputTypeDef = TypedDict(
+    "VirtualGatewayTlsValidationContextFileTrustOutputTypeDef",
+    {
+        "certificateChain": str,
+    },
+)
+
+VirtualGatewayTlsValidationContextSdsTrustOutputTypeDef = TypedDict(
+    "VirtualGatewayTlsValidationContextSdsTrustOutputTypeDef",
+    {
+        "secretName": str,
+    },
+)
+
 VirtualGatewayTlsValidationContextFileTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextFileTrustTypeDef",
     {
         "certificateChain": str,
     },
 )
 
@@ -1439,21 +1841,69 @@
     "VirtualGatewayPortMappingTypeDef",
     {
         "port": int,
         "protocol": VirtualGatewayPortProtocolType,
     },
 )
 
+VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef = TypedDict(
+    "VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef",
+    {
+        "certificateAuthorityArns": List[str],
+    },
+)
+
 VirtualGatewayTlsValidationContextAcmTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextAcmTrustTypeDef",
     {
         "certificateAuthorityArns": Sequence[str],
     },
 )
 
+VirtualNodeGrpcConnectionPoolOutputTypeDef = TypedDict(
+    "VirtualNodeGrpcConnectionPoolOutputTypeDef",
+    {
+        "maxRequests": int,
+    },
+)
+
+VirtualNodeHttp2ConnectionPoolOutputTypeDef = TypedDict(
+    "VirtualNodeHttp2ConnectionPoolOutputTypeDef",
+    {
+        "maxRequests": int,
+    },
+)
+
+_RequiredVirtualNodeHttpConnectionPoolOutputTypeDef = TypedDict(
+    "_RequiredVirtualNodeHttpConnectionPoolOutputTypeDef",
+    {
+        "maxConnections": int,
+    },
+)
+_OptionalVirtualNodeHttpConnectionPoolOutputTypeDef = TypedDict(
+    "_OptionalVirtualNodeHttpConnectionPoolOutputTypeDef",
+    {
+        "maxPendingRequests": int,
+    },
+    total=False,
+)
+
+class VirtualNodeHttpConnectionPoolOutputTypeDef(
+    _RequiredVirtualNodeHttpConnectionPoolOutputTypeDef,
+    _OptionalVirtualNodeHttpConnectionPoolOutputTypeDef,
+):
+    pass
+
+VirtualNodeTcpConnectionPoolOutputTypeDef = TypedDict(
+    "VirtualNodeTcpConnectionPoolOutputTypeDef",
+    {
+        "maxConnections": int,
+    },
+)
+
 VirtualNodeGrpcConnectionPoolTypeDef = TypedDict(
     "VirtualNodeGrpcConnectionPoolTypeDef",
     {
         "maxRequests": int,
     },
 )
 
@@ -1474,63 +1924,97 @@
     "_OptionalVirtualNodeHttpConnectionPoolTypeDef",
     {
         "maxPendingRequests": int,
     },
     total=False,
 )
 
-
 class VirtualNodeHttpConnectionPoolTypeDef(
     _RequiredVirtualNodeHttpConnectionPoolTypeDef, _OptionalVirtualNodeHttpConnectionPoolTypeDef
 ):
     pass
 
-
 VirtualNodeTcpConnectionPoolTypeDef = TypedDict(
     "VirtualNodeTcpConnectionPoolTypeDef",
     {
         "maxConnections": int,
     },
 )
 
 VirtualNodeStatusTypeDef = TypedDict(
     "VirtualNodeStatusTypeDef",
     {
         "status": VirtualNodeStatusCodeType,
     },
 )
 
+VirtualNodeServiceProviderOutputTypeDef = TypedDict(
+    "VirtualNodeServiceProviderOutputTypeDef",
+    {
+        "virtualNodeName": str,
+    },
+)
+
 VirtualNodeServiceProviderTypeDef = TypedDict(
     "VirtualNodeServiceProviderTypeDef",
     {
         "virtualNodeName": str,
     },
 )
 
 VirtualRouterStatusTypeDef = TypedDict(
     "VirtualRouterStatusTypeDef",
     {
         "status": VirtualRouterStatusCodeType,
     },
 )
 
+VirtualRouterServiceProviderOutputTypeDef = TypedDict(
+    "VirtualRouterServiceProviderOutputTypeDef",
+    {
+        "virtualRouterName": str,
+    },
+)
+
 VirtualRouterServiceProviderTypeDef = TypedDict(
     "VirtualRouterServiceProviderTypeDef",
     {
         "virtualRouterName": str,
     },
 )
 
 VirtualServiceStatusTypeDef = TypedDict(
     "VirtualServiceStatusTypeDef",
     {
         "status": VirtualServiceStatusCodeType,
     },
 )
 
+_RequiredAwsCloudMapServiceDiscoveryOutputTypeDef = TypedDict(
+    "_RequiredAwsCloudMapServiceDiscoveryOutputTypeDef",
+    {
+        "namespaceName": str,
+        "serviceName": str,
+    },
+)
+_OptionalAwsCloudMapServiceDiscoveryOutputTypeDef = TypedDict(
+    "_OptionalAwsCloudMapServiceDiscoveryOutputTypeDef",
+    {
+        "attributes": List[AwsCloudMapInstanceAttributeOutputTypeDef],
+        "ipPreference": IpPreferenceType,
+    },
+    total=False,
+)
+
+class AwsCloudMapServiceDiscoveryOutputTypeDef(
+    _RequiredAwsCloudMapServiceDiscoveryOutputTypeDef,
+    _OptionalAwsCloudMapServiceDiscoveryOutputTypeDef,
+):
+    pass
+
 _RequiredAwsCloudMapServiceDiscoveryTypeDef = TypedDict(
     "_RequiredAwsCloudMapServiceDiscoveryTypeDef",
     {
         "namespaceName": str,
         "serviceName": str,
     },
 )
@@ -1539,47 +2023,124 @@
     {
         "attributes": Sequence[AwsCloudMapInstanceAttributeTypeDef],
         "ipPreference": IpPreferenceType,
     },
     total=False,
 )
 
-
 class AwsCloudMapServiceDiscoveryTypeDef(
     _RequiredAwsCloudMapServiceDiscoveryTypeDef, _OptionalAwsCloudMapServiceDiscoveryTypeDef
 ):
     pass
 
+ClientTlsCertificateOutputTypeDef = TypedDict(
+    "ClientTlsCertificateOutputTypeDef",
+    {
+        "file": ListenerTlsFileCertificateOutputTypeDef,
+        "sds": ListenerTlsSdsCertificateOutputTypeDef,
+    },
+    total=False,
+)
 
 ClientTlsCertificateTypeDef = TypedDict(
     "ClientTlsCertificateTypeDef",
     {
         "file": ListenerTlsFileCertificateTypeDef,
         "sds": ListenerTlsSdsCertificateTypeDef,
     },
     total=False,
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "nextToken": str,
-        "tags": List[TagRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagRefTypeDef],
     },
 )
 
+_RequiredGrpcRetryPolicyOutputTypeDef = TypedDict(
+    "_RequiredGrpcRetryPolicyOutputTypeDef",
+    {
+        "maxRetries": int,
+        "perRetryTimeout": DurationOutputTypeDef,
+    },
+)
+_OptionalGrpcRetryPolicyOutputTypeDef = TypedDict(
+    "_OptionalGrpcRetryPolicyOutputTypeDef",
+    {
+        "grpcRetryEvents": List[GrpcRetryPolicyEventType],
+        "httpRetryEvents": List[str],
+        "tcpRetryEvents": List[Literal["connection-error"]],
+    },
+    total=False,
+)
+
+class GrpcRetryPolicyOutputTypeDef(
+    _RequiredGrpcRetryPolicyOutputTypeDef, _OptionalGrpcRetryPolicyOutputTypeDef
+):
+    pass
+
+GrpcTimeoutOutputTypeDef = TypedDict(
+    "GrpcTimeoutOutputTypeDef",
+    {
+        "idle": DurationOutputTypeDef,
+        "perRequest": DurationOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredHttpRetryPolicyOutputTypeDef = TypedDict(
+    "_RequiredHttpRetryPolicyOutputTypeDef",
+    {
+        "maxRetries": int,
+        "perRetryTimeout": DurationOutputTypeDef,
+    },
+)
+_OptionalHttpRetryPolicyOutputTypeDef = TypedDict(
+    "_OptionalHttpRetryPolicyOutputTypeDef",
+    {
+        "httpRetryEvents": List[str],
+        "tcpRetryEvents": List[Literal["connection-error"]],
+    },
+    total=False,
+)
+
+class HttpRetryPolicyOutputTypeDef(
+    _RequiredHttpRetryPolicyOutputTypeDef, _OptionalHttpRetryPolicyOutputTypeDef
+):
+    pass
+
+HttpTimeoutOutputTypeDef = TypedDict(
+    "HttpTimeoutOutputTypeDef",
+    {
+        "idle": DurationOutputTypeDef,
+        "perRequest": DurationOutputTypeDef,
+    },
+    total=False,
+)
+
+OutlierDetectionOutputTypeDef = TypedDict(
+    "OutlierDetectionOutputTypeDef",
+    {
+        "baseEjectionDuration": DurationOutputTypeDef,
+        "interval": DurationOutputTypeDef,
+        "maxEjectionPercent": int,
+        "maxServerErrors": int,
+    },
+)
+
+TcpTimeoutOutputTypeDef = TypedDict(
+    "TcpTimeoutOutputTypeDef",
+    {
+        "idle": DurationOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredGrpcRetryPolicyTypeDef = TypedDict(
     "_RequiredGrpcRetryPolicyTypeDef",
     {
         "maxRetries": int,
         "perRetryTimeout": DurationTypeDef,
     },
 )
@@ -1589,19 +2150,17 @@
         "grpcRetryEvents": Sequence[GrpcRetryPolicyEventType],
         "httpRetryEvents": Sequence[str],
         "tcpRetryEvents": Sequence[Literal["connection-error"]],
     },
     total=False,
 )
 
-
 class GrpcRetryPolicyTypeDef(_RequiredGrpcRetryPolicyTypeDef, _OptionalGrpcRetryPolicyTypeDef):
     pass
 
-
 GrpcTimeoutTypeDef = TypedDict(
     "GrpcTimeoutTypeDef",
     {
         "idle": DurationTypeDef,
         "perRequest": DurationTypeDef,
     },
     total=False,
@@ -1619,19 +2178,17 @@
     {
         "httpRetryEvents": Sequence[str],
         "tcpRetryEvents": Sequence[Literal["connection-error"]],
     },
     total=False,
 )
 
-
 class HttpRetryPolicyTypeDef(_RequiredHttpRetryPolicyTypeDef, _OptionalHttpRetryPolicyTypeDef):
     pass
 
-
 HttpTimeoutTypeDef = TypedDict(
     "HttpTimeoutTypeDef",
     {
         "idle": DurationTypeDef,
         "perRequest": DurationTypeDef,
     },
     total=False,
@@ -1651,14 +2208,22 @@
     "TcpTimeoutTypeDef",
     {
         "idle": DurationTypeDef,
     },
     total=False,
 )
 
+GrpcGatewayRouteRewriteOutputTypeDef = TypedDict(
+    "GrpcGatewayRouteRewriteOutputTypeDef",
+    {
+        "hostname": GatewayRouteHostnameRewriteOutputTypeDef,
+    },
+    total=False,
+)
+
 GrpcGatewayRouteRewriteTypeDef = TypedDict(
     "GrpcGatewayRouteRewriteTypeDef",
     {
         "hostname": GatewayRouteHostnameRewriteTypeDef,
     },
     total=False,
 )
@@ -1668,34 +2233,87 @@
     {
         "gatewayRoutes": List[GatewayRouteRefTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredGatewayRouteTargetOutputTypeDef = TypedDict(
+    "_RequiredGatewayRouteTargetOutputTypeDef",
+    {
+        "virtualService": GatewayRouteVirtualServiceOutputTypeDef,
+    },
+)
+_OptionalGatewayRouteTargetOutputTypeDef = TypedDict(
+    "_OptionalGatewayRouteTargetOutputTypeDef",
+    {
+        "port": int,
+    },
+    total=False,
+)
+
+class GatewayRouteTargetOutputTypeDef(
+    _RequiredGatewayRouteTargetOutputTypeDef, _OptionalGatewayRouteTargetOutputTypeDef
+):
+    pass
+
 _RequiredGatewayRouteTargetTypeDef = TypedDict(
     "_RequiredGatewayRouteTargetTypeDef",
     {
         "virtualService": GatewayRouteVirtualServiceTypeDef,
     },
 )
 _OptionalGatewayRouteTargetTypeDef = TypedDict(
     "_OptionalGatewayRouteTargetTypeDef",
     {
         "port": int,
     },
     total=False,
 )
 
-
 class GatewayRouteTargetTypeDef(
     _RequiredGatewayRouteTargetTypeDef, _OptionalGatewayRouteTargetTypeDef
 ):
     pass
 
+GrpcMetadataMatchMethodOutputTypeDef = TypedDict(
+    "GrpcMetadataMatchMethodOutputTypeDef",
+    {
+        "exact": str,
+        "prefix": str,
+        "range": MatchRangeOutputTypeDef,
+        "regex": str,
+        "suffix": str,
+    },
+    total=False,
+)
+
+GrpcRouteMetadataMatchMethodOutputTypeDef = TypedDict(
+    "GrpcRouteMetadataMatchMethodOutputTypeDef",
+    {
+        "exact": str,
+        "prefix": str,
+        "range": MatchRangeOutputTypeDef,
+        "regex": str,
+        "suffix": str,
+    },
+    total=False,
+)
+
+HeaderMatchMethodOutputTypeDef = TypedDict(
+    "HeaderMatchMethodOutputTypeDef",
+    {
+        "exact": str,
+        "prefix": str,
+        "range": MatchRangeOutputTypeDef,
+        "regex": str,
+        "suffix": str,
+    },
+    total=False,
+)
 
 GrpcMetadataMatchMethodTypeDef = TypedDict(
     "GrpcMetadataMatchMethodTypeDef",
     {
         "exact": str,
         "prefix": str,
         "range": MatchRangeTypeDef,
@@ -1725,14 +2343,35 @@
         "range": MatchRangeTypeDef,
         "regex": str,
         "suffix": str,
     },
     total=False,
 )
 
+GrpcRouteActionOutputTypeDef = TypedDict(
+    "GrpcRouteActionOutputTypeDef",
+    {
+        "weightedTargets": List[WeightedTargetOutputTypeDef],
+    },
+)
+
+HttpRouteActionOutputTypeDef = TypedDict(
+    "HttpRouteActionOutputTypeDef",
+    {
+        "weightedTargets": List[WeightedTargetOutputTypeDef],
+    },
+)
+
+TcpRouteActionOutputTypeDef = TypedDict(
+    "TcpRouteActionOutputTypeDef",
+    {
+        "weightedTargets": List[WeightedTargetOutputTypeDef],
+    },
+)
+
 GrpcRouteActionTypeDef = TypedDict(
     "GrpcRouteActionTypeDef",
     {
         "weightedTargets": Sequence[WeightedTargetTypeDef],
     },
 )
 
@@ -1746,44 +2385,80 @@
 TcpRouteActionTypeDef = TypedDict(
     "TcpRouteActionTypeDef",
     {
         "weightedTargets": Sequence[WeightedTargetTypeDef],
     },
 )
 
+HttpGatewayRouteRewriteOutputTypeDef = TypedDict(
+    "HttpGatewayRouteRewriteOutputTypeDef",
+    {
+        "hostname": GatewayRouteHostnameRewriteOutputTypeDef,
+        "path": HttpGatewayRoutePathRewriteOutputTypeDef,
+        "prefix": HttpGatewayRoutePrefixRewriteOutputTypeDef,
+    },
+    total=False,
+)
+
 HttpGatewayRouteRewriteTypeDef = TypedDict(
     "HttpGatewayRouteRewriteTypeDef",
     {
         "hostname": GatewayRouteHostnameRewriteTypeDef,
         "path": HttpGatewayRoutePathRewriteTypeDef,
         "prefix": HttpGatewayRoutePrefixRewriteTypeDef,
     },
     total=False,
 )
 
+_RequiredHttpQueryParameterOutputTypeDef = TypedDict(
+    "_RequiredHttpQueryParameterOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalHttpQueryParameterOutputTypeDef = TypedDict(
+    "_OptionalHttpQueryParameterOutputTypeDef",
+    {
+        "match": QueryParameterMatchOutputTypeDef,
+    },
+    total=False,
+)
+
+class HttpQueryParameterOutputTypeDef(
+    _RequiredHttpQueryParameterOutputTypeDef, _OptionalHttpQueryParameterOutputTypeDef
+):
+    pass
+
 _RequiredHttpQueryParameterTypeDef = TypedDict(
     "_RequiredHttpQueryParameterTypeDef",
     {
         "name": str,
     },
 )
 _OptionalHttpQueryParameterTypeDef = TypedDict(
     "_OptionalHttpQueryParameterTypeDef",
     {
         "match": QueryParameterMatchTypeDef,
     },
     total=False,
 )
 
-
 class HttpQueryParameterTypeDef(
     _RequiredHttpQueryParameterTypeDef, _OptionalHttpQueryParameterTypeDef
 ):
     pass
 
+LoggingFormatOutputTypeDef = TypedDict(
+    "LoggingFormatOutputTypeDef",
+    {
+        "json": List[JsonFormatRefOutputTypeDef],
+        "text": str,
+    },
+    total=False,
+)
 
 LoggingFormatTypeDef = TypedDict(
     "LoggingFormatTypeDef",
     {
         "json": Sequence[JsonFormatRefTypeDef],
         "text": str,
     },
@@ -1804,14 +2479,23 @@
     {
         "nextToken": str,
         "routes": List[RouteRefTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "nextToken": str,
+        "tags": List[TagRefOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListVirtualGatewaysOutputTypeDef = TypedDict(
     "ListVirtualGatewaysOutputTypeDef",
     {
         "nextToken": str,
         "virtualGateways": List[VirtualGatewayRefTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1840,24 +2524,50 @@
     {
         "nextToken": str,
         "virtualServices": List[VirtualServiceRefTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+VirtualRouterListenerOutputTypeDef = TypedDict(
+    "VirtualRouterListenerOutputTypeDef",
+    {
+        "portMapping": PortMappingOutputTypeDef,
+    },
+)
+
+ListenerTlsCertificateOutputTypeDef = TypedDict(
+    "ListenerTlsCertificateOutputTypeDef",
+    {
+        "acm": ListenerTlsAcmCertificateOutputTypeDef,
+        "file": ListenerTlsFileCertificateOutputTypeDef,
+        "sds": ListenerTlsSdsCertificateOutputTypeDef,
+    },
+    total=False,
+)
+
 ListenerTlsCertificateTypeDef = TypedDict(
     "ListenerTlsCertificateTypeDef",
     {
         "acm": ListenerTlsAcmCertificateTypeDef,
         "file": ListenerTlsFileCertificateTypeDef,
         "sds": ListenerTlsSdsCertificateTypeDef,
     },
     total=False,
 )
 
+ListenerTlsValidationContextTrustOutputTypeDef = TypedDict(
+    "ListenerTlsValidationContextTrustOutputTypeDef",
+    {
+        "file": TlsValidationContextFileTrustOutputTypeDef,
+        "sds": TlsValidationContextSdsTrustOutputTypeDef,
+    },
+    total=False,
+)
+
 ListenerTlsValidationContextTrustTypeDef = TypedDict(
     "ListenerTlsValidationContextTrustTypeDef",
     {
         "file": TlsValidationContextFileTrustTypeDef,
         "sds": TlsValidationContextSdsTrustTypeDef,
     },
     total=False,
@@ -1866,148 +2576,359 @@
 VirtualRouterListenerTypeDef = TypedDict(
     "VirtualRouterListenerTypeDef",
     {
         "portMapping": PortMappingTypeDef,
     },
 )
 
+MeshSpecOutputTypeDef = TypedDict(
+    "MeshSpecOutputTypeDef",
+    {
+        "egressFilter": EgressFilterOutputTypeDef,
+        "serviceDiscovery": MeshServiceDiscoveryOutputTypeDef,
+    },
+    total=False,
+)
+
 MeshSpecTypeDef = TypedDict(
     "MeshSpecTypeDef",
     {
         "egressFilter": EgressFilterTypeDef,
         "serviceDiscovery": MeshServiceDiscoveryTypeDef,
     },
     total=False,
 )
 
+SubjectAlternativeNamesOutputTypeDef = TypedDict(
+    "SubjectAlternativeNamesOutputTypeDef",
+    {
+        "match": SubjectAlternativeNameMatchersOutputTypeDef,
+    },
+)
+
 SubjectAlternativeNamesTypeDef = TypedDict(
     "SubjectAlternativeNamesTypeDef",
     {
         "match": SubjectAlternativeNameMatchersTypeDef,
     },
 )
 
+TlsValidationContextTrustOutputTypeDef = TypedDict(
+    "TlsValidationContextTrustOutputTypeDef",
+    {
+        "acm": TlsValidationContextAcmTrustOutputTypeDef,
+        "file": TlsValidationContextFileTrustOutputTypeDef,
+        "sds": TlsValidationContextSdsTrustOutputTypeDef,
+    },
+    total=False,
+)
+
 TlsValidationContextTrustTypeDef = TypedDict(
     "TlsValidationContextTrustTypeDef",
     {
         "acm": TlsValidationContextAcmTrustTypeDef,
         "file": TlsValidationContextFileTrustTypeDef,
         "sds": TlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
+VirtualGatewayClientTlsCertificateOutputTypeDef = TypedDict(
+    "VirtualGatewayClientTlsCertificateOutputTypeDef",
+    {
+        "file": VirtualGatewayListenerTlsFileCertificateOutputTypeDef,
+        "sds": VirtualGatewayListenerTlsSdsCertificateOutputTypeDef,
+    },
+    total=False,
+)
+
 VirtualGatewayClientTlsCertificateTypeDef = TypedDict(
     "VirtualGatewayClientTlsCertificateTypeDef",
     {
         "file": VirtualGatewayListenerTlsFileCertificateTypeDef,
         "sds": VirtualGatewayListenerTlsSdsCertificateTypeDef,
     },
     total=False,
 )
 
+VirtualGatewayConnectionPoolOutputTypeDef = TypedDict(
+    "VirtualGatewayConnectionPoolOutputTypeDef",
+    {
+        "grpc": VirtualGatewayGrpcConnectionPoolOutputTypeDef,
+        "http": VirtualGatewayHttpConnectionPoolOutputTypeDef,
+        "http2": VirtualGatewayHttp2ConnectionPoolOutputTypeDef,
+    },
+    total=False,
+)
+
 VirtualGatewayConnectionPoolTypeDef = TypedDict(
     "VirtualGatewayConnectionPoolTypeDef",
     {
         "grpc": VirtualGatewayGrpcConnectionPoolTypeDef,
         "http": VirtualGatewayHttpConnectionPoolTypeDef,
         "http2": VirtualGatewayHttp2ConnectionPoolTypeDef,
     },
     total=False,
 )
 
+VirtualGatewayListenerTlsCertificateOutputTypeDef = TypedDict(
+    "VirtualGatewayListenerTlsCertificateOutputTypeDef",
+    {
+        "acm": VirtualGatewayListenerTlsAcmCertificateOutputTypeDef,
+        "file": VirtualGatewayListenerTlsFileCertificateOutputTypeDef,
+        "sds": VirtualGatewayListenerTlsSdsCertificateOutputTypeDef,
+    },
+    total=False,
+)
+
 VirtualGatewayListenerTlsCertificateTypeDef = TypedDict(
     "VirtualGatewayListenerTlsCertificateTypeDef",
     {
         "acm": VirtualGatewayListenerTlsAcmCertificateTypeDef,
         "file": VirtualGatewayListenerTlsFileCertificateTypeDef,
         "sds": VirtualGatewayListenerTlsSdsCertificateTypeDef,
     },
     total=False,
 )
 
+VirtualGatewayListenerTlsValidationContextTrustOutputTypeDef = TypedDict(
+    "VirtualGatewayListenerTlsValidationContextTrustOutputTypeDef",
+    {
+        "file": VirtualGatewayTlsValidationContextFileTrustOutputTypeDef,
+        "sds": VirtualGatewayTlsValidationContextSdsTrustOutputTypeDef,
+    },
+    total=False,
+)
+
 VirtualGatewayListenerTlsValidationContextTrustTypeDef = TypedDict(
     "VirtualGatewayListenerTlsValidationContextTrustTypeDef",
     {
         "file": VirtualGatewayTlsValidationContextFileTrustTypeDef,
         "sds": VirtualGatewayTlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
+VirtualGatewayTlsValidationContextTrustOutputTypeDef = TypedDict(
+    "VirtualGatewayTlsValidationContextTrustOutputTypeDef",
+    {
+        "acm": VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef,
+        "file": VirtualGatewayTlsValidationContextFileTrustOutputTypeDef,
+        "sds": VirtualGatewayTlsValidationContextSdsTrustOutputTypeDef,
+    },
+    total=False,
+)
+
 VirtualGatewayTlsValidationContextTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextTrustTypeDef",
     {
         "acm": VirtualGatewayTlsValidationContextAcmTrustTypeDef,
         "file": VirtualGatewayTlsValidationContextFileTrustTypeDef,
         "sds": VirtualGatewayTlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
+VirtualNodeConnectionPoolOutputTypeDef = TypedDict(
+    "VirtualNodeConnectionPoolOutputTypeDef",
+    {
+        "grpc": VirtualNodeGrpcConnectionPoolOutputTypeDef,
+        "http": VirtualNodeHttpConnectionPoolOutputTypeDef,
+        "http2": VirtualNodeHttp2ConnectionPoolOutputTypeDef,
+        "tcp": VirtualNodeTcpConnectionPoolOutputTypeDef,
+    },
+    total=False,
+)
+
 VirtualNodeConnectionPoolTypeDef = TypedDict(
     "VirtualNodeConnectionPoolTypeDef",
     {
         "grpc": VirtualNodeGrpcConnectionPoolTypeDef,
         "http": VirtualNodeHttpConnectionPoolTypeDef,
         "http2": VirtualNodeHttp2ConnectionPoolTypeDef,
         "tcp": VirtualNodeTcpConnectionPoolTypeDef,
     },
     total=False,
 )
 
+VirtualServiceProviderOutputTypeDef = TypedDict(
+    "VirtualServiceProviderOutputTypeDef",
+    {
+        "virtualNode": VirtualNodeServiceProviderOutputTypeDef,
+        "virtualRouter": VirtualRouterServiceProviderOutputTypeDef,
+    },
+    total=False,
+)
+
 VirtualServiceProviderTypeDef = TypedDict(
     "VirtualServiceProviderTypeDef",
     {
         "virtualNode": VirtualNodeServiceProviderTypeDef,
         "virtualRouter": VirtualRouterServiceProviderTypeDef,
     },
     total=False,
 )
 
+ServiceDiscoveryOutputTypeDef = TypedDict(
+    "ServiceDiscoveryOutputTypeDef",
+    {
+        "awsCloudMap": AwsCloudMapServiceDiscoveryOutputTypeDef,
+        "dns": DnsServiceDiscoveryOutputTypeDef,
+    },
+    total=False,
+)
+
 ServiceDiscoveryTypeDef = TypedDict(
     "ServiceDiscoveryTypeDef",
     {
         "awsCloudMap": AwsCloudMapServiceDiscoveryTypeDef,
         "dns": DnsServiceDiscoveryTypeDef,
     },
     total=False,
 )
 
+ListenerTimeoutOutputTypeDef = TypedDict(
+    "ListenerTimeoutOutputTypeDef",
+    {
+        "grpc": GrpcTimeoutOutputTypeDef,
+        "http": HttpTimeoutOutputTypeDef,
+        "http2": HttpTimeoutOutputTypeDef,
+        "tcp": TcpTimeoutOutputTypeDef,
+    },
+    total=False,
+)
+
 ListenerTimeoutTypeDef = TypedDict(
     "ListenerTimeoutTypeDef",
     {
         "grpc": GrpcTimeoutTypeDef,
         "http": HttpTimeoutTypeDef,
         "http2": HttpTimeoutTypeDef,
         "tcp": TcpTimeoutTypeDef,
     },
     total=False,
 )
 
+_RequiredGrpcGatewayRouteActionOutputTypeDef = TypedDict(
+    "_RequiredGrpcGatewayRouteActionOutputTypeDef",
+    {
+        "target": GatewayRouteTargetOutputTypeDef,
+    },
+)
+_OptionalGrpcGatewayRouteActionOutputTypeDef = TypedDict(
+    "_OptionalGrpcGatewayRouteActionOutputTypeDef",
+    {
+        "rewrite": GrpcGatewayRouteRewriteOutputTypeDef,
+    },
+    total=False,
+)
+
+class GrpcGatewayRouteActionOutputTypeDef(
+    _RequiredGrpcGatewayRouteActionOutputTypeDef, _OptionalGrpcGatewayRouteActionOutputTypeDef
+):
+    pass
+
 _RequiredGrpcGatewayRouteActionTypeDef = TypedDict(
     "_RequiredGrpcGatewayRouteActionTypeDef",
     {
         "target": GatewayRouteTargetTypeDef,
     },
 )
 _OptionalGrpcGatewayRouteActionTypeDef = TypedDict(
     "_OptionalGrpcGatewayRouteActionTypeDef",
     {
         "rewrite": GrpcGatewayRouteRewriteTypeDef,
     },
     total=False,
 )
 
-
 class GrpcGatewayRouteActionTypeDef(
     _RequiredGrpcGatewayRouteActionTypeDef, _OptionalGrpcGatewayRouteActionTypeDef
 ):
     pass
 
+_RequiredGrpcGatewayRouteMetadataOutputTypeDef = TypedDict(
+    "_RequiredGrpcGatewayRouteMetadataOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalGrpcGatewayRouteMetadataOutputTypeDef = TypedDict(
+    "_OptionalGrpcGatewayRouteMetadataOutputTypeDef",
+    {
+        "invert": bool,
+        "match": GrpcMetadataMatchMethodOutputTypeDef,
+    },
+    total=False,
+)
+
+class GrpcGatewayRouteMetadataOutputTypeDef(
+    _RequiredGrpcGatewayRouteMetadataOutputTypeDef, _OptionalGrpcGatewayRouteMetadataOutputTypeDef
+):
+    pass
+
+_RequiredGrpcRouteMetadataOutputTypeDef = TypedDict(
+    "_RequiredGrpcRouteMetadataOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalGrpcRouteMetadataOutputTypeDef = TypedDict(
+    "_OptionalGrpcRouteMetadataOutputTypeDef",
+    {
+        "invert": bool,
+        "match": GrpcRouteMetadataMatchMethodOutputTypeDef,
+    },
+    total=False,
+)
+
+class GrpcRouteMetadataOutputTypeDef(
+    _RequiredGrpcRouteMetadataOutputTypeDef, _OptionalGrpcRouteMetadataOutputTypeDef
+):
+    pass
+
+_RequiredHttpGatewayRouteHeaderOutputTypeDef = TypedDict(
+    "_RequiredHttpGatewayRouteHeaderOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalHttpGatewayRouteHeaderOutputTypeDef = TypedDict(
+    "_OptionalHttpGatewayRouteHeaderOutputTypeDef",
+    {
+        "invert": bool,
+        "match": HeaderMatchMethodOutputTypeDef,
+    },
+    total=False,
+)
+
+class HttpGatewayRouteHeaderOutputTypeDef(
+    _RequiredHttpGatewayRouteHeaderOutputTypeDef, _OptionalHttpGatewayRouteHeaderOutputTypeDef
+):
+    pass
+
+_RequiredHttpRouteHeaderOutputTypeDef = TypedDict(
+    "_RequiredHttpRouteHeaderOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalHttpRouteHeaderOutputTypeDef = TypedDict(
+    "_OptionalHttpRouteHeaderOutputTypeDef",
+    {
+        "invert": bool,
+        "match": HeaderMatchMethodOutputTypeDef,
+    },
+    total=False,
+)
+
+class HttpRouteHeaderOutputTypeDef(
+    _RequiredHttpRouteHeaderOutputTypeDef, _OptionalHttpRouteHeaderOutputTypeDef
+):
+    pass
 
 _RequiredGrpcGatewayRouteMetadataTypeDef = TypedDict(
     "_RequiredGrpcGatewayRouteMetadataTypeDef",
     {
         "name": str,
     },
 )
@@ -2016,21 +2937,19 @@
     {
         "invert": bool,
         "match": GrpcMetadataMatchMethodTypeDef,
     },
     total=False,
 )
 
-
 class GrpcGatewayRouteMetadataTypeDef(
     _RequiredGrpcGatewayRouteMetadataTypeDef, _OptionalGrpcGatewayRouteMetadataTypeDef
 ):
     pass
 
-
 _RequiredGrpcRouteMetadataTypeDef = TypedDict(
     "_RequiredGrpcRouteMetadataTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGrpcRouteMetadataTypeDef = TypedDict(
@@ -2038,21 +2957,19 @@
     {
         "invert": bool,
         "match": GrpcRouteMetadataMatchMethodTypeDef,
     },
     total=False,
 )
 
-
 class GrpcRouteMetadataTypeDef(
     _RequiredGrpcRouteMetadataTypeDef, _OptionalGrpcRouteMetadataTypeDef
 ):
     pass
 
-
 _RequiredHttpGatewayRouteHeaderTypeDef = TypedDict(
     "_RequiredHttpGatewayRouteHeaderTypeDef",
     {
         "name": str,
     },
 )
 _OptionalHttpGatewayRouteHeaderTypeDef = TypedDict(
@@ -2060,21 +2977,19 @@
     {
         "invert": bool,
         "match": HeaderMatchMethodTypeDef,
     },
     total=False,
 )
 
-
 class HttpGatewayRouteHeaderTypeDef(
     _RequiredHttpGatewayRouteHeaderTypeDef, _OptionalHttpGatewayRouteHeaderTypeDef
 ):
     pass
 
-
 _RequiredHttpRouteHeaderTypeDef = TypedDict(
     "_RequiredHttpRouteHeaderTypeDef",
     {
         "name": str,
     },
 )
 _OptionalHttpRouteHeaderTypeDef = TypedDict(
@@ -2082,18 +2997,34 @@
     {
         "invert": bool,
         "match": HeaderMatchMethodTypeDef,
     },
     total=False,
 )
 
-
 class HttpRouteHeaderTypeDef(_RequiredHttpRouteHeaderTypeDef, _OptionalHttpRouteHeaderTypeDef):
     pass
 
+_RequiredTcpRouteOutputTypeDef = TypedDict(
+    "_RequiredTcpRouteOutputTypeDef",
+    {
+        "action": TcpRouteActionOutputTypeDef,
+    },
+)
+_OptionalTcpRouteOutputTypeDef = TypedDict(
+    "_OptionalTcpRouteOutputTypeDef",
+    {
+        "match": TcpRouteMatchOutputTypeDef,
+        "timeout": TcpTimeoutOutputTypeDef,
+    },
+    total=False,
+)
+
+class TcpRouteOutputTypeDef(_RequiredTcpRouteOutputTypeDef, _OptionalTcpRouteOutputTypeDef):
+    pass
 
 _RequiredTcpRouteTypeDef = TypedDict(
     "_RequiredTcpRouteTypeDef",
     {
         "action": TcpRouteActionTypeDef,
     },
 )
@@ -2102,18 +3033,35 @@
     {
         "match": TcpRouteMatchTypeDef,
         "timeout": TcpTimeoutTypeDef,
     },
     total=False,
 )
 
-
 class TcpRouteTypeDef(_RequiredTcpRouteTypeDef, _OptionalTcpRouteTypeDef):
     pass
 
+_RequiredHttpGatewayRouteActionOutputTypeDef = TypedDict(
+    "_RequiredHttpGatewayRouteActionOutputTypeDef",
+    {
+        "target": GatewayRouteTargetOutputTypeDef,
+    },
+)
+_OptionalHttpGatewayRouteActionOutputTypeDef = TypedDict(
+    "_OptionalHttpGatewayRouteActionOutputTypeDef",
+    {
+        "rewrite": HttpGatewayRouteRewriteOutputTypeDef,
+    },
+    total=False,
+)
+
+class HttpGatewayRouteActionOutputTypeDef(
+    _RequiredHttpGatewayRouteActionOutputTypeDef, _OptionalHttpGatewayRouteActionOutputTypeDef
+):
+    pass
 
 _RequiredHttpGatewayRouteActionTypeDef = TypedDict(
     "_RequiredHttpGatewayRouteActionTypeDef",
     {
         "target": GatewayRouteTargetTypeDef,
     },
 )
@@ -2121,20 +3069,57 @@
     "_OptionalHttpGatewayRouteActionTypeDef",
     {
         "rewrite": HttpGatewayRouteRewriteTypeDef,
     },
     total=False,
 )
 
-
 class HttpGatewayRouteActionTypeDef(
     _RequiredHttpGatewayRouteActionTypeDef, _OptionalHttpGatewayRouteActionTypeDef
 ):
     pass
 
+_RequiredFileAccessLogOutputTypeDef = TypedDict(
+    "_RequiredFileAccessLogOutputTypeDef",
+    {
+        "path": str,
+    },
+)
+_OptionalFileAccessLogOutputTypeDef = TypedDict(
+    "_OptionalFileAccessLogOutputTypeDef",
+    {
+        "format": LoggingFormatOutputTypeDef,
+    },
+    total=False,
+)
+
+class FileAccessLogOutputTypeDef(
+    _RequiredFileAccessLogOutputTypeDef, _OptionalFileAccessLogOutputTypeDef
+):
+    pass
+
+_RequiredVirtualGatewayFileAccessLogOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewayFileAccessLogOutputTypeDef",
+    {
+        "path": str,
+    },
+)
+_OptionalVirtualGatewayFileAccessLogOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewayFileAccessLogOutputTypeDef",
+    {
+        "format": LoggingFormatOutputTypeDef,
+    },
+    total=False,
+)
+
+class VirtualGatewayFileAccessLogOutputTypeDef(
+    _RequiredVirtualGatewayFileAccessLogOutputTypeDef,
+    _OptionalVirtualGatewayFileAccessLogOutputTypeDef,
+):
+    pass
 
 _RequiredFileAccessLogTypeDef = TypedDict(
     "_RequiredFileAccessLogTypeDef",
     {
         "path": str,
     },
 )
@@ -2142,48 +3127,62 @@
     "_OptionalFileAccessLogTypeDef",
     {
         "format": LoggingFormatTypeDef,
     },
     total=False,
 )
 
-
 class FileAccessLogTypeDef(_RequiredFileAccessLogTypeDef, _OptionalFileAccessLogTypeDef):
     pass
 
-
 _RequiredVirtualGatewayFileAccessLogTypeDef = TypedDict(
     "_RequiredVirtualGatewayFileAccessLogTypeDef",
     {
         "path": str,
     },
 )
 _OptionalVirtualGatewayFileAccessLogTypeDef = TypedDict(
     "_OptionalVirtualGatewayFileAccessLogTypeDef",
     {
         "format": LoggingFormatTypeDef,
     },
     total=False,
 )
 
-
 class VirtualGatewayFileAccessLogTypeDef(
     _RequiredVirtualGatewayFileAccessLogTypeDef, _OptionalVirtualGatewayFileAccessLogTypeDef
 ):
     pass
 
+VirtualRouterSpecOutputTypeDef = TypedDict(
+    "VirtualRouterSpecOutputTypeDef",
+    {
+        "listeners": List[VirtualRouterListenerOutputTypeDef],
+    },
+    total=False,
+)
 
 VirtualRouterSpecTypeDef = TypedDict(
     "VirtualRouterSpecTypeDef",
     {
         "listeners": Sequence[VirtualRouterListenerTypeDef],
     },
     total=False,
 )
 
+MeshDataTypeDef = TypedDict(
+    "MeshDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "spec": MeshSpecOutputTypeDef,
+        "status": MeshStatusTypeDef,
+    },
+)
+
 _RequiredCreateMeshInputRequestTypeDef = TypedDict(
     "_RequiredCreateMeshInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalCreateMeshInputRequestTypeDef = TypedDict(
@@ -2192,31 +3191,19 @@
         "clientToken": str,
         "spec": MeshSpecTypeDef,
         "tags": Sequence[TagRefTypeDef],
     },
     total=False,
 )
 
-
 class CreateMeshInputRequestTypeDef(
     _RequiredCreateMeshInputRequestTypeDef, _OptionalCreateMeshInputRequestTypeDef
 ):
     pass
 
-
-MeshDataTypeDef = TypedDict(
-    "MeshDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "spec": MeshSpecTypeDef,
-        "status": MeshStatusTypeDef,
-    },
-)
-
 _RequiredUpdateMeshInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMeshInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalUpdateMeshInputRequestTypeDef = TypedDict(
@@ -2224,20 +3211,38 @@
     {
         "clientToken": str,
         "spec": MeshSpecTypeDef,
     },
     total=False,
 )
 
-
 class UpdateMeshInputRequestTypeDef(
     _RequiredUpdateMeshInputRequestTypeDef, _OptionalUpdateMeshInputRequestTypeDef
 ):
     pass
 
+_RequiredListenerTlsValidationContextOutputTypeDef = TypedDict(
+    "_RequiredListenerTlsValidationContextOutputTypeDef",
+    {
+        "trust": ListenerTlsValidationContextTrustOutputTypeDef,
+    },
+)
+_OptionalListenerTlsValidationContextOutputTypeDef = TypedDict(
+    "_OptionalListenerTlsValidationContextOutputTypeDef",
+    {
+        "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+class ListenerTlsValidationContextOutputTypeDef(
+    _RequiredListenerTlsValidationContextOutputTypeDef,
+    _OptionalListenerTlsValidationContextOutputTypeDef,
+):
+    pass
 
 _RequiredListenerTlsValidationContextTypeDef = TypedDict(
     "_RequiredListenerTlsValidationContextTypeDef",
     {
         "trust": ListenerTlsValidationContextTrustTypeDef,
     },
 )
@@ -2245,20 +3250,37 @@
     "_OptionalListenerTlsValidationContextTypeDef",
     {
         "subjectAlternativeNames": SubjectAlternativeNamesTypeDef,
     },
     total=False,
 )
 
-
 class ListenerTlsValidationContextTypeDef(
     _RequiredListenerTlsValidationContextTypeDef, _OptionalListenerTlsValidationContextTypeDef
 ):
     pass
 
+_RequiredTlsValidationContextOutputTypeDef = TypedDict(
+    "_RequiredTlsValidationContextOutputTypeDef",
+    {
+        "trust": TlsValidationContextTrustOutputTypeDef,
+    },
+)
+_OptionalTlsValidationContextOutputTypeDef = TypedDict(
+    "_OptionalTlsValidationContextOutputTypeDef",
+    {
+        "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+class TlsValidationContextOutputTypeDef(
+    _RequiredTlsValidationContextOutputTypeDef, _OptionalTlsValidationContextOutputTypeDef
+):
+    pass
 
 _RequiredTlsValidationContextTypeDef = TypedDict(
     "_RequiredTlsValidationContextTypeDef",
     {
         "trust": TlsValidationContextTrustTypeDef,
     },
 )
@@ -2266,20 +3288,38 @@
     "_OptionalTlsValidationContextTypeDef",
     {
         "subjectAlternativeNames": SubjectAlternativeNamesTypeDef,
     },
     total=False,
 )
 
-
 class TlsValidationContextTypeDef(
     _RequiredTlsValidationContextTypeDef, _OptionalTlsValidationContextTypeDef
 ):
     pass
 
+_RequiredVirtualGatewayListenerTlsValidationContextOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewayListenerTlsValidationContextOutputTypeDef",
+    {
+        "trust": VirtualGatewayListenerTlsValidationContextTrustOutputTypeDef,
+    },
+)
+_OptionalVirtualGatewayListenerTlsValidationContextOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewayListenerTlsValidationContextOutputTypeDef",
+    {
+        "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+class VirtualGatewayListenerTlsValidationContextOutputTypeDef(
+    _RequiredVirtualGatewayListenerTlsValidationContextOutputTypeDef,
+    _OptionalVirtualGatewayListenerTlsValidationContextOutputTypeDef,
+):
+    pass
 
 _RequiredVirtualGatewayListenerTlsValidationContextTypeDef = TypedDict(
     "_RequiredVirtualGatewayListenerTlsValidationContextTypeDef",
     {
         "trust": VirtualGatewayListenerTlsValidationContextTrustTypeDef,
     },
 )
@@ -2287,21 +3327,39 @@
     "_OptionalVirtualGatewayListenerTlsValidationContextTypeDef",
     {
         "subjectAlternativeNames": SubjectAlternativeNamesTypeDef,
     },
     total=False,
 )
 
-
 class VirtualGatewayListenerTlsValidationContextTypeDef(
     _RequiredVirtualGatewayListenerTlsValidationContextTypeDef,
     _OptionalVirtualGatewayListenerTlsValidationContextTypeDef,
 ):
     pass
 
+_RequiredVirtualGatewayTlsValidationContextOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewayTlsValidationContextOutputTypeDef",
+    {
+        "trust": VirtualGatewayTlsValidationContextTrustOutputTypeDef,
+    },
+)
+_OptionalVirtualGatewayTlsValidationContextOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewayTlsValidationContextOutputTypeDef",
+    {
+        "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+class VirtualGatewayTlsValidationContextOutputTypeDef(
+    _RequiredVirtualGatewayTlsValidationContextOutputTypeDef,
+    _OptionalVirtualGatewayTlsValidationContextOutputTypeDef,
+):
+    pass
 
 _RequiredVirtualGatewayTlsValidationContextTypeDef = TypedDict(
     "_RequiredVirtualGatewayTlsValidationContextTypeDef",
     {
         "trust": VirtualGatewayTlsValidationContextTrustTypeDef,
     },
 )
@@ -2309,30 +3367,86 @@
     "_OptionalVirtualGatewayTlsValidationContextTypeDef",
     {
         "subjectAlternativeNames": SubjectAlternativeNamesTypeDef,
     },
     total=False,
 )
 
-
 class VirtualGatewayTlsValidationContextTypeDef(
     _RequiredVirtualGatewayTlsValidationContextTypeDef,
     _OptionalVirtualGatewayTlsValidationContextTypeDef,
 ):
     pass
 
+VirtualServiceSpecOutputTypeDef = TypedDict(
+    "VirtualServiceSpecOutputTypeDef",
+    {
+        "provider": VirtualServiceProviderOutputTypeDef,
+    },
+    total=False,
+)
 
 VirtualServiceSpecTypeDef = TypedDict(
     "VirtualServiceSpecTypeDef",
     {
         "provider": VirtualServiceProviderTypeDef,
     },
     total=False,
 )
 
+GrpcGatewayRouteMatchOutputTypeDef = TypedDict(
+    "GrpcGatewayRouteMatchOutputTypeDef",
+    {
+        "hostname": GatewayRouteHostnameMatchOutputTypeDef,
+        "metadata": List[GrpcGatewayRouteMetadataOutputTypeDef],
+        "port": int,
+        "serviceName": str,
+    },
+    total=False,
+)
+
+GrpcRouteMatchOutputTypeDef = TypedDict(
+    "GrpcRouteMatchOutputTypeDef",
+    {
+        "metadata": List[GrpcRouteMetadataOutputTypeDef],
+        "methodName": str,
+        "port": int,
+        "serviceName": str,
+    },
+    total=False,
+)
+
+HttpGatewayRouteMatchOutputTypeDef = TypedDict(
+    "HttpGatewayRouteMatchOutputTypeDef",
+    {
+        "headers": List[HttpGatewayRouteHeaderOutputTypeDef],
+        "hostname": GatewayRouteHostnameMatchOutputTypeDef,
+        "method": HttpMethodType,
+        "path": HttpPathMatchOutputTypeDef,
+        "port": int,
+        "prefix": str,
+        "queryParameters": List[HttpQueryParameterOutputTypeDef],
+    },
+    total=False,
+)
+
+HttpRouteMatchOutputTypeDef = TypedDict(
+    "HttpRouteMatchOutputTypeDef",
+    {
+        "headers": List[HttpRouteHeaderOutputTypeDef],
+        "method": HttpMethodType,
+        "path": HttpPathMatchOutputTypeDef,
+        "port": int,
+        "prefix": str,
+        "queryParameters": List[HttpQueryParameterOutputTypeDef],
+        "scheme": HttpSchemeType,
+    },
+    total=False,
+)
+
 GrpcGatewayRouteMatchTypeDef = TypedDict(
     "GrpcGatewayRouteMatchTypeDef",
     {
         "hostname": GatewayRouteHostnameMatchTypeDef,
         "metadata": Sequence[GrpcGatewayRouteMetadataTypeDef],
         "port": int,
         "serviceName": str,
@@ -2375,14 +3489,30 @@
         "prefix": str,
         "queryParameters": Sequence[HttpQueryParameterTypeDef],
         "scheme": HttpSchemeType,
     },
     total=False,
 )
 
+AccessLogOutputTypeDef = TypedDict(
+    "AccessLogOutputTypeDef",
+    {
+        "file": FileAccessLogOutputTypeDef,
+    },
+    total=False,
+)
+
+VirtualGatewayAccessLogOutputTypeDef = TypedDict(
+    "VirtualGatewayAccessLogOutputTypeDef",
+    {
+        "file": VirtualGatewayFileAccessLogOutputTypeDef,
+    },
+    total=False,
+)
+
 AccessLogTypeDef = TypedDict(
     "AccessLogTypeDef",
     {
         "file": FileAccessLogTypeDef,
     },
     total=False,
 )
@@ -2391,14 +3521,25 @@
     "VirtualGatewayAccessLogTypeDef",
     {
         "file": VirtualGatewayFileAccessLogTypeDef,
     },
     total=False,
 )
 
+VirtualRouterDataTypeDef = TypedDict(
+    "VirtualRouterDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "spec": VirtualRouterSpecOutputTypeDef,
+        "status": VirtualRouterStatusTypeDef,
+        "virtualRouterName": str,
+    },
+)
+
 _RequiredCreateVirtualRouterInputRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualRouterInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualRouterSpecTypeDef,
         "virtualRouterName": str,
     },
@@ -2409,21 +3550,19 @@
         "clientToken": str,
         "meshOwner": str,
         "tags": Sequence[TagRefTypeDef],
     },
     total=False,
 )
 
-
 class CreateVirtualRouterInputRequestTypeDef(
     _RequiredCreateVirtualRouterInputRequestTypeDef, _OptionalCreateVirtualRouterInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateVirtualRouterInputRequestTypeDef = TypedDict(
     "_RequiredUpdateVirtualRouterInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualRouterSpecTypeDef,
         "virtualRouterName": str,
     },
@@ -2433,32 +3572,19 @@
     {
         "clientToken": str,
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class UpdateVirtualRouterInputRequestTypeDef(
     _RequiredUpdateVirtualRouterInputRequestTypeDef, _OptionalUpdateVirtualRouterInputRequestTypeDef
 ):
     pass
 
-
-VirtualRouterDataTypeDef = TypedDict(
-    "VirtualRouterDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "spec": VirtualRouterSpecTypeDef,
-        "status": VirtualRouterStatusTypeDef,
-        "virtualRouterName": str,
-    },
-)
-
 CreateMeshOutputTypeDef = TypedDict(
     "CreateMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2483,14 +3609,34 @@
     "UpdateMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredListenerTlsOutputTypeDef = TypedDict(
+    "_RequiredListenerTlsOutputTypeDef",
+    {
+        "certificate": ListenerTlsCertificateOutputTypeDef,
+        "mode": ListenerTlsModeType,
+    },
+)
+_OptionalListenerTlsOutputTypeDef = TypedDict(
+    "_OptionalListenerTlsOutputTypeDef",
+    {
+        "validation": ListenerTlsValidationContextOutputTypeDef,
+    },
+    total=False,
+)
+
+class ListenerTlsOutputTypeDef(
+    _RequiredListenerTlsOutputTypeDef, _OptionalListenerTlsOutputTypeDef
+):
+    pass
+
 _RequiredListenerTlsTypeDef = TypedDict(
     "_RequiredListenerTlsTypeDef",
     {
         "certificate": ListenerTlsCertificateTypeDef,
         "mode": ListenerTlsModeType,
     },
 )
@@ -2498,18 +3644,37 @@
     "_OptionalListenerTlsTypeDef",
     {
         "validation": ListenerTlsValidationContextTypeDef,
     },
     total=False,
 )
 
-
 class ListenerTlsTypeDef(_RequiredListenerTlsTypeDef, _OptionalListenerTlsTypeDef):
     pass
 
+_RequiredClientPolicyTlsOutputTypeDef = TypedDict(
+    "_RequiredClientPolicyTlsOutputTypeDef",
+    {
+        "validation": TlsValidationContextOutputTypeDef,
+    },
+)
+_OptionalClientPolicyTlsOutputTypeDef = TypedDict(
+    "_OptionalClientPolicyTlsOutputTypeDef",
+    {
+        "certificate": ClientTlsCertificateOutputTypeDef,
+        "enforce": bool,
+        "ports": List[int],
+    },
+    total=False,
+)
+
+class ClientPolicyTlsOutputTypeDef(
+    _RequiredClientPolicyTlsOutputTypeDef, _OptionalClientPolicyTlsOutputTypeDef
+):
+    pass
 
 _RequiredClientPolicyTlsTypeDef = TypedDict(
     "_RequiredClientPolicyTlsTypeDef",
     {
         "validation": TlsValidationContextTypeDef,
     },
 )
@@ -2519,18 +3684,36 @@
         "certificate": ClientTlsCertificateTypeDef,
         "enforce": bool,
         "ports": Sequence[int],
     },
     total=False,
 )
 
-
 class ClientPolicyTlsTypeDef(_RequiredClientPolicyTlsTypeDef, _OptionalClientPolicyTlsTypeDef):
     pass
 
+_RequiredVirtualGatewayListenerTlsOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewayListenerTlsOutputTypeDef",
+    {
+        "certificate": VirtualGatewayListenerTlsCertificateOutputTypeDef,
+        "mode": VirtualGatewayListenerTlsModeType,
+    },
+)
+_OptionalVirtualGatewayListenerTlsOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewayListenerTlsOutputTypeDef",
+    {
+        "validation": VirtualGatewayListenerTlsValidationContextOutputTypeDef,
+    },
+    total=False,
+)
+
+class VirtualGatewayListenerTlsOutputTypeDef(
+    _RequiredVirtualGatewayListenerTlsOutputTypeDef, _OptionalVirtualGatewayListenerTlsOutputTypeDef
+):
+    pass
 
 _RequiredVirtualGatewayListenerTlsTypeDef = TypedDict(
     "_RequiredVirtualGatewayListenerTlsTypeDef",
     {
         "certificate": VirtualGatewayListenerTlsCertificateTypeDef,
         "mode": VirtualGatewayListenerTlsModeType,
     },
@@ -2539,20 +3722,40 @@
     "_OptionalVirtualGatewayListenerTlsTypeDef",
     {
         "validation": VirtualGatewayListenerTlsValidationContextTypeDef,
     },
     total=False,
 )
 
-
 class VirtualGatewayListenerTlsTypeDef(
     _RequiredVirtualGatewayListenerTlsTypeDef, _OptionalVirtualGatewayListenerTlsTypeDef
 ):
     pass
 
+_RequiredVirtualGatewayClientPolicyTlsOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewayClientPolicyTlsOutputTypeDef",
+    {
+        "validation": VirtualGatewayTlsValidationContextOutputTypeDef,
+    },
+)
+_OptionalVirtualGatewayClientPolicyTlsOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewayClientPolicyTlsOutputTypeDef",
+    {
+        "certificate": VirtualGatewayClientTlsCertificateOutputTypeDef,
+        "enforce": bool,
+        "ports": List[int],
+    },
+    total=False,
+)
+
+class VirtualGatewayClientPolicyTlsOutputTypeDef(
+    _RequiredVirtualGatewayClientPolicyTlsOutputTypeDef,
+    _OptionalVirtualGatewayClientPolicyTlsOutputTypeDef,
+):
+    pass
 
 _RequiredVirtualGatewayClientPolicyTlsTypeDef = TypedDict(
     "_RequiredVirtualGatewayClientPolicyTlsTypeDef",
     {
         "validation": VirtualGatewayTlsValidationContextTypeDef,
     },
 )
@@ -2562,20 +3765,29 @@
         "certificate": VirtualGatewayClientTlsCertificateTypeDef,
         "enforce": bool,
         "ports": Sequence[int],
     },
     total=False,
 )
 
-
 class VirtualGatewayClientPolicyTlsTypeDef(
     _RequiredVirtualGatewayClientPolicyTlsTypeDef, _OptionalVirtualGatewayClientPolicyTlsTypeDef
 ):
     pass
 
+VirtualServiceDataTypeDef = TypedDict(
+    "VirtualServiceDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "spec": VirtualServiceSpecOutputTypeDef,
+        "status": VirtualServiceStatusTypeDef,
+        "virtualServiceName": str,
+    },
+)
 
 _RequiredCreateVirtualServiceInputRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualServiceInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualServiceSpecTypeDef,
         "virtualServiceName": str,
@@ -2587,22 +3799,20 @@
         "clientToken": str,
         "meshOwner": str,
         "tags": Sequence[TagRefTypeDef],
     },
     total=False,
 )
 
-
 class CreateVirtualServiceInputRequestTypeDef(
     _RequiredCreateVirtualServiceInputRequestTypeDef,
     _OptionalCreateVirtualServiceInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateVirtualServiceInputRequestTypeDef = TypedDict(
     "_RequiredUpdateVirtualServiceInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualServiceSpecTypeDef,
         "virtualServiceName": str,
     },
@@ -2612,33 +3822,74 @@
     {
         "clientToken": str,
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class UpdateVirtualServiceInputRequestTypeDef(
     _RequiredUpdateVirtualServiceInputRequestTypeDef,
     _OptionalUpdateVirtualServiceInputRequestTypeDef,
 ):
     pass
 
+GrpcGatewayRouteOutputTypeDef = TypedDict(
+    "GrpcGatewayRouteOutputTypeDef",
+    {
+        "action": GrpcGatewayRouteActionOutputTypeDef,
+        "match": GrpcGatewayRouteMatchOutputTypeDef,
+    },
+)
 
-VirtualServiceDataTypeDef = TypedDict(
-    "VirtualServiceDataTypeDef",
+_RequiredGrpcRouteOutputTypeDef = TypedDict(
+    "_RequiredGrpcRouteOutputTypeDef",
     {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "spec": VirtualServiceSpecTypeDef,
-        "status": VirtualServiceStatusTypeDef,
-        "virtualServiceName": str,
+        "action": GrpcRouteActionOutputTypeDef,
+        "match": GrpcRouteMatchOutputTypeDef,
+    },
+)
+_OptionalGrpcRouteOutputTypeDef = TypedDict(
+    "_OptionalGrpcRouteOutputTypeDef",
+    {
+        "retryPolicy": GrpcRetryPolicyOutputTypeDef,
+        "timeout": GrpcTimeoutOutputTypeDef,
+    },
+    total=False,
+)
+
+class GrpcRouteOutputTypeDef(_RequiredGrpcRouteOutputTypeDef, _OptionalGrpcRouteOutputTypeDef):
+    pass
+
+HttpGatewayRouteOutputTypeDef = TypedDict(
+    "HttpGatewayRouteOutputTypeDef",
+    {
+        "action": HttpGatewayRouteActionOutputTypeDef,
+        "match": HttpGatewayRouteMatchOutputTypeDef,
+    },
+)
+
+_RequiredHttpRouteOutputTypeDef = TypedDict(
+    "_RequiredHttpRouteOutputTypeDef",
+    {
+        "action": HttpRouteActionOutputTypeDef,
+        "match": HttpRouteMatchOutputTypeDef,
+    },
+)
+_OptionalHttpRouteOutputTypeDef = TypedDict(
+    "_OptionalHttpRouteOutputTypeDef",
+    {
+        "retryPolicy": HttpRetryPolicyOutputTypeDef,
+        "timeout": HttpTimeoutOutputTypeDef,
     },
+    total=False,
 )
 
+class HttpRouteOutputTypeDef(_RequiredHttpRouteOutputTypeDef, _OptionalHttpRouteOutputTypeDef):
+    pass
+
 GrpcGatewayRouteTypeDef = TypedDict(
     "GrpcGatewayRouteTypeDef",
     {
         "action": GrpcGatewayRouteActionTypeDef,
         "match": GrpcGatewayRouteMatchTypeDef,
     },
 )
@@ -2655,19 +3906,17 @@
     {
         "retryPolicy": GrpcRetryPolicyTypeDef,
         "timeout": GrpcTimeoutTypeDef,
     },
     total=False,
 )
 
-
 class GrpcRouteTypeDef(_RequiredGrpcRouteTypeDef, _OptionalGrpcRouteTypeDef):
     pass
 
-
 HttpGatewayRouteTypeDef = TypedDict(
     "HttpGatewayRouteTypeDef",
     {
         "action": HttpGatewayRouteActionTypeDef,
         "match": HttpGatewayRouteMatchTypeDef,
     },
 )
@@ -2684,18 +3933,32 @@
     {
         "retryPolicy": HttpRetryPolicyTypeDef,
         "timeout": HttpTimeoutTypeDef,
     },
     total=False,
 )
 
-
 class HttpRouteTypeDef(_RequiredHttpRouteTypeDef, _OptionalHttpRouteTypeDef):
     pass
 
+LoggingOutputTypeDef = TypedDict(
+    "LoggingOutputTypeDef",
+    {
+        "accessLog": AccessLogOutputTypeDef,
+    },
+    total=False,
+)
+
+VirtualGatewayLoggingOutputTypeDef = TypedDict(
+    "VirtualGatewayLoggingOutputTypeDef",
+    {
+        "accessLog": VirtualGatewayAccessLogOutputTypeDef,
+    },
+    total=False,
+)
 
 LoggingTypeDef = TypedDict(
     "LoggingTypeDef",
     {
         "accessLog": AccessLogTypeDef,
     },
     total=False,
@@ -2737,14 +4000,35 @@
     "UpdateVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredListenerOutputTypeDef = TypedDict(
+    "_RequiredListenerOutputTypeDef",
+    {
+        "portMapping": PortMappingOutputTypeDef,
+    },
+)
+_OptionalListenerOutputTypeDef = TypedDict(
+    "_OptionalListenerOutputTypeDef",
+    {
+        "connectionPool": VirtualNodeConnectionPoolOutputTypeDef,
+        "healthCheck": HealthCheckPolicyOutputTypeDef,
+        "outlierDetection": OutlierDetectionOutputTypeDef,
+        "timeout": ListenerTimeoutOutputTypeDef,
+        "tls": ListenerTlsOutputTypeDef,
+    },
+    total=False,
+)
+
+class ListenerOutputTypeDef(_RequiredListenerOutputTypeDef, _OptionalListenerOutputTypeDef):
+    pass
+
 _RequiredListenerTypeDef = TypedDict(
     "_RequiredListenerTypeDef",
     {
         "portMapping": PortMappingTypeDef,
     },
 )
 _OptionalListenerTypeDef = TypedDict(
@@ -2755,27 +4039,54 @@
         "outlierDetection": OutlierDetectionTypeDef,
         "timeout": ListenerTimeoutTypeDef,
         "tls": ListenerTlsTypeDef,
     },
     total=False,
 )
 
-
 class ListenerTypeDef(_RequiredListenerTypeDef, _OptionalListenerTypeDef):
     pass
 
+ClientPolicyOutputTypeDef = TypedDict(
+    "ClientPolicyOutputTypeDef",
+    {
+        "tls": ClientPolicyTlsOutputTypeDef,
+    },
+    total=False,
+)
 
 ClientPolicyTypeDef = TypedDict(
     "ClientPolicyTypeDef",
     {
         "tls": ClientPolicyTlsTypeDef,
     },
     total=False,
 )
 
+_RequiredVirtualGatewayListenerOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewayListenerOutputTypeDef",
+    {
+        "portMapping": VirtualGatewayPortMappingOutputTypeDef,
+    },
+)
+_OptionalVirtualGatewayListenerOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewayListenerOutputTypeDef",
+    {
+        "connectionPool": VirtualGatewayConnectionPoolOutputTypeDef,
+        "healthCheck": VirtualGatewayHealthCheckPolicyOutputTypeDef,
+        "tls": VirtualGatewayListenerTlsOutputTypeDef,
+    },
+    total=False,
+)
+
+class VirtualGatewayListenerOutputTypeDef(
+    _RequiredVirtualGatewayListenerOutputTypeDef, _OptionalVirtualGatewayListenerOutputTypeDef
+):
+    pass
+
 _RequiredVirtualGatewayListenerTypeDef = TypedDict(
     "_RequiredVirtualGatewayListenerTypeDef",
     {
         "portMapping": VirtualGatewayPortMappingTypeDef,
     },
 )
 _OptionalVirtualGatewayListenerTypeDef = TypedDict(
@@ -2784,20 +4095,26 @@
         "connectionPool": VirtualGatewayConnectionPoolTypeDef,
         "healthCheck": VirtualGatewayHealthCheckPolicyTypeDef,
         "tls": VirtualGatewayListenerTlsTypeDef,
     },
     total=False,
 )
 
-
 class VirtualGatewayListenerTypeDef(
     _RequiredVirtualGatewayListenerTypeDef, _OptionalVirtualGatewayListenerTypeDef
 ):
     pass
 
+VirtualGatewayClientPolicyOutputTypeDef = TypedDict(
+    "VirtualGatewayClientPolicyOutputTypeDef",
+    {
+        "tls": VirtualGatewayClientPolicyTlsOutputTypeDef,
+    },
+    total=False,
+)
 
 VirtualGatewayClientPolicyTypeDef = TypedDict(
     "VirtualGatewayClientPolicyTypeDef",
     {
         "tls": VirtualGatewayClientPolicyTlsTypeDef,
     },
     total=False,
@@ -2831,14 +4148,37 @@
     "UpdateVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+GatewayRouteSpecOutputTypeDef = TypedDict(
+    "GatewayRouteSpecOutputTypeDef",
+    {
+        "grpcRoute": GrpcGatewayRouteOutputTypeDef,
+        "http2Route": HttpGatewayRouteOutputTypeDef,
+        "httpRoute": HttpGatewayRouteOutputTypeDef,
+        "priority": int,
+    },
+    total=False,
+)
+
+RouteSpecOutputTypeDef = TypedDict(
+    "RouteSpecOutputTypeDef",
+    {
+        "grpcRoute": GrpcRouteOutputTypeDef,
+        "http2Route": HttpRouteOutputTypeDef,
+        "httpRoute": HttpRouteOutputTypeDef,
+        "priority": int,
+        "tcpRoute": TcpRouteOutputTypeDef,
+    },
+    total=False,
+)
+
 GatewayRouteSpecTypeDef = TypedDict(
     "GatewayRouteSpecTypeDef",
     {
         "grpcRoute": GrpcGatewayRouteTypeDef,
         "http2Route": HttpGatewayRouteTypeDef,
         "httpRoute": HttpGatewayRouteTypeDef,
         "priority": int,
@@ -2854,14 +4194,41 @@
         "httpRoute": HttpRouteTypeDef,
         "priority": int,
         "tcpRoute": TcpRouteTypeDef,
     },
     total=False,
 )
 
+BackendDefaultsOutputTypeDef = TypedDict(
+    "BackendDefaultsOutputTypeDef",
+    {
+        "clientPolicy": ClientPolicyOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredVirtualServiceBackendOutputTypeDef = TypedDict(
+    "_RequiredVirtualServiceBackendOutputTypeDef",
+    {
+        "virtualServiceName": str,
+    },
+)
+_OptionalVirtualServiceBackendOutputTypeDef = TypedDict(
+    "_OptionalVirtualServiceBackendOutputTypeDef",
+    {
+        "clientPolicy": ClientPolicyOutputTypeDef,
+    },
+    total=False,
+)
+
+class VirtualServiceBackendOutputTypeDef(
+    _RequiredVirtualServiceBackendOutputTypeDef, _OptionalVirtualServiceBackendOutputTypeDef
+):
+    pass
+
 BackendDefaultsTypeDef = TypedDict(
     "BackendDefaultsTypeDef",
     {
         "clientPolicy": ClientPolicyTypeDef,
     },
     total=False,
 )
@@ -2876,29 +4243,59 @@
     "_OptionalVirtualServiceBackendTypeDef",
     {
         "clientPolicy": ClientPolicyTypeDef,
     },
     total=False,
 )
 
-
 class VirtualServiceBackendTypeDef(
     _RequiredVirtualServiceBackendTypeDef, _OptionalVirtualServiceBackendTypeDef
 ):
     pass
 
+VirtualGatewayBackendDefaultsOutputTypeDef = TypedDict(
+    "VirtualGatewayBackendDefaultsOutputTypeDef",
+    {
+        "clientPolicy": VirtualGatewayClientPolicyOutputTypeDef,
+    },
+    total=False,
+)
 
 VirtualGatewayBackendDefaultsTypeDef = TypedDict(
     "VirtualGatewayBackendDefaultsTypeDef",
     {
         "clientPolicy": VirtualGatewayClientPolicyTypeDef,
     },
     total=False,
 )
 
+GatewayRouteDataTypeDef = TypedDict(
+    "GatewayRouteDataTypeDef",
+    {
+        "gatewayRouteName": str,
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "spec": GatewayRouteSpecOutputTypeDef,
+        "status": GatewayRouteStatusTypeDef,
+        "virtualGatewayName": str,
+    },
+)
+
+RouteDataTypeDef = TypedDict(
+    "RouteDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "routeName": str,
+        "spec": RouteSpecOutputTypeDef,
+        "status": RouteStatusTypeDef,
+        "virtualRouterName": str,
+    },
+)
+
 _RequiredCreateGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredCreateGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "spec": GatewayRouteSpecTypeDef,
         "virtualGatewayName": str,
@@ -2910,33 +4307,19 @@
         "clientToken": str,
         "meshOwner": str,
         "tags": Sequence[TagRefTypeDef],
     },
     total=False,
 )
 
-
 class CreateGatewayRouteInputRequestTypeDef(
     _RequiredCreateGatewayRouteInputRequestTypeDef, _OptionalCreateGatewayRouteInputRequestTypeDef
 ):
     pass
 
-
-GatewayRouteDataTypeDef = TypedDict(
-    "GatewayRouteDataTypeDef",
-    {
-        "gatewayRouteName": str,
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "spec": GatewayRouteSpecTypeDef,
-        "status": GatewayRouteStatusTypeDef,
-        "virtualGatewayName": str,
-    },
-)
-
 _RequiredUpdateGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "spec": GatewayRouteSpecTypeDef,
         "virtualGatewayName": str,
@@ -2947,21 +4330,19 @@
     {
         "clientToken": str,
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class UpdateGatewayRouteInputRequestTypeDef(
     _RequiredUpdateGatewayRouteInputRequestTypeDef, _OptionalUpdateGatewayRouteInputRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateRouteInputRequestTypeDef = TypedDict(
     "_RequiredCreateRouteInputRequestTypeDef",
     {
         "meshName": str,
         "routeName": str,
         "spec": RouteSpecTypeDef,
         "virtualRouterName": str,
@@ -2973,33 +4354,19 @@
         "clientToken": str,
         "meshOwner": str,
         "tags": Sequence[TagRefTypeDef],
     },
     total=False,
 )
 
-
 class CreateRouteInputRequestTypeDef(
     _RequiredCreateRouteInputRequestTypeDef, _OptionalCreateRouteInputRequestTypeDef
 ):
     pass
 
-
-RouteDataTypeDef = TypedDict(
-    "RouteDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "routeName": str,
-        "spec": RouteSpecTypeDef,
-        "status": RouteStatusTypeDef,
-        "virtualRouterName": str,
-    },
-)
-
 _RequiredUpdateRouteInputRequestTypeDef = TypedDict(
     "_RequiredUpdateRouteInputRequestTypeDef",
     {
         "meshName": str,
         "routeName": str,
         "spec": RouteSpecTypeDef,
         "virtualRouterName": str,
@@ -3010,29 +4377,55 @@
     {
         "clientToken": str,
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class UpdateRouteInputRequestTypeDef(
     _RequiredUpdateRouteInputRequestTypeDef, _OptionalUpdateRouteInputRequestTypeDef
 ):
     pass
 
+BackendOutputTypeDef = TypedDict(
+    "BackendOutputTypeDef",
+    {
+        "virtualService": VirtualServiceBackendOutputTypeDef,
+    },
+    total=False,
+)
 
 BackendTypeDef = TypedDict(
     "BackendTypeDef",
     {
         "virtualService": VirtualServiceBackendTypeDef,
     },
     total=False,
 )
 
+_RequiredVirtualGatewaySpecOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewaySpecOutputTypeDef",
+    {
+        "listeners": List[VirtualGatewayListenerOutputTypeDef],
+    },
+)
+_OptionalVirtualGatewaySpecOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewaySpecOutputTypeDef",
+    {
+        "backendDefaults": VirtualGatewayBackendDefaultsOutputTypeDef,
+        "logging": VirtualGatewayLoggingOutputTypeDef,
+    },
+    total=False,
+)
+
+class VirtualGatewaySpecOutputTypeDef(
+    _RequiredVirtualGatewaySpecOutputTypeDef, _OptionalVirtualGatewaySpecOutputTypeDef
+):
+    pass
+
 _RequiredVirtualGatewaySpecTypeDef = TypedDict(
     "_RequiredVirtualGatewaySpecTypeDef",
     {
         "listeners": Sequence[VirtualGatewayListenerTypeDef],
     },
 )
 _OptionalVirtualGatewaySpecTypeDef = TypedDict(
@@ -3040,21 +4433,19 @@
     {
         "backendDefaults": VirtualGatewayBackendDefaultsTypeDef,
         "logging": VirtualGatewayLoggingTypeDef,
     },
     total=False,
 )
 
-
 class VirtualGatewaySpecTypeDef(
     _RequiredVirtualGatewaySpecTypeDef, _OptionalVirtualGatewaySpecTypeDef
 ):
     pass
 
-
 CreateGatewayRouteOutputTypeDef = TypedDict(
     "CreateGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -3111,26 +4502,49 @@
     "UpdateRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+VirtualNodeSpecOutputTypeDef = TypedDict(
+    "VirtualNodeSpecOutputTypeDef",
+    {
+        "backendDefaults": BackendDefaultsOutputTypeDef,
+        "backends": List[BackendOutputTypeDef],
+        "listeners": List[ListenerOutputTypeDef],
+        "logging": LoggingOutputTypeDef,
+        "serviceDiscovery": ServiceDiscoveryOutputTypeDef,
+    },
+    total=False,
+)
+
 VirtualNodeSpecTypeDef = TypedDict(
     "VirtualNodeSpecTypeDef",
     {
         "backendDefaults": BackendDefaultsTypeDef,
         "backends": Sequence[BackendTypeDef],
         "listeners": Sequence[ListenerTypeDef],
         "logging": LoggingTypeDef,
         "serviceDiscovery": ServiceDiscoveryTypeDef,
     },
     total=False,
 )
 
+VirtualGatewayDataTypeDef = TypedDict(
+    "VirtualGatewayDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "spec": VirtualGatewaySpecOutputTypeDef,
+        "status": VirtualGatewayStatusTypeDef,
+        "virtualGatewayName": str,
+    },
+)
+
 _RequiredCreateVirtualGatewayInputRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualGatewayInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualGatewaySpecTypeDef,
         "virtualGatewayName": str,
     },
@@ -3141,22 +4555,20 @@
         "clientToken": str,
         "meshOwner": str,
         "tags": Sequence[TagRefTypeDef],
     },
     total=False,
 )
 
-
 class CreateVirtualGatewayInputRequestTypeDef(
     _RequiredCreateVirtualGatewayInputRequestTypeDef,
     _OptionalCreateVirtualGatewayInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateVirtualGatewayInputRequestTypeDef = TypedDict(
     "_RequiredUpdateVirtualGatewayInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualGatewaySpecTypeDef,
         "virtualGatewayName": str,
     },
@@ -3166,30 +4578,28 @@
     {
         "clientToken": str,
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class UpdateVirtualGatewayInputRequestTypeDef(
     _RequiredUpdateVirtualGatewayInputRequestTypeDef,
     _OptionalUpdateVirtualGatewayInputRequestTypeDef,
 ):
     pass
 
-
-VirtualGatewayDataTypeDef = TypedDict(
-    "VirtualGatewayDataTypeDef",
+VirtualNodeDataTypeDef = TypedDict(
+    "VirtualNodeDataTypeDef",
     {
         "meshName": str,
         "metadata": ResourceMetadataTypeDef,
-        "spec": VirtualGatewaySpecTypeDef,
-        "status": VirtualGatewayStatusTypeDef,
-        "virtualGatewayName": str,
+        "spec": VirtualNodeSpecOutputTypeDef,
+        "status": VirtualNodeStatusTypeDef,
+        "virtualNodeName": str,
     },
 )
 
 _RequiredCreateVirtualNodeInputRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualNodeInputRequestTypeDef",
     {
         "meshName": str,
@@ -3203,21 +4613,19 @@
         "clientToken": str,
         "meshOwner": str,
         "tags": Sequence[TagRefTypeDef],
     },
     total=False,
 )
 
-
 class CreateVirtualNodeInputRequestTypeDef(
     _RequiredCreateVirtualNodeInputRequestTypeDef, _OptionalCreateVirtualNodeInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateVirtualNodeInputRequestTypeDef = TypedDict(
     "_RequiredUpdateVirtualNodeInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualNodeSpecTypeDef,
         "virtualNodeName": str,
     },
@@ -3227,32 +4635,19 @@
     {
         "clientToken": str,
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class UpdateVirtualNodeInputRequestTypeDef(
     _RequiredUpdateVirtualNodeInputRequestTypeDef, _OptionalUpdateVirtualNodeInputRequestTypeDef
 ):
     pass
 
-
-VirtualNodeDataTypeDef = TypedDict(
-    "VirtualNodeDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "spec": VirtualNodeSpecTypeDef,
-        "status": VirtualNodeStatusTypeDef,
-        "virtualNodeName": str,
-    },
-)
-
 CreateVirtualGatewayOutputTypeDef = TypedDict(
     "CreateVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh.egg-info/PKG-INFO` & `mypy-boto3-appmesh-1.28.12/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-appmesh
-Version: 1.28.0
-Summary: Type annotations for boto3.AppMesh 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 appmesh type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-appmesh"></a>
 
 # mypy-boto3-appmesh
 
 [![PyPI - mypy-boto3-appmesh](https://img.shields.io/pypi/v/mypy-boto3-appmesh.svg?color=blue)](https://pypi.org/project/mypy-boto3-appmesh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appmesh.svg?color=blue)](https://pypi.org/project/mypy-boto3-appmesh)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appmesh?color=blue)](https://pypistats.org/packages/mypy-boto3-appmesh)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appmesh)](https://pepy.tech/project/mypy-boto3-appmesh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppMesh 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
+[boto3.AppMesh 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
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
 [mypy-boto3-appmesh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,15 +339,18 @@
 ### Typed dictionaries
 
 `mypy_boto3_appmesh.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appmesh.type_defs import (
+    AwsCloudMapInstanceAttributeOutputTypeDef,
     AwsCloudMapInstanceAttributeTypeDef,
+    ListenerTlsFileCertificateOutputTypeDef,
+    ListenerTlsSdsCertificateOutputTypeDef,
     ListenerTlsFileCertificateTypeDef,
     ListenerTlsSdsCertificateTypeDef,
     TagRefTypeDef,
     DeleteGatewayRouteInputRequestTypeDef,
     DeleteMeshInputRequestTypeDef,
     DeleteRouteInputRequestTypeDef,
     DeleteVirtualGatewayInputRequestTypeDef,
@@ -389,226 +360,343 @@
     DescribeGatewayRouteInputRequestTypeDef,
     DescribeMeshInputRequestTypeDef,
     DescribeRouteInputRequestTypeDef,
     DescribeVirtualGatewayInputRequestTypeDef,
     DescribeVirtualNodeInputRequestTypeDef,
     DescribeVirtualRouterInputRequestTypeDef,
     DescribeVirtualServiceInputRequestTypeDef,
+    DnsServiceDiscoveryOutputTypeDef,
     DnsServiceDiscoveryTypeDef,
+    DurationOutputTypeDef,
     DurationTypeDef,
+    EgressFilterOutputTypeDef,
     EgressFilterTypeDef,
     GatewayRouteStatusTypeDef,
     ResourceMetadataTypeDef,
+    GatewayRouteHostnameMatchOutputTypeDef,
     GatewayRouteHostnameMatchTypeDef,
+    GatewayRouteHostnameRewriteOutputTypeDef,
     GatewayRouteHostnameRewriteTypeDef,
     GatewayRouteRefTypeDef,
+    GatewayRouteVirtualServiceOutputTypeDef,
     GatewayRouteVirtualServiceTypeDef,
+    MatchRangeOutputTypeDef,
     MatchRangeTypeDef,
+    WeightedTargetOutputTypeDef,
     WeightedTargetTypeDef,
+    HealthCheckPolicyOutputTypeDef,
     HealthCheckPolicyTypeDef,
+    HttpPathMatchOutputTypeDef,
     HttpPathMatchTypeDef,
+    HttpGatewayRoutePathRewriteOutputTypeDef,
     HttpGatewayRoutePathRewriteTypeDef,
+    HttpGatewayRoutePrefixRewriteOutputTypeDef,
     HttpGatewayRoutePrefixRewriteTypeDef,
+    QueryParameterMatchOutputTypeDef,
     QueryParameterMatchTypeDef,
+    JsonFormatRefOutputTypeDef,
     JsonFormatRefTypeDef,
     ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
     ListGatewayRoutesInputRequestTypeDef,
     ListMeshesInputListMeshesPaginateTypeDef,
     ListMeshesInputRequestTypeDef,
     MeshRefTypeDef,
     ListRoutesInputListRoutesPaginateTypeDef,
     ListRoutesInputRequestTypeDef,
     RouteRefTypeDef,
     ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    TagRefOutputTypeDef,
     ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
     ListVirtualGatewaysInputRequestTypeDef,
     VirtualGatewayRefTypeDef,
     ListVirtualNodesInputListVirtualNodesPaginateTypeDef,
     ListVirtualNodesInputRequestTypeDef,
     VirtualNodeRefTypeDef,
     ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
     ListVirtualRoutersInputRequestTypeDef,
     VirtualRouterRefTypeDef,
     ListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     ListVirtualServicesInputRequestTypeDef,
     VirtualServiceRefTypeDef,
+    PortMappingOutputTypeDef,
+    ListenerTlsAcmCertificateOutputTypeDef,
     ListenerTlsAcmCertificateTypeDef,
+    TlsValidationContextFileTrustOutputTypeDef,
+    TlsValidationContextSdsTrustOutputTypeDef,
     TlsValidationContextFileTrustTypeDef,
     TlsValidationContextSdsTrustTypeDef,
     PortMappingTypeDef,
     MeshStatusTypeDef,
+    MeshServiceDiscoveryOutputTypeDef,
     MeshServiceDiscoveryTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     RouteStatusTypeDef,
+    SubjectAlternativeNameMatchersOutputTypeDef,
     SubjectAlternativeNameMatchersTypeDef,
+    TcpRouteMatchOutputTypeDef,
     TcpRouteMatchTypeDef,
+    TlsValidationContextAcmTrustOutputTypeDef,
     TlsValidationContextAcmTrustTypeDef,
     UntagResourceInputRequestTypeDef,
+    VirtualGatewayListenerTlsFileCertificateOutputTypeDef,
+    VirtualGatewayListenerTlsSdsCertificateOutputTypeDef,
     VirtualGatewayListenerTlsFileCertificateTypeDef,
     VirtualGatewayListenerTlsSdsCertificateTypeDef,
+    VirtualGatewayGrpcConnectionPoolOutputTypeDef,
+    VirtualGatewayHttp2ConnectionPoolOutputTypeDef,
+    VirtualGatewayHttpConnectionPoolOutputTypeDef,
     VirtualGatewayGrpcConnectionPoolTypeDef,
     VirtualGatewayHttp2ConnectionPoolTypeDef,
     VirtualGatewayHttpConnectionPoolTypeDef,
     VirtualGatewayStatusTypeDef,
+    VirtualGatewayHealthCheckPolicyOutputTypeDef,
     VirtualGatewayHealthCheckPolicyTypeDef,
+    VirtualGatewayPortMappingOutputTypeDef,
+    VirtualGatewayListenerTlsAcmCertificateOutputTypeDef,
     VirtualGatewayListenerTlsAcmCertificateTypeDef,
+    VirtualGatewayTlsValidationContextFileTrustOutputTypeDef,
+    VirtualGatewayTlsValidationContextSdsTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextFileTrustTypeDef,
     VirtualGatewayTlsValidationContextSdsTrustTypeDef,
     VirtualGatewayPortMappingTypeDef,
+    VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextAcmTrustTypeDef,
+    VirtualNodeGrpcConnectionPoolOutputTypeDef,
+    VirtualNodeHttp2ConnectionPoolOutputTypeDef,
+    VirtualNodeHttpConnectionPoolOutputTypeDef,
+    VirtualNodeTcpConnectionPoolOutputTypeDef,
     VirtualNodeGrpcConnectionPoolTypeDef,
     VirtualNodeHttp2ConnectionPoolTypeDef,
     VirtualNodeHttpConnectionPoolTypeDef,
     VirtualNodeTcpConnectionPoolTypeDef,
     VirtualNodeStatusTypeDef,
+    VirtualNodeServiceProviderOutputTypeDef,
     VirtualNodeServiceProviderTypeDef,
     VirtualRouterStatusTypeDef,
+    VirtualRouterServiceProviderOutputTypeDef,
     VirtualRouterServiceProviderTypeDef,
     VirtualServiceStatusTypeDef,
+    AwsCloudMapServiceDiscoveryOutputTypeDef,
     AwsCloudMapServiceDiscoveryTypeDef,
+    ClientTlsCertificateOutputTypeDef,
     ClientTlsCertificateTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    GrpcRetryPolicyOutputTypeDef,
+    GrpcTimeoutOutputTypeDef,
+    HttpRetryPolicyOutputTypeDef,
+    HttpTimeoutOutputTypeDef,
+    OutlierDetectionOutputTypeDef,
+    TcpTimeoutOutputTypeDef,
     GrpcRetryPolicyTypeDef,
     GrpcTimeoutTypeDef,
     HttpRetryPolicyTypeDef,
     HttpTimeoutTypeDef,
     OutlierDetectionTypeDef,
     TcpTimeoutTypeDef,
+    GrpcGatewayRouteRewriteOutputTypeDef,
     GrpcGatewayRouteRewriteTypeDef,
     ListGatewayRoutesOutputTypeDef,
+    GatewayRouteTargetOutputTypeDef,
     GatewayRouteTargetTypeDef,
+    GrpcMetadataMatchMethodOutputTypeDef,
+    GrpcRouteMetadataMatchMethodOutputTypeDef,
+    HeaderMatchMethodOutputTypeDef,
     GrpcMetadataMatchMethodTypeDef,
     GrpcRouteMetadataMatchMethodTypeDef,
     HeaderMatchMethodTypeDef,
+    GrpcRouteActionOutputTypeDef,
+    HttpRouteActionOutputTypeDef,
+    TcpRouteActionOutputTypeDef,
     GrpcRouteActionTypeDef,
     HttpRouteActionTypeDef,
     TcpRouteActionTypeDef,
+    HttpGatewayRouteRewriteOutputTypeDef,
     HttpGatewayRouteRewriteTypeDef,
+    HttpQueryParameterOutputTypeDef,
     HttpQueryParameterTypeDef,
+    LoggingFormatOutputTypeDef,
     LoggingFormatTypeDef,
     ListMeshesOutputTypeDef,
     ListRoutesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListVirtualGatewaysOutputTypeDef,
     ListVirtualNodesOutputTypeDef,
     ListVirtualRoutersOutputTypeDef,
     ListVirtualServicesOutputTypeDef,
+    VirtualRouterListenerOutputTypeDef,
+    ListenerTlsCertificateOutputTypeDef,
     ListenerTlsCertificateTypeDef,
+    ListenerTlsValidationContextTrustOutputTypeDef,
     ListenerTlsValidationContextTrustTypeDef,
     VirtualRouterListenerTypeDef,
+    MeshSpecOutputTypeDef,
     MeshSpecTypeDef,
+    SubjectAlternativeNamesOutputTypeDef,
     SubjectAlternativeNamesTypeDef,
+    TlsValidationContextTrustOutputTypeDef,
     TlsValidationContextTrustTypeDef,
+    VirtualGatewayClientTlsCertificateOutputTypeDef,
     VirtualGatewayClientTlsCertificateTypeDef,
+    VirtualGatewayConnectionPoolOutputTypeDef,
     VirtualGatewayConnectionPoolTypeDef,
+    VirtualGatewayListenerTlsCertificateOutputTypeDef,
     VirtualGatewayListenerTlsCertificateTypeDef,
+    VirtualGatewayListenerTlsValidationContextTrustOutputTypeDef,
     VirtualGatewayListenerTlsValidationContextTrustTypeDef,
+    VirtualGatewayTlsValidationContextTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextTrustTypeDef,
+    VirtualNodeConnectionPoolOutputTypeDef,
     VirtualNodeConnectionPoolTypeDef,
+    VirtualServiceProviderOutputTypeDef,
     VirtualServiceProviderTypeDef,
+    ServiceDiscoveryOutputTypeDef,
     ServiceDiscoveryTypeDef,
+    ListenerTimeoutOutputTypeDef,
     ListenerTimeoutTypeDef,
+    GrpcGatewayRouteActionOutputTypeDef,
     GrpcGatewayRouteActionTypeDef,
+    GrpcGatewayRouteMetadataOutputTypeDef,
+    GrpcRouteMetadataOutputTypeDef,
+    HttpGatewayRouteHeaderOutputTypeDef,
+    HttpRouteHeaderOutputTypeDef,
     GrpcGatewayRouteMetadataTypeDef,
     GrpcRouteMetadataTypeDef,
     HttpGatewayRouteHeaderTypeDef,
     HttpRouteHeaderTypeDef,
+    TcpRouteOutputTypeDef,
     TcpRouteTypeDef,
+    HttpGatewayRouteActionOutputTypeDef,
     HttpGatewayRouteActionTypeDef,
+    FileAccessLogOutputTypeDef,
+    VirtualGatewayFileAccessLogOutputTypeDef,
     FileAccessLogTypeDef,
     VirtualGatewayFileAccessLogTypeDef,
+    VirtualRouterSpecOutputTypeDef,
     VirtualRouterSpecTypeDef,
-    CreateMeshInputRequestTypeDef,
     MeshDataTypeDef,
+    CreateMeshInputRequestTypeDef,
     UpdateMeshInputRequestTypeDef,
+    ListenerTlsValidationContextOutputTypeDef,
     ListenerTlsValidationContextTypeDef,
+    TlsValidationContextOutputTypeDef,
     TlsValidationContextTypeDef,
+    VirtualGatewayListenerTlsValidationContextOutputTypeDef,
     VirtualGatewayListenerTlsValidationContextTypeDef,
+    VirtualGatewayTlsValidationContextOutputTypeDef,
     VirtualGatewayTlsValidationContextTypeDef,
+    VirtualServiceSpecOutputTypeDef,
     VirtualServiceSpecTypeDef,
+    GrpcGatewayRouteMatchOutputTypeDef,
+    GrpcRouteMatchOutputTypeDef,
+    HttpGatewayRouteMatchOutputTypeDef,
+    HttpRouteMatchOutputTypeDef,
     GrpcGatewayRouteMatchTypeDef,
     GrpcRouteMatchTypeDef,
     HttpGatewayRouteMatchTypeDef,
     HttpRouteMatchTypeDef,
+    AccessLogOutputTypeDef,
+    VirtualGatewayAccessLogOutputTypeDef,
     AccessLogTypeDef,
     VirtualGatewayAccessLogTypeDef,
+    VirtualRouterDataTypeDef,
     CreateVirtualRouterInputRequestTypeDef,
     UpdateVirtualRouterInputRequestTypeDef,
-    VirtualRouterDataTypeDef,
     CreateMeshOutputTypeDef,
     DeleteMeshOutputTypeDef,
     DescribeMeshOutputTypeDef,
     UpdateMeshOutputTypeDef,
+    ListenerTlsOutputTypeDef,
     ListenerTlsTypeDef,
+    ClientPolicyTlsOutputTypeDef,
     ClientPolicyTlsTypeDef,
+    VirtualGatewayListenerTlsOutputTypeDef,
     VirtualGatewayListenerTlsTypeDef,
+    VirtualGatewayClientPolicyTlsOutputTypeDef,
     VirtualGatewayClientPolicyTlsTypeDef,
+    VirtualServiceDataTypeDef,
     CreateVirtualServiceInputRequestTypeDef,
     UpdateVirtualServiceInputRequestTypeDef,
-    VirtualServiceDataTypeDef,
+    GrpcGatewayRouteOutputTypeDef,
+    GrpcRouteOutputTypeDef,
+    HttpGatewayRouteOutputTypeDef,
+    HttpRouteOutputTypeDef,
     GrpcGatewayRouteTypeDef,
     GrpcRouteTypeDef,
     HttpGatewayRouteTypeDef,
     HttpRouteTypeDef,
+    LoggingOutputTypeDef,
+    VirtualGatewayLoggingOutputTypeDef,
     LoggingTypeDef,
     VirtualGatewayLoggingTypeDef,
     CreateVirtualRouterOutputTypeDef,
     DeleteVirtualRouterOutputTypeDef,
     DescribeVirtualRouterOutputTypeDef,
     UpdateVirtualRouterOutputTypeDef,
+    ListenerOutputTypeDef,
     ListenerTypeDef,
+    ClientPolicyOutputTypeDef,
     ClientPolicyTypeDef,
+    VirtualGatewayListenerOutputTypeDef,
     VirtualGatewayListenerTypeDef,
+    VirtualGatewayClientPolicyOutputTypeDef,
     VirtualGatewayClientPolicyTypeDef,
     CreateVirtualServiceOutputTypeDef,
     DeleteVirtualServiceOutputTypeDef,
     DescribeVirtualServiceOutputTypeDef,
     UpdateVirtualServiceOutputTypeDef,
+    GatewayRouteSpecOutputTypeDef,
+    RouteSpecOutputTypeDef,
     GatewayRouteSpecTypeDef,
     RouteSpecTypeDef,
+    BackendDefaultsOutputTypeDef,
+    VirtualServiceBackendOutputTypeDef,
     BackendDefaultsTypeDef,
     VirtualServiceBackendTypeDef,
+    VirtualGatewayBackendDefaultsOutputTypeDef,
     VirtualGatewayBackendDefaultsTypeDef,
-    CreateGatewayRouteInputRequestTypeDef,
     GatewayRouteDataTypeDef,
+    RouteDataTypeDef,
+    CreateGatewayRouteInputRequestTypeDef,
     UpdateGatewayRouteInputRequestTypeDef,
     CreateRouteInputRequestTypeDef,
-    RouteDataTypeDef,
     UpdateRouteInputRequestTypeDef,
+    BackendOutputTypeDef,
     BackendTypeDef,
+    VirtualGatewaySpecOutputTypeDef,
     VirtualGatewaySpecTypeDef,
     CreateGatewayRouteOutputTypeDef,
     DeleteGatewayRouteOutputTypeDef,
     DescribeGatewayRouteOutputTypeDef,
     UpdateGatewayRouteOutputTypeDef,
     CreateRouteOutputTypeDef,
     DeleteRouteOutputTypeDef,
     DescribeRouteOutputTypeDef,
     UpdateRouteOutputTypeDef,
+    VirtualNodeSpecOutputTypeDef,
     VirtualNodeSpecTypeDef,
+    VirtualGatewayDataTypeDef,
     CreateVirtualGatewayInputRequestTypeDef,
     UpdateVirtualGatewayInputRequestTypeDef,
-    VirtualGatewayDataTypeDef,
+    VirtualNodeDataTypeDef,
     CreateVirtualNodeInputRequestTypeDef,
     UpdateVirtualNodeInputRequestTypeDef,
-    VirtualNodeDataTypeDef,
     CreateVirtualGatewayOutputTypeDef,
     DeleteVirtualGatewayOutputTypeDef,
     DescribeVirtualGatewayOutputTypeDef,
     UpdateVirtualGatewayOutputTypeDef,
     CreateVirtualNodeOutputTypeDef,
     DeleteVirtualNodeOutputTypeDef,
     DescribeVirtualNodeOutputTypeDef,
     UpdateVirtualNodeOutputTypeDef,
 )
 
 
-def get_structure() -> AwsCloudMapInstanceAttributeTypeDef:
+def get_structure() -> AwsCloudMapInstanceAttributeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appmesh-1.28.0/mypy_boto3_appmesh.egg-info/SOURCES.txt` & `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.0/setup.py` & `mypy-boto3-appmesh-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appmesh",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_appmesh"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppMesh 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.AppMesh 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

