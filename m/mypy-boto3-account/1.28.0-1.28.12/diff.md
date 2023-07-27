# Comparing `tmp/mypy-boto3-account-1.28.0.tar.gz` & `tmp/mypy-boto3-account-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-account-1.28.0.tar", last modified: Thu Jul  6 20:58:51 2023, max compression
+gzip compressed data, was "mypy-boto3-account-1.28.12.tar", last modified: Thu Jul 27 05:34:13 2023, max compression
```

## Comparing `mypy-boto3-account-1.28.0.tar` & `mypy-boto3-account-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:51.698206 mypy-boto3-account-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:32:29.000000 mypy-boto3-account-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13262 2023-07-06 20:58:51.694206 mypy-boto3-account-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-07-06 20:32:29.000000 mypy-boto3-account-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:51.694206 mypy-boto3-account-1.28.0/mypy_boto3_account/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-06 20:32:29.000000 mypy-boto3-account-1.28.0/mypy_boto3_account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-06 20:32:29.000000 mypy-boto3-account-1.28.0/mypy_boto3_account/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 20:32:29.000000 mypy-boto3-account-1.28.0/mypy_boto3_account/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-07-06 20:32:29.000000 mypy-boto3-account-1.28.0/mypy_boto3_account/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-07-06 20:32:29.000000 mypy-boto3-account-1.28.0/mypy_boto3_account/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-07-06 20:32:29.000000 mypy-boto3-account-1.28.0/mypy_boto3_account/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-06 20:32:29.000000 mypy-boto3-account-1.28.0/mypy_boto3_account/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-06 20:32:29.000000 mypy-boto3-account-1.28.0/mypy_boto3_account/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-06 20:32:29.000000 mypy-boto3-account-1.28.0/mypy_boto3_account/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:32:29.000000 mypy-boto3-account-1.28.0/mypy_boto3_account/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-06 20:32:29.000000 mypy-boto3-account-1.28.0/mypy_boto3_account/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-07-06 20:32:29.000000 mypy-boto3-account-1.28.0/mypy_boto3_account/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:32:29.000000 mypy-boto3-account-1.28.0/mypy_boto3_account/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:51.694206 mypy-boto3-account-1.28.0/mypy_boto3_account.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13262 2023-07-06 20:58:51.000000 mypy-boto3-account-1.28.0/mypy_boto3_account.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-06 20:58:51.000000 mypy-boto3-account-1.28.0/mypy_boto3_account.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:51.000000 mypy-boto3-account-1.28.0/mypy_boto3_account.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:51.000000 mypy-boto3-account-1.28.0/mypy_boto3_account.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:58:51.000000 mypy-boto3-account-1.28.0/mypy_boto3_account.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 20:58:51.000000 mypy-boto3-account-1.28.0/mypy_boto3_account.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:58:51.698206 mypy-boto3-account-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-06 20:32:29.000000 mypy-boto3-account-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.840594 mypy-boto3-account-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-07-27 05:34:13.840594 mypy-boto3-account-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.820594 mypy-boto3-account-1.28.12/mypy_boto3_account/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.820594 mypy-boto3-account-1.28.12/mypy_boto3_account.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-07-27 05:34:13.000000 mypy-boto3-account-1.28.12/mypy_boto3_account.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-27 05:34:13.000000 mypy-boto3-account-1.28.12/mypy_boto3_account.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-account-1.28.12/mypy_boto3_account.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-account-1.28.12/mypy_boto3_account.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:13.000000 mypy-boto3-account-1.28.12/mypy_boto3_account.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:34:13.000000 mypy-boto3-account-1.28.12/mypy_boto3_account.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:13.840594 mypy-boto3-account-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/setup.py
```

### Comparing `mypy-boto3-account-1.28.0/LICENSE` & `mypy-boto3-account-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.28.0/PKG-INFO` & `mypy-boto3-account-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-account
-Version: 1.28.0
-Summary: Type annotations for boto3.Account 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Account 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-account"></a>
 
 # mypy-boto3-account
 
 [![PyPI - mypy-boto3-account](https://img.shields.io/pypi/v/mypy-boto3-account.svg?color=blue)](https://pypi.org/project/mypy-boto3-account)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-account.svg?color=blue)](https://pypi.org/project/mypy-boto3-account)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-account?color=blue)](https://pypistats.org/packages/mypy-boto3-account)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-account)](https://pepy.tech/project/mypy-boto3-account)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Account 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
+[boto3.Account 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
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
 [mypy-boto3-account docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,14 +320,15 @@
 
 `mypy_boto3_account.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_account.type_defs import (
     AlternateContactTypeDef,
+    ContactInformationOutputTypeDef,
     ContactInformationTypeDef,
     DeleteAlternateContactRequestRequestTypeDef,
     DisableRegionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     EnableRegionRequestRequestTypeDef,
     GetAlternateContactRequestRequestTypeDef,
     GetContactInformationRequestRequestTypeDef,
```

### Comparing `mypy-boto3-account-1.28.0/README.md` & `mypy-boto3-account-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-account"></a>
 
 # mypy-boto3-account
 
 [![PyPI - mypy-boto3-account](https://img.shields.io/pypi/v/mypy-boto3-account.svg?color=blue)](https://pypi.org/project/mypy-boto3-account)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-account.svg?color=blue)](https://pypi.org/project/mypy-boto3-account)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-account?color=blue)](https://pypistats.org/packages/mypy-boto3-account)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-account)](https://pepy.tech/project/mypy-boto3-account)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Account 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
+[boto3.Account 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
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
 [mypy-boto3-account docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/).
 
 See how it helps to find and fix potential bugs:
 
@@ -288,14 +288,15 @@
 
 `mypy_boto3_account.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_account.type_defs import (
     AlternateContactTypeDef,
+    ContactInformationOutputTypeDef,
     ContactInformationTypeDef,
     DeleteAlternateContactRequestRequestTypeDef,
     DisableRegionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     EnableRegionRequestRequestTypeDef,
     GetAlternateContactRequestRequestTypeDef,
     GetContactInformationRequestRequestTypeDef,
```

### Comparing `mypy-boto3-account-1.28.0/mypy_boto3_account/__init__.py` & `mypy-boto3-account-1.28.12/mypy_boto3_account/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.28.0/mypy_boto3_account/__init__.pyi` & `mypy-boto3-account-1.28.12/mypy_boto3_account/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.28.0/mypy_boto3_account/__main__.py` & `mypy-boto3-account-1.28.12/mypy_boto3_account/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Account 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Account 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account\nOther"
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

### Comparing `mypy-boto3-account-1.28.0/mypy_boto3_account/client.py` & `mypy-boto3-account-1.28.12/mypy_boto3_account/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.28.0/mypy_boto3_account/client.pyi` & `mypy-boto3-account-1.28.12/mypy_boto3_account/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.28.0/mypy_boto3_account/literals.py` & `mypy-boto3-account-1.28.12/mypy_boto3_account/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,15 @@
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
@@ -235,26 +236,28 @@
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

### Comparing `mypy-boto3-account-1.28.0/mypy_boto3_account/literals.pyi` & `mypy-boto3-account-1.28.12/mypy_boto3_account/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,15 @@
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
@@ -233,26 +234,28 @@
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

### Comparing `mypy-boto3-account-1.28.0/mypy_boto3_account/paginator.py` & `mypy-boto3-account-1.28.12/mypy_boto3_account/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.28.0/mypy_boto3_account/paginator.pyi` & `mypy-boto3-account-1.28.12/mypy_boto3_account/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.28.0/mypy_boto3_account/type_defs.py` & `mypy-boto3-account-1.28.12/mypy_boto3_account/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AlternateContactTypeDef",
+    "ContactInformationOutputTypeDef",
     "ContactInformationTypeDef",
     "DeleteAlternateContactRequestRequestTypeDef",
     "DisableRegionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "EnableRegionRequestRequestTypeDef",
     "GetAlternateContactRequestRequestTypeDef",
     "GetContactInformationRequestRequestTypeDef",
@@ -53,14 +54,45 @@
         "Name": str,
         "PhoneNumber": str,
         "Title": str,
     },
     total=False,
 )
 
+_RequiredContactInformationOutputTypeDef = TypedDict(
+    "_RequiredContactInformationOutputTypeDef",
+    {
+        "AddressLine1": str,
+        "City": str,
+        "CountryCode": str,
+        "FullName": str,
+        "PhoneNumber": str,
+        "PostalCode": str,
+    },
+)
+_OptionalContactInformationOutputTypeDef = TypedDict(
+    "_OptionalContactInformationOutputTypeDef",
+    {
+        "AddressLine2": str,
+        "AddressLine3": str,
+        "CompanyName": str,
+        "DistrictOrCounty": str,
+        "StateOrRegion": str,
+        "WebsiteUrl": str,
+    },
+    total=False,
+)
+
+
+class ContactInformationOutputTypeDef(
+    _RequiredContactInformationOutputTypeDef, _OptionalContactInformationOutputTypeDef
+):
+    pass
+
+
 _RequiredContactInformationTypeDef = TypedDict(
     "_RequiredContactInformationTypeDef",
     {
         "AddressLine1": str,
         "City": str,
         "CountryCode": str,
         "FullName": str,
@@ -307,15 +339,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContactInformationResponseTypeDef = TypedDict(
     "GetContactInformationResponseTypeDef",
     {
-        "ContactInformation": ContactInformationTypeDef,
+        "ContactInformation": ContactInformationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRegionOptStatusResponseTypeDef = TypedDict(
     "GetRegionOptStatusResponseTypeDef",
     {
```

### Comparing `mypy-boto3-account-1.28.0/mypy_boto3_account/type_defs.pyi` & `mypy-boto3-account-1.28.12/mypy_boto3_account/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AlternateContactTypeDef",
+    "ContactInformationOutputTypeDef",
     "ContactInformationTypeDef",
     "DeleteAlternateContactRequestRequestTypeDef",
     "DisableRegionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "EnableRegionRequestRequestTypeDef",
     "GetAlternateContactRequestRequestTypeDef",
     "GetContactInformationRequestRequestTypeDef",
@@ -52,14 +53,43 @@
         "Name": str,
         "PhoneNumber": str,
         "Title": str,
     },
     total=False,
 )
 
+_RequiredContactInformationOutputTypeDef = TypedDict(
+    "_RequiredContactInformationOutputTypeDef",
+    {
+        "AddressLine1": str,
+        "City": str,
+        "CountryCode": str,
+        "FullName": str,
+        "PhoneNumber": str,
+        "PostalCode": str,
+    },
+)
+_OptionalContactInformationOutputTypeDef = TypedDict(
+    "_OptionalContactInformationOutputTypeDef",
+    {
+        "AddressLine2": str,
+        "AddressLine3": str,
+        "CompanyName": str,
+        "DistrictOrCounty": str,
+        "StateOrRegion": str,
+        "WebsiteUrl": str,
+    },
+    total=False,
+)
+
+class ContactInformationOutputTypeDef(
+    _RequiredContactInformationOutputTypeDef, _OptionalContactInformationOutputTypeDef
+):
+    pass
+
 _RequiredContactInformationTypeDef = TypedDict(
     "_RequiredContactInformationTypeDef",
     {
         "AddressLine1": str,
         "City": str,
         "CountryCode": str,
         "FullName": str,
@@ -290,15 +320,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContactInformationResponseTypeDef = TypedDict(
     "GetContactInformationResponseTypeDef",
     {
-        "ContactInformation": ContactInformationTypeDef,
+        "ContactInformation": ContactInformationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRegionOptStatusResponseTypeDef = TypedDict(
     "GetRegionOptStatusResponseTypeDef",
     {
```

### Comparing `mypy-boto3-account-1.28.0/mypy_boto3_account.egg-info/PKG-INFO` & `mypy-boto3-account-1.28.12/mypy_boto3_account.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-account
-Version: 1.28.0
-Summary: Type annotations for boto3.Account 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Account 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-account"></a>
 
 # mypy-boto3-account
 
 [![PyPI - mypy-boto3-account](https://img.shields.io/pypi/v/mypy-boto3-account.svg?color=blue)](https://pypi.org/project/mypy-boto3-account)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-account.svg?color=blue)](https://pypi.org/project/mypy-boto3-account)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-account?color=blue)](https://pypistats.org/packages/mypy-boto3-account)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-account)](https://pepy.tech/project/mypy-boto3-account)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Account 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
+[boto3.Account 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
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
 [mypy-boto3-account docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,14 +320,15 @@
 
 `mypy_boto3_account.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_account.type_defs import (
     AlternateContactTypeDef,
+    ContactInformationOutputTypeDef,
     ContactInformationTypeDef,
     DeleteAlternateContactRequestRequestTypeDef,
     DisableRegionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     EnableRegionRequestRequestTypeDef,
     GetAlternateContactRequestRequestTypeDef,
     GetContactInformationRequestRequestTypeDef,
```

### Comparing `mypy-boto3-account-1.28.0/mypy_boto3_account.egg-info/SOURCES.txt` & `mypy-boto3-account-1.28.12/mypy_boto3_account.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.28.0/setup.py` & `mypy-boto3-account-1.28.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-account",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_account"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Account 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Account 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

