# Comparing `tmp/mypy-boto3-transfer-1.28.11.tar.gz` & `tmp/mypy-boto3-transfer-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-transfer-1.28.11.tar", last modified: Tue Jul 25 19:49:16 2023, max compression
+gzip compressed data, was "mypy-boto3-transfer-1.28.12.tar", last modified: Thu Jul 27 11:49:47 2023, max compression
```

## Comparing `mypy-boto3-transfer-1.28.11.tar` & `mypy-boto3-transfer-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:16.509065 mypy-boto3-transfer-1.28.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 19:48:58.000000 mypy-boto3-transfer-1.28.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22444 2023-07-25 19:49:16.509065 mypy-boto3-transfer-1.28.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20953 2023-07-25 19:48:58.000000 mypy-boto3-transfer-1.28.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:16.509065 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-25 19:48:58.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-25 19:48:58.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-25 19:48:58.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47079 2023-07-25 19:48:58.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47000 2023-07-25 19:48:58.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-07-25 19:49:00.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-07-25 19:49:00.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-25 19:48:59.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-07-25 19:48:59.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:48:58.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    62188 2023-07-25 19:49:01.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    62123 2023-07-25 19:49:00.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 19:48:58.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-25 19:48:59.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-25 19:48:59.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:16.509065 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22444 2023-07-25 19:49:16.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-25 19:49:16.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:16.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:16.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 19:49:16.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 19:49:16.000000 mypy-boto3-transfer-1.28.11/mypy_boto3_transfer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:49:16.509065 mypy-boto3-transfer-1.28.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-25 19:48:58.000000 mypy-boto3-transfer-1.28.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:47.153460 mypy-boto3-transfer-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-07-27 11:49:47.145460 mypy-boto3-transfer-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20937 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:47.145460 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47079 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47000 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-27 11:48:10.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-07-27 11:48:10.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    66431 2023-07-27 11:48:12.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66336 2023-07-27 11:48:11.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:47.145460 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-07-27 11:49:46.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-27 11:49:46.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:46.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:46.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:47.153460 mypy-boto3-transfer-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/setup.py
```

### Comparing `mypy-boto3-transfer-1.28.11/LICENSE` & `mypy-boto3-transfer-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.11/PKG-INFO` & `mypy-boto3-transfer-1.28.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transfer
-Version: 1.28.11
-Summary: Type annotations for boto3.Transfer 1.28.11 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.Transfer 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-transfer"></a>
 
 # mypy-boto3-transfer
 
 [![PyPI - mypy-boto3-transfer](https://img.shields.io/pypi/v/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transfer?color=blue)](https://pypistats.org/packages/mypy-boto3-transfer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transfer)](https://pepy.tech/project/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
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
 [mypy-boto3-transfer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-transfer-1.28.11/README.md` & `mypy-boto3-transfer-1.28.12/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-transfer"></a>
 
 # mypy-boto3-transfer
 
 [![PyPI - mypy-boto3-transfer](https://img.shields.io/pypi/v/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transfer?color=blue)](https://pypistats.org/packages/mypy-boto3-transfer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transfer)](https://pepy.tech/project/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
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
 [mypy-boto3-transfer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/__init__.py` & `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/__init__.pyi` & `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/__main__.py` & `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Transfer 1.28.11\nVersion:         1.28.11\nBuilder version:"
-        " 7.15.1\nDocs:           "
+        "Type annotations for boto3.Transfer 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer\nOther"
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

### Comparing `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/client.py` & `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/client.pyi` & `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/literals.py` & `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AgreementStatusTypeType",
     "As2TransportType",
     "CertificateStatusTypeType",
     "CertificateTypeType",
     "CertificateUsageTypeType",
     "CompressionEnumType",
@@ -63,15 +62,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AgreementStatusTypeType = Literal["ACTIVE", "INACTIVE"]
 As2TransportType = Literal["HTTP"]
 CertificateStatusTypeType = Literal["ACTIVE", "INACTIVE", "PENDING_ROTATION"]
 CertificateTypeType = Literal["CERTIFICATE", "CERTIFICATE_WITH_PRIVATE_KEY"]
 CertificateUsageTypeType = Literal["ENCRYPTION", "SIGNING"]
 CompressionEnumType = Literal["DISABLED", "ZLIB"]
 CustomStepStatusType = Literal["FAILURE", "SUCCESS"]
@@ -236,14 +234,15 @@
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
@@ -322,14 +321,15 @@
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

### Comparing `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/literals.pyi` & `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AgreementStatusTypeType",
     "As2TransportType",
     "CertificateStatusTypeType",
     "CertificateTypeType",
     "CertificateUsageTypeType",
     "CompressionEnumType",
@@ -62,14 +63,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 AgreementStatusTypeType = Literal["ACTIVE", "INACTIVE"]
 As2TransportType = Literal["HTTP"]
 CertificateStatusTypeType = Literal["ACTIVE", "INACTIVE", "PENDING_ROTATION"]
 CertificateTypeType = Literal["CERTIFICATE", "CERTIFICATE_WITH_PRIVATE_KEY"]
 CertificateUsageTypeType = Literal["ENCRYPTION", "SIGNING"]
 CompressionEnumType = Literal["DISABLED", "ZLIB"]
 CustomStepStatusType = Literal["FAILURE", "SUCCESS"]
@@ -234,14 +236,15 @@
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
@@ -320,14 +323,15 @@
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

### Comparing `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/paginator.py` & `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/paginator.pyi` & `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/type_defs.py` & `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,14 +254,15 @@
         "Compression": CompressionEnumType,
         "EncryptionAlgorithm": EncryptionAlgType,
         "SigningAlgorithm": SigningAlgType,
         "MdnSigningAlgorithm": MdnSigningAlgType,
         "MdnResponse": MdnResponseType,
         "BasicAuthSecretId": str,
     },
+    total=False,
 )
 
 As2ConnectorConfigTypeDef = TypedDict(
     "As2ConnectorConfigTypeDef",
     {
         "LocalProfileId": str,
         "PartnerProfileId": str,
@@ -371,14 +372,15 @@
     "CustomStepDetailsOutputTypeDef",
     {
         "Name": str,
         "Target": str,
         "TimeoutSeconds": int,
         "SourceFileLocation": str,
     },
+    total=False,
 )
 
 CustomStepDetailsTypeDef = TypedDict(
     "CustomStepDetailsTypeDef",
     {
         "Name": str,
         "Target": str,
@@ -451,14 +453,15 @@
 
 DeleteStepDetailsOutputTypeDef = TypedDict(
     "DeleteStepDetailsOutputTypeDef",
     {
         "Name": str,
         "SourceFileLocation": str,
     },
+    total=False,
 )
 
 DeleteStepDetailsTypeDef = TypedDict(
     "DeleteStepDetailsTypeDef",
     {
         "Name": str,
         "SourceFileLocation": str,
@@ -537,26 +540,39 @@
 DescribeSecurityPolicyRequestRequestTypeDef = TypedDict(
     "DescribeSecurityPolicyRequestRequestTypeDef",
     {
         "SecurityPolicyName": str,
     },
 )
 
-DescribedSecurityPolicyTypeDef = TypedDict(
-    "DescribedSecurityPolicyTypeDef",
+_RequiredDescribedSecurityPolicyTypeDef = TypedDict(
+    "_RequiredDescribedSecurityPolicyTypeDef",
     {
-        "Fips": bool,
         "SecurityPolicyName": str,
+    },
+)
+_OptionalDescribedSecurityPolicyTypeDef = TypedDict(
+    "_OptionalDescribedSecurityPolicyTypeDef",
+    {
+        "Fips": bool,
         "SshCiphers": List[str],
         "SshKexs": List[str],
         "SshMacs": List[str],
         "TlsCiphers": List[str],
     },
+    total=False,
 )
 
+
+class DescribedSecurityPolicyTypeDef(
+    _RequiredDescribedSecurityPolicyTypeDef, _OptionalDescribedSecurityPolicyTypeDef
+):
+    pass
+
+
 DescribeServerRequestRequestTypeDef = TypedDict(
     "DescribeServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 
@@ -588,77 +604,95 @@
     "HomeDirectoryMapEntryOutputTypeDef",
     {
         "Entry": str,
         "Target": str,
     },
 )
 
-PosixProfileOutputTypeDef = TypedDict(
-    "PosixProfileOutputTypeDef",
+_RequiredPosixProfileOutputTypeDef = TypedDict(
+    "_RequiredPosixProfileOutputTypeDef",
     {
         "Uid": int,
         "Gid": int,
+    },
+)
+_OptionalPosixProfileOutputTypeDef = TypedDict(
+    "_OptionalPosixProfileOutputTypeDef",
+    {
         "SecondaryGids": List[int],
     },
+    total=False,
 )
 
+
+class PosixProfileOutputTypeDef(
+    _RequiredPosixProfileOutputTypeDef, _OptionalPosixProfileOutputTypeDef
+):
+    pass
+
+
 TagOutputTypeDef = TypedDict(
     "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
 SftpConnectorConfigOutputTypeDef = TypedDict(
     "SftpConnectorConfigOutputTypeDef",
     {
         "UserSecretId": str,
         "TrustedHostKeys": List[str],
     },
+    total=False,
 )
 
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
         "LoggingRole": str,
         "LogGroupName": str,
     },
+    total=False,
 )
 
 EndpointDetailsOutputTypeDef = TypedDict(
     "EndpointDetailsOutputTypeDef",
     {
         "AddressAllocationIds": List[str],
         "SubnetIds": List[str],
         "VpcEndpointId": str,
         "VpcId": str,
         "SecurityGroupIds": List[str],
     },
+    total=False,
 )
 
 IdentityProviderDetailsOutputTypeDef = TypedDict(
     "IdentityProviderDetailsOutputTypeDef",
     {
         "Url": str,
         "InvocationRole": str,
         "DirectoryId": str,
         "Function": str,
         "SftpAuthenticationMethods": SftpAuthenticationMethodsType,
     },
+    total=False,
 )
 
 ProtocolDetailsOutputTypeDef = TypedDict(
     "ProtocolDetailsOutputTypeDef",
     {
         "PassiveIp": str,
         "TlsSessionResumptionMode": TlsSessionResumptionModeType,
         "SetStatOption": SetStatOptionType,
         "As2Transports": List[Literal["HTTP"]],
     },
+    total=False,
 )
 
 SshPublicKeyTypeDef = TypedDict(
     "SshPublicKeyTypeDef",
     {
         "DateImported": datetime,
         "SshPublicKeyBody": str,
@@ -668,14 +702,15 @@
 
 EfsFileLocationOutputTypeDef = TypedDict(
     "EfsFileLocationOutputTypeDef",
     {
         "FileSystemId": str,
         "Path": str,
     },
+    total=False,
 )
 
 EfsFileLocationTypeDef = TypedDict(
     "EfsFileLocationTypeDef",
     {
         "FileSystemId": str,
         "Path": str,
@@ -695,14 +730,15 @@
     "S3FileLocationTypeDef",
     {
         "Bucket": str,
         "Key": str,
         "VersionId": str,
         "Etag": str,
     },
+    total=False,
 )
 
 ImportSshPublicKeyRequestRequestTypeDef = TypedDict(
     "ImportSshPublicKeyRequestRequestTypeDef",
     {
         "ServerId": str,
         "SshPublicKeyBody": str,
@@ -712,14 +748,15 @@
 
 S3InputFileLocationOutputTypeDef = TypedDict(
     "S3InputFileLocationOutputTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
+    total=False,
 )
 
 S3InputFileLocationTypeDef = TypedDict(
     "S3InputFileLocationTypeDef",
     {
         "Bucket": str,
         "Key": str,
@@ -763,14 +800,15 @@
     "ListedAccessTypeDef",
     {
         "HomeDirectory": str,
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Role": str,
         "ExternalId": str,
     },
+    total=False,
 )
 
 _RequiredListAgreementsRequestRequestTypeDef = TypedDict(
     "_RequiredListAgreementsRequestRequestTypeDef",
     {
         "ServerId": str,
     },
@@ -798,14 +836,15 @@
         "AgreementId": str,
         "Description": str,
         "Status": AgreementStatusTypeType,
         "ServerId": str,
         "LocalProfileId": str,
         "PartnerProfileId": str,
     },
+    total=False,
 )
 
 ListCertificatesRequestRequestTypeDef = TypedDict(
     "ListCertificatesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
@@ -821,14 +860,15 @@
         "Usage": CertificateUsageTypeType,
         "Status": CertificateStatusTypeType,
         "ActiveDate": datetime,
         "InactiveDate": datetime,
         "Type": CertificateTypeType,
         "Description": str,
     },
+    total=False,
 )
 
 ListConnectorsRequestRequestTypeDef = TypedDict(
     "ListConnectorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
@@ -839,14 +879,15 @@
 ListedConnectorTypeDef = TypedDict(
     "ListedConnectorTypeDef",
     {
         "Arn": str,
         "ConnectorId": str,
         "Url": str,
     },
+    total=False,
 )
 
 _RequiredListExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListExecutionsRequestRequestTypeDef",
     {
         "WorkflowId": str,
     },
@@ -885,26 +926,37 @@
 
 class ListHostKeysRequestRequestTypeDef(
     _RequiredListHostKeysRequestRequestTypeDef, _OptionalListHostKeysRequestRequestTypeDef
 ):
     pass
 
 
-ListedHostKeyTypeDef = TypedDict(
-    "ListedHostKeyTypeDef",
+_RequiredListedHostKeyTypeDef = TypedDict(
+    "_RequiredListedHostKeyTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalListedHostKeyTypeDef = TypedDict(
+    "_OptionalListedHostKeyTypeDef",
+    {
         "HostKeyId": str,
         "Fingerprint": str,
         "Description": str,
         "Type": str,
         "DateImported": datetime,
     },
+    total=False,
 )
 
+
+class ListedHostKeyTypeDef(_RequiredListedHostKeyTypeDef, _OptionalListedHostKeyTypeDef):
+    pass
+
+
 ListProfilesRequestRequestTypeDef = TypedDict(
     "ListProfilesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "ProfileType": ProfileTypeType,
     },
@@ -915,14 +967,15 @@
     "ListedProfileTypeDef",
     {
         "Arn": str,
         "ProfileId": str,
         "As2Id": str,
         "ProfileType": ProfileTypeType,
     },
+    total=False,
 )
 
 ListSecurityPoliciesRequestRequestTypeDef = TypedDict(
     "ListSecurityPoliciesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
@@ -935,28 +988,39 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListedServerTypeDef = TypedDict(
-    "ListedServerTypeDef",
+_RequiredListedServerTypeDef = TypedDict(
+    "_RequiredListedServerTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalListedServerTypeDef = TypedDict(
+    "_OptionalListedServerTypeDef",
+    {
         "Domain": DomainType,
         "IdentityProviderType": IdentityProviderTypeType,
         "EndpointType": EndpointTypeType,
         "LoggingRole": str,
         "ServerId": str,
         "State": StateType,
         "UserCount": int,
     },
+    total=False,
 )
 
+
+class ListedServerTypeDef(_RequiredListedServerTypeDef, _OptionalListedServerTypeDef):
+    pass
+
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -994,26 +1058,37 @@
 
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
 
-ListedUserTypeDef = TypedDict(
-    "ListedUserTypeDef",
+_RequiredListedUserTypeDef = TypedDict(
+    "_RequiredListedUserTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalListedUserTypeDef = TypedDict(
+    "_OptionalListedUserTypeDef",
+    {
         "HomeDirectory": str,
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Role": str,
         "SshPublicKeyCount": int,
         "UserName": str,
     },
+    total=False,
 )
 
+
+class ListedUserTypeDef(_RequiredListedUserTypeDef, _OptionalListedUserTypeDef):
+    pass
+
+
 ListWorkflowsRequestRequestTypeDef = TypedDict(
     "ListWorkflowsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1022,14 +1097,15 @@
 ListedWorkflowTypeDef = TypedDict(
     "ListedWorkflowTypeDef",
     {
         "WorkflowId": str,
         "Description": str,
         "Arn": str,
     },
+    total=False,
 )
 
 S3TagOutputTypeDef = TypedDict(
     "S3TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -1050,23 +1126,34 @@
         "WorkflowId": str,
         "ExecutionId": str,
         "Token": str,
         "Status": CustomStepStatusType,
     },
 )
 
-UserDetailsTypeDef = TypedDict(
-    "UserDetailsTypeDef",
+_RequiredUserDetailsTypeDef = TypedDict(
+    "_RequiredUserDetailsTypeDef",
     {
         "UserName": str,
         "ServerId": str,
+    },
+)
+_OptionalUserDetailsTypeDef = TypedDict(
+    "_OptionalUserDetailsTypeDef",
+    {
         "SessionId": str,
     },
+    total=False,
 )
 
+
+class UserDetailsTypeDef(_RequiredUserDetailsTypeDef, _OptionalUserDetailsTypeDef):
+    pass
+
+
 _RequiredStartFileTransferRequestRequestTypeDef = TypedDict(
     "_RequiredStartFileTransferRequestRequestTypeDef",
     {
         "ConnectorId": str,
     },
 )
 _OptionalStartFileTransferRequestRequestTypeDef = TypedDict(
@@ -1761,140 +1848,216 @@
         "HomeDirectoryMappings": List[HomeDirectoryMapEntryOutputTypeDef],
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Policy": str,
         "PosixProfile": PosixProfileOutputTypeDef,
         "Role": str,
         "ExternalId": str,
     },
+    total=False,
 )
 
-DescribedAgreementTypeDef = TypedDict(
-    "DescribedAgreementTypeDef",
+_RequiredDescribedAgreementTypeDef = TypedDict(
+    "_RequiredDescribedAgreementTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalDescribedAgreementTypeDef = TypedDict(
+    "_OptionalDescribedAgreementTypeDef",
+    {
         "AgreementId": str,
         "Description": str,
         "Status": AgreementStatusTypeType,
         "ServerId": str,
         "LocalProfileId": str,
         "PartnerProfileId": str,
         "BaseDirectory": str,
         "AccessRole": str,
         "Tags": List[TagOutputTypeDef],
     },
+    total=False,
 )
 
-DescribedCertificateTypeDef = TypedDict(
-    "DescribedCertificateTypeDef",
+
+class DescribedAgreementTypeDef(
+    _RequiredDescribedAgreementTypeDef, _OptionalDescribedAgreementTypeDef
+):
+    pass
+
+
+_RequiredDescribedCertificateTypeDef = TypedDict(
+    "_RequiredDescribedCertificateTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalDescribedCertificateTypeDef = TypedDict(
+    "_OptionalDescribedCertificateTypeDef",
+    {
         "CertificateId": str,
         "Usage": CertificateUsageTypeType,
         "Status": CertificateStatusTypeType,
         "Certificate": str,
         "CertificateChain": str,
         "ActiveDate": datetime,
         "InactiveDate": datetime,
         "Serial": str,
         "NotBeforeDate": datetime,
         "NotAfterDate": datetime,
         "Type": CertificateTypeType,
         "Description": str,
         "Tags": List[TagOutputTypeDef],
     },
+    total=False,
 )
 
-DescribedHostKeyTypeDef = TypedDict(
-    "DescribedHostKeyTypeDef",
+
+class DescribedCertificateTypeDef(
+    _RequiredDescribedCertificateTypeDef, _OptionalDescribedCertificateTypeDef
+):
+    pass
+
+
+_RequiredDescribedHostKeyTypeDef = TypedDict(
+    "_RequiredDescribedHostKeyTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalDescribedHostKeyTypeDef = TypedDict(
+    "_OptionalDescribedHostKeyTypeDef",
+    {
         "HostKeyId": str,
         "HostKeyFingerprint": str,
         "Description": str,
         "Type": str,
         "DateImported": datetime,
         "Tags": List[TagOutputTypeDef],
     },
+    total=False,
 )
 
-DescribedProfileTypeDef = TypedDict(
-    "DescribedProfileTypeDef",
+
+class DescribedHostKeyTypeDef(_RequiredDescribedHostKeyTypeDef, _OptionalDescribedHostKeyTypeDef):
+    pass
+
+
+_RequiredDescribedProfileTypeDef = TypedDict(
+    "_RequiredDescribedProfileTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalDescribedProfileTypeDef = TypedDict(
+    "_OptionalDescribedProfileTypeDef",
+    {
         "ProfileId": str,
         "ProfileType": ProfileTypeType,
         "As2Id": str,
         "CertificateIds": List[str],
         "Tags": List[TagOutputTypeDef],
     },
+    total=False,
 )
 
+
+class DescribedProfileTypeDef(_RequiredDescribedProfileTypeDef, _OptionalDescribedProfileTypeDef):
+    pass
+
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Arn": str,
         "NextToken": str,
         "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribedConnectorTypeDef = TypedDict(
-    "DescribedConnectorTypeDef",
+_RequiredDescribedConnectorTypeDef = TypedDict(
+    "_RequiredDescribedConnectorTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalDescribedConnectorTypeDef = TypedDict(
+    "_OptionalDescribedConnectorTypeDef",
+    {
         "ConnectorId": str,
         "Url": str,
         "As2Config": As2ConnectorConfigOutputTypeDef,
         "AccessRole": str,
         "LoggingRole": str,
         "Tags": List[TagOutputTypeDef],
         "SftpConfig": SftpConnectorConfigOutputTypeDef,
     },
+    total=False,
 )
 
-DescribedUserTypeDef = TypedDict(
-    "DescribedUserTypeDef",
+
+class DescribedConnectorTypeDef(
+    _RequiredDescribedConnectorTypeDef, _OptionalDescribedConnectorTypeDef
+):
+    pass
+
+
+_RequiredDescribedUserTypeDef = TypedDict(
+    "_RequiredDescribedUserTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalDescribedUserTypeDef = TypedDict(
+    "_OptionalDescribedUserTypeDef",
+    {
         "HomeDirectory": str,
         "HomeDirectoryMappings": List[HomeDirectoryMapEntryOutputTypeDef],
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Policy": str,
         "PosixProfile": PosixProfileOutputTypeDef,
         "Role": str,
         "SshPublicKeys": List[SshPublicKeyTypeDef],
         "Tags": List[TagOutputTypeDef],
         "UserName": str,
     },
+    total=False,
 )
 
+
+class DescribedUserTypeDef(_RequiredDescribedUserTypeDef, _OptionalDescribedUserTypeDef):
+    pass
+
+
 ExecutionStepResultTypeDef = TypedDict(
     "ExecutionStepResultTypeDef",
     {
         "StepType": WorkflowStepTypeType,
         "Outputs": str,
         "Error": ExecutionErrorTypeDef,
     },
+    total=False,
 )
 
 FileLocationTypeDef = TypedDict(
     "FileLocationTypeDef",
     {
         "S3FileLocation": S3FileLocationTypeDef,
         "EfsFileLocation": EfsFileLocationOutputTypeDef,
     },
+    total=False,
 )
 
 InputFileLocationOutputTypeDef = TypedDict(
     "InputFileLocationOutputTypeDef",
     {
         "S3FileLocation": S3InputFileLocationOutputTypeDef,
         "EfsFileLocation": EfsFileLocationOutputTypeDef,
     },
+    total=False,
 )
 
 InputFileLocationTypeDef = TypedDict(
     "InputFileLocationTypeDef",
     {
         "S3FileLocation": S3InputFileLocationTypeDef,
         "EfsFileLocation": EfsFileLocationTypeDef,
@@ -2148,14 +2311,15 @@
 TagStepDetailsOutputTypeDef = TypedDict(
     "TagStepDetailsOutputTypeDef",
     {
         "Name": str,
         "Tags": List[S3TagOutputTypeDef],
         "SourceFileLocation": str,
     },
+    total=False,
 )
 
 TagStepDetailsTypeDef = TypedDict(
     "TagStepDetailsTypeDef",
     {
         "Name": str,
         "Tags": Sequence[S3TagTypeDef],
@@ -2173,14 +2337,15 @@
 
 WorkflowDetailsOutputTypeDef = TypedDict(
     "WorkflowDetailsOutputTypeDef",
     {
         "OnUpload": List[WorkflowDetailOutputTypeDef],
         "OnPartialUpload": List[WorkflowDetailOutputTypeDef],
     },
+    total=False,
 )
 
 WorkflowDetailsTypeDef = TypedDict(
     "WorkflowDetailsTypeDef",
     {
         "OnUpload": Sequence[WorkflowDetailTypeDef],
         "OnPartialUpload": Sequence[WorkflowDetailTypeDef],
@@ -2248,37 +2413,52 @@
 
 ExecutionResultsTypeDef = TypedDict(
     "ExecutionResultsTypeDef",
     {
         "Steps": List[ExecutionStepResultTypeDef],
         "OnExceptionSteps": List[ExecutionStepResultTypeDef],
     },
+    total=False,
 )
 
 CopyStepDetailsOutputTypeDef = TypedDict(
     "CopyStepDetailsOutputTypeDef",
     {
         "Name": str,
         "DestinationFileLocation": InputFileLocationOutputTypeDef,
         "OverwriteExisting": OverwriteExistingType,
         "SourceFileLocation": str,
     },
+    total=False,
 )
 
-DecryptStepDetailsOutputTypeDef = TypedDict(
-    "DecryptStepDetailsOutputTypeDef",
+_RequiredDecryptStepDetailsOutputTypeDef = TypedDict(
+    "_RequiredDecryptStepDetailsOutputTypeDef",
     {
-        "Name": str,
         "Type": Literal["PGP"],
+        "DestinationFileLocation": InputFileLocationOutputTypeDef,
+    },
+)
+_OptionalDecryptStepDetailsOutputTypeDef = TypedDict(
+    "_OptionalDecryptStepDetailsOutputTypeDef",
+    {
+        "Name": str,
         "SourceFileLocation": str,
         "OverwriteExisting": OverwriteExistingType,
-        "DestinationFileLocation": InputFileLocationOutputTypeDef,
     },
+    total=False,
 )
 
+
+class DecryptStepDetailsOutputTypeDef(
+    _RequiredDecryptStepDetailsOutputTypeDef, _OptionalDecryptStepDetailsOutputTypeDef
+):
+    pass
+
+
 CopyStepDetailsTypeDef = TypedDict(
     "CopyStepDetailsTypeDef",
     {
         "Name": str,
         "DestinationFileLocation": InputFileLocationTypeDef,
         "OverwriteExisting": OverwriteExistingType,
         "SourceFileLocation": str,
@@ -2314,20 +2494,26 @@
     "ListedExecutionTypeDef",
     {
         "ExecutionId": str,
         "InitialFileLocation": FileLocationTypeDef,
         "ServiceMetadata": ServiceMetadataTypeDef,
         "Status": ExecutionStatusType,
     },
+    total=False,
 )
 
-DescribedServerTypeDef = TypedDict(
-    "DescribedServerTypeDef",
+_RequiredDescribedServerTypeDef = TypedDict(
+    "_RequiredDescribedServerTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalDescribedServerTypeDef = TypedDict(
+    "_OptionalDescribedServerTypeDef",
+    {
         "Certificate": str,
         "ProtocolDetails": ProtocolDetailsOutputTypeDef,
         "Domain": DomainType,
         "EndpointDetails": EndpointDetailsOutputTypeDef,
         "EndpointType": EndpointTypeType,
         "HostKeyFingerprint": str,
         "IdentityProviderDetails": IdentityProviderDetailsOutputTypeDef,
@@ -2340,16 +2526,22 @@
         "ServerId": str,
         "State": StateType,
         "Tags": List[TagOutputTypeDef],
         "UserCount": int,
         "WorkflowDetails": WorkflowDetailsOutputTypeDef,
         "StructuredLogDestinations": List[str],
     },
+    total=False,
 )
 
+
+class DescribedServerTypeDef(_RequiredDescribedServerTypeDef, _OptionalDescribedServerTypeDef):
+    pass
+
+
 CreateServerRequestRequestTypeDef = TypedDict(
     "CreateServerRequestRequestTypeDef",
     {
         "Certificate": str,
         "Domain": DomainType,
         "EndpointDetails": EndpointDetailsTypeDef,
         "EndpointType": EndpointTypeType,
@@ -2410,26 +2602,28 @@
         "ServiceMetadata": ServiceMetadataTypeDef,
         "ExecutionRole": str,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
         "PosixProfile": PosixProfileOutputTypeDef,
         "Status": ExecutionStatusType,
         "Results": ExecutionResultsTypeDef,
     },
+    total=False,
 )
 
 WorkflowStepOutputTypeDef = TypedDict(
     "WorkflowStepOutputTypeDef",
     {
         "Type": WorkflowStepTypeType,
         "CopyStepDetails": CopyStepDetailsOutputTypeDef,
         "CustomStepDetails": CustomStepDetailsOutputTypeDef,
         "DeleteStepDetails": DeleteStepDetailsOutputTypeDef,
         "TagStepDetails": TagStepDetailsOutputTypeDef,
         "DecryptStepDetails": DecryptStepDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 WorkflowStepTypeDef = TypedDict(
     "WorkflowStepTypeDef",
     {
         "Type": WorkflowStepTypeType,
         "CopyStepDetails": CopyStepDetailsTypeDef,
@@ -2464,26 +2658,39 @@
     {
         "WorkflowId": str,
         "Execution": DescribedExecutionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribedWorkflowTypeDef = TypedDict(
-    "DescribedWorkflowTypeDef",
+_RequiredDescribedWorkflowTypeDef = TypedDict(
+    "_RequiredDescribedWorkflowTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalDescribedWorkflowTypeDef = TypedDict(
+    "_OptionalDescribedWorkflowTypeDef",
+    {
         "Description": str,
         "Steps": List[WorkflowStepOutputTypeDef],
         "OnExceptionSteps": List[WorkflowStepOutputTypeDef],
         "WorkflowId": str,
         "Tags": List[TagOutputTypeDef],
     },
+    total=False,
 )
 
+
+class DescribedWorkflowTypeDef(
+    _RequiredDescribedWorkflowTypeDef, _OptionalDescribedWorkflowTypeDef
+):
+    pass
+
+
 _RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowRequestRequestTypeDef",
     {
         "Steps": Sequence[WorkflowStepTypeDef],
     },
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/type_defs.pyi` & `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -253,14 +253,15 @@
         "Compression": CompressionEnumType,
         "EncryptionAlgorithm": EncryptionAlgType,
         "SigningAlgorithm": SigningAlgType,
         "MdnSigningAlgorithm": MdnSigningAlgType,
         "MdnResponse": MdnResponseType,
         "BasicAuthSecretId": str,
     },
+    total=False,
 )
 
 As2ConnectorConfigTypeDef = TypedDict(
     "As2ConnectorConfigTypeDef",
     {
         "LocalProfileId": str,
         "PartnerProfileId": str,
@@ -368,14 +369,15 @@
     "CustomStepDetailsOutputTypeDef",
     {
         "Name": str,
         "Target": str,
         "TimeoutSeconds": int,
         "SourceFileLocation": str,
     },
+    total=False,
 )
 
 CustomStepDetailsTypeDef = TypedDict(
     "CustomStepDetailsTypeDef",
     {
         "Name": str,
         "Target": str,
@@ -448,14 +450,15 @@
 
 DeleteStepDetailsOutputTypeDef = TypedDict(
     "DeleteStepDetailsOutputTypeDef",
     {
         "Name": str,
         "SourceFileLocation": str,
     },
+    total=False,
 )
 
 DeleteStepDetailsTypeDef = TypedDict(
     "DeleteStepDetailsTypeDef",
     {
         "Name": str,
         "SourceFileLocation": str,
@@ -534,26 +537,37 @@
 DescribeSecurityPolicyRequestRequestTypeDef = TypedDict(
     "DescribeSecurityPolicyRequestRequestTypeDef",
     {
         "SecurityPolicyName": str,
     },
 )
 
-DescribedSecurityPolicyTypeDef = TypedDict(
-    "DescribedSecurityPolicyTypeDef",
+_RequiredDescribedSecurityPolicyTypeDef = TypedDict(
+    "_RequiredDescribedSecurityPolicyTypeDef",
     {
-        "Fips": bool,
         "SecurityPolicyName": str,
+    },
+)
+_OptionalDescribedSecurityPolicyTypeDef = TypedDict(
+    "_OptionalDescribedSecurityPolicyTypeDef",
+    {
+        "Fips": bool,
         "SshCiphers": List[str],
         "SshKexs": List[str],
         "SshMacs": List[str],
         "TlsCiphers": List[str],
     },
+    total=False,
 )
 
+class DescribedSecurityPolicyTypeDef(
+    _RequiredDescribedSecurityPolicyTypeDef, _OptionalDescribedSecurityPolicyTypeDef
+):
+    pass
+
 DescribeServerRequestRequestTypeDef = TypedDict(
     "DescribeServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 
@@ -585,77 +599,93 @@
     "HomeDirectoryMapEntryOutputTypeDef",
     {
         "Entry": str,
         "Target": str,
     },
 )
 
-PosixProfileOutputTypeDef = TypedDict(
-    "PosixProfileOutputTypeDef",
+_RequiredPosixProfileOutputTypeDef = TypedDict(
+    "_RequiredPosixProfileOutputTypeDef",
     {
         "Uid": int,
         "Gid": int,
+    },
+)
+_OptionalPosixProfileOutputTypeDef = TypedDict(
+    "_OptionalPosixProfileOutputTypeDef",
+    {
         "SecondaryGids": List[int],
     },
+    total=False,
 )
 
+class PosixProfileOutputTypeDef(
+    _RequiredPosixProfileOutputTypeDef, _OptionalPosixProfileOutputTypeDef
+):
+    pass
+
 TagOutputTypeDef = TypedDict(
     "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
 SftpConnectorConfigOutputTypeDef = TypedDict(
     "SftpConnectorConfigOutputTypeDef",
     {
         "UserSecretId": str,
         "TrustedHostKeys": List[str],
     },
+    total=False,
 )
 
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
         "LoggingRole": str,
         "LogGroupName": str,
     },
+    total=False,
 )
 
 EndpointDetailsOutputTypeDef = TypedDict(
     "EndpointDetailsOutputTypeDef",
     {
         "AddressAllocationIds": List[str],
         "SubnetIds": List[str],
         "VpcEndpointId": str,
         "VpcId": str,
         "SecurityGroupIds": List[str],
     },
+    total=False,
 )
 
 IdentityProviderDetailsOutputTypeDef = TypedDict(
     "IdentityProviderDetailsOutputTypeDef",
     {
         "Url": str,
         "InvocationRole": str,
         "DirectoryId": str,
         "Function": str,
         "SftpAuthenticationMethods": SftpAuthenticationMethodsType,
     },
+    total=False,
 )
 
 ProtocolDetailsOutputTypeDef = TypedDict(
     "ProtocolDetailsOutputTypeDef",
     {
         "PassiveIp": str,
         "TlsSessionResumptionMode": TlsSessionResumptionModeType,
         "SetStatOption": SetStatOptionType,
         "As2Transports": List[Literal["HTTP"]],
     },
+    total=False,
 )
 
 SshPublicKeyTypeDef = TypedDict(
     "SshPublicKeyTypeDef",
     {
         "DateImported": datetime,
         "SshPublicKeyBody": str,
@@ -665,14 +695,15 @@
 
 EfsFileLocationOutputTypeDef = TypedDict(
     "EfsFileLocationOutputTypeDef",
     {
         "FileSystemId": str,
         "Path": str,
     },
+    total=False,
 )
 
 EfsFileLocationTypeDef = TypedDict(
     "EfsFileLocationTypeDef",
     {
         "FileSystemId": str,
         "Path": str,
@@ -692,14 +723,15 @@
     "S3FileLocationTypeDef",
     {
         "Bucket": str,
         "Key": str,
         "VersionId": str,
         "Etag": str,
     },
+    total=False,
 )
 
 ImportSshPublicKeyRequestRequestTypeDef = TypedDict(
     "ImportSshPublicKeyRequestRequestTypeDef",
     {
         "ServerId": str,
         "SshPublicKeyBody": str,
@@ -709,14 +741,15 @@
 
 S3InputFileLocationOutputTypeDef = TypedDict(
     "S3InputFileLocationOutputTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
+    total=False,
 )
 
 S3InputFileLocationTypeDef = TypedDict(
     "S3InputFileLocationTypeDef",
     {
         "Bucket": str,
         "Key": str,
@@ -758,14 +791,15 @@
     "ListedAccessTypeDef",
     {
         "HomeDirectory": str,
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Role": str,
         "ExternalId": str,
     },
+    total=False,
 )
 
 _RequiredListAgreementsRequestRequestTypeDef = TypedDict(
     "_RequiredListAgreementsRequestRequestTypeDef",
     {
         "ServerId": str,
     },
@@ -791,14 +825,15 @@
         "AgreementId": str,
         "Description": str,
         "Status": AgreementStatusTypeType,
         "ServerId": str,
         "LocalProfileId": str,
         "PartnerProfileId": str,
     },
+    total=False,
 )
 
 ListCertificatesRequestRequestTypeDef = TypedDict(
     "ListCertificatesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
@@ -814,14 +849,15 @@
         "Usage": CertificateUsageTypeType,
         "Status": CertificateStatusTypeType,
         "ActiveDate": datetime,
         "InactiveDate": datetime,
         "Type": CertificateTypeType,
         "Description": str,
     },
+    total=False,
 )
 
 ListConnectorsRequestRequestTypeDef = TypedDict(
     "ListConnectorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
@@ -832,14 +868,15 @@
 ListedConnectorTypeDef = TypedDict(
     "ListedConnectorTypeDef",
     {
         "Arn": str,
         "ConnectorId": str,
         "Url": str,
     },
+    total=False,
 )
 
 _RequiredListExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListExecutionsRequestRequestTypeDef",
     {
         "WorkflowId": str,
     },
@@ -874,26 +911,35 @@
 )
 
 class ListHostKeysRequestRequestTypeDef(
     _RequiredListHostKeysRequestRequestTypeDef, _OptionalListHostKeysRequestRequestTypeDef
 ):
     pass
 
-ListedHostKeyTypeDef = TypedDict(
-    "ListedHostKeyTypeDef",
+_RequiredListedHostKeyTypeDef = TypedDict(
+    "_RequiredListedHostKeyTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalListedHostKeyTypeDef = TypedDict(
+    "_OptionalListedHostKeyTypeDef",
+    {
         "HostKeyId": str,
         "Fingerprint": str,
         "Description": str,
         "Type": str,
         "DateImported": datetime,
     },
+    total=False,
 )
 
+class ListedHostKeyTypeDef(_RequiredListedHostKeyTypeDef, _OptionalListedHostKeyTypeDef):
+    pass
+
 ListProfilesRequestRequestTypeDef = TypedDict(
     "ListProfilesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "ProfileType": ProfileTypeType,
     },
@@ -904,14 +950,15 @@
     "ListedProfileTypeDef",
     {
         "Arn": str,
         "ProfileId": str,
         "As2Id": str,
         "ProfileType": ProfileTypeType,
     },
+    total=False,
 )
 
 ListSecurityPoliciesRequestRequestTypeDef = TypedDict(
     "ListSecurityPoliciesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
@@ -924,28 +971,37 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListedServerTypeDef = TypedDict(
-    "ListedServerTypeDef",
+_RequiredListedServerTypeDef = TypedDict(
+    "_RequiredListedServerTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalListedServerTypeDef = TypedDict(
+    "_OptionalListedServerTypeDef",
+    {
         "Domain": DomainType,
         "IdentityProviderType": IdentityProviderTypeType,
         "EndpointType": EndpointTypeType,
         "LoggingRole": str,
         "ServerId": str,
         "State": StateType,
         "UserCount": int,
     },
+    total=False,
 )
 
+class ListedServerTypeDef(_RequiredListedServerTypeDef, _OptionalListedServerTypeDef):
+    pass
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -979,26 +1035,35 @@
 )
 
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
-ListedUserTypeDef = TypedDict(
-    "ListedUserTypeDef",
+_RequiredListedUserTypeDef = TypedDict(
+    "_RequiredListedUserTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalListedUserTypeDef = TypedDict(
+    "_OptionalListedUserTypeDef",
+    {
         "HomeDirectory": str,
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Role": str,
         "SshPublicKeyCount": int,
         "UserName": str,
     },
+    total=False,
 )
 
+class ListedUserTypeDef(_RequiredListedUserTypeDef, _OptionalListedUserTypeDef):
+    pass
+
 ListWorkflowsRequestRequestTypeDef = TypedDict(
     "ListWorkflowsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1007,14 +1072,15 @@
 ListedWorkflowTypeDef = TypedDict(
     "ListedWorkflowTypeDef",
     {
         "WorkflowId": str,
         "Description": str,
         "Arn": str,
     },
+    total=False,
 )
 
 S3TagOutputTypeDef = TypedDict(
     "S3TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -1035,23 +1101,32 @@
         "WorkflowId": str,
         "ExecutionId": str,
         "Token": str,
         "Status": CustomStepStatusType,
     },
 )
 
-UserDetailsTypeDef = TypedDict(
-    "UserDetailsTypeDef",
+_RequiredUserDetailsTypeDef = TypedDict(
+    "_RequiredUserDetailsTypeDef",
     {
         "UserName": str,
         "ServerId": str,
+    },
+)
+_OptionalUserDetailsTypeDef = TypedDict(
+    "_OptionalUserDetailsTypeDef",
+    {
         "SessionId": str,
     },
+    total=False,
 )
 
+class UserDetailsTypeDef(_RequiredUserDetailsTypeDef, _OptionalUserDetailsTypeDef):
+    pass
+
 _RequiredStartFileTransferRequestRequestTypeDef = TypedDict(
     "_RequiredStartFileTransferRequestRequestTypeDef",
     {
         "ConnectorId": str,
     },
 )
 _OptionalStartFileTransferRequestRequestTypeDef = TypedDict(
@@ -1712,140 +1787,204 @@
         "HomeDirectoryMappings": List[HomeDirectoryMapEntryOutputTypeDef],
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Policy": str,
         "PosixProfile": PosixProfileOutputTypeDef,
         "Role": str,
         "ExternalId": str,
     },
+    total=False,
 )
 
-DescribedAgreementTypeDef = TypedDict(
-    "DescribedAgreementTypeDef",
+_RequiredDescribedAgreementTypeDef = TypedDict(
+    "_RequiredDescribedAgreementTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalDescribedAgreementTypeDef = TypedDict(
+    "_OptionalDescribedAgreementTypeDef",
+    {
         "AgreementId": str,
         "Description": str,
         "Status": AgreementStatusTypeType,
         "ServerId": str,
         "LocalProfileId": str,
         "PartnerProfileId": str,
         "BaseDirectory": str,
         "AccessRole": str,
         "Tags": List[TagOutputTypeDef],
     },
+    total=False,
 )
 
-DescribedCertificateTypeDef = TypedDict(
-    "DescribedCertificateTypeDef",
+class DescribedAgreementTypeDef(
+    _RequiredDescribedAgreementTypeDef, _OptionalDescribedAgreementTypeDef
+):
+    pass
+
+_RequiredDescribedCertificateTypeDef = TypedDict(
+    "_RequiredDescribedCertificateTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalDescribedCertificateTypeDef = TypedDict(
+    "_OptionalDescribedCertificateTypeDef",
+    {
         "CertificateId": str,
         "Usage": CertificateUsageTypeType,
         "Status": CertificateStatusTypeType,
         "Certificate": str,
         "CertificateChain": str,
         "ActiveDate": datetime,
         "InactiveDate": datetime,
         "Serial": str,
         "NotBeforeDate": datetime,
         "NotAfterDate": datetime,
         "Type": CertificateTypeType,
         "Description": str,
         "Tags": List[TagOutputTypeDef],
     },
+    total=False,
 )
 
-DescribedHostKeyTypeDef = TypedDict(
-    "DescribedHostKeyTypeDef",
+class DescribedCertificateTypeDef(
+    _RequiredDescribedCertificateTypeDef, _OptionalDescribedCertificateTypeDef
+):
+    pass
+
+_RequiredDescribedHostKeyTypeDef = TypedDict(
+    "_RequiredDescribedHostKeyTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalDescribedHostKeyTypeDef = TypedDict(
+    "_OptionalDescribedHostKeyTypeDef",
+    {
         "HostKeyId": str,
         "HostKeyFingerprint": str,
         "Description": str,
         "Type": str,
         "DateImported": datetime,
         "Tags": List[TagOutputTypeDef],
     },
+    total=False,
 )
 
-DescribedProfileTypeDef = TypedDict(
-    "DescribedProfileTypeDef",
+class DescribedHostKeyTypeDef(_RequiredDescribedHostKeyTypeDef, _OptionalDescribedHostKeyTypeDef):
+    pass
+
+_RequiredDescribedProfileTypeDef = TypedDict(
+    "_RequiredDescribedProfileTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalDescribedProfileTypeDef = TypedDict(
+    "_OptionalDescribedProfileTypeDef",
+    {
         "ProfileId": str,
         "ProfileType": ProfileTypeType,
         "As2Id": str,
         "CertificateIds": List[str],
         "Tags": List[TagOutputTypeDef],
     },
+    total=False,
 )
 
+class DescribedProfileTypeDef(_RequiredDescribedProfileTypeDef, _OptionalDescribedProfileTypeDef):
+    pass
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Arn": str,
         "NextToken": str,
         "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribedConnectorTypeDef = TypedDict(
-    "DescribedConnectorTypeDef",
+_RequiredDescribedConnectorTypeDef = TypedDict(
+    "_RequiredDescribedConnectorTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalDescribedConnectorTypeDef = TypedDict(
+    "_OptionalDescribedConnectorTypeDef",
+    {
         "ConnectorId": str,
         "Url": str,
         "As2Config": As2ConnectorConfigOutputTypeDef,
         "AccessRole": str,
         "LoggingRole": str,
         "Tags": List[TagOutputTypeDef],
         "SftpConfig": SftpConnectorConfigOutputTypeDef,
     },
+    total=False,
 )
 
-DescribedUserTypeDef = TypedDict(
-    "DescribedUserTypeDef",
+class DescribedConnectorTypeDef(
+    _RequiredDescribedConnectorTypeDef, _OptionalDescribedConnectorTypeDef
+):
+    pass
+
+_RequiredDescribedUserTypeDef = TypedDict(
+    "_RequiredDescribedUserTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalDescribedUserTypeDef = TypedDict(
+    "_OptionalDescribedUserTypeDef",
+    {
         "HomeDirectory": str,
         "HomeDirectoryMappings": List[HomeDirectoryMapEntryOutputTypeDef],
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Policy": str,
         "PosixProfile": PosixProfileOutputTypeDef,
         "Role": str,
         "SshPublicKeys": List[SshPublicKeyTypeDef],
         "Tags": List[TagOutputTypeDef],
         "UserName": str,
     },
+    total=False,
 )
 
+class DescribedUserTypeDef(_RequiredDescribedUserTypeDef, _OptionalDescribedUserTypeDef):
+    pass
+
 ExecutionStepResultTypeDef = TypedDict(
     "ExecutionStepResultTypeDef",
     {
         "StepType": WorkflowStepTypeType,
         "Outputs": str,
         "Error": ExecutionErrorTypeDef,
     },
+    total=False,
 )
 
 FileLocationTypeDef = TypedDict(
     "FileLocationTypeDef",
     {
         "S3FileLocation": S3FileLocationTypeDef,
         "EfsFileLocation": EfsFileLocationOutputTypeDef,
     },
+    total=False,
 )
 
 InputFileLocationOutputTypeDef = TypedDict(
     "InputFileLocationOutputTypeDef",
     {
         "S3FileLocation": S3InputFileLocationOutputTypeDef,
         "EfsFileLocation": EfsFileLocationOutputTypeDef,
     },
+    total=False,
 )
 
 InputFileLocationTypeDef = TypedDict(
     "InputFileLocationTypeDef",
     {
         "S3FileLocation": S3InputFileLocationTypeDef,
         "EfsFileLocation": EfsFileLocationTypeDef,
@@ -2089,14 +2228,15 @@
 TagStepDetailsOutputTypeDef = TypedDict(
     "TagStepDetailsOutputTypeDef",
     {
         "Name": str,
         "Tags": List[S3TagOutputTypeDef],
         "SourceFileLocation": str,
     },
+    total=False,
 )
 
 TagStepDetailsTypeDef = TypedDict(
     "TagStepDetailsTypeDef",
     {
         "Name": str,
         "Tags": Sequence[S3TagTypeDef],
@@ -2114,14 +2254,15 @@
 
 WorkflowDetailsOutputTypeDef = TypedDict(
     "WorkflowDetailsOutputTypeDef",
     {
         "OnUpload": List[WorkflowDetailOutputTypeDef],
         "OnPartialUpload": List[WorkflowDetailOutputTypeDef],
     },
+    total=False,
 )
 
 WorkflowDetailsTypeDef = TypedDict(
     "WorkflowDetailsTypeDef",
     {
         "OnUpload": Sequence[WorkflowDetailTypeDef],
         "OnPartialUpload": Sequence[WorkflowDetailTypeDef],
@@ -2189,37 +2330,50 @@
 
 ExecutionResultsTypeDef = TypedDict(
     "ExecutionResultsTypeDef",
     {
         "Steps": List[ExecutionStepResultTypeDef],
         "OnExceptionSteps": List[ExecutionStepResultTypeDef],
     },
+    total=False,
 )
 
 CopyStepDetailsOutputTypeDef = TypedDict(
     "CopyStepDetailsOutputTypeDef",
     {
         "Name": str,
         "DestinationFileLocation": InputFileLocationOutputTypeDef,
         "OverwriteExisting": OverwriteExistingType,
         "SourceFileLocation": str,
     },
+    total=False,
 )
 
-DecryptStepDetailsOutputTypeDef = TypedDict(
-    "DecryptStepDetailsOutputTypeDef",
+_RequiredDecryptStepDetailsOutputTypeDef = TypedDict(
+    "_RequiredDecryptStepDetailsOutputTypeDef",
     {
-        "Name": str,
         "Type": Literal["PGP"],
+        "DestinationFileLocation": InputFileLocationOutputTypeDef,
+    },
+)
+_OptionalDecryptStepDetailsOutputTypeDef = TypedDict(
+    "_OptionalDecryptStepDetailsOutputTypeDef",
+    {
+        "Name": str,
         "SourceFileLocation": str,
         "OverwriteExisting": OverwriteExistingType,
-        "DestinationFileLocation": InputFileLocationOutputTypeDef,
     },
+    total=False,
 )
 
+class DecryptStepDetailsOutputTypeDef(
+    _RequiredDecryptStepDetailsOutputTypeDef, _OptionalDecryptStepDetailsOutputTypeDef
+):
+    pass
+
 CopyStepDetailsTypeDef = TypedDict(
     "CopyStepDetailsTypeDef",
     {
         "Name": str,
         "DestinationFileLocation": InputFileLocationTypeDef,
         "OverwriteExisting": OverwriteExistingType,
         "SourceFileLocation": str,
@@ -2253,20 +2407,26 @@
     "ListedExecutionTypeDef",
     {
         "ExecutionId": str,
         "InitialFileLocation": FileLocationTypeDef,
         "ServiceMetadata": ServiceMetadataTypeDef,
         "Status": ExecutionStatusType,
     },
+    total=False,
 )
 
-DescribedServerTypeDef = TypedDict(
-    "DescribedServerTypeDef",
+_RequiredDescribedServerTypeDef = TypedDict(
+    "_RequiredDescribedServerTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalDescribedServerTypeDef = TypedDict(
+    "_OptionalDescribedServerTypeDef",
+    {
         "Certificate": str,
         "ProtocolDetails": ProtocolDetailsOutputTypeDef,
         "Domain": DomainType,
         "EndpointDetails": EndpointDetailsOutputTypeDef,
         "EndpointType": EndpointTypeType,
         "HostKeyFingerprint": str,
         "IdentityProviderDetails": IdentityProviderDetailsOutputTypeDef,
@@ -2279,16 +2439,20 @@
         "ServerId": str,
         "State": StateType,
         "Tags": List[TagOutputTypeDef],
         "UserCount": int,
         "WorkflowDetails": WorkflowDetailsOutputTypeDef,
         "StructuredLogDestinations": List[str],
     },
+    total=False,
 )
 
+class DescribedServerTypeDef(_RequiredDescribedServerTypeDef, _OptionalDescribedServerTypeDef):
+    pass
+
 CreateServerRequestRequestTypeDef = TypedDict(
     "CreateServerRequestRequestTypeDef",
     {
         "Certificate": str,
         "Domain": DomainType,
         "EndpointDetails": EndpointDetailsTypeDef,
         "EndpointType": EndpointTypeType,
@@ -2347,26 +2511,28 @@
         "ServiceMetadata": ServiceMetadataTypeDef,
         "ExecutionRole": str,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
         "PosixProfile": PosixProfileOutputTypeDef,
         "Status": ExecutionStatusType,
         "Results": ExecutionResultsTypeDef,
     },
+    total=False,
 )
 
 WorkflowStepOutputTypeDef = TypedDict(
     "WorkflowStepOutputTypeDef",
     {
         "Type": WorkflowStepTypeType,
         "CopyStepDetails": CopyStepDetailsOutputTypeDef,
         "CustomStepDetails": CustomStepDetailsOutputTypeDef,
         "DeleteStepDetails": DeleteStepDetailsOutputTypeDef,
         "TagStepDetails": TagStepDetailsOutputTypeDef,
         "DecryptStepDetails": DecryptStepDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 WorkflowStepTypeDef = TypedDict(
     "WorkflowStepTypeDef",
     {
         "Type": WorkflowStepTypeType,
         "CopyStepDetails": CopyStepDetailsTypeDef,
@@ -2401,26 +2567,37 @@
     {
         "WorkflowId": str,
         "Execution": DescribedExecutionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribedWorkflowTypeDef = TypedDict(
-    "DescribedWorkflowTypeDef",
+_RequiredDescribedWorkflowTypeDef = TypedDict(
+    "_RequiredDescribedWorkflowTypeDef",
     {
         "Arn": str,
+    },
+)
+_OptionalDescribedWorkflowTypeDef = TypedDict(
+    "_OptionalDescribedWorkflowTypeDef",
+    {
         "Description": str,
         "Steps": List[WorkflowStepOutputTypeDef],
         "OnExceptionSteps": List[WorkflowStepOutputTypeDef],
         "WorkflowId": str,
         "Tags": List[TagOutputTypeDef],
     },
+    total=False,
 )
 
+class DescribedWorkflowTypeDef(
+    _RequiredDescribedWorkflowTypeDef, _OptionalDescribedWorkflowTypeDef
+):
+    pass
+
 _RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowRequestRequestTypeDef",
     {
         "Steps": Sequence[WorkflowStepTypeDef],
     },
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/waiter.py` & `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer/waiter.pyi` & `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer.egg-info/PKG-INFO` & `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transfer
-Version: 1.28.11
-Summary: Type annotations for boto3.Transfer 1.28.11 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.Transfer 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-transfer"></a>
 
 # mypy-boto3-transfer
 
 [![PyPI - mypy-boto3-transfer](https://img.shields.io/pypi/v/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transfer?color=blue)](https://pypistats.org/packages/mypy-boto3-transfer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transfer)](https://pepy.tech/project/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
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
 [mypy-boto3-transfer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-transfer-1.28.11/mypy_boto3_transfer.egg-info/SOURCES.txt` & `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.11/setup.py` & `mypy-boto3-transfer-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-transfer",
-    version="1.28.11",
+    version="1.28.12",
     packages=["mypy_boto3_transfer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Transfer 1.28.11 service generated with mypy-boto3-builder"
-        " 7.15.1"
+        "Type annotations for boto3.Transfer 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

