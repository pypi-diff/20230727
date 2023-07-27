# Comparing `tmp/mypy-boto3-cloudsearchdomain-1.28.0.tar.gz` & `tmp/mypy-boto3-cloudsearchdomain-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudsearchdomain-1.28.0.tar", last modified: Thu Jul  6 20:59:11 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudsearchdomain-1.28.12.tar", last modified: Thu Jul 27 05:34:26 2023, max compression
```

## Comparing `mypy-boto3-cloudsearchdomain-1.28.0.tar` & `mypy-boto3-cloudsearchdomain-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:11.146247 mypy-boto3-cloudsearchdomain-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-07-06 20:59:11.142248 mypy-boto3-cloudsearchdomain-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:11.126248 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-06 20:35:30.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:11.142248 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-07-06 20:59:10.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-06 20:59:10.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:10.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:10.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:10.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 20:59:10.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:11.146247 mypy-boto3-cloudsearchdomain-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:26.460558 mypy-boto3-cloudsearchdomain-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:46.000000 mypy-boto3-cloudsearchdomain-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-07-27 05:34:26.460558 mypy-boto3-cloudsearchdomain-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-07-27 05:18:46.000000 mypy-boto3-cloudsearchdomain-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:26.452558 mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-27 05:18:46.000000 mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-27 05:18:46.000000 mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-27 05:18:46.000000 mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-27 05:18:46.000000 mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-27 05:18:46.000000 mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-07-27 05:18:46.000000 mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-07-27 05:18:46.000000 mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:46.000000 mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-27 05:18:47.000000 mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-07-27 05:18:46.000000 mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:46.000000 mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:26.460558 mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-07-27 05:34:26.000000 mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-27 05:34:26.000000 mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:26.000000 mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:26.000000 mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:26.000000 mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:26.000000 mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:26.460558 mypy-boto3-cloudsearchdomain-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-27 05:18:45.000000 mypy-boto3-cloudsearchdomain-1.28.12/setup.py
```

### Comparing `mypy-boto3-cloudsearchdomain-1.28.0/LICENSE` & `mypy-boto3-cloudsearchdomain-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearchdomain-1.28.0/PKG-INFO` & `mypy-boto3-cloudsearchdomain-1.28.12/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudsearchdomain
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudSearchDomain 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudSearchDomain 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cloudsearchdomain"></a>
 
 # mypy-boto3-cloudsearchdomain
 
 [![PyPI - mypy-boto3-cloudsearchdomain](https://img.shields.io/pypi/v/mypy-boto3-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearchdomain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearchdomain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudsearchdomain?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudsearchdomain)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudsearchdomain)](https://pepy.tech/project/mypy-boto3-cloudsearchdomain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudSearchDomain 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
+[boto3.CloudSearchDomain 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
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
 [mypy-boto3-cloudsearchdomain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cloudsearchdomain-1.28.0/README.md` & `mypy-boto3-cloudsearchdomain-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cloudsearchdomain"></a>
 
 # mypy-boto3-cloudsearchdomain
 
 [![PyPI - mypy-boto3-cloudsearchdomain](https://img.shields.io/pypi/v/mypy-boto3-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearchdomain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearchdomain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudsearchdomain?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudsearchdomain)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudsearchdomain)](https://pepy.tech/project/mypy-boto3-cloudsearchdomain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudSearchDomain 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
+[boto3.CloudSearchDomain 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
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
 [mypy-boto3-cloudsearchdomain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/__main__.py` & `mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudSearchDomain 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.CloudSearchDomain 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain\nOther"
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

### Comparing `mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/client.py` & `mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/client.pyi` & `mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/literals.py` & `mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain/literals.py`

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

### Comparing `mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/literals.pyi` & `mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,15 @@
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
@@ -230,26 +231,28 @@
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

### Comparing `mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/type_defs.py` & `mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/type_defs.pyi` & `mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain.egg-info/PKG-INFO` & `mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudsearchdomain
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudSearchDomain 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudSearchDomain 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cloudsearchdomain"></a>
 
 # mypy-boto3-cloudsearchdomain
 
 [![PyPI - mypy-boto3-cloudsearchdomain](https://img.shields.io/pypi/v/mypy-boto3-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearchdomain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearchdomain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudsearchdomain?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudsearchdomain)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudsearchdomain)](https://pepy.tech/project/mypy-boto3-cloudsearchdomain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudSearchDomain 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
+[boto3.CloudSearchDomain 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
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
 [mypy-boto3-cloudsearchdomain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain.egg-info/SOURCES.txt` & `mypy-boto3-cloudsearchdomain-1.28.12/mypy_boto3_cloudsearchdomain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearchdomain-1.28.0/setup.py` & `mypy-boto3-cloudsearchdomain-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudsearchdomain",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_cloudsearchdomain"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudSearchDomain 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.CloudSearchDomain 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

