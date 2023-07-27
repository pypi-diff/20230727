# Comparing `tmp/mypy-boto3-iotsecuretunneling-1.28.0.tar.gz` & `tmp/mypy-boto3-iotsecuretunneling-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotsecuretunneling-1.28.0.tar", last modified: Thu Jul  6 20:59:48 2023, max compression
+gzip compressed data, was "mypy-boto3-iotsecuretunneling-1.28.12.tar", last modified: Thu Jul 27 05:34:50 2023, max compression
```

## Comparing `mypy-boto3-iotsecuretunneling-1.28.0.tar` & `mypy-boto3-iotsecuretunneling-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:48.906332 mypy-boto3-iotsecuretunneling-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:43:54.000000 mypy-boto3-iotsecuretunneling-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13113 2023-07-06 20:59:48.894332 mypy-boto3-iotsecuretunneling-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-07-06 20:43:54.000000 mypy-boto3-iotsecuretunneling-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:48.894332 mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-06 20:43:54.000000 mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-06 20:43:54.000000 mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-06 20:43:54.000000 mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-06 20:43:54.000000 mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-07-06 20:43:54.000000 mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-07-06 20:43:56.000000 mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-07-06 20:43:56.000000 mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:43:54.000000 mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-07-06 20:43:56.000000 mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-06 20:43:56.000000 mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:43:54.000000 mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:48.894332 mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13113 2023-07-06 20:59:48.000000 mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-06 20:59:48.000000 mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:48.000000 mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:48.000000 mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:48.000000 mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-06 20:59:48.000000 mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:48.906332 mypy-boto3-iotsecuretunneling-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-06 20:43:54.000000 mypy-boto3-iotsecuretunneling-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:50.492479 mypy-boto3-iotsecuretunneling-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-07-27 05:34:50.488479 mypy-boto3-iotsecuretunneling-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:50.484479 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:50.488479 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-07-27 05:34:50.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-27 05:34:50.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:50.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:50.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:50.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-27 05:34:50.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:50.492479 mypy-boto3-iotsecuretunneling-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-27 05:24:08.000000 mypy-boto3-iotsecuretunneling-1.28.12/setup.py
```

### Comparing `mypy-boto3-iotsecuretunneling-1.28.0/LICENSE` & `mypy-boto3-iotsecuretunneling-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsecuretunneling-1.28.0/PKG-INFO` & `mypy-boto3-iotsecuretunneling-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotsecuretunneling
-Version: 1.28.0
-Summary: Type annotations for boto3.IoTSecureTunneling 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTSecureTunneling 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iotsecuretunneling"></a>
 
 # mypy-boto3-iotsecuretunneling
 
 [![PyPI - mypy-boto3-iotsecuretunneling](https://img.shields.io/pypi/v/mypy-boto3-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsecuretunneling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsecuretunneling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotsecuretunneling?color=blue)](https://pypistats.org/packages/mypy-boto3-iotsecuretunneling)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotsecuretunneling)](https://pepy.tech/project/mypy-boto3-iotsecuretunneling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSecureTunneling 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
+[boto3.IoTSecureTunneling 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
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
 [mypy-boto3-iotsecuretunneling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,28 +303,31 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotsecuretunneling.type_defs import (
     CloseTunnelRequestRequestTypeDef,
     ConnectionStateTypeDef,
     DescribeTunnelRequestRequestTypeDef,
+    DestinationConfigOutputTypeDef,
     DestinationConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     ListTunnelsRequestRequestTypeDef,
     TunnelSummaryTypeDef,
+    TagTypeDef,
     TimeoutConfigTypeDef,
     OpenTunnelResponseTypeDef,
     ResponseMetadataTypeDef,
     RotateTunnelAccessTokenResponseTypeDef,
+    TimeoutConfigOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     RotateTunnelAccessTokenRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     ListTunnelsResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     OpenTunnelRequestRequestTypeDef,
     TunnelTypeDef,
     DescribeTunnelResponseTypeDef,
 )
 
 
 def get_structure() -> CloseTunnelRequestRequestTypeDef:
```

### Comparing `mypy-boto3-iotsecuretunneling-1.28.0/README.md` & `mypy-boto3-iotsecuretunneling-1.28.12/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iotsecuretunneling"></a>
 
 # mypy-boto3-iotsecuretunneling
 
 [![PyPI - mypy-boto3-iotsecuretunneling](https://img.shields.io/pypi/v/mypy-boto3-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsecuretunneling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsecuretunneling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotsecuretunneling?color=blue)](https://pypistats.org/packages/mypy-boto3-iotsecuretunneling)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotsecuretunneling)](https://pepy.tech/project/mypy-boto3-iotsecuretunneling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSecureTunneling 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
+[boto3.IoTSecureTunneling 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
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
 [mypy-boto3-iotsecuretunneling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -271,28 +271,31 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotsecuretunneling.type_defs import (
     CloseTunnelRequestRequestTypeDef,
     ConnectionStateTypeDef,
     DescribeTunnelRequestRequestTypeDef,
+    DestinationConfigOutputTypeDef,
     DestinationConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     ListTunnelsRequestRequestTypeDef,
     TunnelSummaryTypeDef,
+    TagTypeDef,
     TimeoutConfigTypeDef,
     OpenTunnelResponseTypeDef,
     ResponseMetadataTypeDef,
     RotateTunnelAccessTokenResponseTypeDef,
+    TimeoutConfigOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     RotateTunnelAccessTokenRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     ListTunnelsResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     OpenTunnelRequestRequestTypeDef,
     TunnelTypeDef,
     DescribeTunnelResponseTypeDef,
 )
 
 
 def get_structure() -> CloseTunnelRequestRequestTypeDef:
```

### Comparing `mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling/__main__.py` & `mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTSecureTunneling 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.IoTSecureTunneling 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling\nOther"
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

### Comparing `mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling/client.py` & `mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling/client.pyi` & `mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling/literals.py` & `mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/literals.py`

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

### Comparing `mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling/literals.pyi` & `mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/literals.pyi`

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

### Comparing `mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling/type_defs.py` & `mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -18,33 +18,35 @@
 from .literals import ClientModeType, ConnectionStatusType, TunnelStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CloseTunnelRequestRequestTypeDef",
     "ConnectionStateTypeDef",
     "DescribeTunnelRequestRequestTypeDef",
+    "DestinationConfigOutputTypeDef",
     "DestinationConfigTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "ListTunnelsRequestRequestTypeDef",
     "TunnelSummaryTypeDef",
+    "TagTypeDef",
     "TimeoutConfigTypeDef",
     "OpenTunnelResponseTypeDef",
     "ResponseMetadataTypeDef",
     "RotateTunnelAccessTokenResponseTypeDef",
+    "TimeoutConfigOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "RotateTunnelAccessTokenRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "ListTunnelsResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "OpenTunnelRequestRequestTypeDef",
     "TunnelTypeDef",
     "DescribeTunnelResponseTypeDef",
 )
 
 _RequiredCloseTunnelRequestRequestTypeDef = TypedDict(
     "_RequiredCloseTunnelRequestRequestTypeDef",
@@ -56,21 +58,19 @@
     "_OptionalCloseTunnelRequestRequestTypeDef",
     {
         "delete": bool,
     },
     total=False,
 )
 
-
 class CloseTunnelRequestRequestTypeDef(
     _RequiredCloseTunnelRequestRequestTypeDef, _OptionalCloseTunnelRequestRequestTypeDef
 ):
     pass
 
-
 ConnectionStateTypeDef = TypedDict(
     "ConnectionStateTypeDef",
     {
         "status": ConnectionStatusType,
         "lastUpdatedAt": datetime,
     },
     total=False,
@@ -79,44 +79,61 @@
 DescribeTunnelRequestRequestTypeDef = TypedDict(
     "DescribeTunnelRequestRequestTypeDef",
     {
         "tunnelId": str,
     },
 )
 
+_RequiredDestinationConfigOutputTypeDef = TypedDict(
+    "_RequiredDestinationConfigOutputTypeDef",
+    {
+        "services": List[str],
+    },
+)
+_OptionalDestinationConfigOutputTypeDef = TypedDict(
+    "_OptionalDestinationConfigOutputTypeDef",
+    {
+        "thingName": str,
+    },
+    total=False,
+)
+
+class DestinationConfigOutputTypeDef(
+    _RequiredDestinationConfigOutputTypeDef, _OptionalDestinationConfigOutputTypeDef
+):
+    pass
+
 _RequiredDestinationConfigTypeDef = TypedDict(
     "_RequiredDestinationConfigTypeDef",
     {
-        "services": List[str],
+        "services": Sequence[str],
     },
 )
 _OptionalDestinationConfigTypeDef = TypedDict(
     "_OptionalDestinationConfigTypeDef",
     {
         "thingName": str,
     },
     total=False,
 )
 
-
 class DestinationConfigTypeDef(
     _RequiredDestinationConfigTypeDef, _OptionalDestinationConfigTypeDef
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
 ListTunnelsRequestRequestTypeDef = TypedDict(
@@ -138,14 +155,22 @@
         "description": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
     },
     total=False,
 )
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 TimeoutConfigTypeDef = TypedDict(
     "TimeoutConfigTypeDef",
     {
         "maxLifetimeTimeoutMinutes": int,
     },
     total=False,
 )
@@ -178,14 +203,22 @@
         "tunnelArn": str,
         "sourceAccessToken": str,
         "destinationAccessToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TimeoutConfigOutputTypeDef = TypedDict(
+    "TimeoutConfigOutputTypeDef",
+    {
+        "maxLifetimeTimeoutMinutes": int,
+    },
+    total=False,
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -201,47 +234,45 @@
     "_OptionalRotateTunnelAccessTokenRequestRequestTypeDef",
     {
         "destinationConfig": DestinationConfigTypeDef,
     },
     total=False,
 )
 
-
 class RotateTunnelAccessTokenRequestRequestTypeDef(
     _RequiredRotateTunnelAccessTokenRequestRequestTypeDef,
     _OptionalRotateTunnelAccessTokenRequestRequestTypeDef,
 ):
     pass
 
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
-    },
-)
-
 ListTunnelsResponseTypeDef = TypedDict(
     "ListTunnelsResponseTypeDef",
     {
         "tunnelSummaries": List[TunnelSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
+    },
+)
+
 OpenTunnelRequestRequestTypeDef = TypedDict(
     "OpenTunnelRequestRequestTypeDef",
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
         "destinationConfig": DestinationConfigTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
@@ -254,17 +285,17 @@
     {
         "tunnelId": str,
         "tunnelArn": str,
         "status": TunnelStatusType,
         "sourceConnectionState": ConnectionStateTypeDef,
         "destinationConnectionState": ConnectionStateTypeDef,
         "description": str,
-        "destinationConfig": DestinationConfigTypeDef,
-        "timeoutConfig": TimeoutConfigTypeDef,
-        "tags": List[TagTypeDef],
+        "destinationConfig": DestinationConfigOutputTypeDef,
+        "timeoutConfig": TimeoutConfigOutputTypeDef,
+        "tags": List[TagOutputTypeDef],
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
     },
     total=False,
 )
 
 DescribeTunnelResponseTypeDef = TypedDict(
```

### Comparing `mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling/type_defs.pyi` & `mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,32 +18,36 @@
 from .literals import ClientModeType, ConnectionStatusType, TunnelStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CloseTunnelRequestRequestTypeDef",
     "ConnectionStateTypeDef",
     "DescribeTunnelRequestRequestTypeDef",
+    "DestinationConfigOutputTypeDef",
     "DestinationConfigTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "ListTunnelsRequestRequestTypeDef",
     "TunnelSummaryTypeDef",
+    "TagTypeDef",
     "TimeoutConfigTypeDef",
     "OpenTunnelResponseTypeDef",
     "ResponseMetadataTypeDef",
     "RotateTunnelAccessTokenResponseTypeDef",
+    "TimeoutConfigOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "RotateTunnelAccessTokenRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "ListTunnelsResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "OpenTunnelRequestRequestTypeDef",
     "TunnelTypeDef",
     "DescribeTunnelResponseTypeDef",
 )
 
 _RequiredCloseTunnelRequestRequestTypeDef = TypedDict(
     "_RequiredCloseTunnelRequestRequestTypeDef",
@@ -55,19 +59,21 @@
     "_OptionalCloseTunnelRequestRequestTypeDef",
     {
         "delete": bool,
     },
     total=False,
 )
 
+
 class CloseTunnelRequestRequestTypeDef(
     _RequiredCloseTunnelRequestRequestTypeDef, _OptionalCloseTunnelRequestRequestTypeDef
 ):
     pass
 
+
 ConnectionStateTypeDef = TypedDict(
     "ConnectionStateTypeDef",
     {
         "status": ConnectionStatusType,
         "lastUpdatedAt": datetime,
     },
     total=False,
@@ -76,42 +82,65 @@
 DescribeTunnelRequestRequestTypeDef = TypedDict(
     "DescribeTunnelRequestRequestTypeDef",
     {
         "tunnelId": str,
     },
 )
 
+_RequiredDestinationConfigOutputTypeDef = TypedDict(
+    "_RequiredDestinationConfigOutputTypeDef",
+    {
+        "services": List[str],
+    },
+)
+_OptionalDestinationConfigOutputTypeDef = TypedDict(
+    "_OptionalDestinationConfigOutputTypeDef",
+    {
+        "thingName": str,
+    },
+    total=False,
+)
+
+
+class DestinationConfigOutputTypeDef(
+    _RequiredDestinationConfigOutputTypeDef, _OptionalDestinationConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredDestinationConfigTypeDef = TypedDict(
     "_RequiredDestinationConfigTypeDef",
     {
-        "services": List[str],
+        "services": Sequence[str],
     },
 )
 _OptionalDestinationConfigTypeDef = TypedDict(
     "_OptionalDestinationConfigTypeDef",
     {
         "thingName": str,
     },
     total=False,
 )
 
+
 class DestinationConfigTypeDef(
     _RequiredDestinationConfigTypeDef, _OptionalDestinationConfigTypeDef
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
 ListTunnelsRequestRequestTypeDef = TypedDict(
@@ -133,14 +162,22 @@
         "description": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
     },
     total=False,
 )
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 TimeoutConfigTypeDef = TypedDict(
     "TimeoutConfigTypeDef",
     {
         "maxLifetimeTimeoutMinutes": int,
     },
     total=False,
 )
@@ -173,14 +210,22 @@
         "tunnelArn": str,
         "sourceAccessToken": str,
         "destinationAccessToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TimeoutConfigOutputTypeDef = TypedDict(
+    "TimeoutConfigOutputTypeDef",
+    {
+        "maxLifetimeTimeoutMinutes": int,
+    },
+    total=False,
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -196,45 +241,47 @@
     "_OptionalRotateTunnelAccessTokenRequestRequestTypeDef",
     {
         "destinationConfig": DestinationConfigTypeDef,
     },
     total=False,
 )
 
+
 class RotateTunnelAccessTokenRequestRequestTypeDef(
     _RequiredRotateTunnelAccessTokenRequestRequestTypeDef,
     _OptionalRotateTunnelAccessTokenRequestRequestTypeDef,
 ):
     pass
 
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
-    },
-)
-
 ListTunnelsResponseTypeDef = TypedDict(
     "ListTunnelsResponseTypeDef",
     {
         "tunnelSummaries": List[TunnelSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
+    },
+)
+
 OpenTunnelRequestRequestTypeDef = TypedDict(
     "OpenTunnelRequestRequestTypeDef",
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
         "destinationConfig": DestinationConfigTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
@@ -247,17 +294,17 @@
     {
         "tunnelId": str,
         "tunnelArn": str,
         "status": TunnelStatusType,
         "sourceConnectionState": ConnectionStateTypeDef,
         "destinationConnectionState": ConnectionStateTypeDef,
         "description": str,
-        "destinationConfig": DestinationConfigTypeDef,
-        "timeoutConfig": TimeoutConfigTypeDef,
-        "tags": List[TagTypeDef],
+        "destinationConfig": DestinationConfigOutputTypeDef,
+        "timeoutConfig": TimeoutConfigOutputTypeDef,
+        "tags": List[TagOutputTypeDef],
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
     },
     total=False,
 )
 
 DescribeTunnelResponseTypeDef = TypedDict(
```

### Comparing `mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling.egg-info/PKG-INFO` & `mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotsecuretunneling
-Version: 1.28.0
-Summary: Type annotations for boto3.IoTSecureTunneling 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTSecureTunneling 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iotsecuretunneling"></a>
 
 # mypy-boto3-iotsecuretunneling
 
 [![PyPI - mypy-boto3-iotsecuretunneling](https://img.shields.io/pypi/v/mypy-boto3-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsecuretunneling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsecuretunneling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotsecuretunneling?color=blue)](https://pypistats.org/packages/mypy-boto3-iotsecuretunneling)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotsecuretunneling)](https://pepy.tech/project/mypy-boto3-iotsecuretunneling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSecureTunneling 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
+[boto3.IoTSecureTunneling 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
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
 [mypy-boto3-iotsecuretunneling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,28 +303,31 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotsecuretunneling.type_defs import (
     CloseTunnelRequestRequestTypeDef,
     ConnectionStateTypeDef,
     DescribeTunnelRequestRequestTypeDef,
+    DestinationConfigOutputTypeDef,
     DestinationConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     ListTunnelsRequestRequestTypeDef,
     TunnelSummaryTypeDef,
+    TagTypeDef,
     TimeoutConfigTypeDef,
     OpenTunnelResponseTypeDef,
     ResponseMetadataTypeDef,
     RotateTunnelAccessTokenResponseTypeDef,
+    TimeoutConfigOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     RotateTunnelAccessTokenRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     ListTunnelsResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     OpenTunnelRequestRequestTypeDef,
     TunnelTypeDef,
     DescribeTunnelResponseTypeDef,
 )
 
 
 def get_structure() -> CloseTunnelRequestRequestTypeDef:
```

### Comparing `mypy-boto3-iotsecuretunneling-1.28.0/mypy_boto3_iotsecuretunneling.egg-info/SOURCES.txt` & `mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsecuretunneling-1.28.0/setup.py` & `mypy-boto3-iotsecuretunneling-1.28.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotsecuretunneling",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_iotsecuretunneling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTSecureTunneling 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.IoTSecureTunneling 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

