# Comparing `tmp/mypy-boto3-ds-1.28.0.tar.gz` & `tmp/mypy-boto3-ds-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ds-1.28.0.tar", last modified: Thu Jul  6 20:59:26 2023, max compression
+gzip compressed data, was "mypy-boto3-ds-1.28.12.tar", last modified: Thu Jul 27 05:34:35 2023, max compression
```

## Comparing `mypy-boto3-ds-1.28.0.tar` & `mypy-boto3-ds-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:26.502283 mypy-boto3-ds-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:38:17.000000 mypy-boto3-ds-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22066 2023-07-06 20:59:26.502283 mypy-boto3-ds-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20587 2023-07-06 20:38:17.000000 mypy-boto3-ds-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:26.502283 mypy-boto3-ds-1.28.0/mypy_boto3_ds/
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-06 20:38:17.000000 mypy-boto3-ds-1.28.0/mypy_boto3_ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-06 20:38:17.000000 mypy-boto3-ds-1.28.0/mypy_boto3_ds/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 20:38:17.000000 mypy-boto3-ds-1.28.0/mypy_boto3_ds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51628 2023-07-06 20:38:18.000000 mypy-boto3-ds-1.28.0/mypy_boto3_ds/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51540 2023-07-06 20:38:18.000000 mypy-boto3-ds-1.28.0/mypy_boto3_ds/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13608 2023-07-06 20:38:19.000000 mypy-boto3-ds-1.28.0/mypy_boto3_ds/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13606 2023-07-06 20:38:18.000000 mypy-boto3-ds-1.28.0/mypy_boto3_ds/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17026 2023-07-06 20:38:18.000000 mypy-boto3-ds-1.28.0/mypy_boto3_ds/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17009 2023-07-06 20:38:18.000000 mypy-boto3-ds-1.28.0/mypy_boto3_ds/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:38:17.000000 mypy-boto3-ds-1.28.0/mypy_boto3_ds/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57733 2023-07-06 20:38:21.000000 mypy-boto3-ds-1.28.0/mypy_boto3_ds/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57660 2023-07-06 20:38:21.000000 mypy-boto3-ds-1.28.0/mypy_boto3_ds/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:38:17.000000 mypy-boto3-ds-1.28.0/mypy_boto3_ds/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:26.502283 mypy-boto3-ds-1.28.0/mypy_boto3_ds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22066 2023-07-06 20:59:26.000000 mypy-boto3-ds-1.28.0/mypy_boto3_ds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-06 20:59:26.000000 mypy-boto3-ds-1.28.0/mypy_boto3_ds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:26.000000 mypy-boto3-ds-1.28.0/mypy_boto3_ds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:26.000000 mypy-boto3-ds-1.28.0/mypy_boto3_ds.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:26.000000 mypy-boto3-ds-1.28.0/mypy_boto3_ds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 20:59:26.000000 mypy-boto3-ds-1.28.0/mypy_boto3_ds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:26.502283 mypy-boto3-ds-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-06 20:38:17.000000 mypy-boto3-ds-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:35.860529 mypy-boto3-ds-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22251 2023-07-27 05:34:35.856529 mypy-boto3-ds-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20770 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:35.856529 mypy-boto3-ds-1.28.12/mypy_boto3_ds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51628 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51540 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17026 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17009 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59090 2023-07-27 05:20:33.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59017 2023-07-27 05:20:33.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:32.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:35.856529 mypy-boto3-ds-1.28.12/mypy_boto3_ds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22251 2023-07-27 05:34:35.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-27 05:34:35.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:35.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:35.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:35.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 05:34:35.000000 mypy-boto3-ds-1.28.12/mypy_boto3_ds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:35.860529 mypy-boto3-ds-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-27 05:20:31.000000 mypy-boto3-ds-1.28.12/setup.py
```

### Comparing `mypy-boto3-ds-1.28.0/LICENSE` & `mypy-boto3-ds-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.0/PKG-INFO` & `mypy-boto3-ds-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ds
-Version: 1.28.0
-Summary: Type annotations for boto3.DirectoryService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.DirectoryService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ds"></a>
 
 # mypy-boto3-ds
 
 [![PyPI - mypy-boto3-ds](https://img.shields.io/pypi/v/mypy-boto3-ds.svg?color=blue)](https://pypi.org/project/mypy-boto3-ds)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ds.svg?color=blue)](https://pypi.org/project/mypy-boto3-ds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ds?color=blue)](https://pypistats.org/packages/mypy-boto3-ds)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ds)](https://pepy.tech/project/mypy-boto3-ds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DirectoryService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
+[boto3.DirectoryService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
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
 [mypy-boto3-ds docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/).
 
 See how it helps to find and fix potential bugs:
 
@@ -414,19 +414,21 @@
 ```python
 from mypy_boto3_ds.type_defs import (
     AcceptSharedDirectoryRequestRequestTypeDef,
     SharedDirectoryTypeDef,
     IpRouteTypeDef,
     DirectoryVpcSettingsTypeDef,
     TagTypeDef,
+    AttributeOutputTypeDef,
     AttributeTypeDef,
     CancelSchemaExtensionRequestRequestTypeDef,
     CertificateInfoTypeDef,
-    ClientCertAuthSettingsTypeDef,
+    ClientCertAuthSettingsOutputTypeDef,
     ClientAuthenticationSettingInfoTypeDef,
+    ClientCertAuthSettingsTypeDef,
     ConditionalForwarderTypeDef,
     DirectoryConnectSettingsTypeDef,
     ConnectDirectoryResultTypeDef,
     CreateAliasRequestRequestTypeDef,
     CreateAliasResultTypeDef,
     CreateConditionalForwarderRequestRequestTypeDef,
     CreateDirectoryResultTypeDef,
@@ -472,23 +474,25 @@
     DescribeTrustsRequestDescribeTrustsPaginateTypeDef,
     DescribeTrustsRequestRequestTypeDef,
     TrustTypeDef,
     DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
     DescribeUpdateDirectoryRequestRequestTypeDef,
     DirectoryConnectSettingsDescriptionTypeDef,
     DirectoryVpcSettingsDescriptionTypeDef,
-    RadiusSettingsTypeDef,
+    RadiusSettingsOutputTypeDef,
     RegionsInfoTypeDef,
     DirectoryLimitsTypeDef,
+    DirectoryVpcSettingsOutputTypeDef,
     DisableClientAuthenticationRequestRequestTypeDef,
     DisableLDAPSRequestRequestTypeDef,
     DisableRadiusRequestRequestTypeDef,
     DisableSsoRequestRequestTypeDef,
     EnableClientAuthenticationRequestRequestTypeDef,
     EnableLDAPSRequestRequestTypeDef,
+    RadiusSettingsTypeDef,
     EnableSsoRequestRequestTypeDef,
     GetSnapshotLimitsRequestRequestTypeDef,
     SnapshotLimitsTypeDef,
     IpRouteInfoTypeDef,
     ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListCertificatesRequestRequestTypeDef,
     ListIpRoutesRequestListIpRoutesPaginateTypeDef,
@@ -497,14 +501,16 @@
     ListLogSubscriptionsRequestRequestTypeDef,
     LogSubscriptionTypeDef,
     ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
     ListSchemaExtensionsRequestRequestTypeDef,
     SchemaExtensionInfoTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    OSUpdateSettingsOutputTypeDef,
     OSUpdateSettingsTypeDef,
     PaginatorConfigTypeDef,
     RegisterCertificateResultTypeDef,
     RegisterEventTopicRequestRequestTypeDef,
     RejectSharedDirectoryRequestRequestTypeDef,
     RejectSharedDirectoryResultTypeDef,
     RemoveIpRoutesRequestRequestTypeDef,
@@ -527,50 +533,50 @@
     UpdateTrustResultTypeDef,
     VerifyTrustRequestRequestTypeDef,
     VerifyTrustResultTypeDef,
     AcceptSharedDirectoryResultTypeDef,
     DescribeSharedDirectoriesResultTypeDef,
     AddIpRoutesRequestRequestTypeDef,
     AddRegionRequestRequestTypeDef,
-    RegionDescriptionTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
     CreateDirectoryRequestRequestTypeDef,
     CreateMicrosoftADRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     ComputerTypeDef,
     CreateComputerRequestRequestTypeDef,
     ListCertificatesResultTypeDef,
     CertificateTypeDef,
-    RegisterCertificateRequestRequestTypeDef,
     DescribeClientAuthenticationSettingsResultTypeDef,
+    RegisterCertificateRequestRequestTypeDef,
     DescribeConditionalForwardersResultTypeDef,
     ConnectDirectoryRequestRequestTypeDef,
     DescribeDomainControllersResultTypeDef,
     DescribeEventTopicsResultTypeDef,
     DescribeLDAPSSettingsResultTypeDef,
     DescribeSettingsResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeTrustsResultTypeDef,
-    EnableRadiusRequestRequestTypeDef,
     OwnerDirectoryDescriptionTypeDef,
-    UpdateRadiusRequestRequestTypeDef,
     GetDirectoryLimitsResultTypeDef,
+    RegionDescriptionTypeDef,
+    EnableRadiusRequestRequestTypeDef,
+    UpdateRadiusRequestRequestTypeDef,
     GetSnapshotLimitsResultTypeDef,
     ListIpRoutesResultTypeDef,
     ListLogSubscriptionsResultTypeDef,
     ListSchemaExtensionsResultTypeDef,
-    UpdateDirectorySetupRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
     UpdateValueTypeDef,
+    UpdateDirectorySetupRequestRequestTypeDef,
     UpdateSettingsRequestRequestTypeDef,
     ShareDirectoryRequestRequestTypeDef,
     UnshareDirectoryRequestRequestTypeDef,
-    DescribeRegionsResultTypeDef,
     CreateComputerResultTypeDef,
     DescribeCertificateResultTypeDef,
     DirectoryDescriptionTypeDef,
+    DescribeRegionsResultTypeDef,
     UpdateInfoEntryTypeDef,
     DescribeDirectoriesResultTypeDef,
     DescribeUpdateDirectoryResultTypeDef,
 )
 
 
 def get_structure() -> AcceptSharedDirectoryRequestRequestTypeDef:
```

### Comparing `mypy-boto3-ds-1.28.0/README.md` & `mypy-boto3-ds-1.28.12/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ds"></a>
 
 # mypy-boto3-ds
 
 [![PyPI - mypy-boto3-ds](https://img.shields.io/pypi/v/mypy-boto3-ds.svg?color=blue)](https://pypi.org/project/mypy-boto3-ds)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ds.svg?color=blue)](https://pypi.org/project/mypy-boto3-ds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ds?color=blue)](https://pypistats.org/packages/mypy-boto3-ds)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ds)](https://pepy.tech/project/mypy-boto3-ds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DirectoryService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
+[boto3.DirectoryService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
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
 [mypy-boto3-ds docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/).
 
 See how it helps to find and fix potential bugs:
 
@@ -382,19 +382,21 @@
 ```python
 from mypy_boto3_ds.type_defs import (
     AcceptSharedDirectoryRequestRequestTypeDef,
     SharedDirectoryTypeDef,
     IpRouteTypeDef,
     DirectoryVpcSettingsTypeDef,
     TagTypeDef,
+    AttributeOutputTypeDef,
     AttributeTypeDef,
     CancelSchemaExtensionRequestRequestTypeDef,
     CertificateInfoTypeDef,
-    ClientCertAuthSettingsTypeDef,
+    ClientCertAuthSettingsOutputTypeDef,
     ClientAuthenticationSettingInfoTypeDef,
+    ClientCertAuthSettingsTypeDef,
     ConditionalForwarderTypeDef,
     DirectoryConnectSettingsTypeDef,
     ConnectDirectoryResultTypeDef,
     CreateAliasRequestRequestTypeDef,
     CreateAliasResultTypeDef,
     CreateConditionalForwarderRequestRequestTypeDef,
     CreateDirectoryResultTypeDef,
@@ -440,23 +442,25 @@
     DescribeTrustsRequestDescribeTrustsPaginateTypeDef,
     DescribeTrustsRequestRequestTypeDef,
     TrustTypeDef,
     DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
     DescribeUpdateDirectoryRequestRequestTypeDef,
     DirectoryConnectSettingsDescriptionTypeDef,
     DirectoryVpcSettingsDescriptionTypeDef,
-    RadiusSettingsTypeDef,
+    RadiusSettingsOutputTypeDef,
     RegionsInfoTypeDef,
     DirectoryLimitsTypeDef,
+    DirectoryVpcSettingsOutputTypeDef,
     DisableClientAuthenticationRequestRequestTypeDef,
     DisableLDAPSRequestRequestTypeDef,
     DisableRadiusRequestRequestTypeDef,
     DisableSsoRequestRequestTypeDef,
     EnableClientAuthenticationRequestRequestTypeDef,
     EnableLDAPSRequestRequestTypeDef,
+    RadiusSettingsTypeDef,
     EnableSsoRequestRequestTypeDef,
     GetSnapshotLimitsRequestRequestTypeDef,
     SnapshotLimitsTypeDef,
     IpRouteInfoTypeDef,
     ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListCertificatesRequestRequestTypeDef,
     ListIpRoutesRequestListIpRoutesPaginateTypeDef,
@@ -465,14 +469,16 @@
     ListLogSubscriptionsRequestRequestTypeDef,
     LogSubscriptionTypeDef,
     ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
     ListSchemaExtensionsRequestRequestTypeDef,
     SchemaExtensionInfoTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    OSUpdateSettingsOutputTypeDef,
     OSUpdateSettingsTypeDef,
     PaginatorConfigTypeDef,
     RegisterCertificateResultTypeDef,
     RegisterEventTopicRequestRequestTypeDef,
     RejectSharedDirectoryRequestRequestTypeDef,
     RejectSharedDirectoryResultTypeDef,
     RemoveIpRoutesRequestRequestTypeDef,
@@ -495,50 +501,50 @@
     UpdateTrustResultTypeDef,
     VerifyTrustRequestRequestTypeDef,
     VerifyTrustResultTypeDef,
     AcceptSharedDirectoryResultTypeDef,
     DescribeSharedDirectoriesResultTypeDef,
     AddIpRoutesRequestRequestTypeDef,
     AddRegionRequestRequestTypeDef,
-    RegionDescriptionTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
     CreateDirectoryRequestRequestTypeDef,
     CreateMicrosoftADRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     ComputerTypeDef,
     CreateComputerRequestRequestTypeDef,
     ListCertificatesResultTypeDef,
     CertificateTypeDef,
-    RegisterCertificateRequestRequestTypeDef,
     DescribeClientAuthenticationSettingsResultTypeDef,
+    RegisterCertificateRequestRequestTypeDef,
     DescribeConditionalForwardersResultTypeDef,
     ConnectDirectoryRequestRequestTypeDef,
     DescribeDomainControllersResultTypeDef,
     DescribeEventTopicsResultTypeDef,
     DescribeLDAPSSettingsResultTypeDef,
     DescribeSettingsResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeTrustsResultTypeDef,
-    EnableRadiusRequestRequestTypeDef,
     OwnerDirectoryDescriptionTypeDef,
-    UpdateRadiusRequestRequestTypeDef,
     GetDirectoryLimitsResultTypeDef,
+    RegionDescriptionTypeDef,
+    EnableRadiusRequestRequestTypeDef,
+    UpdateRadiusRequestRequestTypeDef,
     GetSnapshotLimitsResultTypeDef,
     ListIpRoutesResultTypeDef,
     ListLogSubscriptionsResultTypeDef,
     ListSchemaExtensionsResultTypeDef,
-    UpdateDirectorySetupRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
     UpdateValueTypeDef,
+    UpdateDirectorySetupRequestRequestTypeDef,
     UpdateSettingsRequestRequestTypeDef,
     ShareDirectoryRequestRequestTypeDef,
     UnshareDirectoryRequestRequestTypeDef,
-    DescribeRegionsResultTypeDef,
     CreateComputerResultTypeDef,
     DescribeCertificateResultTypeDef,
     DirectoryDescriptionTypeDef,
+    DescribeRegionsResultTypeDef,
     UpdateInfoEntryTypeDef,
     DescribeDirectoriesResultTypeDef,
     DescribeUpdateDirectoryResultTypeDef,
 )
 
 
 def get_structure() -> AcceptSharedDirectoryRequestRequestTypeDef:
```

### Comparing `mypy-boto3-ds-1.28.0/mypy_boto3_ds/__init__.py` & `mypy-boto3-ds-1.28.12/mypy_boto3_ds/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.0/mypy_boto3_ds/__init__.pyi` & `mypy-boto3-ds-1.28.12/mypy_boto3_ds/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.0/mypy_boto3_ds/client.py` & `mypy-boto3-ds-1.28.12/mypy_boto3_ds/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.0/mypy_boto3_ds/client.pyi` & `mypy-boto3-ds-1.28.12/mypy_boto3_ds/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.0/mypy_boto3_ds/literals.py` & `mypy-boto3-ds-1.28.12/mypy_boto3_ds/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,14 +291,15 @@
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
@@ -377,26 +378,28 @@
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

### Comparing `mypy-boto3-ds-1.28.0/mypy_boto3_ds/literals.pyi` & `mypy-boto3-ds-1.28.12/mypy_boto3_ds/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -289,14 +289,15 @@
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
@@ -375,26 +376,28 @@
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

### Comparing `mypy-boto3-ds-1.28.0/mypy_boto3_ds/paginator.py` & `mypy-boto3-ds-1.28.12/mypy_boto3_ds/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.0/mypy_boto3_ds/paginator.pyi` & `mypy-boto3-ds-1.28.12/mypy_boto3_ds/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.0/mypy_boto3_ds/type_defs.py` & `mypy-boto3-ds-1.28.12/mypy_boto3_ds/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -50,26 +50,27 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptSharedDirectoryRequestRequestTypeDef",
     "SharedDirectoryTypeDef",
     "IpRouteTypeDef",
     "DirectoryVpcSettingsTypeDef",
     "TagTypeDef",
+    "AttributeOutputTypeDef",
     "AttributeTypeDef",
     "CancelSchemaExtensionRequestRequestTypeDef",
     "CertificateInfoTypeDef",
-    "ClientCertAuthSettingsTypeDef",
+    "ClientCertAuthSettingsOutputTypeDef",
     "ClientAuthenticationSettingInfoTypeDef",
+    "ClientCertAuthSettingsTypeDef",
     "ConditionalForwarderTypeDef",
     "DirectoryConnectSettingsTypeDef",
     "ConnectDirectoryResultTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "CreateAliasResultTypeDef",
     "CreateConditionalForwarderRequestRequestTypeDef",
     "CreateDirectoryResultTypeDef",
@@ -115,23 +116,25 @@
     "DescribeTrustsRequestDescribeTrustsPaginateTypeDef",
     "DescribeTrustsRequestRequestTypeDef",
     "TrustTypeDef",
     "DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
     "DescribeUpdateDirectoryRequestRequestTypeDef",
     "DirectoryConnectSettingsDescriptionTypeDef",
     "DirectoryVpcSettingsDescriptionTypeDef",
-    "RadiusSettingsTypeDef",
+    "RadiusSettingsOutputTypeDef",
     "RegionsInfoTypeDef",
     "DirectoryLimitsTypeDef",
+    "DirectoryVpcSettingsOutputTypeDef",
     "DisableClientAuthenticationRequestRequestTypeDef",
     "DisableLDAPSRequestRequestTypeDef",
     "DisableRadiusRequestRequestTypeDef",
     "DisableSsoRequestRequestTypeDef",
     "EnableClientAuthenticationRequestRequestTypeDef",
     "EnableLDAPSRequestRequestTypeDef",
+    "RadiusSettingsTypeDef",
     "EnableSsoRequestRequestTypeDef",
     "GetSnapshotLimitsRequestRequestTypeDef",
     "SnapshotLimitsTypeDef",
     "IpRouteInfoTypeDef",
     "ListCertificatesRequestListCertificatesPaginateTypeDef",
     "ListCertificatesRequestRequestTypeDef",
     "ListIpRoutesRequestListIpRoutesPaginateTypeDef",
@@ -140,14 +143,16 @@
     "ListLogSubscriptionsRequestRequestTypeDef",
     "LogSubscriptionTypeDef",
     "ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
     "ListSchemaExtensionsRequestRequestTypeDef",
     "SchemaExtensionInfoTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "OSUpdateSettingsOutputTypeDef",
     "OSUpdateSettingsTypeDef",
     "PaginatorConfigTypeDef",
     "RegisterCertificateResultTypeDef",
     "RegisterEventTopicRequestRequestTypeDef",
     "RejectSharedDirectoryRequestRequestTypeDef",
     "RejectSharedDirectoryResultTypeDef",
     "RemoveIpRoutesRequestRequestTypeDef",
@@ -170,50 +175,50 @@
     "UpdateTrustResultTypeDef",
     "VerifyTrustRequestRequestTypeDef",
     "VerifyTrustResultTypeDef",
     "AcceptSharedDirectoryResultTypeDef",
     "DescribeSharedDirectoriesResultTypeDef",
     "AddIpRoutesRequestRequestTypeDef",
     "AddRegionRequestRequestTypeDef",
-    "RegionDescriptionTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
     "CreateDirectoryRequestRequestTypeDef",
     "CreateMicrosoftADRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "ComputerTypeDef",
     "CreateComputerRequestRequestTypeDef",
     "ListCertificatesResultTypeDef",
     "CertificateTypeDef",
-    "RegisterCertificateRequestRequestTypeDef",
     "DescribeClientAuthenticationSettingsResultTypeDef",
+    "RegisterCertificateRequestRequestTypeDef",
     "DescribeConditionalForwardersResultTypeDef",
     "ConnectDirectoryRequestRequestTypeDef",
     "DescribeDomainControllersResultTypeDef",
     "DescribeEventTopicsResultTypeDef",
     "DescribeLDAPSSettingsResultTypeDef",
     "DescribeSettingsResultTypeDef",
     "DescribeSnapshotsResultTypeDef",
     "DescribeTrustsResultTypeDef",
-    "EnableRadiusRequestRequestTypeDef",
     "OwnerDirectoryDescriptionTypeDef",
-    "UpdateRadiusRequestRequestTypeDef",
     "GetDirectoryLimitsResultTypeDef",
+    "RegionDescriptionTypeDef",
+    "EnableRadiusRequestRequestTypeDef",
+    "UpdateRadiusRequestRequestTypeDef",
     "GetSnapshotLimitsResultTypeDef",
     "ListIpRoutesResultTypeDef",
     "ListLogSubscriptionsResultTypeDef",
     "ListSchemaExtensionsResultTypeDef",
-    "UpdateDirectorySetupRequestRequestTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "UpdateValueTypeDef",
+    "UpdateDirectorySetupRequestRequestTypeDef",
     "UpdateSettingsRequestRequestTypeDef",
     "ShareDirectoryRequestRequestTypeDef",
     "UnshareDirectoryRequestRequestTypeDef",
-    "DescribeRegionsResultTypeDef",
     "CreateComputerResultTypeDef",
     "DescribeCertificateResultTypeDef",
     "DirectoryDescriptionTypeDef",
+    "DescribeRegionsResultTypeDef",
     "UpdateInfoEntryTypeDef",
     "DescribeDirectoriesResultTypeDef",
     "DescribeUpdateDirectoryResultTypeDef",
 )
 
 AcceptSharedDirectoryRequestRequestTypeDef = TypedDict(
     "AcceptSharedDirectoryRequestRequestTypeDef",
@@ -259,14 +264,23 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+AttributeOutputTypeDef = TypedDict(
+    "AttributeOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 AttributeTypeDef = TypedDict(
     "AttributeTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
@@ -288,16 +302,16 @@
         "State": CertificateStateType,
         "ExpiryDateTime": datetime,
         "Type": CertificateTypeType,
     },
     total=False,
 )
 
-ClientCertAuthSettingsTypeDef = TypedDict(
-    "ClientCertAuthSettingsTypeDef",
+ClientCertAuthSettingsOutputTypeDef = TypedDict(
+    "ClientCertAuthSettingsOutputTypeDef",
     {
         "OCSPUrl": str,
     },
     total=False,
 )
 
 ClientAuthenticationSettingInfoTypeDef = TypedDict(
@@ -306,14 +320,22 @@
         "Type": ClientAuthenticationTypeType,
         "Status": ClientAuthenticationStatusType,
         "LastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
+ClientCertAuthSettingsTypeDef = TypedDict(
+    "ClientCertAuthSettingsTypeDef",
+    {
+        "OCSPUrl": str,
+    },
+    total=False,
+)
+
 ConditionalForwarderTypeDef = TypedDict(
     "ConditionalForwarderTypeDef",
     {
         "RemoteDomainName": str,
         "DnsIpAddrs": List[str],
         "ReplicationScope": Literal["Domain"],
     },
@@ -398,21 +420,19 @@
     "_OptionalCreateSnapshotRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class CreateSnapshotRequestRequestTypeDef(
     _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
 ):
     pass
 
-
 CreateSnapshotResultTypeDef = TypedDict(
     "CreateSnapshotResultTypeDef",
     {
         "SnapshotId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -432,21 +452,19 @@
         "TrustType": TrustTypeType,
         "ConditionalForwarderIpAddrs": Sequence[str],
         "SelectiveAuth": SelectiveAuthType,
     },
     total=False,
 )
 
-
 class CreateTrustRequestRequestTypeDef(
     _RequiredCreateTrustRequestRequestTypeDef, _OptionalCreateTrustRequestRequestTypeDef
 ):
     pass
 
-
 CreateTrustResultTypeDef = TypedDict(
     "CreateTrustResultTypeDef",
     {
         "TrustId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -506,21 +524,19 @@
     "_OptionalDeleteTrustRequestRequestTypeDef",
     {
         "DeleteAssociatedConditionalForwarder": bool,
     },
     total=False,
 )
 
-
 class DeleteTrustRequestRequestTypeDef(
     _RequiredDeleteTrustRequestRequestTypeDef, _OptionalDeleteTrustRequestRequestTypeDef
 ):
     pass
 
-
 DeleteTrustResultTypeDef = TypedDict(
     "DeleteTrustResultTypeDef",
     {
         "TrustId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -560,22 +576,20 @@
     {
         "Type": ClientAuthenticationTypeType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef(
     _RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
     _OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeClientAuthenticationSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeClientAuthenticationSettingsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeClientAuthenticationSettingsRequestRequestTypeDef = TypedDict(
@@ -584,44 +598,40 @@
         "Type": ClientAuthenticationTypeType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class DescribeClientAuthenticationSettingsRequestRequestTypeDef(
     _RequiredDescribeClientAuthenticationSettingsRequestRequestTypeDef,
     _OptionalDescribeClientAuthenticationSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeConditionalForwardersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConditionalForwardersRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeConditionalForwardersRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeConditionalForwardersRequestRequestTypeDef",
     {
         "RemoteDomainNames": Sequence[str],
     },
     total=False,
 )
 
-
 class DescribeConditionalForwardersRequestRequestTypeDef(
     _RequiredDescribeConditionalForwardersRequestRequestTypeDef,
     _OptionalDescribeConditionalForwardersRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef = TypedDict(
     "DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef",
     {
         "DirectoryIds": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -648,22 +658,20 @@
     {
         "DomainControllerIds": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef(
     _RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
     _OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeDomainControllersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDomainControllersRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeDomainControllersRequestRequestTypeDef = TypedDict(
@@ -672,22 +680,20 @@
         "DomainControllerIds": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class DescribeDomainControllersRequestRequestTypeDef(
     _RequiredDescribeDomainControllersRequestRequestTypeDef,
     _OptionalDescribeDomainControllersRequestRequestTypeDef,
 ):
     pass
 
-
 DomainControllerTypeDef = TypedDict(
     "DomainControllerTypeDef",
     {
         "DirectoryId": str,
         "DomainControllerId": str,
         "DnsIpAddr": str,
         "VpcId": str,
@@ -733,22 +739,20 @@
     {
         "Type": Literal["Client"],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef(
     _RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
     _OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeLDAPSSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeLDAPSSettingsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeLDAPSSettingsRequestRequestTypeDef = TypedDict(
@@ -757,22 +761,20 @@
         "Type": Literal["Client"],
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class DescribeLDAPSSettingsRequestRequestTypeDef(
     _RequiredDescribeLDAPSSettingsRequestRequestTypeDef,
     _OptionalDescribeLDAPSSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 LDAPSSettingInfoTypeDef = TypedDict(
     "LDAPSSettingInfoTypeDef",
     {
         "LDAPSStatus": LDAPSStatusType,
         "LDAPSStatusReason": str,
         "LastUpdatedDateTime": datetime,
     },
@@ -790,22 +792,20 @@
     {
         "RegionName": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeRegionsRequestDescribeRegionsPaginateTypeDef(
     _RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef,
     _OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeRegionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRegionsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeRegionsRequestRequestTypeDef = TypedDict(
@@ -813,21 +813,19 @@
     {
         "RegionName": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeRegionsRequestRequestTypeDef(
     _RequiredDescribeRegionsRequestRequestTypeDef, _OptionalDescribeRegionsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSettingsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeSettingsRequestRequestTypeDef = TypedDict(
@@ -835,21 +833,19 @@
     {
         "Status": DirectoryConfigurationStatusType,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeSettingsRequestRequestTypeDef(
     _RequiredDescribeSettingsRequestRequestTypeDef, _OptionalDescribeSettingsRequestRequestTypeDef
 ):
     pass
 
-
 SettingEntryTypeDef = TypedDict(
     "SettingEntryTypeDef",
     {
         "Type": str,
         "Name": str,
         "AllowedValues": str,
         "AppliedValue": str,
@@ -875,22 +871,20 @@
     {
         "SharedDirectoryIds": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef(
     _RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
     _OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeSharedDirectoriesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSharedDirectoriesRequestRequestTypeDef",
     {
         "OwnerDirectoryId": str,
     },
 )
 _OptionalDescribeSharedDirectoriesRequestRequestTypeDef = TypedDict(
@@ -899,22 +893,20 @@
         "SharedDirectoryIds": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class DescribeSharedDirectoriesRequestRequestTypeDef(
     _RequiredDescribeSharedDirectoriesRequestRequestTypeDef,
     _OptionalDescribeSharedDirectoriesRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef = TypedDict(
     "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
     {
         "DirectoryId": str,
         "SnapshotIds": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -996,22 +988,20 @@
     {
         "RegionName": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef(
     _RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
     _OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeUpdateDirectoryRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeUpdateDirectoryRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "UpdateType": Literal["OS"],
     },
 )
@@ -1020,22 +1010,20 @@
     {
         "RegionName": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeUpdateDirectoryRequestRequestTypeDef(
     _RequiredDescribeUpdateDirectoryRequestRequestTypeDef,
     _OptionalDescribeUpdateDirectoryRequestRequestTypeDef,
 ):
     pass
 
-
 DirectoryConnectSettingsDescriptionTypeDef = TypedDict(
     "DirectoryConnectSettingsDescriptionTypeDef",
     {
         "VpcId": str,
         "SubnetIds": List[str],
         "CustomerUserName": str,
         "SecurityGroupId": str,
@@ -1052,16 +1040,16 @@
         "SubnetIds": List[str],
         "SecurityGroupId": str,
         "AvailabilityZones": List[str],
     },
     total=False,
 )
 
-RadiusSettingsTypeDef = TypedDict(
-    "RadiusSettingsTypeDef",
+RadiusSettingsOutputTypeDef = TypedDict(
+    "RadiusSettingsOutputTypeDef",
     {
         "RadiusServers": List[str],
         "RadiusPort": int,
         "RadiusTimeout": int,
         "RadiusRetries": int,
         "SharedSecret": str,
         "AuthenticationProtocol": RadiusAuthenticationProtocolType,
@@ -1092,14 +1080,22 @@
         "ConnectedDirectoriesLimit": int,
         "ConnectedDirectoriesCurrentCount": int,
         "ConnectedDirectoriesLimitReached": bool,
     },
     total=False,
 )
 
+DirectoryVpcSettingsOutputTypeDef = TypedDict(
+    "DirectoryVpcSettingsOutputTypeDef",
+    {
+        "VpcId": str,
+        "SubnetIds": List[str],
+    },
+)
+
 DisableClientAuthenticationRequestRequestTypeDef = TypedDict(
     "DisableClientAuthenticationRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Type": ClientAuthenticationTypeType,
     },
 )
@@ -1130,21 +1126,19 @@
     {
         "UserName": str,
         "Password": str,
     },
     total=False,
 )
 
-
 class DisableSsoRequestRequestTypeDef(
     _RequiredDisableSsoRequestRequestTypeDef, _OptionalDisableSsoRequestRequestTypeDef
 ):
     pass
 
-
 EnableClientAuthenticationRequestRequestTypeDef = TypedDict(
     "EnableClientAuthenticationRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Type": ClientAuthenticationTypeType,
     },
 )
@@ -1153,14 +1147,29 @@
     "EnableLDAPSRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Type": Literal["Client"],
     },
 )
 
+RadiusSettingsTypeDef = TypedDict(
+    "RadiusSettingsTypeDef",
+    {
+        "RadiusServers": Sequence[str],
+        "RadiusPort": int,
+        "RadiusTimeout": int,
+        "RadiusRetries": int,
+        "SharedSecret": str,
+        "AuthenticationProtocol": RadiusAuthenticationProtocolType,
+        "DisplayLabel": str,
+        "UseSameUsername": bool,
+    },
+    total=False,
+)
+
 _RequiredEnableSsoRequestRequestTypeDef = TypedDict(
     "_RequiredEnableSsoRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalEnableSsoRequestRequestTypeDef = TypedDict(
@@ -1168,21 +1177,19 @@
     {
         "UserName": str,
         "Password": str,
     },
     total=False,
 )
 
-
 class EnableSsoRequestRequestTypeDef(
     _RequiredEnableSsoRequestRequestTypeDef, _OptionalEnableSsoRequestRequestTypeDef
 ):
     pass
 
-
 GetSnapshotLimitsRequestRequestTypeDef = TypedDict(
     "GetSnapshotLimitsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 
@@ -1219,22 +1226,20 @@
     "_OptionalListCertificatesRequestListCertificatesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListCertificatesRequestListCertificatesPaginateTypeDef(
     _RequiredListCertificatesRequestListCertificatesPaginateTypeDef,
     _OptionalListCertificatesRequestListCertificatesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListCertificatesRequestRequestTypeDef = TypedDict(
     "_RequiredListCertificatesRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalListCertificatesRequestRequestTypeDef = TypedDict(
@@ -1242,43 +1247,39 @@
     {
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class ListCertificatesRequestRequestTypeDef(
     _RequiredListCertificatesRequestRequestTypeDef, _OptionalListCertificatesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef = TypedDict(
     "_RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef = TypedDict(
     "_OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListIpRoutesRequestListIpRoutesPaginateTypeDef(
     _RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef,
     _OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListIpRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredListIpRoutesRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalListIpRoutesRequestRequestTypeDef = TypedDict(
@@ -1286,21 +1287,19 @@
     {
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class ListIpRoutesRequestRequestTypeDef(
     _RequiredListIpRoutesRequestRequestTypeDef, _OptionalListIpRoutesRequestRequestTypeDef
 ):
     pass
 
-
 ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef = TypedDict(
     "ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef",
     {
         "DirectoryId": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1336,22 +1335,20 @@
     "_OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef(
     _RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
     _OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListSchemaExtensionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemaExtensionsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalListSchemaExtensionsRequestRequestTypeDef = TypedDict(
@@ -1359,22 +1356,20 @@
     {
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class ListSchemaExtensionsRequestRequestTypeDef(
     _RequiredListSchemaExtensionsRequestRequestTypeDef,
     _OptionalListSchemaExtensionsRequestRequestTypeDef,
 ):
     pass
 
-
 SchemaExtensionInfoTypeDef = TypedDict(
     "SchemaExtensionInfoTypeDef",
     {
         "DirectoryId": str,
         "SchemaExtensionId": str,
         "Description": str,
         "SchemaExtensionStatus": SchemaExtensionStatusType,
@@ -1395,22 +1390,20 @@
     "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1418,21 +1411,35 @@
     {
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+OSUpdateSettingsOutputTypeDef = TypedDict(
+    "OSUpdateSettingsOutputTypeDef",
+    {
+        "OSVersion": OSVersionType,
+    },
+    total=False,
+)
 
 OSUpdateSettingsTypeDef = TypedDict(
     "OSUpdateSettingsTypeDef",
     {
         "OSVersion": OSVersionType,
     },
     total=False,
@@ -1622,21 +1629,19 @@
     "_OptionalUpdateTrustRequestRequestTypeDef",
     {
         "SelectiveAuth": SelectiveAuthType,
     },
     total=False,
 )
 
-
 class UpdateTrustRequestRequestTypeDef(
     _RequiredUpdateTrustRequestRequestTypeDef, _OptionalUpdateTrustRequestRequestTypeDef
 ):
     pass
 
-
 UpdateTrustResultTypeDef = TypedDict(
     "UpdateTrustResultTypeDef",
     {
         "RequestId": str,
         "TrustId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1685,46 +1690,28 @@
     "_OptionalAddIpRoutesRequestRequestTypeDef",
     {
         "UpdateSecurityGroupForDirectoryControllers": bool,
     },
     total=False,
 )
 
-
 class AddIpRoutesRequestRequestTypeDef(
     _RequiredAddIpRoutesRequestRequestTypeDef, _OptionalAddIpRoutesRequestRequestTypeDef
 ):
     pass
 
-
 AddRegionRequestRequestTypeDef = TypedDict(
     "AddRegionRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RegionName": str,
         "VPCSettings": DirectoryVpcSettingsTypeDef,
     },
 )
 
-RegionDescriptionTypeDef = TypedDict(
-    "RegionDescriptionTypeDef",
-    {
-        "DirectoryId": str,
-        "RegionName": str,
-        "RegionType": RegionTypeType,
-        "Status": DirectoryStageType,
-        "VpcSettings": DirectoryVpcSettingsTypeDef,
-        "DesiredNumberOfDomainControllers": int,
-        "LaunchTime": datetime,
-        "StatusLastUpdatedDateTime": datetime,
-        "LastUpdatedDateTime": datetime,
-    },
-    total=False,
-)
-
 AddTagsToResourceRequestRequestTypeDef = TypedDict(
     "AddTagsToResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1744,21 +1731,19 @@
         "Description": str,
         "VpcSettings": DirectoryVpcSettingsTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDirectoryRequestRequestTypeDef(
     _RequiredCreateDirectoryRequestRequestTypeDef, _OptionalCreateDirectoryRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateMicrosoftADRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMicrosoftADRequestRequestTypeDef",
     {
         "Name": str,
         "Password": str,
         "VpcSettings": DirectoryVpcSettingsTypeDef,
     },
@@ -1770,36 +1755,25 @@
         "Description": str,
         "Edition": DirectoryEditionType,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMicrosoftADRequestRequestTypeDef(
     _RequiredCreateMicrosoftADRequestRequestTypeDef, _OptionalCreateMicrosoftADRequestRequestTypeDef
 ):
     pass
 
-
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ComputerTypeDef = TypedDict(
     "ComputerTypeDef",
     {
         "ComputerId": str,
         "ComputerName": str,
-        "ComputerAttributes": List[AttributeTypeDef],
+        "ComputerAttributes": List[AttributeOutputTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateComputerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateComputerRequestRequestTypeDef",
     {
@@ -1813,21 +1787,19 @@
     {
         "OrganizationalUnitDistinguishedName": str,
         "ComputerAttributes": Sequence[AttributeTypeDef],
     },
     total=False,
 )
 
-
 class CreateComputerRequestRequestTypeDef(
     _RequiredCreateComputerRequestRequestTypeDef, _OptionalCreateComputerRequestRequestTypeDef
 ):
     pass
 
-
 ListCertificatesResultTypeDef = TypedDict(
     "ListCertificatesResultTypeDef",
     {
         "NextToken": str,
         "CertificatesInfo": List[CertificateInfoTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1839,19 +1811,28 @@
         "CertificateId": str,
         "State": CertificateStateType,
         "StateReason": str,
         "CommonName": str,
         "RegisteredDateTime": datetime,
         "ExpiryDateTime": datetime,
         "Type": CertificateTypeType,
-        "ClientCertAuthSettings": ClientCertAuthSettingsTypeDef,
+        "ClientCertAuthSettings": ClientCertAuthSettingsOutputTypeDef,
     },
     total=False,
 )
 
+DescribeClientAuthenticationSettingsResultTypeDef = TypedDict(
+    "DescribeClientAuthenticationSettingsResultTypeDef",
+    {
+        "ClientAuthenticationSettingsInfo": List[ClientAuthenticationSettingInfoTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRegisterCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterCertificateRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "CertificateData": str,
     },
 )
@@ -1860,31 +1841,20 @@
     {
         "Type": CertificateTypeType,
         "ClientCertAuthSettings": ClientCertAuthSettingsTypeDef,
     },
     total=False,
 )
 
-
 class RegisterCertificateRequestRequestTypeDef(
     _RequiredRegisterCertificateRequestRequestTypeDef,
     _OptionalRegisterCertificateRequestRequestTypeDef,
 ):
     pass
 
-
-DescribeClientAuthenticationSettingsResultTypeDef = TypedDict(
-    "DescribeClientAuthenticationSettingsResultTypeDef",
-    {
-        "ClientAuthenticationSettingsInfo": List[ClientAuthenticationSettingInfoTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeConditionalForwardersResultTypeDef = TypedDict(
     "DescribeConditionalForwardersResultTypeDef",
     {
         "ConditionalForwarders": List[ConditionalForwarderTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1904,21 +1874,19 @@
         "ShortName": str,
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class ConnectDirectoryRequestRequestTypeDef(
     _RequiredConnectDirectoryRequestRequestTypeDef, _OptionalConnectDirectoryRequestRequestTypeDef
 ):
     pass
 
-
 DescribeDomainControllersResultTypeDef = TypedDict(
     "DescribeDomainControllersResultTypeDef",
     {
         "DomainControllers": List[DomainControllerTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1965,48 +1933,64 @@
     {
         "Trusts": List[TrustTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EnableRadiusRequestRequestTypeDef = TypedDict(
-    "EnableRadiusRequestRequestTypeDef",
-    {
-        "DirectoryId": str,
-        "RadiusSettings": RadiusSettingsTypeDef,
-    },
-)
-
 OwnerDirectoryDescriptionTypeDef = TypedDict(
     "OwnerDirectoryDescriptionTypeDef",
     {
         "DirectoryId": str,
         "AccountId": str,
         "DnsIpAddrs": List[str],
         "VpcSettings": DirectoryVpcSettingsDescriptionTypeDef,
-        "RadiusSettings": RadiusSettingsTypeDef,
+        "RadiusSettings": RadiusSettingsOutputTypeDef,
         "RadiusStatus": RadiusStatusType,
     },
     total=False,
 )
 
-UpdateRadiusRequestRequestTypeDef = TypedDict(
-    "UpdateRadiusRequestRequestTypeDef",
+GetDirectoryLimitsResultTypeDef = TypedDict(
+    "GetDirectoryLimitsResultTypeDef",
+    {
+        "DirectoryLimits": DirectoryLimitsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RegionDescriptionTypeDef = TypedDict(
+    "RegionDescriptionTypeDef",
+    {
+        "DirectoryId": str,
+        "RegionName": str,
+        "RegionType": RegionTypeType,
+        "Status": DirectoryStageType,
+        "VpcSettings": DirectoryVpcSettingsOutputTypeDef,
+        "DesiredNumberOfDomainControllers": int,
+        "LaunchTime": datetime,
+        "StatusLastUpdatedDateTime": datetime,
+        "LastUpdatedDateTime": datetime,
+    },
+    total=False,
+)
+
+EnableRadiusRequestRequestTypeDef = TypedDict(
+    "EnableRadiusRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RadiusSettings": RadiusSettingsTypeDef,
     },
 )
 
-GetDirectoryLimitsResultTypeDef = TypedDict(
-    "GetDirectoryLimitsResultTypeDef",
+UpdateRadiusRequestRequestTypeDef = TypedDict(
+    "UpdateRadiusRequestRequestTypeDef",
     {
-        "DirectoryLimits": DirectoryLimitsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DirectoryId": str,
+        "RadiusSettings": RadiusSettingsTypeDef,
     },
 )
 
 GetSnapshotLimitsResultTypeDef = TypedDict(
     "GetSnapshotLimitsResultTypeDef",
     {
         "SnapshotLimits": SnapshotLimitsTypeDef,
@@ -2037,14 +2021,31 @@
     {
         "SchemaExtensionsInfo": List[SchemaExtensionInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateValueTypeDef = TypedDict(
+    "UpdateValueTypeDef",
+    {
+        "OSUpdateSettings": OSUpdateSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateDirectorySetupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDirectorySetupRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "UpdateType": Literal["OS"],
     },
 )
@@ -2053,30 +2054,20 @@
     {
         "OSUpdateSettings": OSUpdateSettingsTypeDef,
         "CreateSnapshotBeforeUpdate": bool,
     },
     total=False,
 )
 
-
 class UpdateDirectorySetupRequestRequestTypeDef(
     _RequiredUpdateDirectorySetupRequestRequestTypeDef,
     _OptionalUpdateDirectorySetupRequestRequestTypeDef,
 ):
     pass
 
-
-UpdateValueTypeDef = TypedDict(
-    "UpdateValueTypeDef",
-    {
-        "OSUpdateSettings": OSUpdateSettingsTypeDef,
-    },
-    total=False,
-)
-
 UpdateSettingsRequestRequestTypeDef = TypedDict(
     "UpdateSettingsRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Settings": Sequence[SettingTypeDef],
     },
 )
@@ -2093,38 +2084,27 @@
     "_OptionalShareDirectoryRequestRequestTypeDef",
     {
         "ShareNotes": str,
     },
     total=False,
 )
 
-
 class ShareDirectoryRequestRequestTypeDef(
     _RequiredShareDirectoryRequestRequestTypeDef, _OptionalShareDirectoryRequestRequestTypeDef
 ):
     pass
 
-
 UnshareDirectoryRequestRequestTypeDef = TypedDict(
     "UnshareDirectoryRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "UnshareTarget": UnshareTargetTypeDef,
     },
 )
 
-DescribeRegionsResultTypeDef = TypedDict(
-    "DescribeRegionsResultTypeDef",
-    {
-        "RegionsDescription": List[RegionDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateComputerResultTypeDef = TypedDict(
     "CreateComputerResultTypeDef",
     {
         "Computer": ComputerTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2154,26 +2134,35 @@
         "ShareMethod": ShareMethodType,
         "ShareNotes": str,
         "LaunchTime": datetime,
         "StageLastUpdatedDateTime": datetime,
         "Type": DirectoryTypeType,
         "VpcSettings": DirectoryVpcSettingsDescriptionTypeDef,
         "ConnectSettings": DirectoryConnectSettingsDescriptionTypeDef,
-        "RadiusSettings": RadiusSettingsTypeDef,
+        "RadiusSettings": RadiusSettingsOutputTypeDef,
         "RadiusStatus": RadiusStatusType,
         "StageReason": str,
         "SsoEnabled": bool,
         "DesiredNumberOfDomainControllers": int,
         "OwnerDirectoryDescription": OwnerDirectoryDescriptionTypeDef,
         "RegionsInfo": RegionsInfoTypeDef,
         "OsVersion": OSVersionType,
     },
     total=False,
 )
 
+DescribeRegionsResultTypeDef = TypedDict(
+    "DescribeRegionsResultTypeDef",
+    {
+        "RegionsDescription": List[RegionDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateInfoEntryTypeDef = TypedDict(
     "UpdateInfoEntryTypeDef",
     {
         "Region": str,
         "Status": UpdateStatusType,
         "StatusReason": str,
         "InitiatedBy": str,
```

### Comparing `mypy-boto3-ds-1.28.0/mypy_boto3_ds/type_defs.pyi` & `mypy-boto3-ds-1.28.12/mypy_boto3_ds/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,25 +50,28 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AcceptSharedDirectoryRequestRequestTypeDef",
     "SharedDirectoryTypeDef",
     "IpRouteTypeDef",
     "DirectoryVpcSettingsTypeDef",
     "TagTypeDef",
+    "AttributeOutputTypeDef",
     "AttributeTypeDef",
     "CancelSchemaExtensionRequestRequestTypeDef",
     "CertificateInfoTypeDef",
-    "ClientCertAuthSettingsTypeDef",
+    "ClientCertAuthSettingsOutputTypeDef",
     "ClientAuthenticationSettingInfoTypeDef",
+    "ClientCertAuthSettingsTypeDef",
     "ConditionalForwarderTypeDef",
     "DirectoryConnectSettingsTypeDef",
     "ConnectDirectoryResultTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "CreateAliasResultTypeDef",
     "CreateConditionalForwarderRequestRequestTypeDef",
     "CreateDirectoryResultTypeDef",
@@ -114,23 +117,25 @@
     "DescribeTrustsRequestDescribeTrustsPaginateTypeDef",
     "DescribeTrustsRequestRequestTypeDef",
     "TrustTypeDef",
     "DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
     "DescribeUpdateDirectoryRequestRequestTypeDef",
     "DirectoryConnectSettingsDescriptionTypeDef",
     "DirectoryVpcSettingsDescriptionTypeDef",
-    "RadiusSettingsTypeDef",
+    "RadiusSettingsOutputTypeDef",
     "RegionsInfoTypeDef",
     "DirectoryLimitsTypeDef",
+    "DirectoryVpcSettingsOutputTypeDef",
     "DisableClientAuthenticationRequestRequestTypeDef",
     "DisableLDAPSRequestRequestTypeDef",
     "DisableRadiusRequestRequestTypeDef",
     "DisableSsoRequestRequestTypeDef",
     "EnableClientAuthenticationRequestRequestTypeDef",
     "EnableLDAPSRequestRequestTypeDef",
+    "RadiusSettingsTypeDef",
     "EnableSsoRequestRequestTypeDef",
     "GetSnapshotLimitsRequestRequestTypeDef",
     "SnapshotLimitsTypeDef",
     "IpRouteInfoTypeDef",
     "ListCertificatesRequestListCertificatesPaginateTypeDef",
     "ListCertificatesRequestRequestTypeDef",
     "ListIpRoutesRequestListIpRoutesPaginateTypeDef",
@@ -139,14 +144,16 @@
     "ListLogSubscriptionsRequestRequestTypeDef",
     "LogSubscriptionTypeDef",
     "ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
     "ListSchemaExtensionsRequestRequestTypeDef",
     "SchemaExtensionInfoTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "OSUpdateSettingsOutputTypeDef",
     "OSUpdateSettingsTypeDef",
     "PaginatorConfigTypeDef",
     "RegisterCertificateResultTypeDef",
     "RegisterEventTopicRequestRequestTypeDef",
     "RejectSharedDirectoryRequestRequestTypeDef",
     "RejectSharedDirectoryResultTypeDef",
     "RemoveIpRoutesRequestRequestTypeDef",
@@ -169,50 +176,50 @@
     "UpdateTrustResultTypeDef",
     "VerifyTrustRequestRequestTypeDef",
     "VerifyTrustResultTypeDef",
     "AcceptSharedDirectoryResultTypeDef",
     "DescribeSharedDirectoriesResultTypeDef",
     "AddIpRoutesRequestRequestTypeDef",
     "AddRegionRequestRequestTypeDef",
-    "RegionDescriptionTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
     "CreateDirectoryRequestRequestTypeDef",
     "CreateMicrosoftADRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "ComputerTypeDef",
     "CreateComputerRequestRequestTypeDef",
     "ListCertificatesResultTypeDef",
     "CertificateTypeDef",
-    "RegisterCertificateRequestRequestTypeDef",
     "DescribeClientAuthenticationSettingsResultTypeDef",
+    "RegisterCertificateRequestRequestTypeDef",
     "DescribeConditionalForwardersResultTypeDef",
     "ConnectDirectoryRequestRequestTypeDef",
     "DescribeDomainControllersResultTypeDef",
     "DescribeEventTopicsResultTypeDef",
     "DescribeLDAPSSettingsResultTypeDef",
     "DescribeSettingsResultTypeDef",
     "DescribeSnapshotsResultTypeDef",
     "DescribeTrustsResultTypeDef",
-    "EnableRadiusRequestRequestTypeDef",
     "OwnerDirectoryDescriptionTypeDef",
-    "UpdateRadiusRequestRequestTypeDef",
     "GetDirectoryLimitsResultTypeDef",
+    "RegionDescriptionTypeDef",
+    "EnableRadiusRequestRequestTypeDef",
+    "UpdateRadiusRequestRequestTypeDef",
     "GetSnapshotLimitsResultTypeDef",
     "ListIpRoutesResultTypeDef",
     "ListLogSubscriptionsResultTypeDef",
     "ListSchemaExtensionsResultTypeDef",
-    "UpdateDirectorySetupRequestRequestTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "UpdateValueTypeDef",
+    "UpdateDirectorySetupRequestRequestTypeDef",
     "UpdateSettingsRequestRequestTypeDef",
     "ShareDirectoryRequestRequestTypeDef",
     "UnshareDirectoryRequestRequestTypeDef",
-    "DescribeRegionsResultTypeDef",
     "CreateComputerResultTypeDef",
     "DescribeCertificateResultTypeDef",
     "DirectoryDescriptionTypeDef",
+    "DescribeRegionsResultTypeDef",
     "UpdateInfoEntryTypeDef",
     "DescribeDirectoriesResultTypeDef",
     "DescribeUpdateDirectoryResultTypeDef",
 )
 
 AcceptSharedDirectoryRequestRequestTypeDef = TypedDict(
     "AcceptSharedDirectoryRequestRequestTypeDef",
@@ -258,14 +265,23 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+AttributeOutputTypeDef = TypedDict(
+    "AttributeOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 AttributeTypeDef = TypedDict(
     "AttributeTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
@@ -287,16 +303,16 @@
         "State": CertificateStateType,
         "ExpiryDateTime": datetime,
         "Type": CertificateTypeType,
     },
     total=False,
 )
 
-ClientCertAuthSettingsTypeDef = TypedDict(
-    "ClientCertAuthSettingsTypeDef",
+ClientCertAuthSettingsOutputTypeDef = TypedDict(
+    "ClientCertAuthSettingsOutputTypeDef",
     {
         "OCSPUrl": str,
     },
     total=False,
 )
 
 ClientAuthenticationSettingInfoTypeDef = TypedDict(
@@ -305,14 +321,22 @@
         "Type": ClientAuthenticationTypeType,
         "Status": ClientAuthenticationStatusType,
         "LastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
+ClientCertAuthSettingsTypeDef = TypedDict(
+    "ClientCertAuthSettingsTypeDef",
+    {
+        "OCSPUrl": str,
+    },
+    total=False,
+)
+
 ConditionalForwarderTypeDef = TypedDict(
     "ConditionalForwarderTypeDef",
     {
         "RemoteDomainName": str,
         "DnsIpAddrs": List[str],
         "ReplicationScope": Literal["Domain"],
     },
@@ -397,19 +421,21 @@
     "_OptionalCreateSnapshotRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class CreateSnapshotRequestRequestTypeDef(
     _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
 ):
     pass
 
+
 CreateSnapshotResultTypeDef = TypedDict(
     "CreateSnapshotResultTypeDef",
     {
         "SnapshotId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -429,19 +455,21 @@
         "TrustType": TrustTypeType,
         "ConditionalForwarderIpAddrs": Sequence[str],
         "SelectiveAuth": SelectiveAuthType,
     },
     total=False,
 )
 
+
 class CreateTrustRequestRequestTypeDef(
     _RequiredCreateTrustRequestRequestTypeDef, _OptionalCreateTrustRequestRequestTypeDef
 ):
     pass
 
+
 CreateTrustResultTypeDef = TypedDict(
     "CreateTrustResultTypeDef",
     {
         "TrustId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -501,19 +529,21 @@
     "_OptionalDeleteTrustRequestRequestTypeDef",
     {
         "DeleteAssociatedConditionalForwarder": bool,
     },
     total=False,
 )
 
+
 class DeleteTrustRequestRequestTypeDef(
     _RequiredDeleteTrustRequestRequestTypeDef, _OptionalDeleteTrustRequestRequestTypeDef
 ):
     pass
 
+
 DeleteTrustResultTypeDef = TypedDict(
     "DeleteTrustResultTypeDef",
     {
         "TrustId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -553,20 +583,22 @@
     {
         "Type": ClientAuthenticationTypeType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef(
     _RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
     _OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeClientAuthenticationSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeClientAuthenticationSettingsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeClientAuthenticationSettingsRequestRequestTypeDef = TypedDict(
@@ -575,40 +607,44 @@
         "Type": ClientAuthenticationTypeType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class DescribeClientAuthenticationSettingsRequestRequestTypeDef(
     _RequiredDescribeClientAuthenticationSettingsRequestRequestTypeDef,
     _OptionalDescribeClientAuthenticationSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeConditionalForwardersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConditionalForwardersRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeConditionalForwardersRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeConditionalForwardersRequestRequestTypeDef",
     {
         "RemoteDomainNames": Sequence[str],
     },
     total=False,
 )
 
+
 class DescribeConditionalForwardersRequestRequestTypeDef(
     _RequiredDescribeConditionalForwardersRequestRequestTypeDef,
     _OptionalDescribeConditionalForwardersRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef = TypedDict(
     "DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef",
     {
         "DirectoryIds": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -635,20 +671,22 @@
     {
         "DomainControllerIds": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef(
     _RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
     _OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeDomainControllersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDomainControllersRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeDomainControllersRequestRequestTypeDef = TypedDict(
@@ -657,20 +695,22 @@
         "DomainControllerIds": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class DescribeDomainControllersRequestRequestTypeDef(
     _RequiredDescribeDomainControllersRequestRequestTypeDef,
     _OptionalDescribeDomainControllersRequestRequestTypeDef,
 ):
     pass
 
+
 DomainControllerTypeDef = TypedDict(
     "DomainControllerTypeDef",
     {
         "DirectoryId": str,
         "DomainControllerId": str,
         "DnsIpAddr": str,
         "VpcId": str,
@@ -716,20 +756,22 @@
     {
         "Type": Literal["Client"],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef(
     _RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
     _OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeLDAPSSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeLDAPSSettingsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeLDAPSSettingsRequestRequestTypeDef = TypedDict(
@@ -738,20 +780,22 @@
         "Type": Literal["Client"],
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class DescribeLDAPSSettingsRequestRequestTypeDef(
     _RequiredDescribeLDAPSSettingsRequestRequestTypeDef,
     _OptionalDescribeLDAPSSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 LDAPSSettingInfoTypeDef = TypedDict(
     "LDAPSSettingInfoTypeDef",
     {
         "LDAPSStatus": LDAPSStatusType,
         "LDAPSStatusReason": str,
         "LastUpdatedDateTime": datetime,
     },
@@ -769,20 +813,22 @@
     {
         "RegionName": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeRegionsRequestDescribeRegionsPaginateTypeDef(
     _RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef,
     _OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeRegionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRegionsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeRegionsRequestRequestTypeDef = TypedDict(
@@ -790,19 +836,21 @@
     {
         "RegionName": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeRegionsRequestRequestTypeDef(
     _RequiredDescribeRegionsRequestRequestTypeDef, _OptionalDescribeRegionsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSettingsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeSettingsRequestRequestTypeDef = TypedDict(
@@ -810,19 +858,21 @@
     {
         "Status": DirectoryConfigurationStatusType,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeSettingsRequestRequestTypeDef(
     _RequiredDescribeSettingsRequestRequestTypeDef, _OptionalDescribeSettingsRequestRequestTypeDef
 ):
     pass
 
+
 SettingEntryTypeDef = TypedDict(
     "SettingEntryTypeDef",
     {
         "Type": str,
         "Name": str,
         "AllowedValues": str,
         "AppliedValue": str,
@@ -848,20 +898,22 @@
     {
         "SharedDirectoryIds": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef(
     _RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
     _OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeSharedDirectoriesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSharedDirectoriesRequestRequestTypeDef",
     {
         "OwnerDirectoryId": str,
     },
 )
 _OptionalDescribeSharedDirectoriesRequestRequestTypeDef = TypedDict(
@@ -870,20 +922,22 @@
         "SharedDirectoryIds": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class DescribeSharedDirectoriesRequestRequestTypeDef(
     _RequiredDescribeSharedDirectoriesRequestRequestTypeDef,
     _OptionalDescribeSharedDirectoriesRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef = TypedDict(
     "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
     {
         "DirectoryId": str,
         "SnapshotIds": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -965,20 +1019,22 @@
     {
         "RegionName": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef(
     _RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
     _OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeUpdateDirectoryRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeUpdateDirectoryRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "UpdateType": Literal["OS"],
     },
 )
@@ -987,20 +1043,22 @@
     {
         "RegionName": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeUpdateDirectoryRequestRequestTypeDef(
     _RequiredDescribeUpdateDirectoryRequestRequestTypeDef,
     _OptionalDescribeUpdateDirectoryRequestRequestTypeDef,
 ):
     pass
 
+
 DirectoryConnectSettingsDescriptionTypeDef = TypedDict(
     "DirectoryConnectSettingsDescriptionTypeDef",
     {
         "VpcId": str,
         "SubnetIds": List[str],
         "CustomerUserName": str,
         "SecurityGroupId": str,
@@ -1017,16 +1075,16 @@
         "SubnetIds": List[str],
         "SecurityGroupId": str,
         "AvailabilityZones": List[str],
     },
     total=False,
 )
 
-RadiusSettingsTypeDef = TypedDict(
-    "RadiusSettingsTypeDef",
+RadiusSettingsOutputTypeDef = TypedDict(
+    "RadiusSettingsOutputTypeDef",
     {
         "RadiusServers": List[str],
         "RadiusPort": int,
         "RadiusTimeout": int,
         "RadiusRetries": int,
         "SharedSecret": str,
         "AuthenticationProtocol": RadiusAuthenticationProtocolType,
@@ -1057,14 +1115,22 @@
         "ConnectedDirectoriesLimit": int,
         "ConnectedDirectoriesCurrentCount": int,
         "ConnectedDirectoriesLimitReached": bool,
     },
     total=False,
 )
 
+DirectoryVpcSettingsOutputTypeDef = TypedDict(
+    "DirectoryVpcSettingsOutputTypeDef",
+    {
+        "VpcId": str,
+        "SubnetIds": List[str],
+    },
+)
+
 DisableClientAuthenticationRequestRequestTypeDef = TypedDict(
     "DisableClientAuthenticationRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Type": ClientAuthenticationTypeType,
     },
 )
@@ -1095,19 +1161,21 @@
     {
         "UserName": str,
         "Password": str,
     },
     total=False,
 )
 
+
 class DisableSsoRequestRequestTypeDef(
     _RequiredDisableSsoRequestRequestTypeDef, _OptionalDisableSsoRequestRequestTypeDef
 ):
     pass
 
+
 EnableClientAuthenticationRequestRequestTypeDef = TypedDict(
     "EnableClientAuthenticationRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Type": ClientAuthenticationTypeType,
     },
 )
@@ -1116,14 +1184,29 @@
     "EnableLDAPSRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Type": Literal["Client"],
     },
 )
 
+RadiusSettingsTypeDef = TypedDict(
+    "RadiusSettingsTypeDef",
+    {
+        "RadiusServers": Sequence[str],
+        "RadiusPort": int,
+        "RadiusTimeout": int,
+        "RadiusRetries": int,
+        "SharedSecret": str,
+        "AuthenticationProtocol": RadiusAuthenticationProtocolType,
+        "DisplayLabel": str,
+        "UseSameUsername": bool,
+    },
+    total=False,
+)
+
 _RequiredEnableSsoRequestRequestTypeDef = TypedDict(
     "_RequiredEnableSsoRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalEnableSsoRequestRequestTypeDef = TypedDict(
@@ -1131,19 +1214,21 @@
     {
         "UserName": str,
         "Password": str,
     },
     total=False,
 )
 
+
 class EnableSsoRequestRequestTypeDef(
     _RequiredEnableSsoRequestRequestTypeDef, _OptionalEnableSsoRequestRequestTypeDef
 ):
     pass
 
+
 GetSnapshotLimitsRequestRequestTypeDef = TypedDict(
     "GetSnapshotLimitsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 
@@ -1180,20 +1265,22 @@
     "_OptionalListCertificatesRequestListCertificatesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListCertificatesRequestListCertificatesPaginateTypeDef(
     _RequiredListCertificatesRequestListCertificatesPaginateTypeDef,
     _OptionalListCertificatesRequestListCertificatesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListCertificatesRequestRequestTypeDef = TypedDict(
     "_RequiredListCertificatesRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalListCertificatesRequestRequestTypeDef = TypedDict(
@@ -1201,39 +1288,43 @@
     {
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class ListCertificatesRequestRequestTypeDef(
     _RequiredListCertificatesRequestRequestTypeDef, _OptionalListCertificatesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef = TypedDict(
     "_RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef = TypedDict(
     "_OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListIpRoutesRequestListIpRoutesPaginateTypeDef(
     _RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef,
     _OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListIpRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredListIpRoutesRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalListIpRoutesRequestRequestTypeDef = TypedDict(
@@ -1241,19 +1332,21 @@
     {
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class ListIpRoutesRequestRequestTypeDef(
     _RequiredListIpRoutesRequestRequestTypeDef, _OptionalListIpRoutesRequestRequestTypeDef
 ):
     pass
 
+
 ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef = TypedDict(
     "ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef",
     {
         "DirectoryId": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1289,20 +1382,22 @@
     "_OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef(
     _RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
     _OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListSchemaExtensionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemaExtensionsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalListSchemaExtensionsRequestRequestTypeDef = TypedDict(
@@ -1310,20 +1405,22 @@
     {
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class ListSchemaExtensionsRequestRequestTypeDef(
     _RequiredListSchemaExtensionsRequestRequestTypeDef,
     _OptionalListSchemaExtensionsRequestRequestTypeDef,
 ):
     pass
 
+
 SchemaExtensionInfoTypeDef = TypedDict(
     "SchemaExtensionInfoTypeDef",
     {
         "DirectoryId": str,
         "SchemaExtensionId": str,
         "Description": str,
         "SchemaExtensionStatus": SchemaExtensionStatusType,
@@ -1344,20 +1441,22 @@
     "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1365,20 +1464,38 @@
     {
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+OSUpdateSettingsOutputTypeDef = TypedDict(
+    "OSUpdateSettingsOutputTypeDef",
+    {
+        "OSVersion": OSVersionType,
+    },
+    total=False,
+)
+
 OSUpdateSettingsTypeDef = TypedDict(
     "OSUpdateSettingsTypeDef",
     {
         "OSVersion": OSVersionType,
     },
     total=False,
 )
@@ -1567,19 +1684,21 @@
     "_OptionalUpdateTrustRequestRequestTypeDef",
     {
         "SelectiveAuth": SelectiveAuthType,
     },
     total=False,
 )
 
+
 class UpdateTrustRequestRequestTypeDef(
     _RequiredUpdateTrustRequestRequestTypeDef, _OptionalUpdateTrustRequestRequestTypeDef
 ):
     pass
 
+
 UpdateTrustResultTypeDef = TypedDict(
     "UpdateTrustResultTypeDef",
     {
         "RequestId": str,
         "TrustId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1628,44 +1747,30 @@
     "_OptionalAddIpRoutesRequestRequestTypeDef",
     {
         "UpdateSecurityGroupForDirectoryControllers": bool,
     },
     total=False,
 )
 
+
 class AddIpRoutesRequestRequestTypeDef(
     _RequiredAddIpRoutesRequestRequestTypeDef, _OptionalAddIpRoutesRequestRequestTypeDef
 ):
     pass
 
+
 AddRegionRequestRequestTypeDef = TypedDict(
     "AddRegionRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RegionName": str,
         "VPCSettings": DirectoryVpcSettingsTypeDef,
     },
 )
 
-RegionDescriptionTypeDef = TypedDict(
-    "RegionDescriptionTypeDef",
-    {
-        "DirectoryId": str,
-        "RegionName": str,
-        "RegionType": RegionTypeType,
-        "Status": DirectoryStageType,
-        "VpcSettings": DirectoryVpcSettingsTypeDef,
-        "DesiredNumberOfDomainControllers": int,
-        "LaunchTime": datetime,
-        "StatusLastUpdatedDateTime": datetime,
-        "LastUpdatedDateTime": datetime,
-    },
-    total=False,
-)
-
 AddTagsToResourceRequestRequestTypeDef = TypedDict(
     "AddTagsToResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1685,19 +1790,21 @@
         "Description": str,
         "VpcSettings": DirectoryVpcSettingsTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDirectoryRequestRequestTypeDef(
     _RequiredCreateDirectoryRequestRequestTypeDef, _OptionalCreateDirectoryRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateMicrosoftADRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMicrosoftADRequestRequestTypeDef",
     {
         "Name": str,
         "Password": str,
         "VpcSettings": DirectoryVpcSettingsTypeDef,
     },
@@ -1709,34 +1816,27 @@
         "Description": str,
         "Edition": DirectoryEditionType,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMicrosoftADRequestRequestTypeDef(
     _RequiredCreateMicrosoftADRequestRequestTypeDef, _OptionalCreateMicrosoftADRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ComputerTypeDef = TypedDict(
     "ComputerTypeDef",
     {
         "ComputerId": str,
         "ComputerName": str,
-        "ComputerAttributes": List[AttributeTypeDef],
+        "ComputerAttributes": List[AttributeOutputTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateComputerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateComputerRequestRequestTypeDef",
     {
@@ -1750,19 +1850,21 @@
     {
         "OrganizationalUnitDistinguishedName": str,
         "ComputerAttributes": Sequence[AttributeTypeDef],
     },
     total=False,
 )
 
+
 class CreateComputerRequestRequestTypeDef(
     _RequiredCreateComputerRequestRequestTypeDef, _OptionalCreateComputerRequestRequestTypeDef
 ):
     pass
 
+
 ListCertificatesResultTypeDef = TypedDict(
     "ListCertificatesResultTypeDef",
     {
         "NextToken": str,
         "CertificatesInfo": List[CertificateInfoTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1774,19 +1876,28 @@
         "CertificateId": str,
         "State": CertificateStateType,
         "StateReason": str,
         "CommonName": str,
         "RegisteredDateTime": datetime,
         "ExpiryDateTime": datetime,
         "Type": CertificateTypeType,
-        "ClientCertAuthSettings": ClientCertAuthSettingsTypeDef,
+        "ClientCertAuthSettings": ClientCertAuthSettingsOutputTypeDef,
     },
     total=False,
 )
 
+DescribeClientAuthenticationSettingsResultTypeDef = TypedDict(
+    "DescribeClientAuthenticationSettingsResultTypeDef",
+    {
+        "ClientAuthenticationSettingsInfo": List[ClientAuthenticationSettingInfoTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRegisterCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterCertificateRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "CertificateData": str,
     },
 )
@@ -1795,28 +1906,21 @@
     {
         "Type": CertificateTypeType,
         "ClientCertAuthSettings": ClientCertAuthSettingsTypeDef,
     },
     total=False,
 )
 
+
 class RegisterCertificateRequestRequestTypeDef(
     _RequiredRegisterCertificateRequestRequestTypeDef,
     _OptionalRegisterCertificateRequestRequestTypeDef,
 ):
     pass
 
-DescribeClientAuthenticationSettingsResultTypeDef = TypedDict(
-    "DescribeClientAuthenticationSettingsResultTypeDef",
-    {
-        "ClientAuthenticationSettingsInfo": List[ClientAuthenticationSettingInfoTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DescribeConditionalForwardersResultTypeDef = TypedDict(
     "DescribeConditionalForwardersResultTypeDef",
     {
         "ConditionalForwarders": List[ConditionalForwarderTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1837,19 +1941,21 @@
         "ShortName": str,
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class ConnectDirectoryRequestRequestTypeDef(
     _RequiredConnectDirectoryRequestRequestTypeDef, _OptionalConnectDirectoryRequestRequestTypeDef
 ):
     pass
 
+
 DescribeDomainControllersResultTypeDef = TypedDict(
     "DescribeDomainControllersResultTypeDef",
     {
         "DomainControllers": List[DomainControllerTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1896,48 +2002,64 @@
     {
         "Trusts": List[TrustTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EnableRadiusRequestRequestTypeDef = TypedDict(
-    "EnableRadiusRequestRequestTypeDef",
-    {
-        "DirectoryId": str,
-        "RadiusSettings": RadiusSettingsTypeDef,
-    },
-)
-
 OwnerDirectoryDescriptionTypeDef = TypedDict(
     "OwnerDirectoryDescriptionTypeDef",
     {
         "DirectoryId": str,
         "AccountId": str,
         "DnsIpAddrs": List[str],
         "VpcSettings": DirectoryVpcSettingsDescriptionTypeDef,
-        "RadiusSettings": RadiusSettingsTypeDef,
+        "RadiusSettings": RadiusSettingsOutputTypeDef,
         "RadiusStatus": RadiusStatusType,
     },
     total=False,
 )
 
-UpdateRadiusRequestRequestTypeDef = TypedDict(
-    "UpdateRadiusRequestRequestTypeDef",
+GetDirectoryLimitsResultTypeDef = TypedDict(
+    "GetDirectoryLimitsResultTypeDef",
+    {
+        "DirectoryLimits": DirectoryLimitsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RegionDescriptionTypeDef = TypedDict(
+    "RegionDescriptionTypeDef",
+    {
+        "DirectoryId": str,
+        "RegionName": str,
+        "RegionType": RegionTypeType,
+        "Status": DirectoryStageType,
+        "VpcSettings": DirectoryVpcSettingsOutputTypeDef,
+        "DesiredNumberOfDomainControllers": int,
+        "LaunchTime": datetime,
+        "StatusLastUpdatedDateTime": datetime,
+        "LastUpdatedDateTime": datetime,
+    },
+    total=False,
+)
+
+EnableRadiusRequestRequestTypeDef = TypedDict(
+    "EnableRadiusRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RadiusSettings": RadiusSettingsTypeDef,
     },
 )
 
-GetDirectoryLimitsResultTypeDef = TypedDict(
-    "GetDirectoryLimitsResultTypeDef",
+UpdateRadiusRequestRequestTypeDef = TypedDict(
+    "UpdateRadiusRequestRequestTypeDef",
     {
-        "DirectoryLimits": DirectoryLimitsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DirectoryId": str,
+        "RadiusSettings": RadiusSettingsTypeDef,
     },
 )
 
 GetSnapshotLimitsResultTypeDef = TypedDict(
     "GetSnapshotLimitsResultTypeDef",
     {
         "SnapshotLimits": SnapshotLimitsTypeDef,
@@ -1968,14 +2090,31 @@
     {
         "SchemaExtensionsInfo": List[SchemaExtensionInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateValueTypeDef = TypedDict(
+    "UpdateValueTypeDef",
+    {
+        "OSUpdateSettings": OSUpdateSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateDirectorySetupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDirectorySetupRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "UpdateType": Literal["OS"],
     },
 )
@@ -1984,27 +2123,21 @@
     {
         "OSUpdateSettings": OSUpdateSettingsTypeDef,
         "CreateSnapshotBeforeUpdate": bool,
     },
     total=False,
 )
 
+
 class UpdateDirectorySetupRequestRequestTypeDef(
     _RequiredUpdateDirectorySetupRequestRequestTypeDef,
     _OptionalUpdateDirectorySetupRequestRequestTypeDef,
 ):
     pass
 
-UpdateValueTypeDef = TypedDict(
-    "UpdateValueTypeDef",
-    {
-        "OSUpdateSettings": OSUpdateSettingsTypeDef,
-    },
-    total=False,
-)
 
 UpdateSettingsRequestRequestTypeDef = TypedDict(
     "UpdateSettingsRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Settings": Sequence[SettingTypeDef],
     },
@@ -2022,36 +2155,29 @@
     "_OptionalShareDirectoryRequestRequestTypeDef",
     {
         "ShareNotes": str,
     },
     total=False,
 )
 
+
 class ShareDirectoryRequestRequestTypeDef(
     _RequiredShareDirectoryRequestRequestTypeDef, _OptionalShareDirectoryRequestRequestTypeDef
 ):
     pass
 
+
 UnshareDirectoryRequestRequestTypeDef = TypedDict(
     "UnshareDirectoryRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "UnshareTarget": UnshareTargetTypeDef,
     },
 )
 
-DescribeRegionsResultTypeDef = TypedDict(
-    "DescribeRegionsResultTypeDef",
-    {
-        "RegionsDescription": List[RegionDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateComputerResultTypeDef = TypedDict(
     "CreateComputerResultTypeDef",
     {
         "Computer": ComputerTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2081,26 +2207,35 @@
         "ShareMethod": ShareMethodType,
         "ShareNotes": str,
         "LaunchTime": datetime,
         "StageLastUpdatedDateTime": datetime,
         "Type": DirectoryTypeType,
         "VpcSettings": DirectoryVpcSettingsDescriptionTypeDef,
         "ConnectSettings": DirectoryConnectSettingsDescriptionTypeDef,
-        "RadiusSettings": RadiusSettingsTypeDef,
+        "RadiusSettings": RadiusSettingsOutputTypeDef,
         "RadiusStatus": RadiusStatusType,
         "StageReason": str,
         "SsoEnabled": bool,
         "DesiredNumberOfDomainControllers": int,
         "OwnerDirectoryDescription": OwnerDirectoryDescriptionTypeDef,
         "RegionsInfo": RegionsInfoTypeDef,
         "OsVersion": OSVersionType,
     },
     total=False,
 )
 
+DescribeRegionsResultTypeDef = TypedDict(
+    "DescribeRegionsResultTypeDef",
+    {
+        "RegionsDescription": List[RegionDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateInfoEntryTypeDef = TypedDict(
     "UpdateInfoEntryTypeDef",
     {
         "Region": str,
         "Status": UpdateStatusType,
         "StatusReason": str,
         "InitiatedBy": str,
```

### Comparing `mypy-boto3-ds-1.28.0/mypy_boto3_ds.egg-info/PKG-INFO` & `mypy-boto3-ds-1.28.12/mypy_boto3_ds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ds
-Version: 1.28.0
-Summary: Type annotations for boto3.DirectoryService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.DirectoryService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ds"></a>
 
 # mypy-boto3-ds
 
 [![PyPI - mypy-boto3-ds](https://img.shields.io/pypi/v/mypy-boto3-ds.svg?color=blue)](https://pypi.org/project/mypy-boto3-ds)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ds.svg?color=blue)](https://pypi.org/project/mypy-boto3-ds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ds?color=blue)](https://pypistats.org/packages/mypy-boto3-ds)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ds)](https://pepy.tech/project/mypy-boto3-ds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DirectoryService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
+[boto3.DirectoryService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
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
 [mypy-boto3-ds docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/).
 
 See how it helps to find and fix potential bugs:
 
@@ -414,19 +414,21 @@
 ```python
 from mypy_boto3_ds.type_defs import (
     AcceptSharedDirectoryRequestRequestTypeDef,
     SharedDirectoryTypeDef,
     IpRouteTypeDef,
     DirectoryVpcSettingsTypeDef,
     TagTypeDef,
+    AttributeOutputTypeDef,
     AttributeTypeDef,
     CancelSchemaExtensionRequestRequestTypeDef,
     CertificateInfoTypeDef,
-    ClientCertAuthSettingsTypeDef,
+    ClientCertAuthSettingsOutputTypeDef,
     ClientAuthenticationSettingInfoTypeDef,
+    ClientCertAuthSettingsTypeDef,
     ConditionalForwarderTypeDef,
     DirectoryConnectSettingsTypeDef,
     ConnectDirectoryResultTypeDef,
     CreateAliasRequestRequestTypeDef,
     CreateAliasResultTypeDef,
     CreateConditionalForwarderRequestRequestTypeDef,
     CreateDirectoryResultTypeDef,
@@ -472,23 +474,25 @@
     DescribeTrustsRequestDescribeTrustsPaginateTypeDef,
     DescribeTrustsRequestRequestTypeDef,
     TrustTypeDef,
     DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
     DescribeUpdateDirectoryRequestRequestTypeDef,
     DirectoryConnectSettingsDescriptionTypeDef,
     DirectoryVpcSettingsDescriptionTypeDef,
-    RadiusSettingsTypeDef,
+    RadiusSettingsOutputTypeDef,
     RegionsInfoTypeDef,
     DirectoryLimitsTypeDef,
+    DirectoryVpcSettingsOutputTypeDef,
     DisableClientAuthenticationRequestRequestTypeDef,
     DisableLDAPSRequestRequestTypeDef,
     DisableRadiusRequestRequestTypeDef,
     DisableSsoRequestRequestTypeDef,
     EnableClientAuthenticationRequestRequestTypeDef,
     EnableLDAPSRequestRequestTypeDef,
+    RadiusSettingsTypeDef,
     EnableSsoRequestRequestTypeDef,
     GetSnapshotLimitsRequestRequestTypeDef,
     SnapshotLimitsTypeDef,
     IpRouteInfoTypeDef,
     ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListCertificatesRequestRequestTypeDef,
     ListIpRoutesRequestListIpRoutesPaginateTypeDef,
@@ -497,14 +501,16 @@
     ListLogSubscriptionsRequestRequestTypeDef,
     LogSubscriptionTypeDef,
     ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
     ListSchemaExtensionsRequestRequestTypeDef,
     SchemaExtensionInfoTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    OSUpdateSettingsOutputTypeDef,
     OSUpdateSettingsTypeDef,
     PaginatorConfigTypeDef,
     RegisterCertificateResultTypeDef,
     RegisterEventTopicRequestRequestTypeDef,
     RejectSharedDirectoryRequestRequestTypeDef,
     RejectSharedDirectoryResultTypeDef,
     RemoveIpRoutesRequestRequestTypeDef,
@@ -527,50 +533,50 @@
     UpdateTrustResultTypeDef,
     VerifyTrustRequestRequestTypeDef,
     VerifyTrustResultTypeDef,
     AcceptSharedDirectoryResultTypeDef,
     DescribeSharedDirectoriesResultTypeDef,
     AddIpRoutesRequestRequestTypeDef,
     AddRegionRequestRequestTypeDef,
-    RegionDescriptionTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
     CreateDirectoryRequestRequestTypeDef,
     CreateMicrosoftADRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     ComputerTypeDef,
     CreateComputerRequestRequestTypeDef,
     ListCertificatesResultTypeDef,
     CertificateTypeDef,
-    RegisterCertificateRequestRequestTypeDef,
     DescribeClientAuthenticationSettingsResultTypeDef,
+    RegisterCertificateRequestRequestTypeDef,
     DescribeConditionalForwardersResultTypeDef,
     ConnectDirectoryRequestRequestTypeDef,
     DescribeDomainControllersResultTypeDef,
     DescribeEventTopicsResultTypeDef,
     DescribeLDAPSSettingsResultTypeDef,
     DescribeSettingsResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeTrustsResultTypeDef,
-    EnableRadiusRequestRequestTypeDef,
     OwnerDirectoryDescriptionTypeDef,
-    UpdateRadiusRequestRequestTypeDef,
     GetDirectoryLimitsResultTypeDef,
+    RegionDescriptionTypeDef,
+    EnableRadiusRequestRequestTypeDef,
+    UpdateRadiusRequestRequestTypeDef,
     GetSnapshotLimitsResultTypeDef,
     ListIpRoutesResultTypeDef,
     ListLogSubscriptionsResultTypeDef,
     ListSchemaExtensionsResultTypeDef,
-    UpdateDirectorySetupRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
     UpdateValueTypeDef,
+    UpdateDirectorySetupRequestRequestTypeDef,
     UpdateSettingsRequestRequestTypeDef,
     ShareDirectoryRequestRequestTypeDef,
     UnshareDirectoryRequestRequestTypeDef,
-    DescribeRegionsResultTypeDef,
     CreateComputerResultTypeDef,
     DescribeCertificateResultTypeDef,
     DirectoryDescriptionTypeDef,
+    DescribeRegionsResultTypeDef,
     UpdateInfoEntryTypeDef,
     DescribeDirectoriesResultTypeDef,
     DescribeUpdateDirectoryResultTypeDef,
 )
 
 
 def get_structure() -> AcceptSharedDirectoryRequestRequestTypeDef:
```

### Comparing `mypy-boto3-ds-1.28.0/mypy_boto3_ds.egg-info/SOURCES.txt` & `mypy-boto3-ds-1.28.12/mypy_boto3_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.0/setup.py` & `mypy-boto3-ds-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ds",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_ds"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DirectoryService 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.DirectoryService 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

