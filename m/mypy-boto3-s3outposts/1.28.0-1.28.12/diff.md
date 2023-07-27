# Comparing `tmp/mypy-boto3-s3outposts-1.28.0.tar.gz` & `tmp/mypy-boto3-s3outposts-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-s3outposts-1.28.0.tar", last modified: Thu Jul  6 21:00:31 2023, max compression
+gzip compressed data, was "mypy-boto3-s3outposts-1.28.12.tar", last modified: Thu Jul 27 11:49:33 2023, max compression
```

## Comparing `mypy-boto3-s3outposts-1.28.0.tar` & `mypy-boto3-s3outposts-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:31.766419 mypy-boto3-s3outposts-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13799 2023-07-06 21:00:31.766419 mypy-boto3-s3outposts-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12302 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:31.766419 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:31.766419 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13799 2023-07-06 21:00:31.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-06 21:00:31.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:31.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:31.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:31.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 21:00:31.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:31.766419 mypy-boto3-s3outposts-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.257241 mypy-boto3-s3outposts-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:45:20.000000 mypy-boto3-s3outposts-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-07-27 11:49:33.249241 mypy-boto3-s3outposts-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12287 2023-07-27 11:45:20.000000 mypy-boto3-s3outposts-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.249241 mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-27 11:45:20.000000 mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-27 11:45:20.000000 mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 11:45:20.000000 mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-07-27 11:45:20.000000 mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-27 11:45:20.000000 mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-07-27 11:45:20.000000 mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-27 11:45:20.000000 mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-27 11:45:20.000000 mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-27 11:45:20.000000 mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:20.000000 mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-07-27 11:45:20.000000 mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-27 11:45:20.000000 mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:45:20.000000 mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.249241 mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-07-27 11:49:33.000000 mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 11:49:33.000000 mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:33.000000 mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:33.000000 mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:33.000000 mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 11:49:33.000000 mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:33.257241 mypy-boto3-s3outposts-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 11:45:19.000000 mypy-boto3-s3outposts-1.28.12/setup.py
```

### Comparing `mypy-boto3-s3outposts-1.28.0/LICENSE` & `mypy-boto3-s3outposts-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.28.0/PKG-INFO` & `mypy-boto3-s3outposts-1.28.12/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-s3outposts
-Version: 1.28.0
-Summary: Type annotations for boto3.S3Outposts 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 s3outposts type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-s3outposts"></a>
 
 # mypy-boto3-s3outposts
 
 [![PyPI - mypy-boto3-s3outposts](https://img.shields.io/pypi/v/mypy-boto3-s3outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3outposts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3outposts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3outposts?color=blue)](https://pypistats.org/packages/mypy-boto3-s3outposts)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-s3outposts)](https://pepy.tech/project/mypy-boto3-s3outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Outposts 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
+[boto3.S3Outposts 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
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
 [mypy-boto3-s3outposts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,29 +301,29 @@
 
 `mypy_boto3_s3outposts.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3outposts.type_defs import (
     CreateEndpointRequestRequestTypeDef,
-    CreateEndpointResultTypeDef,
+    ResponseMetadataTypeDef,
     DeleteEndpointRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     FailedReasonTypeDef,
     NetworkInterfaceTypeDef,
-    ListEndpointsRequestListEndpointsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEndpointsRequestRequestTypeDef,
-    ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef,
     ListOutpostsWithS3RequestRequestTypeDef,
     OutpostTypeDef,
-    ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
     ListSharedEndpointsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    CreateEndpointResultTypeDef,
+    EmptyResponseMetadataTypeDef,
     EndpointTypeDef,
+    ListEndpointsRequestListEndpointsPaginateTypeDef,
+    ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef,
+    ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
     ListOutpostsWithS3ResultTypeDef,
     ListEndpointsResultTypeDef,
     ListSharedEndpointsResultTypeDef,
 )
 
 
 def get_structure() -> CreateEndpointRequestRequestTypeDef:
```

### Comparing `mypy-boto3-s3outposts-1.28.0/README.md` & `mypy-boto3-s3outposts-1.28.12/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-s3outposts
+Version: 1.28.12
+Summary: Type annotations for boto3.S3Outposts 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 s3outposts type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-s3outposts"></a>
 
 # mypy-boto3-s3outposts
 
 [![PyPI - mypy-boto3-s3outposts](https://img.shields.io/pypi/v/mypy-boto3-s3outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3outposts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3outposts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3outposts?color=blue)](https://pypistats.org/packages/mypy-boto3-s3outposts)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-s3outposts)](https://pepy.tech/project/mypy-boto3-s3outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Outposts 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
+[boto3.S3Outposts 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
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
 [mypy-boto3-s3outposts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,29 +333,29 @@
 
 `mypy_boto3_s3outposts.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3outposts.type_defs import (
     CreateEndpointRequestRequestTypeDef,
-    CreateEndpointResultTypeDef,
+    ResponseMetadataTypeDef,
     DeleteEndpointRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     FailedReasonTypeDef,
     NetworkInterfaceTypeDef,
-    ListEndpointsRequestListEndpointsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEndpointsRequestRequestTypeDef,
-    ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef,
     ListOutpostsWithS3RequestRequestTypeDef,
     OutpostTypeDef,
-    ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
     ListSharedEndpointsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    CreateEndpointResultTypeDef,
+    EmptyResponseMetadataTypeDef,
     EndpointTypeDef,
+    ListEndpointsRequestListEndpointsPaginateTypeDef,
+    ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef,
+    ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
     ListOutpostsWithS3ResultTypeDef,
     ListEndpointsResultTypeDef,
     ListSharedEndpointsResultTypeDef,
 )
 
 
 def get_structure() -> CreateEndpointRequestRequestTypeDef:
```

### Comparing `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/__init__.py` & `mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/__init__.pyi` & `mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/__main__.py` & `mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.S3Outposts 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.S3Outposts 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts\nOther"
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

### Comparing `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/client.py` & `mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/client.pyi` & `mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/literals.py` & `mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,29 +14,27 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "EndpointAccessTypeType",
     "EndpointStatusType",
     "ListEndpointsPaginatorName",
     "ListOutpostsWithS3PaginatorName",
     "ListSharedEndpointsPaginatorName",
     "S3OutpostsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 EndpointAccessTypeType = Literal["CustomerOwnedIp", "Private"]
 EndpointStatusType = Literal["Available", "Create_Failed", "Delete_Failed", "Deleting", "Pending"]
 ListEndpointsPaginatorName = Literal["list_endpoints"]
 ListOutpostsWithS3PaginatorName = Literal["list_outposts_with_s3"]
 ListSharedEndpointsPaginatorName = Literal["list_shared_endpoints"]
 S3OutpostsServiceName = Literal["s3outposts"]
 ServiceName = Literal[
@@ -154,14 +152,15 @@
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
@@ -240,26 +239,28 @@
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

### Comparing `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/literals.pyi` & `mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,29 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "EndpointAccessTypeType",
     "EndpointStatusType",
     "ListEndpointsPaginatorName",
     "ListOutpostsWithS3PaginatorName",
     "ListSharedEndpointsPaginatorName",
     "S3OutpostsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 EndpointAccessTypeType = Literal["CustomerOwnedIp", "Private"]
 EndpointStatusType = Literal["Available", "Create_Failed", "Delete_Failed", "Deleting", "Pending"]
 ListEndpointsPaginatorName = Literal["list_endpoints"]
 ListOutpostsWithS3PaginatorName = Literal["list_outposts_with_s3"]
 ListSharedEndpointsPaginatorName = Literal["list_shared_endpoints"]
 S3OutpostsServiceName = Literal["s3outposts"]
 ServiceName = Literal[
@@ -152,14 +154,15 @@
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
@@ -238,26 +241,28 @@
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

### Comparing `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/paginator.py` & `mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,43 +50,43 @@
 class ListEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listendpointspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEndpointsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listendpointspaginator)
         """
 
 
 class ListOutpostsWithS3Paginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListOutpostsWithS3)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listoutpostswiths3paginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOutpostsWithS3ResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListOutpostsWithS3.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listoutpostswiths3paginator)
         """
 
 
 class ListSharedEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListSharedEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listsharedendpointspaginator)
     """
 
     def paginate(
-        self, *, OutpostId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OutpostId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSharedEndpointsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListSharedEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listsharedendpointspaginator)
         """
```

### Comparing `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/paginator.pyi` & `mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -47,41 +47,41 @@
 class ListEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listendpointspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEndpointsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listendpointspaginator)
         """
 
 class ListOutpostsWithS3Paginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListOutpostsWithS3)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listoutpostswiths3paginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOutpostsWithS3ResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListOutpostsWithS3.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listoutpostswiths3paginator)
         """
 
 class ListSharedEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListSharedEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listsharedendpointspaginator)
     """
 
     def paginate(
-        self, *, OutpostId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OutpostId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSharedEndpointsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListSharedEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/paginators/#listsharedendpointspaginator)
         """
```

### Comparing `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/type_defs.py` & `mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,29 +21,29 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CreateEndpointRequestRequestTypeDef",
-    "CreateEndpointResultTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteEndpointRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "FailedReasonTypeDef",
     "NetworkInterfaceTypeDef",
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEndpointsRequestRequestTypeDef",
-    "ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef",
     "ListOutpostsWithS3RequestRequestTypeDef",
     "OutpostTypeDef",
-    "ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
     "ListSharedEndpointsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateEndpointResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EndpointTypeDef",
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+    "ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef",
+    "ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
     "ListOutpostsWithS3ResultTypeDef",
     "ListEndpointsResultTypeDef",
     "ListSharedEndpointsResultTypeDef",
 )
 
 _RequiredCreateEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointRequestRequestTypeDef",
@@ -65,37 +65,33 @@
 
 class CreateEndpointRequestRequestTypeDef(
     _RequiredCreateEndpointRequestRequestTypeDef, _OptionalCreateEndpointRequestRequestTypeDef
 ):
     pass
 
 
-CreateEndpointResultTypeDef = TypedDict(
-    "CreateEndpointResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "EndpointArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteEndpointRequestRequestTypeDef = TypedDict(
     "DeleteEndpointRequestRequestTypeDef",
     {
         "EndpointId": str,
         "OutpostId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FailedReasonTypeDef = TypedDict(
     "FailedReasonTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
@@ -105,39 +101,33 @@
     "NetworkInterfaceTypeDef",
     {
         "NetworkInterfaceId": str,
     },
     total=False,
 )
 
-ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListEndpointsRequestRequestTypeDef = TypedDict(
     "ListEndpointsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef = TypedDict(
-    "ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOutpostsWithS3RequestRequestTypeDef = TypedDict(
     "ListOutpostsWithS3RequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -150,36 +140,14 @@
         "OutpostId": str,
         "OwnerId": str,
         "CapacityInBytes": int,
     },
     total=False,
 )
 
-_RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef = TypedDict(
-    "_RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
-    {
-        "OutpostId": str,
-    },
-)
-_OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef = TypedDict(
-    "_OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef(
-    _RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
-    _OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSharedEndpointsRequestRequestTypeDef = TypedDict(
     "_RequiredListSharedEndpointsRequestRequestTypeDef",
     {
         "OutpostId": str,
     },
 )
 _OptionalListSharedEndpointsRequestRequestTypeDef = TypedDict(
@@ -195,32 +163,26 @@
 class ListSharedEndpointsRequestRequestTypeDef(
     _RequiredListSharedEndpointsRequestRequestTypeDef,
     _OptionalListSharedEndpointsRequestRequestTypeDef,
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+CreateEndpointResultTypeDef = TypedDict(
+    "CreateEndpointResultTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "EndpointArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "EndpointArn": str,
@@ -235,33 +197,71 @@
         "AccessType": EndpointAccessTypeType,
         "CustomerOwnedIpv4Pool": str,
         "FailedReason": FailedReasonTypeDef,
     },
     total=False,
 )
 
+ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef = TypedDict(
+    "ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef = TypedDict(
+    "_RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
+    {
+        "OutpostId": str,
+    },
+)
+_OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef = TypedDict(
+    "_OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef(
+    _RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
+    _OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
+):
+    pass
+
+
 ListOutpostsWithS3ResultTypeDef = TypedDict(
     "ListOutpostsWithS3ResultTypeDef",
     {
         "Outposts": List[OutpostTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEndpointsResultTypeDef = TypedDict(
     "ListEndpointsResultTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSharedEndpointsResultTypeDef = TypedDict(
     "ListSharedEndpointsResultTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/type_defs.pyi` & `mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CreateEndpointRequestRequestTypeDef",
-    "CreateEndpointResultTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteEndpointRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "FailedReasonTypeDef",
     "NetworkInterfaceTypeDef",
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEndpointsRequestRequestTypeDef",
-    "ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef",
     "ListOutpostsWithS3RequestRequestTypeDef",
     "OutpostTypeDef",
-    "ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
     "ListSharedEndpointsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateEndpointResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EndpointTypeDef",
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+    "ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef",
+    "ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
     "ListOutpostsWithS3ResultTypeDef",
     "ListEndpointsResultTypeDef",
     "ListSharedEndpointsResultTypeDef",
 )
 
 _RequiredCreateEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointRequestRequestTypeDef",
@@ -62,37 +62,33 @@
 )
 
 class CreateEndpointRequestRequestTypeDef(
     _RequiredCreateEndpointRequestRequestTypeDef, _OptionalCreateEndpointRequestRequestTypeDef
 ):
     pass
 
-CreateEndpointResultTypeDef = TypedDict(
-    "CreateEndpointResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "EndpointArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteEndpointRequestRequestTypeDef = TypedDict(
     "DeleteEndpointRequestRequestTypeDef",
     {
         "EndpointId": str,
         "OutpostId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FailedReasonTypeDef = TypedDict(
     "FailedReasonTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
@@ -102,39 +98,33 @@
     "NetworkInterfaceTypeDef",
     {
         "NetworkInterfaceId": str,
     },
     total=False,
 )
 
-ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListEndpointsRequestRequestTypeDef = TypedDict(
     "ListEndpointsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef = TypedDict(
-    "ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOutpostsWithS3RequestRequestTypeDef = TypedDict(
     "ListOutpostsWithS3RequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -147,34 +137,14 @@
         "OutpostId": str,
         "OwnerId": str,
         "CapacityInBytes": int,
     },
     total=False,
 )
 
-_RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef = TypedDict(
-    "_RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
-    {
-        "OutpostId": str,
-    },
-)
-_OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef = TypedDict(
-    "_OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef(
-    _RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
-    _OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
-):
-    pass
-
 _RequiredListSharedEndpointsRequestRequestTypeDef = TypedDict(
     "_RequiredListSharedEndpointsRequestRequestTypeDef",
     {
         "OutpostId": str,
     },
 )
 _OptionalListSharedEndpointsRequestRequestTypeDef = TypedDict(
@@ -188,32 +158,26 @@
 
 class ListSharedEndpointsRequestRequestTypeDef(
     _RequiredListSharedEndpointsRequestRequestTypeDef,
     _OptionalListSharedEndpointsRequestRequestTypeDef,
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+CreateEndpointResultTypeDef = TypedDict(
+    "CreateEndpointResultTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "EndpointArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "EndpointArn": str,
@@ -228,33 +192,69 @@
         "AccessType": EndpointAccessTypeType,
         "CustomerOwnedIpv4Pool": str,
         "FailedReason": FailedReasonTypeDef,
     },
     total=False,
 )
 
+ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef = TypedDict(
+    "ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef = TypedDict(
+    "_RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
+    {
+        "OutpostId": str,
+    },
+)
+_OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef = TypedDict(
+    "_OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef(
+    _RequiredListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
+    _OptionalListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
+):
+    pass
+
 ListOutpostsWithS3ResultTypeDef = TypedDict(
     "ListOutpostsWithS3ResultTypeDef",
     {
         "Outposts": List[OutpostTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEndpointsResultTypeDef = TypedDict(
     "ListEndpointsResultTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSharedEndpointsResultTypeDef = TypedDict(
     "ListSharedEndpointsResultTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts.egg-info/PKG-INFO` & `mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3outposts
-Version: 1.28.0
-Summary: Type annotations for boto3.S3Outposts 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.S3Outposts 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-s3outposts"></a>
 
 # mypy-boto3-s3outposts
 
 [![PyPI - mypy-boto3-s3outposts](https://img.shields.io/pypi/v/mypy-boto3-s3outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3outposts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3outposts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3outposts?color=blue)](https://pypistats.org/packages/mypy-boto3-s3outposts)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-s3outposts)](https://pepy.tech/project/mypy-boto3-s3outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Outposts 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
+[boto3.S3Outposts 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
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
 [mypy-boto3-s3outposts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,29 +333,29 @@
 
 `mypy_boto3_s3outposts.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3outposts.type_defs import (
     CreateEndpointRequestRequestTypeDef,
-    CreateEndpointResultTypeDef,
+    ResponseMetadataTypeDef,
     DeleteEndpointRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     FailedReasonTypeDef,
     NetworkInterfaceTypeDef,
-    ListEndpointsRequestListEndpointsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEndpointsRequestRequestTypeDef,
-    ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef,
     ListOutpostsWithS3RequestRequestTypeDef,
     OutpostTypeDef,
-    ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
     ListSharedEndpointsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    CreateEndpointResultTypeDef,
+    EmptyResponseMetadataTypeDef,
     EndpointTypeDef,
+    ListEndpointsRequestListEndpointsPaginateTypeDef,
+    ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef,
+    ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
     ListOutpostsWithS3ResultTypeDef,
     ListEndpointsResultTypeDef,
     ListSharedEndpointsResultTypeDef,
 )
 
 
 def get_structure() -> CreateEndpointRequestRequestTypeDef:
```

### Comparing `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts.egg-info/SOURCES.txt` & `mypy-boto3-s3outposts-1.28.12/mypy_boto3_s3outposts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.28.0/setup.py` & `mypy-boto3-s3outposts-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-s3outposts",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_s3outposts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.S3Outposts 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.S3Outposts 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

