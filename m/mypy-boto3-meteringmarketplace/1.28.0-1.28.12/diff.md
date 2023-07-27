# Comparing `tmp/mypy-boto3-meteringmarketplace-1.28.0.tar.gz` & `tmp/mypy-boto3-meteringmarketplace-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-meteringmarketplace-1.28.0.tar", last modified: Thu Jul  6 21:00:08 2023, max compression
+gzip compressed data, was "mypy-boto3-meteringmarketplace-1.28.12.tar", last modified: Thu Jul 27 05:35:02 2023, max compression
```

## Comparing `mypy-boto3-meteringmarketplace-1.28.0.tar` & `mypy-boto3-meteringmarketplace-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:08.126371 mypy-boto3-meteringmarketplace-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:47:33.000000 mypy-boto3-meteringmarketplace-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-07-06 21:00:08.126371 mypy-boto3-meteringmarketplace-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-07-06 20:47:33.000000 mypy-boto3-meteringmarketplace-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:08.106371 mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-06 20:47:33.000000 mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-06 20:47:33.000000 mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-06 20:47:33.000000 mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-07-06 20:47:33.000000 mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-07-06 20:47:33.000000 mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-06 20:47:33.000000 mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-06 20:47:33.000000 mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:47:33.000000 mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-06 20:47:33.000000 mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-07-06 20:47:33.000000 mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:47:33.000000 mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:08.126371 mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-07-06 21:00:07.000000 mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-06 21:00:07.000000 mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:07.000000 mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:07.000000 mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:07.000000 mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 21:00:07.000000 mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:08.126371 mypy-boto3-meteringmarketplace-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-06 20:47:33.000000 mypy-boto3-meteringmarketplace-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.704435 mypy-boto3-meteringmarketplace-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-07-27 05:35:02.700435 mypy-boto3-meteringmarketplace-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.696435 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.700435 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-07-27 05:35:02.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-27 05:35:02.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:02.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:02.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:02.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 05:35:02.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:02.704435 mypy-boto3-meteringmarketplace-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/setup.py
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.0/LICENSE` & `mypy-boto3-meteringmarketplace-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-meteringmarketplace-1.28.0/PKG-INFO` & `mypy-boto3-meteringmarketplace-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-meteringmarketplace
-Version: 1.28.0
-Summary: Type annotations for boto3.MarketplaceMetering 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MarketplaceMetering 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-meteringmarketplace"></a>
 
 # mypy-boto3-meteringmarketplace
 
 [![PyPI - mypy-boto3-meteringmarketplace](https://img.shields.io/pypi/v/mypy-boto3-meteringmarketplace.svg?color=blue)](https://pypi.org/project/mypy-boto3-meteringmarketplace)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-meteringmarketplace.svg?color=blue)](https://pypi.org/project/mypy-boto3-meteringmarketplace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-meteringmarketplace?color=blue)](https://pypistats.org/packages/mypy-boto3-meteringmarketplace)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-meteringmarketplace)](https://pepy.tech/project/mypy-boto3-meteringmarketplace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceMetering 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
+[boto3.MarketplaceMetering 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
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
 [mypy-boto3-meteringmarketplace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,20 +304,23 @@
 from mypy_boto3_meteringmarketplace.type_defs import (
     MeterUsageResultTypeDef,
     RegisterUsageRequestRequestTypeDef,
     RegisterUsageResultTypeDef,
     ResolveCustomerRequestRequestTypeDef,
     ResolveCustomerResultTypeDef,
     ResponseMetadataTypeDef,
+    TagOutputTypeDef,
     TagTypeDef,
+    UsageAllocationOutputTypeDef,
     UsageAllocationTypeDef,
+    UsageRecordOutputTypeDef,
     MeterUsageRequestRequestTypeDef,
     UsageRecordTypeDef,
-    BatchMeterUsageRequestRequestTypeDef,
     UsageRecordResultTypeDef,
+    BatchMeterUsageRequestRequestTypeDef,
     BatchMeterUsageResultTypeDef,
 )
 
 
 def get_structure() -> MeterUsageResultTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.0/README.md` & `mypy-boto3-meteringmarketplace-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-meteringmarketplace"></a>
 
 # mypy-boto3-meteringmarketplace
 
 [![PyPI - mypy-boto3-meteringmarketplace](https://img.shields.io/pypi/v/mypy-boto3-meteringmarketplace.svg?color=blue)](https://pypi.org/project/mypy-boto3-meteringmarketplace)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-meteringmarketplace.svg?color=blue)](https://pypi.org/project/mypy-boto3-meteringmarketplace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-meteringmarketplace?color=blue)](https://pypistats.org/packages/mypy-boto3-meteringmarketplace)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-meteringmarketplace)](https://pepy.tech/project/mypy-boto3-meteringmarketplace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceMetering 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
+[boto3.MarketplaceMetering 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
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
 [mypy-boto3-meteringmarketplace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/).
 
 See how it helps to find and fix potential bugs:
 
@@ -272,20 +272,23 @@
 from mypy_boto3_meteringmarketplace.type_defs import (
     MeterUsageResultTypeDef,
     RegisterUsageRequestRequestTypeDef,
     RegisterUsageResultTypeDef,
     ResolveCustomerRequestRequestTypeDef,
     ResolveCustomerResultTypeDef,
     ResponseMetadataTypeDef,
+    TagOutputTypeDef,
     TagTypeDef,
+    UsageAllocationOutputTypeDef,
     UsageAllocationTypeDef,
+    UsageRecordOutputTypeDef,
     MeterUsageRequestRequestTypeDef,
     UsageRecordTypeDef,
-    BatchMeterUsageRequestRequestTypeDef,
     UsageRecordResultTypeDef,
+    BatchMeterUsageRequestRequestTypeDef,
     BatchMeterUsageResultTypeDef,
 )
 
 
 def get_structure() -> MeterUsageResultTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace/__main__.py` & `mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MarketplaceMetering 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.MarketplaceMetering 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering\nOther"
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

### Comparing `mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace/client.py` & `mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace/client.pyi` & `mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace/literals.py` & `mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,14 +145,15 @@
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
@@ -231,26 +232,28 @@
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

### Comparing `mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace/literals.pyi` & `mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -143,14 +143,15 @@
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
@@ -229,26 +230,28 @@
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

### Comparing `mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace/type_defs.py` & `mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,20 +26,23 @@
 __all__ = (
     "MeterUsageResultTypeDef",
     "RegisterUsageRequestRequestTypeDef",
     "RegisterUsageResultTypeDef",
     "ResolveCustomerRequestRequestTypeDef",
     "ResolveCustomerResultTypeDef",
     "ResponseMetadataTypeDef",
+    "TagOutputTypeDef",
     "TagTypeDef",
+    "UsageAllocationOutputTypeDef",
     "UsageAllocationTypeDef",
+    "UsageRecordOutputTypeDef",
     "MeterUsageRequestRequestTypeDef",
     "UsageRecordTypeDef",
-    "BatchMeterUsageRequestRequestTypeDef",
     "UsageRecordResultTypeDef",
+    "BatchMeterUsageRequestRequestTypeDef",
     "BatchMeterUsageResultTypeDef",
 )
 
 MeterUsageResultTypeDef = TypedDict(
     "MeterUsageResultTypeDef",
     {
         "MeteringRecordId": str,
@@ -102,22 +105,51 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+_RequiredUsageAllocationOutputTypeDef = TypedDict(
+    "_RequiredUsageAllocationOutputTypeDef",
+    {
+        "AllocatedUsageQuantity": int,
+    },
+)
+_OptionalUsageAllocationOutputTypeDef = TypedDict(
+    "_OptionalUsageAllocationOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class UsageAllocationOutputTypeDef(
+    _RequiredUsageAllocationOutputTypeDef, _OptionalUsageAllocationOutputTypeDef
+):
+    pass
+
+
 _RequiredUsageAllocationTypeDef = TypedDict(
     "_RequiredUsageAllocationTypeDef",
     {
         "AllocatedUsageQuantity": int,
     },
 )
 _OptionalUsageAllocationTypeDef = TypedDict(
@@ -129,14 +161,38 @@
 )
 
 
 class UsageAllocationTypeDef(_RequiredUsageAllocationTypeDef, _OptionalUsageAllocationTypeDef):
     pass
 
 
+_RequiredUsageRecordOutputTypeDef = TypedDict(
+    "_RequiredUsageRecordOutputTypeDef",
+    {
+        "Timestamp": datetime,
+        "CustomerIdentifier": str,
+        "Dimension": str,
+    },
+)
+_OptionalUsageRecordOutputTypeDef = TypedDict(
+    "_OptionalUsageRecordOutputTypeDef",
+    {
+        "Quantity": int,
+        "UsageAllocations": List[UsageAllocationOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class UsageRecordOutputTypeDef(
+    _RequiredUsageRecordOutputTypeDef, _OptionalUsageRecordOutputTypeDef
+):
+    pass
+
+
 _RequiredMeterUsageRequestRequestTypeDef = TypedDict(
     "_RequiredMeterUsageRequestRequestTypeDef",
     {
         "ProductCode": str,
         "Timestamp": Union[datetime, str],
         "UsageDimension": str,
     },
@@ -176,33 +232,33 @@
 )
 
 
 class UsageRecordTypeDef(_RequiredUsageRecordTypeDef, _OptionalUsageRecordTypeDef):
     pass
 
 
-BatchMeterUsageRequestRequestTypeDef = TypedDict(
-    "BatchMeterUsageRequestRequestTypeDef",
-    {
-        "UsageRecords": Sequence[UsageRecordTypeDef],
-        "ProductCode": str,
-    },
-)
-
 UsageRecordResultTypeDef = TypedDict(
     "UsageRecordResultTypeDef",
     {
-        "UsageRecord": UsageRecordTypeDef,
+        "UsageRecord": UsageRecordOutputTypeDef,
         "MeteringRecordId": str,
         "Status": UsageRecordResultStatusType,
     },
     total=False,
 )
 
+BatchMeterUsageRequestRequestTypeDef = TypedDict(
+    "BatchMeterUsageRequestRequestTypeDef",
+    {
+        "UsageRecords": Sequence[UsageRecordTypeDef],
+        "ProductCode": str,
+    },
+)
+
 BatchMeterUsageResultTypeDef = TypedDict(
     "BatchMeterUsageResultTypeDef",
     {
         "Results": List[UsageRecordResultTypeDef],
-        "UnprocessedRecords": List[UsageRecordTypeDef],
+        "UnprocessedRecords": List[UsageRecordOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace/type_defs.pyi` & `mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -25,20 +25,23 @@
 __all__ = (
     "MeterUsageResultTypeDef",
     "RegisterUsageRequestRequestTypeDef",
     "RegisterUsageResultTypeDef",
     "ResolveCustomerRequestRequestTypeDef",
     "ResolveCustomerResultTypeDef",
     "ResponseMetadataTypeDef",
+    "TagOutputTypeDef",
     "TagTypeDef",
+    "UsageAllocationOutputTypeDef",
     "UsageAllocationTypeDef",
+    "UsageRecordOutputTypeDef",
     "MeterUsageRequestRequestTypeDef",
     "UsageRecordTypeDef",
-    "BatchMeterUsageRequestRequestTypeDef",
     "UsageRecordResultTypeDef",
+    "BatchMeterUsageRequestRequestTypeDef",
     "BatchMeterUsageResultTypeDef",
 )
 
 MeterUsageResultTypeDef = TypedDict(
     "MeterUsageResultTypeDef",
     {
         "MeteringRecordId": str,
@@ -99,22 +102,49 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+_RequiredUsageAllocationOutputTypeDef = TypedDict(
+    "_RequiredUsageAllocationOutputTypeDef",
+    {
+        "AllocatedUsageQuantity": int,
+    },
+)
+_OptionalUsageAllocationOutputTypeDef = TypedDict(
+    "_OptionalUsageAllocationOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+class UsageAllocationOutputTypeDef(
+    _RequiredUsageAllocationOutputTypeDef, _OptionalUsageAllocationOutputTypeDef
+):
+    pass
+
 _RequiredUsageAllocationTypeDef = TypedDict(
     "_RequiredUsageAllocationTypeDef",
     {
         "AllocatedUsageQuantity": int,
     },
 )
 _OptionalUsageAllocationTypeDef = TypedDict(
@@ -124,14 +154,36 @@
     },
     total=False,
 )
 
 class UsageAllocationTypeDef(_RequiredUsageAllocationTypeDef, _OptionalUsageAllocationTypeDef):
     pass
 
+_RequiredUsageRecordOutputTypeDef = TypedDict(
+    "_RequiredUsageRecordOutputTypeDef",
+    {
+        "Timestamp": datetime,
+        "CustomerIdentifier": str,
+        "Dimension": str,
+    },
+)
+_OptionalUsageRecordOutputTypeDef = TypedDict(
+    "_OptionalUsageRecordOutputTypeDef",
+    {
+        "Quantity": int,
+        "UsageAllocations": List[UsageAllocationOutputTypeDef],
+    },
+    total=False,
+)
+
+class UsageRecordOutputTypeDef(
+    _RequiredUsageRecordOutputTypeDef, _OptionalUsageRecordOutputTypeDef
+):
+    pass
+
 _RequiredMeterUsageRequestRequestTypeDef = TypedDict(
     "_RequiredMeterUsageRequestRequestTypeDef",
     {
         "ProductCode": str,
         "Timestamp": Union[datetime, str],
         "UsageDimension": str,
     },
@@ -167,33 +219,33 @@
     },
     total=False,
 )
 
 class UsageRecordTypeDef(_RequiredUsageRecordTypeDef, _OptionalUsageRecordTypeDef):
     pass
 
-BatchMeterUsageRequestRequestTypeDef = TypedDict(
-    "BatchMeterUsageRequestRequestTypeDef",
-    {
-        "UsageRecords": Sequence[UsageRecordTypeDef],
-        "ProductCode": str,
-    },
-)
-
 UsageRecordResultTypeDef = TypedDict(
     "UsageRecordResultTypeDef",
     {
-        "UsageRecord": UsageRecordTypeDef,
+        "UsageRecord": UsageRecordOutputTypeDef,
         "MeteringRecordId": str,
         "Status": UsageRecordResultStatusType,
     },
     total=False,
 )
 
+BatchMeterUsageRequestRequestTypeDef = TypedDict(
+    "BatchMeterUsageRequestRequestTypeDef",
+    {
+        "UsageRecords": Sequence[UsageRecordTypeDef],
+        "ProductCode": str,
+    },
+)
+
 BatchMeterUsageResultTypeDef = TypedDict(
     "BatchMeterUsageResultTypeDef",
     {
         "Results": List[UsageRecordResultTypeDef],
-        "UnprocessedRecords": List[UsageRecordTypeDef],
+        "UnprocessedRecords": List[UsageRecordOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace.egg-info/PKG-INFO` & `mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-meteringmarketplace
-Version: 1.28.0
-Summary: Type annotations for boto3.MarketplaceMetering 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MarketplaceMetering 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-meteringmarketplace"></a>
 
 # mypy-boto3-meteringmarketplace
 
 [![PyPI - mypy-boto3-meteringmarketplace](https://img.shields.io/pypi/v/mypy-boto3-meteringmarketplace.svg?color=blue)](https://pypi.org/project/mypy-boto3-meteringmarketplace)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-meteringmarketplace.svg?color=blue)](https://pypi.org/project/mypy-boto3-meteringmarketplace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-meteringmarketplace?color=blue)](https://pypistats.org/packages/mypy-boto3-meteringmarketplace)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-meteringmarketplace)](https://pepy.tech/project/mypy-boto3-meteringmarketplace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceMetering 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
+[boto3.MarketplaceMetering 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
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
 [mypy-boto3-meteringmarketplace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,20 +304,23 @@
 from mypy_boto3_meteringmarketplace.type_defs import (
     MeterUsageResultTypeDef,
     RegisterUsageRequestRequestTypeDef,
     RegisterUsageResultTypeDef,
     ResolveCustomerRequestRequestTypeDef,
     ResolveCustomerResultTypeDef,
     ResponseMetadataTypeDef,
+    TagOutputTypeDef,
     TagTypeDef,
+    UsageAllocationOutputTypeDef,
     UsageAllocationTypeDef,
+    UsageRecordOutputTypeDef,
     MeterUsageRequestRequestTypeDef,
     UsageRecordTypeDef,
-    BatchMeterUsageRequestRequestTypeDef,
     UsageRecordResultTypeDef,
+    BatchMeterUsageRequestRequestTypeDef,
     BatchMeterUsageResultTypeDef,
 )
 
 
 def get_structure() -> MeterUsageResultTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.0/mypy_boto3_meteringmarketplace.egg-info/SOURCES.txt` & `mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-meteringmarketplace-1.28.0/setup.py` & `mypy-boto3-meteringmarketplace-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-meteringmarketplace",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_meteringmarketplace"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MarketplaceMetering 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.MarketplaceMetering 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

