# Comparing `tmp/mypy-boto3-ec2-instance-connect-1.28.0.tar.gz` & `tmp/mypy-boto3-ec2-instance-connect-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ec2-instance-connect-1.28.0.tar", last modified: Thu Jul  6 20:59:28 2023, max compression
+gzip compressed data, was "mypy-boto3-ec2-instance-connect-1.28.12.tar", last modified: Thu Jul 27 05:34:37 2023, max compression
```

## Comparing `mypy-boto3-ec2-instance-connect-1.28.0.tar` & `mypy-boto3-ec2-instance-connect-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:28.274287 mypy-boto3-ec2-instance-connect-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:39:45.000000 mypy-boto3-ec2-instance-connect-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12650 2023-07-06 20:59:28.270287 mypy-boto3-ec2-instance-connect-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-07-06 20:39:45.000000 mypy-boto3-ec2-instance-connect-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:28.266287 mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-06 20:39:45.000000 mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-06 20:39:45.000000 mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-06 20:39:45.000000 mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-06 20:39:45.000000 mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-06 20:39:45.000000 mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-07-06 20:39:46.000000 mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-07-06 20:39:45.000000 mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:39:45.000000 mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-06 20:39:46.000000 mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-07-06 20:39:46.000000 mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:39:45.000000 mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:28.270287 mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12650 2023-07-06 20:59:27.000000 mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-06 20:59:28.000000 mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:27.000000 mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:27.000000 mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:27.000000 mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 20:59:27.000000 mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:28.274287 mypy-boto3-ec2-instance-connect-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-06 20:39:45.000000 mypy-boto3-ec2-instance-connect-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:37.056525 mypy-boto3-ec2-instance-connect-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:26.000000 mypy-boto3-ec2-instance-connect-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-07-27 05:34:37.056525 mypy-boto3-ec2-instance-connect-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-07-27 05:21:26.000000 mypy-boto3-ec2-instance-connect-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:37.052525 mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-27 05:21:26.000000 mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-27 05:21:26.000000 mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-27 05:21:26.000000 mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-27 05:21:26.000000 mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-27 05:21:26.000000 mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-07-27 05:21:27.000000 mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-07-27 05:21:27.000000 mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:26.000000 mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-27 05:21:27.000000 mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-07-27 05:21:27.000000 mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:26.000000 mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:37.056525 mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-07-27 05:34:36.000000 mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-27 05:34:36.000000 mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:36.000000 mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:36.000000 mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:36.000000 mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 05:34:36.000000 mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:37.056525 mypy-boto3-ec2-instance-connect-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-27 05:21:26.000000 mypy-boto3-ec2-instance-connect-1.28.12/setup.py
```

### Comparing `mypy-boto3-ec2-instance-connect-1.28.0/LICENSE` & `mypy-boto3-ec2-instance-connect-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-instance-connect-1.28.0/PKG-INFO` & `mypy-boto3-ec2-instance-connect-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ec2-instance-connect
-Version: 1.28.0
-Summary: Type annotations for boto3.EC2InstanceConnect 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.EC2InstanceConnect 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2_instance_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ec2-instance-connect"></a>
 
 # mypy-boto3-ec2-instance-connect
 
 [![PyPI - mypy-boto3-ec2-instance-connect](https://img.shields.io/pypi/v/mypy-boto3-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2-instance-connect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2-instance-connect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2_instance_connect/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ec2-instance-connect?color=blue)](https://pypistats.org/packages/mypy-boto3-ec2-instance-connect)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ec2-instance-connect)](https://pepy.tech/project/mypy-boto3-ec2-instance-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2InstanceConnect 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
+[boto3.EC2InstanceConnect 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
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
 [mypy-boto3-ec2-instance-connect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2_instance_connect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ec2-instance-connect-1.28.0/README.md` & `mypy-boto3-ec2-instance-connect-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ec2-instance-connect"></a>
 
 # mypy-boto3-ec2-instance-connect
 
 [![PyPI - mypy-boto3-ec2-instance-connect](https://img.shields.io/pypi/v/mypy-boto3-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2-instance-connect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2-instance-connect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2_instance_connect/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ec2-instance-connect?color=blue)](https://pypistats.org/packages/mypy-boto3-ec2-instance-connect)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ec2-instance-connect)](https://pepy.tech/project/mypy-boto3-ec2-instance-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2InstanceConnect 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
+[boto3.EC2InstanceConnect 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
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
 [mypy-boto3-ec2-instance-connect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2_instance_connect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect/client.py` & `mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect/client.pyi` & `mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect/literals.py` & `mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect/literals.py`

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
@@ -224,26 +225,28 @@
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

### Comparing `mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect/literals.pyi` & `mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect/literals.pyi`

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
@@ -222,26 +223,28 @@
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

### Comparing `mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect/type_defs.py` & `mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect/type_defs.pyi` & `mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect.egg-info/PKG-INFO` & `mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ec2-instance-connect
-Version: 1.28.0
-Summary: Type annotations for boto3.EC2InstanceConnect 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.EC2InstanceConnect 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2_instance_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ec2-instance-connect"></a>
 
 # mypy-boto3-ec2-instance-connect
 
 [![PyPI - mypy-boto3-ec2-instance-connect](https://img.shields.io/pypi/v/mypy-boto3-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2-instance-connect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2-instance-connect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2_instance_connect/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ec2-instance-connect?color=blue)](https://pypistats.org/packages/mypy-boto3-ec2-instance-connect)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ec2-instance-connect)](https://pepy.tech/project/mypy-boto3-ec2-instance-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2InstanceConnect 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
+[boto3.EC2InstanceConnect 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
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
 [mypy-boto3-ec2-instance-connect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2_instance_connect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ec2-instance-connect-1.28.0/mypy_boto3_ec2_instance_connect.egg-info/SOURCES.txt` & `mypy-boto3-ec2-instance-connect-1.28.12/mypy_boto3_ec2_instance_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-instance-connect-1.28.0/setup.py` & `mypy-boto3-ec2-instance-connect-1.28.12/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ec2-instance-connect",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_ec2_instance_connect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EC2InstanceConnect 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.EC2InstanceConnect 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

