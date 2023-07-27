# Comparing `tmp/mypy-boto3-mediastore-data-1.28.0.tar.gz` & `tmp/mypy-boto3-mediastore-data-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediastore-data-1.28.0.tar", last modified: Thu Jul  6 21:00:07 2023, max compression
+gzip compressed data, was "mypy-boto3-mediastore-data-1.28.12.tar", last modified: Thu Jul 27 05:35:01 2023, max compression
```

## Comparing `mypy-boto3-mediastore-data-1.28.0.tar` & `mypy-boto3-mediastore-data-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:07.662370 mypy-boto3-mediastore-data-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:47:23.000000 mypy-boto3-mediastore-data-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13387 2023-07-06 21:00:07.662370 mypy-boto3-mediastore-data-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-07-06 20:47:23.000000 mypy-boto3-mediastore-data-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:07.650370 mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-06 20:47:23.000000 mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-06 20:47:23.000000 mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-06 20:47:23.000000 mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-07-06 20:47:23.000000 mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-06 20:47:23.000000 mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-06 20:47:24.000000 mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-06 20:47:24.000000 mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-06 20:47:23.000000 mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-06 20:47:23.000000 mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:47:23.000000 mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-06 20:47:24.000000 mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-07-06 20:47:24.000000 mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:47:23.000000 mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:07.662370 mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13387 2023-07-06 21:00:07.000000 mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-06 21:00:07.000000 mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:07.000000 mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:07.000000 mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:07.000000 mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 21:00:07.000000 mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:07.662370 mypy-boto3-mediastore-data-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-06 20:47:23.000000 mypy-boto3-mediastore-data-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:01.800438 mypy-boto3-mediastore-data-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-data-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-07-27 05:35:01.792438 mypy-boto3-mediastore-data-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-data-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:01.792438 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-07-27 05:26:26.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-27 05:26:26.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-07-27 05:26:26.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-07-27 05:26:26.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-27 05:26:26.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-27 05:26:26.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-27 05:26:26.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-07-27 05:26:26.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:01.792438 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:01.800438 mypy-boto3-mediastore-data-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-data-1.28.12/setup.py
```

### Comparing `mypy-boto3-mediastore-data-1.28.0/LICENSE` & `mypy-boto3-mediastore-data-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.0/PKG-INFO` & `mypy-boto3-mediastore-data-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediastore-data
-Version: 1.28.0
-Summary: Type annotations for boto3.MediaStoreData 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MediaStoreData 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mediastore-data"></a>
 
 # mypy-boto3-mediastore-data
 
 [![PyPI - mypy-boto3-mediastore-data](https://img.shields.io/pypi/v/mypy-boto3-mediastore-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediastore-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediastore-data?color=blue)](https://pypistats.org/packages/mypy-boto3-mediastore-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediastore-data)](https://pepy.tech/project/mypy-boto3-mediastore-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaStoreData 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
+[boto3.MediaStoreData 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
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
 [mypy-boto3-mediastore-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mediastore-data-1.28.0/README.md` & `mypy-boto3-mediastore-data-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-mediastore-data"></a>
 
 # mypy-boto3-mediastore-data
 
 [![PyPI - mypy-boto3-mediastore-data](https://img.shields.io/pypi/v/mypy-boto3-mediastore-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediastore-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediastore-data?color=blue)](https://pypistats.org/packages/mypy-boto3-mediastore-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediastore-data)](https://pepy.tech/project/mypy-boto3-mediastore-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaStoreData 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
+[boto3.MediaStoreData 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
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
 [mypy-boto3-mediastore-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/__init__.py` & `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/__init__.pyi` & `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/__main__.py` & `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaStoreData 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.MediaStoreData 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData\nOther"
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

### Comparing `mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/client.py` & `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/client.pyi` & `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/literals.py` & `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/literals.py`

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

### Comparing `mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/literals.pyi` & `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/literals.pyi`

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

### Comparing `mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/paginator.py` & `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/paginator.pyi` & `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/type_defs.py` & `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data/type_defs.pyi` & `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data.egg-info/PKG-INFO` & `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediastore-data
-Version: 1.28.0
-Summary: Type annotations for boto3.MediaStoreData 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MediaStoreData 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mediastore-data"></a>
 
 # mypy-boto3-mediastore-data
 
 [![PyPI - mypy-boto3-mediastore-data](https://img.shields.io/pypi/v/mypy-boto3-mediastore-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediastore-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediastore-data?color=blue)](https://pypistats.org/packages/mypy-boto3-mediastore-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediastore-data)](https://pepy.tech/project/mypy-boto3-mediastore-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaStoreData 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
+[boto3.MediaStoreData 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
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
 [mypy-boto3-mediastore-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mediastore-data-1.28.0/mypy_boto3_mediastore_data.egg-info/SOURCES.txt` & `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.0/setup.py` & `mypy-boto3-mediastore-data-1.28.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediastore-data",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_mediastore_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaStoreData 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.MediaStoreData 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

