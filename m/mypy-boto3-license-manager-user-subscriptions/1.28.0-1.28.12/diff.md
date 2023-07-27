# Comparing `tmp/mypy-boto3-license-manager-user-subscriptions-1.28.0.tar.gz` & `tmp/mypy-boto3-license-manager-user-subscriptions-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-license-manager-user-subscriptions-1.28.0.tar", last modified: Thu Jul  6 20:59:59 2023, max compression
+gzip compressed data, was "mypy-boto3-license-manager-user-subscriptions-1.28.12.tar", last modified: Thu Jul 27 05:34:56 2023, max compression
```

## Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.0.tar` & `mypy-boto3-license-manager-user-subscriptions-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:59.350353 mypy-boto3-license-manager-user-subscriptions-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:45:47.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-07-06 20:59:59.350353 mypy-boto3-license-manager-user-subscriptions-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14623 2023-07-06 20:45:47.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:59.334353 mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-06 20:45:47.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-06 20:45:47.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-06 20:45:47.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-07-06 20:45:47.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-07-06 20:45:47.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-07-06 20:45:47.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-07-06 20:45:47.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-06 20:45:47.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-07-06 20:45:47.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:45:47.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15859 2023-07-06 20:45:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-07-06 20:45:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:45:47.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:59.350353 mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-07-06 20:59:59.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-06 20:59:59.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:59.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:59.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:59.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-06 20:59:59.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:59.350353 mypy-boto3-license-manager-user-subscriptions-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-06 20:45:47.000000 mypy-boto3-license-manager-user-subscriptions-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:56.940456 mypy-boto3-license-manager-user-subscriptions-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-07-27 05:34:56.940456 mypy-boto3-license-manager-user-subscriptions-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14726 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:56.932456 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16532 2023-07-27 05:25:22.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16503 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:56.940456 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:56.940456 mypy-boto3-license-manager-user-subscriptions-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/setup.py
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.0/LICENSE` & `mypy-boto3-license-manager-user-subscriptions-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.0/PKG-INFO` & `mypy-boto3-license-manager-user-subscriptions-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager-user-subscriptions
-Version: 1.28.0
-Summary: Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-license-manager-user-subscriptions"></a>
 
 # mypy-boto3-license-manager-user-subscriptions
 
 [![PyPI - mypy-boto3-license-manager-user-subscriptions](https://img.shields.io/pypi/v/mypy-boto3-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-user-subscriptions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-user-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-license-manager-user-subscriptions?color=blue)](https://pypistats.org/packages/mypy-boto3-license-manager-user-subscriptions)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager-user-subscriptions)](https://pepy.tech/project/mypy-boto3-license-manager-user-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerUserSubscriptions 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
+[boto3.LicenseManagerUserSubscriptions 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
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
 [mypy-boto3-license-manager-user-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -346,37 +346,40 @@
 
 `mypy_boto3_license_manager_user_subscriptions.type_defs` module contains
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_license_manager_user_subscriptions.type_defs import (
+    ActiveDirectoryIdentityProviderOutputTypeDef,
     ActiveDirectoryIdentityProviderTypeDef,
     FilterTypeDef,
-    SettingsTypeDef,
+    SettingsOutputTypeDef,
     InstanceSummaryTypeDef,
     ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    SettingsTypeDef,
     ResponseMetadataTypeDef,
     UpdateSettingsTypeDef,
+    IdentityProviderOutputTypeDef,
     IdentityProviderTypeDef,
     ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
+    IdentityProviderSummaryTypeDef,
+    InstanceUserSummaryTypeDef,
+    ProductUserSummaryTypeDef,
     AssociateUserRequestRequestTypeDef,
     DeregisterIdentityProviderRequestRequestTypeDef,
     DisassociateUserRequestRequestTypeDef,
-    IdentityProviderSummaryTypeDef,
-    InstanceUserSummaryTypeDef,
     ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
     ListProductSubscriptionsRequestRequestTypeDef,
     ListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
     ListUserAssociationsRequestRequestTypeDef,
-    ProductUserSummaryTypeDef,
     RegisterIdentityProviderRequestRequestTypeDef,
     StartProductSubscriptionRequestRequestTypeDef,
     StopProductSubscriptionRequestRequestTypeDef,
     UpdateIdentityProviderSettingsRequestRequestTypeDef,
     DeregisterIdentityProviderResponseTypeDef,
     ListIdentityProvidersResponseTypeDef,
     RegisterIdentityProviderResponseTypeDef,
@@ -386,15 +389,15 @@
     ListUserAssociationsResponseTypeDef,
     ListProductSubscriptionsResponseTypeDef,
     StartProductSubscriptionResponseTypeDef,
     StopProductSubscriptionResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveDirectoryIdentityProviderTypeDef:
+def get_structure() -> ActiveDirectoryIdentityProviderOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.0/README.md` & `mypy-boto3-license-manager-user-subscriptions-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-license-manager-user-subscriptions"></a>
 
 # mypy-boto3-license-manager-user-subscriptions
 
 [![PyPI - mypy-boto3-license-manager-user-subscriptions](https://img.shields.io/pypi/v/mypy-boto3-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-user-subscriptions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-user-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-license-manager-user-subscriptions?color=blue)](https://pypistats.org/packages/mypy-boto3-license-manager-user-subscriptions)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager-user-subscriptions)](https://pepy.tech/project/mypy-boto3-license-manager-user-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerUserSubscriptions 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
+[boto3.LicenseManagerUserSubscriptions 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
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
 [mypy-boto3-license-manager-user-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -314,37 +314,40 @@
 
 `mypy_boto3_license_manager_user_subscriptions.type_defs` module contains
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_license_manager_user_subscriptions.type_defs import (
+    ActiveDirectoryIdentityProviderOutputTypeDef,
     ActiveDirectoryIdentityProviderTypeDef,
     FilterTypeDef,
-    SettingsTypeDef,
+    SettingsOutputTypeDef,
     InstanceSummaryTypeDef,
     ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    SettingsTypeDef,
     ResponseMetadataTypeDef,
     UpdateSettingsTypeDef,
+    IdentityProviderOutputTypeDef,
     IdentityProviderTypeDef,
     ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
+    IdentityProviderSummaryTypeDef,
+    InstanceUserSummaryTypeDef,
+    ProductUserSummaryTypeDef,
     AssociateUserRequestRequestTypeDef,
     DeregisterIdentityProviderRequestRequestTypeDef,
     DisassociateUserRequestRequestTypeDef,
-    IdentityProviderSummaryTypeDef,
-    InstanceUserSummaryTypeDef,
     ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
     ListProductSubscriptionsRequestRequestTypeDef,
     ListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
     ListUserAssociationsRequestRequestTypeDef,
-    ProductUserSummaryTypeDef,
     RegisterIdentityProviderRequestRequestTypeDef,
     StartProductSubscriptionRequestRequestTypeDef,
     StopProductSubscriptionRequestRequestTypeDef,
     UpdateIdentityProviderSettingsRequestRequestTypeDef,
     DeregisterIdentityProviderResponseTypeDef,
     ListIdentityProvidersResponseTypeDef,
     RegisterIdentityProviderResponseTypeDef,
@@ -354,15 +357,15 @@
     ListUserAssociationsResponseTypeDef,
     ListProductSubscriptionsResponseTypeDef,
     StartProductSubscriptionResponseTypeDef,
     StopProductSubscriptionResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveDirectoryIdentityProviderTypeDef:
+def get_structure() -> ActiveDirectoryIdentityProviderOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/__init__.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/__init__.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/__main__.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.0\nVersion:        "
-        " 1.28.0\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.12\nVersion:        "
+        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions\nOther"
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

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/client.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/client.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/literals.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,15 @@
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
@@ -238,26 +239,28 @@
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

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/literals.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,15 @@
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
@@ -236,26 +237,28 @@
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

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/paginator.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/paginator.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/type_defs.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,52 +2,54 @@
 Type annotations for license-manager-user-subscriptions service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_license_manager_user_subscriptions.type_defs import ActiveDirectoryIdentityProviderTypeDef
+    from mypy_boto3_license_manager_user_subscriptions.type_defs import ActiveDirectoryIdentityProviderOutputTypeDef
 
-    data: ActiveDirectoryIdentityProviderTypeDef = {...}
+    data: ActiveDirectoryIdentityProviderOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "ActiveDirectoryIdentityProviderOutputTypeDef",
     "ActiveDirectoryIdentityProviderTypeDef",
     "FilterTypeDef",
-    "SettingsTypeDef",
+    "SettingsOutputTypeDef",
     "InstanceSummaryTypeDef",
     "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
+    "SettingsTypeDef",
     "ResponseMetadataTypeDef",
     "UpdateSettingsTypeDef",
+    "IdentityProviderOutputTypeDef",
     "IdentityProviderTypeDef",
     "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "ListInstancesResponseTypeDef",
+    "IdentityProviderSummaryTypeDef",
+    "InstanceUserSummaryTypeDef",
+    "ProductUserSummaryTypeDef",
     "AssociateUserRequestRequestTypeDef",
     "DeregisterIdentityProviderRequestRequestTypeDef",
     "DisassociateUserRequestRequestTypeDef",
-    "IdentityProviderSummaryTypeDef",
-    "InstanceUserSummaryTypeDef",
     "ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     "ListProductSubscriptionsRequestRequestTypeDef",
     "ListUserAssociationsRequestListUserAssociationsPaginateTypeDef",
     "ListUserAssociationsRequestRequestTypeDef",
-    "ProductUserSummaryTypeDef",
     "RegisterIdentityProviderRequestRequestTypeDef",
     "StartProductSubscriptionRequestRequestTypeDef",
     "StopProductSubscriptionRequestRequestTypeDef",
     "UpdateIdentityProviderSettingsRequestRequestTypeDef",
     "DeregisterIdentityProviderResponseTypeDef",
     "ListIdentityProvidersResponseTypeDef",
     "RegisterIdentityProviderResponseTypeDef",
@@ -56,14 +58,22 @@
     "DisassociateUserResponseTypeDef",
     "ListUserAssociationsResponseTypeDef",
     "ListProductSubscriptionsResponseTypeDef",
     "StartProductSubscriptionResponseTypeDef",
     "StopProductSubscriptionResponseTypeDef",
 )
 
+ActiveDirectoryIdentityProviderOutputTypeDef = TypedDict(
+    "ActiveDirectoryIdentityProviderOutputTypeDef",
+    {
+        "DirectoryId": str,
+    },
+    total=False,
+)
+
 ActiveDirectoryIdentityProviderTypeDef = TypedDict(
     "ActiveDirectoryIdentityProviderTypeDef",
     {
         "DirectoryId": str,
     },
     total=False,
 )
@@ -74,16 +84,16 @@
         "Attribute": str,
         "Operation": str,
         "Value": str,
     },
     total=False,
 )
 
-SettingsTypeDef = TypedDict(
-    "SettingsTypeDef",
+SettingsOutputTypeDef = TypedDict(
+    "SettingsOutputTypeDef",
     {
         "SecurityGroupId": str,
         "Subnets": List[str],
     },
 )
 
 _RequiredInstanceSummaryTypeDef = TypedDict(
@@ -99,19 +109,17 @@
     {
         "LastStatusCheckDate": str,
         "StatusMessage": str,
     },
     total=False,
 )
 
-
 class InstanceSummaryTypeDef(_RequiredInstanceSummaryTypeDef, _OptionalInstanceSummaryTypeDef):
     pass
 
-
 ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
     "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -131,14 +139,22 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+SettingsTypeDef = TypedDict(
+    "SettingsTypeDef",
+    {
+        "SecurityGroupId": str,
+        "Subnets": Sequence[str],
+    },
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -157,18 +173,24 @@
     "_OptionalUpdateSettingsTypeDef",
     {
         "SecurityGroupId": str,
     },
     total=False,
 )
 
-
 class UpdateSettingsTypeDef(_RequiredUpdateSettingsTypeDef, _OptionalUpdateSettingsTypeDef):
     pass
 
+IdentityProviderOutputTypeDef = TypedDict(
+    "IdentityProviderOutputTypeDef",
+    {
+        "ActiveDirectoryIdentityProvider": ActiveDirectoryIdentityProviderOutputTypeDef,
+    },
+    total=False,
+)
 
 IdentityProviderTypeDef = TypedDict(
     "IdentityProviderTypeDef",
     {
         "ActiveDirectoryIdentityProvider": ActiveDirectoryIdentityProviderTypeDef,
     },
     total=False,
@@ -198,119 +220,136 @@
     {
         "InstanceSummaries": List[InstanceSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredAssociateUserRequestRequestTypeDef = TypedDict(
-    "_RequiredAssociateUserRequestRequestTypeDef",
+_RequiredIdentityProviderSummaryTypeDef = TypedDict(
+    "_RequiredIdentityProviderSummaryTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeDef,
-        "InstanceId": str,
-        "Username": str,
+        "IdentityProvider": IdentityProviderOutputTypeDef,
+        "Product": str,
+        "Settings": SettingsOutputTypeDef,
+        "Status": str,
     },
 )
-_OptionalAssociateUserRequestRequestTypeDef = TypedDict(
-    "_OptionalAssociateUserRequestRequestTypeDef",
+_OptionalIdentityProviderSummaryTypeDef = TypedDict(
+    "_OptionalIdentityProviderSummaryTypeDef",
     {
-        "Domain": str,
+        "FailureMessage": str,
     },
     total=False,
 )
 
-
-class AssociateUserRequestRequestTypeDef(
-    _RequiredAssociateUserRequestRequestTypeDef, _OptionalAssociateUserRequestRequestTypeDef
+class IdentityProviderSummaryTypeDef(
+    _RequiredIdentityProviderSummaryTypeDef, _OptionalIdentityProviderSummaryTypeDef
 ):
     pass
 
-
-DeregisterIdentityProviderRequestRequestTypeDef = TypedDict(
-    "DeregisterIdentityProviderRequestRequestTypeDef",
+_RequiredInstanceUserSummaryTypeDef = TypedDict(
+    "_RequiredInstanceUserSummaryTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeDef,
-        "Product": str,
+        "IdentityProvider": IdentityProviderOutputTypeDef,
+        "InstanceId": str,
+        "Status": str,
+        "Username": str,
+    },
+)
+_OptionalInstanceUserSummaryTypeDef = TypedDict(
+    "_OptionalInstanceUserSummaryTypeDef",
+    {
+        "AssociationDate": str,
+        "DisassociationDate": str,
+        "Domain": str,
+        "StatusMessage": str,
     },
+    total=False,
 )
 
-_RequiredDisassociateUserRequestRequestTypeDef = TypedDict(
-    "_RequiredDisassociateUserRequestRequestTypeDef",
+class InstanceUserSummaryTypeDef(
+    _RequiredInstanceUserSummaryTypeDef, _OptionalInstanceUserSummaryTypeDef
+):
+    pass
+
+_RequiredProductUserSummaryTypeDef = TypedDict(
+    "_RequiredProductUserSummaryTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeDef,
-        "InstanceId": str,
+        "IdentityProvider": IdentityProviderOutputTypeDef,
+        "Product": str,
+        "Status": str,
         "Username": str,
     },
 )
-_OptionalDisassociateUserRequestRequestTypeDef = TypedDict(
-    "_OptionalDisassociateUserRequestRequestTypeDef",
+_OptionalProductUserSummaryTypeDef = TypedDict(
+    "_OptionalProductUserSummaryTypeDef",
     {
         "Domain": str,
+        "StatusMessage": str,
+        "SubscriptionEndDate": str,
+        "SubscriptionStartDate": str,
     },
     total=False,
 )
 
-
-class DisassociateUserRequestRequestTypeDef(
-    _RequiredDisassociateUserRequestRequestTypeDef, _OptionalDisassociateUserRequestRequestTypeDef
+class ProductUserSummaryTypeDef(
+    _RequiredProductUserSummaryTypeDef, _OptionalProductUserSummaryTypeDef
 ):
     pass
 
-
-_RequiredIdentityProviderSummaryTypeDef = TypedDict(
-    "_RequiredIdentityProviderSummaryTypeDef",
+_RequiredAssociateUserRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateUserRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
-        "Product": str,
-        "Settings": SettingsTypeDef,
-        "Status": str,
+        "InstanceId": str,
+        "Username": str,
     },
 )
-_OptionalIdentityProviderSummaryTypeDef = TypedDict(
-    "_OptionalIdentityProviderSummaryTypeDef",
+_OptionalAssociateUserRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateUserRequestRequestTypeDef",
     {
-        "FailureMessage": str,
+        "Domain": str,
     },
     total=False,
 )
 
-
-class IdentityProviderSummaryTypeDef(
-    _RequiredIdentityProviderSummaryTypeDef, _OptionalIdentityProviderSummaryTypeDef
+class AssociateUserRequestRequestTypeDef(
+    _RequiredAssociateUserRequestRequestTypeDef, _OptionalAssociateUserRequestRequestTypeDef
 ):
     pass
 
+DeregisterIdentityProviderRequestRequestTypeDef = TypedDict(
+    "DeregisterIdentityProviderRequestRequestTypeDef",
+    {
+        "IdentityProvider": IdentityProviderTypeDef,
+        "Product": str,
+    },
+)
 
-_RequiredInstanceUserSummaryTypeDef = TypedDict(
-    "_RequiredInstanceUserSummaryTypeDef",
+_RequiredDisassociateUserRequestRequestTypeDef = TypedDict(
+    "_RequiredDisassociateUserRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
-        "Status": str,
         "Username": str,
     },
 )
-_OptionalInstanceUserSummaryTypeDef = TypedDict(
-    "_OptionalInstanceUserSummaryTypeDef",
+_OptionalDisassociateUserRequestRequestTypeDef = TypedDict(
+    "_OptionalDisassociateUserRequestRequestTypeDef",
     {
-        "AssociationDate": str,
-        "DisassociationDate": str,
         "Domain": str,
-        "StatusMessage": str,
     },
     total=False,
 )
 
-
-class InstanceUserSummaryTypeDef(
-    _RequiredInstanceUserSummaryTypeDef, _OptionalInstanceUserSummaryTypeDef
+class DisassociateUserRequestRequestTypeDef(
+    _RequiredDisassociateUserRequestRequestTypeDef, _OptionalDisassociateUserRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef = TypedDict(
     "_RequiredListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
     },
 )
@@ -319,22 +358,20 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef(
     _RequiredListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
     _OptionalListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListProductSubscriptionsRequestRequestTypeDef = TypedDict(
     "_RequiredListProductSubscriptionsRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
     },
 )
@@ -344,22 +381,20 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListProductSubscriptionsRequestRequestTypeDef(
     _RequiredListProductSubscriptionsRequestRequestTypeDef,
     _OptionalListProductSubscriptionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListUserAssociationsRequestListUserAssociationsPaginateTypeDef = TypedDict(
     "_RequiredListUserAssociationsRequestListUserAssociationsPaginateTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
     },
 )
@@ -368,22 +403,20 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListUserAssociationsRequestListUserAssociationsPaginateTypeDef(
     _RequiredListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
     _OptionalListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListUserAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserAssociationsRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
     },
 )
@@ -393,49 +426,20 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListUserAssociationsRequestRequestTypeDef(
     _RequiredListUserAssociationsRequestRequestTypeDef,
     _OptionalListUserAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredProductUserSummaryTypeDef = TypedDict(
-    "_RequiredProductUserSummaryTypeDef",
-    {
-        "IdentityProvider": IdentityProviderTypeDef,
-        "Product": str,
-        "Status": str,
-        "Username": str,
-    },
-)
-_OptionalProductUserSummaryTypeDef = TypedDict(
-    "_OptionalProductUserSummaryTypeDef",
-    {
-        "Domain": str,
-        "StatusMessage": str,
-        "SubscriptionEndDate": str,
-        "SubscriptionStartDate": str,
-    },
-    total=False,
-)
-
-
-class ProductUserSummaryTypeDef(
-    _RequiredProductUserSummaryTypeDef, _OptionalProductUserSummaryTypeDef
-):
-    pass
-
-
 _RequiredRegisterIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterIdentityProviderRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
     },
 )
@@ -443,22 +447,20 @@
     "_OptionalRegisterIdentityProviderRequestRequestTypeDef",
     {
         "Settings": SettingsTypeDef,
     },
     total=False,
 )
 
-
 class RegisterIdentityProviderRequestRequestTypeDef(
     _RequiredRegisterIdentityProviderRequestRequestTypeDef,
     _OptionalRegisterIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartProductSubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredStartProductSubscriptionRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
         "Username": str,
     },
@@ -467,22 +469,20 @@
     "_OptionalStartProductSubscriptionRequestRequestTypeDef",
     {
         "Domain": str,
     },
     total=False,
 )
 
-
 class StartProductSubscriptionRequestRequestTypeDef(
     _RequiredStartProductSubscriptionRequestRequestTypeDef,
     _OptionalStartProductSubscriptionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStopProductSubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredStopProductSubscriptionRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
         "Username": str,
     },
@@ -491,22 +491,20 @@
     "_OptionalStopProductSubscriptionRequestRequestTypeDef",
     {
         "Domain": str,
     },
     total=False,
 )
 
-
 class StopProductSubscriptionRequestRequestTypeDef(
     _RequiredStopProductSubscriptionRequestRequestTypeDef,
     _OptionalStopProductSubscriptionRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateIdentityProviderSettingsRequestRequestTypeDef = TypedDict(
     "UpdateIdentityProviderSettingsRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
         "UpdateSettings": UpdateSettingsTypeDef,
     },
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions/type_defs.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,51 +2,55 @@
 Type annotations for license-manager-user-subscriptions service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_license_manager_user_subscriptions.type_defs import ActiveDirectoryIdentityProviderTypeDef
+    from mypy_boto3_license_manager_user_subscriptions.type_defs import ActiveDirectoryIdentityProviderOutputTypeDef
 
-    data: ActiveDirectoryIdentityProviderTypeDef = {...}
+    data: ActiveDirectoryIdentityProviderOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "ActiveDirectoryIdentityProviderOutputTypeDef",
     "ActiveDirectoryIdentityProviderTypeDef",
     "FilterTypeDef",
-    "SettingsTypeDef",
+    "SettingsOutputTypeDef",
     "InstanceSummaryTypeDef",
     "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
+    "SettingsTypeDef",
     "ResponseMetadataTypeDef",
     "UpdateSettingsTypeDef",
+    "IdentityProviderOutputTypeDef",
     "IdentityProviderTypeDef",
     "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "ListInstancesResponseTypeDef",
+    "IdentityProviderSummaryTypeDef",
+    "InstanceUserSummaryTypeDef",
+    "ProductUserSummaryTypeDef",
     "AssociateUserRequestRequestTypeDef",
     "DeregisterIdentityProviderRequestRequestTypeDef",
     "DisassociateUserRequestRequestTypeDef",
-    "IdentityProviderSummaryTypeDef",
-    "InstanceUserSummaryTypeDef",
     "ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     "ListProductSubscriptionsRequestRequestTypeDef",
     "ListUserAssociationsRequestListUserAssociationsPaginateTypeDef",
     "ListUserAssociationsRequestRequestTypeDef",
-    "ProductUserSummaryTypeDef",
     "RegisterIdentityProviderRequestRequestTypeDef",
     "StartProductSubscriptionRequestRequestTypeDef",
     "StopProductSubscriptionRequestRequestTypeDef",
     "UpdateIdentityProviderSettingsRequestRequestTypeDef",
     "DeregisterIdentityProviderResponseTypeDef",
     "ListIdentityProvidersResponseTypeDef",
     "RegisterIdentityProviderResponseTypeDef",
@@ -55,14 +59,22 @@
     "DisassociateUserResponseTypeDef",
     "ListUserAssociationsResponseTypeDef",
     "ListProductSubscriptionsResponseTypeDef",
     "StartProductSubscriptionResponseTypeDef",
     "StopProductSubscriptionResponseTypeDef",
 )
 
+ActiveDirectoryIdentityProviderOutputTypeDef = TypedDict(
+    "ActiveDirectoryIdentityProviderOutputTypeDef",
+    {
+        "DirectoryId": str,
+    },
+    total=False,
+)
+
 ActiveDirectoryIdentityProviderTypeDef = TypedDict(
     "ActiveDirectoryIdentityProviderTypeDef",
     {
         "DirectoryId": str,
     },
     total=False,
 )
@@ -73,16 +85,16 @@
         "Attribute": str,
         "Operation": str,
         "Value": str,
     },
     total=False,
 )
 
-SettingsTypeDef = TypedDict(
-    "SettingsTypeDef",
+SettingsOutputTypeDef = TypedDict(
+    "SettingsOutputTypeDef",
     {
         "SecurityGroupId": str,
         "Subnets": List[str],
     },
 )
 
 _RequiredInstanceSummaryTypeDef = TypedDict(
@@ -98,17 +110,19 @@
     {
         "LastStatusCheckDate": str,
         "StatusMessage": str,
     },
     total=False,
 )
 
+
 class InstanceSummaryTypeDef(_RequiredInstanceSummaryTypeDef, _OptionalInstanceSummaryTypeDef):
     pass
 
+
 ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
     "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -128,14 +142,22 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+SettingsTypeDef = TypedDict(
+    "SettingsTypeDef",
+    {
+        "SecurityGroupId": str,
+        "Subnets": Sequence[str],
+    },
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -154,17 +176,27 @@
     "_OptionalUpdateSettingsTypeDef",
     {
         "SecurityGroupId": str,
     },
     total=False,
 )
 
+
 class UpdateSettingsTypeDef(_RequiredUpdateSettingsTypeDef, _OptionalUpdateSettingsTypeDef):
     pass
 
+
+IdentityProviderOutputTypeDef = TypedDict(
+    "IdentityProviderOutputTypeDef",
+    {
+        "ActiveDirectoryIdentityProvider": ActiveDirectoryIdentityProviderOutputTypeDef,
+    },
+    total=False,
+)
+
 IdentityProviderTypeDef = TypedDict(
     "IdentityProviderTypeDef",
     {
         "ActiveDirectoryIdentityProvider": ActiveDirectoryIdentityProviderTypeDef,
     },
     total=False,
 )
@@ -193,111 +225,146 @@
     {
         "InstanceSummaries": List[InstanceSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredAssociateUserRequestRequestTypeDef = TypedDict(
-    "_RequiredAssociateUserRequestRequestTypeDef",
+_RequiredIdentityProviderSummaryTypeDef = TypedDict(
+    "_RequiredIdentityProviderSummaryTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeDef,
-        "InstanceId": str,
-        "Username": str,
+        "IdentityProvider": IdentityProviderOutputTypeDef,
+        "Product": str,
+        "Settings": SettingsOutputTypeDef,
+        "Status": str,
     },
 )
-_OptionalAssociateUserRequestRequestTypeDef = TypedDict(
-    "_OptionalAssociateUserRequestRequestTypeDef",
+_OptionalIdentityProviderSummaryTypeDef = TypedDict(
+    "_OptionalIdentityProviderSummaryTypeDef",
     {
-        "Domain": str,
+        "FailureMessage": str,
     },
     total=False,
 )
 
-class AssociateUserRequestRequestTypeDef(
-    _RequiredAssociateUserRequestRequestTypeDef, _OptionalAssociateUserRequestRequestTypeDef
+
+class IdentityProviderSummaryTypeDef(
+    _RequiredIdentityProviderSummaryTypeDef, _OptionalIdentityProviderSummaryTypeDef
 ):
     pass
 
-DeregisterIdentityProviderRequestRequestTypeDef = TypedDict(
-    "DeregisterIdentityProviderRequestRequestTypeDef",
+
+_RequiredInstanceUserSummaryTypeDef = TypedDict(
+    "_RequiredInstanceUserSummaryTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeDef,
-        "Product": str,
+        "IdentityProvider": IdentityProviderOutputTypeDef,
+        "InstanceId": str,
+        "Status": str,
+        "Username": str,
+    },
+)
+_OptionalInstanceUserSummaryTypeDef = TypedDict(
+    "_OptionalInstanceUserSummaryTypeDef",
+    {
+        "AssociationDate": str,
+        "DisassociationDate": str,
+        "Domain": str,
+        "StatusMessage": str,
     },
+    total=False,
 )
 
-_RequiredDisassociateUserRequestRequestTypeDef = TypedDict(
-    "_RequiredDisassociateUserRequestRequestTypeDef",
+
+class InstanceUserSummaryTypeDef(
+    _RequiredInstanceUserSummaryTypeDef, _OptionalInstanceUserSummaryTypeDef
+):
+    pass
+
+
+_RequiredProductUserSummaryTypeDef = TypedDict(
+    "_RequiredProductUserSummaryTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeDef,
-        "InstanceId": str,
+        "IdentityProvider": IdentityProviderOutputTypeDef,
+        "Product": str,
+        "Status": str,
         "Username": str,
     },
 )
-_OptionalDisassociateUserRequestRequestTypeDef = TypedDict(
-    "_OptionalDisassociateUserRequestRequestTypeDef",
+_OptionalProductUserSummaryTypeDef = TypedDict(
+    "_OptionalProductUserSummaryTypeDef",
     {
         "Domain": str,
+        "StatusMessage": str,
+        "SubscriptionEndDate": str,
+        "SubscriptionStartDate": str,
     },
     total=False,
 )
 
-class DisassociateUserRequestRequestTypeDef(
-    _RequiredDisassociateUserRequestRequestTypeDef, _OptionalDisassociateUserRequestRequestTypeDef
+
+class ProductUserSummaryTypeDef(
+    _RequiredProductUserSummaryTypeDef, _OptionalProductUserSummaryTypeDef
 ):
     pass
 
-_RequiredIdentityProviderSummaryTypeDef = TypedDict(
-    "_RequiredIdentityProviderSummaryTypeDef",
+
+_RequiredAssociateUserRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateUserRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
-        "Product": str,
-        "Settings": SettingsTypeDef,
-        "Status": str,
+        "InstanceId": str,
+        "Username": str,
     },
 )
-_OptionalIdentityProviderSummaryTypeDef = TypedDict(
-    "_OptionalIdentityProviderSummaryTypeDef",
+_OptionalAssociateUserRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateUserRequestRequestTypeDef",
     {
-        "FailureMessage": str,
+        "Domain": str,
     },
     total=False,
 )
 
-class IdentityProviderSummaryTypeDef(
-    _RequiredIdentityProviderSummaryTypeDef, _OptionalIdentityProviderSummaryTypeDef
+
+class AssociateUserRequestRequestTypeDef(
+    _RequiredAssociateUserRequestRequestTypeDef, _OptionalAssociateUserRequestRequestTypeDef
 ):
     pass
 
-_RequiredInstanceUserSummaryTypeDef = TypedDict(
-    "_RequiredInstanceUserSummaryTypeDef",
+
+DeregisterIdentityProviderRequestRequestTypeDef = TypedDict(
+    "DeregisterIdentityProviderRequestRequestTypeDef",
+    {
+        "IdentityProvider": IdentityProviderTypeDef,
+        "Product": str,
+    },
+)
+
+_RequiredDisassociateUserRequestRequestTypeDef = TypedDict(
+    "_RequiredDisassociateUserRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
-        "Status": str,
         "Username": str,
     },
 )
-_OptionalInstanceUserSummaryTypeDef = TypedDict(
-    "_OptionalInstanceUserSummaryTypeDef",
+_OptionalDisassociateUserRequestRequestTypeDef = TypedDict(
+    "_OptionalDisassociateUserRequestRequestTypeDef",
     {
-        "AssociationDate": str,
-        "DisassociationDate": str,
         "Domain": str,
-        "StatusMessage": str,
     },
     total=False,
 )
 
-class InstanceUserSummaryTypeDef(
-    _RequiredInstanceUserSummaryTypeDef, _OptionalInstanceUserSummaryTypeDef
+
+class DisassociateUserRequestRequestTypeDef(
+    _RequiredDisassociateUserRequestRequestTypeDef, _OptionalDisassociateUserRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef = TypedDict(
     "_RequiredListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
     },
 )
@@ -306,20 +373,22 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef(
     _RequiredListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
     _OptionalListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListProductSubscriptionsRequestRequestTypeDef = TypedDict(
     "_RequiredListProductSubscriptionsRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
     },
 )
@@ -329,20 +398,22 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListProductSubscriptionsRequestRequestTypeDef(
     _RequiredListProductSubscriptionsRequestRequestTypeDef,
     _OptionalListProductSubscriptionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListUserAssociationsRequestListUserAssociationsPaginateTypeDef = TypedDict(
     "_RequiredListUserAssociationsRequestListUserAssociationsPaginateTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
     },
 )
@@ -351,20 +422,22 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListUserAssociationsRequestListUserAssociationsPaginateTypeDef(
     _RequiredListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
     _OptionalListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListUserAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserAssociationsRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
     },
 )
@@ -374,44 +447,21 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListUserAssociationsRequestRequestTypeDef(
     _RequiredListUserAssociationsRequestRequestTypeDef,
     _OptionalListUserAssociationsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredProductUserSummaryTypeDef = TypedDict(
-    "_RequiredProductUserSummaryTypeDef",
-    {
-        "IdentityProvider": IdentityProviderTypeDef,
-        "Product": str,
-        "Status": str,
-        "Username": str,
-    },
-)
-_OptionalProductUserSummaryTypeDef = TypedDict(
-    "_OptionalProductUserSummaryTypeDef",
-    {
-        "Domain": str,
-        "StatusMessage": str,
-        "SubscriptionEndDate": str,
-        "SubscriptionStartDate": str,
-    },
-    total=False,
-)
-
-class ProductUserSummaryTypeDef(
-    _RequiredProductUserSummaryTypeDef, _OptionalProductUserSummaryTypeDef
-):
-    pass
 
 _RequiredRegisterIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterIdentityProviderRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
     },
@@ -420,20 +470,22 @@
     "_OptionalRegisterIdentityProviderRequestRequestTypeDef",
     {
         "Settings": SettingsTypeDef,
     },
     total=False,
 )
 
+
 class RegisterIdentityProviderRequestRequestTypeDef(
     _RequiredRegisterIdentityProviderRequestRequestTypeDef,
     _OptionalRegisterIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartProductSubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredStartProductSubscriptionRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
         "Username": str,
     },
@@ -442,20 +494,22 @@
     "_OptionalStartProductSubscriptionRequestRequestTypeDef",
     {
         "Domain": str,
     },
     total=False,
 )
 
+
 class StartProductSubscriptionRequestRequestTypeDef(
     _RequiredStartProductSubscriptionRequestRequestTypeDef,
     _OptionalStartProductSubscriptionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStopProductSubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredStopProductSubscriptionRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
         "Username": str,
     },
@@ -464,20 +518,22 @@
     "_OptionalStopProductSubscriptionRequestRequestTypeDef",
     {
         "Domain": str,
     },
     total=False,
 )
 
+
 class StopProductSubscriptionRequestRequestTypeDef(
     _RequiredStopProductSubscriptionRequestRequestTypeDef,
     _OptionalStopProductSubscriptionRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateIdentityProviderSettingsRequestRequestTypeDef = TypedDict(
     "UpdateIdentityProviderSettingsRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
         "UpdateSettings": UpdateSettingsTypeDef,
     },
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions.egg-info/PKG-INFO` & `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager-user-subscriptions
-Version: 1.28.0
-Summary: Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-license-manager-user-subscriptions"></a>
 
 # mypy-boto3-license-manager-user-subscriptions
 
 [![PyPI - mypy-boto3-license-manager-user-subscriptions](https://img.shields.io/pypi/v/mypy-boto3-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-user-subscriptions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-user-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-license-manager-user-subscriptions?color=blue)](https://pypistats.org/packages/mypy-boto3-license-manager-user-subscriptions)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager-user-subscriptions)](https://pepy.tech/project/mypy-boto3-license-manager-user-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerUserSubscriptions 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
+[boto3.LicenseManagerUserSubscriptions 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
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
 [mypy-boto3-license-manager-user-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -346,37 +346,40 @@
 
 `mypy_boto3_license_manager_user_subscriptions.type_defs` module contains
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_license_manager_user_subscriptions.type_defs import (
+    ActiveDirectoryIdentityProviderOutputTypeDef,
     ActiveDirectoryIdentityProviderTypeDef,
     FilterTypeDef,
-    SettingsTypeDef,
+    SettingsOutputTypeDef,
     InstanceSummaryTypeDef,
     ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    SettingsTypeDef,
     ResponseMetadataTypeDef,
     UpdateSettingsTypeDef,
+    IdentityProviderOutputTypeDef,
     IdentityProviderTypeDef,
     ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
+    IdentityProviderSummaryTypeDef,
+    InstanceUserSummaryTypeDef,
+    ProductUserSummaryTypeDef,
     AssociateUserRequestRequestTypeDef,
     DeregisterIdentityProviderRequestRequestTypeDef,
     DisassociateUserRequestRequestTypeDef,
-    IdentityProviderSummaryTypeDef,
-    InstanceUserSummaryTypeDef,
     ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
     ListProductSubscriptionsRequestRequestTypeDef,
     ListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
     ListUserAssociationsRequestRequestTypeDef,
-    ProductUserSummaryTypeDef,
     RegisterIdentityProviderRequestRequestTypeDef,
     StartProductSubscriptionRequestRequestTypeDef,
     StopProductSubscriptionRequestRequestTypeDef,
     UpdateIdentityProviderSettingsRequestRequestTypeDef,
     DeregisterIdentityProviderResponseTypeDef,
     ListIdentityProvidersResponseTypeDef,
     RegisterIdentityProviderResponseTypeDef,
@@ -386,15 +389,15 @@
     ListUserAssociationsResponseTypeDef,
     ListProductSubscriptionsResponseTypeDef,
     StartProductSubscriptionResponseTypeDef,
     StopProductSubscriptionResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveDirectoryIdentityProviderTypeDef:
+def get_structure() -> ActiveDirectoryIdentityProviderOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.0/mypy_boto3_license_manager_user_subscriptions.egg-info/SOURCES.txt` & `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.0/setup.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-license-manager-user-subscriptions",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_license_manager_user_subscriptions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

