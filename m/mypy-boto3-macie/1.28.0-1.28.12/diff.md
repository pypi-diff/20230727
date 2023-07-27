# Comparing `tmp/mypy-boto3-macie-1.28.0.tar.gz` & `tmp/mypy-boto3-macie-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-macie-1.28.0.tar", last modified: Thu Jul  6 21:00:02 2023, max compression
+gzip compressed data, was "mypy-boto3-macie-1.28.12.tar", last modified: Thu Jul 27 05:34:59 2023, max compression
```

## Comparing `mypy-boto3-macie-1.28.0.tar` & `mypy-boto3-macie-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:02.774361 mypy-boto3-macie-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:46:24.000000 mypy-boto3-macie-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-07-06 21:00:02.770361 mypy-boto3-macie-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12121 2023-07-06 20:46:24.000000 mypy-boto3-macie-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:02.770361 mypy-boto3-macie-1.28.0/mypy_boto3_macie/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-06 20:46:24.000000 mypy-boto3-macie-1.28.0/mypy_boto3_macie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-06 20:46:24.000000 mypy-boto3-macie-1.28.0/mypy_boto3_macie/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-06 20:46:24.000000 mypy-boto3-macie-1.28.0/mypy_boto3_macie/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-07-06 20:46:24.000000 mypy-boto3-macie-1.28.0/mypy_boto3_macie/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-07-06 20:46:24.000000 mypy-boto3-macie-1.28.0/mypy_boto3_macie/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-07-06 20:46:24.000000 mypy-boto3-macie-1.28.0/mypy_boto3_macie/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-07-06 20:46:24.000000 mypy-boto3-macie-1.28.0/mypy_boto3_macie/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-06 20:46:24.000000 mypy-boto3-macie-1.28.0/mypy_boto3_macie/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-06 20:46:24.000000 mypy-boto3-macie-1.28.0/mypy_boto3_macie/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:46:24.000000 mypy-boto3-macie-1.28.0/mypy_boto3_macie/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-06 20:46:24.000000 mypy-boto3-macie-1.28.0/mypy_boto3_macie/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-07-06 20:46:24.000000 mypy-boto3-macie-1.28.0/mypy_boto3_macie/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:46:24.000000 mypy-boto3-macie-1.28.0/mypy_boto3_macie/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:02.770361 mypy-boto3-macie-1.28.0/mypy_boto3_macie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-07-06 21:00:02.000000 mypy-boto3-macie-1.28.0/mypy_boto3_macie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-06 21:00:02.000000 mypy-boto3-macie-1.28.0/mypy_boto3_macie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:02.000000 mypy-boto3-macie-1.28.0/mypy_boto3_macie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:02.000000 mypy-boto3-macie-1.28.0/mypy_boto3_macie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:02.000000 mypy-boto3-macie-1.28.0/mypy_boto3_macie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 21:00:02.000000 mypy-boto3-macie-1.28.0/mypy_boto3_macie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:02.774361 mypy-boto3-macie-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-06 20:46:23.000000 mypy-boto3-macie-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.032448 mypy-boto3-macie-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:44.000000 mypy-boto3-macie-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-07-27 05:34:59.032448 mypy-boto3-macie-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-07-27 05:25:44.000000 mypy-boto3-macie-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.032448 mypy-boto3-macie-1.28.12/mypy_boto3_macie/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-27 05:25:44.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-27 05:25:44.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 05:25:44.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-07-27 05:25:45.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-07-27 05:25:44.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-27 05:25:45.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-07-27 05:25:45.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-27 05:25:45.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-27 05:25:45.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:44.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-07-27 05:25:45.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-07-27 05:25:45.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:44.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.032448 mypy-boto3-macie-1.28.12/mypy_boto3_macie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-07-27 05:34:58.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-27 05:34:58.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:58.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:58.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:58.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 05:34:58.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:59.032448 mypy-boto3-macie-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 05:25:44.000000 mypy-boto3-macie-1.28.12/setup.py
```

### Comparing `mypy-boto3-macie-1.28.0/LICENSE` & `mypy-boto3-macie-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie-1.28.0/PKG-INFO` & `mypy-boto3-macie-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-macie
-Version: 1.28.0
-Summary: Type annotations for boto3.Macie 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Macie 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-macie"></a>
 
 # mypy-boto3-macie
 
 [![PyPI - mypy-boto3-macie](https://img.shields.io/pypi/v/mypy-boto3-macie.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-macie.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-macie?color=blue)](https://pypistats.org/packages/mypy-boto3-macie)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-macie)](https://pepy.tech/project/mypy-boto3-macie)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Macie 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
+[boto3.Macie 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
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
 [mypy-boto3-macie docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,33 +325,36 @@
 
 `mypy_boto3_macie.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_macie.type_defs import (
     AssociateMemberAccountRequestRequestTypeDef,
+    ClassificationTypeOutputTypeDef,
     ClassificationTypeTypeDef,
     ClassificationTypeUpdateTypeDef,
     DisassociateMemberAccountRequestRequestTypeDef,
     S3ResourceTypeDef,
     EmptyResponseMetadataTypeDef,
+    S3ResourceOutputTypeDef,
     ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
     ListMemberAccountsRequestRequestTypeDef,
     MemberAccountTypeDef,
     ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
     ListS3ResourcesRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
+    S3ResourceClassificationOutputTypeDef,
     S3ResourceClassificationTypeDef,
     S3ResourceClassificationUpdateTypeDef,
     DisassociateS3ResourcesRequestRequestTypeDef,
     FailedS3ResourceTypeDef,
     ListMemberAccountsResultTypeDef,
-    AssociateS3ResourcesRequestRequestTypeDef,
     ListS3ResourcesResultTypeDef,
+    AssociateS3ResourcesRequestRequestTypeDef,
     UpdateS3ResourcesRequestRequestTypeDef,
     AssociateS3ResourcesResultTypeDef,
     DisassociateS3ResourcesResultTypeDef,
     UpdateS3ResourcesResultTypeDef,
 )
```

### Comparing `mypy-boto3-macie-1.28.0/README.md` & `mypy-boto3-macie-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-macie"></a>
 
 # mypy-boto3-macie
 
 [![PyPI - mypy-boto3-macie](https://img.shields.io/pypi/v/mypy-boto3-macie.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-macie.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-macie?color=blue)](https://pypistats.org/packages/mypy-boto3-macie)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-macie)](https://pepy.tech/project/mypy-boto3-macie)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Macie 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
+[boto3.Macie 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
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
 [mypy-boto3-macie docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/).
 
 See how it helps to find and fix potential bugs:
 
@@ -293,33 +293,36 @@
 
 `mypy_boto3_macie.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_macie.type_defs import (
     AssociateMemberAccountRequestRequestTypeDef,
+    ClassificationTypeOutputTypeDef,
     ClassificationTypeTypeDef,
     ClassificationTypeUpdateTypeDef,
     DisassociateMemberAccountRequestRequestTypeDef,
     S3ResourceTypeDef,
     EmptyResponseMetadataTypeDef,
+    S3ResourceOutputTypeDef,
     ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
     ListMemberAccountsRequestRequestTypeDef,
     MemberAccountTypeDef,
     ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
     ListS3ResourcesRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
+    S3ResourceClassificationOutputTypeDef,
     S3ResourceClassificationTypeDef,
     S3ResourceClassificationUpdateTypeDef,
     DisassociateS3ResourcesRequestRequestTypeDef,
     FailedS3ResourceTypeDef,
     ListMemberAccountsResultTypeDef,
-    AssociateS3ResourcesRequestRequestTypeDef,
     ListS3ResourcesResultTypeDef,
+    AssociateS3ResourcesRequestRequestTypeDef,
     UpdateS3ResourcesRequestRequestTypeDef,
     AssociateS3ResourcesResultTypeDef,
     DisassociateS3ResourcesResultTypeDef,
     UpdateS3ResourcesResultTypeDef,
 )
```

### Comparing `mypy-boto3-macie-1.28.0/mypy_boto3_macie/__init__.py` & `mypy-boto3-macie-1.28.12/mypy_boto3_macie/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie-1.28.0/mypy_boto3_macie/__init__.pyi` & `mypy-boto3-macie-1.28.12/mypy_boto3_macie/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie-1.28.0/mypy_boto3_macie/__main__.py` & `mypy-boto3-macie-1.28.12/mypy_boto3_macie/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Macie 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Macie 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie\nOther"
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

### Comparing `mypy-boto3-macie-1.28.0/mypy_boto3_macie/client.py` & `mypy-boto3-macie-1.28.12/mypy_boto3_macie/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie-1.28.0/mypy_boto3_macie/client.pyi` & `mypy-boto3-macie-1.28.12/mypy_boto3_macie/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie-1.28.0/mypy_boto3_macie/literals.py` & `mypy-boto3-macie-1.28.12/mypy_boto3_macie/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,15 @@
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
@@ -238,26 +239,28 @@
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

### Comparing `mypy-boto3-macie-1.28.0/mypy_boto3_macie/literals.pyi` & `mypy-boto3-macie-1.28.12/mypy_boto3_macie/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,15 @@
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
@@ -236,26 +237,28 @@
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

### Comparing `mypy-boto3-macie-1.28.0/mypy_boto3_macie/paginator.py` & `mypy-boto3-macie-1.28.12/mypy_boto3_macie/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie-1.28.0/mypy_boto3_macie/paginator.pyi` & `mypy-boto3-macie-1.28.12/mypy_boto3_macie/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie-1.28.0/mypy_boto3_macie/type_defs.py` & `mypy-boto3-macie-1.28.12/mypy_boto3_macie/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -21,49 +21,59 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateMemberAccountRequestRequestTypeDef",
+    "ClassificationTypeOutputTypeDef",
     "ClassificationTypeTypeDef",
     "ClassificationTypeUpdateTypeDef",
     "DisassociateMemberAccountRequestRequestTypeDef",
     "S3ResourceTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "S3ResourceOutputTypeDef",
     "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
     "ListMemberAccountsRequestRequestTypeDef",
     "MemberAccountTypeDef",
     "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
     "ListS3ResourcesRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
+    "S3ResourceClassificationOutputTypeDef",
     "S3ResourceClassificationTypeDef",
     "S3ResourceClassificationUpdateTypeDef",
     "DisassociateS3ResourcesRequestRequestTypeDef",
     "FailedS3ResourceTypeDef",
     "ListMemberAccountsResultTypeDef",
-    "AssociateS3ResourcesRequestRequestTypeDef",
     "ListS3ResourcesResultTypeDef",
+    "AssociateS3ResourcesRequestRequestTypeDef",
     "UpdateS3ResourcesRequestRequestTypeDef",
     "AssociateS3ResourcesResultTypeDef",
     "DisassociateS3ResourcesResultTypeDef",
     "UpdateS3ResourcesResultTypeDef",
 )
 
 AssociateMemberAccountRequestRequestTypeDef = TypedDict(
     "AssociateMemberAccountRequestRequestTypeDef",
     {
         "memberAccountId": str,
     },
 )
 
+ClassificationTypeOutputTypeDef = TypedDict(
+    "ClassificationTypeOutputTypeDef",
+    {
+        "oneTime": S3OneTimeClassificationTypeType,
+        "continuous": Literal["FULL"],
+    },
+)
+
 ClassificationTypeTypeDef = TypedDict(
     "ClassificationTypeTypeDef",
     {
         "oneTime": S3OneTimeClassificationTypeType,
         "continuous": Literal["FULL"],
     },
 )
@@ -94,26 +104,41 @@
     "_OptionalS3ResourceTypeDef",
     {
         "prefix": str,
     },
     total=False,
 )
 
-
 class S3ResourceTypeDef(_RequiredS3ResourceTypeDef, _OptionalS3ResourceTypeDef):
     pass
 
-
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredS3ResourceOutputTypeDef = TypedDict(
+    "_RequiredS3ResourceOutputTypeDef",
+    {
+        "bucketName": str,
+    },
+)
+_OptionalS3ResourceOutputTypeDef = TypedDict(
+    "_OptionalS3ResourceOutputTypeDef",
+    {
+        "prefix": str,
+    },
+    total=False,
+)
+
+class S3ResourceOutputTypeDef(_RequiredS3ResourceOutputTypeDef, _OptionalS3ResourceOutputTypeDef):
+    pass
+
 ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
     "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -171,14 +196,34 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+_RequiredS3ResourceClassificationOutputTypeDef = TypedDict(
+    "_RequiredS3ResourceClassificationOutputTypeDef",
+    {
+        "bucketName": str,
+        "classificationType": ClassificationTypeOutputTypeDef,
+    },
+)
+_OptionalS3ResourceClassificationOutputTypeDef = TypedDict(
+    "_OptionalS3ResourceClassificationOutputTypeDef",
+    {
+        "prefix": str,
+    },
+    total=False,
+)
+
+class S3ResourceClassificationOutputTypeDef(
+    _RequiredS3ResourceClassificationOutputTypeDef, _OptionalS3ResourceClassificationOutputTypeDef
+):
+    pass
+
 _RequiredS3ResourceClassificationTypeDef = TypedDict(
     "_RequiredS3ResourceClassificationTypeDef",
     {
         "bucketName": str,
         "classificationType": ClassificationTypeTypeDef,
     },
 )
@@ -186,21 +231,19 @@
     "_OptionalS3ResourceClassificationTypeDef",
     {
         "prefix": str,
     },
     total=False,
 )
 
-
 class S3ResourceClassificationTypeDef(
     _RequiredS3ResourceClassificationTypeDef, _OptionalS3ResourceClassificationTypeDef
 ):
     pass
 
-
 _RequiredS3ResourceClassificationUpdateTypeDef = TypedDict(
     "_RequiredS3ResourceClassificationUpdateTypeDef",
     {
         "bucketName": str,
         "classificationTypeUpdate": ClassificationTypeUpdateTypeDef,
     },
 )
@@ -208,47 +251,43 @@
     "_OptionalS3ResourceClassificationUpdateTypeDef",
     {
         "prefix": str,
     },
     total=False,
 )
 
-
 class S3ResourceClassificationUpdateTypeDef(
     _RequiredS3ResourceClassificationUpdateTypeDef, _OptionalS3ResourceClassificationUpdateTypeDef
 ):
     pass
 
-
 _RequiredDisassociateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateS3ResourcesRequestRequestTypeDef",
     {
         "associatedS3Resources": Sequence[S3ResourceTypeDef],
     },
 )
 _OptionalDisassociateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_OptionalDisassociateS3ResourcesRequestRequestTypeDef",
     {
         "memberAccountId": str,
     },
     total=False,
 )
 
-
 class DisassociateS3ResourcesRequestRequestTypeDef(
     _RequiredDisassociateS3ResourcesRequestRequestTypeDef,
     _OptionalDisassociateS3ResourcesRequestRequestTypeDef,
 ):
     pass
 
-
 FailedS3ResourceTypeDef = TypedDict(
     "FailedS3ResourceTypeDef",
     {
-        "failedItem": S3ResourceTypeDef,
+        "failedItem": S3ResourceOutputTypeDef,
         "errorCode": str,
         "errorMessage": str,
     },
     total=False,
 )
 
 ListMemberAccountsResultTypeDef = TypedDict(
@@ -256,66 +295,62 @@
     {
         "memberAccounts": List[MemberAccountTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListS3ResourcesResultTypeDef = TypedDict(
+    "ListS3ResourcesResultTypeDef",
+    {
+        "s3Resources": List[S3ResourceClassificationOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAssociateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateS3ResourcesRequestRequestTypeDef",
     {
         "s3Resources": Sequence[S3ResourceClassificationTypeDef],
     },
 )
 _OptionalAssociateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_OptionalAssociateS3ResourcesRequestRequestTypeDef",
     {
         "memberAccountId": str,
     },
     total=False,
 )
 
-
 class AssociateS3ResourcesRequestRequestTypeDef(
     _RequiredAssociateS3ResourcesRequestRequestTypeDef,
     _OptionalAssociateS3ResourcesRequestRequestTypeDef,
 ):
     pass
 
-
-ListS3ResourcesResultTypeDef = TypedDict(
-    "ListS3ResourcesResultTypeDef",
-    {
-        "s3Resources": List[S3ResourceClassificationTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateS3ResourcesRequestRequestTypeDef",
     {
         "s3ResourcesUpdate": Sequence[S3ResourceClassificationUpdateTypeDef],
     },
 )
 _OptionalUpdateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateS3ResourcesRequestRequestTypeDef",
     {
         "memberAccountId": str,
     },
     total=False,
 )
 
-
 class UpdateS3ResourcesRequestRequestTypeDef(
     _RequiredUpdateS3ResourcesRequestRequestTypeDef, _OptionalUpdateS3ResourcesRequestRequestTypeDef
 ):
     pass
 
-
 AssociateS3ResourcesResultTypeDef = TypedDict(
     "AssociateS3ResourcesResultTypeDef",
     {
         "failedS3Resources": List[FailedS3ResourceTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-macie-1.28.0/mypy_boto3_macie/type_defs.pyi` & `mypy-boto3-macie-1.28.12/mypy_boto3_macie/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,48 +21,60 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssociateMemberAccountRequestRequestTypeDef",
+    "ClassificationTypeOutputTypeDef",
     "ClassificationTypeTypeDef",
     "ClassificationTypeUpdateTypeDef",
     "DisassociateMemberAccountRequestRequestTypeDef",
     "S3ResourceTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "S3ResourceOutputTypeDef",
     "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
     "ListMemberAccountsRequestRequestTypeDef",
     "MemberAccountTypeDef",
     "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
     "ListS3ResourcesRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
+    "S3ResourceClassificationOutputTypeDef",
     "S3ResourceClassificationTypeDef",
     "S3ResourceClassificationUpdateTypeDef",
     "DisassociateS3ResourcesRequestRequestTypeDef",
     "FailedS3ResourceTypeDef",
     "ListMemberAccountsResultTypeDef",
-    "AssociateS3ResourcesRequestRequestTypeDef",
     "ListS3ResourcesResultTypeDef",
+    "AssociateS3ResourcesRequestRequestTypeDef",
     "UpdateS3ResourcesRequestRequestTypeDef",
     "AssociateS3ResourcesResultTypeDef",
     "DisassociateS3ResourcesResultTypeDef",
     "UpdateS3ResourcesResultTypeDef",
 )
 
 AssociateMemberAccountRequestRequestTypeDef = TypedDict(
     "AssociateMemberAccountRequestRequestTypeDef",
     {
         "memberAccountId": str,
     },
 )
 
+ClassificationTypeOutputTypeDef = TypedDict(
+    "ClassificationTypeOutputTypeDef",
+    {
+        "oneTime": S3OneTimeClassificationTypeType,
+        "continuous": Literal["FULL"],
+    },
+)
+
 ClassificationTypeTypeDef = TypedDict(
     "ClassificationTypeTypeDef",
     {
         "oneTime": S3OneTimeClassificationTypeType,
         "continuous": Literal["FULL"],
     },
 )
@@ -93,24 +105,45 @@
     "_OptionalS3ResourceTypeDef",
     {
         "prefix": str,
     },
     total=False,
 )
 
+
 class S3ResourceTypeDef(_RequiredS3ResourceTypeDef, _OptionalS3ResourceTypeDef):
     pass
 
+
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredS3ResourceOutputTypeDef = TypedDict(
+    "_RequiredS3ResourceOutputTypeDef",
+    {
+        "bucketName": str,
+    },
+)
+_OptionalS3ResourceOutputTypeDef = TypedDict(
+    "_OptionalS3ResourceOutputTypeDef",
+    {
+        "prefix": str,
+    },
+    total=False,
+)
+
+
+class S3ResourceOutputTypeDef(_RequiredS3ResourceOutputTypeDef, _OptionalS3ResourceOutputTypeDef):
+    pass
+
+
 ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
     "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -168,14 +201,36 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+_RequiredS3ResourceClassificationOutputTypeDef = TypedDict(
+    "_RequiredS3ResourceClassificationOutputTypeDef",
+    {
+        "bucketName": str,
+        "classificationType": ClassificationTypeOutputTypeDef,
+    },
+)
+_OptionalS3ResourceClassificationOutputTypeDef = TypedDict(
+    "_OptionalS3ResourceClassificationOutputTypeDef",
+    {
+        "prefix": str,
+    },
+    total=False,
+)
+
+
+class S3ResourceClassificationOutputTypeDef(
+    _RequiredS3ResourceClassificationOutputTypeDef, _OptionalS3ResourceClassificationOutputTypeDef
+):
+    pass
+
+
 _RequiredS3ResourceClassificationTypeDef = TypedDict(
     "_RequiredS3ResourceClassificationTypeDef",
     {
         "bucketName": str,
         "classificationType": ClassificationTypeTypeDef,
     },
 )
@@ -183,19 +238,21 @@
     "_OptionalS3ResourceClassificationTypeDef",
     {
         "prefix": str,
     },
     total=False,
 )
 
+
 class S3ResourceClassificationTypeDef(
     _RequiredS3ResourceClassificationTypeDef, _OptionalS3ResourceClassificationTypeDef
 ):
     pass
 
+
 _RequiredS3ResourceClassificationUpdateTypeDef = TypedDict(
     "_RequiredS3ResourceClassificationUpdateTypeDef",
     {
         "bucketName": str,
         "classificationTypeUpdate": ClassificationTypeUpdateTypeDef,
     },
 )
@@ -203,43 +260,47 @@
     "_OptionalS3ResourceClassificationUpdateTypeDef",
     {
         "prefix": str,
     },
     total=False,
 )
 
+
 class S3ResourceClassificationUpdateTypeDef(
     _RequiredS3ResourceClassificationUpdateTypeDef, _OptionalS3ResourceClassificationUpdateTypeDef
 ):
     pass
 
+
 _RequiredDisassociateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateS3ResourcesRequestRequestTypeDef",
     {
         "associatedS3Resources": Sequence[S3ResourceTypeDef],
     },
 )
 _OptionalDisassociateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_OptionalDisassociateS3ResourcesRequestRequestTypeDef",
     {
         "memberAccountId": str,
     },
     total=False,
 )
 
+
 class DisassociateS3ResourcesRequestRequestTypeDef(
     _RequiredDisassociateS3ResourcesRequestRequestTypeDef,
     _OptionalDisassociateS3ResourcesRequestRequestTypeDef,
 ):
     pass
 
+
 FailedS3ResourceTypeDef = TypedDict(
     "FailedS3ResourceTypeDef",
     {
-        "failedItem": S3ResourceTypeDef,
+        "failedItem": S3ResourceOutputTypeDef,
         "errorCode": str,
         "errorMessage": str,
     },
     total=False,
 )
 
 ListMemberAccountsResultTypeDef = TypedDict(
@@ -247,42 +308,44 @@
     {
         "memberAccounts": List[MemberAccountTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListS3ResourcesResultTypeDef = TypedDict(
+    "ListS3ResourcesResultTypeDef",
+    {
+        "s3Resources": List[S3ResourceClassificationOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAssociateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateS3ResourcesRequestRequestTypeDef",
     {
         "s3Resources": Sequence[S3ResourceClassificationTypeDef],
     },
 )
 _OptionalAssociateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_OptionalAssociateS3ResourcesRequestRequestTypeDef",
     {
         "memberAccountId": str,
     },
     total=False,
 )
 
+
 class AssociateS3ResourcesRequestRequestTypeDef(
     _RequiredAssociateS3ResourcesRequestRequestTypeDef,
     _OptionalAssociateS3ResourcesRequestRequestTypeDef,
 ):
     pass
 
-ListS3ResourcesResultTypeDef = TypedDict(
-    "ListS3ResourcesResultTypeDef",
-    {
-        "s3Resources": List[S3ResourceClassificationTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateS3ResourcesRequestRequestTypeDef",
     {
         "s3ResourcesUpdate": Sequence[S3ResourceClassificationUpdateTypeDef],
     },
 )
@@ -290,19 +353,21 @@
     "_OptionalUpdateS3ResourcesRequestRequestTypeDef",
     {
         "memberAccountId": str,
     },
     total=False,
 )
 
+
 class UpdateS3ResourcesRequestRequestTypeDef(
     _RequiredUpdateS3ResourcesRequestRequestTypeDef, _OptionalUpdateS3ResourcesRequestRequestTypeDef
 ):
     pass
 
+
 AssociateS3ResourcesResultTypeDef = TypedDict(
     "AssociateS3ResourcesResultTypeDef",
     {
         "failedS3Resources": List[FailedS3ResourceTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-macie-1.28.0/mypy_boto3_macie.egg-info/PKG-INFO` & `mypy-boto3-macie-1.28.12/mypy_boto3_macie.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-macie
-Version: 1.28.0
-Summary: Type annotations for boto3.Macie 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Macie 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-macie"></a>
 
 # mypy-boto3-macie
 
 [![PyPI - mypy-boto3-macie](https://img.shields.io/pypi/v/mypy-boto3-macie.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-macie.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-macie?color=blue)](https://pypistats.org/packages/mypy-boto3-macie)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-macie)](https://pepy.tech/project/mypy-boto3-macie)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Macie 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
+[boto3.Macie 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
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
 [mypy-boto3-macie docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,33 +325,36 @@
 
 `mypy_boto3_macie.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_macie.type_defs import (
     AssociateMemberAccountRequestRequestTypeDef,
+    ClassificationTypeOutputTypeDef,
     ClassificationTypeTypeDef,
     ClassificationTypeUpdateTypeDef,
     DisassociateMemberAccountRequestRequestTypeDef,
     S3ResourceTypeDef,
     EmptyResponseMetadataTypeDef,
+    S3ResourceOutputTypeDef,
     ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
     ListMemberAccountsRequestRequestTypeDef,
     MemberAccountTypeDef,
     ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
     ListS3ResourcesRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
+    S3ResourceClassificationOutputTypeDef,
     S3ResourceClassificationTypeDef,
     S3ResourceClassificationUpdateTypeDef,
     DisassociateS3ResourcesRequestRequestTypeDef,
     FailedS3ResourceTypeDef,
     ListMemberAccountsResultTypeDef,
-    AssociateS3ResourcesRequestRequestTypeDef,
     ListS3ResourcesResultTypeDef,
+    AssociateS3ResourcesRequestRequestTypeDef,
     UpdateS3ResourcesRequestRequestTypeDef,
     AssociateS3ResourcesResultTypeDef,
     DisassociateS3ResourcesResultTypeDef,
     UpdateS3ResourcesResultTypeDef,
 )
```

### Comparing `mypy-boto3-macie-1.28.0/mypy_boto3_macie.egg-info/SOURCES.txt` & `mypy-boto3-macie-1.28.12/mypy_boto3_macie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie-1.28.0/setup.py` & `mypy-boto3-macie-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-macie",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_macie"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Macie 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Macie 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

