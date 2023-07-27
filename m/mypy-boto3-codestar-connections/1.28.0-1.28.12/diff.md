# Comparing `tmp/mypy-boto3-codestar-connections-1.28.0.tar.gz` & `tmp/mypy-boto3-codestar-connections-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codestar-connections-1.28.0.tar", last modified: Thu Jul  6 20:59:15 2023, max compression
+gzip compressed data, was "mypy-boto3-codestar-connections-1.28.12.tar", last modified: Thu Jul 27 05:34:29 2023, max compression
```

## Comparing `mypy-boto3-codestar-connections-1.28.0.tar` & `mypy-boto3-codestar-connections-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:15.930259 mypy-boto3-codestar-connections-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:36:16.000000 mypy-boto3-codestar-connections-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-06 20:59:15.926259 mypy-boto3-codestar-connections-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-07-06 20:36:16.000000 mypy-boto3-codestar-connections-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:15.918259 mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-06 20:36:16.000000 mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-06 20:36:16.000000 mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-06 20:36:16.000000 mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-07-06 20:36:16.000000 mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-07-06 20:36:16.000000 mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-07-06 20:36:17.000000 mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-07-06 20:36:16.000000 mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:36:16.000000 mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-06 20:36:17.000000 mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-07-06 20:36:17.000000 mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:36:16.000000 mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:15.926259 mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-06 20:59:15.000000 mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-06 20:59:15.000000 mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:15.000000 mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:15.000000 mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:15.000000 mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 20:59:15.000000 mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:15.930259 mypy-boto3-codestar-connections-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-06 20:36:16.000000 mypy-boto3-codestar-connections-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.256549 mypy-boto3-codestar-connections-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13322 2023-07-27 05:34:29.252550 mypy-boto3-codestar-connections-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.244550 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-07-27 05:19:15.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.252550 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13322 2023-07-27 05:34:29.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-27 05:34:29.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:29.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:29.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:29.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 05:34:29.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:29.256549 mypy-boto3-codestar-connections-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/setup.py
```

### Comparing `mypy-boto3-codestar-connections-1.28.0/LICENSE` & `mypy-boto3-codestar-connections-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-connections-1.28.0/PKG-INFO` & `mypy-boto3-codestar-connections-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codestar-connections
-Version: 1.28.0
-Summary: Type annotations for boto3.CodeStarconnections 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CodeStarconnections 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codestar-connections"></a>
 
 # mypy-boto3-codestar-connections
 
 [![PyPI - mypy-boto3-codestar-connections](https://img.shields.io/pypi/v/mypy-boto3-codestar-connections.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar-connections)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codestar-connections.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar-connections)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codestar-connections?color=blue)](https://pypistats.org/packages/mypy-boto3-codestar-connections)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codestar-connections)](https://pepy.tech/project/mypy-boto3-codestar-connections)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeStarconnections 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
+[boto3.CodeStarconnections 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
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
 [mypy-boto3-codestar-connections docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,35 +301,37 @@
 `mypy_boto3_codestar_connections.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codestar_connections.type_defs import (
     ConnectionTypeDef,
     TagTypeDef,
+    TagOutputTypeDef,
     VpcConfigurationTypeDef,
     DeleteConnectionInputRequestTypeDef,
     DeleteHostInputRequestTypeDef,
     GetConnectionInputRequestTypeDef,
     GetHostInputRequestTypeDef,
+    VpcConfigurationOutputTypeDef,
     ListConnectionsInputRequestTypeDef,
     ListHostsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceInputRequestTypeDef,
     GetConnectionOutputTypeDef,
     ListConnectionsOutputTypeDef,
     CreateConnectionInputRequestTypeDef,
+    TagResourceInputRequestTypeDef,
     CreateConnectionOutputTypeDef,
     CreateHostOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    TagResourceInputRequestTypeDef,
     CreateHostInputRequestTypeDef,
+    UpdateHostInputRequestTypeDef,
     GetHostOutputTypeDef,
     HostTypeDef,
-    UpdateHostInputRequestTypeDef,
     ListHostsOutputTypeDef,
 )
 
 
 def get_structure() -> ConnectionTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-codestar-connections-1.28.0/README.md` & `mypy-boto3-codestar-connections-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codestar-connections"></a>
 
 # mypy-boto3-codestar-connections
 
 [![PyPI - mypy-boto3-codestar-connections](https://img.shields.io/pypi/v/mypy-boto3-codestar-connections.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar-connections)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codestar-connections.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar-connections)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codestar-connections?color=blue)](https://pypistats.org/packages/mypy-boto3-codestar-connections)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codestar-connections)](https://pepy.tech/project/mypy-boto3-codestar-connections)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeStarconnections 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
+[boto3.CodeStarconnections 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
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
 [mypy-boto3-codestar-connections docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/).
 
 See how it helps to find and fix potential bugs:
 
@@ -269,35 +269,37 @@
 `mypy_boto3_codestar_connections.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codestar_connections.type_defs import (
     ConnectionTypeDef,
     TagTypeDef,
+    TagOutputTypeDef,
     VpcConfigurationTypeDef,
     DeleteConnectionInputRequestTypeDef,
     DeleteHostInputRequestTypeDef,
     GetConnectionInputRequestTypeDef,
     GetHostInputRequestTypeDef,
+    VpcConfigurationOutputTypeDef,
     ListConnectionsInputRequestTypeDef,
     ListHostsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceInputRequestTypeDef,
     GetConnectionOutputTypeDef,
     ListConnectionsOutputTypeDef,
     CreateConnectionInputRequestTypeDef,
+    TagResourceInputRequestTypeDef,
     CreateConnectionOutputTypeDef,
     CreateHostOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    TagResourceInputRequestTypeDef,
     CreateHostInputRequestTypeDef,
+    UpdateHostInputRequestTypeDef,
     GetHostOutputTypeDef,
     HostTypeDef,
-    UpdateHostInputRequestTypeDef,
     ListHostsOutputTypeDef,
 )
 
 
 def get_structure() -> ConnectionTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections/__main__.py` & `mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeStarconnections 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.CodeStarconnections 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections\nOther"
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

### Comparing `mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections/client.py` & `mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections/client.pyi` & `mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections/literals.py` & `mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/literals.py`

 * *Files 2% similar despite different names*

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

### Comparing `mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections/literals.pyi` & `mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,15 @@
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
@@ -231,26 +232,28 @@
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

### Comparing `mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections/type_defs.py` & `mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,35 +21,37 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ConnectionTypeDef",
     "TagTypeDef",
+    "TagOutputTypeDef",
     "VpcConfigurationTypeDef",
     "DeleteConnectionInputRequestTypeDef",
     "DeleteHostInputRequestTypeDef",
     "GetConnectionInputRequestTypeDef",
     "GetHostInputRequestTypeDef",
+    "VpcConfigurationOutputTypeDef",
     "ListConnectionsInputRequestTypeDef",
     "ListHostsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "UntagResourceInputRequestTypeDef",
     "GetConnectionOutputTypeDef",
     "ListConnectionsOutputTypeDef",
     "CreateConnectionInputRequestTypeDef",
+    "TagResourceInputRequestTypeDef",
     "CreateConnectionOutputTypeDef",
     "CreateHostOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "TagResourceInputRequestTypeDef",
     "CreateHostInputRequestTypeDef",
+    "UpdateHostInputRequestTypeDef",
     "GetHostOutputTypeDef",
     "HostTypeDef",
-    "UpdateHostInputRequestTypeDef",
     "ListHostsOutputTypeDef",
 )
 
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "ConnectionName": str,
@@ -66,14 +68,22 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
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
 _RequiredVpcConfigurationTypeDef = TypedDict(
     "_RequiredVpcConfigurationTypeDef",
     {
         "VpcId": str,
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
@@ -115,14 +125,37 @@
 GetHostInputRequestTypeDef = TypedDict(
     "GetHostInputRequestTypeDef",
     {
         "HostArn": str,
     },
 )
 
+_RequiredVpcConfigurationOutputTypeDef = TypedDict(
+    "_RequiredVpcConfigurationOutputTypeDef",
+    {
+        "VpcId": str,
+        "SubnetIds": List[str],
+        "SecurityGroupIds": List[str],
+    },
+)
+_OptionalVpcConfigurationOutputTypeDef = TypedDict(
+    "_OptionalVpcConfigurationOutputTypeDef",
+    {
+        "TlsCertificate": str,
+    },
+    total=False,
+)
+
+
+class VpcConfigurationOutputTypeDef(
+    _RequiredVpcConfigurationOutputTypeDef, _OptionalVpcConfigurationOutputTypeDef
+):
+    pass
+
+
 ListConnectionsInputRequestTypeDef = TypedDict(
     "ListConnectionsInputRequestTypeDef",
     {
         "ProviderTypeFilter": ProviderTypeType,
         "HostArnFilter": str,
         "MaxResults": int,
         "NextToken": str,
@@ -201,48 +234,48 @@
 
 class CreateConnectionInputRequestTypeDef(
     _RequiredCreateConnectionInputRequestTypeDef, _OptionalCreateConnectionInputRequestTypeDef
 ):
     pass
 
 
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
 CreateConnectionOutputTypeDef = TypedDict(
     "CreateConnectionOutputTypeDef",
     {
         "ConnectionArn": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateHostOutputTypeDef = TypedDict(
     "CreateHostOutputTypeDef",
     {
         "HostArn": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
 _RequiredCreateHostInputRequestTypeDef = TypedDict(
     "_RequiredCreateHostInputRequestTypeDef",
     {
         "Name": str,
         "ProviderType": ProviderTypeType,
         "ProviderEndpoint": str,
     },
@@ -259,62 +292,62 @@
 
 class CreateHostInputRequestTypeDef(
     _RequiredCreateHostInputRequestTypeDef, _OptionalCreateHostInputRequestTypeDef
 ):
     pass
 
 
+_RequiredUpdateHostInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateHostInputRequestTypeDef",
+    {
+        "HostArn": str,
+    },
+)
+_OptionalUpdateHostInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateHostInputRequestTypeDef",
+    {
+        "ProviderEndpoint": str,
+        "VpcConfiguration": VpcConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateHostInputRequestTypeDef(
+    _RequiredUpdateHostInputRequestTypeDef, _OptionalUpdateHostInputRequestTypeDef
+):
+    pass
+
+
 GetHostOutputTypeDef = TypedDict(
     "GetHostOutputTypeDef",
     {
         "Name": str,
         "Status": str,
         "ProviderType": ProviderTypeType,
         "ProviderEndpoint": str,
-        "VpcConfiguration": VpcConfigurationTypeDef,
+        "VpcConfiguration": VpcConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HostTypeDef = TypedDict(
     "HostTypeDef",
     {
         "Name": str,
         "HostArn": str,
         "ProviderType": ProviderTypeType,
         "ProviderEndpoint": str,
-        "VpcConfiguration": VpcConfigurationTypeDef,
+        "VpcConfiguration": VpcConfigurationOutputTypeDef,
         "Status": str,
         "StatusMessage": str,
     },
     total=False,
 )
 
-_RequiredUpdateHostInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateHostInputRequestTypeDef",
-    {
-        "HostArn": str,
-    },
-)
-_OptionalUpdateHostInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateHostInputRequestTypeDef",
-    {
-        "ProviderEndpoint": str,
-        "VpcConfiguration": VpcConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateHostInputRequestTypeDef(
-    _RequiredUpdateHostInputRequestTypeDef, _OptionalUpdateHostInputRequestTypeDef
-):
-    pass
-
-
 ListHostsOutputTypeDef = TypedDict(
     "ListHostsOutputTypeDef",
     {
         "Hosts": List[HostTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections/type_defs.pyi` & `mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -20,35 +20,37 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ConnectionTypeDef",
     "TagTypeDef",
+    "TagOutputTypeDef",
     "VpcConfigurationTypeDef",
     "DeleteConnectionInputRequestTypeDef",
     "DeleteHostInputRequestTypeDef",
     "GetConnectionInputRequestTypeDef",
     "GetHostInputRequestTypeDef",
+    "VpcConfigurationOutputTypeDef",
     "ListConnectionsInputRequestTypeDef",
     "ListHostsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "UntagResourceInputRequestTypeDef",
     "GetConnectionOutputTypeDef",
     "ListConnectionsOutputTypeDef",
     "CreateConnectionInputRequestTypeDef",
+    "TagResourceInputRequestTypeDef",
     "CreateConnectionOutputTypeDef",
     "CreateHostOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "TagResourceInputRequestTypeDef",
     "CreateHostInputRequestTypeDef",
+    "UpdateHostInputRequestTypeDef",
     "GetHostOutputTypeDef",
     "HostTypeDef",
-    "UpdateHostInputRequestTypeDef",
     "ListHostsOutputTypeDef",
 )
 
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "ConnectionName": str,
@@ -65,14 +67,22 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
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
 _RequiredVpcConfigurationTypeDef = TypedDict(
     "_RequiredVpcConfigurationTypeDef",
     {
         "VpcId": str,
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
@@ -112,14 +122,35 @@
 GetHostInputRequestTypeDef = TypedDict(
     "GetHostInputRequestTypeDef",
     {
         "HostArn": str,
     },
 )
 
+_RequiredVpcConfigurationOutputTypeDef = TypedDict(
+    "_RequiredVpcConfigurationOutputTypeDef",
+    {
+        "VpcId": str,
+        "SubnetIds": List[str],
+        "SecurityGroupIds": List[str],
+    },
+)
+_OptionalVpcConfigurationOutputTypeDef = TypedDict(
+    "_OptionalVpcConfigurationOutputTypeDef",
+    {
+        "TlsCertificate": str,
+    },
+    total=False,
+)
+
+class VpcConfigurationOutputTypeDef(
+    _RequiredVpcConfigurationOutputTypeDef, _OptionalVpcConfigurationOutputTypeDef
+):
+    pass
+
 ListConnectionsInputRequestTypeDef = TypedDict(
     "ListConnectionsInputRequestTypeDef",
     {
         "ProviderTypeFilter": ProviderTypeType,
         "HostArnFilter": str,
         "MaxResults": int,
         "NextToken": str,
@@ -196,48 +227,48 @@
 )
 
 class CreateConnectionInputRequestTypeDef(
     _RequiredCreateConnectionInputRequestTypeDef, _OptionalCreateConnectionInputRequestTypeDef
 ):
     pass
 
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
 CreateConnectionOutputTypeDef = TypedDict(
     "CreateConnectionOutputTypeDef",
     {
         "ConnectionArn": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateHostOutputTypeDef = TypedDict(
     "CreateHostOutputTypeDef",
     {
         "HostArn": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
 _RequiredCreateHostInputRequestTypeDef = TypedDict(
     "_RequiredCreateHostInputRequestTypeDef",
     {
         "Name": str,
         "ProviderType": ProviderTypeType,
         "ProviderEndpoint": str,
     },
@@ -252,60 +283,60 @@
 )
 
 class CreateHostInputRequestTypeDef(
     _RequiredCreateHostInputRequestTypeDef, _OptionalCreateHostInputRequestTypeDef
 ):
     pass
 
+_RequiredUpdateHostInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateHostInputRequestTypeDef",
+    {
+        "HostArn": str,
+    },
+)
+_OptionalUpdateHostInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateHostInputRequestTypeDef",
+    {
+        "ProviderEndpoint": str,
+        "VpcConfiguration": VpcConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class UpdateHostInputRequestTypeDef(
+    _RequiredUpdateHostInputRequestTypeDef, _OptionalUpdateHostInputRequestTypeDef
+):
+    pass
+
 GetHostOutputTypeDef = TypedDict(
     "GetHostOutputTypeDef",
     {
         "Name": str,
         "Status": str,
         "ProviderType": ProviderTypeType,
         "ProviderEndpoint": str,
-        "VpcConfiguration": VpcConfigurationTypeDef,
+        "VpcConfiguration": VpcConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HostTypeDef = TypedDict(
     "HostTypeDef",
     {
         "Name": str,
         "HostArn": str,
         "ProviderType": ProviderTypeType,
         "ProviderEndpoint": str,
-        "VpcConfiguration": VpcConfigurationTypeDef,
+        "VpcConfiguration": VpcConfigurationOutputTypeDef,
         "Status": str,
         "StatusMessage": str,
     },
     total=False,
 )
 
-_RequiredUpdateHostInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateHostInputRequestTypeDef",
-    {
-        "HostArn": str,
-    },
-)
-_OptionalUpdateHostInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateHostInputRequestTypeDef",
-    {
-        "ProviderEndpoint": str,
-        "VpcConfiguration": VpcConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class UpdateHostInputRequestTypeDef(
-    _RequiredUpdateHostInputRequestTypeDef, _OptionalUpdateHostInputRequestTypeDef
-):
-    pass
-
 ListHostsOutputTypeDef = TypedDict(
     "ListHostsOutputTypeDef",
     {
         "Hosts": List[HostTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections.egg-info/PKG-INFO` & `mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codestar-connections
-Version: 1.28.0
-Summary: Type annotations for boto3.CodeStarconnections 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CodeStarconnections 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codestar-connections"></a>
 
 # mypy-boto3-codestar-connections
 
 [![PyPI - mypy-boto3-codestar-connections](https://img.shields.io/pypi/v/mypy-boto3-codestar-connections.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar-connections)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codestar-connections.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar-connections)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codestar-connections?color=blue)](https://pypistats.org/packages/mypy-boto3-codestar-connections)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codestar-connections)](https://pepy.tech/project/mypy-boto3-codestar-connections)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeStarconnections 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
+[boto3.CodeStarconnections 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
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
 [mypy-boto3-codestar-connections docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,35 +301,37 @@
 `mypy_boto3_codestar_connections.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codestar_connections.type_defs import (
     ConnectionTypeDef,
     TagTypeDef,
+    TagOutputTypeDef,
     VpcConfigurationTypeDef,
     DeleteConnectionInputRequestTypeDef,
     DeleteHostInputRequestTypeDef,
     GetConnectionInputRequestTypeDef,
     GetHostInputRequestTypeDef,
+    VpcConfigurationOutputTypeDef,
     ListConnectionsInputRequestTypeDef,
     ListHostsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceInputRequestTypeDef,
     GetConnectionOutputTypeDef,
     ListConnectionsOutputTypeDef,
     CreateConnectionInputRequestTypeDef,
+    TagResourceInputRequestTypeDef,
     CreateConnectionOutputTypeDef,
     CreateHostOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    TagResourceInputRequestTypeDef,
     CreateHostInputRequestTypeDef,
+    UpdateHostInputRequestTypeDef,
     GetHostOutputTypeDef,
     HostTypeDef,
-    UpdateHostInputRequestTypeDef,
     ListHostsOutputTypeDef,
 )
 
 
 def get_structure() -> ConnectionTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-codestar-connections-1.28.0/mypy_boto3_codestar_connections.egg-info/SOURCES.txt` & `mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-connections-1.28.0/setup.py` & `mypy-boto3-codestar-connections-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codestar-connections",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_codestar_connections"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeStarconnections 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.CodeStarconnections 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

