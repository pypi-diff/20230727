# Comparing `tmp/mypy-boto3-elastic-inference-1.28.0.tar.gz` & `tmp/mypy-boto3-elastic-inference-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elastic-inference-1.28.0.tar", last modified: Thu Jul  6 20:59:30 2023, max compression
+gzip compressed data, was "mypy-boto3-elastic-inference-1.28.12.tar", last modified: Thu Jul 27 05:34:38 2023, max compression
```

## Comparing `mypy-boto3-elastic-inference-1.28.0.tar` & `mypy-boto3-elastic-inference-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:30.330292 mypy-boto3-elastic-inference-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:40:09.000000 mypy-boto3-elastic-inference-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-07-06 20:59:30.330292 mypy-boto3-elastic-inference-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-07-06 20:40:09.000000 mypy-boto3-elastic-inference-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:30.318292 mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-06 20:40:09.000000 mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-06 20:40:09.000000 mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-06 20:40:09.000000 mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-07-06 20:40:09.000000 mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-07-06 20:40:09.000000 mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-07-06 20:40:09.000000 mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-07-06 20:40:09.000000 mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-06 20:40:09.000000 mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-06 20:40:09.000000 mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:40:09.000000 mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-07-06 20:40:10.000000 mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-06 20:40:09.000000 mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:40:09.000000 mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:30.330292 mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-07-06 20:59:30.000000 mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-06 20:59:30.000000 mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:30.000000 mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:30.000000 mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:30.000000 mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 20:59:30.000000 mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:30.330292 mypy-boto3-elastic-inference-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-06 20:40:09.000000 mypy-boto3-elastic-inference-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.340521 mypy-boto3-elastic-inference-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-07-27 05:34:38.340521 mypy-boto3-elastic-inference-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.336521 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.340521 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-07-27 05:34:38.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-27 05:34:38.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:38.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:38.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:38.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:38.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:38.340521 mypy-boto3-elastic-inference-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/setup.py
```

### Comparing `mypy-boto3-elastic-inference-1.28.0/LICENSE` & `mypy-boto3-elastic-inference-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.0/PKG-INFO` & `mypy-boto3-elastic-inference-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elastic-inference
-Version: 1.28.0
-Summary: Type annotations for boto3.ElasticInference 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ElasticInference 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-elastic-inference"></a>
 
 # mypy-boto3-elastic-inference
 
 [![PyPI - mypy-boto3-elastic-inference](https://img.shields.io/pypi/v/mypy-boto3-elastic-inference.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastic-inference)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elastic-inference.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastic-inference)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elastic-inference?color=blue)](https://pypistats.org/packages/mypy-boto3-elastic-inference)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elastic-inference)](https://pepy.tech/project/mypy-boto3-elastic-inference)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticInference 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
+[boto3.ElasticInference 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
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
 [mypy-boto3-elastic-inference docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-elastic-inference-1.28.0/README.md` & `mypy-boto3-elastic-inference-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-elastic-inference"></a>
 
 # mypy-boto3-elastic-inference
 
 [![PyPI - mypy-boto3-elastic-inference](https://img.shields.io/pypi/v/mypy-boto3-elastic-inference.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastic-inference)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elastic-inference.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastic-inference)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elastic-inference?color=blue)](https://pypistats.org/packages/mypy-boto3-elastic-inference)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elastic-inference)](https://pepy.tech/project/mypy-boto3-elastic-inference)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticInference 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
+[boto3.ElasticInference 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
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
 [mypy-boto3-elastic-inference docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/__init__.py` & `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/__init__.pyi` & `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/__main__.py` & `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElasticInference 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ElasticInference 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference\nOther"
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

### Comparing `mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/client.py` & `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/client.pyi` & `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/literals.py` & `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/literals.py`

 * *Files 2% similar despite different names*

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

### Comparing `mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/literals.pyi` & `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/literals.pyi`

 * *Files 2% similar despite different names*

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

### Comparing `mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/paginator.py` & `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/paginator.pyi` & `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/type_defs.py` & `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference/type_defs.pyi` & `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference.egg-info/PKG-INFO` & `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elastic-inference
-Version: 1.28.0
-Summary: Type annotations for boto3.ElasticInference 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ElasticInference 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-elastic-inference"></a>
 
 # mypy-boto3-elastic-inference
 
 [![PyPI - mypy-boto3-elastic-inference](https://img.shields.io/pypi/v/mypy-boto3-elastic-inference.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastic-inference)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elastic-inference.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastic-inference)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elastic-inference?color=blue)](https://pypistats.org/packages/mypy-boto3-elastic-inference)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elastic-inference)](https://pepy.tech/project/mypy-boto3-elastic-inference)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticInference 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
+[boto3.ElasticInference 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
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
 [mypy-boto3-elastic-inference docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-elastic-inference-1.28.0/mypy_boto3_elastic_inference.egg-info/SOURCES.txt` & `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.0/setup.py` & `mypy-boto3-elastic-inference-1.28.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elastic-inference",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_elastic_inference"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElasticInference 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ElasticInference 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

