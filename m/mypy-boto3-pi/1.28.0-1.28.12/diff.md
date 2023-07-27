# Comparing `tmp/mypy-boto3-pi-1.28.0.tar.gz` & `tmp/mypy-boto3-pi-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pi-1.28.0.tar", last modified: Thu Jul  6 21:00:18 2023, max compression
+gzip compressed data, was "mypy-boto3-pi-1.28.12.tar", last modified: Thu Jul 27 11:49:24 2023, max compression
```

## Comparing `mypy-boto3-pi-1.28.0.tar` & `mypy-boto3-pi-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:18.610392 mypy-boto3-pi-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:49:14.000000 mypy-boto3-pi-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-07-06 21:00:18.606392 mypy-boto3-pi-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-07-06 20:49:14.000000 mypy-boto3-pi-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:18.594392 mypy-boto3-pi-1.28.0/mypy_boto3_pi/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-06 20:49:14.000000 mypy-boto3-pi-1.28.0/mypy_boto3_pi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-06 20:49:14.000000 mypy-boto3-pi-1.28.0/mypy_boto3_pi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-06 20:49:14.000000 mypy-boto3-pi-1.28.0/mypy_boto3_pi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-07-06 20:49:14.000000 mypy-boto3-pi-1.28.0/mypy_boto3_pi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-06 20:49:14.000000 mypy-boto3-pi-1.28.0/mypy_boto3_pi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-07-06 20:49:15.000000 mypy-boto3-pi-1.28.0/mypy_boto3_pi/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-07-06 20:49:14.000000 mypy-boto3-pi-1.28.0/mypy_boto3_pi/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:49:14.000000 mypy-boto3-pi-1.28.0/mypy_boto3_pi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-07-06 20:49:15.000000 mypy-boto3-pi-1.28.0/mypy_boto3_pi/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-07-06 20:49:15.000000 mypy-boto3-pi-1.28.0/mypy_boto3_pi/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:49:14.000000 mypy-boto3-pi-1.28.0/mypy_boto3_pi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:18.606392 mypy-boto3-pi-1.28.0/mypy_boto3_pi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-07-06 21:00:18.000000 mypy-boto3-pi-1.28.0/mypy_boto3_pi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-06 21:00:18.000000 mypy-boto3-pi-1.28.0/mypy_boto3_pi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:18.000000 mypy-boto3-pi-1.28.0/mypy_boto3_pi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:18.000000 mypy-boto3-pi-1.28.0/mypy_boto3_pi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:18.000000 mypy-boto3-pi-1.28.0/mypy_boto3_pi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 21:00:18.000000 mypy-boto3-pi-1.28.0/mypy_boto3_pi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:18.610392 mypy-boto3-pi-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-06 20:49:14.000000 mypy-boto3-pi-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.801161 mypy-boto3-pi-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:21.000000 mypy-boto3-pi-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-07-27 11:49:24.801161 mypy-boto3-pi-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-07-27 11:41:21.000000 mypy-boto3-pi-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.801161 mypy-boto3-pi-1.28.12/mypy_boto3_pi/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-27 11:41:21.000000 mypy-boto3-pi-1.28.12/mypy_boto3_pi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-27 11:41:21.000000 mypy-boto3-pi-1.28.12/mypy_boto3_pi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-27 11:41:21.000000 mypy-boto3-pi-1.28.12/mypy_boto3_pi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-07-27 11:41:21.000000 mypy-boto3-pi-1.28.12/mypy_boto3_pi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-27 11:41:21.000000 mypy-boto3-pi-1.28.12/mypy_boto3_pi/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-07-27 11:41:21.000000 mypy-boto3-pi-1.28.12/mypy_boto3_pi/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-07-27 11:41:21.000000 mypy-boto3-pi-1.28.12/mypy_boto3_pi/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:21.000000 mypy-boto3-pi-1.28.12/mypy_boto3_pi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-07-27 11:41:22.000000 mypy-boto3-pi-1.28.12/mypy_boto3_pi/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-07-27 11:41:22.000000 mypy-boto3-pi-1.28.12/mypy_boto3_pi/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:21.000000 mypy-boto3-pi-1.28.12/mypy_boto3_pi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.801161 mypy-boto3-pi-1.28.12/mypy_boto3_pi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-07-27 11:49:24.000000 mypy-boto3-pi-1.28.12/mypy_boto3_pi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-27 11:49:24.000000 mypy-boto3-pi-1.28.12/mypy_boto3_pi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-pi-1.28.12/mypy_boto3_pi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-pi-1.28.12/mypy_boto3_pi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:24.000000 mypy-boto3-pi-1.28.12/mypy_boto3_pi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 11:49:24.000000 mypy-boto3-pi-1.28.12/mypy_boto3_pi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:24.801161 mypy-boto3-pi-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-27 11:41:21.000000 mypy-boto3-pi-1.28.12/setup.py
```

### Comparing `mypy-boto3-pi-1.28.0/LICENSE` & `mypy-boto3-pi-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pi-1.28.0/PKG-INFO` & `mypy-boto3-pi-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pi
-Version: 1.28.0
-Summary: Type annotations for boto3.PI 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.PI 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-pi"></a>
 
 # mypy-boto3-pi
 
 [![PyPI - mypy-boto3-pi](https://img.shields.io/pypi/v/mypy-boto3-pi.svg?color=blue)](https://pypi.org/project/mypy-boto3-pi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pi.svg?color=blue)](https://pypi.org/project/mypy-boto3-pi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pi?color=blue)](https://pypistats.org/packages/mypy-boto3-pi)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pi)](https://pepy.tech/project/mypy-boto3-pi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PI 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
+[boto3.PI 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
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
 [mypy-boto3-pi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,25 +302,25 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pi.type_defs import (
     DataPointTypeDef,
     DimensionGroupTypeDef,
     DimensionKeyDescriptionTypeDef,
+    ResponseMetadataTypeDef,
     ResponsePartitionKeyTypeDef,
     DimensionDetailTypeDef,
     DimensionKeyDetailTypeDef,
     FeatureMetadataTypeDef,
     GetDimensionKeyDetailsRequestRequestTypeDef,
     GetResourceMetadataRequestRequestTypeDef,
     ListAvailableResourceDimensionsRequestRequestTypeDef,
     ListAvailableResourceMetricsRequestRequestTypeDef,
     ResponseResourceMetricTypeDef,
     ResponseResourceMetricKeyTypeDef,
-    ResponseMetadataTypeDef,
     DescribeDimensionKeysRequestRequestTypeDef,
     MetricQueryTypeDef,
     DescribeDimensionKeysResponseTypeDef,
     DimensionGroupDetailTypeDef,
     GetDimensionKeyDetailsResponseTypeDef,
     GetResourceMetadataResponseTypeDef,
     ListAvailableResourceMetricsResponseTypeDef,
```

### Comparing `mypy-boto3-pi-1.28.0/README.md` & `mypy-boto3-pi-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-pi"></a>
 
 # mypy-boto3-pi
 
 [![PyPI - mypy-boto3-pi](https://img.shields.io/pypi/v/mypy-boto3-pi.svg?color=blue)](https://pypi.org/project/mypy-boto3-pi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pi.svg?color=blue)](https://pypi.org/project/mypy-boto3-pi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pi?color=blue)](https://pypistats.org/packages/mypy-boto3-pi)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pi)](https://pepy.tech/project/mypy-boto3-pi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PI 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
+[boto3.PI 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
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
 [mypy-boto3-pi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -270,25 +270,25 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pi.type_defs import (
     DataPointTypeDef,
     DimensionGroupTypeDef,
     DimensionKeyDescriptionTypeDef,
+    ResponseMetadataTypeDef,
     ResponsePartitionKeyTypeDef,
     DimensionDetailTypeDef,
     DimensionKeyDetailTypeDef,
     FeatureMetadataTypeDef,
     GetDimensionKeyDetailsRequestRequestTypeDef,
     GetResourceMetadataRequestRequestTypeDef,
     ListAvailableResourceDimensionsRequestRequestTypeDef,
     ListAvailableResourceMetricsRequestRequestTypeDef,
     ResponseResourceMetricTypeDef,
     ResponseResourceMetricKeyTypeDef,
-    ResponseMetadataTypeDef,
     DescribeDimensionKeysRequestRequestTypeDef,
     MetricQueryTypeDef,
     DescribeDimensionKeysResponseTypeDef,
     DimensionGroupDetailTypeDef,
     GetDimensionKeyDetailsResponseTypeDef,
     GetResourceMetadataResponseTypeDef,
     ListAvailableResourceMetricsResponseTypeDef,
```

### Comparing `mypy-boto3-pi-1.28.0/mypy_boto3_pi/__main__.py` & `mypy-boto3-pi-1.28.12/mypy_boto3_pi/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PI 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.PI 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI\nOther"
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

### Comparing `mypy-boto3-pi-1.28.0/mypy_boto3_pi/client.py` & `mypy-boto3-pi-1.28.12/mypy_boto3_pi/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pi-1.28.0/mypy_boto3_pi/client.pyi` & `mypy-boto3-pi-1.28.12/mypy_boto3_pi/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pi-1.28.0/mypy_boto3_pi/literals.py` & `mypy-boto3-pi-1.28.12/mypy_boto3_pi/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,27 +14,25 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DetailStatusType",
     "FeatureStatusType",
     "PeriodAlignmentType",
     "ServiceTypeType",
     "PIServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 DetailStatusType = Literal["AVAILABLE", "PROCESSING", "UNAVAILABLE"]
 FeatureStatusType = Literal[
     "DISABLED",
     "DISABLED_PENDING_REBOOT",
     "ENABLED",
     "ENABLED_PENDING_REBOOT",
     "UNKNOWN",
@@ -158,14 +156,15 @@
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
@@ -244,26 +243,28 @@
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

### Comparing `mypy-boto3-pi-1.28.0/mypy_boto3_pi/literals.pyi` & `mypy-boto3-pi-1.28.12/mypy_boto3_pi/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DetailStatusType",
     "FeatureStatusType",
     "PeriodAlignmentType",
     "ServiceTypeType",
     "PIServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 DetailStatusType = Literal["AVAILABLE", "PROCESSING", "UNAVAILABLE"]
 FeatureStatusType = Literal[
     "DISABLED",
     "DISABLED_PENDING_REBOOT",
     "ENABLED",
     "ENABLED_PENDING_REBOOT",
     "UNKNOWN",
@@ -156,14 +158,15 @@
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
@@ -242,26 +245,28 @@
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

### Comparing `mypy-boto3-pi-1.28.0/mypy_boto3_pi/type_defs.py` & `mypy-boto3-pi-1.28.12/mypy_boto3_pi/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,25 +23,25 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "DataPointTypeDef",
     "DimensionGroupTypeDef",
     "DimensionKeyDescriptionTypeDef",
+    "ResponseMetadataTypeDef",
     "ResponsePartitionKeyTypeDef",
     "DimensionDetailTypeDef",
     "DimensionKeyDetailTypeDef",
     "FeatureMetadataTypeDef",
     "GetDimensionKeyDetailsRequestRequestTypeDef",
     "GetResourceMetadataRequestRequestTypeDef",
     "ListAvailableResourceDimensionsRequestRequestTypeDef",
     "ListAvailableResourceMetricsRequestRequestTypeDef",
     "ResponseResourceMetricTypeDef",
     "ResponseResourceMetricKeyTypeDef",
-    "ResponseMetadataTypeDef",
     "DescribeDimensionKeysRequestRequestTypeDef",
     "MetricQueryTypeDef",
     "DescribeDimensionKeysResponseTypeDef",
     "DimensionGroupDetailTypeDef",
     "GetDimensionKeyDetailsResponseTypeDef",
     "GetResourceMetadataResponseTypeDef",
     "ListAvailableResourceMetricsResponseTypeDef",
@@ -87,14 +87,25 @@
         "Total": float,
         "AdditionalMetrics": Dict[str, float],
         "Partitions": List[float],
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
 ResponsePartitionKeyTypeDef = TypedDict(
     "ResponsePartitionKeyTypeDef",
     {
         "Dimensions": Dict[str, str],
     },
 )
 
@@ -234,25 +245,14 @@
 
 class ResponseResourceMetricKeyTypeDef(
     _RequiredResponseResourceMetricKeyTypeDef, _OptionalResponseResourceMetricKeyTypeDef
 ):
     pass
 
 
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
 _RequiredDescribeDimensionKeysRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDimensionKeysRequestRequestTypeDef",
     {
         "ServiceType": ServiceTypeType,
         "Identifier": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -305,15 +305,15 @@
     "DescribeDimensionKeysResponseTypeDef",
     {
         "AlignedStartTime": datetime,
         "AlignedEndTime": datetime,
         "PartitionKeys": List[ResponsePartitionKeyTypeDef],
         "Keys": List[DimensionKeyDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DimensionGroupDetailTypeDef = TypedDict(
     "DimensionGroupDetailTypeDef",
     {
         "Group": str,
@@ -322,33 +322,33 @@
     total=False,
 )
 
 GetDimensionKeyDetailsResponseTypeDef = TypedDict(
     "GetDimensionKeyDetailsResponseTypeDef",
     {
         "Dimensions": List[DimensionKeyDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceMetadataResponseTypeDef = TypedDict(
     "GetResourceMetadataResponseTypeDef",
     {
         "Identifier": str,
         "Features": Dict[str, FeatureMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAvailableResourceMetricsResponseTypeDef = TypedDict(
     "ListAvailableResourceMetricsResponseTypeDef",
     {
         "Metrics": List[ResponseResourceMetricTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MetricKeyDataPointsTypeDef = TypedDict(
     "MetricKeyDataPointsTypeDef",
     {
         "Key": ResponseResourceMetricKeyTypeDef,
@@ -399,19 +399,19 @@
     "GetResourceMetricsResponseTypeDef",
     {
         "AlignedStartTime": datetime,
         "AlignedEndTime": datetime,
         "Identifier": str,
         "MetricList": List[MetricKeyDataPointsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAvailableResourceDimensionsResponseTypeDef = TypedDict(
     "ListAvailableResourceDimensionsResponseTypeDef",
     {
         "MetricDimensions": List[MetricDimensionGroupsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-pi-1.28.0/mypy_boto3_pi/type_defs.pyi` & `mypy-boto3-pi-1.28.12/mypy_boto3_pi/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -22,25 +22,25 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "DataPointTypeDef",
     "DimensionGroupTypeDef",
     "DimensionKeyDescriptionTypeDef",
+    "ResponseMetadataTypeDef",
     "ResponsePartitionKeyTypeDef",
     "DimensionDetailTypeDef",
     "DimensionKeyDetailTypeDef",
     "FeatureMetadataTypeDef",
     "GetDimensionKeyDetailsRequestRequestTypeDef",
     "GetResourceMetadataRequestRequestTypeDef",
     "ListAvailableResourceDimensionsRequestRequestTypeDef",
     "ListAvailableResourceMetricsRequestRequestTypeDef",
     "ResponseResourceMetricTypeDef",
     "ResponseResourceMetricKeyTypeDef",
-    "ResponseMetadataTypeDef",
     "DescribeDimensionKeysRequestRequestTypeDef",
     "MetricQueryTypeDef",
     "DescribeDimensionKeysResponseTypeDef",
     "DimensionGroupDetailTypeDef",
     "GetDimensionKeyDetailsResponseTypeDef",
     "GetResourceMetadataResponseTypeDef",
     "ListAvailableResourceMetricsResponseTypeDef",
@@ -84,14 +84,25 @@
         "Total": float,
         "AdditionalMetrics": Dict[str, float],
         "Partitions": List[float],
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
 ResponsePartitionKeyTypeDef = TypedDict(
     "ResponsePartitionKeyTypeDef",
     {
         "Dimensions": Dict[str, str],
     },
 )
 
@@ -223,25 +234,14 @@
 )
 
 class ResponseResourceMetricKeyTypeDef(
     _RequiredResponseResourceMetricKeyTypeDef, _OptionalResponseResourceMetricKeyTypeDef
 ):
     pass
 
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
 _RequiredDescribeDimensionKeysRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDimensionKeysRequestRequestTypeDef",
     {
         "ServiceType": ServiceTypeType,
         "Identifier": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -290,15 +290,15 @@
     "DescribeDimensionKeysResponseTypeDef",
     {
         "AlignedStartTime": datetime,
         "AlignedEndTime": datetime,
         "PartitionKeys": List[ResponsePartitionKeyTypeDef],
         "Keys": List[DimensionKeyDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DimensionGroupDetailTypeDef = TypedDict(
     "DimensionGroupDetailTypeDef",
     {
         "Group": str,
@@ -307,33 +307,33 @@
     total=False,
 )
 
 GetDimensionKeyDetailsResponseTypeDef = TypedDict(
     "GetDimensionKeyDetailsResponseTypeDef",
     {
         "Dimensions": List[DimensionKeyDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceMetadataResponseTypeDef = TypedDict(
     "GetResourceMetadataResponseTypeDef",
     {
         "Identifier": str,
         "Features": Dict[str, FeatureMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAvailableResourceMetricsResponseTypeDef = TypedDict(
     "ListAvailableResourceMetricsResponseTypeDef",
     {
         "Metrics": List[ResponseResourceMetricTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MetricKeyDataPointsTypeDef = TypedDict(
     "MetricKeyDataPointsTypeDef",
     {
         "Key": ResponseResourceMetricKeyTypeDef,
@@ -382,19 +382,19 @@
     "GetResourceMetricsResponseTypeDef",
     {
         "AlignedStartTime": datetime,
         "AlignedEndTime": datetime,
         "Identifier": str,
         "MetricList": List[MetricKeyDataPointsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAvailableResourceDimensionsResponseTypeDef = TypedDict(
     "ListAvailableResourceDimensionsResponseTypeDef",
     {
         "MetricDimensions": List[MetricDimensionGroupsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-pi-1.28.0/mypy_boto3_pi.egg-info/PKG-INFO` & `mypy-boto3-pi-1.28.12/mypy_boto3_pi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pi
-Version: 1.28.0
-Summary: Type annotations for boto3.PI 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.PI 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-pi"></a>
 
 # mypy-boto3-pi
 
 [![PyPI - mypy-boto3-pi](https://img.shields.io/pypi/v/mypy-boto3-pi.svg?color=blue)](https://pypi.org/project/mypy-boto3-pi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pi.svg?color=blue)](https://pypi.org/project/mypy-boto3-pi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pi?color=blue)](https://pypistats.org/packages/mypy-boto3-pi)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pi)](https://pepy.tech/project/mypy-boto3-pi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PI 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
+[boto3.PI 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
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
 [mypy-boto3-pi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,25 +302,25 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pi.type_defs import (
     DataPointTypeDef,
     DimensionGroupTypeDef,
     DimensionKeyDescriptionTypeDef,
+    ResponseMetadataTypeDef,
     ResponsePartitionKeyTypeDef,
     DimensionDetailTypeDef,
     DimensionKeyDetailTypeDef,
     FeatureMetadataTypeDef,
     GetDimensionKeyDetailsRequestRequestTypeDef,
     GetResourceMetadataRequestRequestTypeDef,
     ListAvailableResourceDimensionsRequestRequestTypeDef,
     ListAvailableResourceMetricsRequestRequestTypeDef,
     ResponseResourceMetricTypeDef,
     ResponseResourceMetricKeyTypeDef,
-    ResponseMetadataTypeDef,
     DescribeDimensionKeysRequestRequestTypeDef,
     MetricQueryTypeDef,
     DescribeDimensionKeysResponseTypeDef,
     DimensionGroupDetailTypeDef,
     GetDimensionKeyDetailsResponseTypeDef,
     GetResourceMetadataResponseTypeDef,
     ListAvailableResourceMetricsResponseTypeDef,
```

### Comparing `mypy-boto3-pi-1.28.0/mypy_boto3_pi.egg-info/SOURCES.txt` & `mypy-boto3-pi-1.28.12/mypy_boto3_pi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pi-1.28.0/setup.py` & `mypy-boto3-pi-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pi",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_pi"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PI 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.PI 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

