# Comparing `tmp/mypy-boto3-ebs-1.28.0.tar.gz` & `tmp/mypy-boto3-ebs-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ebs-1.28.0.tar", last modified: Thu Jul  6 20:59:27 2023, max compression
+gzip compressed data, was "mypy-boto3-ebs-1.28.12.tar", last modified: Thu Jul 27 05:34:36 2023, max compression
```

## Comparing `mypy-boto3-ebs-1.28.0.tar` & `mypy-boto3-ebs-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:27.966287 mypy-boto3-ebs-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:38:36.000000 mypy-boto3-ebs-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-07-06 20:59:27.966287 mypy-boto3-ebs-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-07-06 20:38:36.000000 mypy-boto3-ebs-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:27.966287 mypy-boto3-ebs-1.28.0/mypy_boto3_ebs/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-06 20:38:36.000000 mypy-boto3-ebs-1.28.0/mypy_boto3_ebs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-06 20:38:36.000000 mypy-boto3-ebs-1.28.0/mypy_boto3_ebs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:38:36.000000 mypy-boto3-ebs-1.28.0/mypy_boto3_ebs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-07-06 20:38:36.000000 mypy-boto3-ebs-1.28.0/mypy_boto3_ebs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-07-06 20:38:36.000000 mypy-boto3-ebs-1.28.0/mypy_boto3_ebs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-07-06 20:38:36.000000 mypy-boto3-ebs-1.28.0/mypy_boto3_ebs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-07-06 20:38:36.000000 mypy-boto3-ebs-1.28.0/mypy_boto3_ebs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:38:36.000000 mypy-boto3-ebs-1.28.0/mypy_boto3_ebs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-07-06 20:38:37.000000 mypy-boto3-ebs-1.28.0/mypy_boto3_ebs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-07-06 20:38:36.000000 mypy-boto3-ebs-1.28.0/mypy_boto3_ebs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:38:36.000000 mypy-boto3-ebs-1.28.0/mypy_boto3_ebs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:27.966287 mypy-boto3-ebs-1.28.0/mypy_boto3_ebs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-07-06 20:59:27.000000 mypy-boto3-ebs-1.28.0/mypy_boto3_ebs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-06 20:59:27.000000 mypy-boto3-ebs-1.28.0/mypy_boto3_ebs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:27.000000 mypy-boto3-ebs-1.28.0/mypy_boto3_ebs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:27.000000 mypy-boto3-ebs-1.28.0/mypy_boto3_ebs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:27.000000 mypy-boto3-ebs-1.28.0/mypy_boto3_ebs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:27.000000 mypy-boto3-ebs-1.28.0/mypy_boto3_ebs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:27.966287 mypy-boto3-ebs-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:38:36.000000 mypy-boto3-ebs-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:36.684526 mypy-boto3-ebs-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-07-27 05:34:36.684526 mypy-boto3-ebs-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:36.684526 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-07-27 05:20:43.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-27 05:20:43.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:36.684526 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-07-27 05:34:36.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-27 05:34:36.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:36.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:36.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:36.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:36.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:36.684526 mypy-boto3-ebs-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/setup.py
```

### Comparing `mypy-boto3-ebs-1.28.0/LICENSE` & `mypy-boto3-ebs-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ebs-1.28.0/PKG-INFO` & `mypy-boto3-ebs-1.28.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ebs
-Version: 1.28.0
-Summary: Type annotations for boto3.EBS 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.EBS 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ebs"></a>
 
 # mypy-boto3-ebs
 
 [![PyPI - mypy-boto3-ebs](https://img.shields.io/pypi/v/mypy-boto3-ebs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ebs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ebs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ebs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ebs?color=blue)](https://pypistats.org/packages/mypy-boto3-ebs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ebs)](https://pepy.tech/project/mypy-boto3-ebs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EBS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
+[boto3.EBS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
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
 [mypy-boto3-ebs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -310,14 +310,15 @@
     GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksRequestRequestTypeDef,
     ListSnapshotBlocksRequestRequestTypeDef,
     PutSnapshotBlockRequestRequestTypeDef,
     PutSnapshotBlockResponseTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
+    TagOutputTypeDef,
     ListSnapshotBlocksResponseTypeDef,
     ListChangedBlocksResponseTypeDef,
     StartSnapshotRequestRequestTypeDef,
     StartSnapshotResponseTypeDef,
 )
```

### Comparing `mypy-boto3-ebs-1.28.0/README.md` & `mypy-boto3-ebs-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ebs"></a>
 
 # mypy-boto3-ebs
 
 [![PyPI - mypy-boto3-ebs](https://img.shields.io/pypi/v/mypy-boto3-ebs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ebs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ebs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ebs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ebs?color=blue)](https://pypistats.org/packages/mypy-boto3-ebs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ebs)](https://pepy.tech/project/mypy-boto3-ebs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EBS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
+[boto3.EBS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
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
 [mypy-boto3-ebs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -278,14 +278,15 @@
     GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksRequestRequestTypeDef,
     ListSnapshotBlocksRequestRequestTypeDef,
     PutSnapshotBlockRequestRequestTypeDef,
     PutSnapshotBlockResponseTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
+    TagOutputTypeDef,
     ListSnapshotBlocksResponseTypeDef,
     ListChangedBlocksResponseTypeDef,
     StartSnapshotRequestRequestTypeDef,
     StartSnapshotResponseTypeDef,
 )
```

### Comparing `mypy-boto3-ebs-1.28.0/mypy_boto3_ebs/__main__.py` & `mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EBS 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.EBS 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS\nOther"
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

### Comparing `mypy-boto3-ebs-1.28.0/mypy_boto3_ebs/client.py` & `mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ebs-1.28.0/mypy_boto3_ebs/client.pyi` & `mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ebs-1.28.0/mypy_boto3_ebs/literals.py` & `mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,26 +14,24 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ChecksumAggregationMethodType",
     "ChecksumAlgorithmType",
     "StatusType",
     "EBSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ChecksumAggregationMethodType = Literal["LINEAR"]
 ChecksumAlgorithmType = Literal["SHA256"]
 StatusType = Literal["completed", "error", "pending"]
 EBSServiceName = Literal["ebs"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -149,14 +147,15 @@
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
@@ -235,26 +234,28 @@
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

### Comparing `mypy-boto3-ebs-1.28.0/mypy_boto3_ebs/literals.pyi` & `mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,24 +14,26 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ChecksumAggregationMethodType",
     "ChecksumAlgorithmType",
     "StatusType",
     "EBSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 ChecksumAggregationMethodType = Literal["LINEAR"]
 ChecksumAlgorithmType = Literal["SHA256"]
 StatusType = Literal["completed", "error", "pending"]
 EBSServiceName = Literal["ebs"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -147,14 +149,15 @@
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
@@ -233,26 +236,28 @@
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

### Comparing `mypy-boto3-ebs-1.28.0/mypy_boto3_ebs/type_defs.py` & `mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     "GetSnapshotBlockResponseTypeDef",
     "ListChangedBlocksRequestRequestTypeDef",
     "ListSnapshotBlocksRequestRequestTypeDef",
     "PutSnapshotBlockRequestRequestTypeDef",
     "PutSnapshotBlockResponseTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
+    "TagOutputTypeDef",
     "ListSnapshotBlocksResponseTypeDef",
     "ListChangedBlocksResponseTypeDef",
     "StartSnapshotRequestRequestTypeDef",
     "StartSnapshotResponseTypeDef",
 )
 
 BlockTypeDef = TypedDict(
@@ -218,14 +219,23 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 ListSnapshotBlocksResponseTypeDef = TypedDict(
     "ListSnapshotBlocksResponseTypeDef",
     {
         "Blocks": List[BlockTypeDef],
         "ExpiryTime": datetime,
         "VolumeSize": int,
         "BlockSize": int,
@@ -279,13 +289,13 @@
         "Description": str,
         "SnapshotId": str,
         "OwnerId": str,
         "Status": StatusType,
         "StartTime": datetime,
         "VolumeSize": int,
         "BlockSize": int,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ParentSnapshotId": str,
         "KmsKeyArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ebs-1.28.0/mypy_boto3_ebs/type_defs.pyi` & `mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     "GetSnapshotBlockResponseTypeDef",
     "ListChangedBlocksRequestRequestTypeDef",
     "ListSnapshotBlocksRequestRequestTypeDef",
     "PutSnapshotBlockRequestRequestTypeDef",
     "PutSnapshotBlockResponseTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
+    "TagOutputTypeDef",
     "ListSnapshotBlocksResponseTypeDef",
     "ListChangedBlocksResponseTypeDef",
     "StartSnapshotRequestRequestTypeDef",
     "StartSnapshotResponseTypeDef",
 )
 
 BlockTypeDef = TypedDict(
@@ -209,14 +210,23 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 ListSnapshotBlocksResponseTypeDef = TypedDict(
     "ListSnapshotBlocksResponseTypeDef",
     {
         "Blocks": List[BlockTypeDef],
         "ExpiryTime": datetime,
         "VolumeSize": int,
         "BlockSize": int,
@@ -268,13 +278,13 @@
         "Description": str,
         "SnapshotId": str,
         "OwnerId": str,
         "Status": StatusType,
         "StartTime": datetime,
         "VolumeSize": int,
         "BlockSize": int,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ParentSnapshotId": str,
         "KmsKeyArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ebs-1.28.0/mypy_boto3_ebs.egg-info/PKG-INFO` & `mypy-boto3-ebs-1.28.12/mypy_boto3_ebs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ebs
-Version: 1.28.0
-Summary: Type annotations for boto3.EBS 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.EBS 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ebs"></a>
 
 # mypy-boto3-ebs
 
 [![PyPI - mypy-boto3-ebs](https://img.shields.io/pypi/v/mypy-boto3-ebs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ebs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ebs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ebs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ebs?color=blue)](https://pypistats.org/packages/mypy-boto3-ebs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ebs)](https://pepy.tech/project/mypy-boto3-ebs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EBS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
+[boto3.EBS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
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
 [mypy-boto3-ebs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -310,14 +310,15 @@
     GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksRequestRequestTypeDef,
     ListSnapshotBlocksRequestRequestTypeDef,
     PutSnapshotBlockRequestRequestTypeDef,
     PutSnapshotBlockResponseTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
+    TagOutputTypeDef,
     ListSnapshotBlocksResponseTypeDef,
     ListChangedBlocksResponseTypeDef,
     StartSnapshotRequestRequestTypeDef,
     StartSnapshotResponseTypeDef,
 )
```

### Comparing `mypy-boto3-ebs-1.28.0/mypy_boto3_ebs.egg-info/SOURCES.txt` & `mypy-boto3-ebs-1.28.12/mypy_boto3_ebs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ebs-1.28.0/setup.py` & `mypy-boto3-ebs-1.28.12/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ebs",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_ebs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EBS 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.EBS 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

