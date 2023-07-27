# Comparing `tmp/mypy-boto3-simspaceweaver-1.28.0.tar.gz` & `tmp/mypy-boto3-simspaceweaver-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-simspaceweaver-1.28.0.tar", last modified: Thu Jul  6 21:00:39 2023, max compression
+gzip compressed data, was "mypy-boto3-simspaceweaver-1.28.12.tar", last modified: Thu Jul 27 11:49:41 2023, max compression
```

## Comparing `mypy-boto3-simspaceweaver-1.28.0.tar` & `mypy-boto3-simspaceweaver-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:39.526435 mypy-boto3-simspaceweaver-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:56:01.000000 mypy-boto3-simspaceweaver-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13606 2023-07-06 21:00:39.518435 mypy-boto3-simspaceweaver-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-07-06 20:56:01.000000 mypy-boto3-simspaceweaver-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:39.506435 mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-06 20:56:01.000000 mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-06 20:56:01.000000 mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 20:56:01.000000 mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-07-06 20:56:01.000000 mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-06 20:56:01.000000 mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-07-06 20:56:01.000000 mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-07-06 20:56:01.000000 mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:56:01.000000 mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-07-06 20:56:02.000000 mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-07-06 20:56:02.000000 mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:56:01.000000 mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:39.518435 mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13606 2023-07-06 21:00:39.000000 mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-06 21:00:39.000000 mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:39.000000 mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:39.000000 mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:39.000000 mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 21:00:39.000000 mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:39.526435 mypy-boto3-simspaceweaver-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-06 20:56:01.000000 mypy-boto3-simspaceweaver-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.045314 mypy-boto3-simspaceweaver-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-07-27 11:49:41.045314 mypy-boto3-simspaceweaver-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.045314 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-07-27 11:47:02.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.045314 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-07-27 11:49:40.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-27 11:49:40.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:40.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:40.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:40.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 11:49:40.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:41.045314 mypy-boto3-simspaceweaver-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/setup.py
```

### Comparing `mypy-boto3-simspaceweaver-1.28.0/LICENSE` & `mypy-boto3-simspaceweaver-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-simspaceweaver-1.28.0/PKG-INFO` & `mypy-boto3-simspaceweaver-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-simspaceweaver
-Version: 1.28.0
-Summary: Type annotations for boto3.SimSpaceWeaver 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SimSpaceWeaver 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-simspaceweaver"></a>
 
 # mypy-boto3-simspaceweaver
 
 [![PyPI - mypy-boto3-simspaceweaver](https://img.shields.io/pypi/v/mypy-boto3-simspaceweaver.svg?color=blue)](https://pypi.org/project/mypy-boto3-simspaceweaver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-simspaceweaver.svg?color=blue)](https://pypi.org/project/mypy-boto3-simspaceweaver)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-simspaceweaver?color=blue)](https://pypistats.org/packages/mypy-boto3-simspaceweaver)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-simspaceweaver)](https://pepy.tech/project/mypy-boto3-simspaceweaver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SimSpaceWeaver 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
+[boto3.SimSpaceWeaver 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
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
 [mypy-boto3-simspaceweaver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/).
 
 See how it helps to find and fix potential bugs:
 
@@ -309,42 +309,44 @@
 ```python
 from mypy_boto3_simspaceweaver.type_defs import (
     CloudWatchLogsLogGroupTypeDef,
     S3DestinationTypeDef,
     DeleteAppInputRequestTypeDef,
     DeleteSimulationInputRequestTypeDef,
     DescribeAppInputRequestTypeDef,
-    LaunchOverridesTypeDef,
+    LaunchOverridesOutputTypeDef,
+    ResponseMetadataTypeDef,
     DescribeSimulationInputRequestTypeDef,
-    S3LocationTypeDef,
+    S3LocationOutputTypeDef,
     DomainTypeDef,
+    LaunchOverridesTypeDef,
     ListAppsInputRequestTypeDef,
     SimulationAppMetadataTypeDef,
     ListSimulationsInputRequestTypeDef,
     SimulationMetadataTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     SimulationClockTypeDef,
-    ResponseMetadataTypeDef,
+    S3LocationTypeDef,
     SimulationAppPortMappingTypeDef,
-    StartAppOutputTypeDef,
     StartClockInputRequestTypeDef,
-    StartSimulationOutputTypeDef,
     StopAppInputRequestTypeDef,
     StopClockInputRequestTypeDef,
     StopSimulationInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     LogDestinationTypeDef,
     CreateSnapshotInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    StartAppOutputTypeDef,
+    StartSimulationOutputTypeDef,
     StartAppInputRequestTypeDef,
-    StartSimulationInputRequestTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
     LiveSimulationStateTypeDef,
+    StartSimulationInputRequestTypeDef,
     SimulationAppEndpointInfoTypeDef,
     LoggingConfigurationTypeDef,
     DescribeAppOutputTypeDef,
     DescribeSimulationOutputTypeDef,
 )
```

### Comparing `mypy-boto3-simspaceweaver-1.28.0/README.md` & `mypy-boto3-simspaceweaver-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-simspaceweaver"></a>
 
 # mypy-boto3-simspaceweaver
 
 [![PyPI - mypy-boto3-simspaceweaver](https://img.shields.io/pypi/v/mypy-boto3-simspaceweaver.svg?color=blue)](https://pypi.org/project/mypy-boto3-simspaceweaver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-simspaceweaver.svg?color=blue)](https://pypi.org/project/mypy-boto3-simspaceweaver)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-simspaceweaver?color=blue)](https://pypistats.org/packages/mypy-boto3-simspaceweaver)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-simspaceweaver)](https://pepy.tech/project/mypy-boto3-simspaceweaver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SimSpaceWeaver 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
+[boto3.SimSpaceWeaver 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
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
 [mypy-boto3-simspaceweaver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/).
 
 See how it helps to find and fix potential bugs:
 
@@ -277,42 +277,44 @@
 ```python
 from mypy_boto3_simspaceweaver.type_defs import (
     CloudWatchLogsLogGroupTypeDef,
     S3DestinationTypeDef,
     DeleteAppInputRequestTypeDef,
     DeleteSimulationInputRequestTypeDef,
     DescribeAppInputRequestTypeDef,
-    LaunchOverridesTypeDef,
+    LaunchOverridesOutputTypeDef,
+    ResponseMetadataTypeDef,
     DescribeSimulationInputRequestTypeDef,
-    S3LocationTypeDef,
+    S3LocationOutputTypeDef,
     DomainTypeDef,
+    LaunchOverridesTypeDef,
     ListAppsInputRequestTypeDef,
     SimulationAppMetadataTypeDef,
     ListSimulationsInputRequestTypeDef,
     SimulationMetadataTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     SimulationClockTypeDef,
-    ResponseMetadataTypeDef,
+    S3LocationTypeDef,
     SimulationAppPortMappingTypeDef,
-    StartAppOutputTypeDef,
     StartClockInputRequestTypeDef,
-    StartSimulationOutputTypeDef,
     StopAppInputRequestTypeDef,
     StopClockInputRequestTypeDef,
     StopSimulationInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     LogDestinationTypeDef,
     CreateSnapshotInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    StartAppOutputTypeDef,
+    StartSimulationOutputTypeDef,
     StartAppInputRequestTypeDef,
-    StartSimulationInputRequestTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
     LiveSimulationStateTypeDef,
+    StartSimulationInputRequestTypeDef,
     SimulationAppEndpointInfoTypeDef,
     LoggingConfigurationTypeDef,
     DescribeAppOutputTypeDef,
     DescribeSimulationOutputTypeDef,
 )
```

### Comparing `mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver/__main__.py` & `mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SimSpaceWeaver 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.SimSpaceWeaver 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver\nOther"
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

### Comparing `mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver/client.py` & `mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver/client.pyi` & `mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver/literals.py` & `mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,14 +169,15 @@
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
@@ -255,26 +256,28 @@
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

### Comparing `mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver/literals.pyi` & `mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -167,14 +167,15 @@
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
@@ -253,26 +254,28 @@
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

### Comparing `mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver/type_defs.py` & `mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,42 +33,44 @@
 
 __all__ = (
     "CloudWatchLogsLogGroupTypeDef",
     "S3DestinationTypeDef",
     "DeleteAppInputRequestTypeDef",
     "DeleteSimulationInputRequestTypeDef",
     "DescribeAppInputRequestTypeDef",
-    "LaunchOverridesTypeDef",
+    "LaunchOverridesOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeSimulationInputRequestTypeDef",
-    "S3LocationTypeDef",
+    "S3LocationOutputTypeDef",
     "DomainTypeDef",
+    "LaunchOverridesTypeDef",
     "ListAppsInputRequestTypeDef",
     "SimulationAppMetadataTypeDef",
     "ListSimulationsInputRequestTypeDef",
     "SimulationMetadataTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "SimulationClockTypeDef",
-    "ResponseMetadataTypeDef",
+    "S3LocationTypeDef",
     "SimulationAppPortMappingTypeDef",
-    "StartAppOutputTypeDef",
     "StartClockInputRequestTypeDef",
-    "StartSimulationOutputTypeDef",
     "StopAppInputRequestTypeDef",
     "StopClockInputRequestTypeDef",
     "StopSimulationInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "LogDestinationTypeDef",
     "CreateSnapshotInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "StartAppOutputTypeDef",
+    "StartSimulationOutputTypeDef",
     "StartAppInputRequestTypeDef",
-    "StartSimulationInputRequestTypeDef",
     "ListAppsOutputTypeDef",
     "ListSimulationsOutputTypeDef",
     "LiveSimulationStateTypeDef",
+    "StartSimulationInputRequestTypeDef",
     "SimulationAppEndpointInfoTypeDef",
     "LoggingConfigurationTypeDef",
     "DescribeAppOutputTypeDef",
     "DescribeSimulationOutputTypeDef",
 )
 
 CloudWatchLogsLogGroupTypeDef = TypedDict(
@@ -109,31 +111,42 @@
     {
         "App": str,
         "Domain": str,
         "Simulation": str,
     },
 )
 
-LaunchOverridesTypeDef = TypedDict(
-    "LaunchOverridesTypeDef",
+LaunchOverridesOutputTypeDef = TypedDict(
+    "LaunchOverridesOutputTypeDef",
     {
         "LaunchCommands": List[str],
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 DescribeSimulationInputRequestTypeDef = TypedDict(
     "DescribeSimulationInputRequestTypeDef",
     {
         "Simulation": str,
     },
 )
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
+S3LocationOutputTypeDef = TypedDict(
+    "S3LocationOutputTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
     total=False,
 )
 
@@ -142,14 +155,22 @@
     {
         "Lifecycle": LifecycleManagementStrategyType,
         "Name": str,
     },
     total=False,
 )
 
+LaunchOverridesTypeDef = TypedDict(
+    "LaunchOverridesTypeDef",
+    {
+        "LaunchCommands": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredListAppsInputRequestTypeDef = TypedDict(
     "_RequiredListAppsInputRequestTypeDef",
     {
         "Simulation": str,
     },
 )
 _OptionalListAppsInputRequestTypeDef = TypedDict(
@@ -205,78 +226,48 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SimulationClockTypeDef = TypedDict(
     "SimulationClockTypeDef",
     {
         "Status": ClockStatusType,
         "TargetStatus": ClockTargetStatusType,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "BucketName": str,
+        "ObjectKey": str,
     },
+    total=False,
 )
 
 SimulationAppPortMappingTypeDef = TypedDict(
     "SimulationAppPortMappingTypeDef",
     {
         "Actual": int,
         "Declared": int,
     },
     total=False,
 )
 
-StartAppOutputTypeDef = TypedDict(
-    "StartAppOutputTypeDef",
-    {
-        "Domain": str,
-        "Name": str,
-        "Simulation": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartClockInputRequestTypeDef = TypedDict(
     "StartClockInputRequestTypeDef",
     {
         "Simulation": str,
     },
 )
 
-StartSimulationOutputTypeDef = TypedDict(
-    "StartSimulationOutputTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "ExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopAppInputRequestTypeDef = TypedDict(
     "StopAppInputRequestTypeDef",
     {
         "App": str,
         "Domain": str,
         "Simulation": str,
     },
@@ -324,14 +315,42 @@
     "CreateSnapshotInputRequestTypeDef",
     {
         "Destination": S3DestinationTypeDef,
         "Simulation": str,
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAppOutputTypeDef = TypedDict(
+    "StartAppOutputTypeDef",
+    {
+        "Domain": str,
+        "Name": str,
+        "Simulation": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSimulationOutputTypeDef = TypedDict(
+    "StartSimulationOutputTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
+        "ExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredStartAppInputRequestTypeDef = TypedDict(
     "_RequiredStartAppInputRequestTypeDef",
     {
         "Domain": str,
         "Name": str,
         "Simulation": str,
     },
@@ -349,14 +368,41 @@
 
 class StartAppInputRequestTypeDef(
     _RequiredStartAppInputRequestTypeDef, _OptionalStartAppInputRequestTypeDef
 ):
     pass
 
 
+ListAppsOutputTypeDef = TypedDict(
+    "ListAppsOutputTypeDef",
+    {
+        "Apps": List[SimulationAppMetadataTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSimulationsOutputTypeDef = TypedDict(
+    "ListSimulationsOutputTypeDef",
+    {
+        "NextToken": str,
+        "Simulations": List[SimulationMetadataTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LiveSimulationStateTypeDef = TypedDict(
+    "LiveSimulationStateTypeDef",
+    {
+        "Clocks": List[SimulationClockTypeDef],
+        "Domains": List[DomainTypeDef],
+    },
+    total=False,
+)
+
 _RequiredStartSimulationInputRequestTypeDef = TypedDict(
     "_RequiredStartSimulationInputRequestTypeDef",
     {
         "Name": str,
         "RoleArn": str,
     },
 )
@@ -376,41 +422,14 @@
 
 class StartSimulationInputRequestTypeDef(
     _RequiredStartSimulationInputRequestTypeDef, _OptionalStartSimulationInputRequestTypeDef
 ):
     pass
 
 
-ListAppsOutputTypeDef = TypedDict(
-    "ListAppsOutputTypeDef",
-    {
-        "Apps": List[SimulationAppMetadataTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSimulationsOutputTypeDef = TypedDict(
-    "ListSimulationsOutputTypeDef",
-    {
-        "NextToken": str,
-        "Simulations": List[SimulationMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LiveSimulationStateTypeDef = TypedDict(
-    "LiveSimulationStateTypeDef",
-    {
-        "Clocks": List[SimulationClockTypeDef],
-        "Domains": List[DomainTypeDef],
-    },
-    total=False,
-)
-
 SimulationAppEndpointInfoTypeDef = TypedDict(
     "SimulationAppEndpointInfoTypeDef",
     {
         "Address": str,
         "IngressPortMappings": List[SimulationAppPortMappingTypeDef],
     },
     total=False,
@@ -426,20 +445,20 @@
 
 DescribeAppOutputTypeDef = TypedDict(
     "DescribeAppOutputTypeDef",
     {
         "Description": str,
         "Domain": str,
         "EndpointInfo": SimulationAppEndpointInfoTypeDef,
-        "LaunchOverrides": LaunchOverridesTypeDef,
+        "LaunchOverrides": LaunchOverridesOutputTypeDef,
         "Name": str,
         "Simulation": str,
         "Status": SimulationAppStatusType,
         "TargetStatus": SimulationAppTargetStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSimulationOutputTypeDef = TypedDict(
     "DescribeSimulationOutputTypeDef",
     {
         "Arn": str,
@@ -448,15 +467,15 @@
         "ExecutionId": str,
         "LiveSimulationState": LiveSimulationStateTypeDef,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
         "MaximumDuration": str,
         "Name": str,
         "RoleArn": str,
         "SchemaError": str,
-        "SchemaS3Location": S3LocationTypeDef,
-        "SnapshotS3Location": S3LocationTypeDef,
+        "SchemaS3Location": S3LocationOutputTypeDef,
+        "SnapshotS3Location": S3LocationOutputTypeDef,
         "StartError": str,
         "Status": SimulationStatusType,
         "TargetStatus": SimulationTargetStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver/type_defs.pyi` & `mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -32,42 +32,44 @@
 
 __all__ = (
     "CloudWatchLogsLogGroupTypeDef",
     "S3DestinationTypeDef",
     "DeleteAppInputRequestTypeDef",
     "DeleteSimulationInputRequestTypeDef",
     "DescribeAppInputRequestTypeDef",
-    "LaunchOverridesTypeDef",
+    "LaunchOverridesOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeSimulationInputRequestTypeDef",
-    "S3LocationTypeDef",
+    "S3LocationOutputTypeDef",
     "DomainTypeDef",
+    "LaunchOverridesTypeDef",
     "ListAppsInputRequestTypeDef",
     "SimulationAppMetadataTypeDef",
     "ListSimulationsInputRequestTypeDef",
     "SimulationMetadataTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "SimulationClockTypeDef",
-    "ResponseMetadataTypeDef",
+    "S3LocationTypeDef",
     "SimulationAppPortMappingTypeDef",
-    "StartAppOutputTypeDef",
     "StartClockInputRequestTypeDef",
-    "StartSimulationOutputTypeDef",
     "StopAppInputRequestTypeDef",
     "StopClockInputRequestTypeDef",
     "StopSimulationInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "LogDestinationTypeDef",
     "CreateSnapshotInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "StartAppOutputTypeDef",
+    "StartSimulationOutputTypeDef",
     "StartAppInputRequestTypeDef",
-    "StartSimulationInputRequestTypeDef",
     "ListAppsOutputTypeDef",
     "ListSimulationsOutputTypeDef",
     "LiveSimulationStateTypeDef",
+    "StartSimulationInputRequestTypeDef",
     "SimulationAppEndpointInfoTypeDef",
     "LoggingConfigurationTypeDef",
     "DescribeAppOutputTypeDef",
     "DescribeSimulationOutputTypeDef",
 )
 
 CloudWatchLogsLogGroupTypeDef = TypedDict(
@@ -108,31 +110,42 @@
     {
         "App": str,
         "Domain": str,
         "Simulation": str,
     },
 )
 
-LaunchOverridesTypeDef = TypedDict(
-    "LaunchOverridesTypeDef",
+LaunchOverridesOutputTypeDef = TypedDict(
+    "LaunchOverridesOutputTypeDef",
     {
         "LaunchCommands": List[str],
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 DescribeSimulationInputRequestTypeDef = TypedDict(
     "DescribeSimulationInputRequestTypeDef",
     {
         "Simulation": str,
     },
 )
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
+S3LocationOutputTypeDef = TypedDict(
+    "S3LocationOutputTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
     total=False,
 )
 
@@ -141,14 +154,22 @@
     {
         "Lifecycle": LifecycleManagementStrategyType,
         "Name": str,
     },
     total=False,
 )
 
+LaunchOverridesTypeDef = TypedDict(
+    "LaunchOverridesTypeDef",
+    {
+        "LaunchCommands": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredListAppsInputRequestTypeDef = TypedDict(
     "_RequiredListAppsInputRequestTypeDef",
     {
         "Simulation": str,
     },
 )
 _OptionalListAppsInputRequestTypeDef = TypedDict(
@@ -202,78 +223,48 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SimulationClockTypeDef = TypedDict(
     "SimulationClockTypeDef",
     {
         "Status": ClockStatusType,
         "TargetStatus": ClockTargetStatusType,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "BucketName": str,
+        "ObjectKey": str,
     },
+    total=False,
 )
 
 SimulationAppPortMappingTypeDef = TypedDict(
     "SimulationAppPortMappingTypeDef",
     {
         "Actual": int,
         "Declared": int,
     },
     total=False,
 )
 
-StartAppOutputTypeDef = TypedDict(
-    "StartAppOutputTypeDef",
-    {
-        "Domain": str,
-        "Name": str,
-        "Simulation": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartClockInputRequestTypeDef = TypedDict(
     "StartClockInputRequestTypeDef",
     {
         "Simulation": str,
     },
 )
 
-StartSimulationOutputTypeDef = TypedDict(
-    "StartSimulationOutputTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "ExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopAppInputRequestTypeDef = TypedDict(
     "StopAppInputRequestTypeDef",
     {
         "App": str,
         "Domain": str,
         "Simulation": str,
     },
@@ -321,89 +312,117 @@
     "CreateSnapshotInputRequestTypeDef",
     {
         "Destination": S3DestinationTypeDef,
         "Simulation": str,
     },
 )
 
-_RequiredStartAppInputRequestTypeDef = TypedDict(
-    "_RequiredStartAppInputRequestTypeDef",
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAppOutputTypeDef = TypedDict(
+    "StartAppOutputTypeDef",
     {
         "Domain": str,
         "Name": str,
         "Simulation": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStartAppInputRequestTypeDef = TypedDict(
-    "_OptionalStartAppInputRequestTypeDef",
+
+StartSimulationOutputTypeDef = TypedDict(
+    "StartSimulationOutputTypeDef",
     {
-        "ClientToken": str,
-        "Description": str,
-        "LaunchOverrides": LaunchOverridesTypeDef,
+        "Arn": str,
+        "CreationTime": datetime,
+        "ExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class StartAppInputRequestTypeDef(
-    _RequiredStartAppInputRequestTypeDef, _OptionalStartAppInputRequestTypeDef
-):
-    pass
-
-_RequiredStartSimulationInputRequestTypeDef = TypedDict(
-    "_RequiredStartSimulationInputRequestTypeDef",
+_RequiredStartAppInputRequestTypeDef = TypedDict(
+    "_RequiredStartAppInputRequestTypeDef",
     {
+        "Domain": str,
         "Name": str,
-        "RoleArn": str,
+        "Simulation": str,
     },
 )
-_OptionalStartSimulationInputRequestTypeDef = TypedDict(
-    "_OptionalStartSimulationInputRequestTypeDef",
+_OptionalStartAppInputRequestTypeDef = TypedDict(
+    "_OptionalStartAppInputRequestTypeDef",
     {
         "ClientToken": str,
         "Description": str,
-        "MaximumDuration": str,
-        "SchemaS3Location": S3LocationTypeDef,
-        "SnapshotS3Location": S3LocationTypeDef,
-        "Tags": Mapping[str, str],
+        "LaunchOverrides": LaunchOverridesTypeDef,
     },
     total=False,
 )
 
-class StartSimulationInputRequestTypeDef(
-    _RequiredStartSimulationInputRequestTypeDef, _OptionalStartSimulationInputRequestTypeDef
+class StartAppInputRequestTypeDef(
+    _RequiredStartAppInputRequestTypeDef, _OptionalStartAppInputRequestTypeDef
 ):
     pass
 
 ListAppsOutputTypeDef = TypedDict(
     "ListAppsOutputTypeDef",
     {
         "Apps": List[SimulationAppMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSimulationsOutputTypeDef = TypedDict(
     "ListSimulationsOutputTypeDef",
     {
         "NextToken": str,
         "Simulations": List[SimulationMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LiveSimulationStateTypeDef = TypedDict(
     "LiveSimulationStateTypeDef",
     {
         "Clocks": List[SimulationClockTypeDef],
         "Domains": List[DomainTypeDef],
     },
     total=False,
 )
 
+_RequiredStartSimulationInputRequestTypeDef = TypedDict(
+    "_RequiredStartSimulationInputRequestTypeDef",
+    {
+        "Name": str,
+        "RoleArn": str,
+    },
+)
+_OptionalStartSimulationInputRequestTypeDef = TypedDict(
+    "_OptionalStartSimulationInputRequestTypeDef",
+    {
+        "ClientToken": str,
+        "Description": str,
+        "MaximumDuration": str,
+        "SchemaS3Location": S3LocationTypeDef,
+        "SnapshotS3Location": S3LocationTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class StartSimulationInputRequestTypeDef(
+    _RequiredStartSimulationInputRequestTypeDef, _OptionalStartSimulationInputRequestTypeDef
+):
+    pass
+
 SimulationAppEndpointInfoTypeDef = TypedDict(
     "SimulationAppEndpointInfoTypeDef",
     {
         "Address": str,
         "IngressPortMappings": List[SimulationAppPortMappingTypeDef],
     },
     total=False,
@@ -419,20 +438,20 @@
 
 DescribeAppOutputTypeDef = TypedDict(
     "DescribeAppOutputTypeDef",
     {
         "Description": str,
         "Domain": str,
         "EndpointInfo": SimulationAppEndpointInfoTypeDef,
-        "LaunchOverrides": LaunchOverridesTypeDef,
+        "LaunchOverrides": LaunchOverridesOutputTypeDef,
         "Name": str,
         "Simulation": str,
         "Status": SimulationAppStatusType,
         "TargetStatus": SimulationAppTargetStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSimulationOutputTypeDef = TypedDict(
     "DescribeSimulationOutputTypeDef",
     {
         "Arn": str,
@@ -441,15 +460,15 @@
         "ExecutionId": str,
         "LiveSimulationState": LiveSimulationStateTypeDef,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
         "MaximumDuration": str,
         "Name": str,
         "RoleArn": str,
         "SchemaError": str,
-        "SchemaS3Location": S3LocationTypeDef,
-        "SnapshotS3Location": S3LocationTypeDef,
+        "SchemaS3Location": S3LocationOutputTypeDef,
+        "SnapshotS3Location": S3LocationOutputTypeDef,
         "StartError": str,
         "Status": SimulationStatusType,
         "TargetStatus": SimulationTargetStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver.egg-info/PKG-INFO` & `mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-simspaceweaver
-Version: 1.28.0
-Summary: Type annotations for boto3.SimSpaceWeaver 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SimSpaceWeaver 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-simspaceweaver"></a>
 
 # mypy-boto3-simspaceweaver
 
 [![PyPI - mypy-boto3-simspaceweaver](https://img.shields.io/pypi/v/mypy-boto3-simspaceweaver.svg?color=blue)](https://pypi.org/project/mypy-boto3-simspaceweaver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-simspaceweaver.svg?color=blue)](https://pypi.org/project/mypy-boto3-simspaceweaver)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-simspaceweaver?color=blue)](https://pypistats.org/packages/mypy-boto3-simspaceweaver)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-simspaceweaver)](https://pepy.tech/project/mypy-boto3-simspaceweaver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SimSpaceWeaver 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
+[boto3.SimSpaceWeaver 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
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
 [mypy-boto3-simspaceweaver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/).
 
 See how it helps to find and fix potential bugs:
 
@@ -309,42 +309,44 @@
 ```python
 from mypy_boto3_simspaceweaver.type_defs import (
     CloudWatchLogsLogGroupTypeDef,
     S3DestinationTypeDef,
     DeleteAppInputRequestTypeDef,
     DeleteSimulationInputRequestTypeDef,
     DescribeAppInputRequestTypeDef,
-    LaunchOverridesTypeDef,
+    LaunchOverridesOutputTypeDef,
+    ResponseMetadataTypeDef,
     DescribeSimulationInputRequestTypeDef,
-    S3LocationTypeDef,
+    S3LocationOutputTypeDef,
     DomainTypeDef,
+    LaunchOverridesTypeDef,
     ListAppsInputRequestTypeDef,
     SimulationAppMetadataTypeDef,
     ListSimulationsInputRequestTypeDef,
     SimulationMetadataTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     SimulationClockTypeDef,
-    ResponseMetadataTypeDef,
+    S3LocationTypeDef,
     SimulationAppPortMappingTypeDef,
-    StartAppOutputTypeDef,
     StartClockInputRequestTypeDef,
-    StartSimulationOutputTypeDef,
     StopAppInputRequestTypeDef,
     StopClockInputRequestTypeDef,
     StopSimulationInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     LogDestinationTypeDef,
     CreateSnapshotInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    StartAppOutputTypeDef,
+    StartSimulationOutputTypeDef,
     StartAppInputRequestTypeDef,
-    StartSimulationInputRequestTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
     LiveSimulationStateTypeDef,
+    StartSimulationInputRequestTypeDef,
     SimulationAppEndpointInfoTypeDef,
     LoggingConfigurationTypeDef,
     DescribeAppOutputTypeDef,
     DescribeSimulationOutputTypeDef,
 )
```

### Comparing `mypy-boto3-simspaceweaver-1.28.0/mypy_boto3_simspaceweaver.egg-info/SOURCES.txt` & `mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-simspaceweaver-1.28.0/setup.py` & `mypy-boto3-simspaceweaver-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-simspaceweaver",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_simspaceweaver"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SimSpaceWeaver 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.SimSpaceWeaver 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

