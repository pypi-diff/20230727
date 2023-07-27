# Comparing `tmp/mypy-boto3-internetmonitor-1.28.0.tar.gz` & `tmp/mypy-boto3-internetmonitor-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-internetmonitor-1.28.0.tar", last modified: Thu Jul  6 20:59:44 2023, max compression
+gzip compressed data, was "mypy-boto3-internetmonitor-1.28.12.tar", last modified: Thu Jul 27 05:34:47 2023, max compression
```

## Comparing `mypy-boto3-internetmonitor-1.28.0.tar` & `mypy-boto3-internetmonitor-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:44.874323 mypy-boto3-internetmonitor-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:43:10.000000 mypy-boto3-internetmonitor-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-07-06 20:59:44.870324 mypy-boto3-internetmonitor-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-07-06 20:43:10.000000 mypy-boto3-internetmonitor-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:44.862323 mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-06 20:43:10.000000 mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-06 20:43:10.000000 mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-06 20:43:10.000000 mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-07-06 20:43:10.000000 mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-07-06 20:43:10.000000 mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-07-06 20:43:10.000000 mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-07-06 20:43:10.000000 mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-06 20:43:10.000000 mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-06 20:43:10.000000 mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:43:10.000000 mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-07-06 20:43:10.000000 mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-07-06 20:43:10.000000 mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:43:10.000000 mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:44.870324 mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-07-06 20:59:44.000000 mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-06 20:59:44.000000 mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:44.000000 mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:44.000000 mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:44.000000 mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 20:59:44.000000 mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:44.874323 mypy-boto3-internetmonitor-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-06 20:43:10.000000 mypy-boto3-internetmonitor-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.560489 mypy-boto3-internetmonitor-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-07-27 05:34:47.560489 mypy-boto3-internetmonitor-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.556489 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13341 2023-07-27 05:23:40.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-07-27 05:23:40.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.560489 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-07-27 05:34:47.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-27 05:34:47.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:47.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:47.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:47.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 05:34:47.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:47.560489 mypy-boto3-internetmonitor-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-27 05:23:38.000000 mypy-boto3-internetmonitor-1.28.12/setup.py
```

### Comparing `mypy-boto3-internetmonitor-1.28.0/LICENSE` & `mypy-boto3-internetmonitor-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.0/PKG-INFO` & `mypy-boto3-internetmonitor-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-internetmonitor
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudWatchInternetMonitor 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudWatchInternetMonitor 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-internetmonitor"></a>
 
 # mypy-boto3-internetmonitor
 
 [![PyPI - mypy-boto3-internetmonitor](https://img.shields.io/pypi/v/mypy-boto3-internetmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-internetmonitor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-internetmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-internetmonitor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-internetmonitor?color=blue)](https://pypistats.org/packages/mypy-boto3-internetmonitor)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-internetmonitor)](https://pepy.tech/project/mypy-boto3-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchInternetMonitor 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
+[boto3.CloudWatchInternetMonitor 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
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
 [mypy-boto3-internetmonitor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,14 +334,16 @@
 from mypy_boto3_internetmonitor.type_defs import (
     AvailabilityMeasurementTypeDef,
     HealthEventsConfigTypeDef,
     CreateMonitorOutputTypeDef,
     DeleteMonitorInputRequestTypeDef,
     GetHealthEventInputRequestTypeDef,
     GetMonitorInputRequestTypeDef,
+    HealthEventsConfigOutputTypeDef,
+    S3ConfigOutputTypeDef,
     S3ConfigTypeDef,
     ListHealthEventsInputListHealthEventsPaginateTypeDef,
     ListHealthEventsInputRequestTypeDef,
     ListMonitorsInputListMonitorsPaginateTypeDef,
     ListMonitorsInputRequestTypeDef,
     MonitorTypeDef,
     ListTagsForResourceInputRequestTypeDef,
@@ -349,20 +351,21 @@
     NetworkTypeDef,
     PaginatorConfigTypeDef,
     RoundTripTimeTypeDef,
     ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateMonitorOutputTypeDef,
+    InternetMeasurementsLogDeliveryOutputTypeDef,
     InternetMeasurementsLogDeliveryTypeDef,
     ListMonitorsOutputTypeDef,
     NetworkImpairmentTypeDef,
     PerformanceMeasurementTypeDef,
-    CreateMonitorInputRequestTypeDef,
     GetMonitorOutputTypeDef,
+    CreateMonitorInputRequestTypeDef,
     UpdateMonitorInputRequestTypeDef,
     InternetHealthTypeDef,
     ImpactedLocationTypeDef,
     GetHealthEventOutputTypeDef,
     HealthEventTypeDef,
     ListHealthEventsOutputTypeDef,
 )
```

### Comparing `mypy-boto3-internetmonitor-1.28.0/README.md` & `mypy-boto3-internetmonitor-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-internetmonitor"></a>
 
 # mypy-boto3-internetmonitor
 
 [![PyPI - mypy-boto3-internetmonitor](https://img.shields.io/pypi/v/mypy-boto3-internetmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-internetmonitor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-internetmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-internetmonitor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-internetmonitor?color=blue)](https://pypistats.org/packages/mypy-boto3-internetmonitor)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-internetmonitor)](https://pepy.tech/project/mypy-boto3-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchInternetMonitor 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
+[boto3.CloudWatchInternetMonitor 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
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
 [mypy-boto3-internetmonitor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,14 +302,16 @@
 from mypy_boto3_internetmonitor.type_defs import (
     AvailabilityMeasurementTypeDef,
     HealthEventsConfigTypeDef,
     CreateMonitorOutputTypeDef,
     DeleteMonitorInputRequestTypeDef,
     GetHealthEventInputRequestTypeDef,
     GetMonitorInputRequestTypeDef,
+    HealthEventsConfigOutputTypeDef,
+    S3ConfigOutputTypeDef,
     S3ConfigTypeDef,
     ListHealthEventsInputListHealthEventsPaginateTypeDef,
     ListHealthEventsInputRequestTypeDef,
     ListMonitorsInputListMonitorsPaginateTypeDef,
     ListMonitorsInputRequestTypeDef,
     MonitorTypeDef,
     ListTagsForResourceInputRequestTypeDef,
@@ -317,20 +319,21 @@
     NetworkTypeDef,
     PaginatorConfigTypeDef,
     RoundTripTimeTypeDef,
     ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateMonitorOutputTypeDef,
+    InternetMeasurementsLogDeliveryOutputTypeDef,
     InternetMeasurementsLogDeliveryTypeDef,
     ListMonitorsOutputTypeDef,
     NetworkImpairmentTypeDef,
     PerformanceMeasurementTypeDef,
-    CreateMonitorInputRequestTypeDef,
     GetMonitorOutputTypeDef,
+    CreateMonitorInputRequestTypeDef,
     UpdateMonitorInputRequestTypeDef,
     InternetHealthTypeDef,
     ImpactedLocationTypeDef,
     GetHealthEventOutputTypeDef,
     HealthEventTypeDef,
     ListHealthEventsOutputTypeDef,
 )
```

### Comparing `mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/__init__.py` & `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/__init__.pyi` & `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/__main__.py` & `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatchInternetMonitor 1.28.0\nVersion:        "
-        " 1.28.0\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.CloudWatchInternetMonitor 1.28.12\nVersion:        "
+        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor\nOther"
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

### Comparing `mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/client.py` & `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/client.pyi` & `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/literals.py` & `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/literals.py`

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
@@ -418,24 +421,31 @@
 ]
 PaginatorName = Literal["list_health_events", "list_monitors"]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
+    "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/literals.pyi` & `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -165,14 +165,15 @@
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
@@ -251,26 +252,28 @@
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
@@ -416,24 +419,31 @@
 ]
 PaginatorName = Literal["list_health_events", "list_monitors"]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
+    "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/paginator.py` & `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/paginator.pyi` & `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/type_defs.py` & `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 __all__ = (
     "AvailabilityMeasurementTypeDef",
     "HealthEventsConfigTypeDef",
     "CreateMonitorOutputTypeDef",
     "DeleteMonitorInputRequestTypeDef",
     "GetHealthEventInputRequestTypeDef",
     "GetMonitorInputRequestTypeDef",
+    "HealthEventsConfigOutputTypeDef",
+    "S3ConfigOutputTypeDef",
     "S3ConfigTypeDef",
     "ListHealthEventsInputListHealthEventsPaginateTypeDef",
     "ListHealthEventsInputRequestTypeDef",
     "ListMonitorsInputListMonitorsPaginateTypeDef",
     "ListMonitorsInputRequestTypeDef",
     "MonitorTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
@@ -48,20 +50,21 @@
     "NetworkTypeDef",
     "PaginatorConfigTypeDef",
     "RoundTripTimeTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateMonitorOutputTypeDef",
+    "InternetMeasurementsLogDeliveryOutputTypeDef",
     "InternetMeasurementsLogDeliveryTypeDef",
     "ListMonitorsOutputTypeDef",
     "NetworkImpairmentTypeDef",
     "PerformanceMeasurementTypeDef",
-    "CreateMonitorInputRequestTypeDef",
     "GetMonitorOutputTypeDef",
+    "CreateMonitorInputRequestTypeDef",
     "UpdateMonitorInputRequestTypeDef",
     "InternetHealthTypeDef",
     "ImpactedLocationTypeDef",
     "GetHealthEventOutputTypeDef",
     "HealthEventTypeDef",
     "ListHealthEventsOutputTypeDef",
 )
@@ -112,14 +115,33 @@
 GetMonitorInputRequestTypeDef = TypedDict(
     "GetMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
     },
 )
 
+HealthEventsConfigOutputTypeDef = TypedDict(
+    "HealthEventsConfigOutputTypeDef",
+    {
+        "AvailabilityScoreThreshold": float,
+        "PerformanceScoreThreshold": float,
+    },
+    total=False,
+)
+
+S3ConfigOutputTypeDef = TypedDict(
+    "S3ConfigOutputTypeDef",
+    {
+        "BucketName": str,
+        "BucketPrefix": str,
+        "LogDeliveryStatus": LogDeliveryStatusType,
+    },
+    total=False,
+)
+
 S3ConfigTypeDef = TypedDict(
     "S3ConfigTypeDef",
     {
         "BucketName": str,
         "BucketPrefix": str,
         "LogDeliveryStatus": LogDeliveryStatusType,
     },
@@ -291,14 +313,22 @@
     {
         "MonitorArn": str,
         "Status": MonitorConfigStateType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+InternetMeasurementsLogDeliveryOutputTypeDef = TypedDict(
+    "InternetMeasurementsLogDeliveryOutputTypeDef",
+    {
+        "S3Config": S3ConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 InternetMeasurementsLogDeliveryTypeDef = TypedDict(
     "InternetMeasurementsLogDeliveryTypeDef",
     {
         "S3Config": S3ConfigTypeDef,
     },
     total=False,
 )
@@ -328,14 +358,34 @@
         "PercentOfTotalTrafficImpacted": float,
         "PercentOfClientLocationImpacted": float,
         "RoundTripTime": RoundTripTimeTypeDef,
     },
     total=False,
 )
 
+GetMonitorOutputTypeDef = TypedDict(
+    "GetMonitorOutputTypeDef",
+    {
+        "MonitorName": str,
+        "MonitorArn": str,
+        "Resources": List[str],
+        "Status": MonitorConfigStateType,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
+        "ProcessingStatus": MonitorProcessingStatusCodeType,
+        "ProcessingStatusInfo": str,
+        "Tags": Dict[str, str],
+        "MaxCityNetworksToMonitor": int,
+        "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryOutputTypeDef,
+        "TrafficPercentageToMonitor": int,
+        "HealthEventsConfig": HealthEventsConfigOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateMonitorInputRequestTypeDef = TypedDict(
     "_RequiredCreateMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
     },
 )
 _OptionalCreateMonitorInputRequestTypeDef = TypedDict(
@@ -355,34 +405,14 @@
 
 class CreateMonitorInputRequestTypeDef(
     _RequiredCreateMonitorInputRequestTypeDef, _OptionalCreateMonitorInputRequestTypeDef
 ):
     pass
 
 
-GetMonitorOutputTypeDef = TypedDict(
-    "GetMonitorOutputTypeDef",
-    {
-        "MonitorName": str,
-        "MonitorArn": str,
-        "Resources": List[str],
-        "Status": MonitorConfigStateType,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-        "ProcessingStatus": MonitorProcessingStatusCodeType,
-        "ProcessingStatusInfo": str,
-        "Tags": Dict[str, str],
-        "MaxCityNetworksToMonitor": int,
-        "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
-        "TrafficPercentageToMonitor": int,
-        "HealthEventsConfig": HealthEventsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateMonitorInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
     },
 )
 _OptionalUpdateMonitorInputRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor/type_defs.pyi` & `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 __all__ = (
     "AvailabilityMeasurementTypeDef",
     "HealthEventsConfigTypeDef",
     "CreateMonitorOutputTypeDef",
     "DeleteMonitorInputRequestTypeDef",
     "GetHealthEventInputRequestTypeDef",
     "GetMonitorInputRequestTypeDef",
+    "HealthEventsConfigOutputTypeDef",
+    "S3ConfigOutputTypeDef",
     "S3ConfigTypeDef",
     "ListHealthEventsInputListHealthEventsPaginateTypeDef",
     "ListHealthEventsInputRequestTypeDef",
     "ListMonitorsInputListMonitorsPaginateTypeDef",
     "ListMonitorsInputRequestTypeDef",
     "MonitorTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
@@ -47,20 +49,21 @@
     "NetworkTypeDef",
     "PaginatorConfigTypeDef",
     "RoundTripTimeTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateMonitorOutputTypeDef",
+    "InternetMeasurementsLogDeliveryOutputTypeDef",
     "InternetMeasurementsLogDeliveryTypeDef",
     "ListMonitorsOutputTypeDef",
     "NetworkImpairmentTypeDef",
     "PerformanceMeasurementTypeDef",
-    "CreateMonitorInputRequestTypeDef",
     "GetMonitorOutputTypeDef",
+    "CreateMonitorInputRequestTypeDef",
     "UpdateMonitorInputRequestTypeDef",
     "InternetHealthTypeDef",
     "ImpactedLocationTypeDef",
     "GetHealthEventOutputTypeDef",
     "HealthEventTypeDef",
     "ListHealthEventsOutputTypeDef",
 )
@@ -111,14 +114,33 @@
 GetMonitorInputRequestTypeDef = TypedDict(
     "GetMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
     },
 )
 
+HealthEventsConfigOutputTypeDef = TypedDict(
+    "HealthEventsConfigOutputTypeDef",
+    {
+        "AvailabilityScoreThreshold": float,
+        "PerformanceScoreThreshold": float,
+    },
+    total=False,
+)
+
+S3ConfigOutputTypeDef = TypedDict(
+    "S3ConfigOutputTypeDef",
+    {
+        "BucketName": str,
+        "BucketPrefix": str,
+        "LogDeliveryStatus": LogDeliveryStatusType,
+    },
+    total=False,
+)
+
 S3ConfigTypeDef = TypedDict(
     "S3ConfigTypeDef",
     {
         "BucketName": str,
         "BucketPrefix": str,
         "LogDeliveryStatus": LogDeliveryStatusType,
     },
@@ -284,14 +306,22 @@
     {
         "MonitorArn": str,
         "Status": MonitorConfigStateType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+InternetMeasurementsLogDeliveryOutputTypeDef = TypedDict(
+    "InternetMeasurementsLogDeliveryOutputTypeDef",
+    {
+        "S3Config": S3ConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 InternetMeasurementsLogDeliveryTypeDef = TypedDict(
     "InternetMeasurementsLogDeliveryTypeDef",
     {
         "S3Config": S3ConfigTypeDef,
     },
     total=False,
 )
@@ -321,14 +351,34 @@
         "PercentOfTotalTrafficImpacted": float,
         "PercentOfClientLocationImpacted": float,
         "RoundTripTime": RoundTripTimeTypeDef,
     },
     total=False,
 )
 
+GetMonitorOutputTypeDef = TypedDict(
+    "GetMonitorOutputTypeDef",
+    {
+        "MonitorName": str,
+        "MonitorArn": str,
+        "Resources": List[str],
+        "Status": MonitorConfigStateType,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
+        "ProcessingStatus": MonitorProcessingStatusCodeType,
+        "ProcessingStatusInfo": str,
+        "Tags": Dict[str, str],
+        "MaxCityNetworksToMonitor": int,
+        "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryOutputTypeDef,
+        "TrafficPercentageToMonitor": int,
+        "HealthEventsConfig": HealthEventsConfigOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateMonitorInputRequestTypeDef = TypedDict(
     "_RequiredCreateMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
     },
 )
 _OptionalCreateMonitorInputRequestTypeDef = TypedDict(
@@ -346,34 +396,14 @@
 )
 
 class CreateMonitorInputRequestTypeDef(
     _RequiredCreateMonitorInputRequestTypeDef, _OptionalCreateMonitorInputRequestTypeDef
 ):
     pass
 
-GetMonitorOutputTypeDef = TypedDict(
-    "GetMonitorOutputTypeDef",
-    {
-        "MonitorName": str,
-        "MonitorArn": str,
-        "Resources": List[str],
-        "Status": MonitorConfigStateType,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-        "ProcessingStatus": MonitorProcessingStatusCodeType,
-        "ProcessingStatusInfo": str,
-        "Tags": Dict[str, str],
-        "MaxCityNetworksToMonitor": int,
-        "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
-        "TrafficPercentageToMonitor": int,
-        "HealthEventsConfig": HealthEventsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateMonitorInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
     },
 )
 _OptionalUpdateMonitorInputRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor.egg-info/PKG-INFO` & `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-internetmonitor
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudWatchInternetMonitor 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudWatchInternetMonitor 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-internetmonitor"></a>
 
 # mypy-boto3-internetmonitor
 
 [![PyPI - mypy-boto3-internetmonitor](https://img.shields.io/pypi/v/mypy-boto3-internetmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-internetmonitor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-internetmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-internetmonitor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-internetmonitor?color=blue)](https://pypistats.org/packages/mypy-boto3-internetmonitor)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-internetmonitor)](https://pepy.tech/project/mypy-boto3-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchInternetMonitor 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
+[boto3.CloudWatchInternetMonitor 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
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
 [mypy-boto3-internetmonitor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,14 +334,16 @@
 from mypy_boto3_internetmonitor.type_defs import (
     AvailabilityMeasurementTypeDef,
     HealthEventsConfigTypeDef,
     CreateMonitorOutputTypeDef,
     DeleteMonitorInputRequestTypeDef,
     GetHealthEventInputRequestTypeDef,
     GetMonitorInputRequestTypeDef,
+    HealthEventsConfigOutputTypeDef,
+    S3ConfigOutputTypeDef,
     S3ConfigTypeDef,
     ListHealthEventsInputListHealthEventsPaginateTypeDef,
     ListHealthEventsInputRequestTypeDef,
     ListMonitorsInputListMonitorsPaginateTypeDef,
     ListMonitorsInputRequestTypeDef,
     MonitorTypeDef,
     ListTagsForResourceInputRequestTypeDef,
@@ -349,20 +351,21 @@
     NetworkTypeDef,
     PaginatorConfigTypeDef,
     RoundTripTimeTypeDef,
     ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateMonitorOutputTypeDef,
+    InternetMeasurementsLogDeliveryOutputTypeDef,
     InternetMeasurementsLogDeliveryTypeDef,
     ListMonitorsOutputTypeDef,
     NetworkImpairmentTypeDef,
     PerformanceMeasurementTypeDef,
-    CreateMonitorInputRequestTypeDef,
     GetMonitorOutputTypeDef,
+    CreateMonitorInputRequestTypeDef,
     UpdateMonitorInputRequestTypeDef,
     InternetHealthTypeDef,
     ImpactedLocationTypeDef,
     GetHealthEventOutputTypeDef,
     HealthEventTypeDef,
     ListHealthEventsOutputTypeDef,
 )
```

### Comparing `mypy-boto3-internetmonitor-1.28.0/mypy_boto3_internetmonitor.egg-info/SOURCES.txt` & `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.0/setup.py` & `mypy-boto3-internetmonitor-1.28.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-internetmonitor",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_internetmonitor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatchInternetMonitor 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.CloudWatchInternetMonitor 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

