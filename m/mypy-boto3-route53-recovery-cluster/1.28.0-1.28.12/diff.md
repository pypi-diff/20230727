# Comparing `tmp/mypy-boto3-route53-recovery-cluster-1.28.0.tar.gz` & `tmp/mypy-boto3-route53-recovery-cluster-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53-recovery-cluster-1.28.0.tar", last modified: Thu Jul  6 21:00:28 2023, max compression
+gzip compressed data, was "mypy-boto3-route53-recovery-cluster-1.28.12.tar", last modified: Thu Jul 27 11:49:30 2023, max compression
```

## Comparing `mypy-boto3-route53-recovery-cluster-1.28.0.tar` & `mypy-boto3-route53-recovery-cluster-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:28.802413 mypy-boto3-route53-recovery-cluster-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:53:35.000000 mypy-boto3-route53-recovery-cluster-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-07-06 21:00:28.802413 mypy-boto3-route53-recovery-cluster-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-07-06 20:53:35.000000 mypy-boto3-route53-recovery-cluster-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:28.786413 mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-06 20:53:35.000000 mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-06 20:53:35.000000 mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-06 20:53:35.000000 mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-07-06 20:53:35.000000 mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-07-06 20:53:35.000000 mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-07-06 20:53:35.000000 mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-07-06 20:53:35.000000 mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-06 20:53:35.000000 mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-06 20:53:35.000000 mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:53:35.000000 mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-07-06 20:53:35.000000 mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-07-06 20:53:35.000000 mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:53:35.000000 mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:28.802413 mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-07-06 21:00:28.000000 mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-06 21:00:28.000000 mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:28.000000 mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:28.000000 mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:28.000000 mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 21:00:28.000000 mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:28.802413 mypy-boto3-route53-recovery-cluster-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-06 20:53:35.000000 mypy-boto3-route53-recovery-cluster-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.813218 mypy-boto3-route53-recovery-cluster-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-cluster-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-07-27 11:49:30.813218 mypy-boto3-route53-recovery-cluster-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-cluster-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.809218 mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.813218 mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-07-27 11:49:30.000000 mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-27 11:49:30.000000 mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:30.000000 mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-27 11:49:30.000000 mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:30.813218 mypy-boto3-route53-recovery-cluster-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-cluster-1.28.12/setup.py
```

### Comparing `mypy-boto3-route53-recovery-cluster-1.28.0/LICENSE` & `mypy-boto3-route53-recovery-cluster-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-cluster-1.28.0/PKG-INFO` & `mypy-boto3-route53-recovery-cluster-1.28.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53-recovery-cluster
-Version: 1.28.0
-Summary: Type annotations for boto3.Route53RecoveryCluster 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Route53RecoveryCluster 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-route53-recovery-cluster"></a>
 
 # mypy-boto3-route53-recovery-cluster
 
 [![PyPI - mypy-boto3-route53-recovery-cluster](https://img.shields.io/pypi/v/mypy-boto3-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-cluster)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-cluster)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53-recovery-cluster?color=blue)](https://pypistats.org/packages/mypy-boto3-route53-recovery-cluster)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53-recovery-cluster)](https://pepy.tech/project/mypy-boto3-route53-recovery-cluster)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryCluster 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
+[boto3.Route53RecoveryCluster 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
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
 [mypy-boto3-route53-recovery-cluster docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/).
 
 See how it helps to find and fix potential bugs:
 
@@ -323,22 +323,22 @@
 
 `mypy_boto3_route53_recovery_cluster.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53_recovery_cluster.type_defs import (
     GetRoutingControlStateRequestRequestTypeDef,
-    GetRoutingControlStateResponseTypeDef,
-    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
+    ResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
     ListRoutingControlsRequestRequestTypeDef,
     RoutingControlTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UpdateRoutingControlStateEntryTypeDef,
     UpdateRoutingControlStateRequestRequestTypeDef,
+    GetRoutingControlStateResponseTypeDef,
+    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
     ListRoutingControlsResponseTypeDef,
     UpdateRoutingControlStatesRequestRequestTypeDef,
 )
 
 
 def get_structure() -> GetRoutingControlStateRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-route53-recovery-cluster-1.28.0/README.md` & `mypy-boto3-route53-recovery-cluster-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-route53-recovery-cluster"></a>
 
 # mypy-boto3-route53-recovery-cluster
 
 [![PyPI - mypy-boto3-route53-recovery-cluster](https://img.shields.io/pypi/v/mypy-boto3-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-cluster)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-cluster)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53-recovery-cluster?color=blue)](https://pypistats.org/packages/mypy-boto3-route53-recovery-cluster)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53-recovery-cluster)](https://pepy.tech/project/mypy-boto3-route53-recovery-cluster)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryCluster 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
+[boto3.Route53RecoveryCluster 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
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
 [mypy-boto3-route53-recovery-cluster docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,22 +291,22 @@
 
 `mypy_boto3_route53_recovery_cluster.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53_recovery_cluster.type_defs import (
     GetRoutingControlStateRequestRequestTypeDef,
-    GetRoutingControlStateResponseTypeDef,
-    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
+    ResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
     ListRoutingControlsRequestRequestTypeDef,
     RoutingControlTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UpdateRoutingControlStateEntryTypeDef,
     UpdateRoutingControlStateRequestRequestTypeDef,
+    GetRoutingControlStateResponseTypeDef,
+    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
     ListRoutingControlsResponseTypeDef,
     UpdateRoutingControlStatesRequestRequestTypeDef,
 )
 
 
 def get_structure() -> GetRoutingControlStateRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/__init__.py` & `mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/__init__.pyi` & `mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/__main__.py` & `mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53RecoveryCluster 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.Route53RecoveryCluster 1.28.12\nVersion:        "
+        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster\nOther"
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

### Comparing `mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/client.py` & `mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/client.pyi` & `mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/literals.py` & `mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/literals.py`

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

### Comparing `mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/literals.pyi` & `mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/literals.pyi`

 * *Files 1% similar despite different names*

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

### Comparing `mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/paginator.py` & `mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListRoutingControlsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Paginator.ListRoutingControls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/paginators/#listroutingcontrolspaginator)
     """
 
     def paginate(
-        self, *, ControlPanelArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ControlPanelArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRoutingControlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Paginator.ListRoutingControls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/paginators/#listroutingcontrolspaginator)
         """
```

### Comparing `mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/paginator.pyi` & `mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListRoutingControlsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Paginator.ListRoutingControls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/paginators/#listroutingcontrolspaginator)
     """
 
     def paginate(
-        self, *, ControlPanelArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ControlPanelArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRoutingControlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Paginator.ListRoutingControls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/paginators/#listroutingcontrolspaginator)
         """
```

### Comparing `mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/type_defs.py` & `mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,48 +20,50 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "GetRoutingControlStateRequestRequestTypeDef",
-    "GetRoutingControlStateResponseTypeDef",
-    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+    "ResponseMetadataTypeDef",
+    "PaginatorConfigTypeDef",
     "ListRoutingControlsRequestRequestTypeDef",
     "RoutingControlTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateRoutingControlStateEntryTypeDef",
     "UpdateRoutingControlStateRequestRequestTypeDef",
+    "GetRoutingControlStateResponseTypeDef",
+    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
     "ListRoutingControlsResponseTypeDef",
     "UpdateRoutingControlStatesRequestRequestTypeDef",
 )
 
 GetRoutingControlStateRequestRequestTypeDef = TypedDict(
     "GetRoutingControlStateRequestRequestTypeDef",
     {
         "RoutingControlArn": str,
     },
 )
 
-GetRoutingControlStateResponseTypeDef = TypedDict(
-    "GetRoutingControlStateResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "RoutingControlArn": str,
-        "RoutingControlState": RoutingControlStateType,
-        "RoutingControlName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-ListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
-    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ControlPanelArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListRoutingControlsRequestRequestTypeDef = TypedDict(
     "ListRoutingControlsRequestRequestTypeDef",
     {
@@ -80,35 +82,14 @@
         "RoutingControlArn": str,
         "RoutingControlName": str,
         "RoutingControlState": RoutingControlStateType,
     },
     total=False,
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
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 UpdateRoutingControlStateEntryTypeDef = TypedDict(
     "UpdateRoutingControlStateEntryTypeDef",
     {
         "RoutingControlArn": str,
         "RoutingControlState": RoutingControlStateType,
     },
 )
@@ -132,20 +113,39 @@
 class UpdateRoutingControlStateRequestRequestTypeDef(
     _RequiredUpdateRoutingControlStateRequestRequestTypeDef,
     _OptionalUpdateRoutingControlStateRequestRequestTypeDef,
 ):
     pass
 
 
+GetRoutingControlStateResponseTypeDef = TypedDict(
+    "GetRoutingControlStateResponseTypeDef",
+    {
+        "RoutingControlArn": str,
+        "RoutingControlState": RoutingControlStateType,
+        "RoutingControlName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
+    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+    {
+        "ControlPanelArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListRoutingControlsResponseTypeDef = TypedDict(
     "ListRoutingControlsResponseTypeDef",
     {
         "RoutingControls": List[RoutingControlTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateRoutingControlStatesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRoutingControlStatesRequestRequestTypeDef",
     {
         "UpdateRoutingControlStateEntries": Sequence[UpdateRoutingControlStateEntryTypeDef],
```

### Comparing `mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster/type_defs.pyi` & `mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -19,48 +19,50 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "GetRoutingControlStateRequestRequestTypeDef",
-    "GetRoutingControlStateResponseTypeDef",
-    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+    "ResponseMetadataTypeDef",
+    "PaginatorConfigTypeDef",
     "ListRoutingControlsRequestRequestTypeDef",
     "RoutingControlTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateRoutingControlStateEntryTypeDef",
     "UpdateRoutingControlStateRequestRequestTypeDef",
+    "GetRoutingControlStateResponseTypeDef",
+    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
     "ListRoutingControlsResponseTypeDef",
     "UpdateRoutingControlStatesRequestRequestTypeDef",
 )
 
 GetRoutingControlStateRequestRequestTypeDef = TypedDict(
     "GetRoutingControlStateRequestRequestTypeDef",
     {
         "RoutingControlArn": str,
     },
 )
 
-GetRoutingControlStateResponseTypeDef = TypedDict(
-    "GetRoutingControlStateResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "RoutingControlArn": str,
-        "RoutingControlState": RoutingControlStateType,
-        "RoutingControlName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-ListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
-    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ControlPanelArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListRoutingControlsRequestRequestTypeDef = TypedDict(
     "ListRoutingControlsRequestRequestTypeDef",
     {
@@ -79,35 +81,14 @@
         "RoutingControlArn": str,
         "RoutingControlName": str,
         "RoutingControlState": RoutingControlStateType,
     },
     total=False,
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
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 UpdateRoutingControlStateEntryTypeDef = TypedDict(
     "UpdateRoutingControlStateEntryTypeDef",
     {
         "RoutingControlArn": str,
         "RoutingControlState": RoutingControlStateType,
     },
 )
@@ -129,20 +110,39 @@
 
 class UpdateRoutingControlStateRequestRequestTypeDef(
     _RequiredUpdateRoutingControlStateRequestRequestTypeDef,
     _OptionalUpdateRoutingControlStateRequestRequestTypeDef,
 ):
     pass
 
+GetRoutingControlStateResponseTypeDef = TypedDict(
+    "GetRoutingControlStateResponseTypeDef",
+    {
+        "RoutingControlArn": str,
+        "RoutingControlState": RoutingControlStateType,
+        "RoutingControlName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
+    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+    {
+        "ControlPanelArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListRoutingControlsResponseTypeDef = TypedDict(
     "ListRoutingControlsResponseTypeDef",
     {
         "RoutingControls": List[RoutingControlTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateRoutingControlStatesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRoutingControlStatesRequestRequestTypeDef",
     {
         "UpdateRoutingControlStateEntries": Sequence[UpdateRoutingControlStateEntryTypeDef],
```

### Comparing `mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster.egg-info/PKG-INFO` & `mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53-recovery-cluster
-Version: 1.28.0
-Summary: Type annotations for boto3.Route53RecoveryCluster 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Route53RecoveryCluster 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-route53-recovery-cluster"></a>
 
 # mypy-boto3-route53-recovery-cluster
 
 [![PyPI - mypy-boto3-route53-recovery-cluster](https://img.shields.io/pypi/v/mypy-boto3-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-cluster)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-cluster)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53-recovery-cluster?color=blue)](https://pypistats.org/packages/mypy-boto3-route53-recovery-cluster)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53-recovery-cluster)](https://pepy.tech/project/mypy-boto3-route53-recovery-cluster)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryCluster 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
+[boto3.Route53RecoveryCluster 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
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
 [mypy-boto3-route53-recovery-cluster docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/).
 
 See how it helps to find and fix potential bugs:
 
@@ -323,22 +323,22 @@
 
 `mypy_boto3_route53_recovery_cluster.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53_recovery_cluster.type_defs import (
     GetRoutingControlStateRequestRequestTypeDef,
-    GetRoutingControlStateResponseTypeDef,
-    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
+    ResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
     ListRoutingControlsRequestRequestTypeDef,
     RoutingControlTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UpdateRoutingControlStateEntryTypeDef,
     UpdateRoutingControlStateRequestRequestTypeDef,
+    GetRoutingControlStateResponseTypeDef,
+    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
     ListRoutingControlsResponseTypeDef,
     UpdateRoutingControlStatesRequestRequestTypeDef,
 )
 
 
 def get_structure() -> GetRoutingControlStateRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-route53-recovery-cluster-1.28.0/mypy_boto3_route53_recovery_cluster.egg-info/SOURCES.txt` & `mypy-boto3-route53-recovery-cluster-1.28.12/mypy_boto3_route53_recovery_cluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-cluster-1.28.0/setup.py` & `mypy-boto3-route53-recovery-cluster-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53-recovery-cluster",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_route53_recovery_cluster"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Route53RecoveryCluster 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Route53RecoveryCluster 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

