# Comparing `tmp/mypy-boto3-workspaces-web-1.28.0.tar.gz` & `tmp/mypy-boto3-workspaces-web-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workspaces-web-1.28.0.tar", last modified: Thu Jul  6 21:00:53 2023, max compression
+gzip compressed data, was "mypy-boto3-workspaces-web-1.28.12.tar", last modified: Thu Jul 27 11:49:51 2023, max compression
```

## Comparing `mypy-boto3-workspaces-web-1.28.0.tar` & `mypy-boto3-workspaces-web-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:53.054463 mypy-boto3-workspaces-web-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:58:25.000000 mypy-boto3-workspaces-web-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17452 2023-07-06 21:00:53.038462 mypy-boto3-workspaces-web-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-07-06 20:58:25.000000 mypy-boto3-workspaces-web-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:53.038462 mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-06 20:58:25.000000 mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-06 20:58:25.000000 mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-06 20:58:25.000000 mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37970 2023-07-06 20:58:25.000000 mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37906 2023-07-06 20:58:25.000000 mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-06 20:58:26.000000 mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-07-06 20:58:26.000000 mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:25.000000 mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41390 2023-07-06 20:58:27.000000 mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41339 2023-07-06 20:58:26.000000 mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:58:25.000000 mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:53.038462 mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17452 2023-07-06 21:00:52.000000 mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-06 21:00:52.000000 mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:52.000000 mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:52.000000 mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:52.000000 mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 21:00:52.000000 mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:53.054463 mypy-boto3-workspaces-web-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-06 20:58:25.000000 mypy-boto3-workspaces-web-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:51.197507 mypy-boto3-workspaces-web-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:49:02.000000 mypy-boto3-workspaces-web-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17486 2023-07-27 11:49:51.197507 mypy-boto3-workspaces-web-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15972 2023-07-27 11:49:02.000000 mypy-boto3-workspaces-web-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:51.197507 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-27 11:49:02.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-27 11:49:02.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 11:49:02.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37970 2023-07-27 11:49:03.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37906 2023-07-27 11:49:03.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-07-27 11:49:03.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-07-27 11:49:03.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:02.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41836 2023-07-27 11:49:04.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41783 2023-07-27 11:49:03.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:49:02.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:51.197507 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17486 2023-07-27 11:49:51.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-27 11:49:51.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:51.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:51.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:51.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 11:49:51.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:51.197507 mypy-boto3-workspaces-web-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-27 11:49:02.000000 mypy-boto3-workspaces-web-1.28.12/setup.py
```

### Comparing `mypy-boto3-workspaces-web-1.28.0/LICENSE` & `mypy-boto3-workspaces-web-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-web-1.28.0/PKG-INFO` & `mypy-boto3-workspaces-web-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces-web
-Version: 1.28.0
-Summary: Type annotations for boto3.WorkSpacesWeb 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.WorkSpacesWeb 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-workspaces-web"></a>
 
 # mypy-boto3-workspaces-web
 
 [![PyPI - mypy-boto3-workspaces-web](https://img.shields.io/pypi/v/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces-web?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces-web)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces-web)](https://pepy.tech/project/mypy-boto3-workspaces-web)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpacesWeb 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
+[boto3.WorkSpacesWeb 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
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
 [mypy-boto3-workspaces-web docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,40 +304,27 @@
 
 `mypy_boto3_workspaces_web.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workspaces_web.type_defs import (
     AssociateBrowserSettingsRequestRequestTypeDef,
-    AssociateBrowserSettingsResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociateIpAccessSettingsRequestRequestTypeDef,
-    AssociateIpAccessSettingsResponseTypeDef,
     AssociateNetworkSettingsRequestRequestTypeDef,
-    AssociateNetworkSettingsResponseTypeDef,
     AssociateTrustStoreRequestRequestTypeDef,
-    AssociateTrustStoreResponseTypeDef,
     AssociateUserAccessLoggingSettingsRequestRequestTypeDef,
-    AssociateUserAccessLoggingSettingsResponseTypeDef,
     AssociateUserSettingsRequestRequestTypeDef,
-    AssociateUserSettingsResponseTypeDef,
     BrowserSettingsSummaryTypeDef,
     BrowserSettingsTypeDef,
     CertificateSummaryTypeDef,
     CertificateTypeDef,
     TagTypeDef,
-    CreateBrowserSettingsResponseTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
-    CreateIdentityProviderResponseTypeDef,
     IpRuleTypeDef,
-    CreateIpAccessSettingsResponseTypeDef,
-    CreateNetworkSettingsResponseTypeDef,
-    CreatePortalResponseTypeDef,
-    CreateTrustStoreResponseTypeDef,
-    CreateUserAccessLoggingSettingsResponseTypeDef,
-    CreateUserSettingsResponseTypeDef,
     DeleteBrowserSettingsRequestRequestTypeDef,
     DeleteIdentityProviderRequestRequestTypeDef,
     DeleteIpAccessSettingsRequestRequestTypeDef,
     DeleteNetworkSettingsRequestRequestTypeDef,
     DeletePortalRequestRequestTypeDef,
     DeleteTrustStoreRequestRequestTypeDef,
     DeleteUserAccessLoggingSettingsRequestRequestTypeDef,
@@ -353,80 +340,95 @@
     IdentityProviderTypeDef,
     GetIpAccessSettingsRequestRequestTypeDef,
     GetNetworkSettingsRequestRequestTypeDef,
     NetworkSettingsTypeDef,
     GetPortalRequestRequestTypeDef,
     PortalTypeDef,
     GetPortalServiceProviderMetadataRequestRequestTypeDef,
-    GetPortalServiceProviderMetadataResponseTypeDef,
     GetTrustStoreCertificateRequestRequestTypeDef,
     GetTrustStoreRequestRequestTypeDef,
     TrustStoreTypeDef,
     GetUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsTypeDef,
     GetUserSettingsRequestRequestTypeDef,
     UserSettingsTypeDef,
     IdentityProviderSummaryTypeDef,
     IpAccessSettingsSummaryTypeDef,
+    IpRuleOutputTypeDef,
     ListBrowserSettingsRequestRequestTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
     ListIpAccessSettingsRequestRequestTypeDef,
     ListNetworkSettingsRequestRequestTypeDef,
     NetworkSettingsSummaryTypeDef,
     ListPortalsRequestRequestTypeDef,
     PortalSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListTrustStoreCertificatesRequestRequestTypeDef,
     ListTrustStoresRequestRequestTypeDef,
     TrustStoreSummaryTypeDef,
     ListUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsSummaryTypeDef,
     ListUserSettingsRequestRequestTypeDef,
     UserSettingsSummaryTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrowserSettingsRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
     UpdateNetworkSettingsRequestRequestTypeDef,
     UpdatePortalRequestRequestTypeDef,
     UpdateTrustStoreRequestRequestTypeDef,
-    UpdateTrustStoreResponseTypeDef,
     UpdateUserAccessLoggingSettingsRequestRequestTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
+    AssociateBrowserSettingsResponseTypeDef,
+    AssociateIpAccessSettingsResponseTypeDef,
+    AssociateNetworkSettingsResponseTypeDef,
+    AssociateTrustStoreResponseTypeDef,
+    AssociateUserAccessLoggingSettingsResponseTypeDef,
+    AssociateUserSettingsResponseTypeDef,
+    CreateBrowserSettingsResponseTypeDef,
+    CreateIdentityProviderResponseTypeDef,
+    CreateIpAccessSettingsResponseTypeDef,
+    CreateNetworkSettingsResponseTypeDef,
+    CreatePortalResponseTypeDef,
+    CreateTrustStoreResponseTypeDef,
+    CreateUserAccessLoggingSettingsResponseTypeDef,
+    CreateUserSettingsResponseTypeDef,
+    GetPortalServiceProviderMetadataResponseTypeDef,
+    UpdateTrustStoreResponseTypeDef,
     ListBrowserSettingsResponseTypeDef,
     GetBrowserSettingsResponseTypeDef,
     UpdateBrowserSettingsResponseTypeDef,
     ListTrustStoreCertificatesResponseTypeDef,
     GetTrustStoreCertificateResponseTypeDef,
     CreateBrowserSettingsRequestRequestTypeDef,
     CreateNetworkSettingsRequestRequestTypeDef,
     CreatePortalRequestRequestTypeDef,
     CreateTrustStoreRequestRequestTypeDef,
     CreateUserAccessLoggingSettingsRequestRequestTypeDef,
     CreateUserSettingsRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIpAccessSettingsRequestRequestTypeDef,
-    IpAccessSettingsTypeDef,
     UpdateIpAccessSettingsRequestRequestTypeDef,
     GetIdentityProviderResponseTypeDef,
     UpdateIdentityProviderResponseTypeDef,
     GetNetworkSettingsResponseTypeDef,
     UpdateNetworkSettingsResponseTypeDef,
     GetPortalResponseTypeDef,
     UpdatePortalResponseTypeDef,
     GetTrustStoreResponseTypeDef,
     GetUserAccessLoggingSettingsResponseTypeDef,
     UpdateUserAccessLoggingSettingsResponseTypeDef,
     GetUserSettingsResponseTypeDef,
     UpdateUserSettingsResponseTypeDef,
     ListIdentityProvidersResponseTypeDef,
     ListIpAccessSettingsResponseTypeDef,
+    IpAccessSettingsTypeDef,
     ListNetworkSettingsResponseTypeDef,
     ListPortalsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTrustStoresResponseTypeDef,
     ListUserAccessLoggingSettingsResponseTypeDef,
     ListUserSettingsResponseTypeDef,
     GetIpAccessSettingsResponseTypeDef,
     UpdateIpAccessSettingsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-workspaces-web-1.28.0/README.md` & `mypy-boto3-workspaces-web-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-workspaces-web"></a>
 
 # mypy-boto3-workspaces-web
 
 [![PyPI - mypy-boto3-workspaces-web](https://img.shields.io/pypi/v/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces-web?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces-web)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces-web)](https://pepy.tech/project/mypy-boto3-workspaces-web)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpacesWeb 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
+[boto3.WorkSpacesWeb 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
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
 [mypy-boto3-workspaces-web docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/).
 
 See how it helps to find and fix potential bugs:
 
@@ -272,40 +272,27 @@
 
 `mypy_boto3_workspaces_web.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workspaces_web.type_defs import (
     AssociateBrowserSettingsRequestRequestTypeDef,
-    AssociateBrowserSettingsResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociateIpAccessSettingsRequestRequestTypeDef,
-    AssociateIpAccessSettingsResponseTypeDef,
     AssociateNetworkSettingsRequestRequestTypeDef,
-    AssociateNetworkSettingsResponseTypeDef,
     AssociateTrustStoreRequestRequestTypeDef,
-    AssociateTrustStoreResponseTypeDef,
     AssociateUserAccessLoggingSettingsRequestRequestTypeDef,
-    AssociateUserAccessLoggingSettingsResponseTypeDef,
     AssociateUserSettingsRequestRequestTypeDef,
-    AssociateUserSettingsResponseTypeDef,
     BrowserSettingsSummaryTypeDef,
     BrowserSettingsTypeDef,
     CertificateSummaryTypeDef,
     CertificateTypeDef,
     TagTypeDef,
-    CreateBrowserSettingsResponseTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
-    CreateIdentityProviderResponseTypeDef,
     IpRuleTypeDef,
-    CreateIpAccessSettingsResponseTypeDef,
-    CreateNetworkSettingsResponseTypeDef,
-    CreatePortalResponseTypeDef,
-    CreateTrustStoreResponseTypeDef,
-    CreateUserAccessLoggingSettingsResponseTypeDef,
-    CreateUserSettingsResponseTypeDef,
     DeleteBrowserSettingsRequestRequestTypeDef,
     DeleteIdentityProviderRequestRequestTypeDef,
     DeleteIpAccessSettingsRequestRequestTypeDef,
     DeleteNetworkSettingsRequestRequestTypeDef,
     DeletePortalRequestRequestTypeDef,
     DeleteTrustStoreRequestRequestTypeDef,
     DeleteUserAccessLoggingSettingsRequestRequestTypeDef,
@@ -321,80 +308,95 @@
     IdentityProviderTypeDef,
     GetIpAccessSettingsRequestRequestTypeDef,
     GetNetworkSettingsRequestRequestTypeDef,
     NetworkSettingsTypeDef,
     GetPortalRequestRequestTypeDef,
     PortalTypeDef,
     GetPortalServiceProviderMetadataRequestRequestTypeDef,
-    GetPortalServiceProviderMetadataResponseTypeDef,
     GetTrustStoreCertificateRequestRequestTypeDef,
     GetTrustStoreRequestRequestTypeDef,
     TrustStoreTypeDef,
     GetUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsTypeDef,
     GetUserSettingsRequestRequestTypeDef,
     UserSettingsTypeDef,
     IdentityProviderSummaryTypeDef,
     IpAccessSettingsSummaryTypeDef,
+    IpRuleOutputTypeDef,
     ListBrowserSettingsRequestRequestTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
     ListIpAccessSettingsRequestRequestTypeDef,
     ListNetworkSettingsRequestRequestTypeDef,
     NetworkSettingsSummaryTypeDef,
     ListPortalsRequestRequestTypeDef,
     PortalSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListTrustStoreCertificatesRequestRequestTypeDef,
     ListTrustStoresRequestRequestTypeDef,
     TrustStoreSummaryTypeDef,
     ListUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsSummaryTypeDef,
     ListUserSettingsRequestRequestTypeDef,
     UserSettingsSummaryTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrowserSettingsRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
     UpdateNetworkSettingsRequestRequestTypeDef,
     UpdatePortalRequestRequestTypeDef,
     UpdateTrustStoreRequestRequestTypeDef,
-    UpdateTrustStoreResponseTypeDef,
     UpdateUserAccessLoggingSettingsRequestRequestTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
+    AssociateBrowserSettingsResponseTypeDef,
+    AssociateIpAccessSettingsResponseTypeDef,
+    AssociateNetworkSettingsResponseTypeDef,
+    AssociateTrustStoreResponseTypeDef,
+    AssociateUserAccessLoggingSettingsResponseTypeDef,
+    AssociateUserSettingsResponseTypeDef,
+    CreateBrowserSettingsResponseTypeDef,
+    CreateIdentityProviderResponseTypeDef,
+    CreateIpAccessSettingsResponseTypeDef,
+    CreateNetworkSettingsResponseTypeDef,
+    CreatePortalResponseTypeDef,
+    CreateTrustStoreResponseTypeDef,
+    CreateUserAccessLoggingSettingsResponseTypeDef,
+    CreateUserSettingsResponseTypeDef,
+    GetPortalServiceProviderMetadataResponseTypeDef,
+    UpdateTrustStoreResponseTypeDef,
     ListBrowserSettingsResponseTypeDef,
     GetBrowserSettingsResponseTypeDef,
     UpdateBrowserSettingsResponseTypeDef,
     ListTrustStoreCertificatesResponseTypeDef,
     GetTrustStoreCertificateResponseTypeDef,
     CreateBrowserSettingsRequestRequestTypeDef,
     CreateNetworkSettingsRequestRequestTypeDef,
     CreatePortalRequestRequestTypeDef,
     CreateTrustStoreRequestRequestTypeDef,
     CreateUserAccessLoggingSettingsRequestRequestTypeDef,
     CreateUserSettingsRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIpAccessSettingsRequestRequestTypeDef,
-    IpAccessSettingsTypeDef,
     UpdateIpAccessSettingsRequestRequestTypeDef,
     GetIdentityProviderResponseTypeDef,
     UpdateIdentityProviderResponseTypeDef,
     GetNetworkSettingsResponseTypeDef,
     UpdateNetworkSettingsResponseTypeDef,
     GetPortalResponseTypeDef,
     UpdatePortalResponseTypeDef,
     GetTrustStoreResponseTypeDef,
     GetUserAccessLoggingSettingsResponseTypeDef,
     UpdateUserAccessLoggingSettingsResponseTypeDef,
     GetUserSettingsResponseTypeDef,
     UpdateUserSettingsResponseTypeDef,
     ListIdentityProvidersResponseTypeDef,
     ListIpAccessSettingsResponseTypeDef,
+    IpAccessSettingsTypeDef,
     ListNetworkSettingsResponseTypeDef,
     ListPortalsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTrustStoresResponseTypeDef,
     ListUserAccessLoggingSettingsResponseTypeDef,
     ListUserSettingsResponseTypeDef,
     GetIpAccessSettingsResponseTypeDef,
     UpdateIpAccessSettingsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web/__main__.py` & `mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkSpacesWeb 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.WorkSpacesWeb 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb\nOther"
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

### Comparing `mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web/client.py` & `mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web/client.pyi` & `mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web/literals.py` & `mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,29 +14,27 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AuthenticationTypeType",
     "BrowserTypeType",
     "EnabledTypeType",
     "IdentityProviderTypeType",
     "PortalStatusType",
     "RendererTypeType",
     "WorkSpacesWebServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AuthenticationTypeType = Literal["IAM_Identity_Center", "Standard"]
 BrowserTypeType = Literal["Chrome"]
 EnabledTypeType = Literal["Disabled", "Enabled"]
 IdentityProviderTypeType = Literal[
     "Facebook", "Google", "LoginWithAmazon", "OIDC", "SAML", "SignInWithApple"
 ]
 PortalStatusType = Literal["Active", "Incomplete", "Pending"]
@@ -157,14 +155,15 @@
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
@@ -243,26 +242,28 @@
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

### Comparing `mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web/literals.pyi` & `mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,27 +14,29 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AuthenticationTypeType",
     "BrowserTypeType",
     "EnabledTypeType",
     "IdentityProviderTypeType",
     "PortalStatusType",
     "RendererTypeType",
     "WorkSpacesWebServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 AuthenticationTypeType = Literal["IAM_Identity_Center", "Standard"]
 BrowserTypeType = Literal["Chrome"]
 EnabledTypeType = Literal["Disabled", "Enabled"]
 IdentityProviderTypeType = Literal[
     "Facebook", "Google", "LoginWithAmazon", "OIDC", "SAML", "SignInWithApple"
 ]
 PortalStatusType = Literal["Active", "Incomplete", "Pending"]
@@ -155,14 +157,15 @@
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
@@ -241,26 +244,28 @@
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

### Comparing `mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web/type_defs.py` & `mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,43 +29,29 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateBrowserSettingsRequestRequestTypeDef",
-    "AssociateBrowserSettingsResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateIpAccessSettingsRequestRequestTypeDef",
-    "AssociateIpAccessSettingsResponseTypeDef",
     "AssociateNetworkSettingsRequestRequestTypeDef",
-    "AssociateNetworkSettingsResponseTypeDef",
     "AssociateTrustStoreRequestRequestTypeDef",
-    "AssociateTrustStoreResponseTypeDef",
     "AssociateUserAccessLoggingSettingsRequestRequestTypeDef",
-    "AssociateUserAccessLoggingSettingsResponseTypeDef",
     "AssociateUserSettingsRequestRequestTypeDef",
-    "AssociateUserSettingsResponseTypeDef",
     "BrowserSettingsSummaryTypeDef",
     "BrowserSettingsTypeDef",
     "CertificateSummaryTypeDef",
     "CertificateTypeDef",
     "TagTypeDef",
-    "CreateBrowserSettingsResponseTypeDef",
     "CreateIdentityProviderRequestRequestTypeDef",
-    "CreateIdentityProviderResponseTypeDef",
     "IpRuleTypeDef",
-    "CreateIpAccessSettingsResponseTypeDef",
-    "CreateNetworkSettingsResponseTypeDef",
-    "CreatePortalResponseTypeDef",
-    "CreateTrustStoreResponseTypeDef",
-    "CreateUserAccessLoggingSettingsResponseTypeDef",
-    "CreateUserSettingsResponseTypeDef",
     "DeleteBrowserSettingsRequestRequestTypeDef",
     "DeleteIdentityProviderRequestRequestTypeDef",
     "DeleteIpAccessSettingsRequestRequestTypeDef",
     "DeleteNetworkSettingsRequestRequestTypeDef",
     "DeletePortalRequestRequestTypeDef",
     "DeleteTrustStoreRequestRequestTypeDef",
     "DeleteUserAccessLoggingSettingsRequestRequestTypeDef",
@@ -81,80 +67,95 @@
     "IdentityProviderTypeDef",
     "GetIpAccessSettingsRequestRequestTypeDef",
     "GetNetworkSettingsRequestRequestTypeDef",
     "NetworkSettingsTypeDef",
     "GetPortalRequestRequestTypeDef",
     "PortalTypeDef",
     "GetPortalServiceProviderMetadataRequestRequestTypeDef",
-    "GetPortalServiceProviderMetadataResponseTypeDef",
     "GetTrustStoreCertificateRequestRequestTypeDef",
     "GetTrustStoreRequestRequestTypeDef",
     "TrustStoreTypeDef",
     "GetUserAccessLoggingSettingsRequestRequestTypeDef",
     "UserAccessLoggingSettingsTypeDef",
     "GetUserSettingsRequestRequestTypeDef",
     "UserSettingsTypeDef",
     "IdentityProviderSummaryTypeDef",
     "IpAccessSettingsSummaryTypeDef",
+    "IpRuleOutputTypeDef",
     "ListBrowserSettingsRequestRequestTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
     "ListIpAccessSettingsRequestRequestTypeDef",
     "ListNetworkSettingsRequestRequestTypeDef",
     "NetworkSettingsSummaryTypeDef",
     "ListPortalsRequestRequestTypeDef",
     "PortalSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListTrustStoreCertificatesRequestRequestTypeDef",
     "ListTrustStoresRequestRequestTypeDef",
     "TrustStoreSummaryTypeDef",
     "ListUserAccessLoggingSettingsRequestRequestTypeDef",
     "UserAccessLoggingSettingsSummaryTypeDef",
     "ListUserSettingsRequestRequestTypeDef",
     "UserSettingsSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrowserSettingsRequestRequestTypeDef",
     "UpdateIdentityProviderRequestRequestTypeDef",
     "UpdateNetworkSettingsRequestRequestTypeDef",
     "UpdatePortalRequestRequestTypeDef",
     "UpdateTrustStoreRequestRequestTypeDef",
-    "UpdateTrustStoreResponseTypeDef",
     "UpdateUserAccessLoggingSettingsRequestRequestTypeDef",
     "UpdateUserSettingsRequestRequestTypeDef",
+    "AssociateBrowserSettingsResponseTypeDef",
+    "AssociateIpAccessSettingsResponseTypeDef",
+    "AssociateNetworkSettingsResponseTypeDef",
+    "AssociateTrustStoreResponseTypeDef",
+    "AssociateUserAccessLoggingSettingsResponseTypeDef",
+    "AssociateUserSettingsResponseTypeDef",
+    "CreateBrowserSettingsResponseTypeDef",
+    "CreateIdentityProviderResponseTypeDef",
+    "CreateIpAccessSettingsResponseTypeDef",
+    "CreateNetworkSettingsResponseTypeDef",
+    "CreatePortalResponseTypeDef",
+    "CreateTrustStoreResponseTypeDef",
+    "CreateUserAccessLoggingSettingsResponseTypeDef",
+    "CreateUserSettingsResponseTypeDef",
+    "GetPortalServiceProviderMetadataResponseTypeDef",
+    "UpdateTrustStoreResponseTypeDef",
     "ListBrowserSettingsResponseTypeDef",
     "GetBrowserSettingsResponseTypeDef",
     "UpdateBrowserSettingsResponseTypeDef",
     "ListTrustStoreCertificatesResponseTypeDef",
     "GetTrustStoreCertificateResponseTypeDef",
     "CreateBrowserSettingsRequestRequestTypeDef",
     "CreateNetworkSettingsRequestRequestTypeDef",
     "CreatePortalRequestRequestTypeDef",
     "CreateTrustStoreRequestRequestTypeDef",
     "CreateUserAccessLoggingSettingsRequestRequestTypeDef",
     "CreateUserSettingsRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIpAccessSettingsRequestRequestTypeDef",
-    "IpAccessSettingsTypeDef",
     "UpdateIpAccessSettingsRequestRequestTypeDef",
     "GetIdentityProviderResponseTypeDef",
     "UpdateIdentityProviderResponseTypeDef",
     "GetNetworkSettingsResponseTypeDef",
     "UpdateNetworkSettingsResponseTypeDef",
     "GetPortalResponseTypeDef",
     "UpdatePortalResponseTypeDef",
     "GetTrustStoreResponseTypeDef",
     "GetUserAccessLoggingSettingsResponseTypeDef",
     "UpdateUserAccessLoggingSettingsResponseTypeDef",
     "GetUserSettingsResponseTypeDef",
     "UpdateUserSettingsResponseTypeDef",
     "ListIdentityProvidersResponseTypeDef",
     "ListIpAccessSettingsResponseTypeDef",
+    "IpAccessSettingsTypeDef",
     "ListNetworkSettingsResponseTypeDef",
     "ListPortalsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTrustStoresResponseTypeDef",
     "ListUserAccessLoggingSettingsResponseTypeDef",
     "ListUserSettingsResponseTypeDef",
     "GetIpAccessSettingsResponseTypeDef",
     "UpdateIpAccessSettingsResponseTypeDef",
 )
 
@@ -162,108 +163,65 @@
     "AssociateBrowserSettingsRequestRequestTypeDef",
     {
         "browserSettingsArn": str,
         "portalArn": str,
     },
 )
 
-AssociateBrowserSettingsResponseTypeDef = TypedDict(
-    "AssociateBrowserSettingsResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "browserSettingsArn": str,
-        "portalArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AssociateIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "AssociateIpAccessSettingsRequestRequestTypeDef",
     {
         "ipAccessSettingsArn": str,
         "portalArn": str,
     },
 )
 
-AssociateIpAccessSettingsResponseTypeDef = TypedDict(
-    "AssociateIpAccessSettingsResponseTypeDef",
-    {
-        "ipAccessSettingsArn": str,
-        "portalArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateNetworkSettingsRequestRequestTypeDef = TypedDict(
     "AssociateNetworkSettingsRequestRequestTypeDef",
     {
         "networkSettingsArn": str,
         "portalArn": str,
     },
 )
 
-AssociateNetworkSettingsResponseTypeDef = TypedDict(
-    "AssociateNetworkSettingsResponseTypeDef",
-    {
-        "networkSettingsArn": str,
-        "portalArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateTrustStoreRequestRequestTypeDef = TypedDict(
     "AssociateTrustStoreRequestRequestTypeDef",
     {
         "portalArn": str,
         "trustStoreArn": str,
     },
 )
 
-AssociateTrustStoreResponseTypeDef = TypedDict(
-    "AssociateTrustStoreResponseTypeDef",
-    {
-        "portalArn": str,
-        "trustStoreArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "AssociateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "portalArn": str,
         "userAccessLoggingSettingsArn": str,
     },
 )
 
-AssociateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
-    "AssociateUserAccessLoggingSettingsResponseTypeDef",
-    {
-        "portalArn": str,
-        "userAccessLoggingSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateUserSettingsRequestRequestTypeDef = TypedDict(
     "AssociateUserSettingsRequestRequestTypeDef",
     {
         "portalArn": str,
         "userSettingsArn": str,
     },
 )
 
-AssociateUserSettingsResponseTypeDef = TypedDict(
-    "AssociateUserSettingsResponseTypeDef",
-    {
-        "portalArn": str,
-        "userSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BrowserSettingsSummaryTypeDef = TypedDict(
     "BrowserSettingsSummaryTypeDef",
     {
         "browserSettingsArn": str,
     },
     total=False,
 )
@@ -279,19 +237,17 @@
     {
         "associatedPortalArns": List[str],
         "browserPolicy": str,
     },
     total=False,
 )
 
-
 class BrowserSettingsTypeDef(_RequiredBrowserSettingsTypeDef, _OptionalBrowserSettingsTypeDef):
     pass
 
-
 CertificateSummaryTypeDef = TypedDict(
     "CertificateSummaryTypeDef",
     {
         "issuer": str,
         "notValidAfter": datetime,
         "notValidBefore": datetime,
         "subject": str,
@@ -317,22 +273,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateBrowserSettingsResponseTypeDef = TypedDict(
-    "CreateBrowserSettingsResponseTypeDef",
-    {
-        "browserSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIdentityProviderRequestRequestTypeDef",
     {
         "identityProviderDetails": Mapping[str, str],
         "identityProviderName": str,
         "identityProviderType": IdentityProviderTypeType,
         "portalArn": str,
@@ -342,98 +290,37 @@
     "_OptionalCreateIdentityProviderRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class CreateIdentityProviderRequestRequestTypeDef(
     _RequiredCreateIdentityProviderRequestRequestTypeDef,
     _OptionalCreateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
-
-CreateIdentityProviderResponseTypeDef = TypedDict(
-    "CreateIdentityProviderResponseTypeDef",
-    {
-        "identityProviderArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredIpRuleTypeDef = TypedDict(
     "_RequiredIpRuleTypeDef",
     {
         "ipRange": str,
     },
 )
 _OptionalIpRuleTypeDef = TypedDict(
     "_OptionalIpRuleTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class IpRuleTypeDef(_RequiredIpRuleTypeDef, _OptionalIpRuleTypeDef):
     pass
 
-
-CreateIpAccessSettingsResponseTypeDef = TypedDict(
-    "CreateIpAccessSettingsResponseTypeDef",
-    {
-        "ipAccessSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateNetworkSettingsResponseTypeDef = TypedDict(
-    "CreateNetworkSettingsResponseTypeDef",
-    {
-        "networkSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePortalResponseTypeDef = TypedDict(
-    "CreatePortalResponseTypeDef",
-    {
-        "portalArn": str,
-        "portalEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateTrustStoreResponseTypeDef = TypedDict(
-    "CreateTrustStoreResponseTypeDef",
-    {
-        "trustStoreArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
-    "CreateUserAccessLoggingSettingsResponseTypeDef",
-    {
-        "userAccessLoggingSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateUserSettingsResponseTypeDef = TypedDict(
-    "CreateUserSettingsResponseTypeDef",
-    {
-        "userSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteBrowserSettingsRequestRequestTypeDef = TypedDict(
     "DeleteBrowserSettingsRequestRequestTypeDef",
     {
         "browserSettingsArn": str,
     },
 )
 
@@ -554,19 +441,17 @@
         "identityProviderDetails": Dict[str, str],
         "identityProviderName": str,
         "identityProviderType": IdentityProviderTypeType,
     },
     total=False,
 )
 
-
 class IdentityProviderTypeDef(_RequiredIdentityProviderTypeDef, _OptionalIdentityProviderTypeDef):
     pass
 
-
 GetIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "GetIpAccessSettingsRequestRequestTypeDef",
     {
         "ipAccessSettingsArn": str,
     },
 )
 
@@ -590,19 +475,17 @@
         "securityGroupIds": List[str],
         "subnetIds": List[str],
         "vpcId": str,
     },
     total=False,
 )
 
-
 class NetworkSettingsTypeDef(_RequiredNetworkSettingsTypeDef, _OptionalNetworkSettingsTypeDef):
     pass
 
-
 GetPortalRequestRequestTypeDef = TypedDict(
     "GetPortalRequestRequestTypeDef",
     {
         "portalArn": str,
     },
 )
 
@@ -631,23 +514,14 @@
 GetPortalServiceProviderMetadataRequestRequestTypeDef = TypedDict(
     "GetPortalServiceProviderMetadataRequestRequestTypeDef",
     {
         "portalArn": str,
     },
 )
 
-GetPortalServiceProviderMetadataResponseTypeDef = TypedDict(
-    "GetPortalServiceProviderMetadataResponseTypeDef",
-    {
-        "portalArn": str,
-        "serviceProviderSamlMetadata": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTrustStoreCertificateRequestRequestTypeDef = TypedDict(
     "GetTrustStoreCertificateRequestRequestTypeDef",
     {
         "thumbprint": str,
         "trustStoreArn": str,
     },
 )
@@ -686,21 +560,19 @@
     {
         "associatedPortalArns": List[str],
         "kinesisStreamArn": str,
     },
     total=False,
 )
 
-
 class UserAccessLoggingSettingsTypeDef(
     _RequiredUserAccessLoggingSettingsTypeDef, _OptionalUserAccessLoggingSettingsTypeDef
 ):
     pass
 
-
 GetUserSettingsRequestRequestTypeDef = TypedDict(
     "GetUserSettingsRequestRequestTypeDef",
     {
         "userSettingsArn": str,
     },
 )
 
@@ -721,19 +593,17 @@
         "pasteAllowed": EnabledTypeType,
         "printAllowed": EnabledTypeType,
         "uploadAllowed": EnabledTypeType,
     },
     total=False,
 )
 
-
 class UserSettingsTypeDef(_RequiredUserSettingsTypeDef, _OptionalUserSettingsTypeDef):
     pass
 
-
 IdentityProviderSummaryTypeDef = TypedDict(
     "IdentityProviderSummaryTypeDef",
     {
         "identityProviderArn": str,
         "identityProviderName": str,
         "identityProviderType": IdentityProviderTypeType,
     },
@@ -747,14 +617,31 @@
         "description": str,
         "displayName": str,
         "ipAccessSettingsArn": str,
     },
     total=False,
 )
 
+_RequiredIpRuleOutputTypeDef = TypedDict(
+    "_RequiredIpRuleOutputTypeDef",
+    {
+        "ipRange": str,
+    },
+)
+_OptionalIpRuleOutputTypeDef = TypedDict(
+    "_OptionalIpRuleOutputTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+class IpRuleOutputTypeDef(_RequiredIpRuleOutputTypeDef, _OptionalIpRuleOutputTypeDef):
+    pass
+
 ListBrowserSettingsRequestRequestTypeDef = TypedDict(
     "ListBrowserSettingsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -771,22 +658,20 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListIdentityProvidersRequestRequestTypeDef(
     _RequiredListIdentityProvidersRequestRequestTypeDef,
     _OptionalListIdentityProvidersRequestRequestTypeDef,
 ):
     pass
 
-
 ListIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "ListIpAccessSettingsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -843,14 +728,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
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
 _RequiredListTrustStoreCertificatesRequestRequestTypeDef = TypedDict(
     "_RequiredListTrustStoreCertificatesRequestRequestTypeDef",
     {
         "trustStoreArn": str,
     },
 )
 _OptionalListTrustStoreCertificatesRequestRequestTypeDef = TypedDict(
@@ -858,22 +751,20 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListTrustStoreCertificatesRequestRequestTypeDef(
     _RequiredListTrustStoreCertificatesRequestRequestTypeDef,
     _OptionalListTrustStoreCertificatesRequestRequestTypeDef,
 ):
     pass
 
-
 ListTrustStoresRequestRequestTypeDef = TypedDict(
     "ListTrustStoresRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -925,25 +816,14 @@
         "printAllowed": EnabledTypeType,
         "uploadAllowed": EnabledTypeType,
         "userSettingsArn": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -959,22 +839,20 @@
     {
         "browserPolicy": str,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateBrowserSettingsRequestRequestTypeDef(
     _RequiredUpdateBrowserSettingsRequestRequestTypeDef,
     _OptionalUpdateBrowserSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIdentityProviderRequestRequestTypeDef",
     {
         "identityProviderArn": str,
     },
 )
 _OptionalUpdateIdentityProviderRequestRequestTypeDef = TypedDict(
@@ -984,22 +862,20 @@
         "identityProviderDetails": Mapping[str, str],
         "identityProviderName": str,
         "identityProviderType": IdentityProviderTypeType,
     },
     total=False,
 )
 
-
 class UpdateIdentityProviderRequestRequestTypeDef(
     _RequiredUpdateIdentityProviderRequestRequestTypeDef,
     _OptionalUpdateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateNetworkSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNetworkSettingsRequestRequestTypeDef",
     {
         "networkSettingsArn": str,
     },
 )
 _OptionalUpdateNetworkSettingsRequestRequestTypeDef = TypedDict(
@@ -1009,22 +885,20 @@
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
         "vpcId": str,
     },
     total=False,
 )
 
-
 class UpdateNetworkSettingsRequestRequestTypeDef(
     _RequiredUpdateNetworkSettingsRequestRequestTypeDef,
     _OptionalUpdateNetworkSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdatePortalRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePortalRequestRequestTypeDef",
     {
         "portalArn": str,
     },
 )
 _OptionalUpdatePortalRequestRequestTypeDef = TypedDict(
@@ -1032,21 +906,19 @@
     {
         "authenticationType": AuthenticationTypeType,
         "displayName": str,
     },
     total=False,
 )
 
-
 class UpdatePortalRequestRequestTypeDef(
     _RequiredUpdatePortalRequestRequestTypeDef, _OptionalUpdatePortalRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateTrustStoreRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTrustStoreRequestRequestTypeDef",
     {
         "trustStoreArn": str,
     },
 )
 _OptionalUpdateTrustStoreRequestRequestTypeDef = TypedDict(
@@ -1055,29 +927,19 @@
         "certificatesToAdd": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
         "certificatesToDelete": Sequence[str],
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateTrustStoreRequestRequestTypeDef(
     _RequiredUpdateTrustStoreRequestRequestTypeDef, _OptionalUpdateTrustStoreRequestRequestTypeDef
 ):
     pass
 
-
-UpdateTrustStoreResponseTypeDef = TypedDict(
-    "UpdateTrustStoreResponseTypeDef",
-    {
-        "trustStoreArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "userAccessLoggingSettingsArn": str,
     },
 )
 _OptionalUpdateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
@@ -1085,22 +947,20 @@
     {
         "clientToken": str,
         "kinesisStreamArn": str,
     },
     total=False,
 )
 
-
 class UpdateUserAccessLoggingSettingsRequestRequestTypeDef(
     _RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef,
     _OptionalUpdateUserAccessLoggingSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateUserSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserSettingsRequestRequestTypeDef",
     {
         "userSettingsArn": str,
     },
 )
 _OptionalUpdateUserSettingsRequestRequestTypeDef = TypedDict(
@@ -1114,63 +974,197 @@
         "pasteAllowed": EnabledTypeType,
         "printAllowed": EnabledTypeType,
         "uploadAllowed": EnabledTypeType,
     },
     total=False,
 )
 
-
 class UpdateUserSettingsRequestRequestTypeDef(
     _RequiredUpdateUserSettingsRequestRequestTypeDef,
     _OptionalUpdateUserSettingsRequestRequestTypeDef,
 ):
     pass
 
+AssociateBrowserSettingsResponseTypeDef = TypedDict(
+    "AssociateBrowserSettingsResponseTypeDef",
+    {
+        "browserSettingsArn": str,
+        "portalArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateIpAccessSettingsResponseTypeDef = TypedDict(
+    "AssociateIpAccessSettingsResponseTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+        "portalArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateNetworkSettingsResponseTypeDef = TypedDict(
+    "AssociateNetworkSettingsResponseTypeDef",
+    {
+        "networkSettingsArn": str,
+        "portalArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateTrustStoreResponseTypeDef = TypedDict(
+    "AssociateTrustStoreResponseTypeDef",
+    {
+        "portalArn": str,
+        "trustStoreArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
+    "AssociateUserAccessLoggingSettingsResponseTypeDef",
+    {
+        "portalArn": str,
+        "userAccessLoggingSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateUserSettingsResponseTypeDef = TypedDict(
+    "AssociateUserSettingsResponseTypeDef",
+    {
+        "portalArn": str,
+        "userSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBrowserSettingsResponseTypeDef = TypedDict(
+    "CreateBrowserSettingsResponseTypeDef",
+    {
+        "browserSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIdentityProviderResponseTypeDef = TypedDict(
+    "CreateIdentityProviderResponseTypeDef",
+    {
+        "identityProviderArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIpAccessSettingsResponseTypeDef = TypedDict(
+    "CreateIpAccessSettingsResponseTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNetworkSettingsResponseTypeDef = TypedDict(
+    "CreateNetworkSettingsResponseTypeDef",
+    {
+        "networkSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePortalResponseTypeDef = TypedDict(
+    "CreatePortalResponseTypeDef",
+    {
+        "portalArn": str,
+        "portalEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTrustStoreResponseTypeDef = TypedDict(
+    "CreateTrustStoreResponseTypeDef",
+    {
+        "trustStoreArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
+    "CreateUserAccessLoggingSettingsResponseTypeDef",
+    {
+        "userAccessLoggingSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserSettingsResponseTypeDef = TypedDict(
+    "CreateUserSettingsResponseTypeDef",
+    {
+        "userSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPortalServiceProviderMetadataResponseTypeDef = TypedDict(
+    "GetPortalServiceProviderMetadataResponseTypeDef",
+    {
+        "portalArn": str,
+        "serviceProviderSamlMetadata": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTrustStoreResponseTypeDef = TypedDict(
+    "UpdateTrustStoreResponseTypeDef",
+    {
+        "trustStoreArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ListBrowserSettingsResponseTypeDef = TypedDict(
     "ListBrowserSettingsResponseTypeDef",
     {
         "browserSettings": List[BrowserSettingsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBrowserSettingsResponseTypeDef = TypedDict(
     "GetBrowserSettingsResponseTypeDef",
     {
         "browserSettings": BrowserSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBrowserSettingsResponseTypeDef = TypedDict(
     "UpdateBrowserSettingsResponseTypeDef",
     {
         "browserSettings": BrowserSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrustStoreCertificatesResponseTypeDef = TypedDict(
     "ListTrustStoreCertificatesResponseTypeDef",
     {
         "certificateList": List[CertificateSummaryTypeDef],
         "nextToken": str,
         "trustStoreArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTrustStoreCertificateResponseTypeDef = TypedDict(
     "GetTrustStoreCertificateResponseTypeDef",
     {
         "certificate": CertificateTypeDef,
         "trustStoreArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateBrowserSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBrowserSettingsRequestRequestTypeDef",
     {
         "browserPolicy": str,
@@ -1183,22 +1177,20 @@
         "clientToken": str,
         "customerManagedKey": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateBrowserSettingsRequestRequestTypeDef(
     _RequiredCreateBrowserSettingsRequestRequestTypeDef,
     _OptionalCreateBrowserSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateNetworkSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNetworkSettingsRequestRequestTypeDef",
     {
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
         "vpcId": str,
     },
@@ -1208,22 +1200,20 @@
     {
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateNetworkSettingsRequestRequestTypeDef(
     _RequiredCreateNetworkSettingsRequestRequestTypeDef,
     _OptionalCreateNetworkSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 CreatePortalRequestRequestTypeDef = TypedDict(
     "CreatePortalRequestRequestTypeDef",
     {
         "additionalEncryptionContext": Mapping[str, str],
         "authenticationType": AuthenticationTypeType,
         "clientToken": str,
         "customerManagedKey": str,
@@ -1244,21 +1234,19 @@
     {
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateTrustStoreRequestRequestTypeDef(
     _RequiredCreateTrustStoreRequestRequestTypeDef, _OptionalCreateTrustStoreRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "kinesisStreamArn": str,
     },
 )
 _OptionalCreateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
@@ -1266,22 +1254,20 @@
     {
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateUserAccessLoggingSettingsRequestRequestTypeDef(
     _RequiredCreateUserAccessLoggingSettingsRequestRequestTypeDef,
     _OptionalCreateUserAccessLoggingSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateUserSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserSettingsRequestRequestTypeDef",
     {
         "copyAllowed": EnabledTypeType,
         "downloadAllowed": EnabledTypeType,
         "pasteAllowed": EnabledTypeType,
         "printAllowed": EnabledTypeType,
@@ -1295,30 +1281,20 @@
         "disconnectTimeoutInMinutes": int,
         "idleDisconnectTimeoutInMinutes": int,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateUserSettingsRequestRequestTypeDef(
     _RequiredCreateUserSettingsRequestRequestTypeDef,
     _OptionalCreateUserSettingsRequestRequestTypeDef,
 ):
     pass
 
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1326,21 +1302,19 @@
     "_OptionalTagResourceRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class TagResourceRequestRequestTypeDef(
     _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIpAccessSettingsRequestRequestTypeDef",
     {
         "ipRules": Sequence[IpRuleTypeDef],
     },
 )
 _OptionalCreateIpAccessSettingsRequestRequestTypeDef = TypedDict(
@@ -1352,45 +1326,20 @@
         "description": str,
         "displayName": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateIpAccessSettingsRequestRequestTypeDef(
     _RequiredCreateIpAccessSettingsRequestRequestTypeDef,
     _OptionalCreateIpAccessSettingsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredIpAccessSettingsTypeDef = TypedDict(
-    "_RequiredIpAccessSettingsTypeDef",
-    {
-        "ipAccessSettingsArn": str,
-    },
-)
-_OptionalIpAccessSettingsTypeDef = TypedDict(
-    "_OptionalIpAccessSettingsTypeDef",
-    {
-        "associatedPortalArns": List[str],
-        "creationDate": datetime,
-        "description": str,
-        "displayName": str,
-        "ipRules": List[IpRuleTypeDef],
-    },
-    total=False,
-)
-
-
-class IpAccessSettingsTypeDef(_RequiredIpAccessSettingsTypeDef, _OptionalIpAccessSettingsTypeDef):
-    pass
-
-
 _RequiredUpdateIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIpAccessSettingsRequestRequestTypeDef",
     {
         "ipAccessSettingsArn": str,
     },
 )
 _OptionalUpdateIpAccessSettingsRequestRequestTypeDef = TypedDict(
@@ -1400,181 +1349,208 @@
         "description": str,
         "displayName": str,
         "ipRules": Sequence[IpRuleTypeDef],
     },
     total=False,
 )
 
-
 class UpdateIpAccessSettingsRequestRequestTypeDef(
     _RequiredUpdateIpAccessSettingsRequestRequestTypeDef,
     _OptionalUpdateIpAccessSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 GetIdentityProviderResponseTypeDef = TypedDict(
     "GetIdentityProviderResponseTypeDef",
     {
         "identityProvider": IdentityProviderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIdentityProviderResponseTypeDef = TypedDict(
     "UpdateIdentityProviderResponseTypeDef",
     {
         "identityProvider": IdentityProviderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNetworkSettingsResponseTypeDef = TypedDict(
     "GetNetworkSettingsResponseTypeDef",
     {
         "networkSettings": NetworkSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNetworkSettingsResponseTypeDef = TypedDict(
     "UpdateNetworkSettingsResponseTypeDef",
     {
         "networkSettings": NetworkSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPortalResponseTypeDef = TypedDict(
     "GetPortalResponseTypeDef",
     {
         "portal": PortalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePortalResponseTypeDef = TypedDict(
     "UpdatePortalResponseTypeDef",
     {
         "portal": PortalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTrustStoreResponseTypeDef = TypedDict(
     "GetTrustStoreResponseTypeDef",
     {
         "trustStore": TrustStoreTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserAccessLoggingSettingsResponseTypeDef = TypedDict(
     "GetUserAccessLoggingSettingsResponseTypeDef",
     {
         "userAccessLoggingSettings": UserAccessLoggingSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
     "UpdateUserAccessLoggingSettingsResponseTypeDef",
     {
         "userAccessLoggingSettings": UserAccessLoggingSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserSettingsResponseTypeDef = TypedDict(
     "GetUserSettingsResponseTypeDef",
     {
         "userSettings": UserSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserSettingsResponseTypeDef = TypedDict(
     "UpdateUserSettingsResponseTypeDef",
     {
         "userSettings": UserSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentityProvidersResponseTypeDef = TypedDict(
     "ListIdentityProvidersResponseTypeDef",
     {
         "identityProviders": List[IdentityProviderSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIpAccessSettingsResponseTypeDef = TypedDict(
     "ListIpAccessSettingsResponseTypeDef",
     {
         "ipAccessSettings": List[IpAccessSettingsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredIpAccessSettingsTypeDef = TypedDict(
+    "_RequiredIpAccessSettingsTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+    },
+)
+_OptionalIpAccessSettingsTypeDef = TypedDict(
+    "_OptionalIpAccessSettingsTypeDef",
+    {
+        "associatedPortalArns": List[str],
+        "creationDate": datetime,
+        "description": str,
+        "displayName": str,
+        "ipRules": List[IpRuleOutputTypeDef],
+    },
+    total=False,
+)
+
+class IpAccessSettingsTypeDef(_RequiredIpAccessSettingsTypeDef, _OptionalIpAccessSettingsTypeDef):
+    pass
+
 ListNetworkSettingsResponseTypeDef = TypedDict(
     "ListNetworkSettingsResponseTypeDef",
     {
         "networkSettings": List[NetworkSettingsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPortalsResponseTypeDef = TypedDict(
     "ListPortalsResponseTypeDef",
     {
         "nextToken": str,
         "portals": List[PortalSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrustStoresResponseTypeDef = TypedDict(
     "ListTrustStoresResponseTypeDef",
     {
         "nextToken": str,
         "trustStores": List[TrustStoreSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserAccessLoggingSettingsResponseTypeDef = TypedDict(
     "ListUserAccessLoggingSettingsResponseTypeDef",
     {
         "nextToken": str,
         "userAccessLoggingSettings": List[UserAccessLoggingSettingsSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserSettingsResponseTypeDef = TypedDict(
     "ListUserSettingsResponseTypeDef",
     {
         "nextToken": str,
         "userSettings": List[UserSettingsSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIpAccessSettingsResponseTypeDef = TypedDict(
     "GetIpAccessSettingsResponseTypeDef",
     {
         "ipAccessSettings": IpAccessSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIpAccessSettingsResponseTypeDef = TypedDict(
     "UpdateIpAccessSettingsResponseTypeDef",
     {
         "ipAccessSettings": IpAccessSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web/type_defs.pyi` & `mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,42 +29,30 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssociateBrowserSettingsRequestRequestTypeDef",
-    "AssociateBrowserSettingsResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateIpAccessSettingsRequestRequestTypeDef",
-    "AssociateIpAccessSettingsResponseTypeDef",
     "AssociateNetworkSettingsRequestRequestTypeDef",
-    "AssociateNetworkSettingsResponseTypeDef",
     "AssociateTrustStoreRequestRequestTypeDef",
-    "AssociateTrustStoreResponseTypeDef",
     "AssociateUserAccessLoggingSettingsRequestRequestTypeDef",
-    "AssociateUserAccessLoggingSettingsResponseTypeDef",
     "AssociateUserSettingsRequestRequestTypeDef",
-    "AssociateUserSettingsResponseTypeDef",
     "BrowserSettingsSummaryTypeDef",
     "BrowserSettingsTypeDef",
     "CertificateSummaryTypeDef",
     "CertificateTypeDef",
     "TagTypeDef",
-    "CreateBrowserSettingsResponseTypeDef",
     "CreateIdentityProviderRequestRequestTypeDef",
-    "CreateIdentityProviderResponseTypeDef",
     "IpRuleTypeDef",
-    "CreateIpAccessSettingsResponseTypeDef",
-    "CreateNetworkSettingsResponseTypeDef",
-    "CreatePortalResponseTypeDef",
-    "CreateTrustStoreResponseTypeDef",
-    "CreateUserAccessLoggingSettingsResponseTypeDef",
-    "CreateUserSettingsResponseTypeDef",
     "DeleteBrowserSettingsRequestRequestTypeDef",
     "DeleteIdentityProviderRequestRequestTypeDef",
     "DeleteIpAccessSettingsRequestRequestTypeDef",
     "DeleteNetworkSettingsRequestRequestTypeDef",
     "DeletePortalRequestRequestTypeDef",
     "DeleteTrustStoreRequestRequestTypeDef",
     "DeleteUserAccessLoggingSettingsRequestRequestTypeDef",
@@ -80,80 +68,95 @@
     "IdentityProviderTypeDef",
     "GetIpAccessSettingsRequestRequestTypeDef",
     "GetNetworkSettingsRequestRequestTypeDef",
     "NetworkSettingsTypeDef",
     "GetPortalRequestRequestTypeDef",
     "PortalTypeDef",
     "GetPortalServiceProviderMetadataRequestRequestTypeDef",
-    "GetPortalServiceProviderMetadataResponseTypeDef",
     "GetTrustStoreCertificateRequestRequestTypeDef",
     "GetTrustStoreRequestRequestTypeDef",
     "TrustStoreTypeDef",
     "GetUserAccessLoggingSettingsRequestRequestTypeDef",
     "UserAccessLoggingSettingsTypeDef",
     "GetUserSettingsRequestRequestTypeDef",
     "UserSettingsTypeDef",
     "IdentityProviderSummaryTypeDef",
     "IpAccessSettingsSummaryTypeDef",
+    "IpRuleOutputTypeDef",
     "ListBrowserSettingsRequestRequestTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
     "ListIpAccessSettingsRequestRequestTypeDef",
     "ListNetworkSettingsRequestRequestTypeDef",
     "NetworkSettingsSummaryTypeDef",
     "ListPortalsRequestRequestTypeDef",
     "PortalSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListTrustStoreCertificatesRequestRequestTypeDef",
     "ListTrustStoresRequestRequestTypeDef",
     "TrustStoreSummaryTypeDef",
     "ListUserAccessLoggingSettingsRequestRequestTypeDef",
     "UserAccessLoggingSettingsSummaryTypeDef",
     "ListUserSettingsRequestRequestTypeDef",
     "UserSettingsSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrowserSettingsRequestRequestTypeDef",
     "UpdateIdentityProviderRequestRequestTypeDef",
     "UpdateNetworkSettingsRequestRequestTypeDef",
     "UpdatePortalRequestRequestTypeDef",
     "UpdateTrustStoreRequestRequestTypeDef",
-    "UpdateTrustStoreResponseTypeDef",
     "UpdateUserAccessLoggingSettingsRequestRequestTypeDef",
     "UpdateUserSettingsRequestRequestTypeDef",
+    "AssociateBrowserSettingsResponseTypeDef",
+    "AssociateIpAccessSettingsResponseTypeDef",
+    "AssociateNetworkSettingsResponseTypeDef",
+    "AssociateTrustStoreResponseTypeDef",
+    "AssociateUserAccessLoggingSettingsResponseTypeDef",
+    "AssociateUserSettingsResponseTypeDef",
+    "CreateBrowserSettingsResponseTypeDef",
+    "CreateIdentityProviderResponseTypeDef",
+    "CreateIpAccessSettingsResponseTypeDef",
+    "CreateNetworkSettingsResponseTypeDef",
+    "CreatePortalResponseTypeDef",
+    "CreateTrustStoreResponseTypeDef",
+    "CreateUserAccessLoggingSettingsResponseTypeDef",
+    "CreateUserSettingsResponseTypeDef",
+    "GetPortalServiceProviderMetadataResponseTypeDef",
+    "UpdateTrustStoreResponseTypeDef",
     "ListBrowserSettingsResponseTypeDef",
     "GetBrowserSettingsResponseTypeDef",
     "UpdateBrowserSettingsResponseTypeDef",
     "ListTrustStoreCertificatesResponseTypeDef",
     "GetTrustStoreCertificateResponseTypeDef",
     "CreateBrowserSettingsRequestRequestTypeDef",
     "CreateNetworkSettingsRequestRequestTypeDef",
     "CreatePortalRequestRequestTypeDef",
     "CreateTrustStoreRequestRequestTypeDef",
     "CreateUserAccessLoggingSettingsRequestRequestTypeDef",
     "CreateUserSettingsRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIpAccessSettingsRequestRequestTypeDef",
-    "IpAccessSettingsTypeDef",
     "UpdateIpAccessSettingsRequestRequestTypeDef",
     "GetIdentityProviderResponseTypeDef",
     "UpdateIdentityProviderResponseTypeDef",
     "GetNetworkSettingsResponseTypeDef",
     "UpdateNetworkSettingsResponseTypeDef",
     "GetPortalResponseTypeDef",
     "UpdatePortalResponseTypeDef",
     "GetTrustStoreResponseTypeDef",
     "GetUserAccessLoggingSettingsResponseTypeDef",
     "UpdateUserAccessLoggingSettingsResponseTypeDef",
     "GetUserSettingsResponseTypeDef",
     "UpdateUserSettingsResponseTypeDef",
     "ListIdentityProvidersResponseTypeDef",
     "ListIpAccessSettingsResponseTypeDef",
+    "IpAccessSettingsTypeDef",
     "ListNetworkSettingsResponseTypeDef",
     "ListPortalsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTrustStoresResponseTypeDef",
     "ListUserAccessLoggingSettingsResponseTypeDef",
     "ListUserSettingsResponseTypeDef",
     "GetIpAccessSettingsResponseTypeDef",
     "UpdateIpAccessSettingsResponseTypeDef",
 )
 
@@ -161,108 +164,65 @@
     "AssociateBrowserSettingsRequestRequestTypeDef",
     {
         "browserSettingsArn": str,
         "portalArn": str,
     },
 )
 
-AssociateBrowserSettingsResponseTypeDef = TypedDict(
-    "AssociateBrowserSettingsResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "browserSettingsArn": str,
-        "portalArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AssociateIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "AssociateIpAccessSettingsRequestRequestTypeDef",
     {
         "ipAccessSettingsArn": str,
         "portalArn": str,
     },
 )
 
-AssociateIpAccessSettingsResponseTypeDef = TypedDict(
-    "AssociateIpAccessSettingsResponseTypeDef",
-    {
-        "ipAccessSettingsArn": str,
-        "portalArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateNetworkSettingsRequestRequestTypeDef = TypedDict(
     "AssociateNetworkSettingsRequestRequestTypeDef",
     {
         "networkSettingsArn": str,
         "portalArn": str,
     },
 )
 
-AssociateNetworkSettingsResponseTypeDef = TypedDict(
-    "AssociateNetworkSettingsResponseTypeDef",
-    {
-        "networkSettingsArn": str,
-        "portalArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateTrustStoreRequestRequestTypeDef = TypedDict(
     "AssociateTrustStoreRequestRequestTypeDef",
     {
         "portalArn": str,
         "trustStoreArn": str,
     },
 )
 
-AssociateTrustStoreResponseTypeDef = TypedDict(
-    "AssociateTrustStoreResponseTypeDef",
-    {
-        "portalArn": str,
-        "trustStoreArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "AssociateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "portalArn": str,
         "userAccessLoggingSettingsArn": str,
     },
 )
 
-AssociateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
-    "AssociateUserAccessLoggingSettingsResponseTypeDef",
-    {
-        "portalArn": str,
-        "userAccessLoggingSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateUserSettingsRequestRequestTypeDef = TypedDict(
     "AssociateUserSettingsRequestRequestTypeDef",
     {
         "portalArn": str,
         "userSettingsArn": str,
     },
 )
 
-AssociateUserSettingsResponseTypeDef = TypedDict(
-    "AssociateUserSettingsResponseTypeDef",
-    {
-        "portalArn": str,
-        "userSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BrowserSettingsSummaryTypeDef = TypedDict(
     "BrowserSettingsSummaryTypeDef",
     {
         "browserSettingsArn": str,
     },
     total=False,
 )
@@ -278,17 +238,19 @@
     {
         "associatedPortalArns": List[str],
         "browserPolicy": str,
     },
     total=False,
 )
 
+
 class BrowserSettingsTypeDef(_RequiredBrowserSettingsTypeDef, _OptionalBrowserSettingsTypeDef):
     pass
 
+
 CertificateSummaryTypeDef = TypedDict(
     "CertificateSummaryTypeDef",
     {
         "issuer": str,
         "notValidAfter": datetime,
         "notValidBefore": datetime,
         "subject": str,
@@ -314,22 +276,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateBrowserSettingsResponseTypeDef = TypedDict(
-    "CreateBrowserSettingsResponseTypeDef",
-    {
-        "browserSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIdentityProviderRequestRequestTypeDef",
     {
         "identityProviderDetails": Mapping[str, str],
         "identityProviderName": str,
         "identityProviderType": IdentityProviderTypeType,
         "portalArn": str,
@@ -339,27 +293,21 @@
     "_OptionalCreateIdentityProviderRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class CreateIdentityProviderRequestRequestTypeDef(
     _RequiredCreateIdentityProviderRequestRequestTypeDef,
     _OptionalCreateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
-CreateIdentityProviderResponseTypeDef = TypedDict(
-    "CreateIdentityProviderResponseTypeDef",
-    {
-        "identityProviderArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredIpRuleTypeDef = TypedDict(
     "_RequiredIpRuleTypeDef",
     {
         "ipRange": str,
     },
 )
@@ -367,65 +315,18 @@
     "_OptionalIpRuleTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class IpRuleTypeDef(_RequiredIpRuleTypeDef, _OptionalIpRuleTypeDef):
     pass
 
-CreateIpAccessSettingsResponseTypeDef = TypedDict(
-    "CreateIpAccessSettingsResponseTypeDef",
-    {
-        "ipAccessSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateNetworkSettingsResponseTypeDef = TypedDict(
-    "CreateNetworkSettingsResponseTypeDef",
-    {
-        "networkSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePortalResponseTypeDef = TypedDict(
-    "CreatePortalResponseTypeDef",
-    {
-        "portalArn": str,
-        "portalEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateTrustStoreResponseTypeDef = TypedDict(
-    "CreateTrustStoreResponseTypeDef",
-    {
-        "trustStoreArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
-    "CreateUserAccessLoggingSettingsResponseTypeDef",
-    {
-        "userAccessLoggingSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateUserSettingsResponseTypeDef = TypedDict(
-    "CreateUserSettingsResponseTypeDef",
-    {
-        "userSettingsArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeleteBrowserSettingsRequestRequestTypeDef = TypedDict(
     "DeleteBrowserSettingsRequestRequestTypeDef",
     {
         "browserSettingsArn": str,
     },
 )
@@ -547,17 +448,19 @@
         "identityProviderDetails": Dict[str, str],
         "identityProviderName": str,
         "identityProviderType": IdentityProviderTypeType,
     },
     total=False,
 )
 
+
 class IdentityProviderTypeDef(_RequiredIdentityProviderTypeDef, _OptionalIdentityProviderTypeDef):
     pass
 
+
 GetIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "GetIpAccessSettingsRequestRequestTypeDef",
     {
         "ipAccessSettingsArn": str,
     },
 )
 
@@ -581,17 +484,19 @@
         "securityGroupIds": List[str],
         "subnetIds": List[str],
         "vpcId": str,
     },
     total=False,
 )
 
+
 class NetworkSettingsTypeDef(_RequiredNetworkSettingsTypeDef, _OptionalNetworkSettingsTypeDef):
     pass
 
+
 GetPortalRequestRequestTypeDef = TypedDict(
     "GetPortalRequestRequestTypeDef",
     {
         "portalArn": str,
     },
 )
 
@@ -620,23 +525,14 @@
 GetPortalServiceProviderMetadataRequestRequestTypeDef = TypedDict(
     "GetPortalServiceProviderMetadataRequestRequestTypeDef",
     {
         "portalArn": str,
     },
 )
 
-GetPortalServiceProviderMetadataResponseTypeDef = TypedDict(
-    "GetPortalServiceProviderMetadataResponseTypeDef",
-    {
-        "portalArn": str,
-        "serviceProviderSamlMetadata": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTrustStoreCertificateRequestRequestTypeDef = TypedDict(
     "GetTrustStoreCertificateRequestRequestTypeDef",
     {
         "thumbprint": str,
         "trustStoreArn": str,
     },
 )
@@ -675,19 +571,21 @@
     {
         "associatedPortalArns": List[str],
         "kinesisStreamArn": str,
     },
     total=False,
 )
 
+
 class UserAccessLoggingSettingsTypeDef(
     _RequiredUserAccessLoggingSettingsTypeDef, _OptionalUserAccessLoggingSettingsTypeDef
 ):
     pass
 
+
 GetUserSettingsRequestRequestTypeDef = TypedDict(
     "GetUserSettingsRequestRequestTypeDef",
     {
         "userSettingsArn": str,
     },
 )
 
@@ -708,17 +606,19 @@
         "pasteAllowed": EnabledTypeType,
         "printAllowed": EnabledTypeType,
         "uploadAllowed": EnabledTypeType,
     },
     total=False,
 )
 
+
 class UserSettingsTypeDef(_RequiredUserSettingsTypeDef, _OptionalUserSettingsTypeDef):
     pass
 
+
 IdentityProviderSummaryTypeDef = TypedDict(
     "IdentityProviderSummaryTypeDef",
     {
         "identityProviderArn": str,
         "identityProviderName": str,
         "identityProviderType": IdentityProviderTypeType,
     },
@@ -732,14 +632,33 @@
         "description": str,
         "displayName": str,
         "ipAccessSettingsArn": str,
     },
     total=False,
 )
 
+_RequiredIpRuleOutputTypeDef = TypedDict(
+    "_RequiredIpRuleOutputTypeDef",
+    {
+        "ipRange": str,
+    },
+)
+_OptionalIpRuleOutputTypeDef = TypedDict(
+    "_OptionalIpRuleOutputTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+
+class IpRuleOutputTypeDef(_RequiredIpRuleOutputTypeDef, _OptionalIpRuleOutputTypeDef):
+    pass
+
+
 ListBrowserSettingsRequestRequestTypeDef = TypedDict(
     "ListBrowserSettingsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -756,20 +675,22 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListIdentityProvidersRequestRequestTypeDef(
     _RequiredListIdentityProvidersRequestRequestTypeDef,
     _OptionalListIdentityProvidersRequestRequestTypeDef,
 ):
     pass
 
+
 ListIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "ListIpAccessSettingsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -826,14 +747,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
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
 _RequiredListTrustStoreCertificatesRequestRequestTypeDef = TypedDict(
     "_RequiredListTrustStoreCertificatesRequestRequestTypeDef",
     {
         "trustStoreArn": str,
     },
 )
 _OptionalListTrustStoreCertificatesRequestRequestTypeDef = TypedDict(
@@ -841,20 +770,22 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListTrustStoreCertificatesRequestRequestTypeDef(
     _RequiredListTrustStoreCertificatesRequestRequestTypeDef,
     _OptionalListTrustStoreCertificatesRequestRequestTypeDef,
 ):
     pass
 
+
 ListTrustStoresRequestRequestTypeDef = TypedDict(
     "ListTrustStoresRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -906,25 +837,14 @@
         "printAllowed": EnabledTypeType,
         "uploadAllowed": EnabledTypeType,
         "userSettingsArn": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -940,20 +860,22 @@
     {
         "browserPolicy": str,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateBrowserSettingsRequestRequestTypeDef(
     _RequiredUpdateBrowserSettingsRequestRequestTypeDef,
     _OptionalUpdateBrowserSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIdentityProviderRequestRequestTypeDef",
     {
         "identityProviderArn": str,
     },
 )
 _OptionalUpdateIdentityProviderRequestRequestTypeDef = TypedDict(
@@ -963,20 +885,22 @@
         "identityProviderDetails": Mapping[str, str],
         "identityProviderName": str,
         "identityProviderType": IdentityProviderTypeType,
     },
     total=False,
 )
 
+
 class UpdateIdentityProviderRequestRequestTypeDef(
     _RequiredUpdateIdentityProviderRequestRequestTypeDef,
     _OptionalUpdateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateNetworkSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNetworkSettingsRequestRequestTypeDef",
     {
         "networkSettingsArn": str,
     },
 )
 _OptionalUpdateNetworkSettingsRequestRequestTypeDef = TypedDict(
@@ -986,20 +910,22 @@
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
         "vpcId": str,
     },
     total=False,
 )
 
+
 class UpdateNetworkSettingsRequestRequestTypeDef(
     _RequiredUpdateNetworkSettingsRequestRequestTypeDef,
     _OptionalUpdateNetworkSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdatePortalRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePortalRequestRequestTypeDef",
     {
         "portalArn": str,
     },
 )
 _OptionalUpdatePortalRequestRequestTypeDef = TypedDict(
@@ -1007,19 +933,21 @@
     {
         "authenticationType": AuthenticationTypeType,
         "displayName": str,
     },
     total=False,
 )
 
+
 class UpdatePortalRequestRequestTypeDef(
     _RequiredUpdatePortalRequestRequestTypeDef, _OptionalUpdatePortalRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateTrustStoreRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTrustStoreRequestRequestTypeDef",
     {
         "trustStoreArn": str,
     },
 )
 _OptionalUpdateTrustStoreRequestRequestTypeDef = TypedDict(
@@ -1028,26 +956,20 @@
         "certificatesToAdd": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
         "certificatesToDelete": Sequence[str],
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateTrustStoreRequestRequestTypeDef(
     _RequiredUpdateTrustStoreRequestRequestTypeDef, _OptionalUpdateTrustStoreRequestRequestTypeDef
 ):
     pass
 
-UpdateTrustStoreResponseTypeDef = TypedDict(
-    "UpdateTrustStoreResponseTypeDef",
-    {
-        "trustStoreArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "userAccessLoggingSettingsArn": str,
     },
 )
@@ -1056,20 +978,22 @@
     {
         "clientToken": str,
         "kinesisStreamArn": str,
     },
     total=False,
 )
 
+
 class UpdateUserAccessLoggingSettingsRequestRequestTypeDef(
     _RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef,
     _OptionalUpdateUserAccessLoggingSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateUserSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserSettingsRequestRequestTypeDef",
     {
         "userSettingsArn": str,
     },
 )
 _OptionalUpdateUserSettingsRequestRequestTypeDef = TypedDict(
@@ -1083,61 +1007,199 @@
         "pasteAllowed": EnabledTypeType,
         "printAllowed": EnabledTypeType,
         "uploadAllowed": EnabledTypeType,
     },
     total=False,
 )
 
+
 class UpdateUserSettingsRequestRequestTypeDef(
     _RequiredUpdateUserSettingsRequestRequestTypeDef,
     _OptionalUpdateUserSettingsRequestRequestTypeDef,
 ):
     pass
 
+
+AssociateBrowserSettingsResponseTypeDef = TypedDict(
+    "AssociateBrowserSettingsResponseTypeDef",
+    {
+        "browserSettingsArn": str,
+        "portalArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateIpAccessSettingsResponseTypeDef = TypedDict(
+    "AssociateIpAccessSettingsResponseTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+        "portalArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateNetworkSettingsResponseTypeDef = TypedDict(
+    "AssociateNetworkSettingsResponseTypeDef",
+    {
+        "networkSettingsArn": str,
+        "portalArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateTrustStoreResponseTypeDef = TypedDict(
+    "AssociateTrustStoreResponseTypeDef",
+    {
+        "portalArn": str,
+        "trustStoreArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
+    "AssociateUserAccessLoggingSettingsResponseTypeDef",
+    {
+        "portalArn": str,
+        "userAccessLoggingSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateUserSettingsResponseTypeDef = TypedDict(
+    "AssociateUserSettingsResponseTypeDef",
+    {
+        "portalArn": str,
+        "userSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBrowserSettingsResponseTypeDef = TypedDict(
+    "CreateBrowserSettingsResponseTypeDef",
+    {
+        "browserSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIdentityProviderResponseTypeDef = TypedDict(
+    "CreateIdentityProviderResponseTypeDef",
+    {
+        "identityProviderArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIpAccessSettingsResponseTypeDef = TypedDict(
+    "CreateIpAccessSettingsResponseTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNetworkSettingsResponseTypeDef = TypedDict(
+    "CreateNetworkSettingsResponseTypeDef",
+    {
+        "networkSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePortalResponseTypeDef = TypedDict(
+    "CreatePortalResponseTypeDef",
+    {
+        "portalArn": str,
+        "portalEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTrustStoreResponseTypeDef = TypedDict(
+    "CreateTrustStoreResponseTypeDef",
+    {
+        "trustStoreArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
+    "CreateUserAccessLoggingSettingsResponseTypeDef",
+    {
+        "userAccessLoggingSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserSettingsResponseTypeDef = TypedDict(
+    "CreateUserSettingsResponseTypeDef",
+    {
+        "userSettingsArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPortalServiceProviderMetadataResponseTypeDef = TypedDict(
+    "GetPortalServiceProviderMetadataResponseTypeDef",
+    {
+        "portalArn": str,
+        "serviceProviderSamlMetadata": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTrustStoreResponseTypeDef = TypedDict(
+    "UpdateTrustStoreResponseTypeDef",
+    {
+        "trustStoreArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListBrowserSettingsResponseTypeDef = TypedDict(
     "ListBrowserSettingsResponseTypeDef",
     {
         "browserSettings": List[BrowserSettingsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBrowserSettingsResponseTypeDef = TypedDict(
     "GetBrowserSettingsResponseTypeDef",
     {
         "browserSettings": BrowserSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBrowserSettingsResponseTypeDef = TypedDict(
     "UpdateBrowserSettingsResponseTypeDef",
     {
         "browserSettings": BrowserSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrustStoreCertificatesResponseTypeDef = TypedDict(
     "ListTrustStoreCertificatesResponseTypeDef",
     {
         "certificateList": List[CertificateSummaryTypeDef],
         "nextToken": str,
         "trustStoreArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTrustStoreCertificateResponseTypeDef = TypedDict(
     "GetTrustStoreCertificateResponseTypeDef",
     {
         "certificate": CertificateTypeDef,
         "trustStoreArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateBrowserSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBrowserSettingsRequestRequestTypeDef",
     {
         "browserPolicy": str,
@@ -1150,20 +1212,22 @@
         "clientToken": str,
         "customerManagedKey": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateBrowserSettingsRequestRequestTypeDef(
     _RequiredCreateBrowserSettingsRequestRequestTypeDef,
     _OptionalCreateBrowserSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateNetworkSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNetworkSettingsRequestRequestTypeDef",
     {
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
         "vpcId": str,
     },
@@ -1173,20 +1237,22 @@
     {
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateNetworkSettingsRequestRequestTypeDef(
     _RequiredCreateNetworkSettingsRequestRequestTypeDef,
     _OptionalCreateNetworkSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 CreatePortalRequestRequestTypeDef = TypedDict(
     "CreatePortalRequestRequestTypeDef",
     {
         "additionalEncryptionContext": Mapping[str, str],
         "authenticationType": AuthenticationTypeType,
         "clientToken": str,
         "customerManagedKey": str,
@@ -1207,19 +1273,21 @@
     {
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateTrustStoreRequestRequestTypeDef(
     _RequiredCreateTrustStoreRequestRequestTypeDef, _OptionalCreateTrustStoreRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "kinesisStreamArn": str,
     },
 )
 _OptionalCreateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
@@ -1227,20 +1295,22 @@
     {
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateUserAccessLoggingSettingsRequestRequestTypeDef(
     _RequiredCreateUserAccessLoggingSettingsRequestRequestTypeDef,
     _OptionalCreateUserAccessLoggingSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateUserSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserSettingsRequestRequestTypeDef",
     {
         "copyAllowed": EnabledTypeType,
         "downloadAllowed": EnabledTypeType,
         "pasteAllowed": EnabledTypeType,
         "printAllowed": EnabledTypeType,
@@ -1254,27 +1324,21 @@
         "disconnectTimeoutInMinutes": int,
         "idleDisconnectTimeoutInMinutes": int,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateUserSettingsRequestRequestTypeDef(
     _RequiredCreateUserSettingsRequestRequestTypeDef,
     _OptionalCreateUserSettingsRequestRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
@@ -1283,19 +1347,21 @@
     "_OptionalTagResourceRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class TagResourceRequestRequestTypeDef(
     _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIpAccessSettingsRequestRequestTypeDef",
     {
         "ipRules": Sequence[IpRuleTypeDef],
     },
 )
 _OptionalCreateIpAccessSettingsRequestRequestTypeDef = TypedDict(
@@ -1307,40 +1373,21 @@
         "description": str,
         "displayName": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateIpAccessSettingsRequestRequestTypeDef(
     _RequiredCreateIpAccessSettingsRequestRequestTypeDef,
     _OptionalCreateIpAccessSettingsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredIpAccessSettingsTypeDef = TypedDict(
-    "_RequiredIpAccessSettingsTypeDef",
-    {
-        "ipAccessSettingsArn": str,
-    },
-)
-_OptionalIpAccessSettingsTypeDef = TypedDict(
-    "_OptionalIpAccessSettingsTypeDef",
-    {
-        "associatedPortalArns": List[str],
-        "creationDate": datetime,
-        "description": str,
-        "displayName": str,
-        "ipRules": List[IpRuleTypeDef],
-    },
-    total=False,
-)
-
-class IpAccessSettingsTypeDef(_RequiredIpAccessSettingsTypeDef, _OptionalIpAccessSettingsTypeDef):
-    pass
 
 _RequiredUpdateIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIpAccessSettingsRequestRequestTypeDef",
     {
         "ipAccessSettingsArn": str,
     },
 )
@@ -1351,179 +1398,212 @@
         "description": str,
         "displayName": str,
         "ipRules": Sequence[IpRuleTypeDef],
     },
     total=False,
 )
 
+
 class UpdateIpAccessSettingsRequestRequestTypeDef(
     _RequiredUpdateIpAccessSettingsRequestRequestTypeDef,
     _OptionalUpdateIpAccessSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 GetIdentityProviderResponseTypeDef = TypedDict(
     "GetIdentityProviderResponseTypeDef",
     {
         "identityProvider": IdentityProviderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIdentityProviderResponseTypeDef = TypedDict(
     "UpdateIdentityProviderResponseTypeDef",
     {
         "identityProvider": IdentityProviderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNetworkSettingsResponseTypeDef = TypedDict(
     "GetNetworkSettingsResponseTypeDef",
     {
         "networkSettings": NetworkSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNetworkSettingsResponseTypeDef = TypedDict(
     "UpdateNetworkSettingsResponseTypeDef",
     {
         "networkSettings": NetworkSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPortalResponseTypeDef = TypedDict(
     "GetPortalResponseTypeDef",
     {
         "portal": PortalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePortalResponseTypeDef = TypedDict(
     "UpdatePortalResponseTypeDef",
     {
         "portal": PortalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTrustStoreResponseTypeDef = TypedDict(
     "GetTrustStoreResponseTypeDef",
     {
         "trustStore": TrustStoreTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserAccessLoggingSettingsResponseTypeDef = TypedDict(
     "GetUserAccessLoggingSettingsResponseTypeDef",
     {
         "userAccessLoggingSettings": UserAccessLoggingSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
     "UpdateUserAccessLoggingSettingsResponseTypeDef",
     {
         "userAccessLoggingSettings": UserAccessLoggingSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserSettingsResponseTypeDef = TypedDict(
     "GetUserSettingsResponseTypeDef",
     {
         "userSettings": UserSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserSettingsResponseTypeDef = TypedDict(
     "UpdateUserSettingsResponseTypeDef",
     {
         "userSettings": UserSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentityProvidersResponseTypeDef = TypedDict(
     "ListIdentityProvidersResponseTypeDef",
     {
         "identityProviders": List[IdentityProviderSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIpAccessSettingsResponseTypeDef = TypedDict(
     "ListIpAccessSettingsResponseTypeDef",
     {
         "ipAccessSettings": List[IpAccessSettingsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredIpAccessSettingsTypeDef = TypedDict(
+    "_RequiredIpAccessSettingsTypeDef",
+    {
+        "ipAccessSettingsArn": str,
     },
 )
+_OptionalIpAccessSettingsTypeDef = TypedDict(
+    "_OptionalIpAccessSettingsTypeDef",
+    {
+        "associatedPortalArns": List[str],
+        "creationDate": datetime,
+        "description": str,
+        "displayName": str,
+        "ipRules": List[IpRuleOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class IpAccessSettingsTypeDef(_RequiredIpAccessSettingsTypeDef, _OptionalIpAccessSettingsTypeDef):
+    pass
+
 
 ListNetworkSettingsResponseTypeDef = TypedDict(
     "ListNetworkSettingsResponseTypeDef",
     {
         "networkSettings": List[NetworkSettingsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPortalsResponseTypeDef = TypedDict(
     "ListPortalsResponseTypeDef",
     {
         "nextToken": str,
         "portals": List[PortalSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrustStoresResponseTypeDef = TypedDict(
     "ListTrustStoresResponseTypeDef",
     {
         "nextToken": str,
         "trustStores": List[TrustStoreSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserAccessLoggingSettingsResponseTypeDef = TypedDict(
     "ListUserAccessLoggingSettingsResponseTypeDef",
     {
         "nextToken": str,
         "userAccessLoggingSettings": List[UserAccessLoggingSettingsSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserSettingsResponseTypeDef = TypedDict(
     "ListUserSettingsResponseTypeDef",
     {
         "nextToken": str,
         "userSettings": List[UserSettingsSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIpAccessSettingsResponseTypeDef = TypedDict(
     "GetIpAccessSettingsResponseTypeDef",
     {
         "ipAccessSettings": IpAccessSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIpAccessSettingsResponseTypeDef = TypedDict(
     "UpdateIpAccessSettingsResponseTypeDef",
     {
         "ipAccessSettings": IpAccessSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web.egg-info/PKG-INFO` & `mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces-web
-Version: 1.28.0
-Summary: Type annotations for boto3.WorkSpacesWeb 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.WorkSpacesWeb 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-workspaces-web"></a>
 
 # mypy-boto3-workspaces-web
 
 [![PyPI - mypy-boto3-workspaces-web](https://img.shields.io/pypi/v/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces-web?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces-web)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces-web)](https://pepy.tech/project/mypy-boto3-workspaces-web)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpacesWeb 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
+[boto3.WorkSpacesWeb 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
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
 [mypy-boto3-workspaces-web docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,40 +304,27 @@
 
 `mypy_boto3_workspaces_web.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workspaces_web.type_defs import (
     AssociateBrowserSettingsRequestRequestTypeDef,
-    AssociateBrowserSettingsResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociateIpAccessSettingsRequestRequestTypeDef,
-    AssociateIpAccessSettingsResponseTypeDef,
     AssociateNetworkSettingsRequestRequestTypeDef,
-    AssociateNetworkSettingsResponseTypeDef,
     AssociateTrustStoreRequestRequestTypeDef,
-    AssociateTrustStoreResponseTypeDef,
     AssociateUserAccessLoggingSettingsRequestRequestTypeDef,
-    AssociateUserAccessLoggingSettingsResponseTypeDef,
     AssociateUserSettingsRequestRequestTypeDef,
-    AssociateUserSettingsResponseTypeDef,
     BrowserSettingsSummaryTypeDef,
     BrowserSettingsTypeDef,
     CertificateSummaryTypeDef,
     CertificateTypeDef,
     TagTypeDef,
-    CreateBrowserSettingsResponseTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
-    CreateIdentityProviderResponseTypeDef,
     IpRuleTypeDef,
-    CreateIpAccessSettingsResponseTypeDef,
-    CreateNetworkSettingsResponseTypeDef,
-    CreatePortalResponseTypeDef,
-    CreateTrustStoreResponseTypeDef,
-    CreateUserAccessLoggingSettingsResponseTypeDef,
-    CreateUserSettingsResponseTypeDef,
     DeleteBrowserSettingsRequestRequestTypeDef,
     DeleteIdentityProviderRequestRequestTypeDef,
     DeleteIpAccessSettingsRequestRequestTypeDef,
     DeleteNetworkSettingsRequestRequestTypeDef,
     DeletePortalRequestRequestTypeDef,
     DeleteTrustStoreRequestRequestTypeDef,
     DeleteUserAccessLoggingSettingsRequestRequestTypeDef,
@@ -353,80 +340,95 @@
     IdentityProviderTypeDef,
     GetIpAccessSettingsRequestRequestTypeDef,
     GetNetworkSettingsRequestRequestTypeDef,
     NetworkSettingsTypeDef,
     GetPortalRequestRequestTypeDef,
     PortalTypeDef,
     GetPortalServiceProviderMetadataRequestRequestTypeDef,
-    GetPortalServiceProviderMetadataResponseTypeDef,
     GetTrustStoreCertificateRequestRequestTypeDef,
     GetTrustStoreRequestRequestTypeDef,
     TrustStoreTypeDef,
     GetUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsTypeDef,
     GetUserSettingsRequestRequestTypeDef,
     UserSettingsTypeDef,
     IdentityProviderSummaryTypeDef,
     IpAccessSettingsSummaryTypeDef,
+    IpRuleOutputTypeDef,
     ListBrowserSettingsRequestRequestTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
     ListIpAccessSettingsRequestRequestTypeDef,
     ListNetworkSettingsRequestRequestTypeDef,
     NetworkSettingsSummaryTypeDef,
     ListPortalsRequestRequestTypeDef,
     PortalSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListTrustStoreCertificatesRequestRequestTypeDef,
     ListTrustStoresRequestRequestTypeDef,
     TrustStoreSummaryTypeDef,
     ListUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsSummaryTypeDef,
     ListUserSettingsRequestRequestTypeDef,
     UserSettingsSummaryTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrowserSettingsRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
     UpdateNetworkSettingsRequestRequestTypeDef,
     UpdatePortalRequestRequestTypeDef,
     UpdateTrustStoreRequestRequestTypeDef,
-    UpdateTrustStoreResponseTypeDef,
     UpdateUserAccessLoggingSettingsRequestRequestTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
+    AssociateBrowserSettingsResponseTypeDef,
+    AssociateIpAccessSettingsResponseTypeDef,
+    AssociateNetworkSettingsResponseTypeDef,
+    AssociateTrustStoreResponseTypeDef,
+    AssociateUserAccessLoggingSettingsResponseTypeDef,
+    AssociateUserSettingsResponseTypeDef,
+    CreateBrowserSettingsResponseTypeDef,
+    CreateIdentityProviderResponseTypeDef,
+    CreateIpAccessSettingsResponseTypeDef,
+    CreateNetworkSettingsResponseTypeDef,
+    CreatePortalResponseTypeDef,
+    CreateTrustStoreResponseTypeDef,
+    CreateUserAccessLoggingSettingsResponseTypeDef,
+    CreateUserSettingsResponseTypeDef,
+    GetPortalServiceProviderMetadataResponseTypeDef,
+    UpdateTrustStoreResponseTypeDef,
     ListBrowserSettingsResponseTypeDef,
     GetBrowserSettingsResponseTypeDef,
     UpdateBrowserSettingsResponseTypeDef,
     ListTrustStoreCertificatesResponseTypeDef,
     GetTrustStoreCertificateResponseTypeDef,
     CreateBrowserSettingsRequestRequestTypeDef,
     CreateNetworkSettingsRequestRequestTypeDef,
     CreatePortalRequestRequestTypeDef,
     CreateTrustStoreRequestRequestTypeDef,
     CreateUserAccessLoggingSettingsRequestRequestTypeDef,
     CreateUserSettingsRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIpAccessSettingsRequestRequestTypeDef,
-    IpAccessSettingsTypeDef,
     UpdateIpAccessSettingsRequestRequestTypeDef,
     GetIdentityProviderResponseTypeDef,
     UpdateIdentityProviderResponseTypeDef,
     GetNetworkSettingsResponseTypeDef,
     UpdateNetworkSettingsResponseTypeDef,
     GetPortalResponseTypeDef,
     UpdatePortalResponseTypeDef,
     GetTrustStoreResponseTypeDef,
     GetUserAccessLoggingSettingsResponseTypeDef,
     UpdateUserAccessLoggingSettingsResponseTypeDef,
     GetUserSettingsResponseTypeDef,
     UpdateUserSettingsResponseTypeDef,
     ListIdentityProvidersResponseTypeDef,
     ListIpAccessSettingsResponseTypeDef,
+    IpAccessSettingsTypeDef,
     ListNetworkSettingsResponseTypeDef,
     ListPortalsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTrustStoresResponseTypeDef,
     ListUserAccessLoggingSettingsResponseTypeDef,
     ListUserSettingsResponseTypeDef,
     GetIpAccessSettingsResponseTypeDef,
     UpdateIpAccessSettingsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-workspaces-web-1.28.0/mypy_boto3_workspaces_web.egg-info/SOURCES.txt` & `mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-web-1.28.0/setup.py` & `mypy-boto3-workspaces-web-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-workspaces-web",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_workspaces_web"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WorkSpacesWeb 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.WorkSpacesWeb 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

