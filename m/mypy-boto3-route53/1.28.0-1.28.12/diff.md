# Comparing `tmp/mypy-boto3-route53-1.28.0.tar.gz` & `tmp/mypy-boto3-route53-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53-1.28.0.tar", last modified: Thu Jul  6 21:00:28 2023, max compression
+gzip compressed data, was "mypy-boto3-route53-1.28.12.tar", last modified: Thu Jul 27 05:44:17 2023, max compression
```

## Comparing `mypy-boto3-route53-1.28.0.tar` & `mypy-boto3-route53-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:28.534412 mypy-boto3-route53-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:53:28.000000 mypy-boto3-route53-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22590 2023-07-06 21:00:28.526413 mypy-boto3-route53-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21105 2023-07-06 20:53:28.000000 mypy-boto3-route53-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:28.514412 mypy-boto3-route53-1.28.0/mypy_boto3_route53/
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-06 20:53:28.000000 mypy-boto3-route53-1.28.0/mypy_boto3_route53/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-06 20:53:28.000000 mypy-boto3-route53-1.28.0/mypy_boto3_route53/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 20:53:28.000000 mypy-boto3-route53-1.28.0/mypy_boto3_route53/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55440 2023-07-06 20:53:29.000000 mypy-boto3-route53-1.28.0/mypy_boto3_route53/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    55354 2023-07-06 20:53:28.000000 mypy-boto3-route53-1.28.0/mypy_boto3_route53/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-07-06 20:53:29.000000 mypy-boto3-route53-1.28.0/mypy_boto3_route53/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-07-06 20:53:29.000000 mypy-boto3-route53-1.28.0/mypy_boto3_route53/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-07-06 20:53:29.000000 mypy-boto3-route53-1.28.0/mypy_boto3_route53/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-07-06 20:53:29.000000 mypy-boto3-route53-1.28.0/mypy_boto3_route53/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:53:28.000000 mypy-boto3-route53-1.28.0/mypy_boto3_route53/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    61189 2023-07-06 20:53:34.000000 mypy-boto3-route53-1.28.0/mypy_boto3_route53/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    61122 2023-07-06 20:53:30.000000 mypy-boto3-route53-1.28.0/mypy_boto3_route53/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:53:28.000000 mypy-boto3-route53-1.28.0/mypy_boto3_route53/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-06 20:53:29.000000 mypy-boto3-route53-1.28.0/mypy_boto3_route53/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-06 20:53:29.000000 mypy-boto3-route53-1.28.0/mypy_boto3_route53/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:28.526413 mypy-boto3-route53-1.28.0/mypy_boto3_route53.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22590 2023-07-06 21:00:28.000000 mypy-boto3-route53-1.28.0/mypy_boto3_route53.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-06 21:00:28.000000 mypy-boto3-route53-1.28.0/mypy_boto3_route53.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:28.000000 mypy-boto3-route53-1.28.0/mypy_boto3_route53.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:28.000000 mypy-boto3-route53-1.28.0/mypy_boto3_route53.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:28.000000 mypy-boto3-route53-1.28.0/mypy_boto3_route53.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 21:00:28.000000 mypy-boto3-route53-1.28.0/mypy_boto3_route53.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:28.534412 mypy-boto3-route53-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-06 20:53:28.000000 mypy-boto3-route53-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:17.375381 mypy-boto3-route53-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-07-27 05:44:17.375381 mypy-boto3-route53-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21404 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:17.375381 mypy-boto3-route53-1.28.12/mypy_boto3_route53/
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55295 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55209 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    64627 2023-07-27 05:44:08.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64556 2023-07-27 05:44:07.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:17.375381 mypy-boto3-route53-1.28.12/mypy_boto3_route53.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-07-27 05:44:17.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-27 05:44:17.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:44:17.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:44:17.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:44:17.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:44:17.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:44:17.375381 mypy-boto3-route53-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/setup.py
```

### Comparing `mypy-boto3-route53-1.28.0/LICENSE` & `mypy-boto3-route53-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.0/PKG-INFO` & `mypy-boto3-route53-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53
-Version: 1.28.0
-Summary: Type annotations for boto3.Route53 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Route53 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-route53"></a>
 
 # mypy-boto3-route53
 
 [![PyPI - mypy-boto3-route53](https://img.shields.io/pypi/v/mypy-boto3-route53.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53?color=blue)](https://pypistats.org/packages/mypy-boto3-route53)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53)](https://pepy.tech/project/mypy-boto3-route53)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
+[boto3.Route53 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
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
 [mypy-boto3-route53 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/).
 
 See how it helps to find and fix potential bugs:
 
@@ -395,28 +395,32 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53.type_defs import (
     AccountLimitTypeDef,
     ActivateKeySigningKeyRequestRequestTypeDef,
     ChangeInfoTypeDef,
+    ResponseMetadataTypeDef,
+    AlarmIdentifierOutputTypeDef,
     AlarmIdentifierTypeDef,
+    AliasTargetOutputTypeDef,
     AliasTargetTypeDef,
     VPCTypeDef,
     CidrCollectionChangeTypeDef,
-    ChangeCidrCollectionResponseTypeDef,
     TagTypeDef,
     CidrBlockSummaryTypeDef,
     CidrCollectionTypeDef,
+    CidrRoutingConfigOutputTypeDef,
     CidrRoutingConfigTypeDef,
     DimensionTypeDef,
     CollectionSummaryTypeDef,
     CreateCidrCollectionRequestRequestTypeDef,
     HostedZoneConfigTypeDef,
     DelegationSetTypeDef,
+    VPCOutputTypeDef,
     CreateKeySigningKeyRequestRequestTypeDef,
     KeySigningKeyTypeDef,
     CreateQueryLoggingConfigRequestRequestTypeDef,
     QueryLoggingConfigTypeDef,
     CreateReusableDelegationSetRequestRequestTypeDef,
     CreateTrafficPolicyInstanceRequestRequestTypeDef,
     TrafficPolicyInstanceTypeDef,
@@ -432,106 +436,102 @@
     DeleteQueryLoggingConfigRequestRequestTypeDef,
     DeleteReusableDelegationSetRequestRequestTypeDef,
     DeleteTrafficPolicyInstanceRequestRequestTypeDef,
     DeleteTrafficPolicyRequestRequestTypeDef,
     DisableHostedZoneDNSSECRequestRequestTypeDef,
     EnableHostedZoneDNSSECRequestRequestTypeDef,
     GeoLocationDetailsTypeDef,
+    GeoLocationOutputTypeDef,
     GeoLocationTypeDef,
     GetAccountLimitRequestRequestTypeDef,
     GetChangeRequestRequestTypeDef,
     WaiterConfigTypeDef,
-    GetCheckerIpRangesResponseTypeDef,
     GetDNSSECRequestRequestTypeDef,
     GetGeoLocationRequestRequestTypeDef,
-    GetHealthCheckCountResponseTypeDef,
     GetHealthCheckLastFailureReasonRequestRequestTypeDef,
     GetHealthCheckRequestRequestTypeDef,
     GetHealthCheckStatusRequestRequestTypeDef,
-    GetHostedZoneCountResponseTypeDef,
     GetHostedZoneLimitRequestRequestTypeDef,
     HostedZoneLimitTypeDef,
     GetHostedZoneRequestRequestTypeDef,
     GetQueryLoggingConfigRequestRequestTypeDef,
     GetReusableDelegationSetLimitRequestRequestTypeDef,
     ReusableDelegationSetLimitTypeDef,
     GetReusableDelegationSetRequestRequestTypeDef,
-    GetTrafficPolicyInstanceCountResponseTypeDef,
     GetTrafficPolicyInstanceRequestRequestTypeDef,
     GetTrafficPolicyRequestRequestTypeDef,
     StatusReportTypeDef,
     LinkedServiceTypeDef,
+    HostedZoneConfigOutputTypeDef,
     HostedZoneOwnerTypeDef,
-    ListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListCidrBlocksRequestRequestTypeDef,
-    ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef,
     ListCidrCollectionsRequestRequestTypeDef,
-    ListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
     ListCidrLocationsRequestRequestTypeDef,
     LocationSummaryTypeDef,
     ListGeoLocationsRequestRequestTypeDef,
-    ListHealthChecksRequestListHealthChecksPaginateTypeDef,
     ListHealthChecksRequestRequestTypeDef,
     ListHostedZonesByNameRequestRequestTypeDef,
     ListHostedZonesByVPCRequestRequestTypeDef,
-    ListHostedZonesRequestListHostedZonesPaginateTypeDef,
     ListHostedZonesRequestRequestTypeDef,
-    ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef,
     ListQueryLoggingConfigsRequestRequestTypeDef,
-    ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
     ListResourceRecordSetsRequestRequestTypeDef,
     ListReusableDelegationSetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourcesRequestRequestTypeDef,
     ListTrafficPoliciesRequestRequestTypeDef,
     TrafficPolicySummaryTypeDef,
     ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef,
     ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef,
     ListTrafficPolicyInstancesRequestRequestTypeDef,
     ListTrafficPolicyVersionsRequestRequestTypeDef,
-    ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
     ListVPCAssociationAuthorizationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ResourceRecordOutputTypeDef,
     ResourceRecordTypeDef,
-    ResponseMetadataTypeDef,
+    TagOutputTypeDef,
     TestDNSAnswerRequestRequestTypeDef,
-    TestDNSAnswerResponseTypeDef,
     UpdateHostedZoneCommentRequestRequestTypeDef,
     UpdateTrafficPolicyCommentRequestRequestTypeDef,
     UpdateTrafficPolicyInstanceRequestRequestTypeDef,
-    GetAccountLimitResponseTypeDef,
     ActivateKeySigningKeyResponseTypeDef,
     AssociateVPCWithHostedZoneResponseTypeDef,
+    ChangeCidrCollectionResponseTypeDef,
     ChangeResourceRecordSetsResponseTypeDef,
     DeactivateKeySigningKeyResponseTypeDef,
     DeleteHostedZoneResponseTypeDef,
     DeleteKeySigningKeyResponseTypeDef,
     DisableHostedZoneDNSSECResponseTypeDef,
     DisassociateVPCFromHostedZoneResponseTypeDef,
     EnableHostedZoneDNSSECResponseTypeDef,
+    GetAccountLimitResponseTypeDef,
     GetChangeResponseTypeDef,
+    GetCheckerIpRangesResponseTypeDef,
+    GetHealthCheckCountResponseTypeDef,
+    GetHostedZoneCountResponseTypeDef,
+    GetTrafficPolicyInstanceCountResponseTypeDef,
+    TestDNSAnswerResponseTypeDef,
+    HealthCheckConfigOutputTypeDef,
     HealthCheckConfigTypeDef,
     UpdateHealthCheckRequestRequestTypeDef,
     AssociateVPCWithHostedZoneRequestRequestTypeDef,
     CreateVPCAssociationAuthorizationRequestRequestTypeDef,
-    CreateVPCAssociationAuthorizationResponseTypeDef,
     DeleteVPCAssociationAuthorizationRequestRequestTypeDef,
     DisassociateVPCFromHostedZoneRequestRequestTypeDef,
-    ListVPCAssociationAuthorizationsResponseTypeDef,
     ChangeCidrCollectionRequestRequestTypeDef,
     ChangeTagsForResourceRequestRequestTypeDef,
-    ResourceTagSetTypeDef,
     ListCidrBlocksResponseTypeDef,
     CreateCidrCollectionResponseTypeDef,
     CloudWatchAlarmConfigurationTypeDef,
     ListCidrCollectionsResponseTypeDef,
     CreateHostedZoneRequestRequestTypeDef,
     CreateReusableDelegationSetResponseTypeDef,
     GetReusableDelegationSetResponseTypeDef,
     ListReusableDelegationSetsResponseTypeDef,
+    CreateVPCAssociationAuthorizationResponseTypeDef,
+    ListVPCAssociationAuthorizationsResponseTypeDef,
     CreateKeySigningKeyResponseTypeDef,
     CreateQueryLoggingConfigResponseTypeDef,
     GetQueryLoggingConfigResponseTypeDef,
     ListQueryLoggingConfigsResponseTypeDef,
     CreateTrafficPolicyInstanceResponseTypeDef,
     GetTrafficPolicyInstanceResponseTypeDef,
     ListTrafficPolicyInstancesByHostedZoneResponseTypeDef,
@@ -548,31 +548,41 @@
     ListGeoLocationsResponseTypeDef,
     GetChangeRequestResourceRecordSetsChangedWaitTypeDef,
     GetHostedZoneLimitResponseTypeDef,
     GetReusableDelegationSetLimitResponseTypeDef,
     HealthCheckObservationTypeDef,
     HostedZoneTypeDef,
     HostedZoneSummaryTypeDef,
+    ListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+    ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef,
+    ListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
+    ListHealthChecksRequestListHealthChecksPaginateTypeDef,
+    ListHostedZonesRequestListHostedZonesPaginateTypeDef,
+    ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef,
+    ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
+    ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
     ListCidrLocationsResponseTypeDef,
     ListTrafficPoliciesResponseTypeDef,
+    ResourceRecordSetOutputTypeDef,
     ResourceRecordSetTypeDef,
+    ResourceTagSetTypeDef,
     CreateHealthCheckRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTagsForResourcesResponseTypeDef,
     HealthCheckTypeDef,
     GetHealthCheckLastFailureReasonResponseTypeDef,
     GetHealthCheckStatusResponseTypeDef,
     CreateHostedZoneResponseTypeDef,
     GetHostedZoneResponseTypeDef,
     ListHostedZonesByNameResponseTypeDef,
     ListHostedZonesResponseTypeDef,
     UpdateHostedZoneCommentResponseTypeDef,
     ListHostedZonesByVPCResponseTypeDef,
-    ChangeTypeDef,
     ListResourceRecordSetsResponseTypeDef,
+    ChangeTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTagsForResourcesResponseTypeDef,
     CreateHealthCheckResponseTypeDef,
     GetHealthCheckResponseTypeDef,
     ListHealthChecksResponseTypeDef,
     UpdateHealthCheckResponseTypeDef,
     ChangeBatchTypeDef,
     ChangeResourceRecordSetsRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-route53-1.28.0/README.md` & `mypy-boto3-route53-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-route53"></a>
 
 # mypy-boto3-route53
 
 [![PyPI - mypy-boto3-route53](https://img.shields.io/pypi/v/mypy-boto3-route53.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53?color=blue)](https://pypistats.org/packages/mypy-boto3-route53)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53)](https://pepy.tech/project/mypy-boto3-route53)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
+[boto3.Route53 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
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
 [mypy-boto3-route53 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/).
 
 See how it helps to find and fix potential bugs:
 
@@ -363,28 +363,32 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53.type_defs import (
     AccountLimitTypeDef,
     ActivateKeySigningKeyRequestRequestTypeDef,
     ChangeInfoTypeDef,
+    ResponseMetadataTypeDef,
+    AlarmIdentifierOutputTypeDef,
     AlarmIdentifierTypeDef,
+    AliasTargetOutputTypeDef,
     AliasTargetTypeDef,
     VPCTypeDef,
     CidrCollectionChangeTypeDef,
-    ChangeCidrCollectionResponseTypeDef,
     TagTypeDef,
     CidrBlockSummaryTypeDef,
     CidrCollectionTypeDef,
+    CidrRoutingConfigOutputTypeDef,
     CidrRoutingConfigTypeDef,
     DimensionTypeDef,
     CollectionSummaryTypeDef,
     CreateCidrCollectionRequestRequestTypeDef,
     HostedZoneConfigTypeDef,
     DelegationSetTypeDef,
+    VPCOutputTypeDef,
     CreateKeySigningKeyRequestRequestTypeDef,
     KeySigningKeyTypeDef,
     CreateQueryLoggingConfigRequestRequestTypeDef,
     QueryLoggingConfigTypeDef,
     CreateReusableDelegationSetRequestRequestTypeDef,
     CreateTrafficPolicyInstanceRequestRequestTypeDef,
     TrafficPolicyInstanceTypeDef,
@@ -400,106 +404,102 @@
     DeleteQueryLoggingConfigRequestRequestTypeDef,
     DeleteReusableDelegationSetRequestRequestTypeDef,
     DeleteTrafficPolicyInstanceRequestRequestTypeDef,
     DeleteTrafficPolicyRequestRequestTypeDef,
     DisableHostedZoneDNSSECRequestRequestTypeDef,
     EnableHostedZoneDNSSECRequestRequestTypeDef,
     GeoLocationDetailsTypeDef,
+    GeoLocationOutputTypeDef,
     GeoLocationTypeDef,
     GetAccountLimitRequestRequestTypeDef,
     GetChangeRequestRequestTypeDef,
     WaiterConfigTypeDef,
-    GetCheckerIpRangesResponseTypeDef,
     GetDNSSECRequestRequestTypeDef,
     GetGeoLocationRequestRequestTypeDef,
-    GetHealthCheckCountResponseTypeDef,
     GetHealthCheckLastFailureReasonRequestRequestTypeDef,
     GetHealthCheckRequestRequestTypeDef,
     GetHealthCheckStatusRequestRequestTypeDef,
-    GetHostedZoneCountResponseTypeDef,
     GetHostedZoneLimitRequestRequestTypeDef,
     HostedZoneLimitTypeDef,
     GetHostedZoneRequestRequestTypeDef,
     GetQueryLoggingConfigRequestRequestTypeDef,
     GetReusableDelegationSetLimitRequestRequestTypeDef,
     ReusableDelegationSetLimitTypeDef,
     GetReusableDelegationSetRequestRequestTypeDef,
-    GetTrafficPolicyInstanceCountResponseTypeDef,
     GetTrafficPolicyInstanceRequestRequestTypeDef,
     GetTrafficPolicyRequestRequestTypeDef,
     StatusReportTypeDef,
     LinkedServiceTypeDef,
+    HostedZoneConfigOutputTypeDef,
     HostedZoneOwnerTypeDef,
-    ListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListCidrBlocksRequestRequestTypeDef,
-    ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef,
     ListCidrCollectionsRequestRequestTypeDef,
-    ListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
     ListCidrLocationsRequestRequestTypeDef,
     LocationSummaryTypeDef,
     ListGeoLocationsRequestRequestTypeDef,
-    ListHealthChecksRequestListHealthChecksPaginateTypeDef,
     ListHealthChecksRequestRequestTypeDef,
     ListHostedZonesByNameRequestRequestTypeDef,
     ListHostedZonesByVPCRequestRequestTypeDef,
-    ListHostedZonesRequestListHostedZonesPaginateTypeDef,
     ListHostedZonesRequestRequestTypeDef,
-    ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef,
     ListQueryLoggingConfigsRequestRequestTypeDef,
-    ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
     ListResourceRecordSetsRequestRequestTypeDef,
     ListReusableDelegationSetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourcesRequestRequestTypeDef,
     ListTrafficPoliciesRequestRequestTypeDef,
     TrafficPolicySummaryTypeDef,
     ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef,
     ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef,
     ListTrafficPolicyInstancesRequestRequestTypeDef,
     ListTrafficPolicyVersionsRequestRequestTypeDef,
-    ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
     ListVPCAssociationAuthorizationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ResourceRecordOutputTypeDef,
     ResourceRecordTypeDef,
-    ResponseMetadataTypeDef,
+    TagOutputTypeDef,
     TestDNSAnswerRequestRequestTypeDef,
-    TestDNSAnswerResponseTypeDef,
     UpdateHostedZoneCommentRequestRequestTypeDef,
     UpdateTrafficPolicyCommentRequestRequestTypeDef,
     UpdateTrafficPolicyInstanceRequestRequestTypeDef,
-    GetAccountLimitResponseTypeDef,
     ActivateKeySigningKeyResponseTypeDef,
     AssociateVPCWithHostedZoneResponseTypeDef,
+    ChangeCidrCollectionResponseTypeDef,
     ChangeResourceRecordSetsResponseTypeDef,
     DeactivateKeySigningKeyResponseTypeDef,
     DeleteHostedZoneResponseTypeDef,
     DeleteKeySigningKeyResponseTypeDef,
     DisableHostedZoneDNSSECResponseTypeDef,
     DisassociateVPCFromHostedZoneResponseTypeDef,
     EnableHostedZoneDNSSECResponseTypeDef,
+    GetAccountLimitResponseTypeDef,
     GetChangeResponseTypeDef,
+    GetCheckerIpRangesResponseTypeDef,
+    GetHealthCheckCountResponseTypeDef,
+    GetHostedZoneCountResponseTypeDef,
+    GetTrafficPolicyInstanceCountResponseTypeDef,
+    TestDNSAnswerResponseTypeDef,
+    HealthCheckConfigOutputTypeDef,
     HealthCheckConfigTypeDef,
     UpdateHealthCheckRequestRequestTypeDef,
     AssociateVPCWithHostedZoneRequestRequestTypeDef,
     CreateVPCAssociationAuthorizationRequestRequestTypeDef,
-    CreateVPCAssociationAuthorizationResponseTypeDef,
     DeleteVPCAssociationAuthorizationRequestRequestTypeDef,
     DisassociateVPCFromHostedZoneRequestRequestTypeDef,
-    ListVPCAssociationAuthorizationsResponseTypeDef,
     ChangeCidrCollectionRequestRequestTypeDef,
     ChangeTagsForResourceRequestRequestTypeDef,
-    ResourceTagSetTypeDef,
     ListCidrBlocksResponseTypeDef,
     CreateCidrCollectionResponseTypeDef,
     CloudWatchAlarmConfigurationTypeDef,
     ListCidrCollectionsResponseTypeDef,
     CreateHostedZoneRequestRequestTypeDef,
     CreateReusableDelegationSetResponseTypeDef,
     GetReusableDelegationSetResponseTypeDef,
     ListReusableDelegationSetsResponseTypeDef,
+    CreateVPCAssociationAuthorizationResponseTypeDef,
+    ListVPCAssociationAuthorizationsResponseTypeDef,
     CreateKeySigningKeyResponseTypeDef,
     CreateQueryLoggingConfigResponseTypeDef,
     GetQueryLoggingConfigResponseTypeDef,
     ListQueryLoggingConfigsResponseTypeDef,
     CreateTrafficPolicyInstanceResponseTypeDef,
     GetTrafficPolicyInstanceResponseTypeDef,
     ListTrafficPolicyInstancesByHostedZoneResponseTypeDef,
@@ -516,31 +516,41 @@
     ListGeoLocationsResponseTypeDef,
     GetChangeRequestResourceRecordSetsChangedWaitTypeDef,
     GetHostedZoneLimitResponseTypeDef,
     GetReusableDelegationSetLimitResponseTypeDef,
     HealthCheckObservationTypeDef,
     HostedZoneTypeDef,
     HostedZoneSummaryTypeDef,
+    ListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+    ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef,
+    ListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
+    ListHealthChecksRequestListHealthChecksPaginateTypeDef,
+    ListHostedZonesRequestListHostedZonesPaginateTypeDef,
+    ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef,
+    ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
+    ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
     ListCidrLocationsResponseTypeDef,
     ListTrafficPoliciesResponseTypeDef,
+    ResourceRecordSetOutputTypeDef,
     ResourceRecordSetTypeDef,
+    ResourceTagSetTypeDef,
     CreateHealthCheckRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTagsForResourcesResponseTypeDef,
     HealthCheckTypeDef,
     GetHealthCheckLastFailureReasonResponseTypeDef,
     GetHealthCheckStatusResponseTypeDef,
     CreateHostedZoneResponseTypeDef,
     GetHostedZoneResponseTypeDef,
     ListHostedZonesByNameResponseTypeDef,
     ListHostedZonesResponseTypeDef,
     UpdateHostedZoneCommentResponseTypeDef,
     ListHostedZonesByVPCResponseTypeDef,
-    ChangeTypeDef,
     ListResourceRecordSetsResponseTypeDef,
+    ChangeTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTagsForResourcesResponseTypeDef,
     CreateHealthCheckResponseTypeDef,
     GetHealthCheckResponseTypeDef,
     ListHealthChecksResponseTypeDef,
     UpdateHealthCheckResponseTypeDef,
     ChangeBatchTypeDef,
     ChangeResourceRecordSetsRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-route53-1.28.0/mypy_boto3_route53/__init__.py` & `mypy-boto3-route53-1.28.12/mypy_boto3_route53/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.0/mypy_boto3_route53/__init__.pyi` & `mypy-boto3-route53-1.28.12/mypy_boto3_route53/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.0/mypy_boto3_route53/__main__.py` & `mypy-boto3-route53-1.28.12/mypy_boto3_route53/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Route53 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53\nOther"
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

### Comparing `mypy-boto3-route53-1.28.0/mypy_boto3_route53/client.py` & `mypy-boto3-route53-1.28.12/mypy_boto3_route53/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1020,16 +1020,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/client/#update_traffic_policy_comment)
         """
 
     def update_traffic_policy_instance(
         self, *, Id: str, TTL: int, TrafficPolicyId: str, TrafficPolicyVersion: int
     ) -> UpdateTrafficPolicyInstanceResponseTypeDef:
         """
-        Updates the resource record sets in a specified hosted zone that were created
-        based on the settings in a specified traffic policy version.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.update_traffic_policy_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/client/#update_traffic_policy_instance)
         """
 
     @overload
     def get_paginator(self, operation_name: Literal["list_cidr_blocks"]) -> ListCidrBlocksPaginator:
```

### Comparing `mypy-boto3-route53-1.28.0/mypy_boto3_route53/client.pyi` & `mypy-boto3-route53-1.28.12/mypy_boto3_route53/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -943,16 +943,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.update_traffic_policy_comment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/client/#update_traffic_policy_comment)
         """
     def update_traffic_policy_instance(
         self, *, Id: str, TTL: int, TrafficPolicyId: str, TrafficPolicyVersion: int
     ) -> UpdateTrafficPolicyInstanceResponseTypeDef:
         """
-        Updates the resource record sets in a specified hosted zone that were created
-        based on the settings in a specified traffic policy version.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.update_traffic_policy_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/client/#update_traffic_policy_instance)
         """
     @overload
     def get_paginator(self, operation_name: Literal["list_cidr_blocks"]) -> ListCidrBlocksPaginator:
         """
```

### Comparing `mypy-boto3-route53-1.28.0/mypy_boto3_route53/literals.py` & `mypy-boto3-route53-1.28.12/mypy_boto3_route53/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,14 +330,15 @@
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
@@ -416,26 +417,28 @@
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

### Comparing `mypy-boto3-route53-1.28.0/mypy_boto3_route53/literals.pyi` & `mypy-boto3-route53-1.28.12/mypy_boto3_route53/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -328,14 +328,15 @@
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
@@ -414,26 +415,28 @@
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

### Comparing `mypy-boto3-route53-1.28.0/mypy_boto3_route53/paginator.py` & `mypy-boto3-route53-1.28.12/mypy_boto3_route53/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,105 +78,105 @@
     """
 
     def paginate(
         self,
         *,
         CollectionId: str,
         LocationName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCidrBlocksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrBlocks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listcidrblockspaginator)
         """
 
 
 class ListCidrCollectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrCollections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listcidrcollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCidrCollectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrCollections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listcidrcollectionspaginator)
         """
 
 
 class ListCidrLocationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrLocations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listcidrlocationspaginator)
     """
 
     def paginate(
-        self, *, CollectionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CollectionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCidrLocationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrLocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listcidrlocationspaginator)
         """
 
 
 class ListHealthChecksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHealthChecks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listhealthcheckspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHealthChecksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHealthChecks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listhealthcheckspaginator)
         """
 
 
 class ListHostedZonesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHostedZones)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listhostedzonespaginator)
     """
 
     def paginate(
-        self, *, DelegationSetId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DelegationSetId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHostedZonesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHostedZones.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listhostedzonespaginator)
         """
 
 
 class ListQueryLoggingConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListQueryLoggingConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listqueryloggingconfigspaginator)
     """
 
     def paginate(
-        self, *, HostedZoneId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, HostedZoneId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListQueryLoggingConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListQueryLoggingConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listqueryloggingconfigspaginator)
         """
 
 
 class ListResourceRecordSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListResourceRecordSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listresourcerecordsetspaginator)
     """
 
     def paginate(
-        self, *, HostedZoneId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, HostedZoneId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceRecordSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListResourceRecordSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listresourcerecordsetspaginator)
         """
 
 
@@ -187,13 +187,13 @@
     """
 
     def paginate(
         self,
         *,
         HostedZoneId: str,
         MaxResults: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVPCAssociationAuthorizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListVPCAssociationAuthorizations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listvpcassociationauthorizationspaginator)
         """
```

### Comparing `mypy-boto3-route53-1.28.0/mypy_boto3_route53/paginator.pyi` & `mypy-boto3-route53-1.28.12/mypy_boto3_route53/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -75,99 +75,99 @@
     """
 
     def paginate(
         self,
         *,
         CollectionId: str,
         LocationName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCidrBlocksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrBlocks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listcidrblockspaginator)
         """
 
 class ListCidrCollectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrCollections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listcidrcollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCidrCollectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrCollections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listcidrcollectionspaginator)
         """
 
 class ListCidrLocationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrLocations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listcidrlocationspaginator)
     """
 
     def paginate(
-        self, *, CollectionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CollectionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCidrLocationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrLocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listcidrlocationspaginator)
         """
 
 class ListHealthChecksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHealthChecks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listhealthcheckspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHealthChecksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHealthChecks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listhealthcheckspaginator)
         """
 
 class ListHostedZonesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHostedZones)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listhostedzonespaginator)
     """
 
     def paginate(
-        self, *, DelegationSetId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DelegationSetId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHostedZonesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHostedZones.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listhostedzonespaginator)
         """
 
 class ListQueryLoggingConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListQueryLoggingConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listqueryloggingconfigspaginator)
     """
 
     def paginate(
-        self, *, HostedZoneId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, HostedZoneId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListQueryLoggingConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListQueryLoggingConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listqueryloggingconfigspaginator)
         """
 
 class ListResourceRecordSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListResourceRecordSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listresourcerecordsetspaginator)
     """
 
     def paginate(
-        self, *, HostedZoneId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, HostedZoneId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceRecordSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListResourceRecordSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listresourcerecordsetspaginator)
         """
 
 class ListVPCAssociationAuthorizationsPaginator(Paginator):
@@ -177,13 +177,13 @@
     """
 
     def paginate(
         self,
         *,
         HostedZoneId: str,
         MaxResults: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVPCAssociationAuthorizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListVPCAssociationAuthorizations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/paginators/#listvpcassociationauthorizationspaginator)
         """
```

### Comparing `mypy-boto3-route53-1.28.0/mypy_boto3_route53/type_defs.py` & `mypy-boto3-route53-1.28.12/mypy_boto3_route53/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,28 +45,32 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountLimitTypeDef",
     "ActivateKeySigningKeyRequestRequestTypeDef",
     "ChangeInfoTypeDef",
+    "ResponseMetadataTypeDef",
+    "AlarmIdentifierOutputTypeDef",
     "AlarmIdentifierTypeDef",
+    "AliasTargetOutputTypeDef",
     "AliasTargetTypeDef",
     "VPCTypeDef",
     "CidrCollectionChangeTypeDef",
-    "ChangeCidrCollectionResponseTypeDef",
     "TagTypeDef",
     "CidrBlockSummaryTypeDef",
     "CidrCollectionTypeDef",
+    "CidrRoutingConfigOutputTypeDef",
     "CidrRoutingConfigTypeDef",
     "DimensionTypeDef",
     "CollectionSummaryTypeDef",
     "CreateCidrCollectionRequestRequestTypeDef",
     "HostedZoneConfigTypeDef",
     "DelegationSetTypeDef",
+    "VPCOutputTypeDef",
     "CreateKeySigningKeyRequestRequestTypeDef",
     "KeySigningKeyTypeDef",
     "CreateQueryLoggingConfigRequestRequestTypeDef",
     "QueryLoggingConfigTypeDef",
     "CreateReusableDelegationSetRequestRequestTypeDef",
     "CreateTrafficPolicyInstanceRequestRequestTypeDef",
     "TrafficPolicyInstanceTypeDef",
@@ -82,106 +86,102 @@
     "DeleteQueryLoggingConfigRequestRequestTypeDef",
     "DeleteReusableDelegationSetRequestRequestTypeDef",
     "DeleteTrafficPolicyInstanceRequestRequestTypeDef",
     "DeleteTrafficPolicyRequestRequestTypeDef",
     "DisableHostedZoneDNSSECRequestRequestTypeDef",
     "EnableHostedZoneDNSSECRequestRequestTypeDef",
     "GeoLocationDetailsTypeDef",
+    "GeoLocationOutputTypeDef",
     "GeoLocationTypeDef",
     "GetAccountLimitRequestRequestTypeDef",
     "GetChangeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
-    "GetCheckerIpRangesResponseTypeDef",
     "GetDNSSECRequestRequestTypeDef",
     "GetGeoLocationRequestRequestTypeDef",
-    "GetHealthCheckCountResponseTypeDef",
     "GetHealthCheckLastFailureReasonRequestRequestTypeDef",
     "GetHealthCheckRequestRequestTypeDef",
     "GetHealthCheckStatusRequestRequestTypeDef",
-    "GetHostedZoneCountResponseTypeDef",
     "GetHostedZoneLimitRequestRequestTypeDef",
     "HostedZoneLimitTypeDef",
     "GetHostedZoneRequestRequestTypeDef",
     "GetQueryLoggingConfigRequestRequestTypeDef",
     "GetReusableDelegationSetLimitRequestRequestTypeDef",
     "ReusableDelegationSetLimitTypeDef",
     "GetReusableDelegationSetRequestRequestTypeDef",
-    "GetTrafficPolicyInstanceCountResponseTypeDef",
     "GetTrafficPolicyInstanceRequestRequestTypeDef",
     "GetTrafficPolicyRequestRequestTypeDef",
     "StatusReportTypeDef",
     "LinkedServiceTypeDef",
+    "HostedZoneConfigOutputTypeDef",
     "HostedZoneOwnerTypeDef",
-    "ListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListCidrBlocksRequestRequestTypeDef",
-    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
     "ListCidrCollectionsRequestRequestTypeDef",
-    "ListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
     "ListCidrLocationsRequestRequestTypeDef",
     "LocationSummaryTypeDef",
     "ListGeoLocationsRequestRequestTypeDef",
-    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
     "ListHealthChecksRequestRequestTypeDef",
     "ListHostedZonesByNameRequestRequestTypeDef",
     "ListHostedZonesByVPCRequestRequestTypeDef",
-    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
     "ListHostedZonesRequestRequestTypeDef",
-    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
     "ListQueryLoggingConfigsRequestRequestTypeDef",
-    "ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
     "ListResourceRecordSetsRequestRequestTypeDef",
     "ListReusableDelegationSetsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourcesRequestRequestTypeDef",
     "ListTrafficPoliciesRequestRequestTypeDef",
     "TrafficPolicySummaryTypeDef",
     "ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef",
     "ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef",
     "ListTrafficPolicyInstancesRequestRequestTypeDef",
     "ListTrafficPolicyVersionsRequestRequestTypeDef",
-    "ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
     "ListVPCAssociationAuthorizationsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ResourceRecordOutputTypeDef",
     "ResourceRecordTypeDef",
-    "ResponseMetadataTypeDef",
+    "TagOutputTypeDef",
     "TestDNSAnswerRequestRequestTypeDef",
-    "TestDNSAnswerResponseTypeDef",
     "UpdateHostedZoneCommentRequestRequestTypeDef",
     "UpdateTrafficPolicyCommentRequestRequestTypeDef",
     "UpdateTrafficPolicyInstanceRequestRequestTypeDef",
-    "GetAccountLimitResponseTypeDef",
     "ActivateKeySigningKeyResponseTypeDef",
     "AssociateVPCWithHostedZoneResponseTypeDef",
+    "ChangeCidrCollectionResponseTypeDef",
     "ChangeResourceRecordSetsResponseTypeDef",
     "DeactivateKeySigningKeyResponseTypeDef",
     "DeleteHostedZoneResponseTypeDef",
     "DeleteKeySigningKeyResponseTypeDef",
     "DisableHostedZoneDNSSECResponseTypeDef",
     "DisassociateVPCFromHostedZoneResponseTypeDef",
     "EnableHostedZoneDNSSECResponseTypeDef",
+    "GetAccountLimitResponseTypeDef",
     "GetChangeResponseTypeDef",
+    "GetCheckerIpRangesResponseTypeDef",
+    "GetHealthCheckCountResponseTypeDef",
+    "GetHostedZoneCountResponseTypeDef",
+    "GetTrafficPolicyInstanceCountResponseTypeDef",
+    "TestDNSAnswerResponseTypeDef",
+    "HealthCheckConfigOutputTypeDef",
     "HealthCheckConfigTypeDef",
     "UpdateHealthCheckRequestRequestTypeDef",
     "AssociateVPCWithHostedZoneRequestRequestTypeDef",
     "CreateVPCAssociationAuthorizationRequestRequestTypeDef",
-    "CreateVPCAssociationAuthorizationResponseTypeDef",
     "DeleteVPCAssociationAuthorizationRequestRequestTypeDef",
     "DisassociateVPCFromHostedZoneRequestRequestTypeDef",
-    "ListVPCAssociationAuthorizationsResponseTypeDef",
     "ChangeCidrCollectionRequestRequestTypeDef",
     "ChangeTagsForResourceRequestRequestTypeDef",
-    "ResourceTagSetTypeDef",
     "ListCidrBlocksResponseTypeDef",
     "CreateCidrCollectionResponseTypeDef",
     "CloudWatchAlarmConfigurationTypeDef",
     "ListCidrCollectionsResponseTypeDef",
     "CreateHostedZoneRequestRequestTypeDef",
     "CreateReusableDelegationSetResponseTypeDef",
     "GetReusableDelegationSetResponseTypeDef",
     "ListReusableDelegationSetsResponseTypeDef",
+    "CreateVPCAssociationAuthorizationResponseTypeDef",
+    "ListVPCAssociationAuthorizationsResponseTypeDef",
     "CreateKeySigningKeyResponseTypeDef",
     "CreateQueryLoggingConfigResponseTypeDef",
     "GetQueryLoggingConfigResponseTypeDef",
     "ListQueryLoggingConfigsResponseTypeDef",
     "CreateTrafficPolicyInstanceResponseTypeDef",
     "GetTrafficPolicyInstanceResponseTypeDef",
     "ListTrafficPolicyInstancesByHostedZoneResponseTypeDef",
@@ -198,31 +198,41 @@
     "ListGeoLocationsResponseTypeDef",
     "GetChangeRequestResourceRecordSetsChangedWaitTypeDef",
     "GetHostedZoneLimitResponseTypeDef",
     "GetReusableDelegationSetLimitResponseTypeDef",
     "HealthCheckObservationTypeDef",
     "HostedZoneTypeDef",
     "HostedZoneSummaryTypeDef",
+    "ListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
+    "ListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
+    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
+    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
+    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
+    "ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
+    "ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
     "ListCidrLocationsResponseTypeDef",
     "ListTrafficPoliciesResponseTypeDef",
+    "ResourceRecordSetOutputTypeDef",
     "ResourceRecordSetTypeDef",
+    "ResourceTagSetTypeDef",
     "CreateHealthCheckRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTagsForResourcesResponseTypeDef",
     "HealthCheckTypeDef",
     "GetHealthCheckLastFailureReasonResponseTypeDef",
     "GetHealthCheckStatusResponseTypeDef",
     "CreateHostedZoneResponseTypeDef",
     "GetHostedZoneResponseTypeDef",
     "ListHostedZonesByNameResponseTypeDef",
     "ListHostedZonesResponseTypeDef",
     "UpdateHostedZoneCommentResponseTypeDef",
     "ListHostedZonesByVPCResponseTypeDef",
-    "ChangeTypeDef",
     "ListResourceRecordSetsResponseTypeDef",
+    "ChangeTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTagsForResourcesResponseTypeDef",
     "CreateHealthCheckResponseTypeDef",
     "GetHealthCheckResponseTypeDef",
     "ListHealthChecksResponseTypeDef",
     "UpdateHealthCheckResponseTypeDef",
     "ChangeBatchTypeDef",
     "ChangeResourceRecordSetsRequestRequestTypeDef",
 )
@@ -260,22 +270,50 @@
 )
 
 
 class ChangeInfoTypeDef(_RequiredChangeInfoTypeDef, _OptionalChangeInfoTypeDef):
     pass
 
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+AlarmIdentifierOutputTypeDef = TypedDict(
+    "AlarmIdentifierOutputTypeDef",
+    {
+        "Region": CloudWatchRegionType,
+        "Name": str,
+    },
+)
+
 AlarmIdentifierTypeDef = TypedDict(
     "AlarmIdentifierTypeDef",
     {
         "Region": CloudWatchRegionType,
         "Name": str,
     },
 )
 
+AliasTargetOutputTypeDef = TypedDict(
+    "AliasTargetOutputTypeDef",
+    {
+        "HostedZoneId": str,
+        "DNSName": str,
+        "EvaluateTargetHealth": bool,
+    },
+)
+
 AliasTargetTypeDef = TypedDict(
     "AliasTargetTypeDef",
     {
         "HostedZoneId": str,
         "DNSName": str,
         "EvaluateTargetHealth": bool,
     },
@@ -295,22 +333,14 @@
     {
         "LocationName": str,
         "Action": CidrCollectionChangeActionType,
         "CidrList": Sequence[str],
     },
 )
 
-ChangeCidrCollectionResponseTypeDef = TypedDict(
-    "ChangeCidrCollectionResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -332,14 +362,22 @@
         "Id": str,
         "Name": str,
         "Version": int,
     },
     total=False,
 )
 
+CidrRoutingConfigOutputTypeDef = TypedDict(
+    "CidrRoutingConfigOutputTypeDef",
+    {
+        "CollectionId": str,
+        "LocationName": str,
+    },
+)
+
 CidrRoutingConfigTypeDef = TypedDict(
     "CidrRoutingConfigTypeDef",
     {
         "CollectionId": str,
         "LocationName": str,
     },
 )
@@ -396,14 +434,23 @@
 )
 
 
 class DelegationSetTypeDef(_RequiredDelegationSetTypeDef, _OptionalDelegationSetTypeDef):
     pass
 
 
+VPCOutputTypeDef = TypedDict(
+    "VPCOutputTypeDef",
+    {
+        "VPCRegion": VPCRegionType,
+        "VPCId": str,
+    },
+    total=False,
+)
+
 CreateKeySigningKeyRequestRequestTypeDef = TypedDict(
     "CreateKeySigningKeyRequestRequestTypeDef",
     {
         "CallerReference": str,
         "HostedZoneId": str,
         "KeyManagementServiceArn": str,
         "Name": str,
@@ -666,14 +713,24 @@
         "CountryName": str,
         "SubdivisionCode": str,
         "SubdivisionName": str,
     },
     total=False,
 )
 
+GeoLocationOutputTypeDef = TypedDict(
+    "GeoLocationOutputTypeDef",
+    {
+        "ContinentCode": str,
+        "CountryCode": str,
+        "SubdivisionCode": str,
+    },
+    total=False,
+)
+
 GeoLocationTypeDef = TypedDict(
     "GeoLocationTypeDef",
     {
         "ContinentCode": str,
         "CountryCode": str,
         "SubdivisionCode": str,
     },
@@ -699,22 +756,14 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-GetCheckerIpRangesResponseTypeDef = TypedDict(
-    "GetCheckerIpRangesResponseTypeDef",
-    {
-        "CheckerIpRanges": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDNSSECRequestRequestTypeDef = TypedDict(
     "GetDNSSECRequestRequestTypeDef",
     {
         "HostedZoneId": str,
     },
 )
 
@@ -724,22 +773,14 @@
         "ContinentCode": str,
         "CountryCode": str,
         "SubdivisionCode": str,
     },
     total=False,
 )
 
-GetHealthCheckCountResponseTypeDef = TypedDict(
-    "GetHealthCheckCountResponseTypeDef",
-    {
-        "HealthCheckCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetHealthCheckLastFailureReasonRequestRequestTypeDef = TypedDict(
     "GetHealthCheckLastFailureReasonRequestRequestTypeDef",
     {
         "HealthCheckId": str,
     },
 )
 
@@ -753,22 +794,14 @@
 GetHealthCheckStatusRequestRequestTypeDef = TypedDict(
     "GetHealthCheckStatusRequestRequestTypeDef",
     {
         "HealthCheckId": str,
     },
 )
 
-GetHostedZoneCountResponseTypeDef = TypedDict(
-    "GetHostedZoneCountResponseTypeDef",
-    {
-        "HostedZoneCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetHostedZoneLimitRequestRequestTypeDef = TypedDict(
     "GetHostedZoneLimitRequestRequestTypeDef",
     {
         "Type": HostedZoneLimitTypeType,
         "HostedZoneId": str,
     },
 )
@@ -814,22 +847,14 @@
 GetReusableDelegationSetRequestRequestTypeDef = TypedDict(
     "GetReusableDelegationSetRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-GetTrafficPolicyInstanceCountResponseTypeDef = TypedDict(
-    "GetTrafficPolicyInstanceCountResponseTypeDef",
-    {
-        "TrafficPolicyInstanceCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTrafficPolicyInstanceRequestRequestTypeDef = TypedDict(
     "GetTrafficPolicyInstanceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -855,46 +880,42 @@
     {
         "ServicePrincipal": str,
         "Description": str,
     },
     total=False,
 )
 
+HostedZoneConfigOutputTypeDef = TypedDict(
+    "HostedZoneConfigOutputTypeDef",
+    {
+        "Comment": str,
+        "PrivateZone": bool,
+    },
+    total=False,
+)
+
 HostedZoneOwnerTypeDef = TypedDict(
     "HostedZoneOwnerTypeDef",
     {
         "OwningAccount": str,
         "OwningService": str,
     },
     total=False,
 )
 
-_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
-    "_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
-    "_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "LocationName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListCidrBlocksRequestListCidrBlocksPaginateTypeDef(
-    _RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
-    _OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListCidrBlocksRequestRequestTypeDef = TypedDict(
     "_RequiredListCidrBlocksRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListCidrBlocksRequestRequestTypeDef = TypedDict(
@@ -910,53 +931,23 @@
 
 class ListCidrBlocksRequestRequestTypeDef(
     _RequiredListCidrBlocksRequestRequestTypeDef, _OptionalListCidrBlocksRequestRequestTypeDef
 ):
     pass
 
 
-ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef = TypedDict(
-    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCidrCollectionsRequestRequestTypeDef = TypedDict(
     "ListCidrCollectionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": str,
     },
     total=False,
 )
 
-_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
-    "_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
-    "_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListCidrLocationsRequestListCidrLocationsPaginateTypeDef(
-    _RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
-    _OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListCidrLocationsRequestRequestTypeDef = TypedDict(
     "_RequiredListCidrLocationsRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListCidrLocationsRequestRequestTypeDef = TypedDict(
@@ -990,22 +981,14 @@
         "StartCountryCode": str,
         "StartSubdivisionCode": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-ListHealthChecksRequestListHealthChecksPaginateTypeDef = TypedDict(
-    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListHealthChecksRequestRequestTypeDef = TypedDict(
     "ListHealthChecksRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -1041,74 +1024,34 @@
 class ListHostedZonesByVPCRequestRequestTypeDef(
     _RequiredListHostedZonesByVPCRequestRequestTypeDef,
     _OptionalListHostedZonesByVPCRequestRequestTypeDef,
 ):
     pass
 
 
-ListHostedZonesRequestListHostedZonesPaginateTypeDef = TypedDict(
-    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
-    {
-        "DelegationSetId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListHostedZonesRequestRequestTypeDef = TypedDict(
     "ListHostedZonesRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
         "DelegationSetId": str,
     },
     total=False,
 )
 
-ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef = TypedDict(
-    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
-    {
-        "HostedZoneId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQueryLoggingConfigsRequestRequestTypeDef = TypedDict(
     "ListQueryLoggingConfigsRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "NextToken": str,
         "MaxResults": str,
     },
     total=False,
 )
 
-_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
-    "_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
-    {
-        "HostedZoneId": str,
-    },
-)
-_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
-    "_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef(
-    _RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
-    _OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResourceRecordSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceRecordSetsRequestRequestTypeDef",
     {
         "HostedZoneId": str,
     },
 )
 _OptionalListResourceRecordSetsRequestRequestTypeDef = TypedDict(
@@ -1255,37 +1198,14 @@
 class ListTrafficPolicyVersionsRequestRequestTypeDef(
     _RequiredListTrafficPolicyVersionsRequestRequestTypeDef,
     _OptionalListTrafficPolicyVersionsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
-    "_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
-    {
-        "HostedZoneId": str,
-    },
-)
-_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
-    "_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
-    {
-        "MaxResults": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef(
-    _RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
-    _OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListVPCAssociationAuthorizationsRequestRequestTypeDef = TypedDict(
     "_RequiredListVPCAssociationAuthorizationsRequestRequestTypeDef",
     {
         "HostedZoneId": str,
     },
 )
 _OptionalListVPCAssociationAuthorizationsRequestRequestTypeDef = TypedDict(
@@ -1301,40 +1221,35 @@
 class ListVPCAssociationAuthorizationsRequestRequestTypeDef(
     _RequiredListVPCAssociationAuthorizationsRequestRequestTypeDef,
     _OptionalListVPCAssociationAuthorizationsRequestRequestTypeDef,
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ResourceRecordOutputTypeDef = TypedDict(
+    "ResourceRecordOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Value": str,
     },
-    total=False,
 )
 
 ResourceRecordTypeDef = TypedDict(
     "ResourceRecordTypeDef",
     {
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Key": str,
+        "Value": str,
     },
+    total=False,
 )
 
 _RequiredTestDNSAnswerRequestRequestTypeDef = TypedDict(
     "_RequiredTestDNSAnswerRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "RecordName": str,
@@ -1354,27 +1269,14 @@
 
 class TestDNSAnswerRequestRequestTypeDef(
     _RequiredTestDNSAnswerRequestRequestTypeDef, _OptionalTestDNSAnswerRequestRequestTypeDef
 ):
     pass
 
 
-TestDNSAnswerResponseTypeDef = TypedDict(
-    "TestDNSAnswerResponseTypeDef",
-    {
-        "Nameserver": str,
-        "RecordName": str,
-        "RecordType": RRTypeType,
-        "RecordData": List[str],
-        "ResponseCode": str,
-        "Protocol": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateHostedZoneCommentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateHostedZoneCommentRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateHostedZoneCommentRequestRequestTypeDef = TypedDict(
@@ -1408,103 +1310,193 @@
         "Id": str,
         "TTL": int,
         "TrafficPolicyId": str,
         "TrafficPolicyVersion": int,
     },
 )
 
-GetAccountLimitResponseTypeDef = TypedDict(
-    "GetAccountLimitResponseTypeDef",
-    {
-        "Limit": AccountLimitTypeDef,
-        "Count": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ActivateKeySigningKeyResponseTypeDef = TypedDict(
     "ActivateKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateVPCWithHostedZoneResponseTypeDef = TypedDict(
     "AssociateVPCWithHostedZoneResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ChangeCidrCollectionResponseTypeDef = TypedDict(
+    "ChangeCidrCollectionResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeResourceRecordSetsResponseTypeDef = TypedDict(
     "ChangeResourceRecordSetsResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeactivateKeySigningKeyResponseTypeDef = TypedDict(
     "DeactivateKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteHostedZoneResponseTypeDef = TypedDict(
     "DeleteHostedZoneResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteKeySigningKeyResponseTypeDef = TypedDict(
     "DeleteKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisableHostedZoneDNSSECResponseTypeDef = TypedDict(
     "DisableHostedZoneDNSSECResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateVPCFromHostedZoneResponseTypeDef = TypedDict(
     "DisassociateVPCFromHostedZoneResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnableHostedZoneDNSSECResponseTypeDef = TypedDict(
     "EnableHostedZoneDNSSECResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountLimitResponseTypeDef = TypedDict(
+    "GetAccountLimitResponseTypeDef",
+    {
+        "Limit": AccountLimitTypeDef,
+        "Count": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChangeResponseTypeDef = TypedDict(
     "GetChangeResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetCheckerIpRangesResponseTypeDef = TypedDict(
+    "GetCheckerIpRangesResponseTypeDef",
+    {
+        "CheckerIpRanges": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetHealthCheckCountResponseTypeDef = TypedDict(
+    "GetHealthCheckCountResponseTypeDef",
+    {
+        "HealthCheckCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetHostedZoneCountResponseTypeDef = TypedDict(
+    "GetHostedZoneCountResponseTypeDef",
+    {
+        "HostedZoneCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTrafficPolicyInstanceCountResponseTypeDef = TypedDict(
+    "GetTrafficPolicyInstanceCountResponseTypeDef",
+    {
+        "TrafficPolicyInstanceCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestDNSAnswerResponseTypeDef = TypedDict(
+    "TestDNSAnswerResponseTypeDef",
+    {
+        "Nameserver": str,
+        "RecordName": str,
+        "RecordType": RRTypeType,
+        "RecordData": List[str],
+        "ResponseCode": str,
+        "Protocol": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredHealthCheckConfigOutputTypeDef = TypedDict(
+    "_RequiredHealthCheckConfigOutputTypeDef",
+    {
+        "Type": HealthCheckTypeType,
+    },
+)
+_OptionalHealthCheckConfigOutputTypeDef = TypedDict(
+    "_OptionalHealthCheckConfigOutputTypeDef",
+    {
+        "IPAddress": str,
+        "Port": int,
+        "ResourcePath": str,
+        "FullyQualifiedDomainName": str,
+        "SearchString": str,
+        "RequestInterval": int,
+        "FailureThreshold": int,
+        "MeasureLatency": bool,
+        "Inverted": bool,
+        "Disabled": bool,
+        "HealthThreshold": int,
+        "ChildHealthChecks": List[str],
+        "EnableSNI": bool,
+        "Regions": List[HealthCheckRegionType],
+        "AlarmIdentifier": AlarmIdentifierOutputTypeDef,
+        "InsufficientDataHealthStatus": InsufficientDataHealthStatusType,
+        "RoutingControlArn": str,
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
 _RequiredHealthCheckConfigTypeDef = TypedDict(
     "_RequiredHealthCheckConfigTypeDef",
     {
         "Type": HealthCheckTypeType,
     },
 )
 _OptionalHealthCheckConfigTypeDef = TypedDict(
@@ -1601,23 +1593,14 @@
     "CreateVPCAssociationAuthorizationRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "VPC": VPCTypeDef,
     },
 )
 
-CreateVPCAssociationAuthorizationResponseTypeDef = TypedDict(
-    "CreateVPCAssociationAuthorizationResponseTypeDef",
-    {
-        "HostedZoneId": str,
-        "VPC": VPCTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteVPCAssociationAuthorizationRequestRequestTypeDef = TypedDict(
     "DeleteVPCAssociationAuthorizationRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "VPC": VPCTypeDef,
     },
 )
@@ -1641,24 +1624,14 @@
 class DisassociateVPCFromHostedZoneRequestRequestTypeDef(
     _RequiredDisassociateVPCFromHostedZoneRequestRequestTypeDef,
     _OptionalDisassociateVPCFromHostedZoneRequestRequestTypeDef,
 ):
     pass
 
 
-ListVPCAssociationAuthorizationsResponseTypeDef = TypedDict(
-    "ListVPCAssociationAuthorizationsResponseTypeDef",
-    {
-        "HostedZoneId": str,
-        "NextToken": str,
-        "VPCs": List[VPCTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredChangeCidrCollectionRequestRequestTypeDef = TypedDict(
     "_RequiredChangeCidrCollectionRequestRequestTypeDef",
     {
         "Id": str,
         "Changes": Sequence[CidrCollectionChangeTypeDef],
     },
 )
@@ -1698,39 +1671,29 @@
 class ChangeTagsForResourceRequestRequestTypeDef(
     _RequiredChangeTagsForResourceRequestRequestTypeDef,
     _OptionalChangeTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-ResourceTagSetTypeDef = TypedDict(
-    "ResourceTagSetTypeDef",
-    {
-        "ResourceType": TagResourceTypeType,
-        "ResourceId": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
 ListCidrBlocksResponseTypeDef = TypedDict(
     "ListCidrBlocksResponseTypeDef",
     {
         "NextToken": str,
         "CidrBlocks": List[CidrBlockSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCidrCollectionResponseTypeDef = TypedDict(
     "CreateCidrCollectionResponseTypeDef",
     {
         "Collection": CidrCollectionTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCloudWatchAlarmConfigurationTypeDef = TypedDict(
     "_RequiredCloudWatchAlarmConfigurationTypeDef",
     {
         "EvaluationPeriods": int,
@@ -1758,15 +1721,15 @@
 
 
 ListCidrCollectionsResponseTypeDef = TypedDict(
     "ListCidrCollectionsResponseTypeDef",
     {
         "NextToken": str,
         "CidrCollections": List[CollectionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateHostedZoneRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHostedZoneRequestRequestTypeDef",
     {
         "Name": str,
@@ -1791,209 +1754,228 @@
 
 
 CreateReusableDelegationSetResponseTypeDef = TypedDict(
     "CreateReusableDelegationSetResponseTypeDef",
     {
         "DelegationSet": DelegationSetTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReusableDelegationSetResponseTypeDef = TypedDict(
     "GetReusableDelegationSetResponseTypeDef",
     {
         "DelegationSet": DelegationSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReusableDelegationSetsResponseTypeDef = TypedDict(
     "ListReusableDelegationSetsResponseTypeDef",
     {
         "DelegationSets": List[DelegationSetTypeDef],
         "Marker": str,
         "IsTruncated": bool,
         "NextMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVPCAssociationAuthorizationResponseTypeDef = TypedDict(
+    "CreateVPCAssociationAuthorizationResponseTypeDef",
+    {
+        "HostedZoneId": str,
+        "VPC": VPCOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListVPCAssociationAuthorizationsResponseTypeDef = TypedDict(
+    "ListVPCAssociationAuthorizationsResponseTypeDef",
+    {
+        "HostedZoneId": str,
+        "NextToken": str,
+        "VPCs": List[VPCOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateKeySigningKeyResponseTypeDef = TypedDict(
     "CreateKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
         "KeySigningKey": KeySigningKeyTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateQueryLoggingConfigResponseTypeDef = TypedDict(
     "CreateQueryLoggingConfigResponseTypeDef",
     {
         "QueryLoggingConfig": QueryLoggingConfigTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueryLoggingConfigResponseTypeDef = TypedDict(
     "GetQueryLoggingConfigResponseTypeDef",
     {
         "QueryLoggingConfig": QueryLoggingConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQueryLoggingConfigsResponseTypeDef = TypedDict(
     "ListQueryLoggingConfigsResponseTypeDef",
     {
         "QueryLoggingConfigs": List[QueryLoggingConfigTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTrafficPolicyInstanceResponseTypeDef = TypedDict(
     "CreateTrafficPolicyInstanceResponseTypeDef",
     {
         "TrafficPolicyInstance": TrafficPolicyInstanceTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTrafficPolicyInstanceResponseTypeDef = TypedDict(
     "GetTrafficPolicyInstanceResponseTypeDef",
     {
         "TrafficPolicyInstance": TrafficPolicyInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrafficPolicyInstancesByHostedZoneResponseTypeDef = TypedDict(
     "ListTrafficPolicyInstancesByHostedZoneResponseTypeDef",
     {
         "TrafficPolicyInstances": List[TrafficPolicyInstanceTypeDef],
         "TrafficPolicyInstanceNameMarker": str,
         "TrafficPolicyInstanceTypeMarker": RRTypeType,
         "IsTruncated": bool,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrafficPolicyInstancesByPolicyResponseTypeDef = TypedDict(
     "ListTrafficPolicyInstancesByPolicyResponseTypeDef",
     {
         "TrafficPolicyInstances": List[TrafficPolicyInstanceTypeDef],
         "HostedZoneIdMarker": str,
         "TrafficPolicyInstanceNameMarker": str,
         "TrafficPolicyInstanceTypeMarker": RRTypeType,
         "IsTruncated": bool,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrafficPolicyInstancesResponseTypeDef = TypedDict(
     "ListTrafficPolicyInstancesResponseTypeDef",
     {
         "TrafficPolicyInstances": List[TrafficPolicyInstanceTypeDef],
         "HostedZoneIdMarker": str,
         "TrafficPolicyInstanceNameMarker": str,
         "TrafficPolicyInstanceTypeMarker": RRTypeType,
         "IsTruncated": bool,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTrafficPolicyInstanceResponseTypeDef = TypedDict(
     "UpdateTrafficPolicyInstanceResponseTypeDef",
     {
         "TrafficPolicyInstance": TrafficPolicyInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTrafficPolicyResponseTypeDef = TypedDict(
     "CreateTrafficPolicyResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTrafficPolicyVersionResponseTypeDef = TypedDict(
     "CreateTrafficPolicyVersionResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTrafficPolicyResponseTypeDef = TypedDict(
     "GetTrafficPolicyResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrafficPolicyVersionsResponseTypeDef = TypedDict(
     "ListTrafficPolicyVersionsResponseTypeDef",
     {
         "TrafficPolicies": List[TrafficPolicyTypeDef],
         "IsTruncated": bool,
         "TrafficPolicyVersionMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTrafficPolicyCommentResponseTypeDef = TypedDict(
     "UpdateTrafficPolicyCommentResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDNSSECResponseTypeDef = TypedDict(
     "GetDNSSECResponseTypeDef",
     {
         "Status": DNSSECStatusTypeDef,
         "KeySigningKeys": List[KeySigningKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGeoLocationResponseTypeDef = TypedDict(
     "GetGeoLocationResponseTypeDef",
     {
         "GeoLocationDetails": GeoLocationDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGeoLocationsResponseTypeDef = TypedDict(
     "ListGeoLocationsResponseTypeDef",
     {
         "GeoLocationDetailsList": List[GeoLocationDetailsTypeDef],
         "IsTruncated": bool,
         "NextContinentCode": str,
         "NextCountryCode": str,
         "NextSubdivisionCode": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetChangeRequestResourceRecordSetsChangedWaitTypeDef = TypedDict(
     "_RequiredGetChangeRequestResourceRecordSetsChangedWaitTypeDef",
     {
         "Id": str,
@@ -2016,24 +1998,24 @@
 
 
 GetHostedZoneLimitResponseTypeDef = TypedDict(
     "GetHostedZoneLimitResponseTypeDef",
     {
         "Limit": HostedZoneLimitTypeDef,
         "Count": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReusableDelegationSetLimitResponseTypeDef = TypedDict(
     "GetReusableDelegationSetLimitResponseTypeDef",
     {
         "Limit": ReusableDelegationSetLimitTypeDef,
         "Count": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HealthCheckObservationTypeDef = TypedDict(
     "HealthCheckObservationTypeDef",
     {
         "Region": HealthCheckRegionType,
@@ -2050,15 +2032,15 @@
         "Name": str,
         "CallerReference": str,
     },
 )
 _OptionalHostedZoneTypeDef = TypedDict(
     "_OptionalHostedZoneTypeDef",
     {
-        "Config": HostedZoneConfigTypeDef,
+        "Config": HostedZoneConfigOutputTypeDef,
         "ResourceRecordSetCount": int,
         "LinkedService": LinkedServiceTypeDef,
     },
     total=False,
 )
 
 
@@ -2071,33 +2053,190 @@
     {
         "HostedZoneId": str,
         "Name": str,
         "Owner": HostedZoneOwnerTypeDef,
     },
 )
 
+_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
+    "_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
+    "_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+    {
+        "LocationName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListCidrBlocksRequestListCidrBlocksPaginateTypeDef(
+    _RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+    _OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+):
+    pass
+
+
+ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef = TypedDict(
+    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
+    "_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
+    "_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListCidrLocationsRequestListCidrLocationsPaginateTypeDef(
+    _RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
+    _OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
+):
+    pass
+
+
+ListHealthChecksRequestListHealthChecksPaginateTypeDef = TypedDict(
+    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListHostedZonesRequestListHostedZonesPaginateTypeDef = TypedDict(
+    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
+    {
+        "DelegationSetId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef = TypedDict(
+    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
+    {
+        "HostedZoneId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
+    "_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
+    {
+        "HostedZoneId": str,
+    },
+)
+_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
+    "_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef(
+    _RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
+    _OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
+    "_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
+    {
+        "HostedZoneId": str,
+    },
+)
+_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
+    "_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
+    {
+        "MaxResults": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef(
+    _RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
+    _OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
+):
+    pass
+
+
 ListCidrLocationsResponseTypeDef = TypedDict(
     "ListCidrLocationsResponseTypeDef",
     {
         "NextToken": str,
         "CidrLocations": List[LocationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrafficPoliciesResponseTypeDef = TypedDict(
     "ListTrafficPoliciesResponseTypeDef",
     {
         "TrafficPolicySummaries": List[TrafficPolicySummaryTypeDef],
         "IsTruncated": bool,
         "TrafficPolicyIdMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredResourceRecordSetOutputTypeDef = TypedDict(
+    "_RequiredResourceRecordSetOutputTypeDef",
+    {
+        "Name": str,
+        "Type": RRTypeType,
     },
 )
+_OptionalResourceRecordSetOutputTypeDef = TypedDict(
+    "_OptionalResourceRecordSetOutputTypeDef",
+    {
+        "SetIdentifier": str,
+        "Weight": int,
+        "Region": ResourceRecordSetRegionType,
+        "GeoLocation": GeoLocationOutputTypeDef,
+        "Failover": ResourceRecordSetFailoverType,
+        "MultiValueAnswer": bool,
+        "TTL": int,
+        "ResourceRecords": List[ResourceRecordOutputTypeDef],
+        "AliasTarget": AliasTargetOutputTypeDef,
+        "HealthCheckId": str,
+        "TrafficPolicyInstanceId": str,
+        "CidrRoutingConfig": CidrRoutingConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ResourceRecordSetOutputTypeDef(
+    _RequiredResourceRecordSetOutputTypeDef, _OptionalResourceRecordSetOutputTypeDef
+):
+    pass
+
 
 _RequiredResourceRecordSetTypeDef = TypedDict(
     "_RequiredResourceRecordSetTypeDef",
     {
         "Name": str,
         "Type": RRTypeType,
     },
@@ -2124,44 +2263,38 @@
 
 class ResourceRecordSetTypeDef(
     _RequiredResourceRecordSetTypeDef, _OptionalResourceRecordSetTypeDef
 ):
     pass
 
 
-CreateHealthCheckRequestRequestTypeDef = TypedDict(
-    "CreateHealthCheckRequestRequestTypeDef",
-    {
-        "CallerReference": str,
-        "HealthCheckConfig": HealthCheckConfigTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ResourceTagSetTypeDef = TypedDict(
+    "ResourceTagSetTypeDef",
     {
-        "ResourceTagSet": ResourceTagSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceType": TagResourceTypeType,
+        "ResourceId": str,
+        "Tags": List[TagOutputTypeDef],
     },
+    total=False,
 )
 
-ListTagsForResourcesResponseTypeDef = TypedDict(
-    "ListTagsForResourcesResponseTypeDef",
+CreateHealthCheckRequestRequestTypeDef = TypedDict(
+    "CreateHealthCheckRequestRequestTypeDef",
     {
-        "ResourceTagSets": List[ResourceTagSetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CallerReference": str,
+        "HealthCheckConfig": HealthCheckConfigTypeDef,
     },
 )
 
 _RequiredHealthCheckTypeDef = TypedDict(
     "_RequiredHealthCheckTypeDef",
     {
         "Id": str,
         "CallerReference": str,
-        "HealthCheckConfig": HealthCheckConfigTypeDef,
+        "HealthCheckConfig": HealthCheckConfigOutputTypeDef,
         "HealthCheckVersion": int,
     },
 )
 _OptionalHealthCheckTypeDef = TypedDict(
     "_OptionalHealthCheckTypeDef",
     {
         "LinkedService": LinkedServiceTypeDef,
@@ -2175,147 +2308,163 @@
     pass
 
 
 GetHealthCheckLastFailureReasonResponseTypeDef = TypedDict(
     "GetHealthCheckLastFailureReasonResponseTypeDef",
     {
         "HealthCheckObservations": List[HealthCheckObservationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHealthCheckStatusResponseTypeDef = TypedDict(
     "GetHealthCheckStatusResponseTypeDef",
     {
         "HealthCheckObservations": List[HealthCheckObservationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateHostedZoneResponseTypeDef = TypedDict(
     "CreateHostedZoneResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
         "ChangeInfo": ChangeInfoTypeDef,
         "DelegationSet": DelegationSetTypeDef,
-        "VPC": VPCTypeDef,
+        "VPC": VPCOutputTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHostedZoneResponseTypeDef = TypedDict(
     "GetHostedZoneResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
         "DelegationSet": DelegationSetTypeDef,
-        "VPCs": List[VPCTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VPCs": List[VPCOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHostedZonesByNameResponseTypeDef = TypedDict(
     "ListHostedZonesByNameResponseTypeDef",
     {
         "HostedZones": List[HostedZoneTypeDef],
         "DNSName": str,
         "HostedZoneId": str,
         "IsTruncated": bool,
         "NextDNSName": str,
         "NextHostedZoneId": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHostedZonesResponseTypeDef = TypedDict(
     "ListHostedZonesResponseTypeDef",
     {
         "HostedZones": List[HostedZoneTypeDef],
         "Marker": str,
         "IsTruncated": bool,
         "NextMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateHostedZoneCommentResponseTypeDef = TypedDict(
     "UpdateHostedZoneCommentResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHostedZonesByVPCResponseTypeDef = TypedDict(
     "ListHostedZonesByVPCResponseTypeDef",
     {
         "HostedZoneSummaries": List[HostedZoneSummaryTypeDef],
         "MaxItems": str,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListResourceRecordSetsResponseTypeDef = TypedDict(
+    "ListResourceRecordSetsResponseTypeDef",
+    {
+        "ResourceRecordSets": List[ResourceRecordSetOutputTypeDef],
+        "IsTruncated": bool,
+        "NextRecordName": str,
+        "NextRecordType": RRTypeType,
+        "NextRecordIdentifier": str,
+        "MaxItems": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeTypeDef = TypedDict(
     "ChangeTypeDef",
     {
         "Action": ChangeActionType,
         "ResourceRecordSet": ResourceRecordSetTypeDef,
     },
 )
 
-ListResourceRecordSetsResponseTypeDef = TypedDict(
-    "ListResourceRecordSetsResponseTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ResourceRecordSets": List[ResourceRecordSetTypeDef],
-        "IsTruncated": bool,
-        "NextRecordName": str,
-        "NextRecordType": RRTypeType,
-        "NextRecordIdentifier": str,
-        "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceTagSet": ResourceTagSetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourcesResponseTypeDef = TypedDict(
+    "ListTagsForResourcesResponseTypeDef",
+    {
+        "ResourceTagSets": List[ResourceTagSetTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateHealthCheckResponseTypeDef = TypedDict(
     "CreateHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHealthCheckResponseTypeDef = TypedDict(
     "GetHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHealthChecksResponseTypeDef = TypedDict(
     "ListHealthChecksResponseTypeDef",
     {
         "HealthChecks": List[HealthCheckTypeDef],
         "Marker": str,
         "IsTruncated": bool,
         "NextMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateHealthCheckResponseTypeDef = TypedDict(
     "UpdateHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredChangeBatchTypeDef = TypedDict(
     "_RequiredChangeBatchTypeDef",
     {
         "Changes": Sequence[ChangeTypeDef],
```

### Comparing `mypy-boto3-route53-1.28.0/mypy_boto3_route53/type_defs.pyi` & `mypy-boto3-route53-1.28.12/mypy_boto3_route53/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,28 +44,32 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountLimitTypeDef",
     "ActivateKeySigningKeyRequestRequestTypeDef",
     "ChangeInfoTypeDef",
+    "ResponseMetadataTypeDef",
+    "AlarmIdentifierOutputTypeDef",
     "AlarmIdentifierTypeDef",
+    "AliasTargetOutputTypeDef",
     "AliasTargetTypeDef",
     "VPCTypeDef",
     "CidrCollectionChangeTypeDef",
-    "ChangeCidrCollectionResponseTypeDef",
     "TagTypeDef",
     "CidrBlockSummaryTypeDef",
     "CidrCollectionTypeDef",
+    "CidrRoutingConfigOutputTypeDef",
     "CidrRoutingConfigTypeDef",
     "DimensionTypeDef",
     "CollectionSummaryTypeDef",
     "CreateCidrCollectionRequestRequestTypeDef",
     "HostedZoneConfigTypeDef",
     "DelegationSetTypeDef",
+    "VPCOutputTypeDef",
     "CreateKeySigningKeyRequestRequestTypeDef",
     "KeySigningKeyTypeDef",
     "CreateQueryLoggingConfigRequestRequestTypeDef",
     "QueryLoggingConfigTypeDef",
     "CreateReusableDelegationSetRequestRequestTypeDef",
     "CreateTrafficPolicyInstanceRequestRequestTypeDef",
     "TrafficPolicyInstanceTypeDef",
@@ -81,106 +85,102 @@
     "DeleteQueryLoggingConfigRequestRequestTypeDef",
     "DeleteReusableDelegationSetRequestRequestTypeDef",
     "DeleteTrafficPolicyInstanceRequestRequestTypeDef",
     "DeleteTrafficPolicyRequestRequestTypeDef",
     "DisableHostedZoneDNSSECRequestRequestTypeDef",
     "EnableHostedZoneDNSSECRequestRequestTypeDef",
     "GeoLocationDetailsTypeDef",
+    "GeoLocationOutputTypeDef",
     "GeoLocationTypeDef",
     "GetAccountLimitRequestRequestTypeDef",
     "GetChangeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
-    "GetCheckerIpRangesResponseTypeDef",
     "GetDNSSECRequestRequestTypeDef",
     "GetGeoLocationRequestRequestTypeDef",
-    "GetHealthCheckCountResponseTypeDef",
     "GetHealthCheckLastFailureReasonRequestRequestTypeDef",
     "GetHealthCheckRequestRequestTypeDef",
     "GetHealthCheckStatusRequestRequestTypeDef",
-    "GetHostedZoneCountResponseTypeDef",
     "GetHostedZoneLimitRequestRequestTypeDef",
     "HostedZoneLimitTypeDef",
     "GetHostedZoneRequestRequestTypeDef",
     "GetQueryLoggingConfigRequestRequestTypeDef",
     "GetReusableDelegationSetLimitRequestRequestTypeDef",
     "ReusableDelegationSetLimitTypeDef",
     "GetReusableDelegationSetRequestRequestTypeDef",
-    "GetTrafficPolicyInstanceCountResponseTypeDef",
     "GetTrafficPolicyInstanceRequestRequestTypeDef",
     "GetTrafficPolicyRequestRequestTypeDef",
     "StatusReportTypeDef",
     "LinkedServiceTypeDef",
+    "HostedZoneConfigOutputTypeDef",
     "HostedZoneOwnerTypeDef",
-    "ListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListCidrBlocksRequestRequestTypeDef",
-    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
     "ListCidrCollectionsRequestRequestTypeDef",
-    "ListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
     "ListCidrLocationsRequestRequestTypeDef",
     "LocationSummaryTypeDef",
     "ListGeoLocationsRequestRequestTypeDef",
-    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
     "ListHealthChecksRequestRequestTypeDef",
     "ListHostedZonesByNameRequestRequestTypeDef",
     "ListHostedZonesByVPCRequestRequestTypeDef",
-    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
     "ListHostedZonesRequestRequestTypeDef",
-    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
     "ListQueryLoggingConfigsRequestRequestTypeDef",
-    "ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
     "ListResourceRecordSetsRequestRequestTypeDef",
     "ListReusableDelegationSetsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourcesRequestRequestTypeDef",
     "ListTrafficPoliciesRequestRequestTypeDef",
     "TrafficPolicySummaryTypeDef",
     "ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef",
     "ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef",
     "ListTrafficPolicyInstancesRequestRequestTypeDef",
     "ListTrafficPolicyVersionsRequestRequestTypeDef",
-    "ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
     "ListVPCAssociationAuthorizationsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ResourceRecordOutputTypeDef",
     "ResourceRecordTypeDef",
-    "ResponseMetadataTypeDef",
+    "TagOutputTypeDef",
     "TestDNSAnswerRequestRequestTypeDef",
-    "TestDNSAnswerResponseTypeDef",
     "UpdateHostedZoneCommentRequestRequestTypeDef",
     "UpdateTrafficPolicyCommentRequestRequestTypeDef",
     "UpdateTrafficPolicyInstanceRequestRequestTypeDef",
-    "GetAccountLimitResponseTypeDef",
     "ActivateKeySigningKeyResponseTypeDef",
     "AssociateVPCWithHostedZoneResponseTypeDef",
+    "ChangeCidrCollectionResponseTypeDef",
     "ChangeResourceRecordSetsResponseTypeDef",
     "DeactivateKeySigningKeyResponseTypeDef",
     "DeleteHostedZoneResponseTypeDef",
     "DeleteKeySigningKeyResponseTypeDef",
     "DisableHostedZoneDNSSECResponseTypeDef",
     "DisassociateVPCFromHostedZoneResponseTypeDef",
     "EnableHostedZoneDNSSECResponseTypeDef",
+    "GetAccountLimitResponseTypeDef",
     "GetChangeResponseTypeDef",
+    "GetCheckerIpRangesResponseTypeDef",
+    "GetHealthCheckCountResponseTypeDef",
+    "GetHostedZoneCountResponseTypeDef",
+    "GetTrafficPolicyInstanceCountResponseTypeDef",
+    "TestDNSAnswerResponseTypeDef",
+    "HealthCheckConfigOutputTypeDef",
     "HealthCheckConfigTypeDef",
     "UpdateHealthCheckRequestRequestTypeDef",
     "AssociateVPCWithHostedZoneRequestRequestTypeDef",
     "CreateVPCAssociationAuthorizationRequestRequestTypeDef",
-    "CreateVPCAssociationAuthorizationResponseTypeDef",
     "DeleteVPCAssociationAuthorizationRequestRequestTypeDef",
     "DisassociateVPCFromHostedZoneRequestRequestTypeDef",
-    "ListVPCAssociationAuthorizationsResponseTypeDef",
     "ChangeCidrCollectionRequestRequestTypeDef",
     "ChangeTagsForResourceRequestRequestTypeDef",
-    "ResourceTagSetTypeDef",
     "ListCidrBlocksResponseTypeDef",
     "CreateCidrCollectionResponseTypeDef",
     "CloudWatchAlarmConfigurationTypeDef",
     "ListCidrCollectionsResponseTypeDef",
     "CreateHostedZoneRequestRequestTypeDef",
     "CreateReusableDelegationSetResponseTypeDef",
     "GetReusableDelegationSetResponseTypeDef",
     "ListReusableDelegationSetsResponseTypeDef",
+    "CreateVPCAssociationAuthorizationResponseTypeDef",
+    "ListVPCAssociationAuthorizationsResponseTypeDef",
     "CreateKeySigningKeyResponseTypeDef",
     "CreateQueryLoggingConfigResponseTypeDef",
     "GetQueryLoggingConfigResponseTypeDef",
     "ListQueryLoggingConfigsResponseTypeDef",
     "CreateTrafficPolicyInstanceResponseTypeDef",
     "GetTrafficPolicyInstanceResponseTypeDef",
     "ListTrafficPolicyInstancesByHostedZoneResponseTypeDef",
@@ -197,31 +197,41 @@
     "ListGeoLocationsResponseTypeDef",
     "GetChangeRequestResourceRecordSetsChangedWaitTypeDef",
     "GetHostedZoneLimitResponseTypeDef",
     "GetReusableDelegationSetLimitResponseTypeDef",
     "HealthCheckObservationTypeDef",
     "HostedZoneTypeDef",
     "HostedZoneSummaryTypeDef",
+    "ListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
+    "ListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
+    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
+    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
+    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
+    "ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
+    "ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
     "ListCidrLocationsResponseTypeDef",
     "ListTrafficPoliciesResponseTypeDef",
+    "ResourceRecordSetOutputTypeDef",
     "ResourceRecordSetTypeDef",
+    "ResourceTagSetTypeDef",
     "CreateHealthCheckRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTagsForResourcesResponseTypeDef",
     "HealthCheckTypeDef",
     "GetHealthCheckLastFailureReasonResponseTypeDef",
     "GetHealthCheckStatusResponseTypeDef",
     "CreateHostedZoneResponseTypeDef",
     "GetHostedZoneResponseTypeDef",
     "ListHostedZonesByNameResponseTypeDef",
     "ListHostedZonesResponseTypeDef",
     "UpdateHostedZoneCommentResponseTypeDef",
     "ListHostedZonesByVPCResponseTypeDef",
-    "ChangeTypeDef",
     "ListResourceRecordSetsResponseTypeDef",
+    "ChangeTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTagsForResourcesResponseTypeDef",
     "CreateHealthCheckResponseTypeDef",
     "GetHealthCheckResponseTypeDef",
     "ListHealthChecksResponseTypeDef",
     "UpdateHealthCheckResponseTypeDef",
     "ChangeBatchTypeDef",
     "ChangeResourceRecordSetsRequestRequestTypeDef",
 )
@@ -257,22 +267,50 @@
     },
     total=False,
 )
 
 class ChangeInfoTypeDef(_RequiredChangeInfoTypeDef, _OptionalChangeInfoTypeDef):
     pass
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+AlarmIdentifierOutputTypeDef = TypedDict(
+    "AlarmIdentifierOutputTypeDef",
+    {
+        "Region": CloudWatchRegionType,
+        "Name": str,
+    },
+)
+
 AlarmIdentifierTypeDef = TypedDict(
     "AlarmIdentifierTypeDef",
     {
         "Region": CloudWatchRegionType,
         "Name": str,
     },
 )
 
+AliasTargetOutputTypeDef = TypedDict(
+    "AliasTargetOutputTypeDef",
+    {
+        "HostedZoneId": str,
+        "DNSName": str,
+        "EvaluateTargetHealth": bool,
+    },
+)
+
 AliasTargetTypeDef = TypedDict(
     "AliasTargetTypeDef",
     {
         "HostedZoneId": str,
         "DNSName": str,
         "EvaluateTargetHealth": bool,
     },
@@ -292,22 +330,14 @@
     {
         "LocationName": str,
         "Action": CidrCollectionChangeActionType,
         "CidrList": Sequence[str],
     },
 )
 
-ChangeCidrCollectionResponseTypeDef = TypedDict(
-    "ChangeCidrCollectionResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -329,14 +359,22 @@
         "Id": str,
         "Name": str,
         "Version": int,
     },
     total=False,
 )
 
+CidrRoutingConfigOutputTypeDef = TypedDict(
+    "CidrRoutingConfigOutputTypeDef",
+    {
+        "CollectionId": str,
+        "LocationName": str,
+    },
+)
+
 CidrRoutingConfigTypeDef = TypedDict(
     "CidrRoutingConfigTypeDef",
     {
         "CollectionId": str,
         "LocationName": str,
     },
 )
@@ -391,14 +429,23 @@
     },
     total=False,
 )
 
 class DelegationSetTypeDef(_RequiredDelegationSetTypeDef, _OptionalDelegationSetTypeDef):
     pass
 
+VPCOutputTypeDef = TypedDict(
+    "VPCOutputTypeDef",
+    {
+        "VPCRegion": VPCRegionType,
+        "VPCId": str,
+    },
+    total=False,
+)
+
 CreateKeySigningKeyRequestRequestTypeDef = TypedDict(
     "CreateKeySigningKeyRequestRequestTypeDef",
     {
         "CallerReference": str,
         "HostedZoneId": str,
         "KeyManagementServiceArn": str,
         "Name": str,
@@ -653,14 +700,24 @@
         "CountryName": str,
         "SubdivisionCode": str,
         "SubdivisionName": str,
     },
     total=False,
 )
 
+GeoLocationOutputTypeDef = TypedDict(
+    "GeoLocationOutputTypeDef",
+    {
+        "ContinentCode": str,
+        "CountryCode": str,
+        "SubdivisionCode": str,
+    },
+    total=False,
+)
+
 GeoLocationTypeDef = TypedDict(
     "GeoLocationTypeDef",
     {
         "ContinentCode": str,
         "CountryCode": str,
         "SubdivisionCode": str,
     },
@@ -686,22 +743,14 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-GetCheckerIpRangesResponseTypeDef = TypedDict(
-    "GetCheckerIpRangesResponseTypeDef",
-    {
-        "CheckerIpRanges": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDNSSECRequestRequestTypeDef = TypedDict(
     "GetDNSSECRequestRequestTypeDef",
     {
         "HostedZoneId": str,
     },
 )
 
@@ -711,22 +760,14 @@
         "ContinentCode": str,
         "CountryCode": str,
         "SubdivisionCode": str,
     },
     total=False,
 )
 
-GetHealthCheckCountResponseTypeDef = TypedDict(
-    "GetHealthCheckCountResponseTypeDef",
-    {
-        "HealthCheckCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetHealthCheckLastFailureReasonRequestRequestTypeDef = TypedDict(
     "GetHealthCheckLastFailureReasonRequestRequestTypeDef",
     {
         "HealthCheckId": str,
     },
 )
 
@@ -740,22 +781,14 @@
 GetHealthCheckStatusRequestRequestTypeDef = TypedDict(
     "GetHealthCheckStatusRequestRequestTypeDef",
     {
         "HealthCheckId": str,
     },
 )
 
-GetHostedZoneCountResponseTypeDef = TypedDict(
-    "GetHostedZoneCountResponseTypeDef",
-    {
-        "HostedZoneCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetHostedZoneLimitRequestRequestTypeDef = TypedDict(
     "GetHostedZoneLimitRequestRequestTypeDef",
     {
         "Type": HostedZoneLimitTypeType,
         "HostedZoneId": str,
     },
 )
@@ -801,22 +834,14 @@
 GetReusableDelegationSetRequestRequestTypeDef = TypedDict(
     "GetReusableDelegationSetRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-GetTrafficPolicyInstanceCountResponseTypeDef = TypedDict(
-    "GetTrafficPolicyInstanceCountResponseTypeDef",
-    {
-        "TrafficPolicyInstanceCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTrafficPolicyInstanceRequestRequestTypeDef = TypedDict(
     "GetTrafficPolicyInstanceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -842,44 +867,42 @@
     {
         "ServicePrincipal": str,
         "Description": str,
     },
     total=False,
 )
 
+HostedZoneConfigOutputTypeDef = TypedDict(
+    "HostedZoneConfigOutputTypeDef",
+    {
+        "Comment": str,
+        "PrivateZone": bool,
+    },
+    total=False,
+)
+
 HostedZoneOwnerTypeDef = TypedDict(
     "HostedZoneOwnerTypeDef",
     {
         "OwningAccount": str,
         "OwningService": str,
     },
     total=False,
 )
 
-_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
-    "_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
-    "_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "LocationName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListCidrBlocksRequestListCidrBlocksPaginateTypeDef(
-    _RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
-    _OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
-):
-    pass
-
 _RequiredListCidrBlocksRequestRequestTypeDef = TypedDict(
     "_RequiredListCidrBlocksRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListCidrBlocksRequestRequestTypeDef = TypedDict(
@@ -893,51 +916,23 @@
 )
 
 class ListCidrBlocksRequestRequestTypeDef(
     _RequiredListCidrBlocksRequestRequestTypeDef, _OptionalListCidrBlocksRequestRequestTypeDef
 ):
     pass
 
-ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef = TypedDict(
-    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCidrCollectionsRequestRequestTypeDef = TypedDict(
     "ListCidrCollectionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": str,
     },
     total=False,
 )
 
-_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
-    "_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
-    "_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListCidrLocationsRequestListCidrLocationsPaginateTypeDef(
-    _RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
-    _OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListCidrLocationsRequestRequestTypeDef = TypedDict(
     "_RequiredListCidrLocationsRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListCidrLocationsRequestRequestTypeDef = TypedDict(
@@ -969,22 +964,14 @@
         "StartCountryCode": str,
         "StartSubdivisionCode": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-ListHealthChecksRequestListHealthChecksPaginateTypeDef = TypedDict(
-    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListHealthChecksRequestRequestTypeDef = TypedDict(
     "ListHealthChecksRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -1018,72 +1005,34 @@
 
 class ListHostedZonesByVPCRequestRequestTypeDef(
     _RequiredListHostedZonesByVPCRequestRequestTypeDef,
     _OptionalListHostedZonesByVPCRequestRequestTypeDef,
 ):
     pass
 
-ListHostedZonesRequestListHostedZonesPaginateTypeDef = TypedDict(
-    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
-    {
-        "DelegationSetId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListHostedZonesRequestRequestTypeDef = TypedDict(
     "ListHostedZonesRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
         "DelegationSetId": str,
     },
     total=False,
 )
 
-ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef = TypedDict(
-    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
-    {
-        "HostedZoneId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQueryLoggingConfigsRequestRequestTypeDef = TypedDict(
     "ListQueryLoggingConfigsRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "NextToken": str,
         "MaxResults": str,
     },
     total=False,
 )
 
-_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
-    "_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
-    {
-        "HostedZoneId": str,
-    },
-)
-_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
-    "_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef(
-    _RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
-    _OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListResourceRecordSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceRecordSetsRequestRequestTypeDef",
     {
         "HostedZoneId": str,
     },
 )
 _OptionalListResourceRecordSetsRequestRequestTypeDef = TypedDict(
@@ -1222,35 +1171,14 @@
 
 class ListTrafficPolicyVersionsRequestRequestTypeDef(
     _RequiredListTrafficPolicyVersionsRequestRequestTypeDef,
     _OptionalListTrafficPolicyVersionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
-    "_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
-    {
-        "HostedZoneId": str,
-    },
-)
-_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
-    "_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
-    {
-        "MaxResults": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef(
-    _RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
-    _OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListVPCAssociationAuthorizationsRequestRequestTypeDef = TypedDict(
     "_RequiredListVPCAssociationAuthorizationsRequestRequestTypeDef",
     {
         "HostedZoneId": str,
     },
 )
 _OptionalListVPCAssociationAuthorizationsRequestRequestTypeDef = TypedDict(
@@ -1264,40 +1192,35 @@
 
 class ListVPCAssociationAuthorizationsRequestRequestTypeDef(
     _RequiredListVPCAssociationAuthorizationsRequestRequestTypeDef,
     _OptionalListVPCAssociationAuthorizationsRequestRequestTypeDef,
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ResourceRecordOutputTypeDef = TypedDict(
+    "ResourceRecordOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Value": str,
     },
-    total=False,
 )
 
 ResourceRecordTypeDef = TypedDict(
     "ResourceRecordTypeDef",
     {
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Key": str,
+        "Value": str,
     },
+    total=False,
 )
 
 _RequiredTestDNSAnswerRequestRequestTypeDef = TypedDict(
     "_RequiredTestDNSAnswerRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "RecordName": str,
@@ -1315,27 +1238,14 @@
 )
 
 class TestDNSAnswerRequestRequestTypeDef(
     _RequiredTestDNSAnswerRequestRequestTypeDef, _OptionalTestDNSAnswerRequestRequestTypeDef
 ):
     pass
 
-TestDNSAnswerResponseTypeDef = TypedDict(
-    "TestDNSAnswerResponseTypeDef",
-    {
-        "Nameserver": str,
-        "RecordName": str,
-        "RecordType": RRTypeType,
-        "RecordData": List[str],
-        "ResponseCode": str,
-        "Protocol": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateHostedZoneCommentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateHostedZoneCommentRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateHostedZoneCommentRequestRequestTypeDef = TypedDict(
@@ -1367,103 +1277,191 @@
         "Id": str,
         "TTL": int,
         "TrafficPolicyId": str,
         "TrafficPolicyVersion": int,
     },
 )
 
-GetAccountLimitResponseTypeDef = TypedDict(
-    "GetAccountLimitResponseTypeDef",
-    {
-        "Limit": AccountLimitTypeDef,
-        "Count": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ActivateKeySigningKeyResponseTypeDef = TypedDict(
     "ActivateKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateVPCWithHostedZoneResponseTypeDef = TypedDict(
     "AssociateVPCWithHostedZoneResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ChangeCidrCollectionResponseTypeDef = TypedDict(
+    "ChangeCidrCollectionResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeResourceRecordSetsResponseTypeDef = TypedDict(
     "ChangeResourceRecordSetsResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeactivateKeySigningKeyResponseTypeDef = TypedDict(
     "DeactivateKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteHostedZoneResponseTypeDef = TypedDict(
     "DeleteHostedZoneResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteKeySigningKeyResponseTypeDef = TypedDict(
     "DeleteKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisableHostedZoneDNSSECResponseTypeDef = TypedDict(
     "DisableHostedZoneDNSSECResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateVPCFromHostedZoneResponseTypeDef = TypedDict(
     "DisassociateVPCFromHostedZoneResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnableHostedZoneDNSSECResponseTypeDef = TypedDict(
     "EnableHostedZoneDNSSECResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountLimitResponseTypeDef = TypedDict(
+    "GetAccountLimitResponseTypeDef",
+    {
+        "Limit": AccountLimitTypeDef,
+        "Count": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChangeResponseTypeDef = TypedDict(
     "GetChangeResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCheckerIpRangesResponseTypeDef = TypedDict(
+    "GetCheckerIpRangesResponseTypeDef",
+    {
+        "CheckerIpRanges": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetHealthCheckCountResponseTypeDef = TypedDict(
+    "GetHealthCheckCountResponseTypeDef",
+    {
+        "HealthCheckCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetHostedZoneCountResponseTypeDef = TypedDict(
+    "GetHostedZoneCountResponseTypeDef",
+    {
+        "HostedZoneCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTrafficPolicyInstanceCountResponseTypeDef = TypedDict(
+    "GetTrafficPolicyInstanceCountResponseTypeDef",
+    {
+        "TrafficPolicyInstanceCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestDNSAnswerResponseTypeDef = TypedDict(
+    "TestDNSAnswerResponseTypeDef",
+    {
+        "Nameserver": str,
+        "RecordName": str,
+        "RecordType": RRTypeType,
+        "RecordData": List[str],
+        "ResponseCode": str,
+        "Protocol": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredHealthCheckConfigOutputTypeDef = TypedDict(
+    "_RequiredHealthCheckConfigOutputTypeDef",
+    {
+        "Type": HealthCheckTypeType,
+    },
+)
+_OptionalHealthCheckConfigOutputTypeDef = TypedDict(
+    "_OptionalHealthCheckConfigOutputTypeDef",
+    {
+        "IPAddress": str,
+        "Port": int,
+        "ResourcePath": str,
+        "FullyQualifiedDomainName": str,
+        "SearchString": str,
+        "RequestInterval": int,
+        "FailureThreshold": int,
+        "MeasureLatency": bool,
+        "Inverted": bool,
+        "Disabled": bool,
+        "HealthThreshold": int,
+        "ChildHealthChecks": List[str],
+        "EnableSNI": bool,
+        "Regions": List[HealthCheckRegionType],
+        "AlarmIdentifier": AlarmIdentifierOutputTypeDef,
+        "InsufficientDataHealthStatus": InsufficientDataHealthStatusType,
+        "RoutingControlArn": str,
+    },
+    total=False,
+)
+
+class HealthCheckConfigOutputTypeDef(
+    _RequiredHealthCheckConfigOutputTypeDef, _OptionalHealthCheckConfigOutputTypeDef
+):
+    pass
+
 _RequiredHealthCheckConfigTypeDef = TypedDict(
     "_RequiredHealthCheckConfigTypeDef",
     {
         "Type": HealthCheckTypeType,
     },
 )
 _OptionalHealthCheckConfigTypeDef = TypedDict(
@@ -1554,23 +1552,14 @@
     "CreateVPCAssociationAuthorizationRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "VPC": VPCTypeDef,
     },
 )
 
-CreateVPCAssociationAuthorizationResponseTypeDef = TypedDict(
-    "CreateVPCAssociationAuthorizationResponseTypeDef",
-    {
-        "HostedZoneId": str,
-        "VPC": VPCTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteVPCAssociationAuthorizationRequestRequestTypeDef = TypedDict(
     "DeleteVPCAssociationAuthorizationRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "VPC": VPCTypeDef,
     },
 )
@@ -1592,24 +1581,14 @@
 
 class DisassociateVPCFromHostedZoneRequestRequestTypeDef(
     _RequiredDisassociateVPCFromHostedZoneRequestRequestTypeDef,
     _OptionalDisassociateVPCFromHostedZoneRequestRequestTypeDef,
 ):
     pass
 
-ListVPCAssociationAuthorizationsResponseTypeDef = TypedDict(
-    "ListVPCAssociationAuthorizationsResponseTypeDef",
-    {
-        "HostedZoneId": str,
-        "NextToken": str,
-        "VPCs": List[VPCTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredChangeCidrCollectionRequestRequestTypeDef = TypedDict(
     "_RequiredChangeCidrCollectionRequestRequestTypeDef",
     {
         "Id": str,
         "Changes": Sequence[CidrCollectionChangeTypeDef],
     },
 )
@@ -1645,39 +1624,29 @@
 
 class ChangeTagsForResourceRequestRequestTypeDef(
     _RequiredChangeTagsForResourceRequestRequestTypeDef,
     _OptionalChangeTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-ResourceTagSetTypeDef = TypedDict(
-    "ResourceTagSetTypeDef",
-    {
-        "ResourceType": TagResourceTypeType,
-        "ResourceId": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
 ListCidrBlocksResponseTypeDef = TypedDict(
     "ListCidrBlocksResponseTypeDef",
     {
         "NextToken": str,
         "CidrBlocks": List[CidrBlockSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCidrCollectionResponseTypeDef = TypedDict(
     "CreateCidrCollectionResponseTypeDef",
     {
         "Collection": CidrCollectionTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCloudWatchAlarmConfigurationTypeDef = TypedDict(
     "_RequiredCloudWatchAlarmConfigurationTypeDef",
     {
         "EvaluationPeriods": int,
@@ -1703,15 +1672,15 @@
     pass
 
 ListCidrCollectionsResponseTypeDef = TypedDict(
     "ListCidrCollectionsResponseTypeDef",
     {
         "NextToken": str,
         "CidrCollections": List[CollectionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateHostedZoneRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHostedZoneRequestRequestTypeDef",
     {
         "Name": str,
@@ -1734,209 +1703,228 @@
     pass
 
 CreateReusableDelegationSetResponseTypeDef = TypedDict(
     "CreateReusableDelegationSetResponseTypeDef",
     {
         "DelegationSet": DelegationSetTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReusableDelegationSetResponseTypeDef = TypedDict(
     "GetReusableDelegationSetResponseTypeDef",
     {
         "DelegationSet": DelegationSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReusableDelegationSetsResponseTypeDef = TypedDict(
     "ListReusableDelegationSetsResponseTypeDef",
     {
         "DelegationSets": List[DelegationSetTypeDef],
         "Marker": str,
         "IsTruncated": bool,
         "NextMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVPCAssociationAuthorizationResponseTypeDef = TypedDict(
+    "CreateVPCAssociationAuthorizationResponseTypeDef",
+    {
+        "HostedZoneId": str,
+        "VPC": VPCOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListVPCAssociationAuthorizationsResponseTypeDef = TypedDict(
+    "ListVPCAssociationAuthorizationsResponseTypeDef",
+    {
+        "HostedZoneId": str,
+        "NextToken": str,
+        "VPCs": List[VPCOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateKeySigningKeyResponseTypeDef = TypedDict(
     "CreateKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
         "KeySigningKey": KeySigningKeyTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateQueryLoggingConfigResponseTypeDef = TypedDict(
     "CreateQueryLoggingConfigResponseTypeDef",
     {
         "QueryLoggingConfig": QueryLoggingConfigTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueryLoggingConfigResponseTypeDef = TypedDict(
     "GetQueryLoggingConfigResponseTypeDef",
     {
         "QueryLoggingConfig": QueryLoggingConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQueryLoggingConfigsResponseTypeDef = TypedDict(
     "ListQueryLoggingConfigsResponseTypeDef",
     {
         "QueryLoggingConfigs": List[QueryLoggingConfigTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTrafficPolicyInstanceResponseTypeDef = TypedDict(
     "CreateTrafficPolicyInstanceResponseTypeDef",
     {
         "TrafficPolicyInstance": TrafficPolicyInstanceTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTrafficPolicyInstanceResponseTypeDef = TypedDict(
     "GetTrafficPolicyInstanceResponseTypeDef",
     {
         "TrafficPolicyInstance": TrafficPolicyInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrafficPolicyInstancesByHostedZoneResponseTypeDef = TypedDict(
     "ListTrafficPolicyInstancesByHostedZoneResponseTypeDef",
     {
         "TrafficPolicyInstances": List[TrafficPolicyInstanceTypeDef],
         "TrafficPolicyInstanceNameMarker": str,
         "TrafficPolicyInstanceTypeMarker": RRTypeType,
         "IsTruncated": bool,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrafficPolicyInstancesByPolicyResponseTypeDef = TypedDict(
     "ListTrafficPolicyInstancesByPolicyResponseTypeDef",
     {
         "TrafficPolicyInstances": List[TrafficPolicyInstanceTypeDef],
         "HostedZoneIdMarker": str,
         "TrafficPolicyInstanceNameMarker": str,
         "TrafficPolicyInstanceTypeMarker": RRTypeType,
         "IsTruncated": bool,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrafficPolicyInstancesResponseTypeDef = TypedDict(
     "ListTrafficPolicyInstancesResponseTypeDef",
     {
         "TrafficPolicyInstances": List[TrafficPolicyInstanceTypeDef],
         "HostedZoneIdMarker": str,
         "TrafficPolicyInstanceNameMarker": str,
         "TrafficPolicyInstanceTypeMarker": RRTypeType,
         "IsTruncated": bool,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTrafficPolicyInstanceResponseTypeDef = TypedDict(
     "UpdateTrafficPolicyInstanceResponseTypeDef",
     {
         "TrafficPolicyInstance": TrafficPolicyInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTrafficPolicyResponseTypeDef = TypedDict(
     "CreateTrafficPolicyResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTrafficPolicyVersionResponseTypeDef = TypedDict(
     "CreateTrafficPolicyVersionResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTrafficPolicyResponseTypeDef = TypedDict(
     "GetTrafficPolicyResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrafficPolicyVersionsResponseTypeDef = TypedDict(
     "ListTrafficPolicyVersionsResponseTypeDef",
     {
         "TrafficPolicies": List[TrafficPolicyTypeDef],
         "IsTruncated": bool,
         "TrafficPolicyVersionMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTrafficPolicyCommentResponseTypeDef = TypedDict(
     "UpdateTrafficPolicyCommentResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDNSSECResponseTypeDef = TypedDict(
     "GetDNSSECResponseTypeDef",
     {
         "Status": DNSSECStatusTypeDef,
         "KeySigningKeys": List[KeySigningKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGeoLocationResponseTypeDef = TypedDict(
     "GetGeoLocationResponseTypeDef",
     {
         "GeoLocationDetails": GeoLocationDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGeoLocationsResponseTypeDef = TypedDict(
     "ListGeoLocationsResponseTypeDef",
     {
         "GeoLocationDetailsList": List[GeoLocationDetailsTypeDef],
         "IsTruncated": bool,
         "NextContinentCode": str,
         "NextCountryCode": str,
         "NextSubdivisionCode": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetChangeRequestResourceRecordSetsChangedWaitTypeDef = TypedDict(
     "_RequiredGetChangeRequestResourceRecordSetsChangedWaitTypeDef",
     {
         "Id": str,
@@ -1957,24 +1945,24 @@
     pass
 
 GetHostedZoneLimitResponseTypeDef = TypedDict(
     "GetHostedZoneLimitResponseTypeDef",
     {
         "Limit": HostedZoneLimitTypeDef,
         "Count": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReusableDelegationSetLimitResponseTypeDef = TypedDict(
     "GetReusableDelegationSetLimitResponseTypeDef",
     {
         "Limit": ReusableDelegationSetLimitTypeDef,
         "Count": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HealthCheckObservationTypeDef = TypedDict(
     "HealthCheckObservationTypeDef",
     {
         "Region": HealthCheckRegionType,
@@ -1991,15 +1979,15 @@
         "Name": str,
         "CallerReference": str,
     },
 )
 _OptionalHostedZoneTypeDef = TypedDict(
     "_OptionalHostedZoneTypeDef",
     {
-        "Config": HostedZoneConfigTypeDef,
+        "Config": HostedZoneConfigOutputTypeDef,
         "ResourceRecordSetCount": int,
         "LinkedService": LinkedServiceTypeDef,
     },
     total=False,
 )
 
 class HostedZoneTypeDef(_RequiredHostedZoneTypeDef, _OptionalHostedZoneTypeDef):
@@ -2010,34 +1998,181 @@
     {
         "HostedZoneId": str,
         "Name": str,
         "Owner": HostedZoneOwnerTypeDef,
     },
 )
 
+_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
+    "_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
+    "_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+    {
+        "LocationName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListCidrBlocksRequestListCidrBlocksPaginateTypeDef(
+    _RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+    _OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+):
+    pass
+
+ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef = TypedDict(
+    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
+    "_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
+    "_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListCidrLocationsRequestListCidrLocationsPaginateTypeDef(
+    _RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
+    _OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
+):
+    pass
+
+ListHealthChecksRequestListHealthChecksPaginateTypeDef = TypedDict(
+    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListHostedZonesRequestListHostedZonesPaginateTypeDef = TypedDict(
+    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
+    {
+        "DelegationSetId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef = TypedDict(
+    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
+    {
+        "HostedZoneId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
+    "_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
+    {
+        "HostedZoneId": str,
+    },
+)
+_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
+    "_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef(
+    _RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
+    _OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
+):
+    pass
+
+_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
+    "_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
+    {
+        "HostedZoneId": str,
+    },
+)
+_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
+    "_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
+    {
+        "MaxResults": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef(
+    _RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
+    _OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
+):
+    pass
+
 ListCidrLocationsResponseTypeDef = TypedDict(
     "ListCidrLocationsResponseTypeDef",
     {
         "NextToken": str,
         "CidrLocations": List[LocationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrafficPoliciesResponseTypeDef = TypedDict(
     "ListTrafficPoliciesResponseTypeDef",
     {
         "TrafficPolicySummaries": List[TrafficPolicySummaryTypeDef],
         "IsTruncated": bool,
         "TrafficPolicyIdMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredResourceRecordSetOutputTypeDef = TypedDict(
+    "_RequiredResourceRecordSetOutputTypeDef",
+    {
+        "Name": str,
+        "Type": RRTypeType,
+    },
+)
+_OptionalResourceRecordSetOutputTypeDef = TypedDict(
+    "_OptionalResourceRecordSetOutputTypeDef",
+    {
+        "SetIdentifier": str,
+        "Weight": int,
+        "Region": ResourceRecordSetRegionType,
+        "GeoLocation": GeoLocationOutputTypeDef,
+        "Failover": ResourceRecordSetFailoverType,
+        "MultiValueAnswer": bool,
+        "TTL": int,
+        "ResourceRecords": List[ResourceRecordOutputTypeDef],
+        "AliasTarget": AliasTargetOutputTypeDef,
+        "HealthCheckId": str,
+        "TrafficPolicyInstanceId": str,
+        "CidrRoutingConfig": CidrRoutingConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class ResourceRecordSetOutputTypeDef(
+    _RequiredResourceRecordSetOutputTypeDef, _OptionalResourceRecordSetOutputTypeDef
+):
+    pass
+
 _RequiredResourceRecordSetTypeDef = TypedDict(
     "_RequiredResourceRecordSetTypeDef",
     {
         "Name": str,
         "Type": RRTypeType,
     },
 )
@@ -2061,44 +2196,38 @@
 )
 
 class ResourceRecordSetTypeDef(
     _RequiredResourceRecordSetTypeDef, _OptionalResourceRecordSetTypeDef
 ):
     pass
 
-CreateHealthCheckRequestRequestTypeDef = TypedDict(
-    "CreateHealthCheckRequestRequestTypeDef",
-    {
-        "CallerReference": str,
-        "HealthCheckConfig": HealthCheckConfigTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ResourceTagSetTypeDef = TypedDict(
+    "ResourceTagSetTypeDef",
     {
-        "ResourceTagSet": ResourceTagSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceType": TagResourceTypeType,
+        "ResourceId": str,
+        "Tags": List[TagOutputTypeDef],
     },
+    total=False,
 )
 
-ListTagsForResourcesResponseTypeDef = TypedDict(
-    "ListTagsForResourcesResponseTypeDef",
+CreateHealthCheckRequestRequestTypeDef = TypedDict(
+    "CreateHealthCheckRequestRequestTypeDef",
     {
-        "ResourceTagSets": List[ResourceTagSetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CallerReference": str,
+        "HealthCheckConfig": HealthCheckConfigTypeDef,
     },
 )
 
 _RequiredHealthCheckTypeDef = TypedDict(
     "_RequiredHealthCheckTypeDef",
     {
         "Id": str,
         "CallerReference": str,
-        "HealthCheckConfig": HealthCheckConfigTypeDef,
+        "HealthCheckConfig": HealthCheckConfigOutputTypeDef,
         "HealthCheckVersion": int,
     },
 )
 _OptionalHealthCheckTypeDef = TypedDict(
     "_OptionalHealthCheckTypeDef",
     {
         "LinkedService": LinkedServiceTypeDef,
@@ -2110,147 +2239,163 @@
 class HealthCheckTypeDef(_RequiredHealthCheckTypeDef, _OptionalHealthCheckTypeDef):
     pass
 
 GetHealthCheckLastFailureReasonResponseTypeDef = TypedDict(
     "GetHealthCheckLastFailureReasonResponseTypeDef",
     {
         "HealthCheckObservations": List[HealthCheckObservationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHealthCheckStatusResponseTypeDef = TypedDict(
     "GetHealthCheckStatusResponseTypeDef",
     {
         "HealthCheckObservations": List[HealthCheckObservationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateHostedZoneResponseTypeDef = TypedDict(
     "CreateHostedZoneResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
         "ChangeInfo": ChangeInfoTypeDef,
         "DelegationSet": DelegationSetTypeDef,
-        "VPC": VPCTypeDef,
+        "VPC": VPCOutputTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHostedZoneResponseTypeDef = TypedDict(
     "GetHostedZoneResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
         "DelegationSet": DelegationSetTypeDef,
-        "VPCs": List[VPCTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VPCs": List[VPCOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHostedZonesByNameResponseTypeDef = TypedDict(
     "ListHostedZonesByNameResponseTypeDef",
     {
         "HostedZones": List[HostedZoneTypeDef],
         "DNSName": str,
         "HostedZoneId": str,
         "IsTruncated": bool,
         "NextDNSName": str,
         "NextHostedZoneId": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHostedZonesResponseTypeDef = TypedDict(
     "ListHostedZonesResponseTypeDef",
     {
         "HostedZones": List[HostedZoneTypeDef],
         "Marker": str,
         "IsTruncated": bool,
         "NextMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateHostedZoneCommentResponseTypeDef = TypedDict(
     "UpdateHostedZoneCommentResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHostedZonesByVPCResponseTypeDef = TypedDict(
     "ListHostedZonesByVPCResponseTypeDef",
     {
         "HostedZoneSummaries": List[HostedZoneSummaryTypeDef],
         "MaxItems": str,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListResourceRecordSetsResponseTypeDef = TypedDict(
+    "ListResourceRecordSetsResponseTypeDef",
+    {
+        "ResourceRecordSets": List[ResourceRecordSetOutputTypeDef],
+        "IsTruncated": bool,
+        "NextRecordName": str,
+        "NextRecordType": RRTypeType,
+        "NextRecordIdentifier": str,
+        "MaxItems": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeTypeDef = TypedDict(
     "ChangeTypeDef",
     {
         "Action": ChangeActionType,
         "ResourceRecordSet": ResourceRecordSetTypeDef,
     },
 )
 
-ListResourceRecordSetsResponseTypeDef = TypedDict(
-    "ListResourceRecordSetsResponseTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ResourceRecordSets": List[ResourceRecordSetTypeDef],
-        "IsTruncated": bool,
-        "NextRecordName": str,
-        "NextRecordType": RRTypeType,
-        "NextRecordIdentifier": str,
-        "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceTagSet": ResourceTagSetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourcesResponseTypeDef = TypedDict(
+    "ListTagsForResourcesResponseTypeDef",
+    {
+        "ResourceTagSets": List[ResourceTagSetTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateHealthCheckResponseTypeDef = TypedDict(
     "CreateHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHealthCheckResponseTypeDef = TypedDict(
     "GetHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHealthChecksResponseTypeDef = TypedDict(
     "ListHealthChecksResponseTypeDef",
     {
         "HealthChecks": List[HealthCheckTypeDef],
         "Marker": str,
         "IsTruncated": bool,
         "NextMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateHealthCheckResponseTypeDef = TypedDict(
     "UpdateHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredChangeBatchTypeDef = TypedDict(
     "_RequiredChangeBatchTypeDef",
     {
         "Changes": Sequence[ChangeTypeDef],
```

### Comparing `mypy-boto3-route53-1.28.0/mypy_boto3_route53/waiter.py` & `mypy-boto3-route53-1.28.12/mypy_boto3_route53/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.0/mypy_boto3_route53/waiter.pyi` & `mypy-boto3-route53-1.28.12/mypy_boto3_route53/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.0/mypy_boto3_route53.egg-info/PKG-INFO` & `mypy-boto3-route53-1.28.12/mypy_boto3_route53.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53
-Version: 1.28.0
-Summary: Type annotations for boto3.Route53 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Route53 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-route53"></a>
 
 # mypy-boto3-route53
 
 [![PyPI - mypy-boto3-route53](https://img.shields.io/pypi/v/mypy-boto3-route53.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53?color=blue)](https://pypistats.org/packages/mypy-boto3-route53)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53)](https://pepy.tech/project/mypy-boto3-route53)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
+[boto3.Route53 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
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
 [mypy-boto3-route53 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/).
 
 See how it helps to find and fix potential bugs:
 
@@ -395,28 +395,32 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53.type_defs import (
     AccountLimitTypeDef,
     ActivateKeySigningKeyRequestRequestTypeDef,
     ChangeInfoTypeDef,
+    ResponseMetadataTypeDef,
+    AlarmIdentifierOutputTypeDef,
     AlarmIdentifierTypeDef,
+    AliasTargetOutputTypeDef,
     AliasTargetTypeDef,
     VPCTypeDef,
     CidrCollectionChangeTypeDef,
-    ChangeCidrCollectionResponseTypeDef,
     TagTypeDef,
     CidrBlockSummaryTypeDef,
     CidrCollectionTypeDef,
+    CidrRoutingConfigOutputTypeDef,
     CidrRoutingConfigTypeDef,
     DimensionTypeDef,
     CollectionSummaryTypeDef,
     CreateCidrCollectionRequestRequestTypeDef,
     HostedZoneConfigTypeDef,
     DelegationSetTypeDef,
+    VPCOutputTypeDef,
     CreateKeySigningKeyRequestRequestTypeDef,
     KeySigningKeyTypeDef,
     CreateQueryLoggingConfigRequestRequestTypeDef,
     QueryLoggingConfigTypeDef,
     CreateReusableDelegationSetRequestRequestTypeDef,
     CreateTrafficPolicyInstanceRequestRequestTypeDef,
     TrafficPolicyInstanceTypeDef,
@@ -432,106 +436,102 @@
     DeleteQueryLoggingConfigRequestRequestTypeDef,
     DeleteReusableDelegationSetRequestRequestTypeDef,
     DeleteTrafficPolicyInstanceRequestRequestTypeDef,
     DeleteTrafficPolicyRequestRequestTypeDef,
     DisableHostedZoneDNSSECRequestRequestTypeDef,
     EnableHostedZoneDNSSECRequestRequestTypeDef,
     GeoLocationDetailsTypeDef,
+    GeoLocationOutputTypeDef,
     GeoLocationTypeDef,
     GetAccountLimitRequestRequestTypeDef,
     GetChangeRequestRequestTypeDef,
     WaiterConfigTypeDef,
-    GetCheckerIpRangesResponseTypeDef,
     GetDNSSECRequestRequestTypeDef,
     GetGeoLocationRequestRequestTypeDef,
-    GetHealthCheckCountResponseTypeDef,
     GetHealthCheckLastFailureReasonRequestRequestTypeDef,
     GetHealthCheckRequestRequestTypeDef,
     GetHealthCheckStatusRequestRequestTypeDef,
-    GetHostedZoneCountResponseTypeDef,
     GetHostedZoneLimitRequestRequestTypeDef,
     HostedZoneLimitTypeDef,
     GetHostedZoneRequestRequestTypeDef,
     GetQueryLoggingConfigRequestRequestTypeDef,
     GetReusableDelegationSetLimitRequestRequestTypeDef,
     ReusableDelegationSetLimitTypeDef,
     GetReusableDelegationSetRequestRequestTypeDef,
-    GetTrafficPolicyInstanceCountResponseTypeDef,
     GetTrafficPolicyInstanceRequestRequestTypeDef,
     GetTrafficPolicyRequestRequestTypeDef,
     StatusReportTypeDef,
     LinkedServiceTypeDef,
+    HostedZoneConfigOutputTypeDef,
     HostedZoneOwnerTypeDef,
-    ListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListCidrBlocksRequestRequestTypeDef,
-    ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef,
     ListCidrCollectionsRequestRequestTypeDef,
-    ListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
     ListCidrLocationsRequestRequestTypeDef,
     LocationSummaryTypeDef,
     ListGeoLocationsRequestRequestTypeDef,
-    ListHealthChecksRequestListHealthChecksPaginateTypeDef,
     ListHealthChecksRequestRequestTypeDef,
     ListHostedZonesByNameRequestRequestTypeDef,
     ListHostedZonesByVPCRequestRequestTypeDef,
-    ListHostedZonesRequestListHostedZonesPaginateTypeDef,
     ListHostedZonesRequestRequestTypeDef,
-    ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef,
     ListQueryLoggingConfigsRequestRequestTypeDef,
-    ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
     ListResourceRecordSetsRequestRequestTypeDef,
     ListReusableDelegationSetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourcesRequestRequestTypeDef,
     ListTrafficPoliciesRequestRequestTypeDef,
     TrafficPolicySummaryTypeDef,
     ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef,
     ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef,
     ListTrafficPolicyInstancesRequestRequestTypeDef,
     ListTrafficPolicyVersionsRequestRequestTypeDef,
-    ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
     ListVPCAssociationAuthorizationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ResourceRecordOutputTypeDef,
     ResourceRecordTypeDef,
-    ResponseMetadataTypeDef,
+    TagOutputTypeDef,
     TestDNSAnswerRequestRequestTypeDef,
-    TestDNSAnswerResponseTypeDef,
     UpdateHostedZoneCommentRequestRequestTypeDef,
     UpdateTrafficPolicyCommentRequestRequestTypeDef,
     UpdateTrafficPolicyInstanceRequestRequestTypeDef,
-    GetAccountLimitResponseTypeDef,
     ActivateKeySigningKeyResponseTypeDef,
     AssociateVPCWithHostedZoneResponseTypeDef,
+    ChangeCidrCollectionResponseTypeDef,
     ChangeResourceRecordSetsResponseTypeDef,
     DeactivateKeySigningKeyResponseTypeDef,
     DeleteHostedZoneResponseTypeDef,
     DeleteKeySigningKeyResponseTypeDef,
     DisableHostedZoneDNSSECResponseTypeDef,
     DisassociateVPCFromHostedZoneResponseTypeDef,
     EnableHostedZoneDNSSECResponseTypeDef,
+    GetAccountLimitResponseTypeDef,
     GetChangeResponseTypeDef,
+    GetCheckerIpRangesResponseTypeDef,
+    GetHealthCheckCountResponseTypeDef,
+    GetHostedZoneCountResponseTypeDef,
+    GetTrafficPolicyInstanceCountResponseTypeDef,
+    TestDNSAnswerResponseTypeDef,
+    HealthCheckConfigOutputTypeDef,
     HealthCheckConfigTypeDef,
     UpdateHealthCheckRequestRequestTypeDef,
     AssociateVPCWithHostedZoneRequestRequestTypeDef,
     CreateVPCAssociationAuthorizationRequestRequestTypeDef,
-    CreateVPCAssociationAuthorizationResponseTypeDef,
     DeleteVPCAssociationAuthorizationRequestRequestTypeDef,
     DisassociateVPCFromHostedZoneRequestRequestTypeDef,
-    ListVPCAssociationAuthorizationsResponseTypeDef,
     ChangeCidrCollectionRequestRequestTypeDef,
     ChangeTagsForResourceRequestRequestTypeDef,
-    ResourceTagSetTypeDef,
     ListCidrBlocksResponseTypeDef,
     CreateCidrCollectionResponseTypeDef,
     CloudWatchAlarmConfigurationTypeDef,
     ListCidrCollectionsResponseTypeDef,
     CreateHostedZoneRequestRequestTypeDef,
     CreateReusableDelegationSetResponseTypeDef,
     GetReusableDelegationSetResponseTypeDef,
     ListReusableDelegationSetsResponseTypeDef,
+    CreateVPCAssociationAuthorizationResponseTypeDef,
+    ListVPCAssociationAuthorizationsResponseTypeDef,
     CreateKeySigningKeyResponseTypeDef,
     CreateQueryLoggingConfigResponseTypeDef,
     GetQueryLoggingConfigResponseTypeDef,
     ListQueryLoggingConfigsResponseTypeDef,
     CreateTrafficPolicyInstanceResponseTypeDef,
     GetTrafficPolicyInstanceResponseTypeDef,
     ListTrafficPolicyInstancesByHostedZoneResponseTypeDef,
@@ -548,31 +548,41 @@
     ListGeoLocationsResponseTypeDef,
     GetChangeRequestResourceRecordSetsChangedWaitTypeDef,
     GetHostedZoneLimitResponseTypeDef,
     GetReusableDelegationSetLimitResponseTypeDef,
     HealthCheckObservationTypeDef,
     HostedZoneTypeDef,
     HostedZoneSummaryTypeDef,
+    ListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+    ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef,
+    ListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
+    ListHealthChecksRequestListHealthChecksPaginateTypeDef,
+    ListHostedZonesRequestListHostedZonesPaginateTypeDef,
+    ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef,
+    ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
+    ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
     ListCidrLocationsResponseTypeDef,
     ListTrafficPoliciesResponseTypeDef,
+    ResourceRecordSetOutputTypeDef,
     ResourceRecordSetTypeDef,
+    ResourceTagSetTypeDef,
     CreateHealthCheckRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTagsForResourcesResponseTypeDef,
     HealthCheckTypeDef,
     GetHealthCheckLastFailureReasonResponseTypeDef,
     GetHealthCheckStatusResponseTypeDef,
     CreateHostedZoneResponseTypeDef,
     GetHostedZoneResponseTypeDef,
     ListHostedZonesByNameResponseTypeDef,
     ListHostedZonesResponseTypeDef,
     UpdateHostedZoneCommentResponseTypeDef,
     ListHostedZonesByVPCResponseTypeDef,
-    ChangeTypeDef,
     ListResourceRecordSetsResponseTypeDef,
+    ChangeTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTagsForResourcesResponseTypeDef,
     CreateHealthCheckResponseTypeDef,
     GetHealthCheckResponseTypeDef,
     ListHealthChecksResponseTypeDef,
     UpdateHealthCheckResponseTypeDef,
     ChangeBatchTypeDef,
     ChangeResourceRecordSetsRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-route53-1.28.0/mypy_boto3_route53.egg-info/SOURCES.txt` & `mypy-boto3-route53-1.28.12/mypy_boto3_route53.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.0/setup.py` & `mypy-boto3-route53-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_route53"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Route53 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Route53 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

