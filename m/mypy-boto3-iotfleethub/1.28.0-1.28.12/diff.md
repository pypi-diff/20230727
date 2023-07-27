# Comparing `tmp/mypy-boto3-iotfleethub-1.28.0.tar.gz` & `tmp/mypy-boto3-iotfleethub-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotfleethub-1.28.0.tar", last modified: Thu Jul  6 20:59:48 2023, max compression
+gzip compressed data, was "mypy-boto3-iotfleethub-1.28.12.tar", last modified: Thu Jul 27 05:34:49 2023, max compression
```

## Comparing `mypy-boto3-iotfleethub-1.28.0.tar` & `mypy-boto3-iotfleethub-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:48.774331 mypy-boto3-iotfleethub-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:43:49.000000 mypy-boto3-iotfleethub-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13376 2023-07-06 20:59:48.774331 mypy-boto3-iotfleethub-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-06 20:43:49.000000 mypy-boto3-iotfleethub-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:48.754331 mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-06 20:43:50.000000 mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-06 20:43:49.000000 mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-06 20:43:50.000000 mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-06 20:43:50.000000 mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-07-06 20:43:50.000000 mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-07-06 20:43:50.000000 mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-06 20:43:50.000000 mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-06 20:43:50.000000 mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-06 20:43:50.000000 mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:43:50.000000 mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-07-06 20:43:50.000000 mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-06 20:43:50.000000 mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:43:49.000000 mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:48.774331 mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13376 2023-07-06 20:59:48.000000 mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-06 20:59:48.000000 mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:48.000000 mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:48.000000 mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:48.000000 mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 20:59:48.000000 mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:48.774331 mypy-boto3-iotfleethub-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-06 20:43:49.000000 mypy-boto3-iotfleethub-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.756482 mypy-boto3-iotfleethub-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13363 2023-07-27 05:34:49.756482 mypy-boto3-iotfleethub-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.756482 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-07-27 05:24:05.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-07-27 05:24:05.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-27 05:24:05.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.756482 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13363 2023-07-27 05:34:49.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-27 05:34:49.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:49.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:49.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:49.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 05:34:49.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:49.756482 mypy-boto3-iotfleethub-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/setup.py
```

### Comparing `mypy-boto3-iotfleethub-1.28.0/LICENSE` & `mypy-boto3-iotfleethub-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleethub-1.28.0/PKG-INFO` & `mypy-boto3-iotfleethub-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotfleethub
-Version: 1.28.0
-Summary: Type annotations for boto3.IoTFleetHub 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTFleetHub 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iotfleethub"></a>
 
 # mypy-boto3-iotfleethub
 
 [![PyPI - mypy-boto3-iotfleethub](https://img.shields.io/pypi/v/mypy-boto3-iotfleethub.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleethub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleethub.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleethub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotfleethub?color=blue)](https://pypistats.org/packages/mypy-boto3-iotfleethub)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotfleethub)](https://pepy.tech/project/mypy-boto3-iotfleethub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetHub 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
+[boto3.IoTFleetHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
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
 [mypy-boto3-iotfleethub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotfleethub-1.28.0/README.md` & `mypy-boto3-iotfleethub-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iotfleethub"></a>
 
 # mypy-boto3-iotfleethub
 
 [![PyPI - mypy-boto3-iotfleethub](https://img.shields.io/pypi/v/mypy-boto3-iotfleethub.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleethub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleethub.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleethub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotfleethub?color=blue)](https://pypistats.org/packages/mypy-boto3-iotfleethub)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotfleethub)](https://pepy.tech/project/mypy-boto3-iotfleethub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetHub 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
+[boto3.IoTFleetHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
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
 [mypy-boto3-iotfleethub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/__init__.py` & `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/__init__.pyi` & `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/__main__.py` & `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTFleetHub 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.IoTFleetHub 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub\nOther"
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

### Comparing `mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/client.py` & `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/client.pyi` & `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/literals.py` & `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/literals.py`

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

### Comparing `mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/literals.pyi` & `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/literals.pyi`

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

### Comparing `mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/paginator.py` & `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/paginator.pyi` & `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/type_defs.py` & `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub/type_defs.pyi` & `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub.egg-info/PKG-INFO` & `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotfleethub
-Version: 1.28.0
-Summary: Type annotations for boto3.IoTFleetHub 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTFleetHub 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iotfleethub"></a>
 
 # mypy-boto3-iotfleethub
 
 [![PyPI - mypy-boto3-iotfleethub](https://img.shields.io/pypi/v/mypy-boto3-iotfleethub.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleethub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleethub.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleethub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotfleethub?color=blue)](https://pypistats.org/packages/mypy-boto3-iotfleethub)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotfleethub)](https://pepy.tech/project/mypy-boto3-iotfleethub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetHub 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
+[boto3.IoTFleetHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
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
 [mypy-boto3-iotfleethub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotfleethub-1.28.0/mypy_boto3_iotfleethub.egg-info/SOURCES.txt` & `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleethub-1.28.0/setup.py` & `mypy-boto3-iotfleethub-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotfleethub",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_iotfleethub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTFleetHub 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.IoTFleetHub 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

