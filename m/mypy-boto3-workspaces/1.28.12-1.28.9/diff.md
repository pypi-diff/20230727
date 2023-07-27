# Comparing `tmp/mypy-boto3-workspaces-1.28.12.tar.gz` & `tmp/mypy-boto3-workspaces-1.28.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workspaces-1.28.12.tar", last modified: Thu Jul 27 11:49:51 2023, max compression
+gzip compressed data, was "mypy-boto3-workspaces-1.28.9.tar", last modified: Fri Jul 21 20:32:58 2023, max compression
```

## Comparing `mypy-boto3-workspaces-1.28.12.tar` & `mypy-boto3-workspaces-1.28.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:51.137507 mypy-boto3-workspaces-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:58.000000 mypy-boto3-workspaces-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22480 2023-07-27 11:49:51.137507 mypy-boto3-workspaces-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-07-27 11:48:58.000000 mypy-boto3-workspaces-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:51.137507 mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-27 11:48:58.000000 mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-27 11:48:58.000000 mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 11:48:58.000000 mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48055 2023-07-27 11:48:58.000000 mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47975 2023-07-27 11:48:58.000000 mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-07-27 11:48:59.000000 mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13352 2023-07-27 11:48:58.000000 mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-07-27 11:48:58.000000 mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-07-27 11:48:58.000000 mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:58.000000 mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    58694 2023-07-27 11:49:02.000000 mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    58647 2023-07-27 11:49:01.000000 mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:58.000000 mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:51.137507 mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22480 2023-07-27 11:49:51.000000 mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 11:49:51.000000 mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:51.000000 mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:51.000000 mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:51.000000 mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 11:49:51.000000 mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:51.137507 mypy-boto3-workspaces-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 11:48:58.000000 mypy-boto3-workspaces-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.251903 mypy-boto3-workspaces-1.28.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22493 2023-07-21 20:32:58.243903 mypy-boto3-workspaces-1.28.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.243903 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48055 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47975 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57338 2023-07-21 20:32:48.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57297 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.243903 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22493 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 20:32:58.251903 mypy-boto3-workspaces-1.28.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/setup.py
```

### Comparing `mypy-boto3-workspaces-1.28.12/LICENSE` & `mypy-boto3-workspaces-1.28.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.12/PKG-INFO` & `mypy-boto3-workspaces-1.28.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces
-Version: 1.28.12
-Summary: Type annotations for boto3.WorkSpaces 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.9
+Summary: Type annotations for boto3.WorkSpaces 1.28.9 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-workspaces"></a>
 
 # mypy-boto3-workspaces
 
 [![PyPI - mypy-boto3-workspaces](https://img.shields.io/pypi/v/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces)](https://pepy.tech/project/mypy-boto3-workspaces)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpaces 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[boto3.WorkSpaces 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-workspaces-1.28.12/README.md` & `mypy-boto3-workspaces-1.28.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-workspaces"></a>
 
 # mypy-boto3-workspaces
 
 [![PyPI - mypy-boto3-workspaces](https://img.shields.io/pypi/v/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces)](https://pepy.tech/project/mypy-boto3-workspaces)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpaces 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[boto3.WorkSpaces 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/__init__.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/__init__.pyi` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/__main__.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkSpaces 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.WorkSpaces 1.28.9\nVersion:         1.28.9\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.9")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/client.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/client.pyi` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/literals.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -368,15 +367,14 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
```

### Comparing `mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/literals.pyi` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -366,15 +365,14 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
```

### Comparing `mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/paginator.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/paginator.pyi` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/type_defs.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,15 +239,14 @@
         "ModificationState": DedicatedTenancyModificationStateEnumType,
         "DedicatedTenancySupport": DedicatedTenancySupportResultEnumType,
         "DedicatedTenancyManagementCidrRange": str,
         "StartTime": datetime,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 AssociateConnectionAliasRequestRequestTypeDef = TypedDict(
     "AssociateConnectionAliasRequestRequestTypeDef",
     {
         "AliasId": str,
         "ResourceId": str,
@@ -284,15 +283,14 @@
 
 CertificateBasedAuthPropertiesOutputTypeDef = TypedDict(
     "CertificateBasedAuthPropertiesOutputTypeDef",
     {
         "Status": CertificateBasedAuthStatusEnumType,
         "CertificateAuthorityArn": str,
     },
-    total=False,
 )
 
 CertificateBasedAuthPropertiesTypeDef = TypedDict(
     "CertificateBasedAuthPropertiesTypeDef",
     {
         "Status": CertificateBasedAuthStatusEnumType,
         "CertificateAuthorityArn": str,
@@ -302,15 +300,14 @@
 
 ClientPropertiesOutputTypeDef = TypedDict(
     "ClientPropertiesOutputTypeDef",
     {
         "ReconnectEnabled": ReconnectEnumType,
         "LogUploadEnabled": LogUploadEnumType,
     },
-    total=False,
 )
 
 ClientPropertiesTypeDef = TypedDict(
     "ClientPropertiesTypeDef",
     {
         "ReconnectEnabled": ReconnectEnumType,
         "LogUploadEnabled": LogUploadEnumType,
@@ -319,15 +316,14 @@
 )
 
 ComputeTypeOutputTypeDef = TypedDict(
     "ComputeTypeOutputTypeDef",
     {
         "Name": ComputeType,
     },
-    total=False,
 )
 
 ComputeTypeTypeDef = TypedDict(
     "ComputeTypeTypeDef",
     {
         "Name": ComputeType,
     },
@@ -338,26 +334,24 @@
     "ConnectClientAddInTypeDef",
     {
         "AddInId": str,
         "ResourceId": str,
         "Name": str,
         "URL": str,
     },
-    total=False,
 )
 
 ConnectionAliasAssociationTypeDef = TypedDict(
     "ConnectionAliasAssociationTypeDef",
     {
         "AssociationStatus": AssociationStatusType,
         "AssociatedAccountId": str,
         "ResourceId": str,
         "ConnectionIdentifier": str,
     },
-    total=False,
 )
 
 ConnectionAliasPermissionOutputTypeDef = TypedDict(
     "ConnectionAliasPermissionOutputTypeDef",
     {
         "SharedAccountId": str,
         "AllowAssociation": bool,
@@ -404,15 +398,14 @@
     "PendingCreateStandbyWorkspacesRequestTypeDef",
     {
         "UserName": str,
         "DirectoryId": str,
         "State": WorkspaceStateType,
         "WorkspaceId": str,
     },
-    total=False,
 )
 
 RootStorageTypeDef = TypedDict(
     "RootStorageTypeDef",
     {
         "Capacity": str,
     },
@@ -428,27 +421,25 @@
 )
 
 OperatingSystemTypeDef = TypedDict(
     "OperatingSystemTypeDef",
     {
         "Type": OperatingSystemTypeType,
     },
-    total=False,
 )
 
 DefaultClientBrandingAttributesTypeDef = TypedDict(
     "DefaultClientBrandingAttributesTypeDef",
     {
         "LogoUrl": str,
         "SupportEmail": str,
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Dict[str, str],
     },
-    total=False,
 )
 
 DefaultImportClientBrandingAttributesTypeDef = TypedDict(
     "DefaultImportClientBrandingAttributesTypeDef",
     {
         "Logo": Union[str, bytes, IO[Any], StreamingBody],
         "SupportEmail": str,
@@ -465,15 +456,14 @@
         "EnableWorkDocs": bool,
         "EnableInternetAccess": bool,
         "DefaultOu": str,
         "CustomSecurityGroupId": str,
         "UserEnabledAsLocalAdministrator": bool,
         "EnableMaintenanceMode": bool,
     },
-    total=False,
 )
 
 DeleteClientBrandingRequestRequestTypeDef = TypedDict(
     "DeleteClientBrandingRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Platforms": Sequence[ClientDeviceTypeType],
@@ -564,15 +554,14 @@
         "Logo2xUrl": str,
         "Logo3xUrl": str,
         "SupportEmail": str,
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Dict[str, str],
     },
-    total=False,
 )
 
 DescribeClientPropertiesRequestRequestTypeDef = TypedDict(
     "DescribeClientPropertiesRequestRequestTypeDef",
     {
         "ResourceIds": Sequence[str],
     },
@@ -648,33 +637,22 @@
 DescribeTagsRequestRequestTypeDef = TypedDict(
     "DescribeTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "Key": str,
-    },
-)
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
-    {
         "Value": str,
     },
-    total=False,
 )
 
-
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
-    pass
-
-
 DescribeWorkspaceBundlesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceBundlesRequestRequestTypeDef",
     {
         "BundleIds": Sequence[str],
         "Owner": str,
         "NextToken": str,
     },
@@ -715,15 +693,14 @@
 
 
 ImagePermissionTypeDef = TypedDict(
     "ImagePermissionTypeDef",
     {
         "SharedAccountId": str,
     },
-    total=False,
 )
 
 DescribeWorkspaceImagesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceImagesRequestRequestTypeDef",
     {
         "ImageIds": Sequence[str],
         "ImageType": ImageTypeType,
@@ -741,15 +718,14 @@
 )
 
 SnapshotTypeDef = TypedDict(
     "SnapshotTypeDef",
     {
         "SnapshotTime": datetime,
     },
-    total=False,
 )
 
 DescribeWorkspacesConnectionStatusRequestRequestTypeDef = TypedDict(
     "DescribeWorkspacesConnectionStatusRequestRequestTypeDef",
     {
         "WorkspaceIds": Sequence[str],
         "NextToken": str,
@@ -761,15 +737,14 @@
     "WorkspaceConnectionStatusTypeDef",
     {
         "WorkspaceId": str,
         "ConnectionState": ConnectionStateType,
         "ConnectionStateCheckTimestamp": datetime,
         "LastKnownUserConnectionTimestamp": datetime,
     },
-    total=False,
 )
 
 DescribeWorkspacesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspacesRequestRequestTypeDef",
     {
         "WorkspaceIds": Sequence[str],
         "DirectoryId": str,
@@ -799,15 +774,14 @@
 FailedWorkspaceChangeRequestTypeDef = TypedDict(
     "FailedWorkspaceChangeRequestTypeDef",
     {
         "WorkspaceId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 IosImportClientBrandingAttributesTypeDef = TypedDict(
     "IosImportClientBrandingAttributesTypeDef",
     {
         "Logo": Union[str, bytes, IO[Any], StreamingBody],
         "Logo2x": Union[str, bytes, IO[Any], StreamingBody],
@@ -822,15 +796,14 @@
 
 IpRuleItemOutputTypeDef = TypedDict(
     "IpRuleItemOutputTypeDef",
     {
         "ipRule": str,
         "ruleDesc": str,
     },
-    total=False,
 )
 
 _RequiredListAvailableManagementCidrRangesRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailableManagementCidrRangesRequestRequestTypeDef",
     {
         "ManagementCidrRangeConstraint": str,
     },
@@ -862,15 +835,14 @@
 
 ModificationStateTypeDef = TypedDict(
     "ModificationStateTypeDef",
     {
         "Resource": ModificationResourceEnumType,
         "State": ModificationStateEnumType,
     },
-    total=False,
 )
 
 ModifyAccountRequestRequestTypeDef = TypedDict(
     "ModifyAccountRequestRequestTypeDef",
     {
         "DedicatedTenancySupport": Literal["ENABLED"],
         "DedicatedTenancyManagementCidrRange": str,
@@ -967,15 +939,14 @@
     "RelatedWorkspacePropertiesTypeDef",
     {
         "WorkspaceId": str,
         "Region": str,
         "State": WorkspaceStateType,
         "Type": StandbyWorkspaceRelationshipTypeType,
     },
-    total=False,
 )
 
 RestoreWorkspaceRequestRequestTypeDef = TypedDict(
     "RestoreWorkspaceRequestRequestTypeDef",
     {
         "WorkspaceId": str,
     },
@@ -990,37 +961,34 @@
 )
 
 RootStorageOutputTypeDef = TypedDict(
     "RootStorageOutputTypeDef",
     {
         "Capacity": str,
     },
-    total=False,
 )
 
 SamlPropertiesOutputTypeDef = TypedDict(
     "SamlPropertiesOutputTypeDef",
     {
         "Status": SamlStatusEnumType,
         "UserAccessUrl": str,
         "RelayStateParameterName": str,
     },
-    total=False,
 )
 
 SelfservicePermissionsOutputTypeDef = TypedDict(
     "SelfservicePermissionsOutputTypeDef",
     {
         "RestartWorkspace": ReconnectEnumType,
         "IncreaseVolumeSize": ReconnectEnumType,
         "ChangeComputeType": ReconnectEnumType,
         "SwitchRunningMode": ReconnectEnumType,
         "RebuildWorkspace": ReconnectEnumType,
     },
-    total=False,
 )
 
 StartRequestTypeDef = TypedDict(
     "StartRequestTypeDef",
     {
         "WorkspaceId": str,
     },
@@ -1068,15 +1036,14 @@
 
 UpdateResultTypeDef = TypedDict(
     "UpdateResultTypeDef",
     {
         "UpdateAvailable": bool,
         "Description": str,
     },
-    total=False,
 )
 
 UpdateWorkspaceBundleRequestRequestTypeDef = TypedDict(
     "UpdateWorkspaceBundleRequestRequestTypeDef",
     {
         "BundleId": str,
         "ImageId": str,
@@ -1094,43 +1061,40 @@
 )
 
 UserStorageOutputTypeDef = TypedDict(
     "UserStorageOutputTypeDef",
     {
         "Capacity": str,
     },
-    total=False,
 )
 
 WorkspaceAccessPropertiesOutputTypeDef = TypedDict(
     "WorkspaceAccessPropertiesOutputTypeDef",
     {
         "DeviceTypeWindows": AccessPropertyValueType,
         "DeviceTypeOsx": AccessPropertyValueType,
         "DeviceTypeWeb": AccessPropertyValueType,
         "DeviceTypeIos": AccessPropertyValueType,
         "DeviceTypeAndroid": AccessPropertyValueType,
         "DeviceTypeChromeOs": AccessPropertyValueType,
         "DeviceTypeZeroClient": AccessPropertyValueType,
         "DeviceTypeLinux": AccessPropertyValueType,
     },
-    total=False,
 )
 
 WorkspacePropertiesOutputTypeDef = TypedDict(
     "WorkspacePropertiesOutputTypeDef",
     {
         "RunningMode": RunningModeType,
         "RunningModeAutoStopTimeoutInMinutes": int,
         "RootVolumeSizeGib": int,
         "UserVolumeSizeGib": int,
         "ComputeTypeName": ComputeType,
         "Protocols": List[ProtocolType],
     },
-    total=False,
 )
 
 AssociateConnectionAliasResultTypeDef = TypedDict(
     "AssociateConnectionAliasResultTypeDef",
     {
         "ConnectionIdentifier": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1264,15 +1228,14 @@
 
 ClientPropertiesResultTypeDef = TypedDict(
     "ClientPropertiesResultTypeDef",
     {
         "ResourceId": str,
         "ClientProperties": ClientPropertiesOutputTypeDef,
     },
-    total=False,
 )
 
 ModifyClientPropertiesRequestRequestTypeDef = TypedDict(
     "ModifyClientPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
         "ClientProperties": ClientPropertiesTypeDef,
@@ -1293,15 +1256,14 @@
     {
         "ConnectionString": str,
         "AliasId": str,
         "State": ConnectionAliasStateType,
         "OwnerAccountId": str,
         "Associations": List[ConnectionAliasAssociationTypeDef],
     },
-    total=False,
 )
 
 DescribeConnectionAliasPermissionsResultTypeDef = TypedDict(
     "DescribeConnectionAliasPermissionsResultTypeDef",
     {
         "AliasId": str,
         "ConnectionAliasPermissions": List[ConnectionAliasPermissionOutputTypeDef],
@@ -1679,37 +1641,24 @@
     "DescribeTagsResultTypeDef",
     {
         "TagList": List[TagOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStandbyWorkspaceOutputTypeDef = TypedDict(
-    "_RequiredStandbyWorkspaceOutputTypeDef",
+StandbyWorkspaceOutputTypeDef = TypedDict(
+    "StandbyWorkspaceOutputTypeDef",
     {
         "PrimaryWorkspaceId": str,
-        "DirectoryId": str,
-    },
-)
-_OptionalStandbyWorkspaceOutputTypeDef = TypedDict(
-    "_OptionalStandbyWorkspaceOutputTypeDef",
-    {
         "VolumeEncryptionKey": str,
+        "DirectoryId": str,
         "Tags": List[TagOutputTypeDef],
     },
-    total=False,
 )
 
-
-class StandbyWorkspaceOutputTypeDef(
-    _RequiredStandbyWorkspaceOutputTypeDef, _OptionalStandbyWorkspaceOutputTypeDef
-):
-    pass
-
-
 DescribeWorkspaceImagePermissionsResultTypeDef = TypedDict(
     "DescribeWorkspaceImagePermissionsResultTypeDef",
     {
         "ImageId": str,
         "ImagePermissions": List[ImagePermissionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1805,15 +1754,14 @@
     "WorkspacesIpGroupTypeDef",
     {
         "groupId": str,
         "groupName": str,
         "groupDesc": str,
         "userRules": List[IpRuleItemOutputTypeDef],
     },
-    total=False,
 )
 
 _RequiredModifySamlPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredModifySamlPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
@@ -1938,15 +1886,14 @@
         "RequiredTenancy": WorkspaceImageRequiredTenancyType,
         "ErrorCode": str,
         "ErrorMessage": str,
         "Created": datetime,
         "OwnerAccountId": str,
         "Updates": UpdateResultTypeDef,
     },
-    total=False,
 )
 
 WorkspaceBundleTypeDef = TypedDict(
     "WorkspaceBundleTypeDef",
     {
         "BundleId": str,
         "Name": str,
@@ -1957,15 +1904,14 @@
         "UserStorage": UserStorageOutputTypeDef,
         "ComputeType": ComputeTypeOutputTypeDef,
         "LastUpdatedTime": datetime,
         "CreationTime": datetime,
         "State": WorkspaceBundleStateType,
         "BundleType": BundleTypeType,
     },
-    total=False,
 )
 
 WorkspaceDirectoryTypeDef = TypedDict(
     "WorkspaceDirectoryTypeDef",
     {
         "DirectoryId": str,
         "Alias": str,
@@ -1982,44 +1928,30 @@
         "ipGroupIds": List[str],
         "WorkspaceAccessProperties": WorkspaceAccessPropertiesOutputTypeDef,
         "Tenancy": TenancyType,
         "SelfservicePermissions": SelfservicePermissionsOutputTypeDef,
         "SamlProperties": SamlPropertiesOutputTypeDef,
         "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesOutputTypeDef,
     },
-    total=False,
 )
 
-_RequiredWorkspaceRequestOutputTypeDef = TypedDict(
-    "_RequiredWorkspaceRequestOutputTypeDef",
+WorkspaceRequestOutputTypeDef = TypedDict(
+    "WorkspaceRequestOutputTypeDef",
     {
         "DirectoryId": str,
         "UserName": str,
         "BundleId": str,
-    },
-)
-_OptionalWorkspaceRequestOutputTypeDef = TypedDict(
-    "_OptionalWorkspaceRequestOutputTypeDef",
-    {
         "VolumeEncryptionKey": str,
         "UserVolumeEncryptionEnabled": bool,
         "RootVolumeEncryptionEnabled": bool,
         "WorkspaceProperties": WorkspacePropertiesOutputTypeDef,
         "Tags": List[TagOutputTypeDef],
     },
-    total=False,
 )
 
-
-class WorkspaceRequestOutputTypeDef(
-    _RequiredWorkspaceRequestOutputTypeDef, _OptionalWorkspaceRequestOutputTypeDef
-):
-    pass
-
-
 WorkspaceTypeDef = TypedDict(
     "WorkspaceTypeDef",
     {
         "WorkspaceId": str,
         "DirectoryId": str,
         "UserName": str,
         "IpAddress": str,
@@ -2032,15 +1964,14 @@
         "VolumeEncryptionKey": str,
         "UserVolumeEncryptionEnabled": bool,
         "RootVolumeEncryptionEnabled": bool,
         "WorkspaceProperties": WorkspacePropertiesOutputTypeDef,
         "ModificationStates": List[ModificationStateTypeDef],
         "RelatedWorkspaces": List[RelatedWorkspacePropertiesTypeDef],
     },
-    total=False,
 )
 
 DescribeClientPropertiesResultTypeDef = TypedDict(
     "DescribeClientPropertiesResultTypeDef",
     {
         "ClientPropertiesList": List[ClientPropertiesResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2067,15 +1998,14 @@
 FailedCreateStandbyWorkspacesRequestTypeDef = TypedDict(
     "FailedCreateStandbyWorkspacesRequestTypeDef",
     {
         "StandbyWorkspaceRequest": StandbyWorkspaceOutputTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 DescribeIpGroupsResultTypeDef = TypedDict(
     "DescribeIpGroupsResultTypeDef",
     {
         "Result": List[WorkspacesIpGroupTypeDef],
         "NextToken": str,
@@ -2128,15 +2058,14 @@
 FailedCreateWorkspaceRequestTypeDef = TypedDict(
     "FailedCreateWorkspaceRequestTypeDef",
     {
         "WorkspaceRequest": WorkspaceRequestOutputTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 DescribeWorkspacesResultTypeDef = TypedDict(
     "DescribeWorkspacesResultTypeDef",
     {
         "Workspaces": List[WorkspaceTypeDef],
         "NextToken": str,
```

### Comparing `mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces/type_defs.pyi` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -238,15 +238,14 @@
         "ModificationState": DedicatedTenancyModificationStateEnumType,
         "DedicatedTenancySupport": DedicatedTenancySupportResultEnumType,
         "DedicatedTenancyManagementCidrRange": str,
         "StartTime": datetime,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 AssociateConnectionAliasRequestRequestTypeDef = TypedDict(
     "AssociateConnectionAliasRequestRequestTypeDef",
     {
         "AliasId": str,
         "ResourceId": str,
@@ -283,15 +282,14 @@
 
 CertificateBasedAuthPropertiesOutputTypeDef = TypedDict(
     "CertificateBasedAuthPropertiesOutputTypeDef",
     {
         "Status": CertificateBasedAuthStatusEnumType,
         "CertificateAuthorityArn": str,
     },
-    total=False,
 )
 
 CertificateBasedAuthPropertiesTypeDef = TypedDict(
     "CertificateBasedAuthPropertiesTypeDef",
     {
         "Status": CertificateBasedAuthStatusEnumType,
         "CertificateAuthorityArn": str,
@@ -301,15 +299,14 @@
 
 ClientPropertiesOutputTypeDef = TypedDict(
     "ClientPropertiesOutputTypeDef",
     {
         "ReconnectEnabled": ReconnectEnumType,
         "LogUploadEnabled": LogUploadEnumType,
     },
-    total=False,
 )
 
 ClientPropertiesTypeDef = TypedDict(
     "ClientPropertiesTypeDef",
     {
         "ReconnectEnabled": ReconnectEnumType,
         "LogUploadEnabled": LogUploadEnumType,
@@ -318,15 +315,14 @@
 )
 
 ComputeTypeOutputTypeDef = TypedDict(
     "ComputeTypeOutputTypeDef",
     {
         "Name": ComputeType,
     },
-    total=False,
 )
 
 ComputeTypeTypeDef = TypedDict(
     "ComputeTypeTypeDef",
     {
         "Name": ComputeType,
     },
@@ -337,26 +333,24 @@
     "ConnectClientAddInTypeDef",
     {
         "AddInId": str,
         "ResourceId": str,
         "Name": str,
         "URL": str,
     },
-    total=False,
 )
 
 ConnectionAliasAssociationTypeDef = TypedDict(
     "ConnectionAliasAssociationTypeDef",
     {
         "AssociationStatus": AssociationStatusType,
         "AssociatedAccountId": str,
         "ResourceId": str,
         "ConnectionIdentifier": str,
     },
-    total=False,
 )
 
 ConnectionAliasPermissionOutputTypeDef = TypedDict(
     "ConnectionAliasPermissionOutputTypeDef",
     {
         "SharedAccountId": str,
         "AllowAssociation": bool,
@@ -401,15 +395,14 @@
     "PendingCreateStandbyWorkspacesRequestTypeDef",
     {
         "UserName": str,
         "DirectoryId": str,
         "State": WorkspaceStateType,
         "WorkspaceId": str,
     },
-    total=False,
 )
 
 RootStorageTypeDef = TypedDict(
     "RootStorageTypeDef",
     {
         "Capacity": str,
     },
@@ -425,27 +418,25 @@
 )
 
 OperatingSystemTypeDef = TypedDict(
     "OperatingSystemTypeDef",
     {
         "Type": OperatingSystemTypeType,
     },
-    total=False,
 )
 
 DefaultClientBrandingAttributesTypeDef = TypedDict(
     "DefaultClientBrandingAttributesTypeDef",
     {
         "LogoUrl": str,
         "SupportEmail": str,
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Dict[str, str],
     },
-    total=False,
 )
 
 DefaultImportClientBrandingAttributesTypeDef = TypedDict(
     "DefaultImportClientBrandingAttributesTypeDef",
     {
         "Logo": Union[str, bytes, IO[Any], StreamingBody],
         "SupportEmail": str,
@@ -462,15 +453,14 @@
         "EnableWorkDocs": bool,
         "EnableInternetAccess": bool,
         "DefaultOu": str,
         "CustomSecurityGroupId": str,
         "UserEnabledAsLocalAdministrator": bool,
         "EnableMaintenanceMode": bool,
     },
-    total=False,
 )
 
 DeleteClientBrandingRequestRequestTypeDef = TypedDict(
     "DeleteClientBrandingRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Platforms": Sequence[ClientDeviceTypeType],
@@ -561,15 +551,14 @@
         "Logo2xUrl": str,
         "Logo3xUrl": str,
         "SupportEmail": str,
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Dict[str, str],
     },
-    total=False,
 )
 
 DescribeClientPropertiesRequestRequestTypeDef = TypedDict(
     "DescribeClientPropertiesRequestRequestTypeDef",
     {
         "ResourceIds": Sequence[str],
     },
@@ -641,31 +630,22 @@
 DescribeTagsRequestRequestTypeDef = TypedDict(
     "DescribeTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "Key": str,
-    },
-)
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
-    {
         "Value": str,
     },
-    total=False,
 )
 
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
-    pass
-
 DescribeWorkspaceBundlesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceBundlesRequestRequestTypeDef",
     {
         "BundleIds": Sequence[str],
         "Owner": str,
         "NextToken": str,
     },
@@ -704,15 +684,14 @@
     pass
 
 ImagePermissionTypeDef = TypedDict(
     "ImagePermissionTypeDef",
     {
         "SharedAccountId": str,
     },
-    total=False,
 )
 
 DescribeWorkspaceImagesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceImagesRequestRequestTypeDef",
     {
         "ImageIds": Sequence[str],
         "ImageType": ImageTypeType,
@@ -730,15 +709,14 @@
 )
 
 SnapshotTypeDef = TypedDict(
     "SnapshotTypeDef",
     {
         "SnapshotTime": datetime,
     },
-    total=False,
 )
 
 DescribeWorkspacesConnectionStatusRequestRequestTypeDef = TypedDict(
     "DescribeWorkspacesConnectionStatusRequestRequestTypeDef",
     {
         "WorkspaceIds": Sequence[str],
         "NextToken": str,
@@ -750,15 +728,14 @@
     "WorkspaceConnectionStatusTypeDef",
     {
         "WorkspaceId": str,
         "ConnectionState": ConnectionStateType,
         "ConnectionStateCheckTimestamp": datetime,
         "LastKnownUserConnectionTimestamp": datetime,
     },
-    total=False,
 )
 
 DescribeWorkspacesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspacesRequestRequestTypeDef",
     {
         "WorkspaceIds": Sequence[str],
         "DirectoryId": str,
@@ -788,15 +765,14 @@
 FailedWorkspaceChangeRequestTypeDef = TypedDict(
     "FailedWorkspaceChangeRequestTypeDef",
     {
         "WorkspaceId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 IosImportClientBrandingAttributesTypeDef = TypedDict(
     "IosImportClientBrandingAttributesTypeDef",
     {
         "Logo": Union[str, bytes, IO[Any], StreamingBody],
         "Logo2x": Union[str, bytes, IO[Any], StreamingBody],
@@ -811,15 +787,14 @@
 
 IpRuleItemOutputTypeDef = TypedDict(
     "IpRuleItemOutputTypeDef",
     {
         "ipRule": str,
         "ruleDesc": str,
     },
-    total=False,
 )
 
 _RequiredListAvailableManagementCidrRangesRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailableManagementCidrRangesRequestRequestTypeDef",
     {
         "ManagementCidrRangeConstraint": str,
     },
@@ -849,15 +824,14 @@
 
 ModificationStateTypeDef = TypedDict(
     "ModificationStateTypeDef",
     {
         "Resource": ModificationResourceEnumType,
         "State": ModificationStateEnumType,
     },
-    total=False,
 )
 
 ModifyAccountRequestRequestTypeDef = TypedDict(
     "ModifyAccountRequestRequestTypeDef",
     {
         "DedicatedTenancySupport": Literal["ENABLED"],
         "DedicatedTenancyManagementCidrRange": str,
@@ -954,15 +928,14 @@
     "RelatedWorkspacePropertiesTypeDef",
     {
         "WorkspaceId": str,
         "Region": str,
         "State": WorkspaceStateType,
         "Type": StandbyWorkspaceRelationshipTypeType,
     },
-    total=False,
 )
 
 RestoreWorkspaceRequestRequestTypeDef = TypedDict(
     "RestoreWorkspaceRequestRequestTypeDef",
     {
         "WorkspaceId": str,
     },
@@ -977,37 +950,34 @@
 )
 
 RootStorageOutputTypeDef = TypedDict(
     "RootStorageOutputTypeDef",
     {
         "Capacity": str,
     },
-    total=False,
 )
 
 SamlPropertiesOutputTypeDef = TypedDict(
     "SamlPropertiesOutputTypeDef",
     {
         "Status": SamlStatusEnumType,
         "UserAccessUrl": str,
         "RelayStateParameterName": str,
     },
-    total=False,
 )
 
 SelfservicePermissionsOutputTypeDef = TypedDict(
     "SelfservicePermissionsOutputTypeDef",
     {
         "RestartWorkspace": ReconnectEnumType,
         "IncreaseVolumeSize": ReconnectEnumType,
         "ChangeComputeType": ReconnectEnumType,
         "SwitchRunningMode": ReconnectEnumType,
         "RebuildWorkspace": ReconnectEnumType,
     },
-    total=False,
 )
 
 StartRequestTypeDef = TypedDict(
     "StartRequestTypeDef",
     {
         "WorkspaceId": str,
     },
@@ -1053,15 +1023,14 @@
 
 UpdateResultTypeDef = TypedDict(
     "UpdateResultTypeDef",
     {
         "UpdateAvailable": bool,
         "Description": str,
     },
-    total=False,
 )
 
 UpdateWorkspaceBundleRequestRequestTypeDef = TypedDict(
     "UpdateWorkspaceBundleRequestRequestTypeDef",
     {
         "BundleId": str,
         "ImageId": str,
@@ -1079,43 +1048,40 @@
 )
 
 UserStorageOutputTypeDef = TypedDict(
     "UserStorageOutputTypeDef",
     {
         "Capacity": str,
     },
-    total=False,
 )
 
 WorkspaceAccessPropertiesOutputTypeDef = TypedDict(
     "WorkspaceAccessPropertiesOutputTypeDef",
     {
         "DeviceTypeWindows": AccessPropertyValueType,
         "DeviceTypeOsx": AccessPropertyValueType,
         "DeviceTypeWeb": AccessPropertyValueType,
         "DeviceTypeIos": AccessPropertyValueType,
         "DeviceTypeAndroid": AccessPropertyValueType,
         "DeviceTypeChromeOs": AccessPropertyValueType,
         "DeviceTypeZeroClient": AccessPropertyValueType,
         "DeviceTypeLinux": AccessPropertyValueType,
     },
-    total=False,
 )
 
 WorkspacePropertiesOutputTypeDef = TypedDict(
     "WorkspacePropertiesOutputTypeDef",
     {
         "RunningMode": RunningModeType,
         "RunningModeAutoStopTimeoutInMinutes": int,
         "RootVolumeSizeGib": int,
         "UserVolumeSizeGib": int,
         "ComputeTypeName": ComputeType,
         "Protocols": List[ProtocolType],
     },
-    total=False,
 )
 
 AssociateConnectionAliasResultTypeDef = TypedDict(
     "AssociateConnectionAliasResultTypeDef",
     {
         "ConnectionIdentifier": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1247,15 +1213,14 @@
 
 ClientPropertiesResultTypeDef = TypedDict(
     "ClientPropertiesResultTypeDef",
     {
         "ResourceId": str,
         "ClientProperties": ClientPropertiesOutputTypeDef,
     },
-    total=False,
 )
 
 ModifyClientPropertiesRequestRequestTypeDef = TypedDict(
     "ModifyClientPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
         "ClientProperties": ClientPropertiesTypeDef,
@@ -1276,15 +1241,14 @@
     {
         "ConnectionString": str,
         "AliasId": str,
         "State": ConnectionAliasStateType,
         "OwnerAccountId": str,
         "Associations": List[ConnectionAliasAssociationTypeDef],
     },
-    total=False,
 )
 
 DescribeConnectionAliasPermissionsResultTypeDef = TypedDict(
     "DescribeConnectionAliasPermissionsResultTypeDef",
     {
         "AliasId": str,
         "ConnectionAliasPermissions": List[ConnectionAliasPermissionOutputTypeDef],
@@ -1642,35 +1606,24 @@
     "DescribeTagsResultTypeDef",
     {
         "TagList": List[TagOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStandbyWorkspaceOutputTypeDef = TypedDict(
-    "_RequiredStandbyWorkspaceOutputTypeDef",
+StandbyWorkspaceOutputTypeDef = TypedDict(
+    "StandbyWorkspaceOutputTypeDef",
     {
         "PrimaryWorkspaceId": str,
-        "DirectoryId": str,
-    },
-)
-_OptionalStandbyWorkspaceOutputTypeDef = TypedDict(
-    "_OptionalStandbyWorkspaceOutputTypeDef",
-    {
         "VolumeEncryptionKey": str,
+        "DirectoryId": str,
         "Tags": List[TagOutputTypeDef],
     },
-    total=False,
 )
 
-class StandbyWorkspaceOutputTypeDef(
-    _RequiredStandbyWorkspaceOutputTypeDef, _OptionalStandbyWorkspaceOutputTypeDef
-):
-    pass
-
 DescribeWorkspaceImagePermissionsResultTypeDef = TypedDict(
     "DescribeWorkspaceImagePermissionsResultTypeDef",
     {
         "ImageId": str,
         "ImagePermissions": List[ImagePermissionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1764,15 +1717,14 @@
     "WorkspacesIpGroupTypeDef",
     {
         "groupId": str,
         "groupName": str,
         "groupDesc": str,
         "userRules": List[IpRuleItemOutputTypeDef],
     },
-    total=False,
 )
 
 _RequiredModifySamlPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredModifySamlPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
@@ -1893,15 +1845,14 @@
         "RequiredTenancy": WorkspaceImageRequiredTenancyType,
         "ErrorCode": str,
         "ErrorMessage": str,
         "Created": datetime,
         "OwnerAccountId": str,
         "Updates": UpdateResultTypeDef,
     },
-    total=False,
 )
 
 WorkspaceBundleTypeDef = TypedDict(
     "WorkspaceBundleTypeDef",
     {
         "BundleId": str,
         "Name": str,
@@ -1912,15 +1863,14 @@
         "UserStorage": UserStorageOutputTypeDef,
         "ComputeType": ComputeTypeOutputTypeDef,
         "LastUpdatedTime": datetime,
         "CreationTime": datetime,
         "State": WorkspaceBundleStateType,
         "BundleType": BundleTypeType,
     },
-    total=False,
 )
 
 WorkspaceDirectoryTypeDef = TypedDict(
     "WorkspaceDirectoryTypeDef",
     {
         "DirectoryId": str,
         "Alias": str,
@@ -1937,42 +1887,30 @@
         "ipGroupIds": List[str],
         "WorkspaceAccessProperties": WorkspaceAccessPropertiesOutputTypeDef,
         "Tenancy": TenancyType,
         "SelfservicePermissions": SelfservicePermissionsOutputTypeDef,
         "SamlProperties": SamlPropertiesOutputTypeDef,
         "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesOutputTypeDef,
     },
-    total=False,
 )
 
-_RequiredWorkspaceRequestOutputTypeDef = TypedDict(
-    "_RequiredWorkspaceRequestOutputTypeDef",
+WorkspaceRequestOutputTypeDef = TypedDict(
+    "WorkspaceRequestOutputTypeDef",
     {
         "DirectoryId": str,
         "UserName": str,
         "BundleId": str,
-    },
-)
-_OptionalWorkspaceRequestOutputTypeDef = TypedDict(
-    "_OptionalWorkspaceRequestOutputTypeDef",
-    {
         "VolumeEncryptionKey": str,
         "UserVolumeEncryptionEnabled": bool,
         "RootVolumeEncryptionEnabled": bool,
         "WorkspaceProperties": WorkspacePropertiesOutputTypeDef,
         "Tags": List[TagOutputTypeDef],
     },
-    total=False,
 )
 
-class WorkspaceRequestOutputTypeDef(
-    _RequiredWorkspaceRequestOutputTypeDef, _OptionalWorkspaceRequestOutputTypeDef
-):
-    pass
-
 WorkspaceTypeDef = TypedDict(
     "WorkspaceTypeDef",
     {
         "WorkspaceId": str,
         "DirectoryId": str,
         "UserName": str,
         "IpAddress": str,
@@ -1985,15 +1923,14 @@
         "VolumeEncryptionKey": str,
         "UserVolumeEncryptionEnabled": bool,
         "RootVolumeEncryptionEnabled": bool,
         "WorkspaceProperties": WorkspacePropertiesOutputTypeDef,
         "ModificationStates": List[ModificationStateTypeDef],
         "RelatedWorkspaces": List[RelatedWorkspacePropertiesTypeDef],
     },
-    total=False,
 )
 
 DescribeClientPropertiesResultTypeDef = TypedDict(
     "DescribeClientPropertiesResultTypeDef",
     {
         "ClientPropertiesList": List[ClientPropertiesResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2020,15 +1957,14 @@
 FailedCreateStandbyWorkspacesRequestTypeDef = TypedDict(
     "FailedCreateStandbyWorkspacesRequestTypeDef",
     {
         "StandbyWorkspaceRequest": StandbyWorkspaceOutputTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 DescribeIpGroupsResultTypeDef = TypedDict(
     "DescribeIpGroupsResultTypeDef",
     {
         "Result": List[WorkspacesIpGroupTypeDef],
         "NextToken": str,
@@ -2081,15 +2017,14 @@
 FailedCreateWorkspaceRequestTypeDef = TypedDict(
     "FailedCreateWorkspaceRequestTypeDef",
     {
         "WorkspaceRequest": WorkspaceRequestOutputTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 DescribeWorkspacesResultTypeDef = TypedDict(
     "DescribeWorkspacesResultTypeDef",
     {
         "Workspaces": List[WorkspaceTypeDef],
         "NextToken": str,
```

### Comparing `mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces.egg-info/PKG-INFO` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces
-Version: 1.28.12
-Summary: Type annotations for boto3.WorkSpaces 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.9
+Summary: Type annotations for boto3.WorkSpaces 1.28.9 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-workspaces"></a>
 
 # mypy-boto3-workspaces
 
 [![PyPI - mypy-boto3-workspaces](https://img.shields.io/pypi/v/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces)](https://pepy.tech/project/mypy-boto3-workspaces)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpaces 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[boto3.WorkSpaces 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-workspaces-1.28.12/mypy_boto3_workspaces.egg-info/SOURCES.txt` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.12/setup.py` & `mypy-boto3-workspaces-1.28.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-workspaces",
-    version="1.28.12",
+    version="1.28.9",
     packages=["mypy_boto3_workspaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WorkSpaces 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.WorkSpaces 1.28.9 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

