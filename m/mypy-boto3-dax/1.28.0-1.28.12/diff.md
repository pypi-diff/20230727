# Comparing `tmp/mypy-boto3-dax-1.28.0.tar.gz` & `tmp/mypy-boto3-dax-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dax-1.28.0.tar", last modified: Thu Jul  6 20:59:22 2023, max compression
+gzip compressed data, was "mypy-boto3-dax-1.28.12.tar", last modified: Thu Jul 27 05:34:33 2023, max compression
```

## Comparing `mypy-boto3-dax-1.28.0.tar` & `mypy-boto3-dax-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:22.958275 mypy-boto3-dax-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:37:34.000000 mypy-boto3-dax-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16099 2023-07-06 20:59:22.950275 mypy-boto3-dax-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14630 2023-07-06 20:37:34.000000 mypy-boto3-dax-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:22.950275 mypy-boto3-dax-1.28.0/mypy_boto3_dax/
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-06 20:37:34.000000 mypy-boto3-dax-1.28.0/mypy_boto3_dax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-06 20:37:34.000000 mypy-boto3-dax-1.28.0/mypy_boto3_dax/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:37:34.000000 mypy-boto3-dax-1.28.0/mypy_boto3_dax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-07-06 20:37:35.000000 mypy-boto3-dax-1.28.0/mypy_boto3_dax/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20389 2023-07-06 20:37:35.000000 mypy-boto3-dax-1.28.0/mypy_boto3_dax/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-07-06 20:37:35.000000 mypy-boto3-dax-1.28.0/mypy_boto3_dax/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-06 20:37:35.000000 mypy-boto3-dax-1.28.0/mypy_boto3_dax/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-06 20:37:35.000000 mypy-boto3-dax-1.28.0/mypy_boto3_dax/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-07-06 20:37:35.000000 mypy-boto3-dax-1.28.0/mypy_boto3_dax/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:37:34.000000 mypy-boto3-dax-1.28.0/mypy_boto3_dax/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22387 2023-07-06 20:37:37.000000 mypy-boto3-dax-1.28.0/mypy_boto3_dax/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22364 2023-07-06 20:37:37.000000 mypy-boto3-dax-1.28.0/mypy_boto3_dax/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:37:34.000000 mypy-boto3-dax-1.28.0/mypy_boto3_dax/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:22.950275 mypy-boto3-dax-1.28.0/mypy_boto3_dax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16099 2023-07-06 20:59:22.000000 mypy-boto3-dax-1.28.0/mypy_boto3_dax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 20:59:22.000000 mypy-boto3-dax-1.28.0/mypy_boto3_dax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:22.000000 mypy-boto3-dax-1.28.0/mypy_boto3_dax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:22.000000 mypy-boto3-dax-1.28.0/mypy_boto3_dax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:22.000000 mypy-boto3-dax-1.28.0/mypy_boto3_dax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:22.000000 mypy-boto3-dax-1.28.0/mypy_boto3_dax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:22.958275 mypy-boto3-dax-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:37:34.000000 mypy-boto3-dax-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.720536 mypy-boto3-dax-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-07-27 05:34:33.720536 mypy-boto3-dax-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.720536 mypy-boto3-dax-1.28.12/mypy_boto3_dax/
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20389 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-07-27 05:20:05.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22535 2023-07-27 05:20:05.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.720536 mypy-boto3-dax-1.28.12/mypy_boto3_dax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-07-27 05:34:33.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 05:34:33.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:33.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:33.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:33.720536 mypy-boto3-dax-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/setup.py
```

### Comparing `mypy-boto3-dax-1.28.0/LICENSE` & `mypy-boto3-dax-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.0/PKG-INFO` & `mypy-boto3-dax-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dax
-Version: 1.28.0
-Summary: Type annotations for boto3.DAX 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.DAX 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-dax"></a>
 
 # mypy-boto3-dax
 
 [![PyPI - mypy-boto3-dax](https://img.shields.io/pypi/v/mypy-boto3-dax.svg?color=blue)](https://pypi.org/project/mypy-boto3-dax)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dax.svg?color=blue)](https://pypi.org/project/mypy-boto3-dax)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dax?color=blue)](https://pypistats.org/packages/mypy-boto3-dax)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dax)](https://pepy.tech/project/mypy-boto3-dax)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DAX 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
+[boto3.DAX 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
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
 [mypy-boto3-dax docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/).
 
 See how it helps to find and fix potential bugs:
 
@@ -383,33 +383,34 @@
     DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeParametersRequestRequestTypeDef,
     DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeSubnetGroupsRequestRequestTypeDef,
     IncreaseReplicationFactorRequestRequestTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     NodeTypeSpecificValueTypeDef,
     PaginatorConfigTypeDef,
     ParameterNameValueTypeDef,
     RebootNodeRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     SubnetTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
     UpdateSubnetGroupRequestRequestTypeDef,
     NodeTypeDef,
     CreateClusterRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    TagResourceResponseTypeDef,
-    UntagResourceResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
     DescribeEventsResponseTypeDef,
+    ListTagsResponseTypeDef,
+    TagResourceResponseTypeDef,
+    UntagResourceResponseTypeDef,
     ParameterTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
     SubnetGroupTypeDef,
     ClusterTypeDef,
     DescribeDefaultParametersResponseTypeDef,
     DescribeParametersResponseTypeDef,
     CreateSubnetGroupResponseTypeDef,
```

### Comparing `mypy-boto3-dax-1.28.0/README.md` & `mypy-boto3-dax-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-dax"></a>
 
 # mypy-boto3-dax
 
 [![PyPI - mypy-boto3-dax](https://img.shields.io/pypi/v/mypy-boto3-dax.svg?color=blue)](https://pypi.org/project/mypy-boto3-dax)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dax.svg?color=blue)](https://pypi.org/project/mypy-boto3-dax)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dax?color=blue)](https://pypistats.org/packages/mypy-boto3-dax)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dax)](https://pepy.tech/project/mypy-boto3-dax)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DAX 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
+[boto3.DAX 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
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
 [mypy-boto3-dax docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/).
 
 See how it helps to find and fix potential bugs:
 
@@ -351,33 +351,34 @@
     DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeParametersRequestRequestTypeDef,
     DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeSubnetGroupsRequestRequestTypeDef,
     IncreaseReplicationFactorRequestRequestTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     NodeTypeSpecificValueTypeDef,
     PaginatorConfigTypeDef,
     ParameterNameValueTypeDef,
     RebootNodeRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     SubnetTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
     UpdateSubnetGroupRequestRequestTypeDef,
     NodeTypeDef,
     CreateClusterRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    TagResourceResponseTypeDef,
-    UntagResourceResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
     DescribeEventsResponseTypeDef,
+    ListTagsResponseTypeDef,
+    TagResourceResponseTypeDef,
+    UntagResourceResponseTypeDef,
     ParameterTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
     SubnetGroupTypeDef,
     ClusterTypeDef,
     DescribeDefaultParametersResponseTypeDef,
     DescribeParametersResponseTypeDef,
     CreateSubnetGroupResponseTypeDef,
```

### Comparing `mypy-boto3-dax-1.28.0/mypy_boto3_dax/__init__.py` & `mypy-boto3-dax-1.28.12/mypy_boto3_dax/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.0/mypy_boto3_dax/__init__.pyi` & `mypy-boto3-dax-1.28.12/mypy_boto3_dax/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.0/mypy_boto3_dax/__main__.py` & `mypy-boto3-dax-1.28.12/mypy_boto3_dax/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DAX 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.DAX 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX\nOther"
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

### Comparing `mypy-boto3-dax-1.28.0/mypy_boto3_dax/client.py` & `mypy-boto3-dax-1.28.12/mypy_boto3_dax/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.0/mypy_boto3_dax/client.pyi` & `mypy-boto3-dax-1.28.12/mypy_boto3_dax/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.0/mypy_boto3_dax/literals.py` & `mypy-boto3-dax-1.28.12/mypy_boto3_dax/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,15 @@
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
@@ -256,26 +257,28 @@
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

### Comparing `mypy-boto3-dax-1.28.0/mypy_boto3_dax/literals.pyi` & `mypy-boto3-dax-1.28.12/mypy_boto3_dax/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,15 @@
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
@@ -254,26 +255,28 @@
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

### Comparing `mypy-boto3-dax-1.28.0/mypy_boto3_dax/paginator.py` & `mypy-boto3-dax-1.28.12/mypy_boto3_dax/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.0/mypy_boto3_dax/paginator.pyi` & `mypy-boto3-dax-1.28.12/mypy_boto3_dax/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.0/mypy_boto3_dax/type_defs.py` & `mypy-boto3-dax-1.28.12/mypy_boto3_dax/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "EndpointTypeDef",
     "NotificationConfigurationTypeDef",
     "ParameterGroupStatusTypeDef",
     "SSEDescriptionTypeDef",
     "SecurityGroupMembershipTypeDef",
     "SSESpecificationTypeDef",
@@ -59,33 +58,34 @@
     "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     "DescribeParametersRequestRequestTypeDef",
     "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
     "DescribeSubnetGroupsRequestRequestTypeDef",
     "IncreaseReplicationFactorRequestRequestTypeDef",
     "ListTagsRequestListTagsPaginateTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "NodeTypeSpecificValueTypeDef",
     "PaginatorConfigTypeDef",
     "ParameterNameValueTypeDef",
     "RebootNodeRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "SubnetTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateClusterRequestRequestTypeDef",
     "UpdateSubnetGroupRequestRequestTypeDef",
     "NodeTypeDef",
     "CreateClusterRequestRequestTypeDef",
-    "ListTagsResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "TagResourceResponseTypeDef",
-    "UntagResourceResponseTypeDef",
     "CreateParameterGroupResponseTypeDef",
     "DescribeParameterGroupsResponseTypeDef",
     "UpdateParameterGroupResponseTypeDef",
     "DescribeEventsResponseTypeDef",
+    "ListTagsResponseTypeDef",
+    "TagResourceResponseTypeDef",
+    "UntagResourceResponseTypeDef",
     "ParameterTypeDef",
     "UpdateParameterGroupRequestRequestTypeDef",
     "SubnetGroupTypeDef",
     "ClusterTypeDef",
     "DescribeDefaultParametersResponseTypeDef",
     "DescribeParametersResponseTypeDef",
     "CreateSubnetGroupResponseTypeDef",
@@ -172,22 +172,20 @@
     "_OptionalCreateParameterGroupRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class CreateParameterGroupRequestRequestTypeDef(
     _RequiredCreateParameterGroupRequestRequestTypeDef,
     _OptionalCreateParameterGroupRequestRequestTypeDef,
 ):
     pass
 
-
 ParameterGroupTypeDef = TypedDict(
     "ParameterGroupTypeDef",
     {
         "ParameterGroupName": str,
         "Description": str,
     },
     total=False,
@@ -204,21 +202,19 @@
     "_OptionalCreateSubnetGroupRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class CreateSubnetGroupRequestRequestTypeDef(
     _RequiredCreateSubnetGroupRequestRequestTypeDef, _OptionalCreateSubnetGroupRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDecreaseReplicationFactorRequestRequestTypeDef = TypedDict(
     "_RequiredDecreaseReplicationFactorRequestRequestTypeDef",
     {
         "ClusterName": str,
         "NewReplicationFactor": int,
     },
 )
@@ -227,22 +223,20 @@
     {
         "AvailabilityZones": Sequence[str],
         "NodeIdsToRemove": Sequence[str],
     },
     total=False,
 )
 
-
 class DecreaseReplicationFactorRequestRequestTypeDef(
     _RequiredDecreaseReplicationFactorRequestRequestTypeDef,
     _OptionalDecreaseReplicationFactorRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteClusterRequestRequestTypeDef = TypedDict(
     "DeleteClusterRequestRequestTypeDef",
     {
         "ClusterName": str,
     },
 )
 
@@ -380,22 +374,20 @@
     {
         "Source": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeParametersRequestDescribeParametersPaginateTypeDef(
     _RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef,
     _OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeParametersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeParametersRequestRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 _OptionalDescribeParametersRequestRequestTypeDef = TypedDict(
@@ -404,22 +396,20 @@
         "Source": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeParametersRequestRequestTypeDef(
     _RequiredDescribeParametersRequestRequestTypeDef,
     _OptionalDescribeParametersRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef = TypedDict(
     "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
     {
         "SubnetGroupNames": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -446,63 +436,66 @@
     "_OptionalIncreaseReplicationFactorRequestRequestTypeDef",
     {
         "AvailabilityZones": Sequence[str],
     },
     total=False,
 )
 
-
 class IncreaseReplicationFactorRequestRequestTypeDef(
     _RequiredIncreaseReplicationFactorRequestRequestTypeDef,
     _OptionalIncreaseReplicationFactorRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
     "_RequiredListTagsRequestListTagsPaginateTypeDef",
     {
         "ResourceName": str,
     },
 )
 _OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
     "_OptionalListTagsRequestListTagsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListTagsRequestListTagsPaginateTypeDef(
     _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
 ):
     pass
 
-
 _RequiredListTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsRequestRequestTypeDef",
     {
         "ResourceName": str,
     },
 )
 _OptionalListTagsRequestRequestTypeDef = TypedDict(
     "_OptionalListTagsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
 
 NodeTypeSpecificValueTypeDef = TypedDict(
     "NodeTypeSpecificValueTypeDef",
     {
         "NodeType": str,
         "Value": str,
     },
@@ -579,21 +572,19 @@
         "NotificationTopicStatus": str,
         "ParameterGroupName": str,
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateClusterRequestRequestTypeDef(
     _RequiredUpdateClusterRequestRequestTypeDef, _OptionalUpdateClusterRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateSubnetGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubnetGroupRequestRequestTypeDef",
     {
         "SubnetGroupName": str,
     },
 )
 _OptionalUpdateSubnetGroupRequestRequestTypeDef = TypedDict(
@@ -601,21 +592,19 @@
     {
         "Description": str,
         "SubnetIds": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateSubnetGroupRequestRequestTypeDef(
     _RequiredUpdateSubnetGroupRequestRequestTypeDef, _OptionalUpdateSubnetGroupRequestRequestTypeDef
 ):
     pass
 
-
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "NodeId": str,
         "Endpoint": EndpointTypeDef,
         "NodeCreateTime": datetime,
         "AvailabilityZone": str,
@@ -647,54 +636,27 @@
         "Tags": Sequence[TagTypeDef],
         "SSESpecification": SSESpecificationTypeDef,
         "ClusterEndpointEncryptionType": ClusterEndpointEncryptionTypeType,
     },
     total=False,
 )
 
-
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
-
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceName": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-TagResourceResponseTypeDef = TypedDict(
-    "TagResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UntagResourceResponseTypeDef = TypedDict(
-    "UntagResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateParameterGroupResponseTypeDef = TypedDict(
     "CreateParameterGroupResponseTypeDef",
     {
         "ParameterGroup": ParameterGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -721,14 +683,39 @@
     {
         "NextToken": str,
         "Events": List[EventTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TagResourceResponseTypeDef = TypedDict(
+    "TagResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UntagResourceResponseTypeDef = TypedDict(
+    "UntagResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ParameterTypeDef = TypedDict(
     "ParameterTypeDef",
     {
         "ParameterName": str,
         "ParameterType": ParameterTypeType,
         "ParameterValue": str,
         "NodeTypeSpecificValues": List[NodeTypeSpecificValueTypeDef],
```

### Comparing `mypy-boto3-dax-1.28.0/mypy_boto3_dax/type_defs.pyi` & `mypy-boto3-dax-1.28.12/mypy_boto3_dax/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "EndpointTypeDef",
     "NotificationConfigurationTypeDef",
     "ParameterGroupStatusTypeDef",
     "SSEDescriptionTypeDef",
     "SecurityGroupMembershipTypeDef",
     "SSESpecificationTypeDef",
@@ -58,33 +59,34 @@
     "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     "DescribeParametersRequestRequestTypeDef",
     "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
     "DescribeSubnetGroupsRequestRequestTypeDef",
     "IncreaseReplicationFactorRequestRequestTypeDef",
     "ListTagsRequestListTagsPaginateTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "NodeTypeSpecificValueTypeDef",
     "PaginatorConfigTypeDef",
     "ParameterNameValueTypeDef",
     "RebootNodeRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "SubnetTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateClusterRequestRequestTypeDef",
     "UpdateSubnetGroupRequestRequestTypeDef",
     "NodeTypeDef",
     "CreateClusterRequestRequestTypeDef",
-    "ListTagsResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "TagResourceResponseTypeDef",
-    "UntagResourceResponseTypeDef",
     "CreateParameterGroupResponseTypeDef",
     "DescribeParameterGroupsResponseTypeDef",
     "UpdateParameterGroupResponseTypeDef",
     "DescribeEventsResponseTypeDef",
+    "ListTagsResponseTypeDef",
+    "TagResourceResponseTypeDef",
+    "UntagResourceResponseTypeDef",
     "ParameterTypeDef",
     "UpdateParameterGroupRequestRequestTypeDef",
     "SubnetGroupTypeDef",
     "ClusterTypeDef",
     "DescribeDefaultParametersResponseTypeDef",
     "DescribeParametersResponseTypeDef",
     "CreateSubnetGroupResponseTypeDef",
@@ -171,20 +173,22 @@
     "_OptionalCreateParameterGroupRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class CreateParameterGroupRequestRequestTypeDef(
     _RequiredCreateParameterGroupRequestRequestTypeDef,
     _OptionalCreateParameterGroupRequestRequestTypeDef,
 ):
     pass
 
+
 ParameterGroupTypeDef = TypedDict(
     "ParameterGroupTypeDef",
     {
         "ParameterGroupName": str,
         "Description": str,
     },
     total=False,
@@ -201,19 +205,21 @@
     "_OptionalCreateSubnetGroupRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class CreateSubnetGroupRequestRequestTypeDef(
     _RequiredCreateSubnetGroupRequestRequestTypeDef, _OptionalCreateSubnetGroupRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDecreaseReplicationFactorRequestRequestTypeDef = TypedDict(
     "_RequiredDecreaseReplicationFactorRequestRequestTypeDef",
     {
         "ClusterName": str,
         "NewReplicationFactor": int,
     },
 )
@@ -222,20 +228,22 @@
     {
         "AvailabilityZones": Sequence[str],
         "NodeIdsToRemove": Sequence[str],
     },
     total=False,
 )
 
+
 class DecreaseReplicationFactorRequestRequestTypeDef(
     _RequiredDecreaseReplicationFactorRequestRequestTypeDef,
     _OptionalDecreaseReplicationFactorRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteClusterRequestRequestTypeDef = TypedDict(
     "DeleteClusterRequestRequestTypeDef",
     {
         "ClusterName": str,
     },
 )
 
@@ -373,20 +381,22 @@
     {
         "Source": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeParametersRequestDescribeParametersPaginateTypeDef(
     _RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef,
     _OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeParametersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeParametersRequestRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 _OptionalDescribeParametersRequestRequestTypeDef = TypedDict(
@@ -395,20 +405,22 @@
         "Source": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeParametersRequestRequestTypeDef(
     _RequiredDescribeParametersRequestRequestTypeDef,
     _OptionalDescribeParametersRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef = TypedDict(
     "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
     {
         "SubnetGroupNames": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -435,58 +447,73 @@
     "_OptionalIncreaseReplicationFactorRequestRequestTypeDef",
     {
         "AvailabilityZones": Sequence[str],
     },
     total=False,
 )
 
+
 class IncreaseReplicationFactorRequestRequestTypeDef(
     _RequiredIncreaseReplicationFactorRequestRequestTypeDef,
     _OptionalIncreaseReplicationFactorRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
     "_RequiredListTagsRequestListTagsPaginateTypeDef",
     {
         "ResourceName": str,
     },
 )
 _OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
     "_OptionalListTagsRequestListTagsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListTagsRequestListTagsPaginateTypeDef(
     _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
 ):
     pass
 
+
 _RequiredListTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsRequestRequestTypeDef",
     {
         "ResourceName": str,
     },
 )
 _OptionalListTagsRequestRequestTypeDef = TypedDict(
     "_OptionalListTagsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 NodeTypeSpecificValueTypeDef = TypedDict(
     "NodeTypeSpecificValueTypeDef",
     {
         "NodeType": str,
         "Value": str,
     },
     total=False,
@@ -562,19 +589,21 @@
         "NotificationTopicStatus": str,
         "ParameterGroupName": str,
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateClusterRequestRequestTypeDef(
     _RequiredUpdateClusterRequestRequestTypeDef, _OptionalUpdateClusterRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateSubnetGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubnetGroupRequestRequestTypeDef",
     {
         "SubnetGroupName": str,
     },
 )
 _OptionalUpdateSubnetGroupRequestRequestTypeDef = TypedDict(
@@ -582,19 +611,21 @@
     {
         "Description": str,
         "SubnetIds": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateSubnetGroupRequestRequestTypeDef(
     _RequiredUpdateSubnetGroupRequestRequestTypeDef, _OptionalUpdateSubnetGroupRequestRequestTypeDef
 ):
     pass
 
+
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "NodeId": str,
         "Endpoint": EndpointTypeDef,
         "NodeCreateTime": datetime,
         "AvailabilityZone": str,
@@ -626,52 +657,29 @@
         "Tags": Sequence[TagTypeDef],
         "SSESpecification": SSESpecificationTypeDef,
         "ClusterEndpointEncryptionType": ClusterEndpointEncryptionTypeType,
     },
     total=False,
 )
 
+
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceName": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-TagResourceResponseTypeDef = TypedDict(
-    "TagResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UntagResourceResponseTypeDef = TypedDict(
-    "UntagResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateParameterGroupResponseTypeDef = TypedDict(
     "CreateParameterGroupResponseTypeDef",
     {
         "ParameterGroup": ParameterGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -698,14 +706,39 @@
     {
         "NextToken": str,
         "Events": List[EventTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TagResourceResponseTypeDef = TypedDict(
+    "TagResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UntagResourceResponseTypeDef = TypedDict(
+    "UntagResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ParameterTypeDef = TypedDict(
     "ParameterTypeDef",
     {
         "ParameterName": str,
         "ParameterType": ParameterTypeType,
         "ParameterValue": str,
         "NodeTypeSpecificValues": List[NodeTypeSpecificValueTypeDef],
```

### Comparing `mypy-boto3-dax-1.28.0/mypy_boto3_dax.egg-info/PKG-INFO` & `mypy-boto3-dax-1.28.12/mypy_boto3_dax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dax
-Version: 1.28.0
-Summary: Type annotations for boto3.DAX 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.DAX 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-dax"></a>
 
 # mypy-boto3-dax
 
 [![PyPI - mypy-boto3-dax](https://img.shields.io/pypi/v/mypy-boto3-dax.svg?color=blue)](https://pypi.org/project/mypy-boto3-dax)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dax.svg?color=blue)](https://pypi.org/project/mypy-boto3-dax)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dax?color=blue)](https://pypistats.org/packages/mypy-boto3-dax)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dax)](https://pepy.tech/project/mypy-boto3-dax)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DAX 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
+[boto3.DAX 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
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
 [mypy-boto3-dax docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/).
 
 See how it helps to find and fix potential bugs:
 
@@ -383,33 +383,34 @@
     DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeParametersRequestRequestTypeDef,
     DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeSubnetGroupsRequestRequestTypeDef,
     IncreaseReplicationFactorRequestRequestTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     NodeTypeSpecificValueTypeDef,
     PaginatorConfigTypeDef,
     ParameterNameValueTypeDef,
     RebootNodeRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     SubnetTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
     UpdateSubnetGroupRequestRequestTypeDef,
     NodeTypeDef,
     CreateClusterRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    TagResourceResponseTypeDef,
-    UntagResourceResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
     DescribeEventsResponseTypeDef,
+    ListTagsResponseTypeDef,
+    TagResourceResponseTypeDef,
+    UntagResourceResponseTypeDef,
     ParameterTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
     SubnetGroupTypeDef,
     ClusterTypeDef,
     DescribeDefaultParametersResponseTypeDef,
     DescribeParametersResponseTypeDef,
     CreateSubnetGroupResponseTypeDef,
```

### Comparing `mypy-boto3-dax-1.28.0/mypy_boto3_dax.egg-info/SOURCES.txt` & `mypy-boto3-dax-1.28.12/mypy_boto3_dax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.0/setup.py` & `mypy-boto3-dax-1.28.12/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dax",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_dax"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DAX 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.DAX 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

