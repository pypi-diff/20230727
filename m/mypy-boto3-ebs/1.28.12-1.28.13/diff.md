# Comparing `tmp/mypy-boto3-ebs-1.28.12.tar.gz` & `tmp/mypy-boto3-ebs-1.28.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ebs-1.28.12.tar", last modified: Thu Jul 27 05:34:36 2023, max compression
+gzip compressed data, was "mypy-boto3-ebs-1.28.13.tar", last modified: Thu Jul 27 19:34:20 2023, max compression
```

## Comparing `mypy-boto3-ebs-1.28.12.tar` & `mypy-boto3-ebs-1.28.13.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:36.684526 mypy-boto3-ebs-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-07-27 05:34:36.684526 mypy-boto3-ebs-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:36.684526 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-07-27 05:20:43.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-27 05:20:43.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:36.684526 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-07-27 05:34:36.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-27 05:34:36.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:36.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:36.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:36.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:36.000000 mypy-boto3-ebs-1.28.12/mypy_boto3_ebs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:36.684526 mypy-boto3-ebs-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:20:42.000000 mypy-boto3-ebs-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:34:20.087558 mypy-boto3-ebs-1.28.13/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 19:32:17.000000 mypy-boto3-ebs-1.28.13/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-07-27 19:34:20.087558 mypy-boto3-ebs-1.28.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-07-27 19:32:17.000000 mypy-boto3-ebs-1.28.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:34:20.087558 mypy-boto3-ebs-1.28.13/mypy_boto3_ebs/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-27 19:32:17.000000 mypy-boto3-ebs-1.28.13/mypy_boto3_ebs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-27 19:32:17.000000 mypy-boto3-ebs-1.28.13/mypy_boto3_ebs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 19:32:17.000000 mypy-boto3-ebs-1.28.13/mypy_boto3_ebs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-07-27 19:32:18.000000 mypy-boto3-ebs-1.28.13/mypy_boto3_ebs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-07-27 19:32:18.000000 mypy-boto3-ebs-1.28.13/mypy_boto3_ebs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-07-27 19:32:19.000000 mypy-boto3-ebs-1.28.13/mypy_boto3_ebs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-07-27 19:32:18.000000 mypy-boto3-ebs-1.28.13/mypy_boto3_ebs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:32:17.000000 mypy-boto3-ebs-1.28.13/mypy_boto3_ebs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-07-27 19:32:19.000000 mypy-boto3-ebs-1.28.13/mypy_boto3_ebs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-07-27 19:32:19.000000 mypy-boto3-ebs-1.28.13/mypy_boto3_ebs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 19:32:17.000000 mypy-boto3-ebs-1.28.13/mypy_boto3_ebs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:34:20.087558 mypy-boto3-ebs-1.28.13/mypy_boto3_ebs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-07-27 19:34:19.000000 mypy-boto3-ebs-1.28.13/mypy_boto3_ebs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-27 19:34:19.000000 mypy-boto3-ebs-1.28.13/mypy_boto3_ebs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:34:19.000000 mypy-boto3-ebs-1.28.13/mypy_boto3_ebs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:34:19.000000 mypy-boto3-ebs-1.28.13/mypy_boto3_ebs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 19:34:19.000000 mypy-boto3-ebs-1.28.13/mypy_boto3_ebs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 19:34:19.000000 mypy-boto3-ebs-1.28.13/mypy_boto3_ebs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 19:34:20.087558 mypy-boto3-ebs-1.28.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 19:32:17.000000 mypy-boto3-ebs-1.28.13/setup.py
```

### Comparing `mypy-boto3-ebs-1.28.12/LICENSE` & `mypy-boto3-ebs-1.28.13/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ebs-1.28.12/PKG-INFO` & `mypy-boto3-ebs-1.28.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ebs
-Version: 1.28.12
-Summary: Type annotations for boto3.EBS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.13
+Summary: Type annotations for boto3.EBS 1.28.13 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ebs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ebs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ebs)](https://pepy.tech/project/mypy-boto3-ebs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EBS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
+[boto3.EBS 1.28.13](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -277,14 +277,15 @@
 `mypy_boto3_ebs.literals` module contains literals extracted from shapes that
 can be used in user code for type checking.
 
 ```python
 from mypy_boto3_ebs.literals import (
     ChecksumAggregationMethodType,
     ChecksumAlgorithmType,
+    SSETypeType,
     StatusType,
     EBSServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
@@ -301,26 +302,26 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ebs.type_defs import (
     BlockTypeDef,
     ChangedBlockTypeDef,
     CompleteSnapshotRequestRequestTypeDef,
-    CompleteSnapshotResponseTypeDef,
+    ResponseMetadataTypeDef,
     GetSnapshotBlockRequestRequestTypeDef,
-    GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksRequestRequestTypeDef,
     ListSnapshotBlocksRequestRequestTypeDef,
     PutSnapshotBlockRequestRequestTypeDef,
-    PutSnapshotBlockResponseTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
     TagOutputTypeDef,
-    ListSnapshotBlocksResponseTypeDef,
+    CompleteSnapshotResponseTypeDef,
+    GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksResponseTypeDef,
+    ListSnapshotBlocksResponseTypeDef,
+    PutSnapshotBlockResponseTypeDef,
     StartSnapshotRequestRequestTypeDef,
     StartSnapshotResponseTypeDef,
 )
 
 
 def get_structure() -> BlockTypeDef:
     return {...}
```

### Comparing `mypy-boto3-ebs-1.28.12/README.md` & `mypy-boto3-ebs-1.28.13/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ebs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ebs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ebs)](https://pepy.tech/project/mypy-boto3-ebs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EBS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
+[boto3.EBS 1.28.13](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -245,14 +245,15 @@
 `mypy_boto3_ebs.literals` module contains literals extracted from shapes that
 can be used in user code for type checking.
 
 ```python
 from mypy_boto3_ebs.literals import (
     ChecksumAggregationMethodType,
     ChecksumAlgorithmType,
+    SSETypeType,
     StatusType,
     EBSServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
@@ -269,26 +270,26 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ebs.type_defs import (
     BlockTypeDef,
     ChangedBlockTypeDef,
     CompleteSnapshotRequestRequestTypeDef,
-    CompleteSnapshotResponseTypeDef,
+    ResponseMetadataTypeDef,
     GetSnapshotBlockRequestRequestTypeDef,
-    GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksRequestRequestTypeDef,
     ListSnapshotBlocksRequestRequestTypeDef,
     PutSnapshotBlockRequestRequestTypeDef,
-    PutSnapshotBlockResponseTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
     TagOutputTypeDef,
-    ListSnapshotBlocksResponseTypeDef,
+    CompleteSnapshotResponseTypeDef,
+    GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksResponseTypeDef,
+    ListSnapshotBlocksResponseTypeDef,
+    PutSnapshotBlockResponseTypeDef,
     StartSnapshotRequestRequestTypeDef,
     StartSnapshotResponseTypeDef,
 )
 
 
 def get_structure() -> BlockTypeDef:
     return {...}
```

### Comparing `mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/__main__.py` & `mypy-boto3-ebs-1.28.13/mypy_boto3_ebs/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EBS 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        "Type annotations for boto3.EBS 1.28.13\nVersion:         1.28.13\nBuilder version:"
         " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.13")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/client.py` & `mypy-boto3-ebs-1.28.13/mypy_boto3_ebs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/client.pyi` & `mypy-boto3-ebs-1.28.13/mypy_boto3_ebs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/literals.py` & `mypy-boto3-ebs-1.28.13/mypy_boto3_ebs/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ChecksumAggregationMethodType",
     "ChecksumAlgorithmType",
+    "SSETypeType",
     "StatusType",
     "EBSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ChecksumAggregationMethodType = Literal["LINEAR"]
 ChecksumAlgorithmType = Literal["SHA256"]
+SSETypeType = Literal["none", "sse-ebs", "sse-kms"]
 StatusType = Literal["completed", "error", "pending"]
 EBSServiceName = Literal["ebs"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
```

### Comparing `mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/literals.pyi` & `mypy-boto3-ebs-1.28.13/mypy_boto3_ebs/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,30 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ChecksumAggregationMethodType",
     "ChecksumAlgorithmType",
+    "SSETypeType",
     "StatusType",
     "EBSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 ChecksumAggregationMethodType = Literal["LINEAR"]
 ChecksumAlgorithmType = Literal["SHA256"]
+SSETypeType = Literal["none", "sse-ebs", "sse-kms"]
 StatusType = Literal["completed", "error", "pending"]
 EBSServiceName = Literal["ebs"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
```

### Comparing `mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/type_defs.py` & `mypy-boto3-ebs-1.28.13/mypy_boto3_ebs/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
 
-from .literals import StatusType
+from .literals import SSETypeType, StatusType
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
@@ -29,26 +29,26 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BlockTypeDef",
     "ChangedBlockTypeDef",
     "CompleteSnapshotRequestRequestTypeDef",
-    "CompleteSnapshotResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "GetSnapshotBlockRequestRequestTypeDef",
-    "GetSnapshotBlockResponseTypeDef",
     "ListChangedBlocksRequestRequestTypeDef",
     "ListSnapshotBlocksRequestRequestTypeDef",
     "PutSnapshotBlockRequestRequestTypeDef",
-    "PutSnapshotBlockResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "TagOutputTypeDef",
-    "ListSnapshotBlocksResponseTypeDef",
+    "CompleteSnapshotResponseTypeDef",
+    "GetSnapshotBlockResponseTypeDef",
     "ListChangedBlocksResponseTypeDef",
+    "ListSnapshotBlocksResponseTypeDef",
+    "PutSnapshotBlockResponseTypeDef",
     "StartSnapshotRequestRequestTypeDef",
     "StartSnapshotResponseTypeDef",
 )
 
 BlockTypeDef = TypedDict(
     "BlockTypeDef",
     {
@@ -88,42 +88,34 @@
 
 class CompleteSnapshotRequestRequestTypeDef(
     _RequiredCompleteSnapshotRequestRequestTypeDef, _OptionalCompleteSnapshotRequestRequestTypeDef
 ):
     pass
 
 
-CompleteSnapshotResponseTypeDef = TypedDict(
-    "CompleteSnapshotResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetSnapshotBlockRequestRequestTypeDef = TypedDict(
     "GetSnapshotBlockRequestRequestTypeDef",
     {
         "SnapshotId": str,
         "BlockIndex": int,
         "BlockToken": str,
     },
 )
 
-GetSnapshotBlockResponseTypeDef = TypedDict(
-    "GetSnapshotBlockResponseTypeDef",
-    {
-        "DataLength": int,
-        "BlockData": StreamingBody,
-        "Checksum": str,
-        "ChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListChangedBlocksRequestRequestTypeDef = TypedDict(
     "_RequiredListChangedBlocksRequestRequestTypeDef",
     {
         "SecondSnapshotId": str,
     },
 )
 _OptionalListChangedBlocksRequestRequestTypeDef = TypedDict(
@@ -190,34 +182,14 @@
 
 class PutSnapshotBlockRequestRequestTypeDef(
     _RequiredPutSnapshotBlockRequestRequestTypeDef, _OptionalPutSnapshotBlockRequestRequestTypeDef
 ):
     pass
 
 
-PutSnapshotBlockResponseTypeDef = TypedDict(
-    "PutSnapshotBlockResponseTypeDef",
-    {
-        "Checksum": str,
-        "ChecksumAlgorithm": Literal["SHA256"],
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -228,35 +200,63 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-ListSnapshotBlocksResponseTypeDef = TypedDict(
-    "ListSnapshotBlocksResponseTypeDef",
+CompleteSnapshotResponseTypeDef = TypedDict(
+    "CompleteSnapshotResponseTypeDef",
     {
-        "Blocks": List[BlockTypeDef],
+        "Status": StatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSnapshotBlockResponseTypeDef = TypedDict(
+    "GetSnapshotBlockResponseTypeDef",
+    {
+        "DataLength": int,
+        "BlockData": StreamingBody,
+        "Checksum": str,
+        "ChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListChangedBlocksResponseTypeDef = TypedDict(
+    "ListChangedBlocksResponseTypeDef",
+    {
+        "ChangedBlocks": List[ChangedBlockTypeDef],
         "ExpiryTime": datetime,
         "VolumeSize": int,
         "BlockSize": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListChangedBlocksResponseTypeDef = TypedDict(
-    "ListChangedBlocksResponseTypeDef",
+ListSnapshotBlocksResponseTypeDef = TypedDict(
+    "ListSnapshotBlocksResponseTypeDef",
     {
-        "ChangedBlocks": List[ChangedBlockTypeDef],
+        "Blocks": List[BlockTypeDef],
         "ExpiryTime": datetime,
         "VolumeSize": int,
         "BlockSize": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutSnapshotBlockResponseTypeDef = TypedDict(
+    "PutSnapshotBlockResponseTypeDef",
+    {
+        "Checksum": str,
+        "ChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredStartSnapshotRequestRequestTypeDef",
     {
         "VolumeSize": int,
@@ -292,10 +292,11 @@
         "Status": StatusType,
         "StartTime": datetime,
         "VolumeSize": int,
         "BlockSize": int,
         "Tags": List[TagOutputTypeDef],
         "ParentSnapshotId": str,
         "KmsKeyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SseType": SSETypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ebs-1.28.12/mypy_boto3_ebs/type_defs.pyi` & `mypy-boto3-ebs-1.28.13/mypy_boto3_ebs/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -13,41 +13,41 @@
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
 
-from .literals import StatusType
+from .literals import SSETypeType, StatusType
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BlockTypeDef",
     "ChangedBlockTypeDef",
     "CompleteSnapshotRequestRequestTypeDef",
-    "CompleteSnapshotResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "GetSnapshotBlockRequestRequestTypeDef",
-    "GetSnapshotBlockResponseTypeDef",
     "ListChangedBlocksRequestRequestTypeDef",
     "ListSnapshotBlocksRequestRequestTypeDef",
     "PutSnapshotBlockRequestRequestTypeDef",
-    "PutSnapshotBlockResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "TagOutputTypeDef",
-    "ListSnapshotBlocksResponseTypeDef",
+    "CompleteSnapshotResponseTypeDef",
+    "GetSnapshotBlockResponseTypeDef",
     "ListChangedBlocksResponseTypeDef",
+    "ListSnapshotBlocksResponseTypeDef",
+    "PutSnapshotBlockResponseTypeDef",
     "StartSnapshotRequestRequestTypeDef",
     "StartSnapshotResponseTypeDef",
 )
 
 BlockTypeDef = TypedDict(
     "BlockTypeDef",
     {
@@ -85,42 +85,34 @@
 )
 
 class CompleteSnapshotRequestRequestTypeDef(
     _RequiredCompleteSnapshotRequestRequestTypeDef, _OptionalCompleteSnapshotRequestRequestTypeDef
 ):
     pass
 
-CompleteSnapshotResponseTypeDef = TypedDict(
-    "CompleteSnapshotResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetSnapshotBlockRequestRequestTypeDef = TypedDict(
     "GetSnapshotBlockRequestRequestTypeDef",
     {
         "SnapshotId": str,
         "BlockIndex": int,
         "BlockToken": str,
     },
 )
 
-GetSnapshotBlockResponseTypeDef = TypedDict(
-    "GetSnapshotBlockResponseTypeDef",
-    {
-        "DataLength": int,
-        "BlockData": StreamingBody,
-        "Checksum": str,
-        "ChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListChangedBlocksRequestRequestTypeDef = TypedDict(
     "_RequiredListChangedBlocksRequestRequestTypeDef",
     {
         "SecondSnapshotId": str,
     },
 )
 _OptionalListChangedBlocksRequestRequestTypeDef = TypedDict(
@@ -181,34 +173,14 @@
 )
 
 class PutSnapshotBlockRequestRequestTypeDef(
     _RequiredPutSnapshotBlockRequestRequestTypeDef, _OptionalPutSnapshotBlockRequestRequestTypeDef
 ):
     pass
 
-PutSnapshotBlockResponseTypeDef = TypedDict(
-    "PutSnapshotBlockResponseTypeDef",
-    {
-        "Checksum": str,
-        "ChecksumAlgorithm": Literal["SHA256"],
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -219,35 +191,63 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-ListSnapshotBlocksResponseTypeDef = TypedDict(
-    "ListSnapshotBlocksResponseTypeDef",
+CompleteSnapshotResponseTypeDef = TypedDict(
+    "CompleteSnapshotResponseTypeDef",
     {
-        "Blocks": List[BlockTypeDef],
+        "Status": StatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSnapshotBlockResponseTypeDef = TypedDict(
+    "GetSnapshotBlockResponseTypeDef",
+    {
+        "DataLength": int,
+        "BlockData": StreamingBody,
+        "Checksum": str,
+        "ChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListChangedBlocksResponseTypeDef = TypedDict(
+    "ListChangedBlocksResponseTypeDef",
+    {
+        "ChangedBlocks": List[ChangedBlockTypeDef],
         "ExpiryTime": datetime,
         "VolumeSize": int,
         "BlockSize": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListChangedBlocksResponseTypeDef = TypedDict(
-    "ListChangedBlocksResponseTypeDef",
+ListSnapshotBlocksResponseTypeDef = TypedDict(
+    "ListSnapshotBlocksResponseTypeDef",
     {
-        "ChangedBlocks": List[ChangedBlockTypeDef],
+        "Blocks": List[BlockTypeDef],
         "ExpiryTime": datetime,
         "VolumeSize": int,
         "BlockSize": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutSnapshotBlockResponseTypeDef = TypedDict(
+    "PutSnapshotBlockResponseTypeDef",
+    {
+        "Checksum": str,
+        "ChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredStartSnapshotRequestRequestTypeDef",
     {
         "VolumeSize": int,
@@ -281,10 +281,11 @@
         "Status": StatusType,
         "StartTime": datetime,
         "VolumeSize": int,
         "BlockSize": int,
         "Tags": List[TagOutputTypeDef],
         "ParentSnapshotId": str,
         "KmsKeyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SseType": SSETypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ebs-1.28.12/mypy_boto3_ebs.egg-info/PKG-INFO` & `mypy-boto3-ebs-1.28.13/mypy_boto3_ebs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ebs
-Version: 1.28.12
-Summary: Type annotations for boto3.EBS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.13
+Summary: Type annotations for boto3.EBS 1.28.13 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ebs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ebs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ebs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ebs)](https://pepy.tech/project/mypy-boto3-ebs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EBS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
+[boto3.EBS 1.28.13](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -277,14 +277,15 @@
 `mypy_boto3_ebs.literals` module contains literals extracted from shapes that
 can be used in user code for type checking.
 
 ```python
 from mypy_boto3_ebs.literals import (
     ChecksumAggregationMethodType,
     ChecksumAlgorithmType,
+    SSETypeType,
     StatusType,
     EBSServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
@@ -301,26 +302,26 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ebs.type_defs import (
     BlockTypeDef,
     ChangedBlockTypeDef,
     CompleteSnapshotRequestRequestTypeDef,
-    CompleteSnapshotResponseTypeDef,
+    ResponseMetadataTypeDef,
     GetSnapshotBlockRequestRequestTypeDef,
-    GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksRequestRequestTypeDef,
     ListSnapshotBlocksRequestRequestTypeDef,
     PutSnapshotBlockRequestRequestTypeDef,
-    PutSnapshotBlockResponseTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
     TagOutputTypeDef,
-    ListSnapshotBlocksResponseTypeDef,
+    CompleteSnapshotResponseTypeDef,
+    GetSnapshotBlockResponseTypeDef,
     ListChangedBlocksResponseTypeDef,
+    ListSnapshotBlocksResponseTypeDef,
+    PutSnapshotBlockResponseTypeDef,
     StartSnapshotRequestRequestTypeDef,
     StartSnapshotResponseTypeDef,
 )
 
 
 def get_structure() -> BlockTypeDef:
     return {...}
```

### Comparing `mypy-boto3-ebs-1.28.12/mypy_boto3_ebs.egg-info/SOURCES.txt` & `mypy-boto3-ebs-1.28.13/mypy_boto3_ebs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ebs-1.28.12/setup.py` & `mypy-boto3-ebs-1.28.13/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ebs",
-    version="1.28.12",
+    version="1.28.13",
     packages=["mypy_boto3_ebs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EBS 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.EBS 1.28.13 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

