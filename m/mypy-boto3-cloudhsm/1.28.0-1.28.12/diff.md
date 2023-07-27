# Comparing `tmp/mypy-boto3-cloudhsm-1.28.0.tar.gz` & `tmp/mypy-boto3-cloudhsm-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudhsm-1.28.0.tar", last modified: Thu Jul  6 20:59:09 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudhsm-1.28.12.tar", last modified: Thu Jul 27 05:34:25 2023, max compression
```

## Comparing `mypy-boto3-cloudhsm-1.28.0.tar` & `mypy-boto3-cloudhsm-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:09.194243 mypy-boto3-cloudhsm-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:35:23.000000 mypy-boto3-cloudhsm-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-07-06 20:59:09.186243 mypy-boto3-cloudhsm-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-07-06 20:35:23.000000 mypy-boto3-cloudhsm-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:09.182243 mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-06 20:35:23.000000 mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-06 20:35:23.000000 mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:35:23.000000 mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-07-06 20:35:23.000000 mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-07-06 20:35:23.000000 mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-06 20:35:23.000000 mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-07-06 20:35:23.000000 mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-06 20:35:23.000000 mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-06 20:35:23.000000 mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:23.000000 mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-07-06 20:35:24.000000 mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-07-06 20:35:23.000000 mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:35:23.000000 mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:09.186243 mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-07-06 20:59:08.000000 mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 20:59:08.000000 mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:08.000000 mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:08.000000 mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:08.000000 mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 20:59:08.000000 mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:09.194243 mypy-boto3-cloudhsm-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:35:23.000000 mypy-boto3-cloudhsm-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.140562 mypy-boto3-cloudhsm-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-07-27 05:34:25.136562 mypy-boto3-cloudhsm-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.136562 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12773 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.136562 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:25.140562 mypy-boto3-cloudhsm-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/setup.py
```

### Comparing `mypy-boto3-cloudhsm-1.28.0/LICENSE` & `mypy-boto3-cloudhsm-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsm-1.28.0/PKG-INFO` & `mypy-boto3-cloudhsm-1.28.12/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudhsm
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudHSM 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudHSM 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cloudhsm"></a>
 
 # mypy-boto3-cloudhsm
 
 [![PyPI - mypy-boto3-cloudhsm](https://img.shields.io/pypi/v/mypy-boto3-cloudhsm.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudhsm.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudhsm?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudhsm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudhsm)](https://pepy.tech/project/mypy-boto3-cloudhsm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudHSM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
+[boto3.CloudHSM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
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
 [mypy-boto3-cloudhsm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -363,14 +363,15 @@
     ListHsmsRequestListHsmsPaginateTypeDef,
     ListHsmsRequestRequestTypeDef,
     ListHsmsResponseTypeDef,
     ListLunaClientsRequestListLunaClientsPaginateTypeDef,
     ListLunaClientsRequestRequestTypeDef,
     ListLunaClientsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ModifyHapgRequestRequestTypeDef,
     ModifyHapgResponseTypeDef,
     ModifyHsmRequestRequestTypeDef,
     ModifyHsmResponseTypeDef,
     ModifyLunaClientRequestRequestTypeDef,
     ModifyLunaClientResponseTypeDef,
     PaginatorConfigTypeDef,
```

### Comparing `mypy-boto3-cloudhsm-1.28.0/README.md` & `mypy-boto3-cloudhsm-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cloudhsm"></a>
 
 # mypy-boto3-cloudhsm
 
 [![PyPI - mypy-boto3-cloudhsm](https://img.shields.io/pypi/v/mypy-boto3-cloudhsm.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudhsm.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudhsm?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudhsm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudhsm)](https://pepy.tech/project/mypy-boto3-cloudhsm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudHSM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
+[boto3.CloudHSM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
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
 [mypy-boto3-cloudhsm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -331,14 +331,15 @@
     ListHsmsRequestListHsmsPaginateTypeDef,
     ListHsmsRequestRequestTypeDef,
     ListHsmsResponseTypeDef,
     ListLunaClientsRequestListLunaClientsPaginateTypeDef,
     ListLunaClientsRequestRequestTypeDef,
     ListLunaClientsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ModifyHapgRequestRequestTypeDef,
     ModifyHapgResponseTypeDef,
     ModifyHsmRequestRequestTypeDef,
     ModifyHsmResponseTypeDef,
     ModifyLunaClientRequestRequestTypeDef,
     ModifyLunaClientResponseTypeDef,
     PaginatorConfigTypeDef,
```

### Comparing `mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/__init__.py` & `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/__init__.pyi` & `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/__main__.py` & `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudHSM 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.CloudHSM 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM\nOther"
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

### Comparing `mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/client.py` & `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/client.pyi` & `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/literals.py` & `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,14 +160,15 @@
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
@@ -246,26 +247,28 @@
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

### Comparing `mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/literals.pyi` & `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -158,14 +158,15 @@
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
@@ -244,26 +245,28 @@
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

### Comparing `mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/paginator.py` & `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/paginator.pyi` & `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/type_defs.py` & `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     "ListHsmsRequestListHsmsPaginateTypeDef",
     "ListHsmsRequestRequestTypeDef",
     "ListHsmsResponseTypeDef",
     "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
     "ListLunaClientsRequestRequestTypeDef",
     "ListLunaClientsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ModifyHapgRequestRequestTypeDef",
     "ModifyHapgResponseTypeDef",
     "ModifyHsmRequestRequestTypeDef",
     "ModifyHsmResponseTypeDef",
     "ModifyLunaClientRequestRequestTypeDef",
     "ModifyLunaClientResponseTypeDef",
     "PaginatorConfigTypeDef",
@@ -400,14 +401,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 _RequiredModifyHapgRequestRequestTypeDef = TypedDict(
     "_RequiredModifyHapgRequestRequestTypeDef",
     {
         "HapgArn": str,
     },
 )
 _OptionalModifyHapgRequestRequestTypeDef = TypedDict(
@@ -527,11 +536,11 @@
         "TagList": Sequence[TagTypeDef],
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "TagList": List[TagTypeDef],
+        "TagList": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm/type_defs.pyi` & `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     "ListHsmsRequestListHsmsPaginateTypeDef",
     "ListHsmsRequestRequestTypeDef",
     "ListHsmsResponseTypeDef",
     "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
     "ListLunaClientsRequestRequestTypeDef",
     "ListLunaClientsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ModifyHapgRequestRequestTypeDef",
     "ModifyHapgResponseTypeDef",
     "ModifyHsmRequestRequestTypeDef",
     "ModifyHsmResponseTypeDef",
     "ModifyLunaClientRequestRequestTypeDef",
     "ModifyLunaClientResponseTypeDef",
     "PaginatorConfigTypeDef",
@@ -395,14 +396,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 _RequiredModifyHapgRequestRequestTypeDef = TypedDict(
     "_RequiredModifyHapgRequestRequestTypeDef",
     {
         "HapgArn": str,
     },
 )
 _OptionalModifyHapgRequestRequestTypeDef = TypedDict(
@@ -518,11 +527,11 @@
         "TagList": Sequence[TagTypeDef],
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "TagList": List[TagTypeDef],
+        "TagList": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm.egg-info/PKG-INFO` & `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudhsm
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudHSM 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudHSM 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cloudhsm"></a>
 
 # mypy-boto3-cloudhsm
 
 [![PyPI - mypy-boto3-cloudhsm](https://img.shields.io/pypi/v/mypy-boto3-cloudhsm.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudhsm.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudhsm?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudhsm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudhsm)](https://pepy.tech/project/mypy-boto3-cloudhsm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudHSM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
+[boto3.CloudHSM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
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
 [mypy-boto3-cloudhsm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -363,14 +363,15 @@
     ListHsmsRequestListHsmsPaginateTypeDef,
     ListHsmsRequestRequestTypeDef,
     ListHsmsResponseTypeDef,
     ListLunaClientsRequestListLunaClientsPaginateTypeDef,
     ListLunaClientsRequestRequestTypeDef,
     ListLunaClientsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ModifyHapgRequestRequestTypeDef,
     ModifyHapgResponseTypeDef,
     ModifyHsmRequestRequestTypeDef,
     ModifyHsmResponseTypeDef,
     ModifyLunaClientRequestRequestTypeDef,
     ModifyLunaClientResponseTypeDef,
     PaginatorConfigTypeDef,
```

### Comparing `mypy-boto3-cloudhsm-1.28.0/mypy_boto3_cloudhsm.egg-info/SOURCES.txt` & `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsm-1.28.0/setup.py` & `mypy-boto3-cloudhsm-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudhsm",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_cloudhsm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudHSM 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.CloudHSM 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

