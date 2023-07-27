# Comparing `tmp/mypy-boto3-cloud9-1.28.0.tar.gz` & `tmp/mypy-boto3-cloud9-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloud9-1.28.0.tar", last modified: Thu Jul  6 20:59:08 2023, max compression
+gzip compressed data, was "mypy-boto3-cloud9-1.28.12.tar", last modified: Thu Jul 27 05:34:24 2023, max compression
```

## Comparing `mypy-boto3-cloud9-1.28.0.tar` & `mypy-boto3-cloud9-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:08.978242 mypy-boto3-cloud9-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:34:56.000000 mypy-boto3-cloud9-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-07-06 20:59:08.974243 mypy-boto3-cloud9-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-07-06 20:34:56.000000 mypy-boto3-cloud9-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:08.970243 mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-06 20:34:56.000000 mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-06 20:34:56.000000 mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-06 20:34:56.000000 mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-06 20:34:56.000000 mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-07-06 20:34:56.000000 mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-07-06 20:34:56.000000 mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-07-06 20:34:56.000000 mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-07-06 20:34:56.000000 mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-06 20:34:56.000000 mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:56.000000 mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-07-06 20:34:58.000000 mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-07-06 20:34:57.000000 mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:34:56.000000 mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:08.974243 mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-07-06 20:59:08.000000 mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-06 20:59:08.000000 mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:08.000000 mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:08.000000 mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:08.000000 mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 20:59:08.000000 mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:08.978242 mypy-boto3-cloud9-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-06 20:34:56.000000 mypy-boto3-cloud9-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.860563 mypy-boto3-cloud9-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-07-27 05:34:24.860563 mypy-boto3-cloud9-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12674 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.856563 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9526 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.860563 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-07-27 05:34:24.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 05:34:24.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:24.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 05:34:24.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:24.860563 mypy-boto3-cloud9-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/setup.py
```

### Comparing `mypy-boto3-cloud9-1.28.0/LICENSE` & `mypy-boto3-cloud9-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloud9-1.28.0/PKG-INFO` & `mypy-boto3-cloud9-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloud9
-Version: 1.28.0
-Summary: Type annotations for boto3.Cloud9 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Cloud9 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cloud9"></a>
 
 # mypy-boto3-cloud9
 
 [![PyPI - mypy-boto3-cloud9](https://img.shields.io/pypi/v/mypy-boto3-cloud9.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloud9)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloud9.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloud9)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloud9?color=blue)](https://pypistats.org/packages/mypy-boto3-cloud9)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloud9)](https://pepy.tech/project/mypy-boto3-cloud9)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Cloud9 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
+[boto3.Cloud9 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
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
 [mypy-boto3-cloud9 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,26 +349,27 @@
     DescribeEnvironmentStatusResultTypeDef,
     DescribeEnvironmentsRequestRequestTypeDef,
     EnvironmentLifecycleTypeDef,
     ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListEnvironmentsResultTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEnvironmentMembershipRequestRequestTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentEC2RequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateEnvironmentMembershipResultTypeDef,
     DescribeEnvironmentMembershipsResultTypeDef,
     UpdateEnvironmentMembershipResultTypeDef,
     EnvironmentTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DescribeEnvironmentsResultTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-cloud9-1.28.0/README.md` & `mypy-boto3-cloud9-1.28.12/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cloud9"></a>
 
 # mypy-boto3-cloud9
 
 [![PyPI - mypy-boto3-cloud9](https://img.shields.io/pypi/v/mypy-boto3-cloud9.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloud9)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloud9.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloud9)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloud9?color=blue)](https://pypistats.org/packages/mypy-boto3-cloud9)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloud9)](https://pepy.tech/project/mypy-boto3-cloud9)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Cloud9 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
+[boto3.Cloud9 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
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
 [mypy-boto3-cloud9 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/).
 
 See how it helps to find and fix potential bugs:
 
@@ -317,26 +317,27 @@
     DescribeEnvironmentStatusResultTypeDef,
     DescribeEnvironmentsRequestRequestTypeDef,
     EnvironmentLifecycleTypeDef,
     ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListEnvironmentsResultTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEnvironmentMembershipRequestRequestTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentEC2RequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateEnvironmentMembershipResultTypeDef,
     DescribeEnvironmentMembershipsResultTypeDef,
     UpdateEnvironmentMembershipResultTypeDef,
     EnvironmentTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DescribeEnvironmentsResultTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/__init__.py` & `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/__init__.pyi` & `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/__main__.py` & `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Cloud9 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Cloud9 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9\nOther"
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

### Comparing `mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/client.py` & `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/client.pyi` & `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/literals.py` & `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,15 @@
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
@@ -266,26 +267,28 @@
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

### Comparing `mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/literals.pyi` & `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -178,14 +178,15 @@
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
@@ -264,26 +265,28 @@
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

### Comparing `mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/paginator.py` & `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/paginator.pyi` & `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/type_defs.py` & `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
     "CreateEnvironmentEC2ResultTypeDef",
     "CreateEnvironmentMembershipRequestRequestTypeDef",
     "EnvironmentMemberTypeDef",
     "DeleteEnvironmentMembershipRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
@@ -45,26 +44,27 @@
     "DescribeEnvironmentStatusResultTypeDef",
     "DescribeEnvironmentsRequestRequestTypeDef",
     "EnvironmentLifecycleTypeDef",
     "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListEnvironmentsResultTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEnvironmentMembershipRequestRequestTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentEC2RequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateEnvironmentMembershipResultTypeDef",
     "DescribeEnvironmentMembershipsResultTypeDef",
     "UpdateEnvironmentMembershipResultTypeDef",
     "EnvironmentTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "DescribeEnvironmentsResultTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
@@ -102,21 +102,19 @@
     "_OptionalEnvironmentMemberTypeDef",
     {
         "lastAccess": datetime,
     },
     total=False,
 )
 
-
 class EnvironmentMemberTypeDef(
     _RequiredEnvironmentMemberTypeDef, _OptionalEnvironmentMemberTypeDef
 ):
     pass
 
-
 DeleteEnvironmentMembershipRequestRequestTypeDef = TypedDict(
     "DeleteEnvironmentMembershipRequestRequestTypeDef",
     {
         "environmentId": str,
         "userArn": str,
     },
 )
@@ -213,14 +211,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -267,21 +273,19 @@
         "name": str,
         "description": str,
         "managedCredentialsAction": ManagedCredentialsActionType,
     },
     total=False,
 )
 
-
 class UpdateEnvironmentRequestRequestTypeDef(
     _RequiredUpdateEnvironmentRequestRequestTypeDef, _OptionalUpdateEnvironmentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateEnvironmentEC2RequestRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentEC2RequestRequestTypeDef",
     {
         "name": str,
         "instanceType": str,
     },
 )
@@ -297,30 +301,20 @@
         "tags": Sequence[TagTypeDef],
         "connectionType": ConnectionTypeType,
         "dryRun": bool,
     },
     total=False,
 )
 
-
 class CreateEnvironmentEC2RequestRequestTypeDef(
     _RequiredCreateEnvironmentEC2RequestRequestTypeDef,
     _OptionalCreateEnvironmentEC2RequestRequestTypeDef,
 ):
     pass
 
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -367,18 +361,24 @@
         "connectionType": ConnectionTypeType,
         "lifecycle": EnvironmentLifecycleTypeDef,
         "managedCredentialsStatus": ManagedCredentialsStatusType,
     },
     total=False,
 )
 
-
 class EnvironmentTypeDef(_RequiredEnvironmentTypeDef, _OptionalEnvironmentTypeDef):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 DescribeEnvironmentsResultTypeDef = TypedDict(
     "DescribeEnvironmentsResultTypeDef",
     {
         "environments": List[EnvironmentTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9/type_defs.pyi` & `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TagTypeDef",
     "CreateEnvironmentEC2ResultTypeDef",
     "CreateEnvironmentMembershipRequestRequestTypeDef",
     "EnvironmentMemberTypeDef",
     "DeleteEnvironmentMembershipRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
@@ -44,26 +45,27 @@
     "DescribeEnvironmentStatusResultTypeDef",
     "DescribeEnvironmentsRequestRequestTypeDef",
     "EnvironmentLifecycleTypeDef",
     "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListEnvironmentsResultTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEnvironmentMembershipRequestRequestTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentEC2RequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateEnvironmentMembershipResultTypeDef",
     "DescribeEnvironmentMembershipsResultTypeDef",
     "UpdateEnvironmentMembershipResultTypeDef",
     "EnvironmentTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "DescribeEnvironmentsResultTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
@@ -101,19 +103,21 @@
     "_OptionalEnvironmentMemberTypeDef",
     {
         "lastAccess": datetime,
     },
     total=False,
 )
 
+
 class EnvironmentMemberTypeDef(
     _RequiredEnvironmentMemberTypeDef, _OptionalEnvironmentMemberTypeDef
 ):
     pass
 
+
 DeleteEnvironmentMembershipRequestRequestTypeDef = TypedDict(
     "DeleteEnvironmentMembershipRequestRequestTypeDef",
     {
         "environmentId": str,
         "userArn": str,
     },
 )
@@ -210,14 +214,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -264,19 +276,21 @@
         "name": str,
         "description": str,
         "managedCredentialsAction": ManagedCredentialsActionType,
     },
     total=False,
 )
 
+
 class UpdateEnvironmentRequestRequestTypeDef(
     _RequiredUpdateEnvironmentRequestRequestTypeDef, _OptionalUpdateEnvironmentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateEnvironmentEC2RequestRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentEC2RequestRequestTypeDef",
     {
         "name": str,
         "instanceType": str,
     },
 )
@@ -292,27 +306,21 @@
         "tags": Sequence[TagTypeDef],
         "connectionType": ConnectionTypeType,
         "dryRun": bool,
     },
     total=False,
 )
 
+
 class CreateEnvironmentEC2RequestRequestTypeDef(
     _RequiredCreateEnvironmentEC2RequestRequestTypeDef,
     _OptionalCreateEnvironmentEC2RequestRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
@@ -360,17 +368,27 @@
         "connectionType": ConnectionTypeType,
         "lifecycle": EnvironmentLifecycleTypeDef,
         "managedCredentialsStatus": ManagedCredentialsStatusType,
     },
     total=False,
 )
 
+
 class EnvironmentTypeDef(_RequiredEnvironmentTypeDef, _OptionalEnvironmentTypeDef):
     pass
 
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeEnvironmentsResultTypeDef = TypedDict(
     "DescribeEnvironmentsResultTypeDef",
     {
         "environments": List[EnvironmentTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9.egg-info/PKG-INFO` & `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloud9
-Version: 1.28.0
-Summary: Type annotations for boto3.Cloud9 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Cloud9 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cloud9"></a>
 
 # mypy-boto3-cloud9
 
 [![PyPI - mypy-boto3-cloud9](https://img.shields.io/pypi/v/mypy-boto3-cloud9.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloud9)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloud9.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloud9)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloud9?color=blue)](https://pypistats.org/packages/mypy-boto3-cloud9)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloud9)](https://pepy.tech/project/mypy-boto3-cloud9)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Cloud9 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
+[boto3.Cloud9 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
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
 [mypy-boto3-cloud9 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,26 +349,27 @@
     DescribeEnvironmentStatusResultTypeDef,
     DescribeEnvironmentsRequestRequestTypeDef,
     EnvironmentLifecycleTypeDef,
     ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListEnvironmentsResultTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEnvironmentMembershipRequestRequestTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentEC2RequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateEnvironmentMembershipResultTypeDef,
     DescribeEnvironmentMembershipsResultTypeDef,
     UpdateEnvironmentMembershipResultTypeDef,
     EnvironmentTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DescribeEnvironmentsResultTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-cloud9-1.28.0/mypy_boto3_cloud9.egg-info/SOURCES.txt` & `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloud9-1.28.0/setup.py` & `mypy-boto3-cloud9-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloud9",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_cloud9"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Cloud9 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Cloud9 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

