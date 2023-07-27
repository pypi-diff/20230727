# Comparing `tmp/mypy-boto3-backupstorage-1.28.0.tar.gz` & `tmp/mypy-boto3-backupstorage-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-backupstorage-1.28.0.tar", last modified: Thu Jul  6 20:59:03 2023, max compression
+gzip compressed data, was "mypy-boto3-backupstorage-1.28.12.tar", last modified: Thu Jul 27 05:34:21 2023, max compression
```

## Comparing `mypy-boto3-backupstorage-1.28.0.tar` & `mypy-boto3-backupstorage-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:03.734231 mypy-boto3-backupstorage-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:34:10.000000 mypy-boto3-backupstorage-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-07-06 20:59:03.730231 mypy-boto3-backupstorage-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-06 20:34:10.000000 mypy-boto3-backupstorage-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:03.730231 mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-06 20:34:10.000000 mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-06 20:34:10.000000 mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-06 20:34:10.000000 mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-06 20:34:10.000000 mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-07-06 20:34:10.000000 mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-06 20:34:11.000000 mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-07-06 20:34:10.000000 mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:10.000000 mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-07-06 20:34:11.000000 mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-07-06 20:34:11.000000 mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:34:10.000000 mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:03.730231 mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-07-06 20:59:03.000000 mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-06 20:59:03.000000 mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:03.000000 mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:03.000000 mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:03.000000 mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 20:59:03.000000 mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:03.734231 mypy-boto3-backupstorage-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-06 20:34:10.000000 mypy-boto3-backupstorage-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:21.884569 mypy-boto3-backupstorage-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-07-27 05:34:21.884569 mypy-boto3-backupstorage-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:21.880569 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-07-27 05:17:56.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-07-27 05:17:56.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-07-27 05:17:56.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:21.884569 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-07-27 05:34:21.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-27 05:34:21.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:21.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:21.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:21.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 05:34:21.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:21.884569 mypy-boto3-backupstorage-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/setup.py
```

### Comparing `mypy-boto3-backupstorage-1.28.0/LICENSE` & `mypy-boto3-backupstorage-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backupstorage-1.28.0/PKG-INFO` & `mypy-boto3-backupstorage-1.28.12/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backupstorage
-Version: 1.28.0
-Summary: Type annotations for boto3.BackupStorage 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.BackupStorage 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-backupstorage"></a>
 
 # mypy-boto3-backupstorage
 
 [![PyPI - mypy-boto3-backupstorage](https://img.shields.io/pypi/v/mypy-boto3-backupstorage.svg?color=blue)](https://pypi.org/project/mypy-boto3-backupstorage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backupstorage.svg?color=blue)](https://pypi.org/project/mypy-boto3-backupstorage)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-backupstorage?color=blue)](https://pypistats.org/packages/mypy-boto3-backupstorage)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-backupstorage)](https://pepy.tech/project/mypy-boto3-backupstorage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BackupStorage 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
+[boto3.BackupStorage 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
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
 [mypy-boto3-backupstorage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-backupstorage-1.28.0/README.md` & `mypy-boto3-backupstorage-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-backupstorage"></a>
 
 # mypy-boto3-backupstorage
 
 [![PyPI - mypy-boto3-backupstorage](https://img.shields.io/pypi/v/mypy-boto3-backupstorage.svg?color=blue)](https://pypi.org/project/mypy-boto3-backupstorage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backupstorage.svg?color=blue)](https://pypi.org/project/mypy-boto3-backupstorage)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-backupstorage?color=blue)](https://pypistats.org/packages/mypy-boto3-backupstorage)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-backupstorage)](https://pepy.tech/project/mypy-boto3-backupstorage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BackupStorage 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
+[boto3.BackupStorage 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
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
 [mypy-boto3-backupstorage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage/__main__.py` & `mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.BackupStorage 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.BackupStorage 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage\nOther"
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

### Comparing `mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage/client.py` & `mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage/client.pyi` & `mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage/literals.py` & `mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/literals.py`

 * *Files 0% similar despite different names*

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

### Comparing `mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage/literals.pyi` & `mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/literals.pyi`

 * *Files 0% similar despite different names*

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

### Comparing `mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage/type_defs.py` & `mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage/type_defs.pyi` & `mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage.egg-info/PKG-INFO` & `mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backupstorage
-Version: 1.28.0
-Summary: Type annotations for boto3.BackupStorage 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.BackupStorage 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-backupstorage"></a>
 
 # mypy-boto3-backupstorage
 
 [![PyPI - mypy-boto3-backupstorage](https://img.shields.io/pypi/v/mypy-boto3-backupstorage.svg?color=blue)](https://pypi.org/project/mypy-boto3-backupstorage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backupstorage.svg?color=blue)](https://pypi.org/project/mypy-boto3-backupstorage)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-backupstorage?color=blue)](https://pypistats.org/packages/mypy-boto3-backupstorage)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-backupstorage)](https://pepy.tech/project/mypy-boto3-backupstorage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BackupStorage 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
+[boto3.BackupStorage 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
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
 [mypy-boto3-backupstorage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-backupstorage-1.28.0/mypy_boto3_backupstorage.egg-info/SOURCES.txt` & `mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backupstorage-1.28.0/setup.py` & `mypy-boto3-backupstorage-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-backupstorage",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_backupstorage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.BackupStorage 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.BackupStorage 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

