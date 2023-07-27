# Comparing `tmp/mypy-boto3-sagemaker-a2i-runtime-1.28.0.tar.gz` & `tmp/mypy-boto3-sagemaker-a2i-runtime-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sagemaker-a2i-runtime-1.28.0.tar", last modified: Thu Jul  6 21:00:32 2023, max compression
+gzip compressed data, was "mypy-boto3-sagemaker-a2i-runtime-1.28.12.tar", last modified: Thu Jul 27 11:49:33 2023, max compression
```

## Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.0.tar` & `mypy-boto3-sagemaker-a2i-runtime-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:31.994420 mypy-boto3-sagemaker-a2i-runtime-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:54:48.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-07-06 21:00:31.994420 mypy-boto3-sagemaker-a2i-runtime-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-07-06 20:54:48.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:31.994420 mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-06 20:54:48.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-06 20:54:48.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-06 20:54:48.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-07-06 20:54:48.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-07-06 20:54:48.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-07-06 20:54:48.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-07-06 20:54:48.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-06 20:54:48.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-06 20:54:48.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:54:48.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-06 20:54:48.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-07-06 20:54:48.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:54:48.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:31.994420 mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-07-06 21:00:31.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-06 21:00:31.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:31.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:31.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:31.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-06 21:00:31.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:31.994420 mypy-boto3-sagemaker-a2i-runtime-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-06 20:54:48.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.373242 mypy-boto3-sagemaker-a2i-runtime-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:45:52.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-27 11:49:33.373242 mypy-boto3-sagemaker-a2i-runtime-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12296 2023-07-27 11:45:52.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.361242 mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-27 11:45:52.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-27 11:45:52.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-27 11:45:52.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-07-27 11:45:52.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-07-27 11:45:52.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-07-27 11:45:53.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-07-27 11:45:53.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-27 11:45:53.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-27 11:45:53.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:52.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-07-27 11:45:53.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-07-27 11:45:53.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:45:52.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.373242 mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-27 11:49:33.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-27 11:49:33.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:33.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:33.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:33.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-27 11:49:33.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:33.373242 mypy-boto3-sagemaker-a2i-runtime-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-27 11:45:52.000000 mypy-boto3-sagemaker-a2i-runtime-1.28.12/setup.py
```

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.0/LICENSE` & `mypy-boto3-sagemaker-a2i-runtime-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.0/PKG-INFO` & `mypy-boto3-sagemaker-a2i-runtime-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-a2i-runtime
-Version: 1.28.0
-Summary: Type annotations for boto3.AugmentedAIRuntime 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AugmentedAIRuntime 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sagemaker-a2i-runtime"></a>
 
 # mypy-boto3-sagemaker-a2i-runtime
 
 [![PyPI - mypy-boto3-sagemaker-a2i-runtime](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-a2i-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-a2i-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-a2i-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-a2i-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-a2i-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-a2i-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-a2i-runtime)](https://pepy.tech/project/mypy-boto3-sagemaker-a2i-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AugmentedAIRuntime 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
+[boto3.AugmentedAIRuntime 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
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
 [mypy-boto3-sagemaker-a2i-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,26 +325,26 @@
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_a2i_runtime.type_defs import (
     DeleteHumanLoopRequestRequestTypeDef,
     DescribeHumanLoopRequestRequestTypeDef,
     HumanLoopOutputTypeDef,
+    ResponseMetadataTypeDef,
     HumanLoopDataAttributesTypeDef,
     HumanLoopInputTypeDef,
     HumanLoopSummaryTypeDef,
-    ListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
-    ListHumanLoopsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartHumanLoopResponseTypeDef,
+    ListHumanLoopsRequestRequestTypeDef,
     StopHumanLoopRequestRequestTypeDef,
     DescribeHumanLoopResponseTypeDef,
+    StartHumanLoopResponseTypeDef,
     StartHumanLoopRequestRequestTypeDef,
     ListHumanLoopsResponseTypeDef,
+    ListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
 )
 
 
 def get_structure() -> DeleteHumanLoopRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.0/README.md` & `mypy-boto3-sagemaker-a2i-runtime-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sagemaker-a2i-runtime"></a>
 
 # mypy-boto3-sagemaker-a2i-runtime
 
 [![PyPI - mypy-boto3-sagemaker-a2i-runtime](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-a2i-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-a2i-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-a2i-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-a2i-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-a2i-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-a2i-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-a2i-runtime)](https://pepy.tech/project/mypy-boto3-sagemaker-a2i-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AugmentedAIRuntime 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
+[boto3.AugmentedAIRuntime 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
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
 [mypy-boto3-sagemaker-a2i-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -293,26 +293,26 @@
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_a2i_runtime.type_defs import (
     DeleteHumanLoopRequestRequestTypeDef,
     DescribeHumanLoopRequestRequestTypeDef,
     HumanLoopOutputTypeDef,
+    ResponseMetadataTypeDef,
     HumanLoopDataAttributesTypeDef,
     HumanLoopInputTypeDef,
     HumanLoopSummaryTypeDef,
-    ListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
-    ListHumanLoopsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartHumanLoopResponseTypeDef,
+    ListHumanLoopsRequestRequestTypeDef,
     StopHumanLoopRequestRequestTypeDef,
     DescribeHumanLoopResponseTypeDef,
+    StartHumanLoopResponseTypeDef,
     StartHumanLoopRequestRequestTypeDef,
     ListHumanLoopsResponseTypeDef,
+    ListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
 )
 
 
 def get_structure() -> DeleteHumanLoopRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/__init__.py` & `mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/__init__.pyi` & `mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/client.py` & `mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/client.pyi` & `mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/literals.py` & `mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
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
@@ -237,26 +238,28 @@
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

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/literals.pyi` & `mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,15 @@
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
@@ -235,26 +236,28 @@
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

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/paginator.py` & `mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -25,37 +25,34 @@
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import SortOrderType
 from .type_defs import ListHumanLoopsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListHumanLoopsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListHumanLoopsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Paginator.ListHumanLoops)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/paginators/#listhumanloopspaginator)
     """
 
     def paginate(
         self,
         *,
         FlowDefinitionArn: str,
         CreationTimeAfter: Union[datetime, str] = ...,
         CreationTimeBefore: Union[datetime, str] = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHumanLoopsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Paginator.ListHumanLoops.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/paginators/#listhumanloopspaginator)
         """
```

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/paginator.pyi` & `mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/paginator.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,34 +25,37 @@
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import SortOrderType
 from .type_defs import ListHumanLoopsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListHumanLoopsPaginator",)
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListHumanLoopsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Paginator.ListHumanLoops)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/paginators/#listhumanloopspaginator)
     """
 
     def paginate(
         self,
         *,
         FlowDefinitionArn: str,
         CreationTimeAfter: Union[datetime, str] = ...,
         CreationTimeBefore: Union[datetime, str] = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHumanLoopsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Paginator.ListHumanLoops.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/paginators/#listhumanloopspaginator)
         """
```

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/type_defs.py` & `mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,26 +23,26 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "DeleteHumanLoopRequestRequestTypeDef",
     "DescribeHumanLoopRequestRequestTypeDef",
     "HumanLoopOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "HumanLoopDataAttributesTypeDef",
     "HumanLoopInputTypeDef",
     "HumanLoopSummaryTypeDef",
-    "ListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
-    "ListHumanLoopsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartHumanLoopResponseTypeDef",
+    "ListHumanLoopsRequestRequestTypeDef",
     "StopHumanLoopRequestRequestTypeDef",
     "DescribeHumanLoopResponseTypeDef",
+    "StartHumanLoopResponseTypeDef",
     "StartHumanLoopRequestRequestTypeDef",
     "ListHumanLoopsResponseTypeDef",
+    "ListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
 )
 
 DeleteHumanLoopRequestRequestTypeDef = TypedDict(
     "DeleteHumanLoopRequestRequestTypeDef",
     {
         "HumanLoopName": str,
     },
@@ -58,14 +58,25 @@
 HumanLoopOutputTypeDef = TypedDict(
     "HumanLoopOutputTypeDef",
     {
         "OutputS3Uri": str,
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 HumanLoopDataAttributesTypeDef = TypedDict(
     "HumanLoopDataAttributesTypeDef",
     {
         "ContentClassifiers": Sequence[ContentClassifierType],
     },
 )
 
@@ -84,39 +95,24 @@
         "CreationTime": datetime,
         "FailureReason": str,
         "FlowDefinitionArn": str,
     },
     total=False,
 )
 
-_RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef = TypedDict(
-    "_RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
-    {
-        "FlowDefinitionArn": str,
-    },
-)
-_OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef = TypedDict(
-    "_OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListHumanLoopsRequestListHumanLoopsPaginateTypeDef(
-    _RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
-    _OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListHumanLoopsRequestRequestTypeDef = TypedDict(
     "_RequiredListHumanLoopsRequestRequestTypeDef",
     {
         "FlowDefinitionArn": str,
     },
 )
 _OptionalListHumanLoopsRequestRequestTypeDef = TypedDict(
@@ -134,43 +130,14 @@
 
 class ListHumanLoopsRequestRequestTypeDef(
     _RequiredListHumanLoopsRequestRequestTypeDef, _OptionalListHumanLoopsRequestRequestTypeDef
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
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
-StartHumanLoopResponseTypeDef = TypedDict(
-    "StartHumanLoopResponseTypeDef",
-    {
-        "HumanLoopArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopHumanLoopRequestRequestTypeDef = TypedDict(
     "StopHumanLoopRequestRequestTypeDef",
     {
         "HumanLoopName": str,
     },
 )
 
@@ -181,15 +148,23 @@
         "FailureReason": str,
         "FailureCode": str,
         "HumanLoopStatus": HumanLoopStatusType,
         "HumanLoopName": str,
         "HumanLoopArn": str,
         "FlowDefinitionArn": str,
         "HumanLoopOutput": HumanLoopOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartHumanLoopResponseTypeDef = TypedDict(
+    "StartHumanLoopResponseTypeDef",
+    {
+        "HumanLoopArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartHumanLoopRequestRequestTypeDef = TypedDict(
     "_RequiredStartHumanLoopRequestRequestTypeDef",
     {
         "HumanLoopName": str,
@@ -213,10 +188,34 @@
 
 
 ListHumanLoopsResponseTypeDef = TypedDict(
     "ListHumanLoopsResponseTypeDef",
     {
         "HumanLoopSummaries": List[HumanLoopSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef = TypedDict(
+    "_RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
+    {
+        "FlowDefinitionArn": str,
+    },
+)
+_OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef = TypedDict(
+    "_OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
+    {
+        "CreationTimeAfter": Union[datetime, str],
+        "CreationTimeBefore": Union[datetime, str],
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListHumanLoopsRequestListHumanLoopsPaginateTypeDef(
+    _RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
+    _OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime/type_defs.pyi` & `mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -22,26 +22,26 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "DeleteHumanLoopRequestRequestTypeDef",
     "DescribeHumanLoopRequestRequestTypeDef",
     "HumanLoopOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "HumanLoopDataAttributesTypeDef",
     "HumanLoopInputTypeDef",
     "HumanLoopSummaryTypeDef",
-    "ListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
-    "ListHumanLoopsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartHumanLoopResponseTypeDef",
+    "ListHumanLoopsRequestRequestTypeDef",
     "StopHumanLoopRequestRequestTypeDef",
     "DescribeHumanLoopResponseTypeDef",
+    "StartHumanLoopResponseTypeDef",
     "StartHumanLoopRequestRequestTypeDef",
     "ListHumanLoopsResponseTypeDef",
+    "ListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
 )
 
 DeleteHumanLoopRequestRequestTypeDef = TypedDict(
     "DeleteHumanLoopRequestRequestTypeDef",
     {
         "HumanLoopName": str,
     },
@@ -57,14 +57,25 @@
 HumanLoopOutputTypeDef = TypedDict(
     "HumanLoopOutputTypeDef",
     {
         "OutputS3Uri": str,
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 HumanLoopDataAttributesTypeDef = TypedDict(
     "HumanLoopDataAttributesTypeDef",
     {
         "ContentClassifiers": Sequence[ContentClassifierType],
     },
 )
 
@@ -83,37 +94,24 @@
         "CreationTime": datetime,
         "FailureReason": str,
         "FlowDefinitionArn": str,
     },
     total=False,
 )
 
-_RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef = TypedDict(
-    "_RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
-    {
-        "FlowDefinitionArn": str,
-    },
-)
-_OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef = TypedDict(
-    "_OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListHumanLoopsRequestListHumanLoopsPaginateTypeDef(
-    _RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
-    _OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
-):
-    pass
-
 _RequiredListHumanLoopsRequestRequestTypeDef = TypedDict(
     "_RequiredListHumanLoopsRequestRequestTypeDef",
     {
         "FlowDefinitionArn": str,
     },
 )
 _OptionalListHumanLoopsRequestRequestTypeDef = TypedDict(
@@ -129,43 +127,14 @@
 )
 
 class ListHumanLoopsRequestRequestTypeDef(
     _RequiredListHumanLoopsRequestRequestTypeDef, _OptionalListHumanLoopsRequestRequestTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
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
-StartHumanLoopResponseTypeDef = TypedDict(
-    "StartHumanLoopResponseTypeDef",
-    {
-        "HumanLoopArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopHumanLoopRequestRequestTypeDef = TypedDict(
     "StopHumanLoopRequestRequestTypeDef",
     {
         "HumanLoopName": str,
     },
 )
 
@@ -176,15 +145,23 @@
         "FailureReason": str,
         "FailureCode": str,
         "HumanLoopStatus": HumanLoopStatusType,
         "HumanLoopName": str,
         "HumanLoopArn": str,
         "FlowDefinitionArn": str,
         "HumanLoopOutput": HumanLoopOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartHumanLoopResponseTypeDef = TypedDict(
+    "StartHumanLoopResponseTypeDef",
+    {
+        "HumanLoopArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartHumanLoopRequestRequestTypeDef = TypedDict(
     "_RequiredStartHumanLoopRequestRequestTypeDef",
     {
         "HumanLoopName": str,
@@ -206,10 +183,33 @@
     pass
 
 ListHumanLoopsResponseTypeDef = TypedDict(
     "ListHumanLoopsResponseTypeDef",
     {
         "HumanLoopSummaries": List[HumanLoopSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef = TypedDict(
+    "_RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
+    {
+        "FlowDefinitionArn": str,
+    },
+)
+_OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef = TypedDict(
+    "_OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
+    {
+        "CreationTimeAfter": Union[datetime, str],
+        "CreationTimeBefore": Union[datetime, str],
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
+
+class ListHumanLoopsRequestListHumanLoopsPaginateTypeDef(
+    _RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
+    _OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime.egg-info/PKG-INFO` & `mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-a2i-runtime
-Version: 1.28.0
-Summary: Type annotations for boto3.AugmentedAIRuntime 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AugmentedAIRuntime 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sagemaker-a2i-runtime"></a>
 
 # mypy-boto3-sagemaker-a2i-runtime
 
 [![PyPI - mypy-boto3-sagemaker-a2i-runtime](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-a2i-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-a2i-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-a2i-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-a2i-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-a2i-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-a2i-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-a2i-runtime)](https://pepy.tech/project/mypy-boto3-sagemaker-a2i-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AugmentedAIRuntime 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
+[boto3.AugmentedAIRuntime 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
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
 [mypy-boto3-sagemaker-a2i-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_a2i_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,26 +325,26 @@
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_a2i_runtime.type_defs import (
     DeleteHumanLoopRequestRequestTypeDef,
     DescribeHumanLoopRequestRequestTypeDef,
     HumanLoopOutputTypeDef,
+    ResponseMetadataTypeDef,
     HumanLoopDataAttributesTypeDef,
     HumanLoopInputTypeDef,
     HumanLoopSummaryTypeDef,
-    ListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
-    ListHumanLoopsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartHumanLoopResponseTypeDef,
+    ListHumanLoopsRequestRequestTypeDef,
     StopHumanLoopRequestRequestTypeDef,
     DescribeHumanLoopResponseTypeDef,
+    StartHumanLoopResponseTypeDef,
     StartHumanLoopRequestRequestTypeDef,
     ListHumanLoopsResponseTypeDef,
+    ListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
 )
 
 
 def get_structure() -> DeleteHumanLoopRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.0/mypy_boto3_sagemaker_a2i_runtime.egg-info/SOURCES.txt` & `mypy-boto3-sagemaker-a2i-runtime-1.28.12/mypy_boto3_sagemaker_a2i_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-a2i-runtime-1.28.0/setup.py` & `mypy-boto3-sagemaker-a2i-runtime-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker-a2i-runtime",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_sagemaker_a2i_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AugmentedAIRuntime 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.AugmentedAIRuntime 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

