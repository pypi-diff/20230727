# Comparing `tmp/mypy-boto3-qldb-1.28.0.tar.gz` & `tmp/mypy-boto3-qldb-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-qldb-1.28.0.tar", last modified: Thu Jul  6 21:00:22 2023, max compression
+gzip compressed data, was "mypy-boto3-qldb-1.28.12.tar", last modified: Thu Jul 27 11:49:27 2023, max compression
```

## Comparing `mypy-boto3-qldb-1.28.0.tar` & `mypy-boto3-qldb-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:22.022399 mypy-boto3-qldb-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:49:55.000000 mypy-boto3-qldb-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13774 2023-07-06 21:00:22.022399 mypy-boto3-qldb-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-07-06 20:49:55.000000 mypy-boto3-qldb-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:22.022399 mypy-boto3-qldb-1.28.0/mypy_boto3_qldb/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-06 20:49:55.000000 mypy-boto3-qldb-1.28.0/mypy_boto3_qldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-06 20:49:55.000000 mypy-boto3-qldb-1.28.0/mypy_boto3_qldb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-06 20:49:55.000000 mypy-boto3-qldb-1.28.0/mypy_boto3_qldb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15217 2023-07-06 20:49:55.000000 mypy-boto3-qldb-1.28.0/mypy_boto3_qldb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-07-06 20:49:55.000000 mypy-boto3-qldb-1.28.0/mypy_boto3_qldb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-07-06 20:49:55.000000 mypy-boto3-qldb-1.28.0/mypy_boto3_qldb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-07-06 20:49:55.000000 mypy-boto3-qldb-1.28.0/mypy_boto3_qldb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:49:55.000000 mypy-boto3-qldb-1.28.0/mypy_boto3_qldb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17789 2023-07-06 20:49:56.000000 mypy-boto3-qldb-1.28.0/mypy_boto3_qldb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17762 2023-07-06 20:49:56.000000 mypy-boto3-qldb-1.28.0/mypy_boto3_qldb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:49:55.000000 mypy-boto3-qldb-1.28.0/mypy_boto3_qldb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:22.022399 mypy-boto3-qldb-1.28.0/mypy_boto3_qldb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13774 2023-07-06 21:00:21.000000 mypy-boto3-qldb-1.28.0/mypy_boto3_qldb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-06 21:00:21.000000 mypy-boto3-qldb-1.28.0/mypy_boto3_qldb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:21.000000 mypy-boto3-qldb-1.28.0/mypy_boto3_qldb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:21.000000 mypy-boto3-qldb-1.28.0/mypy_boto3_qldb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:21.000000 mypy-boto3-qldb-1.28.0/mypy_boto3_qldb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 21:00:21.000000 mypy-boto3-qldb-1.28.0/mypy_boto3_qldb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:22.022399 mypy-boto3-qldb-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-06 20:49:55.000000 mypy-boto3-qldb-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.497187 mypy-boto3-qldb-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-07-27 11:49:27.497187 mypy-boto3-qldb-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.485187 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15217 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-07-27 11:41:52.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19276 2023-07-27 11:41:52.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.497187 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-07-27 11:49:27.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-27 11:49:27.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:27.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 11:49:27.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:27.497187 mypy-boto3-qldb-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/setup.py
```

### Comparing `mypy-boto3-qldb-1.28.0/LICENSE` & `mypy-boto3-qldb-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.0/PKG-INFO` & `mypy-boto3-qldb-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-qldb
-Version: 1.28.0
-Summary: Type annotations for boto3.QLDB 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.QLDB 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-qldb"></a>
 
 # mypy-boto3-qldb
 
 [![PyPI - mypy-boto3-qldb](https://img.shields.io/pypi/v/mypy-boto3-qldb.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qldb.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-qldb?color=blue)](https://pypistats.org/packages/mypy-boto3-qldb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qldb)](https://pepy.tech/project/mypy-boto3-qldb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QLDB 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
+[boto3.QLDB 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
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
 [mypy-boto3-qldb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,57 +304,61 @@
 
 `mypy_boto3_qldb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_qldb.type_defs import (
     CancelJournalKinesisStreamRequestRequestTypeDef,
-    CancelJournalKinesisStreamResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateLedgerRequestRequestTypeDef,
-    CreateLedgerResponseTypeDef,
     DeleteLedgerRequestRequestTypeDef,
     DescribeJournalKinesisStreamRequestRequestTypeDef,
     DescribeJournalS3ExportRequestRequestTypeDef,
     DescribeLedgerRequestRequestTypeDef,
     LedgerEncryptionDescriptionTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportJournalToS3ResponseTypeDef,
     ValueHolderTypeDef,
+    ValueHolderOutputTypeDef,
     GetDigestRequestRequestTypeDef,
+    KinesisConfigurationOutputTypeDef,
     KinesisConfigurationTypeDef,
     LedgerSummaryTypeDef,
     ListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsRequestRequestTypeDef,
     ListLedgersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
+    S3EncryptionConfigurationOutputTypeDef,
     S3EncryptionConfigurationTypeDef,
-    StreamJournalToKinesisResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLedgerPermissionsModeRequestRequestTypeDef,
-    UpdateLedgerPermissionsModeResponseTypeDef,
     UpdateLedgerRequestRequestTypeDef,
+    CancelJournalKinesisStreamResponseTypeDef,
+    CreateLedgerResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportJournalToS3ResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StreamJournalToKinesisResponseTypeDef,
+    UpdateLedgerPermissionsModeResponseTypeDef,
     DescribeLedgerResponseTypeDef,
     UpdateLedgerResponseTypeDef,
     GetBlockRequestRequestTypeDef,
+    GetRevisionRequestRequestTypeDef,
     GetBlockResponseTypeDef,
     GetDigestResponseTypeDef,
-    GetRevisionRequestRequestTypeDef,
     GetRevisionResponseTypeDef,
     JournalKinesisStreamDescriptionTypeDef,
     StreamJournalToKinesisRequestRequestTypeDef,
     ListLedgersResponseTypeDef,
+    S3ExportConfigurationOutputTypeDef,
     S3ExportConfigurationTypeDef,
     DescribeJournalKinesisStreamResponseTypeDef,
     ListJournalKinesisStreamsForLedgerResponseTypeDef,
-    ExportJournalToS3RequestRequestTypeDef,
     JournalS3ExportDescriptionTypeDef,
+    ExportJournalToS3RequestRequestTypeDef,
     DescribeJournalS3ExportResponseTypeDef,
     ListJournalS3ExportsForLedgerResponseTypeDef,
     ListJournalS3ExportsResponseTypeDef,
 )
 
 
 def get_structure() -> CancelJournalKinesisStreamRequestRequestTypeDef:
```

### Comparing `mypy-boto3-qldb-1.28.0/README.md` & `mypy-boto3-qldb-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-qldb"></a>
 
 # mypy-boto3-qldb
 
 [![PyPI - mypy-boto3-qldb](https://img.shields.io/pypi/v/mypy-boto3-qldb.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qldb.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-qldb?color=blue)](https://pypistats.org/packages/mypy-boto3-qldb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qldb)](https://pepy.tech/project/mypy-boto3-qldb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QLDB 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
+[boto3.QLDB 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
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
 [mypy-boto3-qldb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -272,57 +272,61 @@
 
 `mypy_boto3_qldb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_qldb.type_defs import (
     CancelJournalKinesisStreamRequestRequestTypeDef,
-    CancelJournalKinesisStreamResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateLedgerRequestRequestTypeDef,
-    CreateLedgerResponseTypeDef,
     DeleteLedgerRequestRequestTypeDef,
     DescribeJournalKinesisStreamRequestRequestTypeDef,
     DescribeJournalS3ExportRequestRequestTypeDef,
     DescribeLedgerRequestRequestTypeDef,
     LedgerEncryptionDescriptionTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportJournalToS3ResponseTypeDef,
     ValueHolderTypeDef,
+    ValueHolderOutputTypeDef,
     GetDigestRequestRequestTypeDef,
+    KinesisConfigurationOutputTypeDef,
     KinesisConfigurationTypeDef,
     LedgerSummaryTypeDef,
     ListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsRequestRequestTypeDef,
     ListLedgersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
+    S3EncryptionConfigurationOutputTypeDef,
     S3EncryptionConfigurationTypeDef,
-    StreamJournalToKinesisResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLedgerPermissionsModeRequestRequestTypeDef,
-    UpdateLedgerPermissionsModeResponseTypeDef,
     UpdateLedgerRequestRequestTypeDef,
+    CancelJournalKinesisStreamResponseTypeDef,
+    CreateLedgerResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportJournalToS3ResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StreamJournalToKinesisResponseTypeDef,
+    UpdateLedgerPermissionsModeResponseTypeDef,
     DescribeLedgerResponseTypeDef,
     UpdateLedgerResponseTypeDef,
     GetBlockRequestRequestTypeDef,
+    GetRevisionRequestRequestTypeDef,
     GetBlockResponseTypeDef,
     GetDigestResponseTypeDef,
-    GetRevisionRequestRequestTypeDef,
     GetRevisionResponseTypeDef,
     JournalKinesisStreamDescriptionTypeDef,
     StreamJournalToKinesisRequestRequestTypeDef,
     ListLedgersResponseTypeDef,
+    S3ExportConfigurationOutputTypeDef,
     S3ExportConfigurationTypeDef,
     DescribeJournalKinesisStreamResponseTypeDef,
     ListJournalKinesisStreamsForLedgerResponseTypeDef,
-    ExportJournalToS3RequestRequestTypeDef,
     JournalS3ExportDescriptionTypeDef,
+    ExportJournalToS3RequestRequestTypeDef,
     DescribeJournalS3ExportResponseTypeDef,
     ListJournalS3ExportsForLedgerResponseTypeDef,
     ListJournalS3ExportsResponseTypeDef,
 )
 
 
 def get_structure() -> CancelJournalKinesisStreamRequestRequestTypeDef:
```

### Comparing `mypy-boto3-qldb-1.28.0/mypy_boto3_qldb/__main__.py` & `mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.QLDB 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.QLDB 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB\nOther"
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

### Comparing `mypy-boto3-qldb-1.28.0/mypy_boto3_qldb/client.py` & `mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.0/mypy_boto3_qldb/client.pyi` & `mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.0/mypy_boto3_qldb/literals.py` & `mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,15 @@
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
@@ -245,26 +246,28 @@
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

### Comparing `mypy-boto3-qldb-1.28.0/mypy_boto3_qldb/literals.pyi` & `mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,15 @@
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
@@ -243,26 +244,28 @@
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

### Comparing `mypy-boto3-qldb-1.28.0/mypy_boto3_qldb/type_defs.py` & `mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,75 +30,82 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CancelJournalKinesisStreamRequestRequestTypeDef",
-    "CancelJournalKinesisStreamResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateLedgerRequestRequestTypeDef",
-    "CreateLedgerResponseTypeDef",
     "DeleteLedgerRequestRequestTypeDef",
     "DescribeJournalKinesisStreamRequestRequestTypeDef",
     "DescribeJournalS3ExportRequestRequestTypeDef",
     "DescribeLedgerRequestRequestTypeDef",
     "LedgerEncryptionDescriptionTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ExportJournalToS3ResponseTypeDef",
     "ValueHolderTypeDef",
+    "ValueHolderOutputTypeDef",
     "GetDigestRequestRequestTypeDef",
+    "KinesisConfigurationOutputTypeDef",
     "KinesisConfigurationTypeDef",
     "LedgerSummaryTypeDef",
     "ListJournalKinesisStreamsForLedgerRequestRequestTypeDef",
     "ListJournalS3ExportsForLedgerRequestRequestTypeDef",
     "ListJournalS3ExportsRequestRequestTypeDef",
     "ListLedgersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
+    "S3EncryptionConfigurationOutputTypeDef",
     "S3EncryptionConfigurationTypeDef",
-    "StreamJournalToKinesisResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateLedgerPermissionsModeRequestRequestTypeDef",
-    "UpdateLedgerPermissionsModeResponseTypeDef",
     "UpdateLedgerRequestRequestTypeDef",
+    "CancelJournalKinesisStreamResponseTypeDef",
+    "CreateLedgerResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportJournalToS3ResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StreamJournalToKinesisResponseTypeDef",
+    "UpdateLedgerPermissionsModeResponseTypeDef",
     "DescribeLedgerResponseTypeDef",
     "UpdateLedgerResponseTypeDef",
     "GetBlockRequestRequestTypeDef",
+    "GetRevisionRequestRequestTypeDef",
     "GetBlockResponseTypeDef",
     "GetDigestResponseTypeDef",
-    "GetRevisionRequestRequestTypeDef",
     "GetRevisionResponseTypeDef",
     "JournalKinesisStreamDescriptionTypeDef",
     "StreamJournalToKinesisRequestRequestTypeDef",
     "ListLedgersResponseTypeDef",
+    "S3ExportConfigurationOutputTypeDef",
     "S3ExportConfigurationTypeDef",
     "DescribeJournalKinesisStreamResponseTypeDef",
     "ListJournalKinesisStreamsForLedgerResponseTypeDef",
-    "ExportJournalToS3RequestRequestTypeDef",
     "JournalS3ExportDescriptionTypeDef",
+    "ExportJournalToS3RequestRequestTypeDef",
     "DescribeJournalS3ExportResponseTypeDef",
     "ListJournalS3ExportsForLedgerResponseTypeDef",
     "ListJournalS3ExportsResponseTypeDef",
 )
 
 CancelJournalKinesisStreamRequestRequestTypeDef = TypedDict(
     "CancelJournalKinesisStreamRequestRequestTypeDef",
     {
         "LedgerName": str,
         "StreamId": str,
     },
 )
 
-CancelJournalKinesisStreamResponseTypeDef = TypedDict(
-    "CancelJournalKinesisStreamResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "StreamId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateLedgerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLedgerRequestRequestTypeDef",
     {
         "Name": str,
@@ -118,28 +125,14 @@
 
 class CreateLedgerRequestRequestTypeDef(
     _RequiredCreateLedgerRequestRequestTypeDef, _OptionalCreateLedgerRequestRequestTypeDef
 ):
     pass
 
 
-CreateLedgerResponseTypeDef = TypedDict(
-    "CreateLedgerResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "State": LedgerStateType,
-        "CreationDateTime": datetime,
-        "PermissionsMode": PermissionsModeType,
-        "DeletionProtection": bool,
-        "KmsKeyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLedgerRequestRequestTypeDef = TypedDict(
     "DeleteLedgerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -184,44 +177,58 @@
 
 class LedgerEncryptionDescriptionTypeDef(
     _RequiredLedgerEncryptionDescriptionTypeDef, _OptionalLedgerEncryptionDescriptionTypeDef
 ):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ExportJournalToS3ResponseTypeDef = TypedDict(
-    "ExportJournalToS3ResponseTypeDef",
+ValueHolderTypeDef = TypedDict(
+    "ValueHolderTypeDef",
     {
-        "ExportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "IonText": str,
     },
+    total=False,
 )
 
-ValueHolderTypeDef = TypedDict(
-    "ValueHolderTypeDef",
+ValueHolderOutputTypeDef = TypedDict(
+    "ValueHolderOutputTypeDef",
     {
         "IonText": str,
     },
     total=False,
 )
 
 GetDigestRequestRequestTypeDef = TypedDict(
     "GetDigestRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+_RequiredKinesisConfigurationOutputTypeDef = TypedDict(
+    "_RequiredKinesisConfigurationOutputTypeDef",
+    {
+        "StreamArn": str,
+    },
+)
+_OptionalKinesisConfigurationOutputTypeDef = TypedDict(
+    "_OptionalKinesisConfigurationOutputTypeDef",
+    {
+        "AggregationEnabled": bool,
+    },
+    total=False,
+)
+
+
+class KinesisConfigurationOutputTypeDef(
+    _RequiredKinesisConfigurationOutputTypeDef, _OptionalKinesisConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredKinesisConfigurationTypeDef = TypedDict(
     "_RequiredKinesisConfigurationTypeDef",
     {
         "StreamArn": str,
     },
 )
 _OptionalKinesisConfigurationTypeDef = TypedDict(
@@ -316,33 +323,35 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_RequiredS3EncryptionConfigurationOutputTypeDef = TypedDict(
+    "_RequiredS3EncryptionConfigurationOutputTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ObjectEncryptionType": S3ObjectEncryptionTypeType,
     },
 )
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_OptionalS3EncryptionConfigurationOutputTypeDef = TypedDict(
+    "_OptionalS3EncryptionConfigurationOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "KmsKeyArn": str,
     },
+    total=False,
 )
 
+
+class S3EncryptionConfigurationOutputTypeDef(
+    _RequiredS3EncryptionConfigurationOutputTypeDef, _OptionalS3EncryptionConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredS3EncryptionConfigurationTypeDef = TypedDict(
     "_RequiredS3EncryptionConfigurationTypeDef",
     {
         "ObjectEncryptionType": S3ObjectEncryptionTypeType,
     },
 )
 _OptionalS3EncryptionConfigurationTypeDef = TypedDict(
@@ -356,22 +365,14 @@
 
 class S3EncryptionConfigurationTypeDef(
     _RequiredS3EncryptionConfigurationTypeDef, _OptionalS3EncryptionConfigurationTypeDef
 ):
     pass
 
 
-StreamJournalToKinesisResponseTypeDef = TypedDict(
-    "StreamJournalToKinesisResponseTypeDef",
-    {
-        "StreamId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -388,24 +389,14 @@
     "UpdateLedgerPermissionsModeRequestRequestTypeDef",
     {
         "Name": str,
         "PermissionsMode": PermissionsModeType,
     },
 )
 
-UpdateLedgerPermissionsModeResponseTypeDef = TypedDict(
-    "UpdateLedgerPermissionsModeResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "PermissionsMode": PermissionsModeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateLedgerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLedgerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateLedgerRequestRequestTypeDef = TypedDict(
@@ -420,38 +411,101 @@
 
 class UpdateLedgerRequestRequestTypeDef(
     _RequiredUpdateLedgerRequestRequestTypeDef, _OptionalUpdateLedgerRequestRequestTypeDef
 ):
     pass
 
 
+CancelJournalKinesisStreamResponseTypeDef = TypedDict(
+    "CancelJournalKinesisStreamResponseTypeDef",
+    {
+        "StreamId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLedgerResponseTypeDef = TypedDict(
+    "CreateLedgerResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "State": LedgerStateType,
+        "CreationDateTime": datetime,
+        "PermissionsMode": PermissionsModeType,
+        "DeletionProtection": bool,
+        "KmsKeyArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportJournalToS3ResponseTypeDef = TypedDict(
+    "ExportJournalToS3ResponseTypeDef",
+    {
+        "ExportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StreamJournalToKinesisResponseTypeDef = TypedDict(
+    "StreamJournalToKinesisResponseTypeDef",
+    {
+        "StreamId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateLedgerPermissionsModeResponseTypeDef = TypedDict(
+    "UpdateLedgerPermissionsModeResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "PermissionsMode": PermissionsModeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeLedgerResponseTypeDef = TypedDict(
     "DescribeLedgerResponseTypeDef",
     {
         "Name": str,
         "Arn": str,
         "State": LedgerStateType,
         "CreationDateTime": datetime,
         "PermissionsMode": PermissionsModeType,
         "DeletionProtection": bool,
         "EncryptionDescription": LedgerEncryptionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLedgerResponseTypeDef = TypedDict(
     "UpdateLedgerResponseTypeDef",
     {
         "Name": str,
         "Arn": str,
         "State": LedgerStateType,
         "CreationDateTime": datetime,
         "DeletionProtection": bool,
         "EncryptionDescription": LedgerEncryptionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetBlockRequestRequestTypeDef = TypedDict(
     "_RequiredGetBlockRequestRequestTypeDef",
     {
         "Name": str,
@@ -469,32 +523,14 @@
 
 class GetBlockRequestRequestTypeDef(
     _RequiredGetBlockRequestRequestTypeDef, _OptionalGetBlockRequestRequestTypeDef
 ):
     pass
 
 
-GetBlockResponseTypeDef = TypedDict(
-    "GetBlockResponseTypeDef",
-    {
-        "Block": ValueHolderTypeDef,
-        "Proof": ValueHolderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDigestResponseTypeDef = TypedDict(
-    "GetDigestResponseTypeDef",
-    {
-        "Digest": bytes,
-        "DigestTipAddress": ValueHolderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRevisionRequestRequestTypeDef = TypedDict(
     "_RequiredGetRevisionRequestRequestTypeDef",
     {
         "Name": str,
         "BlockAddress": ValueHolderTypeDef,
         "DocumentId": str,
     },
@@ -510,31 +546,49 @@
 
 class GetRevisionRequestRequestTypeDef(
     _RequiredGetRevisionRequestRequestTypeDef, _OptionalGetRevisionRequestRequestTypeDef
 ):
     pass
 
 
+GetBlockResponseTypeDef = TypedDict(
+    "GetBlockResponseTypeDef",
+    {
+        "Block": ValueHolderOutputTypeDef,
+        "Proof": ValueHolderOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDigestResponseTypeDef = TypedDict(
+    "GetDigestResponseTypeDef",
+    {
+        "Digest": bytes,
+        "DigestTipAddress": ValueHolderOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetRevisionResponseTypeDef = TypedDict(
     "GetRevisionResponseTypeDef",
     {
-        "Proof": ValueHolderTypeDef,
-        "Revision": ValueHolderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Proof": ValueHolderOutputTypeDef,
+        "Revision": ValueHolderOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJournalKinesisStreamDescriptionTypeDef = TypedDict(
     "_RequiredJournalKinesisStreamDescriptionTypeDef",
     {
         "LedgerName": str,
         "RoleArn": str,
         "StreamId": str,
         "Status": StreamStatusType,
-        "KinesisConfiguration": KinesisConfigurationTypeDef,
+        "KinesisConfiguration": KinesisConfigurationOutputTypeDef,
         "StreamName": str,
     },
 )
 _OptionalJournalKinesisStreamDescriptionTypeDef = TypedDict(
     "_OptionalJournalKinesisStreamDescriptionTypeDef",
     {
         "CreationTime": datetime,
@@ -581,15 +635,24 @@
 
 
 ListLedgersResponseTypeDef = TypedDict(
     "ListLedgersResponseTypeDef",
     {
         "Ledgers": List[LedgerSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+S3ExportConfigurationOutputTypeDef = TypedDict(
+    "S3ExportConfigurationOutputTypeDef",
+    {
+        "Bucket": str,
+        "Prefix": str,
+        "EncryptionConfiguration": S3EncryptionConfigurationOutputTypeDef,
     },
 )
 
 S3ExportConfigurationTypeDef = TypedDict(
     "S3ExportConfigurationTypeDef",
     {
         "Bucket": str,
@@ -598,98 +661,98 @@
     },
 )
 
 DescribeJournalKinesisStreamResponseTypeDef = TypedDict(
     "DescribeJournalKinesisStreamResponseTypeDef",
     {
         "Stream": JournalKinesisStreamDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJournalKinesisStreamsForLedgerResponseTypeDef = TypedDict(
     "ListJournalKinesisStreamsForLedgerResponseTypeDef",
     {
         "Streams": List[JournalKinesisStreamDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredExportJournalToS3RequestRequestTypeDef = TypedDict(
-    "_RequiredExportJournalToS3RequestRequestTypeDef",
+_RequiredJournalS3ExportDescriptionTypeDef = TypedDict(
+    "_RequiredJournalS3ExportDescriptionTypeDef",
     {
-        "Name": str,
-        "InclusiveStartTime": Union[datetime, str],
-        "ExclusiveEndTime": Union[datetime, str],
-        "S3ExportConfiguration": S3ExportConfigurationTypeDef,
+        "LedgerName": str,
+        "ExportId": str,
+        "ExportCreationTime": datetime,
+        "Status": ExportStatusType,
+        "InclusiveStartTime": datetime,
+        "ExclusiveEndTime": datetime,
+        "S3ExportConfiguration": S3ExportConfigurationOutputTypeDef,
         "RoleArn": str,
     },
 )
-_OptionalExportJournalToS3RequestRequestTypeDef = TypedDict(
-    "_OptionalExportJournalToS3RequestRequestTypeDef",
+_OptionalJournalS3ExportDescriptionTypeDef = TypedDict(
+    "_OptionalJournalS3ExportDescriptionTypeDef",
     {
         "OutputFormat": OutputFormatType,
     },
     total=False,
 )
 
 
-class ExportJournalToS3RequestRequestTypeDef(
-    _RequiredExportJournalToS3RequestRequestTypeDef, _OptionalExportJournalToS3RequestRequestTypeDef
+class JournalS3ExportDescriptionTypeDef(
+    _RequiredJournalS3ExportDescriptionTypeDef, _OptionalJournalS3ExportDescriptionTypeDef
 ):
     pass
 
 
-_RequiredJournalS3ExportDescriptionTypeDef = TypedDict(
-    "_RequiredJournalS3ExportDescriptionTypeDef",
+_RequiredExportJournalToS3RequestRequestTypeDef = TypedDict(
+    "_RequiredExportJournalToS3RequestRequestTypeDef",
     {
-        "LedgerName": str,
-        "ExportId": str,
-        "ExportCreationTime": datetime,
-        "Status": ExportStatusType,
-        "InclusiveStartTime": datetime,
-        "ExclusiveEndTime": datetime,
+        "Name": str,
+        "InclusiveStartTime": Union[datetime, str],
+        "ExclusiveEndTime": Union[datetime, str],
         "S3ExportConfiguration": S3ExportConfigurationTypeDef,
         "RoleArn": str,
     },
 )
-_OptionalJournalS3ExportDescriptionTypeDef = TypedDict(
-    "_OptionalJournalS3ExportDescriptionTypeDef",
+_OptionalExportJournalToS3RequestRequestTypeDef = TypedDict(
+    "_OptionalExportJournalToS3RequestRequestTypeDef",
     {
         "OutputFormat": OutputFormatType,
     },
     total=False,
 )
 
 
-class JournalS3ExportDescriptionTypeDef(
-    _RequiredJournalS3ExportDescriptionTypeDef, _OptionalJournalS3ExportDescriptionTypeDef
+class ExportJournalToS3RequestRequestTypeDef(
+    _RequiredExportJournalToS3RequestRequestTypeDef, _OptionalExportJournalToS3RequestRequestTypeDef
 ):
     pass
 
 
 DescribeJournalS3ExportResponseTypeDef = TypedDict(
     "DescribeJournalS3ExportResponseTypeDef",
     {
         "ExportDescription": JournalS3ExportDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJournalS3ExportsForLedgerResponseTypeDef = TypedDict(
     "ListJournalS3ExportsForLedgerResponseTypeDef",
     {
         "JournalS3Exports": List[JournalS3ExportDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJournalS3ExportsResponseTypeDef = TypedDict(
     "ListJournalS3ExportsResponseTypeDef",
     {
         "JournalS3Exports": List[JournalS3ExportDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-qldb-1.28.0/mypy_boto3_qldb/type_defs.pyi` & `mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -29,75 +29,82 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CancelJournalKinesisStreamRequestRequestTypeDef",
-    "CancelJournalKinesisStreamResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateLedgerRequestRequestTypeDef",
-    "CreateLedgerResponseTypeDef",
     "DeleteLedgerRequestRequestTypeDef",
     "DescribeJournalKinesisStreamRequestRequestTypeDef",
     "DescribeJournalS3ExportRequestRequestTypeDef",
     "DescribeLedgerRequestRequestTypeDef",
     "LedgerEncryptionDescriptionTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ExportJournalToS3ResponseTypeDef",
     "ValueHolderTypeDef",
+    "ValueHolderOutputTypeDef",
     "GetDigestRequestRequestTypeDef",
+    "KinesisConfigurationOutputTypeDef",
     "KinesisConfigurationTypeDef",
     "LedgerSummaryTypeDef",
     "ListJournalKinesisStreamsForLedgerRequestRequestTypeDef",
     "ListJournalS3ExportsForLedgerRequestRequestTypeDef",
     "ListJournalS3ExportsRequestRequestTypeDef",
     "ListLedgersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
+    "S3EncryptionConfigurationOutputTypeDef",
     "S3EncryptionConfigurationTypeDef",
-    "StreamJournalToKinesisResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateLedgerPermissionsModeRequestRequestTypeDef",
-    "UpdateLedgerPermissionsModeResponseTypeDef",
     "UpdateLedgerRequestRequestTypeDef",
+    "CancelJournalKinesisStreamResponseTypeDef",
+    "CreateLedgerResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportJournalToS3ResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StreamJournalToKinesisResponseTypeDef",
+    "UpdateLedgerPermissionsModeResponseTypeDef",
     "DescribeLedgerResponseTypeDef",
     "UpdateLedgerResponseTypeDef",
     "GetBlockRequestRequestTypeDef",
+    "GetRevisionRequestRequestTypeDef",
     "GetBlockResponseTypeDef",
     "GetDigestResponseTypeDef",
-    "GetRevisionRequestRequestTypeDef",
     "GetRevisionResponseTypeDef",
     "JournalKinesisStreamDescriptionTypeDef",
     "StreamJournalToKinesisRequestRequestTypeDef",
     "ListLedgersResponseTypeDef",
+    "S3ExportConfigurationOutputTypeDef",
     "S3ExportConfigurationTypeDef",
     "DescribeJournalKinesisStreamResponseTypeDef",
     "ListJournalKinesisStreamsForLedgerResponseTypeDef",
-    "ExportJournalToS3RequestRequestTypeDef",
     "JournalS3ExportDescriptionTypeDef",
+    "ExportJournalToS3RequestRequestTypeDef",
     "DescribeJournalS3ExportResponseTypeDef",
     "ListJournalS3ExportsForLedgerResponseTypeDef",
     "ListJournalS3ExportsResponseTypeDef",
 )
 
 CancelJournalKinesisStreamRequestRequestTypeDef = TypedDict(
     "CancelJournalKinesisStreamRequestRequestTypeDef",
     {
         "LedgerName": str,
         "StreamId": str,
     },
 )
 
-CancelJournalKinesisStreamResponseTypeDef = TypedDict(
-    "CancelJournalKinesisStreamResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "StreamId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateLedgerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLedgerRequestRequestTypeDef",
     {
         "Name": str,
@@ -115,28 +122,14 @@
 )
 
 class CreateLedgerRequestRequestTypeDef(
     _RequiredCreateLedgerRequestRequestTypeDef, _OptionalCreateLedgerRequestRequestTypeDef
 ):
     pass
 
-CreateLedgerResponseTypeDef = TypedDict(
-    "CreateLedgerResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "State": LedgerStateType,
-        "CreationDateTime": datetime,
-        "PermissionsMode": PermissionsModeType,
-        "DeletionProtection": bool,
-        "KmsKeyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLedgerRequestRequestTypeDef = TypedDict(
     "DeleteLedgerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -179,44 +172,56 @@
 )
 
 class LedgerEncryptionDescriptionTypeDef(
     _RequiredLedgerEncryptionDescriptionTypeDef, _OptionalLedgerEncryptionDescriptionTypeDef
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ExportJournalToS3ResponseTypeDef = TypedDict(
-    "ExportJournalToS3ResponseTypeDef",
+ValueHolderTypeDef = TypedDict(
+    "ValueHolderTypeDef",
     {
-        "ExportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "IonText": str,
     },
+    total=False,
 )
 
-ValueHolderTypeDef = TypedDict(
-    "ValueHolderTypeDef",
+ValueHolderOutputTypeDef = TypedDict(
+    "ValueHolderOutputTypeDef",
     {
         "IonText": str,
     },
     total=False,
 )
 
 GetDigestRequestRequestTypeDef = TypedDict(
     "GetDigestRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+_RequiredKinesisConfigurationOutputTypeDef = TypedDict(
+    "_RequiredKinesisConfigurationOutputTypeDef",
+    {
+        "StreamArn": str,
+    },
+)
+_OptionalKinesisConfigurationOutputTypeDef = TypedDict(
+    "_OptionalKinesisConfigurationOutputTypeDef",
+    {
+        "AggregationEnabled": bool,
+    },
+    total=False,
+)
+
+class KinesisConfigurationOutputTypeDef(
+    _RequiredKinesisConfigurationOutputTypeDef, _OptionalKinesisConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredKinesisConfigurationTypeDef = TypedDict(
     "_RequiredKinesisConfigurationTypeDef",
     {
         "StreamArn": str,
     },
 )
 _OptionalKinesisConfigurationTypeDef = TypedDict(
@@ -305,33 +310,33 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_RequiredS3EncryptionConfigurationOutputTypeDef = TypedDict(
+    "_RequiredS3EncryptionConfigurationOutputTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ObjectEncryptionType": S3ObjectEncryptionTypeType,
     },
 )
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_OptionalS3EncryptionConfigurationOutputTypeDef = TypedDict(
+    "_OptionalS3EncryptionConfigurationOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "KmsKeyArn": str,
     },
+    total=False,
 )
 
+class S3EncryptionConfigurationOutputTypeDef(
+    _RequiredS3EncryptionConfigurationOutputTypeDef, _OptionalS3EncryptionConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredS3EncryptionConfigurationTypeDef = TypedDict(
     "_RequiredS3EncryptionConfigurationTypeDef",
     {
         "ObjectEncryptionType": S3ObjectEncryptionTypeType,
     },
 )
 _OptionalS3EncryptionConfigurationTypeDef = TypedDict(
@@ -343,22 +348,14 @@
 )
 
 class S3EncryptionConfigurationTypeDef(
     _RequiredS3EncryptionConfigurationTypeDef, _OptionalS3EncryptionConfigurationTypeDef
 ):
     pass
 
-StreamJournalToKinesisResponseTypeDef = TypedDict(
-    "StreamJournalToKinesisResponseTypeDef",
-    {
-        "StreamId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -375,24 +372,14 @@
     "UpdateLedgerPermissionsModeRequestRequestTypeDef",
     {
         "Name": str,
         "PermissionsMode": PermissionsModeType,
     },
 )
 
-UpdateLedgerPermissionsModeResponseTypeDef = TypedDict(
-    "UpdateLedgerPermissionsModeResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "PermissionsMode": PermissionsModeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateLedgerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLedgerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateLedgerRequestRequestTypeDef = TypedDict(
@@ -405,38 +392,101 @@
 )
 
 class UpdateLedgerRequestRequestTypeDef(
     _RequiredUpdateLedgerRequestRequestTypeDef, _OptionalUpdateLedgerRequestRequestTypeDef
 ):
     pass
 
+CancelJournalKinesisStreamResponseTypeDef = TypedDict(
+    "CancelJournalKinesisStreamResponseTypeDef",
+    {
+        "StreamId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLedgerResponseTypeDef = TypedDict(
+    "CreateLedgerResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "State": LedgerStateType,
+        "CreationDateTime": datetime,
+        "PermissionsMode": PermissionsModeType,
+        "DeletionProtection": bool,
+        "KmsKeyArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportJournalToS3ResponseTypeDef = TypedDict(
+    "ExportJournalToS3ResponseTypeDef",
+    {
+        "ExportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StreamJournalToKinesisResponseTypeDef = TypedDict(
+    "StreamJournalToKinesisResponseTypeDef",
+    {
+        "StreamId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateLedgerPermissionsModeResponseTypeDef = TypedDict(
+    "UpdateLedgerPermissionsModeResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "PermissionsMode": PermissionsModeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeLedgerResponseTypeDef = TypedDict(
     "DescribeLedgerResponseTypeDef",
     {
         "Name": str,
         "Arn": str,
         "State": LedgerStateType,
         "CreationDateTime": datetime,
         "PermissionsMode": PermissionsModeType,
         "DeletionProtection": bool,
         "EncryptionDescription": LedgerEncryptionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLedgerResponseTypeDef = TypedDict(
     "UpdateLedgerResponseTypeDef",
     {
         "Name": str,
         "Arn": str,
         "State": LedgerStateType,
         "CreationDateTime": datetime,
         "DeletionProtection": bool,
         "EncryptionDescription": LedgerEncryptionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetBlockRequestRequestTypeDef = TypedDict(
     "_RequiredGetBlockRequestRequestTypeDef",
     {
         "Name": str,
@@ -452,32 +502,14 @@
 )
 
 class GetBlockRequestRequestTypeDef(
     _RequiredGetBlockRequestRequestTypeDef, _OptionalGetBlockRequestRequestTypeDef
 ):
     pass
 
-GetBlockResponseTypeDef = TypedDict(
-    "GetBlockResponseTypeDef",
-    {
-        "Block": ValueHolderTypeDef,
-        "Proof": ValueHolderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDigestResponseTypeDef = TypedDict(
-    "GetDigestResponseTypeDef",
-    {
-        "Digest": bytes,
-        "DigestTipAddress": ValueHolderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRevisionRequestRequestTypeDef = TypedDict(
     "_RequiredGetRevisionRequestRequestTypeDef",
     {
         "Name": str,
         "BlockAddress": ValueHolderTypeDef,
         "DocumentId": str,
     },
@@ -491,31 +523,49 @@
 )
 
 class GetRevisionRequestRequestTypeDef(
     _RequiredGetRevisionRequestRequestTypeDef, _OptionalGetRevisionRequestRequestTypeDef
 ):
     pass
 
+GetBlockResponseTypeDef = TypedDict(
+    "GetBlockResponseTypeDef",
+    {
+        "Block": ValueHolderOutputTypeDef,
+        "Proof": ValueHolderOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDigestResponseTypeDef = TypedDict(
+    "GetDigestResponseTypeDef",
+    {
+        "Digest": bytes,
+        "DigestTipAddress": ValueHolderOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetRevisionResponseTypeDef = TypedDict(
     "GetRevisionResponseTypeDef",
     {
-        "Proof": ValueHolderTypeDef,
-        "Revision": ValueHolderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Proof": ValueHolderOutputTypeDef,
+        "Revision": ValueHolderOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJournalKinesisStreamDescriptionTypeDef = TypedDict(
     "_RequiredJournalKinesisStreamDescriptionTypeDef",
     {
         "LedgerName": str,
         "RoleArn": str,
         "StreamId": str,
         "Status": StreamStatusType,
-        "KinesisConfiguration": KinesisConfigurationTypeDef,
+        "KinesisConfiguration": KinesisConfigurationOutputTypeDef,
         "StreamName": str,
     },
 )
 _OptionalJournalKinesisStreamDescriptionTypeDef = TypedDict(
     "_OptionalJournalKinesisStreamDescriptionTypeDef",
     {
         "CreationTime": datetime,
@@ -558,15 +608,24 @@
     pass
 
 ListLedgersResponseTypeDef = TypedDict(
     "ListLedgersResponseTypeDef",
     {
         "Ledgers": List[LedgerSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+S3ExportConfigurationOutputTypeDef = TypedDict(
+    "S3ExportConfigurationOutputTypeDef",
+    {
+        "Bucket": str,
+        "Prefix": str,
+        "EncryptionConfiguration": S3EncryptionConfigurationOutputTypeDef,
     },
 )
 
 S3ExportConfigurationTypeDef = TypedDict(
     "S3ExportConfigurationTypeDef",
     {
         "Bucket": str,
@@ -575,94 +634,94 @@
     },
 )
 
 DescribeJournalKinesisStreamResponseTypeDef = TypedDict(
     "DescribeJournalKinesisStreamResponseTypeDef",
     {
         "Stream": JournalKinesisStreamDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJournalKinesisStreamsForLedgerResponseTypeDef = TypedDict(
     "ListJournalKinesisStreamsForLedgerResponseTypeDef",
     {
         "Streams": List[JournalKinesisStreamDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredExportJournalToS3RequestRequestTypeDef = TypedDict(
-    "_RequiredExportJournalToS3RequestRequestTypeDef",
+_RequiredJournalS3ExportDescriptionTypeDef = TypedDict(
+    "_RequiredJournalS3ExportDescriptionTypeDef",
     {
-        "Name": str,
-        "InclusiveStartTime": Union[datetime, str],
-        "ExclusiveEndTime": Union[datetime, str],
-        "S3ExportConfiguration": S3ExportConfigurationTypeDef,
+        "LedgerName": str,
+        "ExportId": str,
+        "ExportCreationTime": datetime,
+        "Status": ExportStatusType,
+        "InclusiveStartTime": datetime,
+        "ExclusiveEndTime": datetime,
+        "S3ExportConfiguration": S3ExportConfigurationOutputTypeDef,
         "RoleArn": str,
     },
 )
-_OptionalExportJournalToS3RequestRequestTypeDef = TypedDict(
-    "_OptionalExportJournalToS3RequestRequestTypeDef",
+_OptionalJournalS3ExportDescriptionTypeDef = TypedDict(
+    "_OptionalJournalS3ExportDescriptionTypeDef",
     {
         "OutputFormat": OutputFormatType,
     },
     total=False,
 )
 
-class ExportJournalToS3RequestRequestTypeDef(
-    _RequiredExportJournalToS3RequestRequestTypeDef, _OptionalExportJournalToS3RequestRequestTypeDef
+class JournalS3ExportDescriptionTypeDef(
+    _RequiredJournalS3ExportDescriptionTypeDef, _OptionalJournalS3ExportDescriptionTypeDef
 ):
     pass
 
-_RequiredJournalS3ExportDescriptionTypeDef = TypedDict(
-    "_RequiredJournalS3ExportDescriptionTypeDef",
+_RequiredExportJournalToS3RequestRequestTypeDef = TypedDict(
+    "_RequiredExportJournalToS3RequestRequestTypeDef",
     {
-        "LedgerName": str,
-        "ExportId": str,
-        "ExportCreationTime": datetime,
-        "Status": ExportStatusType,
-        "InclusiveStartTime": datetime,
-        "ExclusiveEndTime": datetime,
+        "Name": str,
+        "InclusiveStartTime": Union[datetime, str],
+        "ExclusiveEndTime": Union[datetime, str],
         "S3ExportConfiguration": S3ExportConfigurationTypeDef,
         "RoleArn": str,
     },
 )
-_OptionalJournalS3ExportDescriptionTypeDef = TypedDict(
-    "_OptionalJournalS3ExportDescriptionTypeDef",
+_OptionalExportJournalToS3RequestRequestTypeDef = TypedDict(
+    "_OptionalExportJournalToS3RequestRequestTypeDef",
     {
         "OutputFormat": OutputFormatType,
     },
     total=False,
 )
 
-class JournalS3ExportDescriptionTypeDef(
-    _RequiredJournalS3ExportDescriptionTypeDef, _OptionalJournalS3ExportDescriptionTypeDef
+class ExportJournalToS3RequestRequestTypeDef(
+    _RequiredExportJournalToS3RequestRequestTypeDef, _OptionalExportJournalToS3RequestRequestTypeDef
 ):
     pass
 
 DescribeJournalS3ExportResponseTypeDef = TypedDict(
     "DescribeJournalS3ExportResponseTypeDef",
     {
         "ExportDescription": JournalS3ExportDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJournalS3ExportsForLedgerResponseTypeDef = TypedDict(
     "ListJournalS3ExportsForLedgerResponseTypeDef",
     {
         "JournalS3Exports": List[JournalS3ExportDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJournalS3ExportsResponseTypeDef = TypedDict(
     "ListJournalS3ExportsResponseTypeDef",
     {
         "JournalS3Exports": List[JournalS3ExportDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-qldb-1.28.0/mypy_boto3_qldb.egg-info/PKG-INFO` & `mypy-boto3-qldb-1.28.12/mypy_boto3_qldb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-qldb
-Version: 1.28.0
-Summary: Type annotations for boto3.QLDB 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.QLDB 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-qldb"></a>
 
 # mypy-boto3-qldb
 
 [![PyPI - mypy-boto3-qldb](https://img.shields.io/pypi/v/mypy-boto3-qldb.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qldb.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-qldb?color=blue)](https://pypistats.org/packages/mypy-boto3-qldb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qldb)](https://pepy.tech/project/mypy-boto3-qldb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QLDB 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
+[boto3.QLDB 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
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
 [mypy-boto3-qldb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,57 +304,61 @@
 
 `mypy_boto3_qldb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_qldb.type_defs import (
     CancelJournalKinesisStreamRequestRequestTypeDef,
-    CancelJournalKinesisStreamResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateLedgerRequestRequestTypeDef,
-    CreateLedgerResponseTypeDef,
     DeleteLedgerRequestRequestTypeDef,
     DescribeJournalKinesisStreamRequestRequestTypeDef,
     DescribeJournalS3ExportRequestRequestTypeDef,
     DescribeLedgerRequestRequestTypeDef,
     LedgerEncryptionDescriptionTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportJournalToS3ResponseTypeDef,
     ValueHolderTypeDef,
+    ValueHolderOutputTypeDef,
     GetDigestRequestRequestTypeDef,
+    KinesisConfigurationOutputTypeDef,
     KinesisConfigurationTypeDef,
     LedgerSummaryTypeDef,
     ListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsRequestRequestTypeDef,
     ListLedgersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
+    S3EncryptionConfigurationOutputTypeDef,
     S3EncryptionConfigurationTypeDef,
-    StreamJournalToKinesisResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLedgerPermissionsModeRequestRequestTypeDef,
-    UpdateLedgerPermissionsModeResponseTypeDef,
     UpdateLedgerRequestRequestTypeDef,
+    CancelJournalKinesisStreamResponseTypeDef,
+    CreateLedgerResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportJournalToS3ResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StreamJournalToKinesisResponseTypeDef,
+    UpdateLedgerPermissionsModeResponseTypeDef,
     DescribeLedgerResponseTypeDef,
     UpdateLedgerResponseTypeDef,
     GetBlockRequestRequestTypeDef,
+    GetRevisionRequestRequestTypeDef,
     GetBlockResponseTypeDef,
     GetDigestResponseTypeDef,
-    GetRevisionRequestRequestTypeDef,
     GetRevisionResponseTypeDef,
     JournalKinesisStreamDescriptionTypeDef,
     StreamJournalToKinesisRequestRequestTypeDef,
     ListLedgersResponseTypeDef,
+    S3ExportConfigurationOutputTypeDef,
     S3ExportConfigurationTypeDef,
     DescribeJournalKinesisStreamResponseTypeDef,
     ListJournalKinesisStreamsForLedgerResponseTypeDef,
-    ExportJournalToS3RequestRequestTypeDef,
     JournalS3ExportDescriptionTypeDef,
+    ExportJournalToS3RequestRequestTypeDef,
     DescribeJournalS3ExportResponseTypeDef,
     ListJournalS3ExportsForLedgerResponseTypeDef,
     ListJournalS3ExportsResponseTypeDef,
 )
 
 
 def get_structure() -> CancelJournalKinesisStreamRequestRequestTypeDef:
```

### Comparing `mypy-boto3-qldb-1.28.0/mypy_boto3_qldb.egg-info/SOURCES.txt` & `mypy-boto3-qldb-1.28.12/mypy_boto3_qldb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.0/setup.py` & `mypy-boto3-qldb-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-qldb",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_qldb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.QLDB 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.QLDB 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

