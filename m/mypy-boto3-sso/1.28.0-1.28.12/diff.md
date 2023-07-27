# Comparing `tmp/mypy-boto3-sso-1.28.0.tar.gz` & `tmp/mypy-boto3-sso-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sso-1.28.0.tar", last modified: Thu Jul  6 21:00:43 2023, max compression
+gzip compressed data, was "mypy-boto3-sso-1.28.12.tar", last modified: Thu Jul 27 11:49:44 2023, max compression
```

## Comparing `mypy-boto3-sso-1.28.0.tar` & `mypy-boto3-sso-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:43.734444 mypy-boto3-sso-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:56:41.000000 mypy-boto3-sso-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12936 2023-07-06 21:00:43.734444 mypy-boto3-sso-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-07-06 20:56:41.000000 mypy-boto3-sso-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:43.714444 mypy-boto3-sso-1.28.0/mypy_boto3_sso/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-06 20:56:41.000000 mypy-boto3-sso-1.28.0/mypy_boto3_sso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-06 20:56:41.000000 mypy-boto3-sso-1.28.0/mypy_boto3_sso/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:56:41.000000 mypy-boto3-sso-1.28.0/mypy_boto3_sso/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-07-06 20:56:41.000000 mypy-boto3-sso-1.28.0/mypy_boto3_sso/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-07-06 20:56:41.000000 mypy-boto3-sso-1.28.0/mypy_boto3_sso/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-07-06 20:56:42.000000 mypy-boto3-sso-1.28.0/mypy_boto3_sso/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-07-06 20:56:42.000000 mypy-boto3-sso-1.28.0/mypy_boto3_sso/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-06 20:56:41.000000 mypy-boto3-sso-1.28.0/mypy_boto3_sso/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-06 20:56:41.000000 mypy-boto3-sso-1.28.0/mypy_boto3_sso/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:56:41.000000 mypy-boto3-sso-1.28.0/mypy_boto3_sso/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-07-06 20:56:42.000000 mypy-boto3-sso-1.28.0/mypy_boto3_sso/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-07-06 20:56:42.000000 mypy-boto3-sso-1.28.0/mypy_boto3_sso/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:56:41.000000 mypy-boto3-sso-1.28.0/mypy_boto3_sso/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:43.714444 mypy-boto3-sso-1.28.0/mypy_boto3_sso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12936 2023-07-06 21:00:43.000000 mypy-boto3-sso-1.28.0/mypy_boto3_sso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 21:00:43.000000 mypy-boto3-sso-1.28.0/mypy_boto3_sso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:43.000000 mypy-boto3-sso-1.28.0/mypy_boto3_sso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:43.000000 mypy-boto3-sso-1.28.0/mypy_boto3_sso.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:43.000000 mypy-boto3-sso-1.28.0/mypy_boto3_sso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 21:00:43.000000 mypy-boto3-sso-1.28.0/mypy_boto3_sso.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:43.734444 mypy-boto3-sso-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:56:41.000000 mypy-boto3-sso-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.041343 mypy-boto3-sso-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:35.000000 mypy-boto3-sso-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-07-27 11:49:44.033343 mypy-boto3-sso-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-27 11:47:35.000000 mypy-boto3-sso-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.033343 mypy-boto3-sso-1.28.12/mypy_boto3_sso/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-27 11:47:35.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-27 11:47:35.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 11:47:35.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-07-27 11:47:36.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-07-27 11:47:36.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-07-27 11:47:36.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-27 11:47:36.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-27 11:47:36.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-27 11:47:36.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:35.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-27 11:47:36.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-27 11:47:36.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:35.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.033343 mypy-boto3-sso-1.28.12/mypy_boto3_sso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-07-27 11:49:43.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 11:49:43.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:43.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:43.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:43.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:43.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:44.041343 mypy-boto3-sso-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 11:47:35.000000 mypy-boto3-sso-1.28.12/setup.py
```

### Comparing `mypy-boto3-sso-1.28.0/LICENSE` & `mypy-boto3-sso-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.28.0/PKG-INFO` & `mypy-boto3-sso-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sso
-Version: 1.28.0
-Summary: Type annotations for boto3.SSO 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SSO 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sso"></a>
 
 # mypy-boto3-sso
 
 [![PyPI - mypy-boto3-sso](https://img.shields.io/pypi/v/mypy-boto3-sso.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sso?color=blue)](https://pypistats.org/packages/mypy-boto3-sso)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sso)](https://pepy.tech/project/mypy-boto3-sso)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSO 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
+[boto3.SSO 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
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
 [mypy-boto3-sso docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,27 +320,27 @@
 
 `mypy_boto3_sso.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sso.type_defs import (
     AccountInfoTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetRoleCredentialsRequestRequestTypeDef,
     RoleCredentialsTypeDef,
-    ListAccountRolesRequestListAccountRolesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountRolesRequestRequestTypeDef,
     RoleInfoTypeDef,
-    ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountsRequestRequestTypeDef,
     LogoutRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListAccountsResponseTypeDef,
     GetRoleCredentialsResponseTypeDef,
+    ListAccountRolesRequestListAccountRolesPaginateTypeDef,
+    ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountRolesResponseTypeDef,
 )
 
 
 def get_structure() -> AccountInfoTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-sso-1.28.0/README.md` & `mypy-boto3-sso-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sso"></a>
 
 # mypy-boto3-sso
 
 [![PyPI - mypy-boto3-sso](https://img.shields.io/pypi/v/mypy-boto3-sso.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sso?color=blue)](https://pypistats.org/packages/mypy-boto3-sso)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sso)](https://pepy.tech/project/mypy-boto3-sso)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSO 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
+[boto3.SSO 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
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
 [mypy-boto3-sso docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/).
 
 See how it helps to find and fix potential bugs:
 
@@ -288,27 +288,27 @@
 
 `mypy_boto3_sso.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sso.type_defs import (
     AccountInfoTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetRoleCredentialsRequestRequestTypeDef,
     RoleCredentialsTypeDef,
-    ListAccountRolesRequestListAccountRolesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountRolesRequestRequestTypeDef,
     RoleInfoTypeDef,
-    ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountsRequestRequestTypeDef,
     LogoutRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListAccountsResponseTypeDef,
     GetRoleCredentialsResponseTypeDef,
+    ListAccountRolesRequestListAccountRolesPaginateTypeDef,
+    ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountRolesResponseTypeDef,
 )
 
 
 def get_structure() -> AccountInfoTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-sso-1.28.0/mypy_boto3_sso/__init__.py` & `mypy-boto3-sso-1.28.12/mypy_boto3_sso/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.28.0/mypy_boto3_sso/__init__.pyi` & `mypy-boto3-sso-1.28.12/mypy_boto3_sso/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.28.0/mypy_boto3_sso/__main__.py` & `mypy-boto3-sso-1.28.12/mypy_boto3_sso/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSO 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.SSO 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO\nOther"
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

### Comparing `mypy-boto3-sso-1.28.0/mypy_boto3_sso/client.py` & `mypy-boto3-sso-1.28.12/mypy_boto3_sso/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.28.0/mypy_boto3_sso/client.pyi` & `mypy-boto3-sso-1.28.12/mypy_boto3_sso/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.28.0/mypy_boto3_sso/literals.py` & `mypy-boto3-sso-1.28.12/mypy_boto3_sso/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,15 @@
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
@@ -234,26 +235,28 @@
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

### Comparing `mypy-boto3-sso-1.28.0/mypy_boto3_sso/literals.pyi` & `mypy-boto3-sso-1.28.12/mypy_boto3_sso/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,15 @@
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
@@ -232,26 +233,28 @@
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

### Comparing `mypy-boto3-sso-1.28.0/mypy_boto3_sso/paginator.py` & `mypy-boto3-sso-1.28.12/mypy_boto3_sso/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,28 +47,28 @@
 class ListAccountRolesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccountRoles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/paginators/#listaccountrolespaginator)
     """
 
     def paginate(
-        self, *, accessToken: str, accountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accessToken: str, accountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccountRolesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccountRoles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/paginators/#listaccountrolespaginator)
         """
 
 
 class ListAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/paginators/#listaccountspaginator)
     """
 
     def paginate(
-        self, *, accessToken: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accessToken: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/paginators/#listaccountspaginator)
         """
```

### Comparing `mypy-boto3-sso-1.28.0/mypy_boto3_sso/paginator.pyi` & `mypy-boto3-sso-1.28.12/mypy_boto3_sso/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -44,27 +44,27 @@
 class ListAccountRolesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccountRoles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/paginators/#listaccountrolespaginator)
     """
 
     def paginate(
-        self, *, accessToken: str, accountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accessToken: str, accountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccountRolesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccountRoles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/paginators/#listaccountrolespaginator)
         """
 
 class ListAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/paginators/#listaccountspaginator)
     """
 
     def paginate(
-        self, *, accessToken: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accessToken: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/paginators/#listaccountspaginator)
         """
```

### Comparing `mypy-boto3-sso-1.28.0/mypy_boto3_sso/type_defs.py` & `mypy-boto3-sso-1.28.12/mypy_boto3_sso/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -15,47 +15,50 @@
 from typing import Dict, List
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountInfoTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "GetRoleCredentialsRequestRequestTypeDef",
     "RoleCredentialsTypeDef",
-    "ListAccountRolesRequestListAccountRolesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccountRolesRequestRequestTypeDef",
     "RoleInfoTypeDef",
-    "ListAccountsRequestListAccountsPaginateTypeDef",
     "ListAccountsRequestRequestTypeDef",
     "LogoutRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListAccountsResponseTypeDef",
     "GetRoleCredentialsResponseTypeDef",
+    "ListAccountRolesRequestListAccountRolesPaginateTypeDef",
+    "ListAccountsRequestListAccountsPaginateTypeDef",
     "ListAccountRolesResponseTypeDef",
 )
 
 AccountInfoTypeDef = TypedDict(
     "AccountInfoTypeDef",
     {
         "accountId": str,
         "accountName": str,
         "emailAddress": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetRoleCredentialsRequestRequestTypeDef = TypedDict(
     "GetRoleCredentialsRequestRequestTypeDef",
     {
         "roleName": str,
@@ -71,37 +74,24 @@
         "secretAccessKey": str,
         "sessionToken": str,
         "expiration": int,
     },
     total=False,
 )
 
-_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
-    "_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef",
-    {
-        "accessToken": str,
-        "accountId": str,
-    },
-)
-_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
-    "_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef",
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
-class ListAccountRolesRequestListAccountRolesPaginateTypeDef(
-    _RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef,
-    _OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAccountRolesRequestRequestTypeDef = TypedDict(
     "_RequiredListAccountRolesRequestRequestTypeDef",
     {
         "accessToken": str,
         "accountId": str,
     },
 )
@@ -110,52 +100,28 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListAccountRolesRequestRequestTypeDef(
     _RequiredListAccountRolesRequestRequestTypeDef, _OptionalListAccountRolesRequestRequestTypeDef
 ):
     pass
 
-
 RoleInfoTypeDef = TypedDict(
     "RoleInfoTypeDef",
     {
         "roleName": str,
         "accountId": str,
     },
     total=False,
 )
 
-_RequiredListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
-    "_RequiredListAccountsRequestListAccountsPaginateTypeDef",
-    {
-        "accessToken": str,
-    },
-)
-_OptionalListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
-    "_OptionalListAccountsRequestListAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAccountsRequestListAccountsPaginateTypeDef(
-    _RequiredListAccountsRequestListAccountsPaginateTypeDef,
-    _OptionalListAccountsRequestListAccountsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAccountsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccountsRequestRequestTypeDef",
     {
         "accessToken": str,
     },
 )
 _OptionalListAccountsRequestRequestTypeDef = TypedDict(
@@ -163,67 +129,92 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListAccountsRequestRequestTypeDef(
     _RequiredListAccountsRequestRequestTypeDef, _OptionalListAccountsRequestRequestTypeDef
 ):
     pass
 
-
 LogoutRequestRequestTypeDef = TypedDict(
     "LogoutRequestRequestTypeDef",
     {
         "accessToken": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccountsResponseTypeDef = TypedDict(
     "ListAccountsResponseTypeDef",
     {
         "nextToken": str,
         "accountList": List[AccountInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoleCredentialsResponseTypeDef = TypedDict(
     "GetRoleCredentialsResponseTypeDef",
     {
         "roleCredentials": RoleCredentialsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
+    "_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef",
+    {
+        "accessToken": str,
+        "accountId": str,
     },
 )
+_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
+    "_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAccountRolesRequestListAccountRolesPaginateTypeDef(
+    _RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef,
+    _OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef,
+):
+    pass
+
+_RequiredListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
+    "_RequiredListAccountsRequestListAccountsPaginateTypeDef",
+    {
+        "accessToken": str,
+    },
+)
+_OptionalListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
+    "_OptionalListAccountsRequestListAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAccountsRequestListAccountsPaginateTypeDef(
+    _RequiredListAccountsRequestListAccountsPaginateTypeDef,
+    _OptionalListAccountsRequestListAccountsPaginateTypeDef,
+):
+    pass
 
 ListAccountRolesResponseTypeDef = TypedDict(
     "ListAccountRolesResponseTypeDef",
     {
         "nextToken": str,
         "roleList": List[RoleInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-sso-1.28.0/mypy_boto3_sso/type_defs.pyi` & `mypy-boto3-sso-1.28.12/mypy_boto3_sso/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,46 +15,51 @@
 from typing import Dict, List
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccountInfoTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "GetRoleCredentialsRequestRequestTypeDef",
     "RoleCredentialsTypeDef",
-    "ListAccountRolesRequestListAccountRolesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccountRolesRequestRequestTypeDef",
     "RoleInfoTypeDef",
-    "ListAccountsRequestListAccountsPaginateTypeDef",
     "ListAccountsRequestRequestTypeDef",
     "LogoutRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListAccountsResponseTypeDef",
     "GetRoleCredentialsResponseTypeDef",
+    "ListAccountRolesRequestListAccountRolesPaginateTypeDef",
+    "ListAccountsRequestListAccountsPaginateTypeDef",
     "ListAccountRolesResponseTypeDef",
 )
 
 AccountInfoTypeDef = TypedDict(
     "AccountInfoTypeDef",
     {
         "accountId": str,
         "accountName": str,
         "emailAddress": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetRoleCredentialsRequestRequestTypeDef = TypedDict(
     "GetRoleCredentialsRequestRequestTypeDef",
     {
         "roleName": str,
@@ -70,35 +75,24 @@
         "secretAccessKey": str,
         "sessionToken": str,
         "expiration": int,
     },
     total=False,
 )
 
-_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
-    "_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef",
-    {
-        "accessToken": str,
-        "accountId": str,
-    },
-)
-_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
-    "_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef",
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
 
-class ListAccountRolesRequestListAccountRolesPaginateTypeDef(
-    _RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef,
-    _OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef,
-):
-    pass
-
 _RequiredListAccountRolesRequestRequestTypeDef = TypedDict(
     "_RequiredListAccountRolesRequestRequestTypeDef",
     {
         "accessToken": str,
         "accountId": str,
     },
 )
@@ -107,48 +101,30 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListAccountRolesRequestRequestTypeDef(
     _RequiredListAccountRolesRequestRequestTypeDef, _OptionalListAccountRolesRequestRequestTypeDef
 ):
     pass
 
+
 RoleInfoTypeDef = TypedDict(
     "RoleInfoTypeDef",
     {
         "roleName": str,
         "accountId": str,
     },
     total=False,
 )
 
-_RequiredListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
-    "_RequiredListAccountsRequestListAccountsPaginateTypeDef",
-    {
-        "accessToken": str,
-    },
-)
-_OptionalListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
-    "_OptionalListAccountsRequestListAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAccountsRequestListAccountsPaginateTypeDef(
-    _RequiredListAccountsRequestListAccountsPaginateTypeDef,
-    _OptionalListAccountsRequestListAccountsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAccountsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccountsRequestRequestTypeDef",
     {
         "accessToken": str,
     },
 )
 _OptionalListAccountsRequestRequestTypeDef = TypedDict(
@@ -156,65 +132,98 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListAccountsRequestRequestTypeDef(
     _RequiredListAccountsRequestRequestTypeDef, _OptionalListAccountsRequestRequestTypeDef
 ):
     pass
 
+
 LogoutRequestRequestTypeDef = TypedDict(
     "LogoutRequestRequestTypeDef",
     {
         "accessToken": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccountsResponseTypeDef = TypedDict(
     "ListAccountsResponseTypeDef",
     {
         "nextToken": str,
         "accountList": List[AccountInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoleCredentialsResponseTypeDef = TypedDict(
     "GetRoleCredentialsResponseTypeDef",
     {
         "roleCredentials": RoleCredentialsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
+    "_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef",
+    {
+        "accessToken": str,
+        "accountId": str,
+    },
+)
+_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
+    "_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+
+class ListAccountRolesRequestListAccountRolesPaginateTypeDef(
+    _RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef,
+    _OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
+    "_RequiredListAccountsRequestListAccountsPaginateTypeDef",
+    {
+        "accessToken": str,
+    },
+)
+_OptionalListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
+    "_OptionalListAccountsRequestListAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAccountsRequestListAccountsPaginateTypeDef(
+    _RequiredListAccountsRequestListAccountsPaginateTypeDef,
+    _OptionalListAccountsRequestListAccountsPaginateTypeDef,
+):
+    pass
+
+
 ListAccountRolesResponseTypeDef = TypedDict(
     "ListAccountRolesResponseTypeDef",
     {
         "nextToken": str,
         "roleList": List[RoleInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-sso-1.28.0/mypy_boto3_sso.egg-info/PKG-INFO` & `mypy-boto3-sso-1.28.12/mypy_boto3_sso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sso
-Version: 1.28.0
-Summary: Type annotations for boto3.SSO 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SSO 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sso"></a>
 
 # mypy-boto3-sso
 
 [![PyPI - mypy-boto3-sso](https://img.shields.io/pypi/v/mypy-boto3-sso.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sso?color=blue)](https://pypistats.org/packages/mypy-boto3-sso)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sso)](https://pepy.tech/project/mypy-boto3-sso)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSO 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
+[boto3.SSO 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
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
 [mypy-boto3-sso docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,27 +320,27 @@
 
 `mypy_boto3_sso.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sso.type_defs import (
     AccountInfoTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetRoleCredentialsRequestRequestTypeDef,
     RoleCredentialsTypeDef,
-    ListAccountRolesRequestListAccountRolesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountRolesRequestRequestTypeDef,
     RoleInfoTypeDef,
-    ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountsRequestRequestTypeDef,
     LogoutRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListAccountsResponseTypeDef,
     GetRoleCredentialsResponseTypeDef,
+    ListAccountRolesRequestListAccountRolesPaginateTypeDef,
+    ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountRolesResponseTypeDef,
 )
 
 
 def get_structure() -> AccountInfoTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-sso-1.28.0/mypy_boto3_sso.egg-info/SOURCES.txt` & `mypy-boto3-sso-1.28.12/mypy_boto3_sso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.28.0/setup.py` & `mypy-boto3-sso-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sso",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_sso"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSO 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SSO 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

