# Comparing `tmp/mypy-boto3-worklink-1.28.0.tar.gz` & `tmp/mypy-boto3-worklink-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-worklink-1.28.0.tar", last modified: Thu Jul  6 21:00:52 2023, max compression
+gzip compressed data, was "mypy-boto3-worklink-1.28.12.tar", last modified: Thu Jul 27 11:49:50 2023, max compression
```

## Comparing `mypy-boto3-worklink-1.28.0.tar` & `mypy-boto3-worklink-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:52.314461 mypy-boto3-worklink-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:58:12.000000 mypy-boto3-worklink-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14620 2023-07-06 21:00:52.314461 mypy-boto3-worklink-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13131 2023-07-06 20:58:12.000000 mypy-boto3-worklink-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:52.310461 mypy-boto3-worklink-1.28.0/mypy_boto3_worklink/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-06 20:58:12.000000 mypy-boto3-worklink-1.28.0/mypy_boto3_worklink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-06 20:58:12.000000 mypy-boto3-worklink-1.28.0/mypy_boto3_worklink/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:58:12.000000 mypy-boto3-worklink-1.28.0/mypy_boto3_worklink/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22013 2023-07-06 20:58:12.000000 mypy-boto3-worklink-1.28.0/mypy_boto3_worklink/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21973 2023-07-06 20:58:12.000000 mypy-boto3-worklink-1.28.0/mypy_boto3_worklink/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-07-06 20:58:12.000000 mypy-boto3-worklink-1.28.0/mypy_boto3_worklink/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-06 20:58:12.000000 mypy-boto3-worklink-1.28.0/mypy_boto3_worklink/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:12.000000 mypy-boto3-worklink-1.28.0/mypy_boto3_worklink/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21253 2023-07-06 20:58:13.000000 mypy-boto3-worklink-1.28.0/mypy_boto3_worklink/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21222 2023-07-06 20:58:13.000000 mypy-boto3-worklink-1.28.0/mypy_boto3_worklink/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:58:12.000000 mypy-boto3-worklink-1.28.0/mypy_boto3_worklink/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:52.314461 mypy-boto3-worklink-1.28.0/mypy_boto3_worklink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14620 2023-07-06 21:00:52.000000 mypy-boto3-worklink-1.28.0/mypy_boto3_worklink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-06 21:00:52.000000 mypy-boto3-worklink-1.28.0/mypy_boto3_worklink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:52.000000 mypy-boto3-worklink-1.28.0/mypy_boto3_worklink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:52.000000 mypy-boto3-worklink-1.28.0/mypy_boto3_worklink.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:52.000000 mypy-boto3-worklink-1.28.0/mypy_boto3_worklink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:00:52.000000 mypy-boto3-worklink-1.28.0/mypy_boto3_worklink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:52.314461 mypy-boto3-worklink-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:58:12.000000 mypy-boto3-worklink-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.989496 mypy-boto3-worklink-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:51.000000 mypy-boto3-worklink-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-07-27 11:49:49.989496 mypy-boto3-worklink-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-07-27 11:48:51.000000 mypy-boto3-worklink-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.981496 mypy-boto3-worklink-1.28.12/mypy_boto3_worklink/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-27 11:48:51.000000 mypy-boto3-worklink-1.28.12/mypy_boto3_worklink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-27 11:48:51.000000 mypy-boto3-worklink-1.28.12/mypy_boto3_worklink/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:48:51.000000 mypy-boto3-worklink-1.28.12/mypy_boto3_worklink/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22013 2023-07-27 11:48:53.000000 mypy-boto3-worklink-1.28.12/mypy_boto3_worklink/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21973 2023-07-27 11:48:53.000000 mypy-boto3-worklink-1.28.12/mypy_boto3_worklink/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-07-27 11:48:53.000000 mypy-boto3-worklink-1.28.12/mypy_boto3_worklink/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-07-27 11:48:53.000000 mypy-boto3-worklink-1.28.12/mypy_boto3_worklink/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:51.000000 mypy-boto3-worklink-1.28.12/mypy_boto3_worklink/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21219 2023-07-27 11:48:54.000000 mypy-boto3-worklink-1.28.12/mypy_boto3_worklink/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21188 2023-07-27 11:48:54.000000 mypy-boto3-worklink-1.28.12/mypy_boto3_worklink/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:51.000000 mypy-boto3-worklink-1.28.12/mypy_boto3_worklink/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.989496 mypy-boto3-worklink-1.28.12/mypy_boto3_worklink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-07-27 11:49:49.000000 mypy-boto3-worklink-1.28.12/mypy_boto3_worklink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-27 11:49:49.000000 mypy-boto3-worklink-1.28.12/mypy_boto3_worklink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:49.000000 mypy-boto3-worklink-1.28.12/mypy_boto3_worklink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:49.000000 mypy-boto3-worklink-1.28.12/mypy_boto3_worklink.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:49.000000 mypy-boto3-worklink-1.28.12/mypy_boto3_worklink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:49.000000 mypy-boto3-worklink-1.28.12/mypy_boto3_worklink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:49.989496 mypy-boto3-worklink-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:48:51.000000 mypy-boto3-worklink-1.28.12/setup.py
```

### Comparing `mypy-boto3-worklink-1.28.0/LICENSE` & `mypy-boto3-worklink-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-worklink-1.28.0/PKG-INFO` & `mypy-boto3-worklink-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-worklink
-Version: 1.28.0
-Summary: Type annotations for boto3.WorkLink 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.WorkLink 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_worklink/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-worklink"></a>
 
 # mypy-boto3-worklink
 
 [![PyPI - mypy-boto3-worklink](https://img.shields.io/pypi/v/mypy-boto3-worklink.svg?color=blue)](https://pypi.org/project/mypy-boto3-worklink)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-worklink.svg?color=blue)](https://pypi.org/project/mypy-boto3-worklink)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_worklink/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-worklink?color=blue)](https://pypistats.org/packages/mypy-boto3-worklink)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-worklink)](https://pepy.tech/project/mypy-boto3-worklink)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkLink 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
+[boto3.WorkLink 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
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
 [mypy-boto3-worklink docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_worklink/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,63 +301,63 @@
 `mypy_boto3_worklink.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_worklink.type_defs import (
     AssociateDomainRequestRequestTypeDef,
     AssociateWebsiteAuthorizationProviderRequestRequestTypeDef,
-    AssociateWebsiteAuthorizationProviderResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociateWebsiteCertificateAuthorityRequestRequestTypeDef,
-    AssociateWebsiteCertificateAuthorityResponseTypeDef,
     CreateFleetRequestRequestTypeDef,
-    CreateFleetResponseTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DescribeAuditStreamConfigurationRequestRequestTypeDef,
-    DescribeAuditStreamConfigurationResponseTypeDef,
     DescribeCompanyNetworkConfigurationRequestRequestTypeDef,
-    DescribeCompanyNetworkConfigurationResponseTypeDef,
     DescribeDevicePolicyConfigurationRequestRequestTypeDef,
-    DescribeDevicePolicyConfigurationResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
-    DescribeDeviceResponseTypeDef,
     DescribeDomainRequestRequestTypeDef,
-    DescribeDomainResponseTypeDef,
     DescribeFleetMetadataRequestRequestTypeDef,
-    DescribeFleetMetadataResponseTypeDef,
     DescribeIdentityProviderConfigurationRequestRequestTypeDef,
-    DescribeIdentityProviderConfigurationResponseTypeDef,
     DescribeWebsiteCertificateAuthorityRequestRequestTypeDef,
-    DescribeWebsiteCertificateAuthorityResponseTypeDef,
     DeviceSummaryTypeDef,
     DisassociateDomainRequestRequestTypeDef,
     DisassociateWebsiteAuthorizationProviderRequestRequestTypeDef,
     DisassociateWebsiteCertificateAuthorityRequestRequestTypeDef,
     DomainSummaryTypeDef,
     FleetSummaryTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFleetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWebsiteAuthorizationProvidersRequestRequestTypeDef,
     WebsiteAuthorizationProviderSummaryTypeDef,
     ListWebsiteCertificateAuthoritiesRequestRequestTypeDef,
     WebsiteCaSummaryTypeDef,
-    ResponseMetadataTypeDef,
     RestoreDomainAccessRequestRequestTypeDef,
     RevokeDomainAccessRequestRequestTypeDef,
     SignOutUserRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuditStreamConfigurationRequestRequestTypeDef,
     UpdateCompanyNetworkConfigurationRequestRequestTypeDef,
     UpdateDevicePolicyConfigurationRequestRequestTypeDef,
     UpdateDomainMetadataRequestRequestTypeDef,
     UpdateFleetMetadataRequestRequestTypeDef,
     UpdateIdentityProviderConfigurationRequestRequestTypeDef,
+    AssociateWebsiteAuthorizationProviderResponseTypeDef,
+    AssociateWebsiteCertificateAuthorityResponseTypeDef,
+    CreateFleetResponseTypeDef,
+    DescribeAuditStreamConfigurationResponseTypeDef,
+    DescribeCompanyNetworkConfigurationResponseTypeDef,
+    DescribeDevicePolicyConfigurationResponseTypeDef,
+    DescribeDeviceResponseTypeDef,
+    DescribeDomainResponseTypeDef,
+    DescribeFleetMetadataResponseTypeDef,
+    DescribeIdentityProviderConfigurationResponseTypeDef,
+    DescribeWebsiteCertificateAuthorityResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListDevicesResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListFleetsResponseTypeDef,
     ListWebsiteAuthorizationProvidersResponseTypeDef,
     ListWebsiteCertificateAuthoritiesResponseTypeDef,
 )
```

### Comparing `mypy-boto3-worklink-1.28.0/README.md` & `mypy-boto3-worklink-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-worklink"></a>
 
 # mypy-boto3-worklink
 
 [![PyPI - mypy-boto3-worklink](https://img.shields.io/pypi/v/mypy-boto3-worklink.svg?color=blue)](https://pypi.org/project/mypy-boto3-worklink)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-worklink.svg?color=blue)](https://pypi.org/project/mypy-boto3-worklink)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_worklink/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-worklink?color=blue)](https://pypistats.org/packages/mypy-boto3-worklink)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-worklink)](https://pepy.tech/project/mypy-boto3-worklink)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkLink 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
+[boto3.WorkLink 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
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
 [mypy-boto3-worklink docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_worklink/).
 
 See how it helps to find and fix potential bugs:
 
@@ -269,63 +269,63 @@
 `mypy_boto3_worklink.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_worklink.type_defs import (
     AssociateDomainRequestRequestTypeDef,
     AssociateWebsiteAuthorizationProviderRequestRequestTypeDef,
-    AssociateWebsiteAuthorizationProviderResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociateWebsiteCertificateAuthorityRequestRequestTypeDef,
-    AssociateWebsiteCertificateAuthorityResponseTypeDef,
     CreateFleetRequestRequestTypeDef,
-    CreateFleetResponseTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DescribeAuditStreamConfigurationRequestRequestTypeDef,
-    DescribeAuditStreamConfigurationResponseTypeDef,
     DescribeCompanyNetworkConfigurationRequestRequestTypeDef,
-    DescribeCompanyNetworkConfigurationResponseTypeDef,
     DescribeDevicePolicyConfigurationRequestRequestTypeDef,
-    DescribeDevicePolicyConfigurationResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
-    DescribeDeviceResponseTypeDef,
     DescribeDomainRequestRequestTypeDef,
-    DescribeDomainResponseTypeDef,
     DescribeFleetMetadataRequestRequestTypeDef,
-    DescribeFleetMetadataResponseTypeDef,
     DescribeIdentityProviderConfigurationRequestRequestTypeDef,
-    DescribeIdentityProviderConfigurationResponseTypeDef,
     DescribeWebsiteCertificateAuthorityRequestRequestTypeDef,
-    DescribeWebsiteCertificateAuthorityResponseTypeDef,
     DeviceSummaryTypeDef,
     DisassociateDomainRequestRequestTypeDef,
     DisassociateWebsiteAuthorizationProviderRequestRequestTypeDef,
     DisassociateWebsiteCertificateAuthorityRequestRequestTypeDef,
     DomainSummaryTypeDef,
     FleetSummaryTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFleetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWebsiteAuthorizationProvidersRequestRequestTypeDef,
     WebsiteAuthorizationProviderSummaryTypeDef,
     ListWebsiteCertificateAuthoritiesRequestRequestTypeDef,
     WebsiteCaSummaryTypeDef,
-    ResponseMetadataTypeDef,
     RestoreDomainAccessRequestRequestTypeDef,
     RevokeDomainAccessRequestRequestTypeDef,
     SignOutUserRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuditStreamConfigurationRequestRequestTypeDef,
     UpdateCompanyNetworkConfigurationRequestRequestTypeDef,
     UpdateDevicePolicyConfigurationRequestRequestTypeDef,
     UpdateDomainMetadataRequestRequestTypeDef,
     UpdateFleetMetadataRequestRequestTypeDef,
     UpdateIdentityProviderConfigurationRequestRequestTypeDef,
+    AssociateWebsiteAuthorizationProviderResponseTypeDef,
+    AssociateWebsiteCertificateAuthorityResponseTypeDef,
+    CreateFleetResponseTypeDef,
+    DescribeAuditStreamConfigurationResponseTypeDef,
+    DescribeCompanyNetworkConfigurationResponseTypeDef,
+    DescribeDevicePolicyConfigurationResponseTypeDef,
+    DescribeDeviceResponseTypeDef,
+    DescribeDomainResponseTypeDef,
+    DescribeFleetMetadataResponseTypeDef,
+    DescribeIdentityProviderConfigurationResponseTypeDef,
+    DescribeWebsiteCertificateAuthorityResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListDevicesResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListFleetsResponseTypeDef,
     ListWebsiteAuthorizationProvidersResponseTypeDef,
     ListWebsiteCertificateAuthoritiesResponseTypeDef,
 )
```

### Comparing `mypy-boto3-worklink-1.28.0/mypy_boto3_worklink/__main__.py` & `mypy-boto3-worklink-1.28.12/mypy_boto3_worklink/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkLink 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.WorkLink 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_worklink//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink\nOther"
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

### Comparing `mypy-boto3-worklink-1.28.0/mypy_boto3_worklink/client.py` & `mypy-boto3-worklink-1.28.12/mypy_boto3_worklink/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-worklink-1.28.0/mypy_boto3_worklink/client.pyi` & `mypy-boto3-worklink-1.28.12/mypy_boto3_worklink/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-worklink-1.28.0/mypy_boto3_worklink/literals.py` & `mypy-boto3-worklink-1.28.12/mypy_boto3_worklink/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,15 @@
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
@@ -249,26 +250,28 @@
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

### Comparing `mypy-boto3-worklink-1.28.0/mypy_boto3_worklink/literals.pyi` & `mypy-boto3-worklink-1.28.12/mypy_boto3_worklink/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,15 @@
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
@@ -247,26 +248,28 @@
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

### Comparing `mypy-boto3-worklink-1.28.0/mypy_boto3_worklink/type_defs.py` & `mypy-boto3-worklink-1.28.12/mypy_boto3_worklink/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -22,67 +22,66 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateDomainRequestRequestTypeDef",
     "AssociateWebsiteAuthorizationProviderRequestRequestTypeDef",
-    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateWebsiteCertificateAuthorityRequestRequestTypeDef",
-    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
     "CreateFleetRequestRequestTypeDef",
-    "CreateFleetResponseTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DescribeAuditStreamConfigurationRequestRequestTypeDef",
-    "DescribeAuditStreamConfigurationResponseTypeDef",
     "DescribeCompanyNetworkConfigurationRequestRequestTypeDef",
-    "DescribeCompanyNetworkConfigurationResponseTypeDef",
     "DescribeDevicePolicyConfigurationRequestRequestTypeDef",
-    "DescribeDevicePolicyConfigurationResponseTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
-    "DescribeDeviceResponseTypeDef",
     "DescribeDomainRequestRequestTypeDef",
-    "DescribeDomainResponseTypeDef",
     "DescribeFleetMetadataRequestRequestTypeDef",
-    "DescribeFleetMetadataResponseTypeDef",
     "DescribeIdentityProviderConfigurationRequestRequestTypeDef",
-    "DescribeIdentityProviderConfigurationResponseTypeDef",
     "DescribeWebsiteCertificateAuthorityRequestRequestTypeDef",
-    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
     "DeviceSummaryTypeDef",
     "DisassociateDomainRequestRequestTypeDef",
     "DisassociateWebsiteAuthorizationProviderRequestRequestTypeDef",
     "DisassociateWebsiteCertificateAuthorityRequestRequestTypeDef",
     "DomainSummaryTypeDef",
     "FleetSummaryTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFleetsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListWebsiteAuthorizationProvidersRequestRequestTypeDef",
     "WebsiteAuthorizationProviderSummaryTypeDef",
     "ListWebsiteCertificateAuthoritiesRequestRequestTypeDef",
     "WebsiteCaSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreDomainAccessRequestRequestTypeDef",
     "RevokeDomainAccessRequestRequestTypeDef",
     "SignOutUserRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuditStreamConfigurationRequestRequestTypeDef",
     "UpdateCompanyNetworkConfigurationRequestRequestTypeDef",
     "UpdateDevicePolicyConfigurationRequestRequestTypeDef",
     "UpdateDomainMetadataRequestRequestTypeDef",
     "UpdateFleetMetadataRequestRequestTypeDef",
     "UpdateIdentityProviderConfigurationRequestRequestTypeDef",
+    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
+    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
+    "CreateFleetResponseTypeDef",
+    "DescribeAuditStreamConfigurationResponseTypeDef",
+    "DescribeCompanyNetworkConfigurationResponseTypeDef",
+    "DescribeDevicePolicyConfigurationResponseTypeDef",
+    "DescribeDeviceResponseTypeDef",
+    "DescribeDomainResponseTypeDef",
+    "DescribeFleetMetadataResponseTypeDef",
+    "DescribeIdentityProviderConfigurationResponseTypeDef",
+    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "ListDomainsResponseTypeDef",
     "ListFleetsResponseTypeDef",
     "ListWebsiteAuthorizationProvidersResponseTypeDef",
     "ListWebsiteCertificateAuthoritiesResponseTypeDef",
 )
 
@@ -98,21 +97,19 @@
     "_OptionalAssociateDomainRequestRequestTypeDef",
     {
         "DisplayName": str,
     },
     total=False,
 )
 
-
 class AssociateDomainRequestRequestTypeDef(
     _RequiredAssociateDomainRequestRequestTypeDef, _OptionalAssociateDomainRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredAssociateWebsiteAuthorizationProviderRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateWebsiteAuthorizationProviderRequestRequestTypeDef",
     {
         "FleetArn": str,
         "AuthorizationProviderType": Literal["SAML"],
     },
 )
@@ -120,27 +117,28 @@
     "_OptionalAssociateWebsiteAuthorizationProviderRequestRequestTypeDef",
     {
         "DomainName": str,
     },
     total=False,
 )
 
-
 class AssociateWebsiteAuthorizationProviderRequestRequestTypeDef(
     _RequiredAssociateWebsiteAuthorizationProviderRequestRequestTypeDef,
     _OptionalAssociateWebsiteAuthorizationProviderRequestRequestTypeDef,
 ):
     pass
 
-
-AssociateWebsiteAuthorizationProviderResponseTypeDef = TypedDict(
-    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AuthorizationProviderId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredAssociateWebsiteCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateWebsiteCertificateAuthorityRequestRequestTypeDef",
     {
         "FleetArn": str,
@@ -151,30 +149,20 @@
     "_OptionalAssociateWebsiteCertificateAuthorityRequestRequestTypeDef",
     {
         "DisplayName": str,
     },
     total=False,
 )
 
-
 class AssociateWebsiteCertificateAuthorityRequestRequestTypeDef(
     _RequiredAssociateWebsiteCertificateAuthorityRequestRequestTypeDef,
     _OptionalAssociateWebsiteCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
-
-AssociateWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
-    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
-    {
-        "WebsiteCaId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateFleetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFleetRequestRequestTypeDef",
     {
         "FleetName": str,
     },
 )
 _OptionalCreateFleetRequestRequestTypeDef = TypedDict(
@@ -183,184 +171,85 @@
         "DisplayName": str,
         "OptimizeForEndUserLocation": bool,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateFleetRequestRequestTypeDef(
     _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
 ):
     pass
 
-
-CreateFleetResponseTypeDef = TypedDict(
-    "CreateFleetResponseTypeDef",
-    {
-        "FleetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteFleetRequestRequestTypeDef = TypedDict(
     "DeleteFleetRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
 DescribeAuditStreamConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeAuditStreamConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
-DescribeAuditStreamConfigurationResponseTypeDef = TypedDict(
-    "DescribeAuditStreamConfigurationResponseTypeDef",
-    {
-        "AuditStreamArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeCompanyNetworkConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeCompanyNetworkConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
-DescribeCompanyNetworkConfigurationResponseTypeDef = TypedDict(
-    "DescribeCompanyNetworkConfigurationResponseTypeDef",
-    {
-        "VpcId": str,
-        "SubnetIds": List[str],
-        "SecurityGroupIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDevicePolicyConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeDevicePolicyConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
-DescribeDevicePolicyConfigurationResponseTypeDef = TypedDict(
-    "DescribeDevicePolicyConfigurationResponseTypeDef",
-    {
-        "DeviceCaCertificate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDeviceRequestRequestTypeDef = TypedDict(
     "DescribeDeviceRequestRequestTypeDef",
     {
         "FleetArn": str,
         "DeviceId": str,
     },
 )
 
-DescribeDeviceResponseTypeDef = TypedDict(
-    "DescribeDeviceResponseTypeDef",
-    {
-        "Status": DeviceStatusType,
-        "Model": str,
-        "Manufacturer": str,
-        "OperatingSystem": str,
-        "OperatingSystemVersion": str,
-        "PatchLevel": str,
-        "FirstAccessedTime": datetime,
-        "LastAccessedTime": datetime,
-        "Username": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDomainRequestRequestTypeDef = TypedDict(
     "DescribeDomainRequestRequestTypeDef",
     {
         "FleetArn": str,
         "DomainName": str,
     },
 )
 
-DescribeDomainResponseTypeDef = TypedDict(
-    "DescribeDomainResponseTypeDef",
-    {
-        "DomainName": str,
-        "DisplayName": str,
-        "CreatedTime": datetime,
-        "DomainStatus": DomainStatusType,
-        "AcmCertificateArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeFleetMetadataRequestRequestTypeDef = TypedDict(
     "DescribeFleetMetadataRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
-DescribeFleetMetadataResponseTypeDef = TypedDict(
-    "DescribeFleetMetadataResponseTypeDef",
-    {
-        "CreatedTime": datetime,
-        "LastUpdatedTime": datetime,
-        "FleetName": str,
-        "DisplayName": str,
-        "OptimizeForEndUserLocation": bool,
-        "CompanyCode": str,
-        "FleetStatus": FleetStatusType,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeIdentityProviderConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeIdentityProviderConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
-DescribeIdentityProviderConfigurationResponseTypeDef = TypedDict(
-    "DescribeIdentityProviderConfigurationResponseTypeDef",
-    {
-        "IdentityProviderType": Literal["SAML"],
-        "ServiceProviderSamlMetadata": str,
-        "IdentityProviderSamlMetadata": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeWebsiteCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "DescribeWebsiteCertificateAuthorityRequestRequestTypeDef",
     {
         "FleetArn": str,
         "WebsiteCaId": str,
     },
 )
 
-DescribeWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
-    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
-    {
-        "Certificate": str,
-        "CreatedTime": datetime,
-        "DisplayName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeviceSummaryTypeDef = TypedDict(
     "DeviceSummaryTypeDef",
     {
         "DeviceId": str,
         "DeviceStatus": DeviceStatusType,
     },
     total=False,
@@ -402,19 +291,17 @@
     "_OptionalDomainSummaryTypeDef",
     {
         "DisplayName": str,
     },
     total=False,
 )
 
-
 class DomainSummaryTypeDef(_RequiredDomainSummaryTypeDef, _OptionalDomainSummaryTypeDef):
     pass
 
-
 FleetSummaryTypeDef = TypedDict(
     "FleetSummaryTypeDef",
     {
         "FleetArn": str,
         "CreatedTime": datetime,
         "LastUpdatedTime": datetime,
         "FleetName": str,
@@ -437,21 +324,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListDevicesRequestRequestTypeDef(
     _RequiredListDevicesRequestRequestTypeDef, _OptionalListDevicesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListDomainsRequestRequestTypeDef = TypedDict(
     "_RequiredListDomainsRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 _OptionalListDomainsRequestRequestTypeDef = TypedDict(
@@ -459,21 +344,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListDomainsRequestRequestTypeDef(
     _RequiredListDomainsRequestRequestTypeDef, _OptionalListDomainsRequestRequestTypeDef
 ):
     pass
 
-
 ListFleetsRequestRequestTypeDef = TypedDict(
     "ListFleetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -482,22 +365,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListWebsiteAuthorizationProvidersRequestRequestTypeDef = TypedDict(
     "_RequiredListWebsiteAuthorizationProvidersRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 _OptionalListWebsiteAuthorizationProvidersRequestRequestTypeDef = TypedDict(
@@ -505,22 +380,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListWebsiteAuthorizationProvidersRequestRequestTypeDef(
     _RequiredListWebsiteAuthorizationProvidersRequestRequestTypeDef,
     _OptionalListWebsiteAuthorizationProvidersRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredWebsiteAuthorizationProviderSummaryTypeDef = TypedDict(
     "_RequiredWebsiteAuthorizationProviderSummaryTypeDef",
     {
         "AuthorizationProviderType": Literal["SAML"],
     },
 )
 _OptionalWebsiteAuthorizationProviderSummaryTypeDef = TypedDict(
@@ -529,22 +402,20 @@
         "AuthorizationProviderId": str,
         "DomainName": str,
         "CreatedTime": datetime,
     },
     total=False,
 )
 
-
 class WebsiteAuthorizationProviderSummaryTypeDef(
     _RequiredWebsiteAuthorizationProviderSummaryTypeDef,
     _OptionalWebsiteAuthorizationProviderSummaryTypeDef,
 ):
     pass
 
-
 _RequiredListWebsiteCertificateAuthoritiesRequestRequestTypeDef = TypedDict(
     "_RequiredListWebsiteCertificateAuthoritiesRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 _OptionalListWebsiteCertificateAuthoritiesRequestRequestTypeDef = TypedDict(
@@ -552,43 +423,30 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListWebsiteCertificateAuthoritiesRequestRequestTypeDef(
     _RequiredListWebsiteCertificateAuthoritiesRequestRequestTypeDef,
     _OptionalListWebsiteCertificateAuthoritiesRequestRequestTypeDef,
 ):
     pass
 
-
 WebsiteCaSummaryTypeDef = TypedDict(
     "WebsiteCaSummaryTypeDef",
     {
         "WebsiteCaId": str,
         "CreatedTime": datetime,
         "DisplayName": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 RestoreDomainAccessRequestRequestTypeDef = TypedDict(
     "RestoreDomainAccessRequestRequestTypeDef",
     {
         "FleetArn": str,
         "DomainName": str,
     },
 )
@@ -635,22 +493,20 @@
     "_OptionalUpdateAuditStreamConfigurationRequestRequestTypeDef",
     {
         "AuditStreamArn": str,
     },
     total=False,
 )
 
-
 class UpdateAuditStreamConfigurationRequestRequestTypeDef(
     _RequiredUpdateAuditStreamConfigurationRequestRequestTypeDef,
     _OptionalUpdateAuditStreamConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateCompanyNetworkConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateCompanyNetworkConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
         "VpcId": str,
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
@@ -667,22 +523,20 @@
     "_OptionalUpdateDevicePolicyConfigurationRequestRequestTypeDef",
     {
         "DeviceCaCertificate": str,
     },
     total=False,
 )
 
-
 class UpdateDevicePolicyConfigurationRequestRequestTypeDef(
     _RequiredUpdateDevicePolicyConfigurationRequestRequestTypeDef,
     _OptionalUpdateDevicePolicyConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateDomainMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDomainMetadataRequestRequestTypeDef",
     {
         "FleetArn": str,
         "DomainName": str,
     },
 )
@@ -690,22 +544,20 @@
     "_OptionalUpdateDomainMetadataRequestRequestTypeDef",
     {
         "DisplayName": str,
     },
     total=False,
 )
 
-
 class UpdateDomainMetadataRequestRequestTypeDef(
     _RequiredUpdateDomainMetadataRequestRequestTypeDef,
     _OptionalUpdateDomainMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateFleetMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFleetMetadataRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 _OptionalUpdateFleetMetadataRequestRequestTypeDef = TypedDict(
@@ -713,22 +565,20 @@
     {
         "DisplayName": str,
         "OptimizeForEndUserLocation": bool,
     },
     total=False,
 )
 
-
 class UpdateFleetMetadataRequestRequestTypeDef(
     _RequiredUpdateFleetMetadataRequestRequestTypeDef,
     _OptionalUpdateFleetMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateIdentityProviderConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIdentityProviderConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
         "IdentityProviderType": Literal["SAML"],
     },
 )
@@ -736,59 +586,178 @@
     "_OptionalUpdateIdentityProviderConfigurationRequestRequestTypeDef",
     {
         "IdentityProviderSamlMetadata": str,
     },
     total=False,
 )
 
-
 class UpdateIdentityProviderConfigurationRequestRequestTypeDef(
     _RequiredUpdateIdentityProviderConfigurationRequestRequestTypeDef,
     _OptionalUpdateIdentityProviderConfigurationRequestRequestTypeDef,
 ):
     pass
 
+AssociateWebsiteAuthorizationProviderResponseTypeDef = TypedDict(
+    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
+    {
+        "AuthorizationProviderId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
+    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
+    {
+        "WebsiteCaId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFleetResponseTypeDef = TypedDict(
+    "CreateFleetResponseTypeDef",
+    {
+        "FleetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAuditStreamConfigurationResponseTypeDef = TypedDict(
+    "DescribeAuditStreamConfigurationResponseTypeDef",
+    {
+        "AuditStreamArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCompanyNetworkConfigurationResponseTypeDef = TypedDict(
+    "DescribeCompanyNetworkConfigurationResponseTypeDef",
+    {
+        "VpcId": str,
+        "SubnetIds": List[str],
+        "SecurityGroupIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDevicePolicyConfigurationResponseTypeDef = TypedDict(
+    "DescribeDevicePolicyConfigurationResponseTypeDef",
+    {
+        "DeviceCaCertificate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDeviceResponseTypeDef = TypedDict(
+    "DescribeDeviceResponseTypeDef",
+    {
+        "Status": DeviceStatusType,
+        "Model": str,
+        "Manufacturer": str,
+        "OperatingSystem": str,
+        "OperatingSystemVersion": str,
+        "PatchLevel": str,
+        "FirstAccessedTime": datetime,
+        "LastAccessedTime": datetime,
+        "Username": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDomainResponseTypeDef = TypedDict(
+    "DescribeDomainResponseTypeDef",
+    {
+        "DomainName": str,
+        "DisplayName": str,
+        "CreatedTime": datetime,
+        "DomainStatus": DomainStatusType,
+        "AcmCertificateArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFleetMetadataResponseTypeDef = TypedDict(
+    "DescribeFleetMetadataResponseTypeDef",
+    {
+        "CreatedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "FleetName": str,
+        "DisplayName": str,
+        "OptimizeForEndUserLocation": bool,
+        "CompanyCode": str,
+        "FleetStatus": FleetStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeIdentityProviderConfigurationResponseTypeDef = TypedDict(
+    "DescribeIdentityProviderConfigurationResponseTypeDef",
+    {
+        "IdentityProviderType": Literal["SAML"],
+        "ServiceProviderSamlMetadata": str,
+        "IdentityProviderSamlMetadata": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
+    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
+    {
+        "Certificate": str,
+        "CreatedTime": datetime,
+        "DisplayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Domains": List[DomainSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFleetsResponseTypeDef = TypedDict(
     "ListFleetsResponseTypeDef",
     {
         "FleetSummaryList": List[FleetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWebsiteAuthorizationProvidersResponseTypeDef = TypedDict(
     "ListWebsiteAuthorizationProvidersResponseTypeDef",
     {
         "WebsiteAuthorizationProviders": List[WebsiteAuthorizationProviderSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWebsiteCertificateAuthoritiesResponseTypeDef = TypedDict(
     "ListWebsiteCertificateAuthoritiesResponseTypeDef",
     {
         "WebsiteCertificateAuthorities": List[WebsiteCaSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-worklink-1.28.0/mypy_boto3_worklink/type_defs.pyi` & `mypy-boto3-worklink-1.28.12/mypy_boto3_worklink/type_defs.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,66 +22,67 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssociateDomainRequestRequestTypeDef",
     "AssociateWebsiteAuthorizationProviderRequestRequestTypeDef",
-    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateWebsiteCertificateAuthorityRequestRequestTypeDef",
-    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
     "CreateFleetRequestRequestTypeDef",
-    "CreateFleetResponseTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DescribeAuditStreamConfigurationRequestRequestTypeDef",
-    "DescribeAuditStreamConfigurationResponseTypeDef",
     "DescribeCompanyNetworkConfigurationRequestRequestTypeDef",
-    "DescribeCompanyNetworkConfigurationResponseTypeDef",
     "DescribeDevicePolicyConfigurationRequestRequestTypeDef",
-    "DescribeDevicePolicyConfigurationResponseTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
-    "DescribeDeviceResponseTypeDef",
     "DescribeDomainRequestRequestTypeDef",
-    "DescribeDomainResponseTypeDef",
     "DescribeFleetMetadataRequestRequestTypeDef",
-    "DescribeFleetMetadataResponseTypeDef",
     "DescribeIdentityProviderConfigurationRequestRequestTypeDef",
-    "DescribeIdentityProviderConfigurationResponseTypeDef",
     "DescribeWebsiteCertificateAuthorityRequestRequestTypeDef",
-    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
     "DeviceSummaryTypeDef",
     "DisassociateDomainRequestRequestTypeDef",
     "DisassociateWebsiteAuthorizationProviderRequestRequestTypeDef",
     "DisassociateWebsiteCertificateAuthorityRequestRequestTypeDef",
     "DomainSummaryTypeDef",
     "FleetSummaryTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFleetsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListWebsiteAuthorizationProvidersRequestRequestTypeDef",
     "WebsiteAuthorizationProviderSummaryTypeDef",
     "ListWebsiteCertificateAuthoritiesRequestRequestTypeDef",
     "WebsiteCaSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreDomainAccessRequestRequestTypeDef",
     "RevokeDomainAccessRequestRequestTypeDef",
     "SignOutUserRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuditStreamConfigurationRequestRequestTypeDef",
     "UpdateCompanyNetworkConfigurationRequestRequestTypeDef",
     "UpdateDevicePolicyConfigurationRequestRequestTypeDef",
     "UpdateDomainMetadataRequestRequestTypeDef",
     "UpdateFleetMetadataRequestRequestTypeDef",
     "UpdateIdentityProviderConfigurationRequestRequestTypeDef",
+    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
+    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
+    "CreateFleetResponseTypeDef",
+    "DescribeAuditStreamConfigurationResponseTypeDef",
+    "DescribeCompanyNetworkConfigurationResponseTypeDef",
+    "DescribeDevicePolicyConfigurationResponseTypeDef",
+    "DescribeDeviceResponseTypeDef",
+    "DescribeDomainResponseTypeDef",
+    "DescribeFleetMetadataResponseTypeDef",
+    "DescribeIdentityProviderConfigurationResponseTypeDef",
+    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "ListDomainsResponseTypeDef",
     "ListFleetsResponseTypeDef",
     "ListWebsiteAuthorizationProvidersResponseTypeDef",
     "ListWebsiteCertificateAuthoritiesResponseTypeDef",
 )
 
@@ -97,19 +98,21 @@
     "_OptionalAssociateDomainRequestRequestTypeDef",
     {
         "DisplayName": str,
     },
     total=False,
 )
 
+
 class AssociateDomainRequestRequestTypeDef(
     _RequiredAssociateDomainRequestRequestTypeDef, _OptionalAssociateDomainRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredAssociateWebsiteAuthorizationProviderRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateWebsiteAuthorizationProviderRequestRequestTypeDef",
     {
         "FleetArn": str,
         "AuthorizationProviderType": Literal["SAML"],
     },
 )
@@ -117,25 +120,30 @@
     "_OptionalAssociateWebsiteAuthorizationProviderRequestRequestTypeDef",
     {
         "DomainName": str,
     },
     total=False,
 )
 
+
 class AssociateWebsiteAuthorizationProviderRequestRequestTypeDef(
     _RequiredAssociateWebsiteAuthorizationProviderRequestRequestTypeDef,
     _OptionalAssociateWebsiteAuthorizationProviderRequestRequestTypeDef,
 ):
     pass
 
-AssociateWebsiteAuthorizationProviderResponseTypeDef = TypedDict(
-    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AuthorizationProviderId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredAssociateWebsiteCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateWebsiteCertificateAuthorityRequestRequestTypeDef",
     {
         "FleetArn": str,
@@ -146,27 +154,21 @@
     "_OptionalAssociateWebsiteCertificateAuthorityRequestRequestTypeDef",
     {
         "DisplayName": str,
     },
     total=False,
 )
 
+
 class AssociateWebsiteCertificateAuthorityRequestRequestTypeDef(
     _RequiredAssociateWebsiteCertificateAuthorityRequestRequestTypeDef,
     _OptionalAssociateWebsiteCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
-AssociateWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
-    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
-    {
-        "WebsiteCaId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreateFleetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFleetRequestRequestTypeDef",
     {
         "FleetName": str,
     },
 )
@@ -176,26 +178,20 @@
         "DisplayName": str,
         "OptimizeForEndUserLocation": bool,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateFleetRequestRequestTypeDef(
     _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
 ):
     pass
 
-CreateFleetResponseTypeDef = TypedDict(
-    "CreateFleetResponseTypeDef",
-    {
-        "FleetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeleteFleetRequestRequestTypeDef = TypedDict(
     "DeleteFleetRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
@@ -203,155 +199,66 @@
 DescribeAuditStreamConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeAuditStreamConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
-DescribeAuditStreamConfigurationResponseTypeDef = TypedDict(
-    "DescribeAuditStreamConfigurationResponseTypeDef",
-    {
-        "AuditStreamArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeCompanyNetworkConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeCompanyNetworkConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
-DescribeCompanyNetworkConfigurationResponseTypeDef = TypedDict(
-    "DescribeCompanyNetworkConfigurationResponseTypeDef",
-    {
-        "VpcId": str,
-        "SubnetIds": List[str],
-        "SecurityGroupIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDevicePolicyConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeDevicePolicyConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
-DescribeDevicePolicyConfigurationResponseTypeDef = TypedDict(
-    "DescribeDevicePolicyConfigurationResponseTypeDef",
-    {
-        "DeviceCaCertificate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDeviceRequestRequestTypeDef = TypedDict(
     "DescribeDeviceRequestRequestTypeDef",
     {
         "FleetArn": str,
         "DeviceId": str,
     },
 )
 
-DescribeDeviceResponseTypeDef = TypedDict(
-    "DescribeDeviceResponseTypeDef",
-    {
-        "Status": DeviceStatusType,
-        "Model": str,
-        "Manufacturer": str,
-        "OperatingSystem": str,
-        "OperatingSystemVersion": str,
-        "PatchLevel": str,
-        "FirstAccessedTime": datetime,
-        "LastAccessedTime": datetime,
-        "Username": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDomainRequestRequestTypeDef = TypedDict(
     "DescribeDomainRequestRequestTypeDef",
     {
         "FleetArn": str,
         "DomainName": str,
     },
 )
 
-DescribeDomainResponseTypeDef = TypedDict(
-    "DescribeDomainResponseTypeDef",
-    {
-        "DomainName": str,
-        "DisplayName": str,
-        "CreatedTime": datetime,
-        "DomainStatus": DomainStatusType,
-        "AcmCertificateArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeFleetMetadataRequestRequestTypeDef = TypedDict(
     "DescribeFleetMetadataRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
-DescribeFleetMetadataResponseTypeDef = TypedDict(
-    "DescribeFleetMetadataResponseTypeDef",
-    {
-        "CreatedTime": datetime,
-        "LastUpdatedTime": datetime,
-        "FleetName": str,
-        "DisplayName": str,
-        "OptimizeForEndUserLocation": bool,
-        "CompanyCode": str,
-        "FleetStatus": FleetStatusType,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeIdentityProviderConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeIdentityProviderConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
-DescribeIdentityProviderConfigurationResponseTypeDef = TypedDict(
-    "DescribeIdentityProviderConfigurationResponseTypeDef",
-    {
-        "IdentityProviderType": Literal["SAML"],
-        "ServiceProviderSamlMetadata": str,
-        "IdentityProviderSamlMetadata": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeWebsiteCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "DescribeWebsiteCertificateAuthorityRequestRequestTypeDef",
     {
         "FleetArn": str,
         "WebsiteCaId": str,
     },
 )
 
-DescribeWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
-    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
-    {
-        "Certificate": str,
-        "CreatedTime": datetime,
-        "DisplayName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeviceSummaryTypeDef = TypedDict(
     "DeviceSummaryTypeDef",
     {
         "DeviceId": str,
         "DeviceStatus": DeviceStatusType,
     },
     total=False,
@@ -393,17 +300,19 @@
     "_OptionalDomainSummaryTypeDef",
     {
         "DisplayName": str,
     },
     total=False,
 )
 
+
 class DomainSummaryTypeDef(_RequiredDomainSummaryTypeDef, _OptionalDomainSummaryTypeDef):
     pass
 
+
 FleetSummaryTypeDef = TypedDict(
     "FleetSummaryTypeDef",
     {
         "FleetArn": str,
         "CreatedTime": datetime,
         "LastUpdatedTime": datetime,
         "FleetName": str,
@@ -426,19 +335,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListDevicesRequestRequestTypeDef(
     _RequiredListDevicesRequestRequestTypeDef, _OptionalListDevicesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListDomainsRequestRequestTypeDef = TypedDict(
     "_RequiredListDomainsRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 _OptionalListDomainsRequestRequestTypeDef = TypedDict(
@@ -446,19 +357,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListDomainsRequestRequestTypeDef(
     _RequiredListDomainsRequestRequestTypeDef, _OptionalListDomainsRequestRequestTypeDef
 ):
     pass
 
+
 ListFleetsRequestRequestTypeDef = TypedDict(
     "ListFleetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -467,22 +380,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListWebsiteAuthorizationProvidersRequestRequestTypeDef = TypedDict(
     "_RequiredListWebsiteAuthorizationProvidersRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 _OptionalListWebsiteAuthorizationProvidersRequestRequestTypeDef = TypedDict(
@@ -490,20 +395,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListWebsiteAuthorizationProvidersRequestRequestTypeDef(
     _RequiredListWebsiteAuthorizationProvidersRequestRequestTypeDef,
     _OptionalListWebsiteAuthorizationProvidersRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredWebsiteAuthorizationProviderSummaryTypeDef = TypedDict(
     "_RequiredWebsiteAuthorizationProviderSummaryTypeDef",
     {
         "AuthorizationProviderType": Literal["SAML"],
     },
 )
 _OptionalWebsiteAuthorizationProviderSummaryTypeDef = TypedDict(
@@ -512,20 +419,22 @@
         "AuthorizationProviderId": str,
         "DomainName": str,
         "CreatedTime": datetime,
     },
     total=False,
 )
 
+
 class WebsiteAuthorizationProviderSummaryTypeDef(
     _RequiredWebsiteAuthorizationProviderSummaryTypeDef,
     _OptionalWebsiteAuthorizationProviderSummaryTypeDef,
 ):
     pass
 
+
 _RequiredListWebsiteCertificateAuthoritiesRequestRequestTypeDef = TypedDict(
     "_RequiredListWebsiteCertificateAuthoritiesRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 _OptionalListWebsiteCertificateAuthoritiesRequestRequestTypeDef = TypedDict(
@@ -533,41 +442,32 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListWebsiteCertificateAuthoritiesRequestRequestTypeDef(
     _RequiredListWebsiteCertificateAuthoritiesRequestRequestTypeDef,
     _OptionalListWebsiteCertificateAuthoritiesRequestRequestTypeDef,
 ):
     pass
 
+
 WebsiteCaSummaryTypeDef = TypedDict(
     "WebsiteCaSummaryTypeDef",
     {
         "WebsiteCaId": str,
         "CreatedTime": datetime,
         "DisplayName": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 RestoreDomainAccessRequestRequestTypeDef = TypedDict(
     "RestoreDomainAccessRequestRequestTypeDef",
     {
         "FleetArn": str,
         "DomainName": str,
     },
 )
@@ -614,20 +514,22 @@
     "_OptionalUpdateAuditStreamConfigurationRequestRequestTypeDef",
     {
         "AuditStreamArn": str,
     },
     total=False,
 )
 
+
 class UpdateAuditStreamConfigurationRequestRequestTypeDef(
     _RequiredUpdateAuditStreamConfigurationRequestRequestTypeDef,
     _OptionalUpdateAuditStreamConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateCompanyNetworkConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateCompanyNetworkConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
         "VpcId": str,
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
@@ -644,20 +546,22 @@
     "_OptionalUpdateDevicePolicyConfigurationRequestRequestTypeDef",
     {
         "DeviceCaCertificate": str,
     },
     total=False,
 )
 
+
 class UpdateDevicePolicyConfigurationRequestRequestTypeDef(
     _RequiredUpdateDevicePolicyConfigurationRequestRequestTypeDef,
     _OptionalUpdateDevicePolicyConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateDomainMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDomainMetadataRequestRequestTypeDef",
     {
         "FleetArn": str,
         "DomainName": str,
     },
 )
@@ -665,20 +569,22 @@
     "_OptionalUpdateDomainMetadataRequestRequestTypeDef",
     {
         "DisplayName": str,
     },
     total=False,
 )
 
+
 class UpdateDomainMetadataRequestRequestTypeDef(
     _RequiredUpdateDomainMetadataRequestRequestTypeDef,
     _OptionalUpdateDomainMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateFleetMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFleetMetadataRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 _OptionalUpdateFleetMetadataRequestRequestTypeDef = TypedDict(
@@ -686,20 +592,22 @@
     {
         "DisplayName": str,
         "OptimizeForEndUserLocation": bool,
     },
     total=False,
 )
 
+
 class UpdateFleetMetadataRequestRequestTypeDef(
     _RequiredUpdateFleetMetadataRequestRequestTypeDef,
     _OptionalUpdateFleetMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateIdentityProviderConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIdentityProviderConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
         "IdentityProviderType": Literal["SAML"],
     },
 )
@@ -707,57 +615,180 @@
     "_OptionalUpdateIdentityProviderConfigurationRequestRequestTypeDef",
     {
         "IdentityProviderSamlMetadata": str,
     },
     total=False,
 )
 
+
 class UpdateIdentityProviderConfigurationRequestRequestTypeDef(
     _RequiredUpdateIdentityProviderConfigurationRequestRequestTypeDef,
     _OptionalUpdateIdentityProviderConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
+AssociateWebsiteAuthorizationProviderResponseTypeDef = TypedDict(
+    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
+    {
+        "AuthorizationProviderId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
+    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
+    {
+        "WebsiteCaId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFleetResponseTypeDef = TypedDict(
+    "CreateFleetResponseTypeDef",
+    {
+        "FleetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAuditStreamConfigurationResponseTypeDef = TypedDict(
+    "DescribeAuditStreamConfigurationResponseTypeDef",
+    {
+        "AuditStreamArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCompanyNetworkConfigurationResponseTypeDef = TypedDict(
+    "DescribeCompanyNetworkConfigurationResponseTypeDef",
+    {
+        "VpcId": str,
+        "SubnetIds": List[str],
+        "SecurityGroupIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDevicePolicyConfigurationResponseTypeDef = TypedDict(
+    "DescribeDevicePolicyConfigurationResponseTypeDef",
+    {
+        "DeviceCaCertificate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDeviceResponseTypeDef = TypedDict(
+    "DescribeDeviceResponseTypeDef",
+    {
+        "Status": DeviceStatusType,
+        "Model": str,
+        "Manufacturer": str,
+        "OperatingSystem": str,
+        "OperatingSystemVersion": str,
+        "PatchLevel": str,
+        "FirstAccessedTime": datetime,
+        "LastAccessedTime": datetime,
+        "Username": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDomainResponseTypeDef = TypedDict(
+    "DescribeDomainResponseTypeDef",
+    {
+        "DomainName": str,
+        "DisplayName": str,
+        "CreatedTime": datetime,
+        "DomainStatus": DomainStatusType,
+        "AcmCertificateArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFleetMetadataResponseTypeDef = TypedDict(
+    "DescribeFleetMetadataResponseTypeDef",
+    {
+        "CreatedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "FleetName": str,
+        "DisplayName": str,
+        "OptimizeForEndUserLocation": bool,
+        "CompanyCode": str,
+        "FleetStatus": FleetStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeIdentityProviderConfigurationResponseTypeDef = TypedDict(
+    "DescribeIdentityProviderConfigurationResponseTypeDef",
+    {
+        "IdentityProviderType": Literal["SAML"],
+        "ServiceProviderSamlMetadata": str,
+        "IdentityProviderSamlMetadata": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
+    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
+    {
+        "Certificate": str,
+        "CreatedTime": datetime,
+        "DisplayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Domains": List[DomainSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFleetsResponseTypeDef = TypedDict(
     "ListFleetsResponseTypeDef",
     {
         "FleetSummaryList": List[FleetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWebsiteAuthorizationProvidersResponseTypeDef = TypedDict(
     "ListWebsiteAuthorizationProvidersResponseTypeDef",
     {
         "WebsiteAuthorizationProviders": List[WebsiteAuthorizationProviderSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWebsiteCertificateAuthoritiesResponseTypeDef = TypedDict(
     "ListWebsiteCertificateAuthoritiesResponseTypeDef",
     {
         "WebsiteCertificateAuthorities": List[WebsiteCaSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-worklink-1.28.0/mypy_boto3_worklink.egg-info/PKG-INFO` & `mypy-boto3-worklink-1.28.12/mypy_boto3_worklink.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-worklink
-Version: 1.28.0
-Summary: Type annotations for boto3.WorkLink 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.WorkLink 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_worklink/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-worklink"></a>
 
 # mypy-boto3-worklink
 
 [![PyPI - mypy-boto3-worklink](https://img.shields.io/pypi/v/mypy-boto3-worklink.svg?color=blue)](https://pypi.org/project/mypy-boto3-worklink)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-worklink.svg?color=blue)](https://pypi.org/project/mypy-boto3-worklink)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_worklink/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-worklink?color=blue)](https://pypistats.org/packages/mypy-boto3-worklink)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-worklink)](https://pepy.tech/project/mypy-boto3-worklink)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkLink 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
+[boto3.WorkLink 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
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
 [mypy-boto3-worklink docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_worklink/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,63 +301,63 @@
 `mypy_boto3_worklink.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_worklink.type_defs import (
     AssociateDomainRequestRequestTypeDef,
     AssociateWebsiteAuthorizationProviderRequestRequestTypeDef,
-    AssociateWebsiteAuthorizationProviderResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociateWebsiteCertificateAuthorityRequestRequestTypeDef,
-    AssociateWebsiteCertificateAuthorityResponseTypeDef,
     CreateFleetRequestRequestTypeDef,
-    CreateFleetResponseTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DescribeAuditStreamConfigurationRequestRequestTypeDef,
-    DescribeAuditStreamConfigurationResponseTypeDef,
     DescribeCompanyNetworkConfigurationRequestRequestTypeDef,
-    DescribeCompanyNetworkConfigurationResponseTypeDef,
     DescribeDevicePolicyConfigurationRequestRequestTypeDef,
-    DescribeDevicePolicyConfigurationResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
-    DescribeDeviceResponseTypeDef,
     DescribeDomainRequestRequestTypeDef,
-    DescribeDomainResponseTypeDef,
     DescribeFleetMetadataRequestRequestTypeDef,
-    DescribeFleetMetadataResponseTypeDef,
     DescribeIdentityProviderConfigurationRequestRequestTypeDef,
-    DescribeIdentityProviderConfigurationResponseTypeDef,
     DescribeWebsiteCertificateAuthorityRequestRequestTypeDef,
-    DescribeWebsiteCertificateAuthorityResponseTypeDef,
     DeviceSummaryTypeDef,
     DisassociateDomainRequestRequestTypeDef,
     DisassociateWebsiteAuthorizationProviderRequestRequestTypeDef,
     DisassociateWebsiteCertificateAuthorityRequestRequestTypeDef,
     DomainSummaryTypeDef,
     FleetSummaryTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFleetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWebsiteAuthorizationProvidersRequestRequestTypeDef,
     WebsiteAuthorizationProviderSummaryTypeDef,
     ListWebsiteCertificateAuthoritiesRequestRequestTypeDef,
     WebsiteCaSummaryTypeDef,
-    ResponseMetadataTypeDef,
     RestoreDomainAccessRequestRequestTypeDef,
     RevokeDomainAccessRequestRequestTypeDef,
     SignOutUserRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuditStreamConfigurationRequestRequestTypeDef,
     UpdateCompanyNetworkConfigurationRequestRequestTypeDef,
     UpdateDevicePolicyConfigurationRequestRequestTypeDef,
     UpdateDomainMetadataRequestRequestTypeDef,
     UpdateFleetMetadataRequestRequestTypeDef,
     UpdateIdentityProviderConfigurationRequestRequestTypeDef,
+    AssociateWebsiteAuthorizationProviderResponseTypeDef,
+    AssociateWebsiteCertificateAuthorityResponseTypeDef,
+    CreateFleetResponseTypeDef,
+    DescribeAuditStreamConfigurationResponseTypeDef,
+    DescribeCompanyNetworkConfigurationResponseTypeDef,
+    DescribeDevicePolicyConfigurationResponseTypeDef,
+    DescribeDeviceResponseTypeDef,
+    DescribeDomainResponseTypeDef,
+    DescribeFleetMetadataResponseTypeDef,
+    DescribeIdentityProviderConfigurationResponseTypeDef,
+    DescribeWebsiteCertificateAuthorityResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListDevicesResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListFleetsResponseTypeDef,
     ListWebsiteAuthorizationProvidersResponseTypeDef,
     ListWebsiteCertificateAuthoritiesResponseTypeDef,
 )
```

### Comparing `mypy-boto3-worklink-1.28.0/mypy_boto3_worklink.egg-info/SOURCES.txt` & `mypy-boto3-worklink-1.28.12/mypy_boto3_worklink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-worklink-1.28.0/setup.py` & `mypy-boto3-worklink-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-worklink",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_worklink"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WorkLink 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.WorkLink 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

