# Comparing `tmp/mypy-boto3-license-manager-linux-subscriptions-1.28.0.tar.gz` & `tmp/mypy-boto3-license-manager-linux-subscriptions-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-license-manager-linux-subscriptions-1.28.0.tar", last modified: Thu Jul  6 20:59:58 2023, max compression
+gzip compressed data, was "mypy-boto3-license-manager-linux-subscriptions-1.28.12.tar", last modified: Thu Jul 27 05:34:56 2023, max compression
```

## Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.0.tar` & `mypy-boto3-license-manager-linux-subscriptions-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:58.878352 mypy-boto3-license-manager-linux-subscriptions-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:45:46.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-07-06 20:59:58.874353 mypy-boto3-license-manager-linux-subscriptions-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13519 2023-07-06 20:45:46.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:58.862352 mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-06 20:45:46.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-06 20:45:46.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-06 20:45:46.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-06 20:45:46.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-07-06 20:45:46.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-07-06 20:45:46.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-07-06 20:45:46.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-06 20:45:46.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-06 20:45:46.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:45:46.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-06 20:45:46.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-06 20:45:46.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:45:46.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:58.874353 mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-07-06 20:59:58.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-06 20:59:58.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:58.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:58.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:58.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-06 20:59:58.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:58.878352 mypy-boto3-license-manager-linux-subscriptions-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-06 20:45:46.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:56.096459 mypy-boto3-license-manager-linux-subscriptions-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-07-27 05:34:56.096459 mypy-boto3-license-manager-linux-subscriptions-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13558 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:56.088459 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9072 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:56.096459 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-07-27 05:34:55.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-27 05:34:55.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:55.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 05:34:55.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:56.096459 mypy-boto3-license-manager-linux-subscriptions-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/setup.py
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.0/LICENSE` & `mypy-boto3-license-manager-linux-subscriptions-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.0/PKG-INFO` & `mypy-boto3-license-manager-linux-subscriptions-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager-linux-subscriptions
-Version: 1.28.0
-Summary: Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-license-manager-linux-subscriptions"></a>
 
 # mypy-boto3-license-manager-linux-subscriptions
 
 [![PyPI - mypy-boto3-license-manager-linux-subscriptions](https://img.shields.io/pypi/v/mypy-boto3-license-manager-linux-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-linux-subscriptions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-linux-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-linux-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-license-manager-linux-subscriptions?color=blue)](https://pypistats.org/packages/mypy-boto3-license-manager-linux-subscriptions)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager-linux-subscriptions)](https://pepy.tech/project/mypy-boto3-license-manager-linux-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerLinuxSubscriptions 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
+[boto3.LicenseManagerLinuxSubscriptions 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
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
 [mypy-boto3-license-manager-linux-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -344,27 +344,28 @@
 `mypy_boto3_license_manager_linux_subscriptions.type_defs` module contains
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_license_manager_linux_subscriptions.type_defs import (
     FilterTypeDef,
-    LinuxSubscriptionsDiscoverySettingsTypeDef,
+    LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
     InstanceTypeDef,
+    LinuxSubscriptionsDiscoverySettingsTypeDef,
     SubscriptionTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef,
     ListLinuxSubscriptionInstancesRequestRequestTypeDef,
     ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef,
     ListLinuxSubscriptionsRequestRequestTypeDef,
     GetServiceSettingsResponseTypeDef,
-    UpdateServiceSettingsRequestRequestTypeDef,
     UpdateServiceSettingsResponseTypeDef,
     ListLinuxSubscriptionInstancesResponseTypeDef,
+    UpdateServiceSettingsRequestRequestTypeDef,
     ListLinuxSubscriptionsResponseTypeDef,
 )
 
 
 def get_structure() -> FilterTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.0/README.md` & `mypy-boto3-license-manager-linux-subscriptions-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-license-manager-linux-subscriptions"></a>
 
 # mypy-boto3-license-manager-linux-subscriptions
 
 [![PyPI - mypy-boto3-license-manager-linux-subscriptions](https://img.shields.io/pypi/v/mypy-boto3-license-manager-linux-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-linux-subscriptions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-linux-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-linux-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-license-manager-linux-subscriptions?color=blue)](https://pypistats.org/packages/mypy-boto3-license-manager-linux-subscriptions)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager-linux-subscriptions)](https://pepy.tech/project/mypy-boto3-license-manager-linux-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerLinuxSubscriptions 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
+[boto3.LicenseManagerLinuxSubscriptions 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
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
 [mypy-boto3-license-manager-linux-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,27 +312,28 @@
 `mypy_boto3_license_manager_linux_subscriptions.type_defs` module contains
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_license_manager_linux_subscriptions.type_defs import (
     FilterTypeDef,
-    LinuxSubscriptionsDiscoverySettingsTypeDef,
+    LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
     InstanceTypeDef,
+    LinuxSubscriptionsDiscoverySettingsTypeDef,
     SubscriptionTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef,
     ListLinuxSubscriptionInstancesRequestRequestTypeDef,
     ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef,
     ListLinuxSubscriptionsRequestRequestTypeDef,
     GetServiceSettingsResponseTypeDef,
-    UpdateServiceSettingsRequestRequestTypeDef,
     UpdateServiceSettingsResponseTypeDef,
     ListLinuxSubscriptionInstancesResponseTypeDef,
+    UpdateServiceSettingsRequestRequestTypeDef,
     ListLinuxSubscriptionsResponseTypeDef,
 )
 
 
 def get_structure() -> FilterTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/__init__.py` & `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/__init__.pyi` & `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/__main__.py` & `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.0\nVersion:        "
-        " 1.28.0\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.12\nVersion:        "
+        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions\nOther"
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

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/client.py` & `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/client.pyi` & `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/literals.py` & `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,15 @@
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
@@ -242,26 +243,28 @@
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

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/literals.pyi` & `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,15 @@
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
@@ -240,26 +241,28 @@
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

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/paginator.py` & `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/paginator.pyi` & `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/type_defs.py` & `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -22,45 +22,45 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "FilterTypeDef",
-    "LinuxSubscriptionsDiscoverySettingsTypeDef",
+    "LinuxSubscriptionsDiscoverySettingsOutputTypeDef",
     "InstanceTypeDef",
+    "LinuxSubscriptionsDiscoverySettingsTypeDef",
     "SubscriptionTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
     "ListLinuxSubscriptionInstancesRequestRequestTypeDef",
     "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
     "ListLinuxSubscriptionsRequestRequestTypeDef",
     "GetServiceSettingsResponseTypeDef",
-    "UpdateServiceSettingsRequestRequestTypeDef",
     "UpdateServiceSettingsResponseTypeDef",
     "ListLinuxSubscriptionInstancesResponseTypeDef",
+    "UpdateServiceSettingsRequestRequestTypeDef",
     "ListLinuxSubscriptionsResponseTypeDef",
 )
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
         "Operator": OperatorType,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-LinuxSubscriptionsDiscoverySettingsTypeDef = TypedDict(
-    "LinuxSubscriptionsDiscoverySettingsTypeDef",
+LinuxSubscriptionsDiscoverySettingsOutputTypeDef = TypedDict(
+    "LinuxSubscriptionsDiscoverySettingsOutputTypeDef",
     {
         "OrganizationIntegration": OrganizationIntegrationType,
         "SourceRegions": List[str],
     },
 )
 
 InstanceTypeDef = TypedDict(
@@ -76,14 +76,22 @@
         "Status": str,
         "SubscriptionName": str,
         "UsageOperation": str,
     },
     total=False,
 )
 
+LinuxSubscriptionsDiscoverySettingsTypeDef = TypedDict(
+    "LinuxSubscriptionsDiscoverySettingsTypeDef",
+    {
+        "OrganizationIntegration": OrganizationIntegrationType,
+        "SourceRegions": Sequence[str],
+    },
+)
+
 SubscriptionTypeDef = TypedDict(
     "SubscriptionTypeDef",
     {
         "InstanceCount": int,
         "Name": str,
         "Type": str,
     },
@@ -150,21 +158,42 @@
 )
 
 GetServiceSettingsResponseTypeDef = TypedDict(
     "GetServiceSettingsResponseTypeDef",
     {
         "HomeRegions": List[str],
         "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
-        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
+        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
         "Status": StatusType,
         "StatusMessage": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+UpdateServiceSettingsResponseTypeDef = TypedDict(
+    "UpdateServiceSettingsResponseTypeDef",
+    {
+        "HomeRegions": List[str],
+        "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
+        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
+        "Status": StatusType,
+        "StatusMessage": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListLinuxSubscriptionInstancesResponseTypeDef = TypedDict(
+    "ListLinuxSubscriptionInstancesResponseTypeDef",
+    {
+        "Instances": List[InstanceTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateServiceSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceSettingsRequestRequestTypeDef",
     {
         "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
         "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
     },
 )
@@ -172,43 +201,20 @@
     "_OptionalUpdateServiceSettingsRequestRequestTypeDef",
     {
         "AllowUpdate": bool,
     },
     total=False,
 )
 
-
 class UpdateServiceSettingsRequestRequestTypeDef(
     _RequiredUpdateServiceSettingsRequestRequestTypeDef,
     _OptionalUpdateServiceSettingsRequestRequestTypeDef,
 ):
     pass
 
-
-UpdateServiceSettingsResponseTypeDef = TypedDict(
-    "UpdateServiceSettingsResponseTypeDef",
-    {
-        "HomeRegions": List[str],
-        "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
-        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
-        "Status": StatusType,
-        "StatusMessage": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListLinuxSubscriptionInstancesResponseTypeDef = TypedDict(
-    "ListLinuxSubscriptionInstancesResponseTypeDef",
-    {
-        "Instances": List[InstanceTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListLinuxSubscriptionsResponseTypeDef = TypedDict(
     "ListLinuxSubscriptionsResponseTypeDef",
     {
         "NextToken": str,
         "Subscriptions": List[SubscriptionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions/type_defs.pyi` & `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,44 +22,46 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "FilterTypeDef",
-    "LinuxSubscriptionsDiscoverySettingsTypeDef",
+    "LinuxSubscriptionsDiscoverySettingsOutputTypeDef",
     "InstanceTypeDef",
+    "LinuxSubscriptionsDiscoverySettingsTypeDef",
     "SubscriptionTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
     "ListLinuxSubscriptionInstancesRequestRequestTypeDef",
     "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
     "ListLinuxSubscriptionsRequestRequestTypeDef",
     "GetServiceSettingsResponseTypeDef",
-    "UpdateServiceSettingsRequestRequestTypeDef",
     "UpdateServiceSettingsResponseTypeDef",
     "ListLinuxSubscriptionInstancesResponseTypeDef",
+    "UpdateServiceSettingsRequestRequestTypeDef",
     "ListLinuxSubscriptionsResponseTypeDef",
 )
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
         "Operator": OperatorType,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-LinuxSubscriptionsDiscoverySettingsTypeDef = TypedDict(
-    "LinuxSubscriptionsDiscoverySettingsTypeDef",
+LinuxSubscriptionsDiscoverySettingsOutputTypeDef = TypedDict(
+    "LinuxSubscriptionsDiscoverySettingsOutputTypeDef",
     {
         "OrganizationIntegration": OrganizationIntegrationType,
         "SourceRegions": List[str],
     },
 )
 
 InstanceTypeDef = TypedDict(
@@ -75,14 +77,22 @@
         "Status": str,
         "SubscriptionName": str,
         "UsageOperation": str,
     },
     total=False,
 )
 
+LinuxSubscriptionsDiscoverySettingsTypeDef = TypedDict(
+    "LinuxSubscriptionsDiscoverySettingsTypeDef",
+    {
+        "OrganizationIntegration": OrganizationIntegrationType,
+        "SourceRegions": Sequence[str],
+    },
+)
+
 SubscriptionTypeDef = TypedDict(
     "SubscriptionTypeDef",
     {
         "InstanceCount": int,
         "Name": str,
         "Type": str,
     },
@@ -149,21 +159,42 @@
 )
 
 GetServiceSettingsResponseTypeDef = TypedDict(
     "GetServiceSettingsResponseTypeDef",
     {
         "HomeRegions": List[str],
         "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
-        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
+        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
+        "Status": StatusType,
+        "StatusMessage": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateServiceSettingsResponseTypeDef = TypedDict(
+    "UpdateServiceSettingsResponseTypeDef",
+    {
+        "HomeRegions": List[str],
+        "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
+        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
         "Status": StatusType,
         "StatusMessage": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListLinuxSubscriptionInstancesResponseTypeDef = TypedDict(
+    "ListLinuxSubscriptionInstancesResponseTypeDef",
+    {
+        "Instances": List[InstanceTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateServiceSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceSettingsRequestRequestTypeDef",
     {
         "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
         "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
     },
 )
@@ -171,40 +202,21 @@
     "_OptionalUpdateServiceSettingsRequestRequestTypeDef",
     {
         "AllowUpdate": bool,
     },
     total=False,
 )
 
+
 class UpdateServiceSettingsRequestRequestTypeDef(
     _RequiredUpdateServiceSettingsRequestRequestTypeDef,
     _OptionalUpdateServiceSettingsRequestRequestTypeDef,
 ):
     pass
 
-UpdateServiceSettingsResponseTypeDef = TypedDict(
-    "UpdateServiceSettingsResponseTypeDef",
-    {
-        "HomeRegions": List[str],
-        "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
-        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
-        "Status": StatusType,
-        "StatusMessage": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListLinuxSubscriptionInstancesResponseTypeDef = TypedDict(
-    "ListLinuxSubscriptionInstancesResponseTypeDef",
-    {
-        "Instances": List[InstanceTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ListLinuxSubscriptionsResponseTypeDef = TypedDict(
     "ListLinuxSubscriptionsResponseTypeDef",
     {
         "NextToken": str,
         "Subscriptions": List[SubscriptionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions.egg-info/PKG-INFO` & `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager-linux-subscriptions
-Version: 1.28.0
-Summary: Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-license-manager-linux-subscriptions"></a>
 
 # mypy-boto3-license-manager-linux-subscriptions
 
 [![PyPI - mypy-boto3-license-manager-linux-subscriptions](https://img.shields.io/pypi/v/mypy-boto3-license-manager-linux-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-linux-subscriptions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-linux-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-linux-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-license-manager-linux-subscriptions?color=blue)](https://pypistats.org/packages/mypy-boto3-license-manager-linux-subscriptions)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager-linux-subscriptions)](https://pepy.tech/project/mypy-boto3-license-manager-linux-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerLinuxSubscriptions 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
+[boto3.LicenseManagerLinuxSubscriptions 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
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
 [mypy-boto3-license-manager-linux-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -344,27 +344,28 @@
 `mypy_boto3_license_manager_linux_subscriptions.type_defs` module contains
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_license_manager_linux_subscriptions.type_defs import (
     FilterTypeDef,
-    LinuxSubscriptionsDiscoverySettingsTypeDef,
+    LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
     InstanceTypeDef,
+    LinuxSubscriptionsDiscoverySettingsTypeDef,
     SubscriptionTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef,
     ListLinuxSubscriptionInstancesRequestRequestTypeDef,
     ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef,
     ListLinuxSubscriptionsRequestRequestTypeDef,
     GetServiceSettingsResponseTypeDef,
-    UpdateServiceSettingsRequestRequestTypeDef,
     UpdateServiceSettingsResponseTypeDef,
     ListLinuxSubscriptionInstancesResponseTypeDef,
+    UpdateServiceSettingsRequestRequestTypeDef,
     ListLinuxSubscriptionsResponseTypeDef,
 )
 
 
 def get_structure() -> FilterTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.0/mypy_boto3_license_manager_linux_subscriptions.egg-info/SOURCES.txt` & `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.0/setup.py` & `mypy-boto3-license-manager-linux-subscriptions-1.28.12/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-license-manager-linux-subscriptions",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_license_manager_linux_subscriptions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

