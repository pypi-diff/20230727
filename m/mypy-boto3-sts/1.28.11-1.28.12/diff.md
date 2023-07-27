# Comparing `tmp/mypy-boto3-sts-1.28.11.tar.gz` & `tmp/mypy-boto3-sts-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sts-1.28.11.tar", last modified: Tue Jul 25 19:49:16 2023, max compression
+gzip compressed data, was "mypy-boto3-sts-1.28.12.tar", last modified: Thu Jul 27 11:49:44 2023, max compression
```

## Comparing `mypy-boto3-sts-1.28.11.tar` & `mypy-boto3-sts-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:16.429064 mypy-boto3-sts-1.28.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 19:48:57.000000 mypy-boto3-sts-1.28.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-07-25 19:49:16.429064 mypy-boto3-sts-1.28.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-07-25 19:48:57.000000 mypy-boto3-sts-1.28.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:16.421064 mypy-boto3-sts-1.28.11/mypy_boto3_sts/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-25 19:48:57.000000 mypy-boto3-sts-1.28.11/mypy_boto3_sts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-25 19:48:57.000000 mypy-boto3-sts-1.28.11/mypy_boto3_sts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-25 19:48:57.000000 mypy-boto3-sts-1.28.11/mypy_boto3_sts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-07-25 19:48:57.000000 mypy-boto3-sts-1.28.11/mypy_boto3_sts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-07-25 19:48:57.000000 mypy-boto3-sts-1.28.11/mypy_boto3_sts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-07-25 19:48:57.000000 mypy-boto3-sts-1.28.11/mypy_boto3_sts/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-07-25 19:48:57.000000 mypy-boto3-sts-1.28.11/mypy_boto3_sts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:48:57.000000 mypy-boto3-sts-1.28.11/mypy_boto3_sts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-07-25 19:48:58.000000 mypy-boto3-sts-1.28.11/mypy_boto3_sts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-25 19:48:57.000000 mypy-boto3-sts-1.28.11/mypy_boto3_sts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 19:48:57.000000 mypy-boto3-sts-1.28.11/mypy_boto3_sts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:16.429064 mypy-boto3-sts-1.28.11/mypy_boto3_sts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-07-25 19:49:16.000000 mypy-boto3-sts-1.28.11/mypy_boto3_sts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-25 19:49:16.000000 mypy-boto3-sts-1.28.11/mypy_boto3_sts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:16.000000 mypy-boto3-sts-1.28.11/mypy_boto3_sts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:16.000000 mypy-boto3-sts-1.28.11/mypy_boto3_sts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 19:49:16.000000 mypy-boto3-sts-1.28.11/mypy_boto3_sts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 19:49:16.000000 mypy-boto3-sts-1.28.11/mypy_boto3_sts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:49:16.429064 mypy-boto3-sts-1.28.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-25 19:48:57.000000 mypy-boto3-sts-1.28.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.265351 mypy-boto3-sts-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:47.000000 mypy-boto3-sts-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-07-27 11:49:44.265351 mypy-boto3-sts-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-07-27 11:47:47.000000 mypy-boto3-sts-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.257351 mypy-boto3-sts-1.28.12/mypy_boto3_sts/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-27 11:47:47.000000 mypy-boto3-sts-1.28.12/mypy_boto3_sts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-27 11:47:47.000000 mypy-boto3-sts-1.28.12/mypy_boto3_sts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 11:47:47.000000 mypy-boto3-sts-1.28.12/mypy_boto3_sts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-07-27 11:47:47.000000 mypy-boto3-sts-1.28.12/mypy_boto3_sts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-07-27 11:47:47.000000 mypy-boto3-sts-1.28.12/mypy_boto3_sts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-07-27 11:47:47.000000 mypy-boto3-sts-1.28.12/mypy_boto3_sts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-07-27 11:47:47.000000 mypy-boto3-sts-1.28.12/mypy_boto3_sts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:47.000000 mypy-boto3-sts-1.28.12/mypy_boto3_sts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-07-27 11:47:47.000000 mypy-boto3-sts-1.28.12/mypy_boto3_sts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-27 11:47:47.000000 mypy-boto3-sts-1.28.12/mypy_boto3_sts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:47.000000 mypy-boto3-sts-1.28.12/mypy_boto3_sts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.265351 mypy-boto3-sts-1.28.12/mypy_boto3_sts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-07-27 11:49:44.000000 mypy-boto3-sts-1.28.12/mypy_boto3_sts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-27 11:49:44.000000 mypy-boto3-sts-1.28.12/mypy_boto3_sts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:44.000000 mypy-boto3-sts-1.28.12/mypy_boto3_sts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:44.000000 mypy-boto3-sts-1.28.12/mypy_boto3_sts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:44.000000 mypy-boto3-sts-1.28.12/mypy_boto3_sts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:44.000000 mypy-boto3-sts-1.28.12/mypy_boto3_sts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:44.265351 mypy-boto3-sts-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 11:47:47.000000 mypy-boto3-sts-1.28.12/setup.py
```

### Comparing `mypy-boto3-sts-1.28.11/LICENSE` & `mypy-boto3-sts-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sts-1.28.11/PKG-INFO` & `mypy-boto3-sts-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sts
-Version: 1.28.11
-Summary: Type annotations for boto3.STS 1.28.11 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.STS 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sts"></a>
 
 # mypy-boto3-sts
 
 [![PyPI - mypy-boto3-sts](https://img.shields.io/pypi/v/mypy-boto3-sts.svg?color=blue)](https://pypi.org/project/mypy-boto3-sts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sts.svg?color=blue)](https://pypi.org/project/mypy-boto3-sts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sts?color=blue)](https://pypistats.org/packages/mypy-boto3-sts)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sts)](https://pepy.tech/project/mypy-boto3-sts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.STS 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
+[boto3.STS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sts-1.28.11/README.md` & `mypy-boto3-sts-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sts"></a>
 
 # mypy-boto3-sts
 
 [![PyPI - mypy-boto3-sts](https://img.shields.io/pypi/v/mypy-boto3-sts.svg?color=blue)](https://pypi.org/project/mypy-boto3-sts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sts.svg?color=blue)](https://pypi.org/project/mypy-boto3-sts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sts?color=blue)](https://pypistats.org/packages/mypy-boto3-sts)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sts)](https://pepy.tech/project/mypy-boto3-sts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.STS 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
+[boto3.STS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sts-1.28.11/mypy_boto3_sts/__main__.py` & `mypy-boto3-sts-1.28.12/mypy_boto3_sts/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.STS 1.28.11\nVersion:         1.28.11\nBuilder version:"
-        " 7.15.1\nDocs:           "
+        "Type annotations for boto3.STS 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.11")
+    print("1.28.12")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-sts-1.28.11/mypy_boto3_sts/client.py` & `mypy-boto3-sts-1.28.12/mypy_boto3_sts/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sts-1.28.11/mypy_boto3_sts/client.pyi` & `mypy-boto3-sts-1.28.12/mypy_boto3_sts/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sts-1.28.11/mypy_boto3_sts/literals.py` & `mypy-boto3-sts-1.28.12/mypy_boto3_sts/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,15 @@
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
@@ -224,14 +225,15 @@
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
```

### Comparing `mypy-boto3-sts-1.28.11/mypy_boto3_sts/literals.pyi` & `mypy-boto3-sts-1.28.12/mypy_boto3_sts/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,15 @@
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
@@ -222,14 +223,15 @@
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
```

### Comparing `mypy-boto3-sts-1.28.11/mypy_boto3_sts/type_defs.py` & `mypy-boto3-sts-1.28.12/mypy_boto3_sts/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sts-1.28.11/mypy_boto3_sts/type_defs.pyi` & `mypy-boto3-sts-1.28.12/mypy_boto3_sts/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sts-1.28.11/mypy_boto3_sts.egg-info/PKG-INFO` & `mypy-boto3-sts-1.28.12/mypy_boto3_sts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sts
-Version: 1.28.11
-Summary: Type annotations for boto3.STS 1.28.11 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.STS 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sts"></a>
 
 # mypy-boto3-sts
 
 [![PyPI - mypy-boto3-sts](https://img.shields.io/pypi/v/mypy-boto3-sts.svg?color=blue)](https://pypi.org/project/mypy-boto3-sts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sts.svg?color=blue)](https://pypi.org/project/mypy-boto3-sts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sts?color=blue)](https://pypistats.org/packages/mypy-boto3-sts)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sts)](https://pepy.tech/project/mypy-boto3-sts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.STS 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
+[boto3.STS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sts-1.28.11/mypy_boto3_sts.egg-info/SOURCES.txt` & `mypy-boto3-sts-1.28.12/mypy_boto3_sts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sts-1.28.11/setup.py` & `mypy-boto3-sts-1.28.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sts",
-    version="1.28.11",
+    version="1.28.12",
     packages=["mypy_boto3_sts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.STS 1.28.11 service generated with mypy-boto3-builder 7.15.1"
+        "Type annotations for boto3.STS 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

