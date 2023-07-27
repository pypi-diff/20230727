# Comparing `tmp/mypy-boto3-mediastore-1.28.0.tar.gz` & `tmp/mypy-boto3-mediastore-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediastore-1.28.0.tar", last modified: Thu Jul  6 21:00:08 2023, max compression
+gzip compressed data, was "mypy-boto3-mediastore-1.28.12.tar", last modified: Thu Jul 27 05:35:02 2023, max compression
```

## Comparing `mypy-boto3-mediastore-1.28.0.tar` & `mypy-boto3-mediastore-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:08.022371 mypy-boto3-mediastore-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:47:22.000000 mypy-boto3-mediastore-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-07-06 21:00:08.006371 mypy-boto3-mediastore-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12583 2023-07-06 20:47:22.000000 mypy-boto3-mediastore-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:08.006371 mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-06 20:47:22.000000 mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-06 20:47:22.000000 mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 20:47:22.000000 mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14585 2023-07-06 20:47:22.000000 mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-07-06 20:47:22.000000 mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-07-06 20:47:22.000000 mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-07-06 20:47:22.000000 mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-06 20:47:22.000000 mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-06 20:47:22.000000 mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:47:22.000000 mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-06 20:47:23.000000 mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-07-06 20:47:23.000000 mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:47:22.000000 mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:08.006371 mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-07-06 21:00:07.000000 mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-06 21:00:07.000000 mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:07.000000 mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:07.000000 mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:07.000000 mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 21:00:07.000000 mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:08.022371 mypy-boto3-mediastore-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:47:22.000000 mypy-boto3-mediastore-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.036437 mypy-boto3-mediastore-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14182 2023-07-27 05:35:02.032437 mypy-boto3-mediastore-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.028437 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14585 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.032437 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14182 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:02.036437 mypy-boto3-mediastore-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/setup.py
```

### Comparing `mypy-boto3-mediastore-1.28.0/LICENSE` & `mypy-boto3-mediastore-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.0/PKG-INFO` & `mypy-boto3-mediastore-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediastore
-Version: 1.28.0
-Summary: Type annotations for boto3.MediaStore 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MediaStore 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mediastore"></a>
 
 # mypy-boto3-mediastore
 
 [![PyPI - mypy-boto3-mediastore](https://img.shields.io/pypi/v/mypy-boto3-mediastore.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediastore.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediastore?color=blue)](https://pypistats.org/packages/mypy-boto3-mediastore)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediastore)](https://pepy.tech/project/mypy-boto3-mediastore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaStore 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
+[boto3.MediaStore 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
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
 [mypy-boto3-mediastore docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,14 +322,15 @@
 
 `mypy_boto3_mediastore.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediastore.type_defs import (
     ContainerTypeDef,
+    CorsRuleOutputTypeDef,
     CorsRuleTypeDef,
     TagTypeDef,
     DeleteContainerInputRequestTypeDef,
     DeleteContainerPolicyInputRequestTypeDef,
     DeleteCorsPolicyInputRequestTypeDef,
     DeleteLifecyclePolicyInputRequestTypeDef,
     DeleteMetricPolicyInputRequestTypeDef,
@@ -339,30 +340,33 @@
     GetCorsPolicyInputRequestTypeDef,
     GetLifecyclePolicyInputRequestTypeDef,
     GetLifecyclePolicyOutputTypeDef,
     GetMetricPolicyInputRequestTypeDef,
     ListContainersInputListContainersPaginateTypeDef,
     ListContainersInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    TagOutputTypeDef,
+    MetricPolicyRuleOutputTypeDef,
     MetricPolicyRuleTypeDef,
     PaginatorConfigTypeDef,
     PutContainerPolicyInputRequestTypeDef,
     PutLifecyclePolicyInputRequestTypeDef,
     ResponseMetadataTypeDef,
     StartAccessLoggingInputRequestTypeDef,
     StopAccessLoggingInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     CreateContainerOutputTypeDef,
     DescribeContainerOutputTypeDef,
     ListContainersOutputTypeDef,
     GetCorsPolicyOutputTypeDef,
     PutCorsPolicyInputRequestTypeDef,
     CreateContainerInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    MetricPolicyOutputTypeDef,
     MetricPolicyTypeDef,
     GetMetricPolicyOutputTypeDef,
     PutMetricPolicyInputRequestTypeDef,
 )
 
 
 def get_structure() -> ContainerTypeDef:
```

### Comparing `mypy-boto3-mediastore-1.28.0/README.md` & `mypy-boto3-mediastore-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-mediastore"></a>
 
 # mypy-boto3-mediastore
 
 [![PyPI - mypy-boto3-mediastore](https://img.shields.io/pypi/v/mypy-boto3-mediastore.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediastore.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediastore?color=blue)](https://pypistats.org/packages/mypy-boto3-mediastore)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediastore)](https://pepy.tech/project/mypy-boto3-mediastore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaStore 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
+[boto3.MediaStore 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
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
 [mypy-boto3-mediastore docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,14 +290,15 @@
 
 `mypy_boto3_mediastore.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediastore.type_defs import (
     ContainerTypeDef,
+    CorsRuleOutputTypeDef,
     CorsRuleTypeDef,
     TagTypeDef,
     DeleteContainerInputRequestTypeDef,
     DeleteContainerPolicyInputRequestTypeDef,
     DeleteCorsPolicyInputRequestTypeDef,
     DeleteLifecyclePolicyInputRequestTypeDef,
     DeleteMetricPolicyInputRequestTypeDef,
@@ -307,30 +308,33 @@
     GetCorsPolicyInputRequestTypeDef,
     GetLifecyclePolicyInputRequestTypeDef,
     GetLifecyclePolicyOutputTypeDef,
     GetMetricPolicyInputRequestTypeDef,
     ListContainersInputListContainersPaginateTypeDef,
     ListContainersInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    TagOutputTypeDef,
+    MetricPolicyRuleOutputTypeDef,
     MetricPolicyRuleTypeDef,
     PaginatorConfigTypeDef,
     PutContainerPolicyInputRequestTypeDef,
     PutLifecyclePolicyInputRequestTypeDef,
     ResponseMetadataTypeDef,
     StartAccessLoggingInputRequestTypeDef,
     StopAccessLoggingInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     CreateContainerOutputTypeDef,
     DescribeContainerOutputTypeDef,
     ListContainersOutputTypeDef,
     GetCorsPolicyOutputTypeDef,
     PutCorsPolicyInputRequestTypeDef,
     CreateContainerInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    MetricPolicyOutputTypeDef,
     MetricPolicyTypeDef,
     GetMetricPolicyOutputTypeDef,
     PutMetricPolicyInputRequestTypeDef,
 )
 
 
 def get_structure() -> ContainerTypeDef:
```

### Comparing `mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/__init__.py` & `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/__init__.pyi` & `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/__main__.py` & `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaStore 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.MediaStore 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore\nOther"
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

### Comparing `mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/client.py` & `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/client.pyi` & `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/literals.py` & `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,28 +14,26 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ContainerLevelMetricsType",
     "ContainerStatusType",
     "ListContainersPaginatorName",
     "MethodNameType",
     "MediaStoreServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ContainerLevelMetricsType = Literal["DISABLED", "ENABLED"]
 ContainerStatusType = Literal["ACTIVE", "CREATING", "DELETING"]
 ListContainersPaginatorName = Literal["list_containers"]
 MethodNameType = Literal["DELETE", "GET", "HEAD", "PUT"]
 MediaStoreServiceName = Literal["mediastore"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -152,14 +150,15 @@
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
@@ -238,26 +237,28 @@
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

### Comparing `mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/literals.pyi` & `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,28 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ContainerLevelMetricsType",
     "ContainerStatusType",
     "ListContainersPaginatorName",
     "MethodNameType",
     "MediaStoreServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ContainerLevelMetricsType = Literal["DISABLED", "ENABLED"]
 ContainerStatusType = Literal["ACTIVE", "CREATING", "DELETING"]
 ListContainersPaginatorName = Literal["list_containers"]
 MethodNameType = Literal["DELETE", "GET", "HEAD", "PUT"]
 MediaStoreServiceName = Literal["mediastore"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -150,14 +152,15 @@
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
@@ -236,26 +239,28 @@
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

### Comparing `mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/paginator.py` & `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/paginator.pyi` & `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/type_defs.py` & `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 from .literals import ContainerLevelMetricsType, ContainerStatusType, MethodNameType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ContainerTypeDef",
+    "CorsRuleOutputTypeDef",
     "CorsRuleTypeDef",
     "TagTypeDef",
     "DeleteContainerInputRequestTypeDef",
     "DeleteContainerPolicyInputRequestTypeDef",
     "DeleteCorsPolicyInputRequestTypeDef",
     "DeleteLifecyclePolicyInputRequestTypeDef",
     "DeleteMetricPolicyInputRequestTypeDef",
@@ -38,30 +38,33 @@
     "GetCorsPolicyInputRequestTypeDef",
     "GetLifecyclePolicyInputRequestTypeDef",
     "GetLifecyclePolicyOutputTypeDef",
     "GetMetricPolicyInputRequestTypeDef",
     "ListContainersInputListContainersPaginateTypeDef",
     "ListContainersInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "TagOutputTypeDef",
+    "MetricPolicyRuleOutputTypeDef",
     "MetricPolicyRuleTypeDef",
     "PaginatorConfigTypeDef",
     "PutContainerPolicyInputRequestTypeDef",
     "PutLifecyclePolicyInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "StartAccessLoggingInputRequestTypeDef",
     "StopAccessLoggingInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "CreateContainerOutputTypeDef",
     "DescribeContainerOutputTypeDef",
     "ListContainersOutputTypeDef",
     "GetCorsPolicyOutputTypeDef",
     "PutCorsPolicyInputRequestTypeDef",
     "CreateContainerInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "MetricPolicyOutputTypeDef",
     "MetricPolicyTypeDef",
     "GetMetricPolicyOutputTypeDef",
     "PutMetricPolicyInputRequestTypeDef",
 )
 
 ContainerTypeDef = TypedDict(
     "ContainerTypeDef",
@@ -72,55 +75,71 @@
         "Name": str,
         "Status": ContainerStatusType,
         "AccessLoggingEnabled": bool,
     },
     total=False,
 )
 
-_RequiredCorsRuleTypeDef = TypedDict(
-    "_RequiredCorsRuleTypeDef",
+_RequiredCorsRuleOutputTypeDef = TypedDict(
+    "_RequiredCorsRuleOutputTypeDef",
     {
         "AllowedOrigins": List[str],
         "AllowedHeaders": List[str],
     },
 )
-_OptionalCorsRuleTypeDef = TypedDict(
-    "_OptionalCorsRuleTypeDef",
+_OptionalCorsRuleOutputTypeDef = TypedDict(
+    "_OptionalCorsRuleOutputTypeDef",
     {
         "AllowedMethods": List[MethodNameType],
         "MaxAgeSeconds": int,
         "ExposeHeaders": List[str],
     },
     total=False,
 )
 
+class CorsRuleOutputTypeDef(_RequiredCorsRuleOutputTypeDef, _OptionalCorsRuleOutputTypeDef):
+    pass
+
+_RequiredCorsRuleTypeDef = TypedDict(
+    "_RequiredCorsRuleTypeDef",
+    {
+        "AllowedOrigins": Sequence[str],
+        "AllowedHeaders": Sequence[str],
+    },
+)
+_OptionalCorsRuleTypeDef = TypedDict(
+    "_OptionalCorsRuleTypeDef",
+    {
+        "AllowedMethods": Sequence[MethodNameType],
+        "MaxAgeSeconds": int,
+        "ExposeHeaders": Sequence[str],
+    },
+    total=False,
+)
 
 class CorsRuleTypeDef(_RequiredCorsRuleTypeDef, _OptionalCorsRuleTypeDef):
     pass
 
-
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-
 DeleteContainerInputRequestTypeDef = TypedDict(
     "DeleteContainerInputRequestTypeDef",
     {
         "ContainerName": str,
     },
 )
 
@@ -224,14 +243,39 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "Resource": str,
     },
 )
 
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
+    pass
+
+MetricPolicyRuleOutputTypeDef = TypedDict(
+    "MetricPolicyRuleOutputTypeDef",
+    {
+        "ObjectGroup": str,
+        "ObjectGroupName": str,
+    },
+)
+
 MetricPolicyRuleTypeDef = TypedDict(
     "MetricPolicyRuleTypeDef",
     {
         "ObjectGroup": str,
         "ObjectGroupName": str,
     },
 )
@@ -319,15 +363,15 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCorsPolicyOutputTypeDef = TypedDict(
     "GetCorsPolicyOutputTypeDef",
     {
-        "CorsPolicy": List[CorsRuleTypeDef],
+        "CorsPolicy": List[CorsRuleOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutCorsPolicyInputRequestTypeDef = TypedDict(
     "PutCorsPolicyInputRequestTypeDef",
     {
@@ -346,60 +390,75 @@
     "_OptionalCreateContainerInputRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateContainerInputRequestTypeDef(
     _RequiredCreateContainerInputRequestTypeDef, _OptionalCreateContainerInputRequestTypeDef
 ):
     pass
 
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
+    {
+        "Resource": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
+_RequiredMetricPolicyOutputTypeDef = TypedDict(
+    "_RequiredMetricPolicyOutputTypeDef",
     {
-        "Resource": str,
-        "Tags": Sequence[TagTypeDef],
+        "ContainerLevelMetrics": ContainerLevelMetricsType,
+    },
+)
+_OptionalMetricPolicyOutputTypeDef = TypedDict(
+    "_OptionalMetricPolicyOutputTypeDef",
+    {
+        "MetricPolicyRules": List[MetricPolicyRuleOutputTypeDef],
     },
+    total=False,
 )
 
+class MetricPolicyOutputTypeDef(
+    _RequiredMetricPolicyOutputTypeDef, _OptionalMetricPolicyOutputTypeDef
+):
+    pass
+
 _RequiredMetricPolicyTypeDef = TypedDict(
     "_RequiredMetricPolicyTypeDef",
     {
         "ContainerLevelMetrics": ContainerLevelMetricsType,
     },
 )
 _OptionalMetricPolicyTypeDef = TypedDict(
     "_OptionalMetricPolicyTypeDef",
     {
-        "MetricPolicyRules": List[MetricPolicyRuleTypeDef],
+        "MetricPolicyRules": Sequence[MetricPolicyRuleTypeDef],
     },
     total=False,
 )
 
-
 class MetricPolicyTypeDef(_RequiredMetricPolicyTypeDef, _OptionalMetricPolicyTypeDef):
     pass
 
-
 GetMetricPolicyOutputTypeDef = TypedDict(
     "GetMetricPolicyOutputTypeDef",
     {
-        "MetricPolicy": MetricPolicyTypeDef,
+        "MetricPolicy": MetricPolicyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutMetricPolicyInputRequestTypeDef = TypedDict(
     "PutMetricPolicyInputRequestTypeDef",
     {
```

### Comparing `mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore/type_defs.pyi` & `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/type_defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,16 +18,18 @@
 from .literals import ContainerLevelMetricsType, ContainerStatusType, MethodNameType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ContainerTypeDef",
+    "CorsRuleOutputTypeDef",
     "CorsRuleTypeDef",
     "TagTypeDef",
     "DeleteContainerInputRequestTypeDef",
     "DeleteContainerPolicyInputRequestTypeDef",
     "DeleteCorsPolicyInputRequestTypeDef",
     "DeleteLifecyclePolicyInputRequestTypeDef",
     "DeleteMetricPolicyInputRequestTypeDef",
@@ -37,30 +39,33 @@
     "GetCorsPolicyInputRequestTypeDef",
     "GetLifecyclePolicyInputRequestTypeDef",
     "GetLifecyclePolicyOutputTypeDef",
     "GetMetricPolicyInputRequestTypeDef",
     "ListContainersInputListContainersPaginateTypeDef",
     "ListContainersInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "TagOutputTypeDef",
+    "MetricPolicyRuleOutputTypeDef",
     "MetricPolicyRuleTypeDef",
     "PaginatorConfigTypeDef",
     "PutContainerPolicyInputRequestTypeDef",
     "PutLifecyclePolicyInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "StartAccessLoggingInputRequestTypeDef",
     "StopAccessLoggingInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "CreateContainerOutputTypeDef",
     "DescribeContainerOutputTypeDef",
     "ListContainersOutputTypeDef",
     "GetCorsPolicyOutputTypeDef",
     "PutCorsPolicyInputRequestTypeDef",
     "CreateContainerInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "MetricPolicyOutputTypeDef",
     "MetricPolicyTypeDef",
     "GetMetricPolicyOutputTypeDef",
     "PutMetricPolicyInputRequestTypeDef",
 )
 
 ContainerTypeDef = TypedDict(
     "ContainerTypeDef",
@@ -71,51 +76,77 @@
         "Name": str,
         "Status": ContainerStatusType,
         "AccessLoggingEnabled": bool,
     },
     total=False,
 )
 
-_RequiredCorsRuleTypeDef = TypedDict(
-    "_RequiredCorsRuleTypeDef",
+_RequiredCorsRuleOutputTypeDef = TypedDict(
+    "_RequiredCorsRuleOutputTypeDef",
     {
         "AllowedOrigins": List[str],
         "AllowedHeaders": List[str],
     },
 )
-_OptionalCorsRuleTypeDef = TypedDict(
-    "_OptionalCorsRuleTypeDef",
+_OptionalCorsRuleOutputTypeDef = TypedDict(
+    "_OptionalCorsRuleOutputTypeDef",
     {
         "AllowedMethods": List[MethodNameType],
         "MaxAgeSeconds": int,
         "ExposeHeaders": List[str],
     },
     total=False,
 )
 
+
+class CorsRuleOutputTypeDef(_RequiredCorsRuleOutputTypeDef, _OptionalCorsRuleOutputTypeDef):
+    pass
+
+
+_RequiredCorsRuleTypeDef = TypedDict(
+    "_RequiredCorsRuleTypeDef",
+    {
+        "AllowedOrigins": Sequence[str],
+        "AllowedHeaders": Sequence[str],
+    },
+)
+_OptionalCorsRuleTypeDef = TypedDict(
+    "_OptionalCorsRuleTypeDef",
+    {
+        "AllowedMethods": Sequence[MethodNameType],
+        "MaxAgeSeconds": int,
+        "ExposeHeaders": Sequence[str],
+    },
+    total=False,
+)
+
+
 class CorsRuleTypeDef(_RequiredCorsRuleTypeDef, _OptionalCorsRuleTypeDef):
     pass
 
+
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+
 DeleteContainerInputRequestTypeDef = TypedDict(
     "DeleteContainerInputRequestTypeDef",
     {
         "ContainerName": str,
     },
 )
 
@@ -219,14 +250,41 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "Resource": str,
     },
 )
 
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
+    pass
+
+
+MetricPolicyRuleOutputTypeDef = TypedDict(
+    "MetricPolicyRuleOutputTypeDef",
+    {
+        "ObjectGroup": str,
+        "ObjectGroupName": str,
+    },
+)
+
 MetricPolicyRuleTypeDef = TypedDict(
     "MetricPolicyRuleTypeDef",
     {
         "ObjectGroup": str,
         "ObjectGroupName": str,
     },
 )
@@ -314,15 +372,15 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCorsPolicyOutputTypeDef = TypedDict(
     "GetCorsPolicyOutputTypeDef",
     {
-        "CorsPolicy": List[CorsRuleTypeDef],
+        "CorsPolicy": List[CorsRuleOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutCorsPolicyInputRequestTypeDef = TypedDict(
     "PutCorsPolicyInputRequestTypeDef",
     {
@@ -341,56 +399,81 @@
     "_OptionalCreateContainerInputRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateContainerInputRequestTypeDef(
     _RequiredCreateContainerInputRequestTypeDef, _OptionalCreateContainerInputRequestTypeDef
 ):
     pass
 
+
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
+    {
+        "Resource": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
+_RequiredMetricPolicyOutputTypeDef = TypedDict(
+    "_RequiredMetricPolicyOutputTypeDef",
     {
-        "Resource": str,
-        "Tags": Sequence[TagTypeDef],
+        "ContainerLevelMetrics": ContainerLevelMetricsType,
+    },
+)
+_OptionalMetricPolicyOutputTypeDef = TypedDict(
+    "_OptionalMetricPolicyOutputTypeDef",
+    {
+        "MetricPolicyRules": List[MetricPolicyRuleOutputTypeDef],
     },
+    total=False,
 )
 
+
+class MetricPolicyOutputTypeDef(
+    _RequiredMetricPolicyOutputTypeDef, _OptionalMetricPolicyOutputTypeDef
+):
+    pass
+
+
 _RequiredMetricPolicyTypeDef = TypedDict(
     "_RequiredMetricPolicyTypeDef",
     {
         "ContainerLevelMetrics": ContainerLevelMetricsType,
     },
 )
 _OptionalMetricPolicyTypeDef = TypedDict(
     "_OptionalMetricPolicyTypeDef",
     {
-        "MetricPolicyRules": List[MetricPolicyRuleTypeDef],
+        "MetricPolicyRules": Sequence[MetricPolicyRuleTypeDef],
     },
     total=False,
 )
 
+
 class MetricPolicyTypeDef(_RequiredMetricPolicyTypeDef, _OptionalMetricPolicyTypeDef):
     pass
 
+
 GetMetricPolicyOutputTypeDef = TypedDict(
     "GetMetricPolicyOutputTypeDef",
     {
-        "MetricPolicy": MetricPolicyTypeDef,
+        "MetricPolicy": MetricPolicyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutMetricPolicyInputRequestTypeDef = TypedDict(
     "PutMetricPolicyInputRequestTypeDef",
     {
```

### Comparing `mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore.egg-info/PKG-INFO` & `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediastore
-Version: 1.28.0
-Summary: Type annotations for boto3.MediaStore 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MediaStore 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mediastore"></a>
 
 # mypy-boto3-mediastore
 
 [![PyPI - mypy-boto3-mediastore](https://img.shields.io/pypi/v/mypy-boto3-mediastore.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediastore.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediastore?color=blue)](https://pypistats.org/packages/mypy-boto3-mediastore)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediastore)](https://pepy.tech/project/mypy-boto3-mediastore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaStore 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
+[boto3.MediaStore 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
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
 [mypy-boto3-mediastore docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,14 +322,15 @@
 
 `mypy_boto3_mediastore.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediastore.type_defs import (
     ContainerTypeDef,
+    CorsRuleOutputTypeDef,
     CorsRuleTypeDef,
     TagTypeDef,
     DeleteContainerInputRequestTypeDef,
     DeleteContainerPolicyInputRequestTypeDef,
     DeleteCorsPolicyInputRequestTypeDef,
     DeleteLifecyclePolicyInputRequestTypeDef,
     DeleteMetricPolicyInputRequestTypeDef,
@@ -339,30 +340,33 @@
     GetCorsPolicyInputRequestTypeDef,
     GetLifecyclePolicyInputRequestTypeDef,
     GetLifecyclePolicyOutputTypeDef,
     GetMetricPolicyInputRequestTypeDef,
     ListContainersInputListContainersPaginateTypeDef,
     ListContainersInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    TagOutputTypeDef,
+    MetricPolicyRuleOutputTypeDef,
     MetricPolicyRuleTypeDef,
     PaginatorConfigTypeDef,
     PutContainerPolicyInputRequestTypeDef,
     PutLifecyclePolicyInputRequestTypeDef,
     ResponseMetadataTypeDef,
     StartAccessLoggingInputRequestTypeDef,
     StopAccessLoggingInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     CreateContainerOutputTypeDef,
     DescribeContainerOutputTypeDef,
     ListContainersOutputTypeDef,
     GetCorsPolicyOutputTypeDef,
     PutCorsPolicyInputRequestTypeDef,
     CreateContainerInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    MetricPolicyOutputTypeDef,
     MetricPolicyTypeDef,
     GetMetricPolicyOutputTypeDef,
     PutMetricPolicyInputRequestTypeDef,
 )
 
 
 def get_structure() -> ContainerTypeDef:
```

### Comparing `mypy-boto3-mediastore-1.28.0/mypy_boto3_mediastore.egg-info/SOURCES.txt` & `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.0/setup.py` & `mypy-boto3-mediastore-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediastore",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_mediastore"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaStore 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.MediaStore 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

