# Comparing `tmp/mypy-boto3-sso-oidc-1.28.0.tar.gz` & `tmp/mypy-boto3-sso-oidc-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sso-oidc-1.28.0.tar", last modified: Thu Jul  6 21:00:43 2023, max compression
+gzip compressed data, was "mypy-boto3-sso-oidc-1.28.12.tar", last modified: Thu Jul 27 11:49:43 2023, max compression
```

## Comparing `mypy-boto3-sso-oidc-1.28.0.tar` & `mypy-boto3-sso-oidc-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:43.574443 mypy-boto3-sso-oidc-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:56:45.000000 mypy-boto3-sso-oidc-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-07-06 21:00:43.574443 mypy-boto3-sso-oidc-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-07-06 20:56:45.000000 mypy-boto3-sso-oidc-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:43.570443 mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-06 20:56:45.000000 mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-06 20:56:45.000000 mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-06 20:56:45.000000 mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-06 20:56:45.000000 mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-07-06 20:56:45.000000 mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-07-06 20:56:45.000000 mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-07-06 20:56:45.000000 mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:56:45.000000 mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-06 20:56:46.000000 mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-06 20:56:45.000000 mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:56:45.000000 mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:43.574443 mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-07-06 21:00:43.000000 mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-06 21:00:43.000000 mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:43.000000 mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:43.000000 mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:43.000000 mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:00:43.000000 mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:43.574443 mypy-boto3-sso-oidc-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-06 20:56:45.000000 mypy-boto3-sso-oidc-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:43.773341 mypy-boto3-sso-oidc-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:38.000000 mypy-boto3-sso-oidc-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-07-27 11:49:43.773341 mypy-boto3-sso-oidc-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-07-27 11:47:38.000000 mypy-boto3-sso-oidc-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:43.761340 mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-27 11:47:38.000000 mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-27 11:47:38.000000 mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-27 11:47:38.000000 mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-27 11:47:38.000000 mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-07-27 11:47:38.000000 mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-07-27 11:47:38.000000 mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-07-27 11:47:38.000000 mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:38.000000 mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-07-27 11:47:38.000000 mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-27 11:47:38.000000 mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:38.000000 mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:43.773341 mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-07-27 11:49:43.000000 mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-27 11:49:43.000000 mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:43.000000 mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:43.000000 mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:43.000000 mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:43.000000 mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:43.773341 mypy-boto3-sso-oidc-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-27 11:47:38.000000 mypy-boto3-sso-oidc-1.28.12/setup.py
```

### Comparing `mypy-boto3-sso-oidc-1.28.0/LICENSE` & `mypy-boto3-sso-oidc-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-oidc-1.28.0/PKG-INFO` & `mypy-boto3-sso-oidc-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sso-oidc
-Version: 1.28.0
-Summary: Type annotations for boto3.SSOOIDC 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SSOOIDC 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sso-oidc"></a>
 
 # mypy-boto3-sso-oidc
 
 [![PyPI - mypy-boto3-sso-oidc](https://img.shields.io/pypi/v/mypy-boto3-sso-oidc.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-oidc)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso-oidc.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-oidc)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sso-oidc?color=blue)](https://pypistats.org/packages/mypy-boto3-sso-oidc)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sso-oidc)](https://pepy.tech/project/mypy-boto3-sso-oidc)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSOOIDC 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
+[boto3.SSOOIDC 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
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
 [mypy-boto3-sso-oidc docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/).
 
 See how it helps to find and fix potential bugs:
 
@@ -296,19 +296,19 @@
 
 `mypy_boto3_sso_oidc.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sso_oidc.type_defs import (
     CreateTokenRequestRequestTypeDef,
-    CreateTokenResponseTypeDef,
-    RegisterClientRequestRequestTypeDef,
-    RegisterClientResponseTypeDef,
     ResponseMetadataTypeDef,
+    RegisterClientRequestRequestTypeDef,
     StartDeviceAuthorizationRequestRequestTypeDef,
+    CreateTokenResponseTypeDef,
+    RegisterClientResponseTypeDef,
     StartDeviceAuthorizationResponseTypeDef,
 )
 
 
 def get_structure() -> CreateTokenRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-sso-oidc-1.28.0/README.md` & `mypy-boto3-sso-oidc-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sso-oidc"></a>
 
 # mypy-boto3-sso-oidc
 
 [![PyPI - mypy-boto3-sso-oidc](https://img.shields.io/pypi/v/mypy-boto3-sso-oidc.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-oidc)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso-oidc.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-oidc)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sso-oidc?color=blue)](https://pypistats.org/packages/mypy-boto3-sso-oidc)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sso-oidc)](https://pepy.tech/project/mypy-boto3-sso-oidc)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSOOIDC 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
+[boto3.SSOOIDC 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
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
 [mypy-boto3-sso-oidc docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/).
 
 See how it helps to find and fix potential bugs:
 
@@ -264,19 +264,19 @@
 
 `mypy_boto3_sso_oidc.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sso_oidc.type_defs import (
     CreateTokenRequestRequestTypeDef,
-    CreateTokenResponseTypeDef,
-    RegisterClientRequestRequestTypeDef,
-    RegisterClientResponseTypeDef,
     ResponseMetadataTypeDef,
+    RegisterClientRequestRequestTypeDef,
     StartDeviceAuthorizationRequestRequestTypeDef,
+    CreateTokenResponseTypeDef,
+    RegisterClientResponseTypeDef,
     StartDeviceAuthorizationResponseTypeDef,
 )
 
 
 def get_structure() -> CreateTokenRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc/__main__.py` & `mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSOOIDC 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.SSOOIDC 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC\nOther"
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

### Comparing `mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc/client.py` & `mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc/client.pyi` & `mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc/literals.py` & `mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,15 @@
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
@@ -224,26 +225,28 @@
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

### Comparing `mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc/literals.pyi` & `mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -136,14 +136,15 @@
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
@@ -222,26 +223,28 @@
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

### Comparing `mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc/type_defs.py` & `mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -15,22 +15,21 @@
 from typing import Dict, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CreateTokenRequestRequestTypeDef",
-    "CreateTokenResponseTypeDef",
-    "RegisterClientRequestRequestTypeDef",
-    "RegisterClientResponseTypeDef",
     "ResponseMetadataTypeDef",
+    "RegisterClientRequestRequestTypeDef",
     "StartDeviceAuthorizationRequestRequestTypeDef",
+    "CreateTokenResponseTypeDef",
+    "RegisterClientResponseTypeDef",
     "StartDeviceAuthorizationResponseTypeDef",
 )
 
 _RequiredCreateTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTokenRequestRequestTypeDef",
     {
         "clientId": str,
@@ -46,30 +45,27 @@
         "refreshToken": str,
         "scope": Sequence[str],
         "redirectUri": str,
     },
     total=False,
 )
 
-
 class CreateTokenRequestRequestTypeDef(
     _RequiredCreateTokenRequestRequestTypeDef, _OptionalCreateTokenRequestRequestTypeDef
 ):
     pass
 
-
-CreateTokenResponseTypeDef = TypedDict(
-    "CreateTokenResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "accessToken": str,
-        "tokenType": str,
-        "expiresIn": int,
-        "refreshToken": str,
-        "idToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredRegisterClientRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterClientRequestRequestTypeDef",
     {
         "clientName": str,
@@ -80,59 +76,58 @@
     "_OptionalRegisterClientRequestRequestTypeDef",
     {
         "scopes": Sequence[str],
     },
     total=False,
 )
 
-
 class RegisterClientRequestRequestTypeDef(
     _RequiredRegisterClientRequestRequestTypeDef, _OptionalRegisterClientRequestRequestTypeDef
 ):
     pass
 
-
-RegisterClientResponseTypeDef = TypedDict(
-    "RegisterClientResponseTypeDef",
+StartDeviceAuthorizationRequestRequestTypeDef = TypedDict(
+    "StartDeviceAuthorizationRequestRequestTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
-        "clientIdIssuedAt": int,
-        "clientSecretExpiresAt": int,
-        "authorizationEndpoint": str,
-        "tokenEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "startUrl": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateTokenResponseTypeDef = TypedDict(
+    "CreateTokenResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "accessToken": str,
+        "tokenType": str,
+        "expiresIn": int,
+        "refreshToken": str,
+        "idToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartDeviceAuthorizationRequestRequestTypeDef = TypedDict(
-    "StartDeviceAuthorizationRequestRequestTypeDef",
+RegisterClientResponseTypeDef = TypedDict(
+    "RegisterClientResponseTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
-        "startUrl": str,
+        "clientIdIssuedAt": int,
+        "clientSecretExpiresAt": int,
+        "authorizationEndpoint": str,
+        "tokenEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartDeviceAuthorizationResponseTypeDef = TypedDict(
     "StartDeviceAuthorizationResponseTypeDef",
     {
         "deviceCode": str,
         "userCode": str,
         "verificationUri": str,
         "verificationUriComplete": str,
         "expiresIn": int,
         "interval": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc/type_defs.pyi` & `mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,21 +15,22 @@
 from typing import Dict, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CreateTokenRequestRequestTypeDef",
-    "CreateTokenResponseTypeDef",
-    "RegisterClientRequestRequestTypeDef",
-    "RegisterClientResponseTypeDef",
     "ResponseMetadataTypeDef",
+    "RegisterClientRequestRequestTypeDef",
     "StartDeviceAuthorizationRequestRequestTypeDef",
+    "CreateTokenResponseTypeDef",
+    "RegisterClientResponseTypeDef",
     "StartDeviceAuthorizationResponseTypeDef",
 )
 
 _RequiredCreateTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTokenRequestRequestTypeDef",
     {
         "clientId": str,
@@ -45,28 +46,29 @@
         "refreshToken": str,
         "scope": Sequence[str],
         "redirectUri": str,
     },
     total=False,
 )
 
+
 class CreateTokenRequestRequestTypeDef(
     _RequiredCreateTokenRequestRequestTypeDef, _OptionalCreateTokenRequestRequestTypeDef
 ):
     pass
 
-CreateTokenResponseTypeDef = TypedDict(
-    "CreateTokenResponseTypeDef",
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "accessToken": str,
-        "tokenType": str,
-        "expiresIn": int,
-        "refreshToken": str,
-        "idToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredRegisterClientRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterClientRequestRequestTypeDef",
     {
         "clientName": str,
@@ -77,57 +79,60 @@
     "_OptionalRegisterClientRequestRequestTypeDef",
     {
         "scopes": Sequence[str],
     },
     total=False,
 )
 
+
 class RegisterClientRequestRequestTypeDef(
     _RequiredRegisterClientRequestRequestTypeDef, _OptionalRegisterClientRequestRequestTypeDef
 ):
     pass
 
-RegisterClientResponseTypeDef = TypedDict(
-    "RegisterClientResponseTypeDef",
+
+StartDeviceAuthorizationRequestRequestTypeDef = TypedDict(
+    "StartDeviceAuthorizationRequestRequestTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
-        "clientIdIssuedAt": int,
-        "clientSecretExpiresAt": int,
-        "authorizationEndpoint": str,
-        "tokenEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "startUrl": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateTokenResponseTypeDef = TypedDict(
+    "CreateTokenResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "accessToken": str,
+        "tokenType": str,
+        "expiresIn": int,
+        "refreshToken": str,
+        "idToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartDeviceAuthorizationRequestRequestTypeDef = TypedDict(
-    "StartDeviceAuthorizationRequestRequestTypeDef",
+RegisterClientResponseTypeDef = TypedDict(
+    "RegisterClientResponseTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
-        "startUrl": str,
+        "clientIdIssuedAt": int,
+        "clientSecretExpiresAt": int,
+        "authorizationEndpoint": str,
+        "tokenEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartDeviceAuthorizationResponseTypeDef = TypedDict(
     "StartDeviceAuthorizationResponseTypeDef",
     {
         "deviceCode": str,
         "userCode": str,
         "verificationUri": str,
         "verificationUriComplete": str,
         "expiresIn": int,
         "interval": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc.egg-info/PKG-INFO` & `mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sso-oidc
-Version: 1.28.0
-Summary: Type annotations for boto3.SSOOIDC 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SSOOIDC 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sso-oidc"></a>
 
 # mypy-boto3-sso-oidc
 
 [![PyPI - mypy-boto3-sso-oidc](https://img.shields.io/pypi/v/mypy-boto3-sso-oidc.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-oidc)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso-oidc.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-oidc)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sso-oidc?color=blue)](https://pypistats.org/packages/mypy-boto3-sso-oidc)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sso-oidc)](https://pepy.tech/project/mypy-boto3-sso-oidc)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSOOIDC 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
+[boto3.SSOOIDC 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
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
 [mypy-boto3-sso-oidc docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_oidc/).
 
 See how it helps to find and fix potential bugs:
 
@@ -296,19 +296,19 @@
 
 `mypy_boto3_sso_oidc.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sso_oidc.type_defs import (
     CreateTokenRequestRequestTypeDef,
-    CreateTokenResponseTypeDef,
-    RegisterClientRequestRequestTypeDef,
-    RegisterClientResponseTypeDef,
     ResponseMetadataTypeDef,
+    RegisterClientRequestRequestTypeDef,
     StartDeviceAuthorizationRequestRequestTypeDef,
+    CreateTokenResponseTypeDef,
+    RegisterClientResponseTypeDef,
     StartDeviceAuthorizationResponseTypeDef,
 )
 
 
 def get_structure() -> CreateTokenRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-sso-oidc-1.28.0/mypy_boto3_sso_oidc.egg-info/SOURCES.txt` & `mypy-boto3-sso-oidc-1.28.12/mypy_boto3_sso_oidc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-oidc-1.28.0/setup.py` & `mypy-boto3-sso-oidc-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sso-oidc",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_sso_oidc"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSOOIDC 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SSOOIDC 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

