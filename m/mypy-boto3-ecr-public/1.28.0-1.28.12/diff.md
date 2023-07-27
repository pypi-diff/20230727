# Comparing `tmp/mypy-boto3-ecr-public-1.28.0.tar.gz` & `tmp/mypy-boto3-ecr-public-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ecr-public-1.28.0.tar", last modified: Thu Jul  6 20:59:29 2023, max compression
+gzip compressed data, was "mypy-boto3-ecr-public-1.28.12.tar", last modified: Thu Jul 27 05:34:37 2023, max compression
```

## Comparing `mypy-boto3-ecr-public-1.28.0.tar` & `mypy-boto3-ecr-public-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:29.622290 mypy-boto3-ecr-public-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:39:51.000000 mypy-boto3-ecr-public-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15810 2023-07-06 20:59:29.618291 mypy-boto3-ecr-public-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14314 2023-07-06 20:39:51.000000 mypy-boto3-ecr-public-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:29.610291 mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-06 20:39:51.000000 mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-06 20:39:51.000000 mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-06 20:39:51.000000 mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20578 2023-07-06 20:39:52.000000 mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-07-06 20:39:52.000000 mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-07-06 20:39:52.000000 mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-07-06 20:39:52.000000 mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-06 20:39:52.000000 mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-06 20:39:52.000000 mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:39:51.000000 mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23758 2023-07-06 20:39:53.000000 mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23723 2023-07-06 20:39:52.000000 mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:39:51.000000 mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:29.618291 mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15810 2023-07-06 20:59:29.000000 mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-06 20:59:29.000000 mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:29.000000 mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:29.000000 mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:29.000000 mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 20:59:29.000000 mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:29.622290 mypy-boto3-ecr-public-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-06 20:39:51.000000 mypy-boto3-ecr-public-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:37.804523 mypy-boto3-ecr-public-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15853 2023-07-27 05:34:37.804523 mypy-boto3-ecr-public-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14355 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:37.800523 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20578 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24135 2023-07-27 05:21:31.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-07-27 05:21:31.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:37.804523 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15853 2023-07-27 05:34:37.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:37.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:37.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:37.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:37.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:37.000000 mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:37.804523 mypy-boto3-ecr-public-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-27 05:21:29.000000 mypy-boto3-ecr-public-1.28.12/setup.py
```

### Comparing `mypy-boto3-ecr-public-1.28.0/LICENSE` & `mypy-boto3-ecr-public-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.0/PKG-INFO` & `mypy-boto3-ecr-public-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr-public
-Version: 1.28.0
-Summary: Type annotations for boto3.ECRPublic 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ECRPublic 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ecr-public"></a>
 
 # mypy-boto3-ecr-public
 
 [![PyPI - mypy-boto3-ecr-public](https://img.shields.io/pypi/v/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecr-public?color=blue)](https://pypistats.org/packages/mypy-boto3-ecr-public)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecr-public)](https://pepy.tech/project/mypy-boto3-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECRPublic 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[boto3.ECRPublic 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
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
 [mypy-boto3-ecr-public docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/).
 
 See how it helps to find and fix potential bugs:
 
@@ -344,14 +344,15 @@
 ```python
 from mypy_boto3_ecr_public.type_defs import (
     AuthorizationDataTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
     ImageIdentifierTypeDef,
+    ImageIdentifierOutputTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
     CompleteLayerUploadResponseTypeDef,
     RepositoryCatalogDataInputTypeDef,
     TagTypeDef,
     RepositoryCatalogDataTypeDef,
     RepositoryTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
@@ -368,14 +369,15 @@
     GetRepositoryCatalogDataRequestRequestTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
     GetRepositoryPolicyResponseTypeDef,
     ReferencedImageDetailTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
     InitiateLayerUploadResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutRegistryCatalogDataRequestRequestTypeDef,
     RegistryAliasTypeDef,
     ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
     SetRepositoryPolicyResponseTypeDef,
@@ -387,25 +389,25 @@
     BatchDeleteImageRequestRequestTypeDef,
     DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     PutRepositoryCatalogDataRequestRequestTypeDef,
     CreateRepositoryRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetRepositoryCatalogDataResponseTypeDef,
     PutRepositoryCatalogDataResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
     DescribeImagesResponseTypeDef,
     GetRegistryCatalogDataResponseTypeDef,
     PutRegistryCatalogDataResponseTypeDef,
     ImageTagDetailTypeDef,
+    ListTagsForResourceResponseTypeDef,
     RegistryTypeDef,
     BatchDeleteImageResponseTypeDef,
     PutImageResponseTypeDef,
     DescribeImageTagsResponseTypeDef,
     DescribeRegistriesResponseTypeDef,
 )
```

### Comparing `mypy-boto3-ecr-public-1.28.0/README.md` & `mypy-boto3-ecr-public-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ecr-public"></a>
 
 # mypy-boto3-ecr-public
 
 [![PyPI - mypy-boto3-ecr-public](https://img.shields.io/pypi/v/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecr-public?color=blue)](https://pypistats.org/packages/mypy-boto3-ecr-public)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecr-public)](https://pepy.tech/project/mypy-boto3-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECRPublic 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[boto3.ECRPublic 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
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
 [mypy-boto3-ecr-public docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,14 +312,15 @@
 ```python
 from mypy_boto3_ecr_public.type_defs import (
     AuthorizationDataTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
     ImageIdentifierTypeDef,
+    ImageIdentifierOutputTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
     CompleteLayerUploadResponseTypeDef,
     RepositoryCatalogDataInputTypeDef,
     TagTypeDef,
     RepositoryCatalogDataTypeDef,
     RepositoryTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
@@ -336,14 +337,15 @@
     GetRepositoryCatalogDataRequestRequestTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
     GetRepositoryPolicyResponseTypeDef,
     ReferencedImageDetailTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
     InitiateLayerUploadResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutRegistryCatalogDataRequestRequestTypeDef,
     RegistryAliasTypeDef,
     ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
     SetRepositoryPolicyResponseTypeDef,
@@ -355,25 +357,25 @@
     BatchDeleteImageRequestRequestTypeDef,
     DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     PutRepositoryCatalogDataRequestRequestTypeDef,
     CreateRepositoryRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetRepositoryCatalogDataResponseTypeDef,
     PutRepositoryCatalogDataResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
     DescribeImagesResponseTypeDef,
     GetRegistryCatalogDataResponseTypeDef,
     PutRegistryCatalogDataResponseTypeDef,
     ImageTagDetailTypeDef,
+    ListTagsForResourceResponseTypeDef,
     RegistryTypeDef,
     BatchDeleteImageResponseTypeDef,
     PutImageResponseTypeDef,
     DescribeImageTagsResponseTypeDef,
     DescribeRegistriesResponseTypeDef,
 )
```

### Comparing `mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/__init__.py` & `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/__init__.pyi` & `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/__main__.py` & `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ECRPublic 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.ECRPublic 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic\nOther"
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

### Comparing `mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/client.py` & `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/client.pyi` & `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/literals.py` & `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/literals.py`

 * *Files 0% similar despite different names*

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

### Comparing `mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/literals.pyi` & `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -166,14 +166,15 @@
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
@@ -252,26 +253,28 @@
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

### Comparing `mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/paginator.py` & `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/paginator.pyi` & `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/type_defs.py` & `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,21 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AuthorizationDataTypeDef",
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
     "ImageIdentifierTypeDef",
+    "ImageIdentifierOutputTypeDef",
     "CompleteLayerUploadRequestRequestTypeDef",
     "CompleteLayerUploadResponseTypeDef",
     "RepositoryCatalogDataInputTypeDef",
     "TagTypeDef",
     "RepositoryCatalogDataTypeDef",
     "RepositoryTypeDef",
     "DeleteRepositoryPolicyRequestRequestTypeDef",
@@ -56,14 +56,15 @@
     "GetRepositoryCatalogDataRequestRequestTypeDef",
     "GetRepositoryPolicyRequestRequestTypeDef",
     "GetRepositoryPolicyResponseTypeDef",
     "ReferencedImageDetailTypeDef",
     "InitiateLayerUploadRequestRequestTypeDef",
     "InitiateLayerUploadResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "PaginatorConfigTypeDef",
     "PutImageRequestRequestTypeDef",
     "PutRegistryCatalogDataRequestRequestTypeDef",
     "RegistryAliasTypeDef",
     "ResponseMetadataTypeDef",
     "SetRepositoryPolicyRequestRequestTypeDef",
     "SetRepositoryPolicyResponseTypeDef",
@@ -75,25 +76,25 @@
     "BatchDeleteImageRequestRequestTypeDef",
     "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeImagesRequestRequestTypeDef",
     "ImageFailureTypeDef",
     "ImageTypeDef",
     "PutRepositoryCatalogDataRequestRequestTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetRepositoryCatalogDataResponseTypeDef",
     "PutRepositoryCatalogDataResponseTypeDef",
     "CreateRepositoryResponseTypeDef",
     "DeleteRepositoryResponseTypeDef",
     "DescribeRepositoriesResponseTypeDef",
     "DescribeImagesResponseTypeDef",
     "GetRegistryCatalogDataResponseTypeDef",
     "PutRegistryCatalogDataResponseTypeDef",
     "ImageTagDetailTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "RegistryTypeDef",
     "BatchDeleteImageResponseTypeDef",
     "PutImageResponseTypeDef",
     "DescribeImageTagsResponseTypeDef",
     "DescribeRegistriesResponseTypeDef",
 )
 
@@ -117,22 +118,20 @@
     "_OptionalBatchCheckLayerAvailabilityRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class BatchCheckLayerAvailabilityRequestRequestTypeDef(
     _RequiredBatchCheckLayerAvailabilityRequestRequestTypeDef,
     _OptionalBatchCheckLayerAvailabilityRequestRequestTypeDef,
 ):
     pass
 
-
 LayerFailureTypeDef = TypedDict(
     "LayerFailureTypeDef",
     {
         "layerDigest": str,
         "failureCode": LayerFailureCodeType,
         "failureReason": str,
     },
@@ -155,14 +154,23 @@
     {
         "imageDigest": str,
         "imageTag": str,
     },
     total=False,
 )
 
+ImageIdentifierOutputTypeDef = TypedDict(
+    "ImageIdentifierOutputTypeDef",
+    {
+        "imageDigest": str,
+        "imageTag": str,
+    },
+    total=False,
+)
+
 _RequiredCompleteLayerUploadRequestRequestTypeDef = TypedDict(
     "_RequiredCompleteLayerUploadRequestRequestTypeDef",
     {
         "repositoryName": str,
         "uploadId": str,
         "layerDigests": Sequence[str],
     },
@@ -171,22 +179,20 @@
     "_OptionalCompleteLayerUploadRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class CompleteLayerUploadRequestRequestTypeDef(
     _RequiredCompleteLayerUploadRequestRequestTypeDef,
     _OptionalCompleteLayerUploadRequestRequestTypeDef,
 ):
     pass
 
-
 CompleteLayerUploadResponseTypeDef = TypedDict(
     "CompleteLayerUploadResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "uploadId": str,
         "layerDigest": str,
@@ -252,22 +258,20 @@
     "_OptionalDeleteRepositoryPolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class DeleteRepositoryPolicyRequestRequestTypeDef(
     _RequiredDeleteRepositoryPolicyRequestRequestTypeDef,
     _OptionalDeleteRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteRepositoryPolicyResponseTypeDef = TypedDict(
     "DeleteRepositoryPolicyResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "policyText": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -285,21 +289,19 @@
     {
         "registryId": str,
         "force": bool,
     },
     total=False,
 )
 
-
 class DeleteRepositoryRequestRequestTypeDef(
     _RequiredDeleteRepositoryRequestRequestTypeDef, _OptionalDeleteRepositoryRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
     "_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
@@ -307,22 +309,20 @@
     {
         "registryId": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef(
     _RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
     _OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeImageTagsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageTagsRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImageTagsRequestRequestTypeDef = TypedDict(
@@ -331,21 +331,19 @@
         "registryId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class DescribeImageTagsRequestRequestTypeDef(
     _RequiredDescribeImageTagsRequestRequestTypeDef, _OptionalDescribeImageTagsRequestRequestTypeDef
 ):
     pass
 
-
 ImageDetailTypeDef = TypedDict(
     "ImageDetailTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "imageDigest": str,
         "imageTags": List[str],
@@ -413,44 +411,40 @@
     "_OptionalGetRepositoryCatalogDataRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class GetRepositoryCatalogDataRequestRequestTypeDef(
     _RequiredGetRepositoryCatalogDataRequestRequestTypeDef,
     _OptionalGetRepositoryCatalogDataRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalGetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalGetRepositoryPolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class GetRepositoryPolicyRequestRequestTypeDef(
     _RequiredGetRepositoryPolicyRequestRequestTypeDef,
     _OptionalGetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 GetRepositoryPolicyResponseTypeDef = TypedDict(
     "GetRepositoryPolicyResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "policyText": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -479,22 +473,20 @@
     "_OptionalInitiateLayerUploadRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class InitiateLayerUploadRequestRequestTypeDef(
     _RequiredInitiateLayerUploadRequestRequestTypeDef,
     _OptionalInitiateLayerUploadRequestRequestTypeDef,
 ):
     pass
 
-
 InitiateLayerUploadResponseTypeDef = TypedDict(
     "InitiateLayerUploadResponseTypeDef",
     {
         "uploadId": str,
         "partSize": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -503,14 +495,23 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -531,21 +532,19 @@
         "imageManifestMediaType": str,
         "imageTag": str,
         "imageDigest": str,
     },
     total=False,
 )
 
-
 class PutImageRequestRequestTypeDef(
     _RequiredPutImageRequestRequestTypeDef, _OptionalPutImageRequestRequestTypeDef
 ):
     pass
 
-
 PutRegistryCatalogDataRequestRequestTypeDef = TypedDict(
     "PutRegistryCatalogDataRequestRequestTypeDef",
     {
         "displayName": str,
     },
     total=False,
 )
@@ -583,22 +582,20 @@
     {
         "registryId": str,
         "force": bool,
     },
     total=False,
 )
 
-
 class SetRepositoryPolicyRequestRequestTypeDef(
     _RequiredSetRepositoryPolicyRequestRequestTypeDef,
     _OptionalSetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 SetRepositoryPolicyResponseTypeDef = TypedDict(
     "SetRepositoryPolicyResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "policyText": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -627,21 +624,19 @@
     "_OptionalUploadLayerPartRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class UploadLayerPartRequestRequestTypeDef(
     _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
 ):
     pass
 
-
 UploadLayerPartResponseTypeDef = TypedDict(
     "UploadLayerPartResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "uploadId": str,
         "lastByteReceived": int,
@@ -677,21 +672,19 @@
     "_OptionalBatchDeleteImageRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class BatchDeleteImageRequestRequestTypeDef(
     _RequiredBatchDeleteImageRequestRequestTypeDef, _OptionalBatchDeleteImageRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
@@ -700,22 +693,20 @@
         "registryId": str,
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeImagesRequestDescribeImagesPaginateTypeDef(
     _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
     _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeImagesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImagesRequestRequestTypeDef = TypedDict(
@@ -725,37 +716,35 @@
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class DescribeImagesRequestRequestTypeDef(
     _RequiredDescribeImagesRequestRequestTypeDef, _OptionalDescribeImagesRequestRequestTypeDef
 ):
     pass
 
-
 ImageFailureTypeDef = TypedDict(
     "ImageFailureTypeDef",
     {
-        "imageId": ImageIdentifierTypeDef,
+        "imageId": ImageIdentifierOutputTypeDef,
         "failureCode": ImageFailureCodeType,
         "failureReason": str,
     },
     total=False,
 )
 
 ImageTypeDef = TypedDict(
     "ImageTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
-        "imageId": ImageIdentifierTypeDef,
+        "imageId": ImageIdentifierOutputTypeDef,
         "imageManifest": str,
         "imageManifestMediaType": str,
     },
     total=False,
 )
 
 _RequiredPutRepositoryCatalogDataRequestRequestTypeDef = TypedDict(
@@ -769,22 +758,20 @@
     "_OptionalPutRepositoryCatalogDataRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class PutRepositoryCatalogDataRequestRequestTypeDef(
     _RequiredPutRepositoryCatalogDataRequestRequestTypeDef,
     _OptionalPutRepositoryCatalogDataRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRepositoryRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalCreateRepositoryRequestRequestTypeDef = TypedDict(
@@ -792,29 +779,19 @@
     {
         "catalogData": RepositoryCatalogDataInputTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateRepositoryRequestRequestTypeDef(
     _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
 ):
     pass
 
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -892,29 +869,37 @@
         "imageTag": str,
         "createdAt": datetime,
         "imageDetail": ReferencedImageDetailTypeDef,
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegistryTypeDef = TypedDict(
     "RegistryTypeDef",
     {
         "registryId": str,
         "registryArn": str,
         "registryUri": str,
         "verified": bool,
         "aliases": List[RegistryAliasTypeDef],
     },
 )
 
 BatchDeleteImageResponseTypeDef = TypedDict(
     "BatchDeleteImageResponseTypeDef",
     {
-        "imageIds": List[ImageIdentifierTypeDef],
+        "imageIds": List[ImageIdentifierOutputTypeDef],
         "failures": List[ImageFailureTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutImageResponseTypeDef = TypedDict(
     "PutImageResponseTypeDef",
```

### Comparing `mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public/type_defs.pyi` & `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,20 +25,22 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AuthorizationDataTypeDef",
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
     "ImageIdentifierTypeDef",
+    "ImageIdentifierOutputTypeDef",
     "CompleteLayerUploadRequestRequestTypeDef",
     "CompleteLayerUploadResponseTypeDef",
     "RepositoryCatalogDataInputTypeDef",
     "TagTypeDef",
     "RepositoryCatalogDataTypeDef",
     "RepositoryTypeDef",
     "DeleteRepositoryPolicyRequestRequestTypeDef",
@@ -55,14 +57,15 @@
     "GetRepositoryCatalogDataRequestRequestTypeDef",
     "GetRepositoryPolicyRequestRequestTypeDef",
     "GetRepositoryPolicyResponseTypeDef",
     "ReferencedImageDetailTypeDef",
     "InitiateLayerUploadRequestRequestTypeDef",
     "InitiateLayerUploadResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "PaginatorConfigTypeDef",
     "PutImageRequestRequestTypeDef",
     "PutRegistryCatalogDataRequestRequestTypeDef",
     "RegistryAliasTypeDef",
     "ResponseMetadataTypeDef",
     "SetRepositoryPolicyRequestRequestTypeDef",
     "SetRepositoryPolicyResponseTypeDef",
@@ -74,25 +77,25 @@
     "BatchDeleteImageRequestRequestTypeDef",
     "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeImagesRequestRequestTypeDef",
     "ImageFailureTypeDef",
     "ImageTypeDef",
     "PutRepositoryCatalogDataRequestRequestTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetRepositoryCatalogDataResponseTypeDef",
     "PutRepositoryCatalogDataResponseTypeDef",
     "CreateRepositoryResponseTypeDef",
     "DeleteRepositoryResponseTypeDef",
     "DescribeRepositoriesResponseTypeDef",
     "DescribeImagesResponseTypeDef",
     "GetRegistryCatalogDataResponseTypeDef",
     "PutRegistryCatalogDataResponseTypeDef",
     "ImageTagDetailTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "RegistryTypeDef",
     "BatchDeleteImageResponseTypeDef",
     "PutImageResponseTypeDef",
     "DescribeImageTagsResponseTypeDef",
     "DescribeRegistriesResponseTypeDef",
 )
 
@@ -116,20 +119,22 @@
     "_OptionalBatchCheckLayerAvailabilityRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class BatchCheckLayerAvailabilityRequestRequestTypeDef(
     _RequiredBatchCheckLayerAvailabilityRequestRequestTypeDef,
     _OptionalBatchCheckLayerAvailabilityRequestRequestTypeDef,
 ):
     pass
 
+
 LayerFailureTypeDef = TypedDict(
     "LayerFailureTypeDef",
     {
         "layerDigest": str,
         "failureCode": LayerFailureCodeType,
         "failureReason": str,
     },
@@ -152,14 +157,23 @@
     {
         "imageDigest": str,
         "imageTag": str,
     },
     total=False,
 )
 
+ImageIdentifierOutputTypeDef = TypedDict(
+    "ImageIdentifierOutputTypeDef",
+    {
+        "imageDigest": str,
+        "imageTag": str,
+    },
+    total=False,
+)
+
 _RequiredCompleteLayerUploadRequestRequestTypeDef = TypedDict(
     "_RequiredCompleteLayerUploadRequestRequestTypeDef",
     {
         "repositoryName": str,
         "uploadId": str,
         "layerDigests": Sequence[str],
     },
@@ -168,20 +182,22 @@
     "_OptionalCompleteLayerUploadRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class CompleteLayerUploadRequestRequestTypeDef(
     _RequiredCompleteLayerUploadRequestRequestTypeDef,
     _OptionalCompleteLayerUploadRequestRequestTypeDef,
 ):
     pass
 
+
 CompleteLayerUploadResponseTypeDef = TypedDict(
     "CompleteLayerUploadResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "uploadId": str,
         "layerDigest": str,
@@ -247,20 +263,22 @@
     "_OptionalDeleteRepositoryPolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class DeleteRepositoryPolicyRequestRequestTypeDef(
     _RequiredDeleteRepositoryPolicyRequestRequestTypeDef,
     _OptionalDeleteRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteRepositoryPolicyResponseTypeDef = TypedDict(
     "DeleteRepositoryPolicyResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "policyText": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -278,19 +296,21 @@
     {
         "registryId": str,
         "force": bool,
     },
     total=False,
 )
 
+
 class DeleteRepositoryRequestRequestTypeDef(
     _RequiredDeleteRepositoryRequestRequestTypeDef, _OptionalDeleteRepositoryRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
     "_RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = TypedDict(
@@ -298,20 +318,22 @@
     {
         "registryId": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef(
     _RequiredDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
     _OptionalDescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeImageTagsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageTagsRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImageTagsRequestRequestTypeDef = TypedDict(
@@ -320,19 +342,21 @@
         "registryId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class DescribeImageTagsRequestRequestTypeDef(
     _RequiredDescribeImageTagsRequestRequestTypeDef, _OptionalDescribeImageTagsRequestRequestTypeDef
 ):
     pass
 
+
 ImageDetailTypeDef = TypedDict(
     "ImageDetailTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "imageDigest": str,
         "imageTags": List[str],
@@ -400,40 +424,44 @@
     "_OptionalGetRepositoryCatalogDataRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class GetRepositoryCatalogDataRequestRequestTypeDef(
     _RequiredGetRepositoryCatalogDataRequestRequestTypeDef,
     _OptionalGetRepositoryCatalogDataRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalGetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalGetRepositoryPolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class GetRepositoryPolicyRequestRequestTypeDef(
     _RequiredGetRepositoryPolicyRequestRequestTypeDef,
     _OptionalGetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 GetRepositoryPolicyResponseTypeDef = TypedDict(
     "GetRepositoryPolicyResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "policyText": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -462,20 +490,22 @@
     "_OptionalInitiateLayerUploadRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class InitiateLayerUploadRequestRequestTypeDef(
     _RequiredInitiateLayerUploadRequestRequestTypeDef,
     _OptionalInitiateLayerUploadRequestRequestTypeDef,
 ):
     pass
 
+
 InitiateLayerUploadResponseTypeDef = TypedDict(
     "InitiateLayerUploadResponseTypeDef",
     {
         "uploadId": str,
         "partSize": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -484,14 +514,23 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -512,19 +551,21 @@
         "imageManifestMediaType": str,
         "imageTag": str,
         "imageDigest": str,
     },
     total=False,
 )
 
+
 class PutImageRequestRequestTypeDef(
     _RequiredPutImageRequestRequestTypeDef, _OptionalPutImageRequestRequestTypeDef
 ):
     pass
 
+
 PutRegistryCatalogDataRequestRequestTypeDef = TypedDict(
     "PutRegistryCatalogDataRequestRequestTypeDef",
     {
         "displayName": str,
     },
     total=False,
 )
@@ -562,20 +603,22 @@
     {
         "registryId": str,
         "force": bool,
     },
     total=False,
 )
 
+
 class SetRepositoryPolicyRequestRequestTypeDef(
     _RequiredSetRepositoryPolicyRequestRequestTypeDef,
     _OptionalSetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 SetRepositoryPolicyResponseTypeDef = TypedDict(
     "SetRepositoryPolicyResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "policyText": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -604,19 +647,21 @@
     "_OptionalUploadLayerPartRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class UploadLayerPartRequestRequestTypeDef(
     _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
 ):
     pass
 
+
 UploadLayerPartResponseTypeDef = TypedDict(
     "UploadLayerPartResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "uploadId": str,
         "lastByteReceived": int,
@@ -652,19 +697,21 @@
     "_OptionalBatchDeleteImageRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class BatchDeleteImageRequestRequestTypeDef(
     _RequiredBatchDeleteImageRequestRequestTypeDef, _OptionalBatchDeleteImageRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
@@ -673,20 +720,22 @@
         "registryId": str,
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeImagesRequestDescribeImagesPaginateTypeDef(
     _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
     _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeImagesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImagesRequestRequestTypeDef = TypedDict(
@@ -696,35 +745,37 @@
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class DescribeImagesRequestRequestTypeDef(
     _RequiredDescribeImagesRequestRequestTypeDef, _OptionalDescribeImagesRequestRequestTypeDef
 ):
     pass
 
+
 ImageFailureTypeDef = TypedDict(
     "ImageFailureTypeDef",
     {
-        "imageId": ImageIdentifierTypeDef,
+        "imageId": ImageIdentifierOutputTypeDef,
         "failureCode": ImageFailureCodeType,
         "failureReason": str,
     },
     total=False,
 )
 
 ImageTypeDef = TypedDict(
     "ImageTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
-        "imageId": ImageIdentifierTypeDef,
+        "imageId": ImageIdentifierOutputTypeDef,
         "imageManifest": str,
         "imageManifestMediaType": str,
     },
     total=False,
 )
 
 _RequiredPutRepositoryCatalogDataRequestRequestTypeDef = TypedDict(
@@ -738,20 +789,22 @@
     "_OptionalPutRepositoryCatalogDataRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class PutRepositoryCatalogDataRequestRequestTypeDef(
     _RequiredPutRepositoryCatalogDataRequestRequestTypeDef,
     _OptionalPutRepositoryCatalogDataRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRepositoryRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalCreateRepositoryRequestRequestTypeDef = TypedDict(
@@ -759,26 +812,20 @@
     {
         "catalogData": RepositoryCatalogDataInputTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateRepositoryRequestRequestTypeDef(
     _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
@@ -857,29 +904,37 @@
         "imageTag": str,
         "createdAt": datetime,
         "imageDetail": ReferencedImageDetailTypeDef,
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegistryTypeDef = TypedDict(
     "RegistryTypeDef",
     {
         "registryId": str,
         "registryArn": str,
         "registryUri": str,
         "verified": bool,
         "aliases": List[RegistryAliasTypeDef],
     },
 )
 
 BatchDeleteImageResponseTypeDef = TypedDict(
     "BatchDeleteImageResponseTypeDef",
     {
-        "imageIds": List[ImageIdentifierTypeDef],
+        "imageIds": List[ImageIdentifierOutputTypeDef],
         "failures": List[ImageFailureTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutImageResponseTypeDef = TypedDict(
     "PutImageResponseTypeDef",
```

### Comparing `mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public.egg-info/PKG-INFO` & `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr-public
-Version: 1.28.0
-Summary: Type annotations for boto3.ECRPublic 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ECRPublic 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ecr-public"></a>
 
 # mypy-boto3-ecr-public
 
 [![PyPI - mypy-boto3-ecr-public](https://img.shields.io/pypi/v/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecr-public?color=blue)](https://pypistats.org/packages/mypy-boto3-ecr-public)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecr-public)](https://pepy.tech/project/mypy-boto3-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECRPublic 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[boto3.ECRPublic 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
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
 [mypy-boto3-ecr-public docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/).
 
 See how it helps to find and fix potential bugs:
 
@@ -344,14 +344,15 @@
 ```python
 from mypy_boto3_ecr_public.type_defs import (
     AuthorizationDataTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
     ImageIdentifierTypeDef,
+    ImageIdentifierOutputTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
     CompleteLayerUploadResponseTypeDef,
     RepositoryCatalogDataInputTypeDef,
     TagTypeDef,
     RepositoryCatalogDataTypeDef,
     RepositoryTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
@@ -368,14 +369,15 @@
     GetRepositoryCatalogDataRequestRequestTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
     GetRepositoryPolicyResponseTypeDef,
     ReferencedImageDetailTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
     InitiateLayerUploadResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutRegistryCatalogDataRequestRequestTypeDef,
     RegistryAliasTypeDef,
     ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
     SetRepositoryPolicyResponseTypeDef,
@@ -387,25 +389,25 @@
     BatchDeleteImageRequestRequestTypeDef,
     DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     PutRepositoryCatalogDataRequestRequestTypeDef,
     CreateRepositoryRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetRepositoryCatalogDataResponseTypeDef,
     PutRepositoryCatalogDataResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
     DescribeImagesResponseTypeDef,
     GetRegistryCatalogDataResponseTypeDef,
     PutRegistryCatalogDataResponseTypeDef,
     ImageTagDetailTypeDef,
+    ListTagsForResourceResponseTypeDef,
     RegistryTypeDef,
     BatchDeleteImageResponseTypeDef,
     PutImageResponseTypeDef,
     DescribeImageTagsResponseTypeDef,
     DescribeRegistriesResponseTypeDef,
 )
```

### Comparing `mypy-boto3-ecr-public-1.28.0/mypy_boto3_ecr_public.egg-info/SOURCES.txt` & `mypy-boto3-ecr-public-1.28.12/mypy_boto3_ecr_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.0/setup.py` & `mypy-boto3-ecr-public-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ecr-public",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_ecr_public"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ECRPublic 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.ECRPublic 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

