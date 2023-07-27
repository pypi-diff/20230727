# Comparing `tmp/mypy-boto3-sagemaker-edge-1.28.0.tar.gz` & `tmp/mypy-boto3-sagemaker-edge-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sagemaker-edge-1.28.0.tar", last modified: Thu Jul  6 21:00:32 2023, max compression
+gzip compressed data, was "mypy-boto3-sagemaker-edge-1.28.12.tar", last modified: Thu Jul 27 11:49:33 2023, max compression
```

## Comparing `mypy-boto3-sagemaker-edge-1.28.0.tar` & `mypy-boto3-sagemaker-edge-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:32.222420 mypy-boto3-sagemaker-edge-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:54:49.000000 mypy-boto3-sagemaker-edge-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12753 2023-07-06 21:00:32.214420 mypy-boto3-sagemaker-edge-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11234 2023-07-06 20:54:49.000000 mypy-boto3-sagemaker-edge-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:32.206420 mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-06 20:54:49.000000 mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-06 20:54:49.000000 mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-06 20:54:49.000000 mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-06 20:54:49.000000 mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-07-06 20:54:49.000000 mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-07-06 20:54:49.000000 mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-07-06 20:54:49.000000 mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:54:49.000000 mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-06 20:54:50.000000 mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-06 20:54:49.000000 mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:54:49.000000 mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:32.214420 mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12753 2023-07-06 21:00:31.000000 mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-06 21:00:31.000000 mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:31.000000 mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:31.000000 mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:31.000000 mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 21:00:31.000000 mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:32.222420 mypy-boto3-sagemaker-edge-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-06 20:54:49.000000 mypy-boto3-sagemaker-edge-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.501243 mypy-boto3-sagemaker-edge-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:45:53.000000 mypy-boto3-sagemaker-edge-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-07-27 11:49:33.493243 mypy-boto3-sagemaker-edge-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-07-27 11:45:53.000000 mypy-boto3-sagemaker-edge-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.493243 mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-27 11:45:53.000000 mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-27 11:45:53.000000 mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-27 11:45:53.000000 mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-27 11:45:53.000000 mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-07-27 11:45:53.000000 mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-07-27 11:45:53.000000 mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-07-27 11:45:53.000000 mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:53.000000 mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-27 11:45:54.000000 mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-27 11:45:53.000000 mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:45:53.000000 mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.493243 mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-07-27 11:49:33.000000 mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-27 11:49:33.000000 mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:33.000000 mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:33.000000 mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:33.000000 mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 11:49:33.000000 mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:33.501243 mypy-boto3-sagemaker-edge-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-27 11:45:53.000000 mypy-boto3-sagemaker-edge-1.28.12/setup.py
```

### Comparing `mypy-boto3-sagemaker-edge-1.28.0/LICENSE` & `mypy-boto3-sagemaker-edge-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-edge-1.28.0/PKG-INFO` & `mypy-boto3-sagemaker-edge-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-edge
-Version: 1.28.0
-Summary: Type annotations for boto3.SagemakerEdgeManager 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SagemakerEdgeManager 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_edge/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sagemaker-edge"></a>
 
 # mypy-boto3-sagemaker-edge
 
 [![PyPI - mypy-boto3-sagemaker-edge](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-edge.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-edge)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-edge.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-edge)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_edge/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-edge?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-edge)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-edge)](https://pepy.tech/project/mypy-boto3-sagemaker-edge)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SagemakerEdgeManager 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
+[boto3.SagemakerEdgeManager 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
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
 [mypy-boto3-sagemaker-edge docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_edge/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,22 +305,22 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_edge.type_defs import (
     ChecksumTypeDef,
     DeploymentModelTypeDef,
     EdgeMetricTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetDeploymentsRequestRequestTypeDef,
     GetDeviceRegistrationRequestRequestTypeDef,
-    GetDeviceRegistrationResultTypeDef,
-    ResponseMetadataTypeDef,
     DefinitionTypeDef,
     DeploymentResultTypeDef,
     ModelTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDeviceRegistrationResultTypeDef,
     EdgeDeploymentTypeDef,
     SendHeartbeatRequestRequestTypeDef,
     GetDeploymentsResultTypeDef,
 )
 
 
 def get_structure() -> ChecksumTypeDef:
```

### Comparing `mypy-boto3-sagemaker-edge-1.28.0/README.md` & `mypy-boto3-sagemaker-edge-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sagemaker-edge"></a>
 
 # mypy-boto3-sagemaker-edge
 
 [![PyPI - mypy-boto3-sagemaker-edge](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-edge.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-edge)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-edge.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-edge)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_edge/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-edge?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-edge)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-edge)](https://pepy.tech/project/mypy-boto3-sagemaker-edge)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SagemakerEdgeManager 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
+[boto3.SagemakerEdgeManager 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
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
 [mypy-boto3-sagemaker-edge docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_edge/).
 
 See how it helps to find and fix potential bugs:
 
@@ -273,22 +273,22 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_edge.type_defs import (
     ChecksumTypeDef,
     DeploymentModelTypeDef,
     EdgeMetricTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetDeploymentsRequestRequestTypeDef,
     GetDeviceRegistrationRequestRequestTypeDef,
-    GetDeviceRegistrationResultTypeDef,
-    ResponseMetadataTypeDef,
     DefinitionTypeDef,
     DeploymentResultTypeDef,
     ModelTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDeviceRegistrationResultTypeDef,
     EdgeDeploymentTypeDef,
     SendHeartbeatRequestRequestTypeDef,
     GetDeploymentsResultTypeDef,
 )
 
 
 def get_structure() -> ChecksumTypeDef:
```

### Comparing `mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge/__main__.py` & `mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SagemakerEdgeManager 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.SagemakerEdgeManager 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_edge//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager\nOther"
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

### Comparing `mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge/client.py` & `mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge/client.pyi` & `mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge/literals.py` & `mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,15 @@
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
@@ -239,26 +240,28 @@
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

### Comparing `mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge/literals.pyi` & `mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -151,14 +151,15 @@
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
@@ -237,26 +238,28 @@
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

### Comparing `mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge/type_defs.py` & `mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,22 +27,22 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ChecksumTypeDef",
     "DeploymentModelTypeDef",
     "EdgeMetricTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "GetDeploymentsRequestRequestTypeDef",
     "GetDeviceRegistrationRequestRequestTypeDef",
-    "GetDeviceRegistrationResultTypeDef",
-    "ResponseMetadataTypeDef",
     "DefinitionTypeDef",
     "DeploymentResultTypeDef",
     "ModelTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetDeviceRegistrationResultTypeDef",
     "EdgeDeploymentTypeDef",
     "SendHeartbeatRequestRequestTypeDef",
     "GetDeploymentsResultTypeDef",
 )
 
 ChecksumTypeDef = TypedDict(
     "ChecksumTypeDef",
@@ -75,18 +75,22 @@
         "MetricName": str,
         "Value": float,
         "Timestamp": Union[datetime, str],
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetDeploymentsRequestRequestTypeDef = TypedDict(
     "GetDeploymentsRequestRequestTypeDef",
     {
         "DeviceName": str,
@@ -98,34 +102,14 @@
     "GetDeviceRegistrationRequestRequestTypeDef",
     {
         "DeviceName": str,
         "DeviceFleetName": str,
     },
 )
 
-GetDeviceRegistrationResultTypeDef = TypedDict(
-    "GetDeviceRegistrationResultTypeDef",
-    {
-        "DeviceRegistration": str,
-        "CacheTTL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 DefinitionTypeDef = TypedDict(
     "DefinitionTypeDef",
     {
         "ModelHandle": str,
         "S3Url": str,
         "Checksum": ChecksumTypeDef,
         "State": ModelStateType,
@@ -154,14 +138,30 @@
         "LatestSampleTime": Union[datetime, str],
         "LatestInference": Union[datetime, str],
         "ModelMetrics": Sequence[EdgeMetricTypeDef],
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeviceRegistrationResultTypeDef = TypedDict(
+    "GetDeviceRegistrationResultTypeDef",
+    {
+        "DeviceRegistration": str,
+        "CacheTTL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 EdgeDeploymentTypeDef = TypedDict(
     "EdgeDeploymentTypeDef",
     {
         "DeploymentName": str,
         "Type": Literal["Model"],
         "FailureHandlingPolicy": FailureHandlingPolicyType,
         "Definitions": List[DefinitionTypeDef],
@@ -194,10 +194,10 @@
     pass
 
 
 GetDeploymentsResultTypeDef = TypedDict(
     "GetDeploymentsResultTypeDef",
     {
         "Deployments": List[EdgeDeploymentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge/type_defs.pyi` & `mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -26,22 +26,22 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ChecksumTypeDef",
     "DeploymentModelTypeDef",
     "EdgeMetricTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "GetDeploymentsRequestRequestTypeDef",
     "GetDeviceRegistrationRequestRequestTypeDef",
-    "GetDeviceRegistrationResultTypeDef",
-    "ResponseMetadataTypeDef",
     "DefinitionTypeDef",
     "DeploymentResultTypeDef",
     "ModelTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetDeviceRegistrationResultTypeDef",
     "EdgeDeploymentTypeDef",
     "SendHeartbeatRequestRequestTypeDef",
     "GetDeploymentsResultTypeDef",
 )
 
 ChecksumTypeDef = TypedDict(
     "ChecksumTypeDef",
@@ -74,18 +74,22 @@
         "MetricName": str,
         "Value": float,
         "Timestamp": Union[datetime, str],
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetDeploymentsRequestRequestTypeDef = TypedDict(
     "GetDeploymentsRequestRequestTypeDef",
     {
         "DeviceName": str,
@@ -97,34 +101,14 @@
     "GetDeviceRegistrationRequestRequestTypeDef",
     {
         "DeviceName": str,
         "DeviceFleetName": str,
     },
 )
 
-GetDeviceRegistrationResultTypeDef = TypedDict(
-    "GetDeviceRegistrationResultTypeDef",
-    {
-        "DeviceRegistration": str,
-        "CacheTTL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 DefinitionTypeDef = TypedDict(
     "DefinitionTypeDef",
     {
         "ModelHandle": str,
         "S3Url": str,
         "Checksum": ChecksumTypeDef,
         "State": ModelStateType,
@@ -153,14 +137,30 @@
         "LatestSampleTime": Union[datetime, str],
         "LatestInference": Union[datetime, str],
         "ModelMetrics": Sequence[EdgeMetricTypeDef],
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeviceRegistrationResultTypeDef = TypedDict(
+    "GetDeviceRegistrationResultTypeDef",
+    {
+        "DeviceRegistration": str,
+        "CacheTTL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 EdgeDeploymentTypeDef = TypedDict(
     "EdgeDeploymentTypeDef",
     {
         "DeploymentName": str,
         "Type": Literal["Model"],
         "FailureHandlingPolicy": FailureHandlingPolicyType,
         "Definitions": List[DefinitionTypeDef],
@@ -191,10 +191,10 @@
 ):
     pass
 
 GetDeploymentsResultTypeDef = TypedDict(
     "GetDeploymentsResultTypeDef",
     {
         "Deployments": List[EdgeDeploymentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge.egg-info/PKG-INFO` & `mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-edge
-Version: 1.28.0
-Summary: Type annotations for boto3.SagemakerEdgeManager 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SagemakerEdgeManager 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_edge/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sagemaker-edge"></a>
 
 # mypy-boto3-sagemaker-edge
 
 [![PyPI - mypy-boto3-sagemaker-edge](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-edge.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-edge)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-edge.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-edge)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_edge/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-edge?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-edge)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-edge)](https://pepy.tech/project/mypy-boto3-sagemaker-edge)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SagemakerEdgeManager 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
+[boto3.SagemakerEdgeManager 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
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
 [mypy-boto3-sagemaker-edge docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_edge/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,22 +305,22 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_edge.type_defs import (
     ChecksumTypeDef,
     DeploymentModelTypeDef,
     EdgeMetricTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetDeploymentsRequestRequestTypeDef,
     GetDeviceRegistrationRequestRequestTypeDef,
-    GetDeviceRegistrationResultTypeDef,
-    ResponseMetadataTypeDef,
     DefinitionTypeDef,
     DeploymentResultTypeDef,
     ModelTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDeviceRegistrationResultTypeDef,
     EdgeDeploymentTypeDef,
     SendHeartbeatRequestRequestTypeDef,
     GetDeploymentsResultTypeDef,
 )
 
 
 def get_structure() -> ChecksumTypeDef:
```

### Comparing `mypy-boto3-sagemaker-edge-1.28.0/mypy_boto3_sagemaker_edge.egg-info/SOURCES.txt` & `mypy-boto3-sagemaker-edge-1.28.12/mypy_boto3_sagemaker_edge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-edge-1.28.0/setup.py` & `mypy-boto3-sagemaker-edge-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker-edge",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_sagemaker_edge"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SagemakerEdgeManager 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SagemakerEdgeManager 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

