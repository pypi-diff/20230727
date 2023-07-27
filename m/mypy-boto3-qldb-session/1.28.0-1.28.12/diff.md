# Comparing `tmp/mypy-boto3-qldb-session-1.28.0.tar.gz` & `tmp/mypy-boto3-qldb-session-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-qldb-session-1.28.0.tar", last modified: Thu Jul  6 21:00:22 2023, max compression
+gzip compressed data, was "mypy-boto3-qldb-session-1.28.12.tar", last modified: Thu Jul 27 11:49:27 2023, max compression
```

## Comparing `mypy-boto3-qldb-session-1.28.0.tar` & `mypy-boto3-qldb-session-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:22.622400 mypy-boto3-qldb-session-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:49:56.000000 mypy-boto3-qldb-session-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-07-06 21:00:22.622400 mypy-boto3-qldb-session-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-07-06 20:49:56.000000 mypy-boto3-qldb-session-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:22.622400 mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-06 20:49:56.000000 mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-06 20:49:56.000000 mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-06 20:49:56.000000 mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-06 20:49:57.000000 mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-06 20:49:56.000000 mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-07-06 20:49:57.000000 mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-07-06 20:49:57.000000 mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:49:56.000000 mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-07-06 20:49:57.000000 mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-07-06 20:49:57.000000 mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:49:56.000000 mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:22.622400 mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-07-06 21:00:22.000000 mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-06 21:00:22.000000 mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:22.000000 mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:22.000000 mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:22.000000 mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 21:00:22.000000 mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:22.622400 mypy-boto3-qldb-session-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-06 20:49:56.000000 mypy-boto3-qldb-session-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.497187 mypy-boto3-qldb-session-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:52.000000 mypy-boto3-qldb-session-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12614 2023-07-27 11:49:27.497187 mypy-boto3-qldb-session-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-07-27 11:41:52.000000 mypy-boto3-qldb-session-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.485187 mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-27 11:41:52.000000 mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-27 11:41:52.000000 mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-27 11:41:52.000000 mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-27 11:41:52.000000 mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-27 11:41:52.000000 mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-27 11:41:52.000000 mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-27 11:41:52.000000 mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:52.000000 mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-27 11:41:53.000000 mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-27 11:41:53.000000 mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:52.000000 mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.497187 mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12614 2023-07-27 11:49:27.000000 mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-27 11:49:27.000000 mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:27.000000 mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 11:49:27.000000 mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:27.497187 mypy-boto3-qldb-session-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-27 11:41:52.000000 mypy-boto3-qldb-session-1.28.12/setup.py
```

### Comparing `mypy-boto3-qldb-session-1.28.0/LICENSE` & `mypy-boto3-qldb-session-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-session-1.28.0/PKG-INFO` & `mypy-boto3-qldb-session-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-qldb-session
-Version: 1.28.0
-Summary: Type annotations for boto3.QLDBSession 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.QLDBSession 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-qldb-session"></a>
 
 # mypy-boto3-qldb-session
 
 [![PyPI - mypy-boto3-qldb-session](https://img.shields.io/pypi/v/mypy-boto3-qldb-session.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb-session)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qldb-session.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb-session)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-qldb-session?color=blue)](https://pypistats.org/packages/mypy-boto3-qldb-session)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qldb-session)](https://pepy.tech/project/mypy-boto3-qldb-session)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QLDBSession 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession)
+[boto3.QLDBSession 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession)
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
 [mypy-boto3-qldb-session docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,14 +301,15 @@
 ```python
 from mypy_boto3_qldb_session.type_defs import (
     TimingInformationTypeDef,
     CommitTransactionRequestTypeDef,
     IOUsageTypeDef,
     ValueHolderTypeDef,
     FetchPageRequestTypeDef,
+    ValueHolderOutputTypeDef,
     ResponseMetadataTypeDef,
     StartSessionRequestTypeDef,
     AbortTransactionResultTypeDef,
     EndSessionResultTypeDef,
     StartSessionResultTypeDef,
     StartTransactionResultTypeDef,
     CommitTransactionResultTypeDef,
```

### Comparing `mypy-boto3-qldb-session-1.28.0/README.md` & `mypy-boto3-qldb-session-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-qldb-session"></a>
 
 # mypy-boto3-qldb-session
 
 [![PyPI - mypy-boto3-qldb-session](https://img.shields.io/pypi/v/mypy-boto3-qldb-session.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb-session)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qldb-session.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb-session)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-qldb-session?color=blue)](https://pypistats.org/packages/mypy-boto3-qldb-session)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qldb-session)](https://pepy.tech/project/mypy-boto3-qldb-session)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QLDBSession 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession)
+[boto3.QLDBSession 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession)
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
 [mypy-boto3-qldb-session docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session/).
 
 See how it helps to find and fix potential bugs:
 
@@ -269,14 +269,15 @@
 ```python
 from mypy_boto3_qldb_session.type_defs import (
     TimingInformationTypeDef,
     CommitTransactionRequestTypeDef,
     IOUsageTypeDef,
     ValueHolderTypeDef,
     FetchPageRequestTypeDef,
+    ValueHolderOutputTypeDef,
     ResponseMetadataTypeDef,
     StartSessionRequestTypeDef,
     AbortTransactionResultTypeDef,
     EndSessionResultTypeDef,
     StartSessionResultTypeDef,
     StartTransactionResultTypeDef,
     CommitTransactionResultTypeDef,
```

### Comparing `mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session/__main__.py` & `mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.QLDBSession 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.QLDBSession 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession\nOther"
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

### Comparing `mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session/client.py` & `mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session/client.pyi` & `mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session/literals.py` & `mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session/literals.py`

 * *Files 0% similar despite different names*

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

### Comparing `mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session/literals.pyi` & `mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session/literals.pyi`

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

### Comparing `mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session/type_defs.py` & `mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 __all__ = (
     "TimingInformationTypeDef",
     "CommitTransactionRequestTypeDef",
     "IOUsageTypeDef",
     "ValueHolderTypeDef",
     "FetchPageRequestTypeDef",
+    "ValueHolderOutputTypeDef",
     "ResponseMetadataTypeDef",
     "StartSessionRequestTypeDef",
     "AbortTransactionResultTypeDef",
     "EndSessionResultTypeDef",
     "StartSessionResultTypeDef",
     "StartTransactionResultTypeDef",
     "CommitTransactionResultTypeDef",
@@ -81,14 +82,23 @@
     "FetchPageRequestTypeDef",
     {
         "TransactionId": str,
         "NextPageToken": str,
     },
 )
 
+ValueHolderOutputTypeDef = TypedDict(
+    "ValueHolderOutputTypeDef",
+    {
+        "IonBinary": bytes,
+        "IonText": str,
+    },
+    total=False,
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -169,15 +179,15 @@
 ):
     pass
 
 
 PageTypeDef = TypedDict(
     "PageTypeDef",
     {
-        "Values": List[ValueHolderTypeDef],
+        "Values": List[ValueHolderOutputTypeDef],
         "NextPageToken": str,
     },
     total=False,
 )
 
 SendCommandRequestRequestTypeDef = TypedDict(
     "SendCommandRequestRequestTypeDef",
@@ -220,10 +230,10 @@
         "StartSession": StartSessionResultTypeDef,
         "StartTransaction": StartTransactionResultTypeDef,
         "EndSession": EndSessionResultTypeDef,
         "CommitTransaction": CommitTransactionResultTypeDef,
         "AbortTransaction": AbortTransactionResultTypeDef,
         "ExecuteStatement": ExecuteStatementResultTypeDef,
         "FetchPage": FetchPageResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session/type_defs.pyi` & `mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 __all__ = (
     "TimingInformationTypeDef",
     "CommitTransactionRequestTypeDef",
     "IOUsageTypeDef",
     "ValueHolderTypeDef",
     "FetchPageRequestTypeDef",
+    "ValueHolderOutputTypeDef",
     "ResponseMetadataTypeDef",
     "StartSessionRequestTypeDef",
     "AbortTransactionResultTypeDef",
     "EndSessionResultTypeDef",
     "StartSessionResultTypeDef",
     "StartTransactionResultTypeDef",
     "CommitTransactionResultTypeDef",
@@ -80,14 +81,23 @@
     "FetchPageRequestTypeDef",
     {
         "TransactionId": str,
         "NextPageToken": str,
     },
 )
 
+ValueHolderOutputTypeDef = TypedDict(
+    "ValueHolderOutputTypeDef",
+    {
+        "IonBinary": bytes,
+        "IonText": str,
+    },
+    total=False,
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -166,15 +176,15 @@
     _RequiredExecuteStatementRequestTypeDef, _OptionalExecuteStatementRequestTypeDef
 ):
     pass
 
 PageTypeDef = TypedDict(
     "PageTypeDef",
     {
-        "Values": List[ValueHolderTypeDef],
+        "Values": List[ValueHolderOutputTypeDef],
         "NextPageToken": str,
     },
     total=False,
 )
 
 SendCommandRequestRequestTypeDef = TypedDict(
     "SendCommandRequestRequestTypeDef",
@@ -217,10 +227,10 @@
         "StartSession": StartSessionResultTypeDef,
         "StartTransaction": StartTransactionResultTypeDef,
         "EndSession": EndSessionResultTypeDef,
         "CommitTransaction": CommitTransactionResultTypeDef,
         "AbortTransaction": AbortTransactionResultTypeDef,
         "ExecuteStatement": ExecuteStatementResultTypeDef,
         "FetchPage": FetchPageResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session.egg-info/PKG-INFO` & `mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-qldb-session
-Version: 1.28.0
-Summary: Type annotations for boto3.QLDBSession 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.QLDBSession 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-qldb-session"></a>
 
 # mypy-boto3-qldb-session
 
 [![PyPI - mypy-boto3-qldb-session](https://img.shields.io/pypi/v/mypy-boto3-qldb-session.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb-session)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qldb-session.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb-session)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-qldb-session?color=blue)](https://pypistats.org/packages/mypy-boto3-qldb-session)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qldb-session)](https://pepy.tech/project/mypy-boto3-qldb-session)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QLDBSession 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession)
+[boto3.QLDBSession 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession)
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
 [mypy-boto3-qldb-session docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb_session/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,14 +301,15 @@
 ```python
 from mypy_boto3_qldb_session.type_defs import (
     TimingInformationTypeDef,
     CommitTransactionRequestTypeDef,
     IOUsageTypeDef,
     ValueHolderTypeDef,
     FetchPageRequestTypeDef,
+    ValueHolderOutputTypeDef,
     ResponseMetadataTypeDef,
     StartSessionRequestTypeDef,
     AbortTransactionResultTypeDef,
     EndSessionResultTypeDef,
     StartSessionResultTypeDef,
     StartTransactionResultTypeDef,
     CommitTransactionResultTypeDef,
```

### Comparing `mypy-boto3-qldb-session-1.28.0/mypy_boto3_qldb_session.egg-info/SOURCES.txt` & `mypy-boto3-qldb-session-1.28.12/mypy_boto3_qldb_session.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-session-1.28.0/setup.py` & `mypy-boto3-qldb-session-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-qldb-session",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_qldb_session"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.QLDBSession 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.QLDBSession 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

