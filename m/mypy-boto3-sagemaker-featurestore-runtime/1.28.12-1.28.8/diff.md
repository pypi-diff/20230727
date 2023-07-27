# Comparing `tmp/mypy-boto3-sagemaker-featurestore-runtime-1.28.12.tar.gz` & `tmp/mypy-boto3-sagemaker-featurestore-runtime-1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sagemaker-featurestore-runtime-1.28.12.tar", last modified: Thu Jul 27 11:49:34 2023, max compression
+gzip compressed data, was "mypy-boto3-sagemaker-featurestore-runtime-1.28.8.tar", last modified: Thu Jul 20 19:47:56 2023, max compression
```

## Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.12.tar` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.993248 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:45:54.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-07-27 11:49:33.981248 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-07-27 11:45:54.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.981248 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-27 11:45:54.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-27 11:45:54.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-27 11:45:54.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-27 11:45:54.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-07-27 11:45:54.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-07-27 11:45:54.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-07-27 11:45:54.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:54.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-27 11:45:54.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-27 11:45:54.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:45:54.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.981248 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-07-27 11:49:33.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-27 11:49:33.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:33.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:33.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:33.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-27 11:49:33.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:33.993248 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-27 11:45:54.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.008775 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-07-20 19:47:56.008775 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.000775 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.008775 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-07-20 19:47:55.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-20 19:47:55.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 19:47:55.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-20 19:47:55.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:56.008775 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-20 19:47:15.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/setup.py
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.12/LICENSE` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.12/PKG-INFO` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-featurestore-runtime
-Version: 1.28.12
-Summary: Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.8
+Summary: Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sagemaker-featurestore-runtime"></a>
 
 # mypy-boto3-sagemaker-featurestore-runtime
 
 [![PyPI - mypy-boto3-sagemaker-featurestore-runtime](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-featurestore-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-featurestore-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-featurestore-runtime)](https://pepy.tech/project/mypy-boto3-sagemaker-featurestore-runtime)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-featurestore-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-featurestore-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerFeatureStoreRuntime 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
+[boto3.SageMakerFeatureStoreRuntime 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
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
 [mypy-boto3-sagemaker-featurestore-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.12/README.md` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sagemaker-featurestore-runtime"></a>
 
 # mypy-boto3-sagemaker-featurestore-runtime
 
 [![PyPI - mypy-boto3-sagemaker-featurestore-runtime](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-featurestore-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-featurestore-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-featurestore-runtime)](https://pepy.tech/project/mypy-boto3-sagemaker-featurestore-runtime)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-featurestore-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-featurestore-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerFeatureStoreRuntime 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
+[boto3.SageMakerFeatureStoreRuntime 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
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
 [mypy-boto3-sagemaker-featurestore-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime/__init__.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime/__init__.pyi` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime/__main__.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.8\nVersion:        "
+        " 1.28.8\nBuilder version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.8")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime/client.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime/client.pyi` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime/literals.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,14 @@
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
@@ -237,15 +236,14 @@
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

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime/literals.pyi` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,14 @@
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
@@ -235,15 +234,14 @@
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

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime/type_defs.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,36 +51,23 @@
         "FeatureGroupName": str,
         "RecordIdentifierValueAsString": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
 )
 
-_RequiredBatchGetRecordIdentifierOutputTypeDef = TypedDict(
-    "_RequiredBatchGetRecordIdentifierOutputTypeDef",
+BatchGetRecordIdentifierOutputTypeDef = TypedDict(
+    "BatchGetRecordIdentifierOutputTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifiersValueAsString": List[str],
-    },
-)
-_OptionalBatchGetRecordIdentifierOutputTypeDef = TypedDict(
-    "_OptionalBatchGetRecordIdentifierOutputTypeDef",
-    {
         "FeatureNames": List[str],
     },
-    total=False,
 )
 
-
-class BatchGetRecordIdentifierOutputTypeDef(
-    _RequiredBatchGetRecordIdentifierOutputTypeDef, _OptionalBatchGetRecordIdentifierOutputTypeDef
-):
-    pass
-
-
 _RequiredBatchGetRecordIdentifierTypeDef = TypedDict(
     "_RequiredBatchGetRecordIdentifierTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifiersValueAsString": Sequence[str],
     },
 )
@@ -205,37 +192,24 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchGetRecordResultDetailTypeDef = TypedDict(
-    "_RequiredBatchGetRecordResultDetailTypeDef",
+BatchGetRecordResultDetailTypeDef = TypedDict(
+    "BatchGetRecordResultDetailTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifierValueAsString": str,
         "Record": List[FeatureValueOutputTypeDef],
-    },
-)
-_OptionalBatchGetRecordResultDetailTypeDef = TypedDict(
-    "_OptionalBatchGetRecordResultDetailTypeDef",
-    {
         "ExpiresAt": str,
     },
-    total=False,
 )
 
-
-class BatchGetRecordResultDetailTypeDef(
-    _RequiredBatchGetRecordResultDetailTypeDef, _OptionalBatchGetRecordResultDetailTypeDef
-):
-    pass
-
-
 GetRecordResponseTypeDef = TypedDict(
     "GetRecordResponseTypeDef",
     {
         "Record": List[FeatureValueOutputTypeDef],
         "ExpiresAt": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime/type_defs.pyi` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -50,34 +50,23 @@
         "FeatureGroupName": str,
         "RecordIdentifierValueAsString": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
 )
 
-_RequiredBatchGetRecordIdentifierOutputTypeDef = TypedDict(
-    "_RequiredBatchGetRecordIdentifierOutputTypeDef",
+BatchGetRecordIdentifierOutputTypeDef = TypedDict(
+    "BatchGetRecordIdentifierOutputTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifiersValueAsString": List[str],
-    },
-)
-_OptionalBatchGetRecordIdentifierOutputTypeDef = TypedDict(
-    "_OptionalBatchGetRecordIdentifierOutputTypeDef",
-    {
         "FeatureNames": List[str],
     },
-    total=False,
 )
 
-class BatchGetRecordIdentifierOutputTypeDef(
-    _RequiredBatchGetRecordIdentifierOutputTypeDef, _OptionalBatchGetRecordIdentifierOutputTypeDef
-):
-    pass
-
 _RequiredBatchGetRecordIdentifierTypeDef = TypedDict(
     "_RequiredBatchGetRecordIdentifierTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifiersValueAsString": Sequence[str],
     },
 )
@@ -194,35 +183,24 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchGetRecordResultDetailTypeDef = TypedDict(
-    "_RequiredBatchGetRecordResultDetailTypeDef",
+BatchGetRecordResultDetailTypeDef = TypedDict(
+    "BatchGetRecordResultDetailTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifierValueAsString": str,
         "Record": List[FeatureValueOutputTypeDef],
-    },
-)
-_OptionalBatchGetRecordResultDetailTypeDef = TypedDict(
-    "_OptionalBatchGetRecordResultDetailTypeDef",
-    {
         "ExpiresAt": str,
     },
-    total=False,
 )
 
-class BatchGetRecordResultDetailTypeDef(
-    _RequiredBatchGetRecordResultDetailTypeDef, _OptionalBatchGetRecordResultDetailTypeDef
-):
-    pass
-
 GetRecordResponseTypeDef = TypedDict(
     "GetRecordResponseTypeDef",
     {
         "Record": List[FeatureValueOutputTypeDef],
         "ExpiresAt": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime.egg-info/PKG-INFO` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-featurestore-runtime
-Version: 1.28.12
-Summary: Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.8
+Summary: Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sagemaker-featurestore-runtime"></a>
 
 # mypy-boto3-sagemaker-featurestore-runtime
 
 [![PyPI - mypy-boto3-sagemaker-featurestore-runtime](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-featurestore-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-featurestore-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-featurestore-runtime)](https://pepy.tech/project/mypy-boto3-sagemaker-featurestore-runtime)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-featurestore-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-featurestore-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerFeatureStoreRuntime 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
+[boto3.SageMakerFeatureStoreRuntime 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
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
 [mypy-boto3-sagemaker-featurestore-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.12/mypy_boto3_sagemaker_featurestore_runtime.egg-info/SOURCES.txt` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.12/setup.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker-featurestore-runtime",
-    version="1.28.12",
+    version="1.28.8",
     packages=["mypy_boto3_sagemaker_featurestore_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.8 service generated with"
+        " mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

