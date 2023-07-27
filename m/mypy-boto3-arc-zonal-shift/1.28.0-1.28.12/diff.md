# Comparing `tmp/mypy-boto3-arc-zonal-shift-1.28.0.tar.gz` & `tmp/mypy-boto3-arc-zonal-shift-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-arc-zonal-shift-1.28.0.tar", last modified: Thu Jul  6 20:59:02 2023, max compression
+gzip compressed data, was "mypy-boto3-arc-zonal-shift-1.28.12.tar", last modified: Thu Jul 27 05:34:20 2023, max compression
```

## Comparing `mypy-boto3-arc-zonal-shift-1.28.0.tar` & `mypy-boto3-arc-zonal-shift-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:02.026227 mypy-boto3-arc-zonal-shift-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:33:46.000000 mypy-boto3-arc-zonal-shift-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-07-06 20:59:02.026227 mypy-boto3-arc-zonal-shift-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12334 2023-07-06 20:33:46.000000 mypy-boto3-arc-zonal-shift-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:02.018227 mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-06 20:33:46.000000 mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-06 20:33:46.000000 mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 20:33:46.000000 mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-07-06 20:33:46.000000 mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-06 20:33:46.000000 mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-07-06 20:33:46.000000 mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-07-06 20:33:46.000000 mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-07-06 20:33:46.000000 mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-06 20:33:46.000000 mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:33:46.000000 mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-07-06 20:33:46.000000 mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-06 20:33:46.000000 mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:33:46.000000 mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:02.022227 mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-07-06 20:59:01.000000 mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-06 20:59:01.000000 mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:01.000000 mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:01.000000 mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:01.000000 mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 20:59:01.000000 mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:02.026227 mypy-boto3-arc-zonal-shift-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-06 20:33:45.000000 mypy-boto3-arc-zonal-shift-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.588572 mypy-boto3-arc-zonal-shift-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-27 05:34:20.584572 mypy-boto3-arc-zonal-shift-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.584572 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.584572 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-27 05:34:20.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-27 05:34:20.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:20.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 05:34:20.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:20.588572 mypy-boto3-arc-zonal-shift-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/setup.py
```

### Comparing `mypy-boto3-arc-zonal-shift-1.28.0/LICENSE` & `mypy-boto3-arc-zonal-shift-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.0/PKG-INFO` & `mypy-boto3-arc-zonal-shift-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-arc-zonal-shift
-Version: 1.28.0
-Summary: Type annotations for boto3.ARCZonalShift 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ARCZonalShift 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-arc-zonal-shift"></a>
 
 # mypy-boto3-arc-zonal-shift
 
 [![PyPI - mypy-boto3-arc-zonal-shift](https://img.shields.io/pypi/v/mypy-boto3-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/mypy-boto3-arc-zonal-shift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/mypy-boto3-arc-zonal-shift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-arc-zonal-shift?color=blue)](https://pypistats.org/packages/mypy-boto3-arc-zonal-shift)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-arc-zonal-shift)](https://pepy.tech/project/mypy-boto3-arc-zonal-shift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ARCZonalShift 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
+[boto3.ARCZonalShift 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
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
 [mypy-boto3-arc-zonal-shift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-arc-zonal-shift-1.28.0/README.md` & `mypy-boto3-arc-zonal-shift-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-arc-zonal-shift"></a>
 
 # mypy-boto3-arc-zonal-shift
 
 [![PyPI - mypy-boto3-arc-zonal-shift](https://img.shields.io/pypi/v/mypy-boto3-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/mypy-boto3-arc-zonal-shift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/mypy-boto3-arc-zonal-shift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-arc-zonal-shift?color=blue)](https://pypistats.org/packages/mypy-boto3-arc-zonal-shift)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-arc-zonal-shift)](https://pepy.tech/project/mypy-boto3-arc-zonal-shift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ARCZonalShift 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
+[boto3.ARCZonalShift 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
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
 [mypy-boto3-arc-zonal-shift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/__init__.py` & `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/__init__.pyi` & `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/__main__.py` & `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ARCZonalShift 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.ARCZonalShift 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift\nOther"
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

### Comparing `mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/client.py` & `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/client.pyi` & `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/literals.py` & `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/literals.py`

 * *Files 0% similar despite different names*

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

### Comparing `mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/literals.pyi` & `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/literals.pyi`

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

### Comparing `mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/paginator.py` & `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/paginator.pyi` & `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/type_defs.py` & `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift/type_defs.pyi` & `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift.egg-info/PKG-INFO` & `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-arc-zonal-shift
-Version: 1.28.0
-Summary: Type annotations for boto3.ARCZonalShift 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ARCZonalShift 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-arc-zonal-shift"></a>
 
 # mypy-boto3-arc-zonal-shift
 
 [![PyPI - mypy-boto3-arc-zonal-shift](https://img.shields.io/pypi/v/mypy-boto3-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/mypy-boto3-arc-zonal-shift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/mypy-boto3-arc-zonal-shift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-arc-zonal-shift?color=blue)](https://pypistats.org/packages/mypy-boto3-arc-zonal-shift)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-arc-zonal-shift)](https://pepy.tech/project/mypy-boto3-arc-zonal-shift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ARCZonalShift 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
+[boto3.ARCZonalShift 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
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
 [mypy-boto3-arc-zonal-shift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-arc-zonal-shift-1.28.0/mypy_boto3_arc_zonal_shift.egg-info/SOURCES.txt` & `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.0/setup.py` & `mypy-boto3-arc-zonal-shift-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-arc-zonal-shift",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_arc_zonal_shift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ARCZonalShift 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.ARCZonalShift 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

