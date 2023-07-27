# Comparing `tmp/mypy-boto3-cloudcontrol-1.28.0.tar.gz` & `tmp/mypy-boto3-cloudcontrol-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudcontrol-1.28.0.tar", last modified: Thu Jul  6 20:59:09 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudcontrol-1.28.12.tar", last modified: Thu Jul 27 05:34:24 2023, max compression
```

## Comparing `mypy-boto3-cloudcontrol-1.28.0.tar` & `mypy-boto3-cloudcontrol-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:09.006243 mypy-boto3-cloudcontrol-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:34:58.000000 mypy-boto3-cloudcontrol-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14745 2023-07-06 20:59:09.002243 mypy-boto3-cloudcontrol-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-07-06 20:34:58.000000 mypy-boto3-cloudcontrol-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:08.998243 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-06 20:34:58.000000 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-06 20:34:58.000000 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-06 20:34:58.000000 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10839 2023-07-06 20:34:58.000000 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-07-06 20:34:58.000000 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-07-06 20:34:59.000000 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-07-06 20:34:58.000000 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-06 20:34:58.000000 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-06 20:34:58.000000 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:58.000000 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-07-06 20:34:59.000000 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-07-06 20:34:59.000000 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:34:58.000000 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-06 20:34:58.000000 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-06 20:34:58.000000 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:09.002243 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14745 2023-07-06 20:59:08.000000 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-06 20:59:08.000000 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:08.000000 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:08.000000 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:08.000000 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 20:59:08.000000 mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:09.006243 mypy-boto3-cloudcontrol-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-06 20:34:58.000000 mypy-boto3-cloudcontrol-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.956563 mypy-boto3-cloudcontrol-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-07-27 05:34:24.952563 mypy-boto3-cloudcontrol-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.952563 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10839 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.952563 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-07-27 05:34:24.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-27 05:34:24.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:24.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:24.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:24.956563 mypy-boto3-cloudcontrol-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-27 05:18:25.000000 mypy-boto3-cloudcontrol-1.28.12/setup.py
```

### Comparing `mypy-boto3-cloudcontrol-1.28.0/LICENSE` & `mypy-boto3-cloudcontrol-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.0/PKG-INFO` & `mypy-boto3-cloudcontrol-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudcontrol
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudControlApi 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudControlApi 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cloudcontrol"></a>
 
 # mypy-boto3-cloudcontrol
 
 [![PyPI - mypy-boto3-cloudcontrol](https://img.shields.io/pypi/v/mypy-boto3-cloudcontrol.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudcontrol)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudcontrol.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudcontrol)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudcontrol?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudcontrol)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudcontrol)](https://pepy.tech/project/mypy-boto3-cloudcontrol)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudControlApi 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
+[boto3.CloudControlApi 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
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
 [mypy-boto3-cloudcontrol docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cloudcontrol-1.28.0/README.md` & `mypy-boto3-cloudcontrol-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cloudcontrol"></a>
 
 # mypy-boto3-cloudcontrol
 
 [![PyPI - mypy-boto3-cloudcontrol](https://img.shields.io/pypi/v/mypy-boto3-cloudcontrol.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudcontrol)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudcontrol.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudcontrol)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudcontrol?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudcontrol)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudcontrol)](https://pepy.tech/project/mypy-boto3-cloudcontrol)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudControlApi 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
+[boto3.CloudControlApi 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
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
 [mypy-boto3-cloudcontrol docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/__init__.py` & `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/__init__.pyi` & `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/__main__.py` & `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudControlApi 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.CloudControlApi 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi\nOther"
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

### Comparing `mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/client.py` & `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/client.pyi` & `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/literals.py` & `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,14 +175,15 @@
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
@@ -261,26 +262,28 @@
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

### Comparing `mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/literals.pyi` & `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -173,14 +173,15 @@
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
@@ -259,26 +260,28 @@
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

### Comparing `mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/paginator.py` & `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/paginator.pyi` & `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/type_defs.py` & `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/type_defs.pyi` & `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/waiter.py` & `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol/waiter.pyi` & `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol.egg-info/PKG-INFO` & `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudcontrol
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudControlApi 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudControlApi 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cloudcontrol"></a>
 
 # mypy-boto3-cloudcontrol
 
 [![PyPI - mypy-boto3-cloudcontrol](https://img.shields.io/pypi/v/mypy-boto3-cloudcontrol.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudcontrol)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudcontrol.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudcontrol)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudcontrol?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudcontrol)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudcontrol)](https://pepy.tech/project/mypy-boto3-cloudcontrol)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudControlApi 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
+[boto3.CloudControlApi 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
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
 [mypy-boto3-cloudcontrol docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cloudcontrol-1.28.0/mypy_boto3_cloudcontrol.egg-info/SOURCES.txt` & `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.0/setup.py` & `mypy-boto3-cloudcontrol-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudcontrol",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_cloudcontrol"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudControlApi 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.CloudControlApi 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

