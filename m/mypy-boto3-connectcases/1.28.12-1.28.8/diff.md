# Comparing `tmp/mypy-boto3-connectcases-1.28.12.tar.gz` & `tmp/mypy-boto3-connectcases-1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connectcases-1.28.12.tar", last modified: Thu Jul 27 05:34:31 2023, max compression
+gzip compressed data, was "mypy-boto3-connectcases-1.28.8.tar", last modified: Thu Jul 20 19:47:56 2023, max compression
```

## Comparing `mypy-boto3-connectcases-1.28.12.tar` & `mypy-boto3-connectcases-1.28.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.572542 mypy-boto3-connectcases-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:48.000000 mypy-boto3-connectcases-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-27 05:34:31.568542 mypy-boto3-connectcases-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15307 2023-07-27 05:19:48.000000 mypy-boto3-connectcases-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.560542 mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-27 05:19:48.000000 mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-27 05:19:48.000000 mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:19:48.000000 mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22107 2023-07-27 05:19:48.000000 mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22068 2023-07-27 05:19:48.000000 mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-07-27 05:19:48.000000 mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-07-27 05:19:48.000000 mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-27 05:19:48.000000 mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-27 05:19:48.000000 mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:48.000000 mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33541 2023-07-27 05:19:49.000000 mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33493 2023-07-27 05:19:48.000000 mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:48.000000 mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.568542 mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-27 05:34:31.000000 mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:34:31.000000 mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:31.000000 mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:31.000000 mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:31.000000 mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:31.000000 mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:31.572542 mypy-boto3-connectcases-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:19:47.000000 mypy-boto3-connectcases-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.012775 mypy-boto3-connectcases-1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-07-20 19:47:56.004775 mypy-boto3-connectcases-1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.000775 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22107 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22068 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31710 2023-07-20 19:46:48.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31674 2023-07-20 19:46:48.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.004775 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:56.012775 mypy-boto3-connectcases-1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/setup.py
```

### Comparing `mypy-boto3-connectcases-1.28.12/LICENSE` & `mypy-boto3-connectcases-1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.12/PKG-INFO` & `mypy-boto3-connectcases-1.28.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcases
-Version: 1.28.12
-Summary: Type annotations for boto3.ConnectCases 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.8
+Summary: Type annotations for boto3.ConnectCases 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-connectcases"></a>
 
 # mypy-boto3-connectcases
 
 [![PyPI - mypy-boto3-connectcases](https://img.shields.io/pypi/v/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcases)](https://pepy.tech/project/mypy-boto3-connectcases)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcases?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connectcases docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,71 +333,71 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connectcases.type_defs import (
     FieldIdentifierTypeDef,
     FieldErrorTypeDef,
     GetFieldResponseTypeDef,
+    ResponseMetadataTypeDef,
     FieldOptionTypeDef,
     FieldOptionErrorTypeDef,
     FieldIdentifierOutputTypeDef,
     CaseSummaryTypeDef,
     CommentContentOutputTypeDef,
     CommentContentTypeDef,
     ContactContentTypeDef,
     ContactFilterTypeDef,
     ContactTypeDef,
-    CreateCaseResponseTypeDef,
     CreateDomainRequestRequestTypeDef,
-    CreateDomainResponseTypeDef,
     CreateFieldRequestRequestTypeDef,
-    CreateFieldResponseTypeDef,
-    CreateLayoutResponseTypeDef,
-    CreateRelatedItemResponseTypeDef,
     LayoutConfigurationTypeDef,
     RequiredFieldTypeDef,
-    CreateTemplateResponseTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
     RelatedItemEventIncludedDataOutputTypeDef,
     RelatedItemEventIncludedDataTypeDef,
     FieldItemOutputTypeDef,
     FieldItemTypeDef,
     FieldOptionOutputTypeDef,
     FieldSummaryTypeDef,
     FieldValueUnionOutputTypeDef,
     FieldValueUnionTypeDef,
     GetCaseEventConfigurationRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
-    GetDomainResponseTypeDef,
     GetLayoutRequestRequestTypeDef,
     GetTemplateRequestRequestTypeDef,
     LayoutConfigurationOutputTypeDef,
     RequiredFieldOutputTypeDef,
     LayoutSummaryTypeDef,
     ListCasesForContactRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFieldOptionsRequestRequestTypeDef,
     ListFieldsRequestRequestTypeDef,
     ListLayoutsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SortTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFieldRequestRequestTypeDef,
     BatchGetFieldRequestRequestTypeDef,
     CaseEventIncludedDataTypeDef,
     GetCaseRequestRequestTypeDef,
     BatchGetFieldResponseTypeDef,
+    CreateCaseResponseTypeDef,
+    CreateDomainResponseTypeDef,
+    CreateFieldResponseTypeDef,
+    CreateLayoutResponseTypeDef,
+    CreateRelatedItemResponseTypeDef,
+    CreateTemplateResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDomainResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     BatchPutFieldOptionsRequestRequestTypeDef,
     BatchPutFieldOptionsResponseTypeDef,
     CaseEventIncludedDataOutputTypeDef,
     ListCasesForContactResponseTypeDef,
     RelatedItemContentTypeDef,
     RelatedItemTypeFilterTypeDef,
     RelatedItemInputContentTypeDef,
```

### Comparing `mypy-boto3-connectcases-1.28.12/README.md` & `mypy-boto3-connectcases-1.28.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-connectcases"></a>
 
 # mypy-boto3-connectcases
 
 [![PyPI - mypy-boto3-connectcases](https://img.shields.io/pypi/v/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcases)](https://pepy.tech/project/mypy-boto3-connectcases)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcases?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connectcases docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,71 +301,71 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connectcases.type_defs import (
     FieldIdentifierTypeDef,
     FieldErrorTypeDef,
     GetFieldResponseTypeDef,
+    ResponseMetadataTypeDef,
     FieldOptionTypeDef,
     FieldOptionErrorTypeDef,
     FieldIdentifierOutputTypeDef,
     CaseSummaryTypeDef,
     CommentContentOutputTypeDef,
     CommentContentTypeDef,
     ContactContentTypeDef,
     ContactFilterTypeDef,
     ContactTypeDef,
-    CreateCaseResponseTypeDef,
     CreateDomainRequestRequestTypeDef,
-    CreateDomainResponseTypeDef,
     CreateFieldRequestRequestTypeDef,
-    CreateFieldResponseTypeDef,
-    CreateLayoutResponseTypeDef,
-    CreateRelatedItemResponseTypeDef,
     LayoutConfigurationTypeDef,
     RequiredFieldTypeDef,
-    CreateTemplateResponseTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
     RelatedItemEventIncludedDataOutputTypeDef,
     RelatedItemEventIncludedDataTypeDef,
     FieldItemOutputTypeDef,
     FieldItemTypeDef,
     FieldOptionOutputTypeDef,
     FieldSummaryTypeDef,
     FieldValueUnionOutputTypeDef,
     FieldValueUnionTypeDef,
     GetCaseEventConfigurationRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
-    GetDomainResponseTypeDef,
     GetLayoutRequestRequestTypeDef,
     GetTemplateRequestRequestTypeDef,
     LayoutConfigurationOutputTypeDef,
     RequiredFieldOutputTypeDef,
     LayoutSummaryTypeDef,
     ListCasesForContactRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFieldOptionsRequestRequestTypeDef,
     ListFieldsRequestRequestTypeDef,
     ListLayoutsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SortTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFieldRequestRequestTypeDef,
     BatchGetFieldRequestRequestTypeDef,
     CaseEventIncludedDataTypeDef,
     GetCaseRequestRequestTypeDef,
     BatchGetFieldResponseTypeDef,
+    CreateCaseResponseTypeDef,
+    CreateDomainResponseTypeDef,
+    CreateFieldResponseTypeDef,
+    CreateLayoutResponseTypeDef,
+    CreateRelatedItemResponseTypeDef,
+    CreateTemplateResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDomainResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     BatchPutFieldOptionsRequestRequestTypeDef,
     BatchPutFieldOptionsResponseTypeDef,
     CaseEventIncludedDataOutputTypeDef,
     ListCasesForContactResponseTypeDef,
     RelatedItemContentTypeDef,
     RelatedItemTypeFilterTypeDef,
     RelatedItemInputContentTypeDef,
```

### Comparing `mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/__init__.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/__init__.pyi` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/__main__.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConnectCases 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ConnectCases 1.28.8\nVersion:         1.28.8\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.8")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/client.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/client.pyi` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/literals.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -249,15 +248,14 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
```

### Comparing `mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/literals.pyi` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -247,15 +246,14 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
```

### Comparing `mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/paginator.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         self,
         *,
         domainId: str,
         fields: Sequence[FieldIdentifierTypeDef] = ...,
         filter: "CaseFilterTypeDef" = ...,
         searchTerm: str = ...,
         sorts: Sequence[SortTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Paginator.SearchCases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/paginators/#searchcasespaginator)
         """
 
 
@@ -78,13 +78,13 @@
 
     def paginate(
         self,
         *,
         caseId: str,
         domainId: str,
         filters: Sequence[RelatedItemTypeFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchRelatedItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Paginator.SearchRelatedItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/paginators/#searchrelateditemspaginator)
         """
```

### Comparing `mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/paginator.pyi` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         self,
         *,
         domainId: str,
         fields: Sequence[FieldIdentifierTypeDef] = ...,
         filter: "CaseFilterTypeDef" = ...,
         searchTerm: str = ...,
         sorts: Sequence[SortTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Paginator.SearchCases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/paginators/#searchcasespaginator)
         """
 
 class SearchRelatedItemsPaginator(Paginator):
@@ -74,13 +74,13 @@
 
     def paginate(
         self,
         *,
         caseId: str,
         domainId: str,
         filters: Sequence[RelatedItemTypeFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchRelatedItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Paginator.SearchRelatedItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/paginators/#searchrelateditemspaginator)
         """
```

### Comparing `mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/type_defs.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,71 +34,71 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "FieldIdentifierTypeDef",
     "FieldErrorTypeDef",
     "GetFieldResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "FieldOptionTypeDef",
     "FieldOptionErrorTypeDef",
     "FieldIdentifierOutputTypeDef",
     "CaseSummaryTypeDef",
     "CommentContentOutputTypeDef",
     "CommentContentTypeDef",
     "ContactContentTypeDef",
     "ContactFilterTypeDef",
     "ContactTypeDef",
-    "CreateCaseResponseTypeDef",
     "CreateDomainRequestRequestTypeDef",
-    "CreateDomainResponseTypeDef",
     "CreateFieldRequestRequestTypeDef",
-    "CreateFieldResponseTypeDef",
-    "CreateLayoutResponseTypeDef",
-    "CreateRelatedItemResponseTypeDef",
     "LayoutConfigurationTypeDef",
     "RequiredFieldTypeDef",
-    "CreateTemplateResponseTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DomainSummaryTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "RelatedItemEventIncludedDataOutputTypeDef",
     "RelatedItemEventIncludedDataTypeDef",
     "FieldItemOutputTypeDef",
     "FieldItemTypeDef",
     "FieldOptionOutputTypeDef",
     "FieldSummaryTypeDef",
     "FieldValueUnionOutputTypeDef",
     "FieldValueUnionTypeDef",
     "GetCaseEventConfigurationRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
-    "GetDomainResponseTypeDef",
     "GetLayoutRequestRequestTypeDef",
     "GetTemplateRequestRequestTypeDef",
     "LayoutConfigurationOutputTypeDef",
     "RequiredFieldOutputTypeDef",
     "LayoutSummaryTypeDef",
     "ListCasesForContactRequestRequestTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFieldOptionsRequestRequestTypeDef",
     "ListFieldsRequestRequestTypeDef",
     "ListLayoutsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "SortTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFieldRequestRequestTypeDef",
     "BatchGetFieldRequestRequestTypeDef",
     "CaseEventIncludedDataTypeDef",
     "GetCaseRequestRequestTypeDef",
     "BatchGetFieldResponseTypeDef",
+    "CreateCaseResponseTypeDef",
+    "CreateDomainResponseTypeDef",
+    "CreateFieldResponseTypeDef",
+    "CreateLayoutResponseTypeDef",
+    "CreateRelatedItemResponseTypeDef",
+    "CreateTemplateResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetDomainResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "BatchPutFieldOptionsRequestRequestTypeDef",
     "BatchPutFieldOptionsResponseTypeDef",
     "CaseEventIncludedDataOutputTypeDef",
     "ListCasesForContactResponseTypeDef",
     "RelatedItemContentTypeDef",
     "RelatedItemTypeFilterTypeDef",
     "RelatedItemInputContentTypeDef",
@@ -150,58 +150,47 @@
 FieldIdentifierTypeDef = TypedDict(
     "FieldIdentifierTypeDef",
     {
         "id": str,
     },
 )
 
-_RequiredFieldErrorTypeDef = TypedDict(
-    "_RequiredFieldErrorTypeDef",
+FieldErrorTypeDef = TypedDict(
+    "FieldErrorTypeDef",
     {
         "errorCode": str,
         "id": str,
-    },
-)
-_OptionalFieldErrorTypeDef = TypedDict(
-    "_OptionalFieldErrorTypeDef",
-    {
         "message": str,
     },
-    total=False,
 )
 
-
-class FieldErrorTypeDef(_RequiredFieldErrorTypeDef, _OptionalFieldErrorTypeDef):
-    pass
-
-
-_RequiredGetFieldResponseTypeDef = TypedDict(
-    "_RequiredGetFieldResponseTypeDef",
+GetFieldResponseTypeDef = TypedDict(
+    "GetFieldResponseTypeDef",
     {
+        "description": str,
         "fieldArn": str,
         "fieldId": str,
         "name": str,
         "namespace": FieldNamespaceType,
+        "tags": Dict[str, str],
         "type": FieldTypeType,
     },
 )
-_OptionalGetFieldResponseTypeDef = TypedDict(
-    "_OptionalGetFieldResponseTypeDef",
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "description": str,
-        "tags": Dict[str, str],
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-
-class GetFieldResponseTypeDef(_RequiredGetFieldResponseTypeDef, _OptionalGetFieldResponseTypeDef):
-    pass
-
-
 FieldOptionTypeDef = TypedDict(
     "FieldOptionTypeDef",
     {
         "active": bool,
         "name": str,
         "value": str,
     },
@@ -268,40 +257,21 @@
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "contactArn": str,
     },
 )
 
-CreateCaseResponseTypeDef = TypedDict(
-    "CreateCaseResponseTypeDef",
-    {
-        "caseArn": str,
-        "caseId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateDomainRequestRequestTypeDef = TypedDict(
     "CreateDomainRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-CreateDomainResponseTypeDef = TypedDict(
-    "CreateDomainResponseTypeDef",
-    {
-        "domainArn": str,
-        "domainId": str,
-        "domainStatus": DomainStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateFieldRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFieldRequestRequestTypeDef",
     {
         "domainId": str,
         "name": str,
         "type": FieldTypeType,
     },
@@ -317,41 +287,14 @@
 
 class CreateFieldRequestRequestTypeDef(
     _RequiredCreateFieldRequestRequestTypeDef, _OptionalCreateFieldRequestRequestTypeDef
 ):
     pass
 
 
-CreateFieldResponseTypeDef = TypedDict(
-    "CreateFieldResponseTypeDef",
-    {
-        "fieldArn": str,
-        "fieldId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateLayoutResponseTypeDef = TypedDict(
-    "CreateLayoutResponseTypeDef",
-    {
-        "layoutArn": str,
-        "layoutId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateRelatedItemResponseTypeDef = TypedDict(
-    "CreateRelatedItemResponseTypeDef",
-    {
-        "relatedItemArn": str,
-        "relatedItemId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LayoutConfigurationTypeDef = TypedDict(
     "LayoutConfigurationTypeDef",
     {
         "defaultLayout": str,
     },
     total=False,
 )
@@ -359,23 +302,14 @@
 RequiredFieldTypeDef = TypedDict(
     "RequiredFieldTypeDef",
     {
         "fieldId": str,
     },
 )
 
-CreateTemplateResponseTypeDef = TypedDict(
-    "CreateTemplateResponseTypeDef",
-    {
-        "templateArn": str,
-        "templateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 
@@ -384,21 +318,14 @@
     {
         "domainArn": str,
         "domainId": str,
         "name": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RelatedItemEventIncludedDataOutputTypeDef = TypedDict(
     "RelatedItemEventIncludedDataOutputTypeDef",
     {
         "includeContent": bool,
     },
 )
 
@@ -447,15 +374,14 @@
     "FieldValueUnionOutputTypeDef",
     {
         "booleanValue": bool,
         "doubleValue": float,
         "emptyValue": Dict[str, Any],
         "stringValue": str,
     },
-    total=False,
 )
 
 FieldValueUnionTypeDef = TypedDict(
     "FieldValueUnionTypeDef",
     {
         "booleanValue": bool,
         "doubleValue": float,
@@ -475,27 +401,14 @@
 GetDomainRequestRequestTypeDef = TypedDict(
     "GetDomainRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 
-GetDomainResponseTypeDef = TypedDict(
-    "GetDomainResponseTypeDef",
-    {
-        "createdTime": datetime,
-        "domainArn": str,
-        "domainId": str,
-        "domainStatus": DomainStatusType,
-        "name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLayoutRequestRequestTypeDef = TypedDict(
     "GetLayoutRequestRequestTypeDef",
     {
         "domainId": str,
         "layoutId": str,
     },
 )
@@ -509,15 +422,14 @@
 )
 
 LayoutConfigurationOutputTypeDef = TypedDict(
     "LayoutConfigurationOutputTypeDef",
     {
         "defaultLayout": str,
     },
-    total=False,
 )
 
 RequiredFieldOutputTypeDef = TypedDict(
     "RequiredFieldOutputTypeDef",
     {
         "fieldId": str,
     },
@@ -636,22 +548,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListTemplatesRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplatesRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 _OptionalListTemplatesRequestRequestTypeDef = TypedDict(
@@ -687,25 +591,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
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
 SortTypeDef = TypedDict(
     "SortTypeDef",
     {
         "fieldId": str,
         "sortOrder": OrderType,
     },
 )
@@ -788,15 +681,98 @@
 
 
 BatchGetFieldResponseTypeDef = TypedDict(
     "BatchGetFieldResponseTypeDef",
     {
         "errors": List[FieldErrorTypeDef],
         "fields": List[GetFieldResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCaseResponseTypeDef = TypedDict(
+    "CreateCaseResponseTypeDef",
+    {
+        "caseArn": str,
+        "caseId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDomainResponseTypeDef = TypedDict(
+    "CreateDomainResponseTypeDef",
+    {
+        "domainArn": str,
+        "domainId": str,
+        "domainStatus": DomainStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFieldResponseTypeDef = TypedDict(
+    "CreateFieldResponseTypeDef",
+    {
+        "fieldArn": str,
+        "fieldId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLayoutResponseTypeDef = TypedDict(
+    "CreateLayoutResponseTypeDef",
+    {
+        "layoutArn": str,
+        "layoutId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRelatedItemResponseTypeDef = TypedDict(
+    "CreateRelatedItemResponseTypeDef",
+    {
+        "relatedItemArn": str,
+        "relatedItemId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTemplateResponseTypeDef = TypedDict(
+    "CreateTemplateResponseTypeDef",
+    {
+        "templateArn": str,
+        "templateId": str,
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
+GetDomainResponseTypeDef = TypedDict(
+    "GetDomainResponseTypeDef",
+    {
+        "createdTime": datetime,
+        "domainArn": str,
+        "domainId": str,
+        "domainStatus": DomainStatusType,
+        "name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutFieldOptionsRequestRequestTypeDef = TypedDict(
     "BatchPutFieldOptionsRequestRequestTypeDef",
     {
         "domainId": str,
@@ -805,15 +781,15 @@
     },
 )
 
 BatchPutFieldOptionsResponseTypeDef = TypedDict(
     "BatchPutFieldOptionsResponseTypeDef",
     {
         "errors": List[FieldOptionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CaseEventIncludedDataOutputTypeDef = TypedDict(
     "CaseEventIncludedDataOutputTypeDef",
     {
         "fields": List[FieldIdentifierOutputTypeDef],
@@ -821,25 +797,24 @@
 )
 
 ListCasesForContactResponseTypeDef = TypedDict(
     "ListCasesForContactResponseTypeDef",
     {
         "cases": List[CaseSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RelatedItemContentTypeDef = TypedDict(
     "RelatedItemContentTypeDef",
     {
         "comment": CommentContentOutputTypeDef,
         "contact": ContactContentTypeDef,
     },
-    total=False,
 )
 
 RelatedItemTypeFilterTypeDef = TypedDict(
     "RelatedItemTypeFilterTypeDef",
     {
         "comment": Mapping[str, Any],
         "contact": ContactFilterTypeDef,
@@ -908,37 +883,26 @@
 
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFieldGroupOutputTypeDef = TypedDict(
-    "_RequiredFieldGroupOutputTypeDef",
+FieldGroupOutputTypeDef = TypedDict(
+    "FieldGroupOutputTypeDef",
     {
         "fields": List[FieldItemOutputTypeDef],
-    },
-)
-_OptionalFieldGroupOutputTypeDef = TypedDict(
-    "_OptionalFieldGroupOutputTypeDef",
-    {
         "name": str,
     },
-    total=False,
 )
 
-
-class FieldGroupOutputTypeDef(_RequiredFieldGroupOutputTypeDef, _OptionalFieldGroupOutputTypeDef):
-    pass
-
-
 _RequiredFieldGroupTypeDef = TypedDict(
     "_RequiredFieldGroupTypeDef",
     {
         "fields": Sequence[FieldItemTypeDef],
     },
 )
 _OptionalFieldGroupTypeDef = TypedDict(
@@ -955,24 +919,24 @@
 
 
 ListFieldOptionsResponseTypeDef = TypedDict(
     "ListFieldOptionsResponseTypeDef",
     {
         "nextToken": str,
         "options": List[FieldOptionOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFieldsResponseTypeDef = TypedDict(
     "ListFieldsResponseTypeDef",
     {
         "fields": List[FieldSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FieldValueOutputTypeDef = TypedDict(
     "FieldValueOutputTypeDef",
     {
         "id": str,
@@ -995,33 +959,33 @@
         "layoutConfiguration": LayoutConfigurationOutputTypeDef,
         "name": str,
         "requiredFields": List[RequiredFieldOutputTypeDef],
         "status": TemplateStatusType,
         "tags": Dict[str, str],
         "templateArn": str,
         "templateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLayoutsResponseTypeDef = TypedDict(
     "ListLayoutsResponseTypeDef",
     {
         "layouts": List[LayoutSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "templates": List[TemplateSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchCasesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchCasesRequestRequestTypeDef",
     {
         "domainId": str,
@@ -1056,15 +1020,15 @@
 _OptionalSearchCasesRequestSearchCasesPaginateTypeDef = TypedDict(
     "_OptionalSearchCasesRequestSearchCasesPaginateTypeDef",
     {
         "fields": Sequence[FieldIdentifierTypeDef],
         "filter": "CaseFilterTypeDef",
         "searchTerm": str,
         "sorts": Sequence[SortTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchCasesRequestSearchCasesPaginateTypeDef(
     _RequiredSearchCasesRequestSearchCasesPaginateTypeDef,
@@ -1084,41 +1048,27 @@
 
 EventIncludedDataOutputTypeDef = TypedDict(
     "EventIncludedDataOutputTypeDef",
     {
         "caseData": CaseEventIncludedDataOutputTypeDef,
         "relatedItemData": RelatedItemEventIncludedDataOutputTypeDef,
     },
-    total=False,
 )
 
-_RequiredSearchRelatedItemsResponseItemTypeDef = TypedDict(
-    "_RequiredSearchRelatedItemsResponseItemTypeDef",
+SearchRelatedItemsResponseItemTypeDef = TypedDict(
+    "SearchRelatedItemsResponseItemTypeDef",
     {
         "associationTime": datetime,
         "content": RelatedItemContentTypeDef,
         "relatedItemId": str,
-        "type": RelatedItemTypeType,
-    },
-)
-_OptionalSearchRelatedItemsResponseItemTypeDef = TypedDict(
-    "_OptionalSearchRelatedItemsResponseItemTypeDef",
-    {
         "tags": Dict[str, str],
+        "type": RelatedItemTypeType,
     },
-    total=False,
 )
 
-
-class SearchRelatedItemsResponseItemTypeDef(
-    _RequiredSearchRelatedItemsResponseItemTypeDef, _OptionalSearchRelatedItemsResponseItemTypeDef
-):
-    pass
-
-
 _RequiredSearchRelatedItemsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchRelatedItemsRequestRequestTypeDef",
     {
         "caseId": str,
         "domainId": str,
     },
 )
@@ -1147,15 +1097,15 @@
         "domainId": str,
     },
 )
 _OptionalSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef = TypedDict(
     "_OptionalSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     {
         "filters": Sequence[RelatedItemTypeFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef(
     _RequiredSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
@@ -1175,15 +1125,14 @@
 )
 
 SectionOutputTypeDef = TypedDict(
     "SectionOutputTypeDef",
     {
         "fieldGroup": FieldGroupOutputTypeDef,
     },
-    total=False,
 )
 
 SectionTypeDef = TypedDict(
     "SectionTypeDef",
     {
         "fieldGroup": FieldGroupTypeDef,
     },
@@ -1193,41 +1142,28 @@
 GetCaseResponseTypeDef = TypedDict(
     "GetCaseResponseTypeDef",
     {
         "fields": List[FieldValueOutputTypeDef],
         "nextToken": str,
         "tags": Dict[str, str],
         "templateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSearchCasesResponseItemTypeDef = TypedDict(
-    "_RequiredSearchCasesResponseItemTypeDef",
+SearchCasesResponseItemTypeDef = TypedDict(
+    "SearchCasesResponseItemTypeDef",
     {
         "caseId": str,
         "fields": List[FieldValueOutputTypeDef],
-        "templateId": str,
-    },
-)
-_OptionalSearchCasesResponseItemTypeDef = TypedDict(
-    "_OptionalSearchCasesResponseItemTypeDef",
-    {
         "tags": Dict[str, str],
+        "templateId": str,
     },
-    total=False,
 )
 
-
-class SearchCasesResponseItemTypeDef(
-    _RequiredSearchCasesResponseItemTypeDef, _OptionalSearchCasesResponseItemTypeDef
-):
-    pass
-
-
 _RequiredCreateCaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCaseRequestRequestTypeDef",
     {
         "domainId": str,
         "fields": Sequence[FieldValueTypeDef],
         "templateId": str,
     },
@@ -1286,50 +1222,36 @@
 
 class EventBridgeConfigurationTypeDef(
     _RequiredEventBridgeConfigurationTypeDef, _OptionalEventBridgeConfigurationTypeDef
 ):
     pass
 
 
-_RequiredEventBridgeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEventBridgeConfigurationOutputTypeDef",
+EventBridgeConfigurationOutputTypeDef = TypedDict(
+    "EventBridgeConfigurationOutputTypeDef",
     {
         "enabled": bool,
-    },
-)
-_OptionalEventBridgeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEventBridgeConfigurationOutputTypeDef",
-    {
         "includedData": EventIncludedDataOutputTypeDef,
     },
-    total=False,
 )
 
-
-class EventBridgeConfigurationOutputTypeDef(
-    _RequiredEventBridgeConfigurationOutputTypeDef, _OptionalEventBridgeConfigurationOutputTypeDef
-):
-    pass
-
-
 SearchRelatedItemsResponseTypeDef = TypedDict(
     "SearchRelatedItemsResponseTypeDef",
     {
         "nextToken": str,
         "relatedItems": List[SearchRelatedItemsResponseItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LayoutSectionsOutputTypeDef = TypedDict(
     "LayoutSectionsOutputTypeDef",
     {
         "sections": List[SectionOutputTypeDef],
     },
-    total=False,
 )
 
 LayoutSectionsTypeDef = TypedDict(
     "LayoutSectionsTypeDef",
     {
         "sections": Sequence[SectionTypeDef],
     },
@@ -1337,15 +1259,15 @@
 )
 
 SearchCasesResponseTypeDef = TypedDict(
     "SearchCasesResponseTypeDef",
     {
         "cases": List[SearchCasesResponseItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CaseFilterTypeDef = TypedDict(
     "CaseFilterTypeDef",
     {
         "andAll": Sequence[Dict[str, Any]],
@@ -1364,25 +1286,24 @@
     },
 )
 
 GetCaseEventConfigurationResponseTypeDef = TypedDict(
     "GetCaseEventConfigurationResponseTypeDef",
     {
         "eventBridge": EventBridgeConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BasicLayoutOutputTypeDef = TypedDict(
     "BasicLayoutOutputTypeDef",
     {
         "moreInfo": LayoutSectionsOutputTypeDef,
         "topPanel": LayoutSectionsOutputTypeDef,
     },
-    total=False,
 )
 
 BasicLayoutTypeDef = TypedDict(
     "BasicLayoutTypeDef",
     {
         "moreInfo": LayoutSectionsTypeDef,
         "topPanel": LayoutSectionsTypeDef,
@@ -1391,15 +1312,14 @@
 )
 
 LayoutContentOutputTypeDef = TypedDict(
     "LayoutContentOutputTypeDef",
     {
         "basic": BasicLayoutOutputTypeDef,
     },
-    total=False,
 )
 
 LayoutContentTypeDef = TypedDict(
     "LayoutContentTypeDef",
     {
         "basic": BasicLayoutTypeDef,
     },
@@ -1410,15 +1330,15 @@
     "GetLayoutResponseTypeDef",
     {
         "content": LayoutContentOutputTypeDef,
         "layoutArn": str,
         "layoutId": str,
         "name": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLayoutRequestRequestTypeDef = TypedDict(
     "CreateLayoutRequestRequestTypeDef",
     {
         "content": LayoutContentTypeDef,
```

### Comparing `mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases/type_defs.pyi` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -33,71 +33,71 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "FieldIdentifierTypeDef",
     "FieldErrorTypeDef",
     "GetFieldResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "FieldOptionTypeDef",
     "FieldOptionErrorTypeDef",
     "FieldIdentifierOutputTypeDef",
     "CaseSummaryTypeDef",
     "CommentContentOutputTypeDef",
     "CommentContentTypeDef",
     "ContactContentTypeDef",
     "ContactFilterTypeDef",
     "ContactTypeDef",
-    "CreateCaseResponseTypeDef",
     "CreateDomainRequestRequestTypeDef",
-    "CreateDomainResponseTypeDef",
     "CreateFieldRequestRequestTypeDef",
-    "CreateFieldResponseTypeDef",
-    "CreateLayoutResponseTypeDef",
-    "CreateRelatedItemResponseTypeDef",
     "LayoutConfigurationTypeDef",
     "RequiredFieldTypeDef",
-    "CreateTemplateResponseTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DomainSummaryTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "RelatedItemEventIncludedDataOutputTypeDef",
     "RelatedItemEventIncludedDataTypeDef",
     "FieldItemOutputTypeDef",
     "FieldItemTypeDef",
     "FieldOptionOutputTypeDef",
     "FieldSummaryTypeDef",
     "FieldValueUnionOutputTypeDef",
     "FieldValueUnionTypeDef",
     "GetCaseEventConfigurationRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
-    "GetDomainResponseTypeDef",
     "GetLayoutRequestRequestTypeDef",
     "GetTemplateRequestRequestTypeDef",
     "LayoutConfigurationOutputTypeDef",
     "RequiredFieldOutputTypeDef",
     "LayoutSummaryTypeDef",
     "ListCasesForContactRequestRequestTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFieldOptionsRequestRequestTypeDef",
     "ListFieldsRequestRequestTypeDef",
     "ListLayoutsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "SortTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFieldRequestRequestTypeDef",
     "BatchGetFieldRequestRequestTypeDef",
     "CaseEventIncludedDataTypeDef",
     "GetCaseRequestRequestTypeDef",
     "BatchGetFieldResponseTypeDef",
+    "CreateCaseResponseTypeDef",
+    "CreateDomainResponseTypeDef",
+    "CreateFieldResponseTypeDef",
+    "CreateLayoutResponseTypeDef",
+    "CreateRelatedItemResponseTypeDef",
+    "CreateTemplateResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetDomainResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "BatchPutFieldOptionsRequestRequestTypeDef",
     "BatchPutFieldOptionsResponseTypeDef",
     "CaseEventIncludedDataOutputTypeDef",
     "ListCasesForContactResponseTypeDef",
     "RelatedItemContentTypeDef",
     "RelatedItemTypeFilterTypeDef",
     "RelatedItemInputContentTypeDef",
@@ -149,54 +149,47 @@
 FieldIdentifierTypeDef = TypedDict(
     "FieldIdentifierTypeDef",
     {
         "id": str,
     },
 )
 
-_RequiredFieldErrorTypeDef = TypedDict(
-    "_RequiredFieldErrorTypeDef",
+FieldErrorTypeDef = TypedDict(
+    "FieldErrorTypeDef",
     {
         "errorCode": str,
         "id": str,
-    },
-)
-_OptionalFieldErrorTypeDef = TypedDict(
-    "_OptionalFieldErrorTypeDef",
-    {
         "message": str,
     },
-    total=False,
 )
 
-class FieldErrorTypeDef(_RequiredFieldErrorTypeDef, _OptionalFieldErrorTypeDef):
-    pass
-
-_RequiredGetFieldResponseTypeDef = TypedDict(
-    "_RequiredGetFieldResponseTypeDef",
+GetFieldResponseTypeDef = TypedDict(
+    "GetFieldResponseTypeDef",
     {
+        "description": str,
         "fieldArn": str,
         "fieldId": str,
         "name": str,
         "namespace": FieldNamespaceType,
+        "tags": Dict[str, str],
         "type": FieldTypeType,
     },
 )
-_OptionalGetFieldResponseTypeDef = TypedDict(
-    "_OptionalGetFieldResponseTypeDef",
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "description": str,
-        "tags": Dict[str, str],
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-class GetFieldResponseTypeDef(_RequiredGetFieldResponseTypeDef, _OptionalGetFieldResponseTypeDef):
-    pass
-
 FieldOptionTypeDef = TypedDict(
     "FieldOptionTypeDef",
     {
         "active": bool,
         "name": str,
         "value": str,
     },
@@ -263,40 +256,21 @@
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "contactArn": str,
     },
 )
 
-CreateCaseResponseTypeDef = TypedDict(
-    "CreateCaseResponseTypeDef",
-    {
-        "caseArn": str,
-        "caseId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateDomainRequestRequestTypeDef = TypedDict(
     "CreateDomainRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-CreateDomainResponseTypeDef = TypedDict(
-    "CreateDomainResponseTypeDef",
-    {
-        "domainArn": str,
-        "domainId": str,
-        "domainStatus": DomainStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateFieldRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFieldRequestRequestTypeDef",
     {
         "domainId": str,
         "name": str,
         "type": FieldTypeType,
     },
@@ -310,41 +284,14 @@
 )
 
 class CreateFieldRequestRequestTypeDef(
     _RequiredCreateFieldRequestRequestTypeDef, _OptionalCreateFieldRequestRequestTypeDef
 ):
     pass
 
-CreateFieldResponseTypeDef = TypedDict(
-    "CreateFieldResponseTypeDef",
-    {
-        "fieldArn": str,
-        "fieldId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateLayoutResponseTypeDef = TypedDict(
-    "CreateLayoutResponseTypeDef",
-    {
-        "layoutArn": str,
-        "layoutId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateRelatedItemResponseTypeDef = TypedDict(
-    "CreateRelatedItemResponseTypeDef",
-    {
-        "relatedItemArn": str,
-        "relatedItemId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LayoutConfigurationTypeDef = TypedDict(
     "LayoutConfigurationTypeDef",
     {
         "defaultLayout": str,
     },
     total=False,
 )
@@ -352,23 +299,14 @@
 RequiredFieldTypeDef = TypedDict(
     "RequiredFieldTypeDef",
     {
         "fieldId": str,
     },
 )
 
-CreateTemplateResponseTypeDef = TypedDict(
-    "CreateTemplateResponseTypeDef",
-    {
-        "templateArn": str,
-        "templateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 
@@ -377,21 +315,14 @@
     {
         "domainArn": str,
         "domainId": str,
         "name": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RelatedItemEventIncludedDataOutputTypeDef = TypedDict(
     "RelatedItemEventIncludedDataOutputTypeDef",
     {
         "includeContent": bool,
     },
 )
 
@@ -440,15 +371,14 @@
     "FieldValueUnionOutputTypeDef",
     {
         "booleanValue": bool,
         "doubleValue": float,
         "emptyValue": Dict[str, Any],
         "stringValue": str,
     },
-    total=False,
 )
 
 FieldValueUnionTypeDef = TypedDict(
     "FieldValueUnionTypeDef",
     {
         "booleanValue": bool,
         "doubleValue": float,
@@ -468,27 +398,14 @@
 GetDomainRequestRequestTypeDef = TypedDict(
     "GetDomainRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 
-GetDomainResponseTypeDef = TypedDict(
-    "GetDomainResponseTypeDef",
-    {
-        "createdTime": datetime,
-        "domainArn": str,
-        "domainId": str,
-        "domainStatus": DomainStatusType,
-        "name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLayoutRequestRequestTypeDef = TypedDict(
     "GetLayoutRequestRequestTypeDef",
     {
         "domainId": str,
         "layoutId": str,
     },
 )
@@ -502,15 +419,14 @@
 )
 
 LayoutConfigurationOutputTypeDef = TypedDict(
     "LayoutConfigurationOutputTypeDef",
     {
         "defaultLayout": str,
     },
-    total=False,
 )
 
 RequiredFieldOutputTypeDef = TypedDict(
     "RequiredFieldOutputTypeDef",
     {
         "fieldId": str,
     },
@@ -621,22 +537,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListTemplatesRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplatesRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 _OptionalListTemplatesRequestRequestTypeDef = TypedDict(
@@ -670,25 +578,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
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
 SortTypeDef = TypedDict(
     "SortTypeDef",
     {
         "fieldId": str,
         "sortOrder": OrderType,
     },
 )
@@ -767,15 +664,98 @@
     pass
 
 BatchGetFieldResponseTypeDef = TypedDict(
     "BatchGetFieldResponseTypeDef",
     {
         "errors": List[FieldErrorTypeDef],
         "fields": List[GetFieldResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCaseResponseTypeDef = TypedDict(
+    "CreateCaseResponseTypeDef",
+    {
+        "caseArn": str,
+        "caseId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDomainResponseTypeDef = TypedDict(
+    "CreateDomainResponseTypeDef",
+    {
+        "domainArn": str,
+        "domainId": str,
+        "domainStatus": DomainStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFieldResponseTypeDef = TypedDict(
+    "CreateFieldResponseTypeDef",
+    {
+        "fieldArn": str,
+        "fieldId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLayoutResponseTypeDef = TypedDict(
+    "CreateLayoutResponseTypeDef",
+    {
+        "layoutArn": str,
+        "layoutId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRelatedItemResponseTypeDef = TypedDict(
+    "CreateRelatedItemResponseTypeDef",
+    {
+        "relatedItemArn": str,
+        "relatedItemId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTemplateResponseTypeDef = TypedDict(
+    "CreateTemplateResponseTypeDef",
+    {
+        "templateArn": str,
+        "templateId": str,
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
+GetDomainResponseTypeDef = TypedDict(
+    "GetDomainResponseTypeDef",
+    {
+        "createdTime": datetime,
+        "domainArn": str,
+        "domainId": str,
+        "domainStatus": DomainStatusType,
+        "name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutFieldOptionsRequestRequestTypeDef = TypedDict(
     "BatchPutFieldOptionsRequestRequestTypeDef",
     {
         "domainId": str,
@@ -784,15 +764,15 @@
     },
 )
 
 BatchPutFieldOptionsResponseTypeDef = TypedDict(
     "BatchPutFieldOptionsResponseTypeDef",
     {
         "errors": List[FieldOptionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CaseEventIncludedDataOutputTypeDef = TypedDict(
     "CaseEventIncludedDataOutputTypeDef",
     {
         "fields": List[FieldIdentifierOutputTypeDef],
@@ -800,25 +780,24 @@
 )
 
 ListCasesForContactResponseTypeDef = TypedDict(
     "ListCasesForContactResponseTypeDef",
     {
         "cases": List[CaseSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RelatedItemContentTypeDef = TypedDict(
     "RelatedItemContentTypeDef",
     {
         "comment": CommentContentOutputTypeDef,
         "contact": ContactContentTypeDef,
     },
-    total=False,
 )
 
 RelatedItemTypeFilterTypeDef = TypedDict(
     "RelatedItemTypeFilterTypeDef",
     {
         "comment": Mapping[str, Any],
         "contact": ContactFilterTypeDef,
@@ -883,35 +862,26 @@
     pass
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFieldGroupOutputTypeDef = TypedDict(
-    "_RequiredFieldGroupOutputTypeDef",
+FieldGroupOutputTypeDef = TypedDict(
+    "FieldGroupOutputTypeDef",
     {
         "fields": List[FieldItemOutputTypeDef],
-    },
-)
-_OptionalFieldGroupOutputTypeDef = TypedDict(
-    "_OptionalFieldGroupOutputTypeDef",
-    {
         "name": str,
     },
-    total=False,
 )
 
-class FieldGroupOutputTypeDef(_RequiredFieldGroupOutputTypeDef, _OptionalFieldGroupOutputTypeDef):
-    pass
-
 _RequiredFieldGroupTypeDef = TypedDict(
     "_RequiredFieldGroupTypeDef",
     {
         "fields": Sequence[FieldItemTypeDef],
     },
 )
 _OptionalFieldGroupTypeDef = TypedDict(
@@ -926,24 +896,24 @@
     pass
 
 ListFieldOptionsResponseTypeDef = TypedDict(
     "ListFieldOptionsResponseTypeDef",
     {
         "nextToken": str,
         "options": List[FieldOptionOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFieldsResponseTypeDef = TypedDict(
     "ListFieldsResponseTypeDef",
     {
         "fields": List[FieldSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FieldValueOutputTypeDef = TypedDict(
     "FieldValueOutputTypeDef",
     {
         "id": str,
@@ -966,33 +936,33 @@
         "layoutConfiguration": LayoutConfigurationOutputTypeDef,
         "name": str,
         "requiredFields": List[RequiredFieldOutputTypeDef],
         "status": TemplateStatusType,
         "tags": Dict[str, str],
         "templateArn": str,
         "templateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLayoutsResponseTypeDef = TypedDict(
     "ListLayoutsResponseTypeDef",
     {
         "layouts": List[LayoutSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "templates": List[TemplateSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchCasesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchCasesRequestRequestTypeDef",
     {
         "domainId": str,
@@ -1025,15 +995,15 @@
 _OptionalSearchCasesRequestSearchCasesPaginateTypeDef = TypedDict(
     "_OptionalSearchCasesRequestSearchCasesPaginateTypeDef",
     {
         "fields": Sequence[FieldIdentifierTypeDef],
         "filter": "CaseFilterTypeDef",
         "searchTerm": str,
         "sorts": Sequence[SortTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchCasesRequestSearchCasesPaginateTypeDef(
     _RequiredSearchCasesRequestSearchCasesPaginateTypeDef,
     _OptionalSearchCasesRequestSearchCasesPaginateTypeDef,
@@ -1051,39 +1021,27 @@
 
 EventIncludedDataOutputTypeDef = TypedDict(
     "EventIncludedDataOutputTypeDef",
     {
         "caseData": CaseEventIncludedDataOutputTypeDef,
         "relatedItemData": RelatedItemEventIncludedDataOutputTypeDef,
     },
-    total=False,
 )
 
-_RequiredSearchRelatedItemsResponseItemTypeDef = TypedDict(
-    "_RequiredSearchRelatedItemsResponseItemTypeDef",
+SearchRelatedItemsResponseItemTypeDef = TypedDict(
+    "SearchRelatedItemsResponseItemTypeDef",
     {
         "associationTime": datetime,
         "content": RelatedItemContentTypeDef,
         "relatedItemId": str,
-        "type": RelatedItemTypeType,
-    },
-)
-_OptionalSearchRelatedItemsResponseItemTypeDef = TypedDict(
-    "_OptionalSearchRelatedItemsResponseItemTypeDef",
-    {
         "tags": Dict[str, str],
+        "type": RelatedItemTypeType,
     },
-    total=False,
 )
 
-class SearchRelatedItemsResponseItemTypeDef(
-    _RequiredSearchRelatedItemsResponseItemTypeDef, _OptionalSearchRelatedItemsResponseItemTypeDef
-):
-    pass
-
 _RequiredSearchRelatedItemsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchRelatedItemsRequestRequestTypeDef",
     {
         "caseId": str,
         "domainId": str,
     },
 )
@@ -1110,15 +1068,15 @@
         "domainId": str,
     },
 )
 _OptionalSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef = TypedDict(
     "_OptionalSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     {
         "filters": Sequence[RelatedItemTypeFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef(
     _RequiredSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
     _OptionalSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
@@ -1136,15 +1094,14 @@
 )
 
 SectionOutputTypeDef = TypedDict(
     "SectionOutputTypeDef",
     {
         "fieldGroup": FieldGroupOutputTypeDef,
     },
-    total=False,
 )
 
 SectionTypeDef = TypedDict(
     "SectionTypeDef",
     {
         "fieldGroup": FieldGroupTypeDef,
     },
@@ -1154,39 +1111,28 @@
 GetCaseResponseTypeDef = TypedDict(
     "GetCaseResponseTypeDef",
     {
         "fields": List[FieldValueOutputTypeDef],
         "nextToken": str,
         "tags": Dict[str, str],
         "templateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSearchCasesResponseItemTypeDef = TypedDict(
-    "_RequiredSearchCasesResponseItemTypeDef",
+SearchCasesResponseItemTypeDef = TypedDict(
+    "SearchCasesResponseItemTypeDef",
     {
         "caseId": str,
         "fields": List[FieldValueOutputTypeDef],
-        "templateId": str,
-    },
-)
-_OptionalSearchCasesResponseItemTypeDef = TypedDict(
-    "_OptionalSearchCasesResponseItemTypeDef",
-    {
         "tags": Dict[str, str],
+        "templateId": str,
     },
-    total=False,
 )
 
-class SearchCasesResponseItemTypeDef(
-    _RequiredSearchCasesResponseItemTypeDef, _OptionalSearchCasesResponseItemTypeDef
-):
-    pass
-
 _RequiredCreateCaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCaseRequestRequestTypeDef",
     {
         "domainId": str,
         "fields": Sequence[FieldValueTypeDef],
         "templateId": str,
     },
@@ -1241,48 +1187,36 @@
 )
 
 class EventBridgeConfigurationTypeDef(
     _RequiredEventBridgeConfigurationTypeDef, _OptionalEventBridgeConfigurationTypeDef
 ):
     pass
 
-_RequiredEventBridgeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEventBridgeConfigurationOutputTypeDef",
+EventBridgeConfigurationOutputTypeDef = TypedDict(
+    "EventBridgeConfigurationOutputTypeDef",
     {
         "enabled": bool,
-    },
-)
-_OptionalEventBridgeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEventBridgeConfigurationOutputTypeDef",
-    {
         "includedData": EventIncludedDataOutputTypeDef,
     },
-    total=False,
 )
 
-class EventBridgeConfigurationOutputTypeDef(
-    _RequiredEventBridgeConfigurationOutputTypeDef, _OptionalEventBridgeConfigurationOutputTypeDef
-):
-    pass
-
 SearchRelatedItemsResponseTypeDef = TypedDict(
     "SearchRelatedItemsResponseTypeDef",
     {
         "nextToken": str,
         "relatedItems": List[SearchRelatedItemsResponseItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LayoutSectionsOutputTypeDef = TypedDict(
     "LayoutSectionsOutputTypeDef",
     {
         "sections": List[SectionOutputTypeDef],
     },
-    total=False,
 )
 
 LayoutSectionsTypeDef = TypedDict(
     "LayoutSectionsTypeDef",
     {
         "sections": Sequence[SectionTypeDef],
     },
@@ -1290,15 +1224,15 @@
 )
 
 SearchCasesResponseTypeDef = TypedDict(
     "SearchCasesResponseTypeDef",
     {
         "cases": List[SearchCasesResponseItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CaseFilterTypeDef = TypedDict(
     "CaseFilterTypeDef",
     {
         "andAll": Sequence[Dict[str, Any]],
@@ -1317,25 +1251,24 @@
     },
 )
 
 GetCaseEventConfigurationResponseTypeDef = TypedDict(
     "GetCaseEventConfigurationResponseTypeDef",
     {
         "eventBridge": EventBridgeConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BasicLayoutOutputTypeDef = TypedDict(
     "BasicLayoutOutputTypeDef",
     {
         "moreInfo": LayoutSectionsOutputTypeDef,
         "topPanel": LayoutSectionsOutputTypeDef,
     },
-    total=False,
 )
 
 BasicLayoutTypeDef = TypedDict(
     "BasicLayoutTypeDef",
     {
         "moreInfo": LayoutSectionsTypeDef,
         "topPanel": LayoutSectionsTypeDef,
@@ -1344,15 +1277,14 @@
 )
 
 LayoutContentOutputTypeDef = TypedDict(
     "LayoutContentOutputTypeDef",
     {
         "basic": BasicLayoutOutputTypeDef,
     },
-    total=False,
 )
 
 LayoutContentTypeDef = TypedDict(
     "LayoutContentTypeDef",
     {
         "basic": BasicLayoutTypeDef,
     },
@@ -1363,15 +1295,15 @@
     "GetLayoutResponseTypeDef",
     {
         "content": LayoutContentOutputTypeDef,
         "layoutArn": str,
         "layoutId": str,
         "name": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLayoutRequestRequestTypeDef = TypedDict(
     "CreateLayoutRequestRequestTypeDef",
     {
         "content": LayoutContentTypeDef,
```

### Comparing `mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases.egg-info/PKG-INFO` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcases
-Version: 1.28.12
-Summary: Type annotations for boto3.ConnectCases 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.8
+Summary: Type annotations for boto3.ConnectCases 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-connectcases"></a>
 
 # mypy-boto3-connectcases
 
 [![PyPI - mypy-boto3-connectcases](https://img.shields.io/pypi/v/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcases)](https://pepy.tech/project/mypy-boto3-connectcases)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcases?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connectcases docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,71 +333,71 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connectcases.type_defs import (
     FieldIdentifierTypeDef,
     FieldErrorTypeDef,
     GetFieldResponseTypeDef,
+    ResponseMetadataTypeDef,
     FieldOptionTypeDef,
     FieldOptionErrorTypeDef,
     FieldIdentifierOutputTypeDef,
     CaseSummaryTypeDef,
     CommentContentOutputTypeDef,
     CommentContentTypeDef,
     ContactContentTypeDef,
     ContactFilterTypeDef,
     ContactTypeDef,
-    CreateCaseResponseTypeDef,
     CreateDomainRequestRequestTypeDef,
-    CreateDomainResponseTypeDef,
     CreateFieldRequestRequestTypeDef,
-    CreateFieldResponseTypeDef,
-    CreateLayoutResponseTypeDef,
-    CreateRelatedItemResponseTypeDef,
     LayoutConfigurationTypeDef,
     RequiredFieldTypeDef,
-    CreateTemplateResponseTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
     RelatedItemEventIncludedDataOutputTypeDef,
     RelatedItemEventIncludedDataTypeDef,
     FieldItemOutputTypeDef,
     FieldItemTypeDef,
     FieldOptionOutputTypeDef,
     FieldSummaryTypeDef,
     FieldValueUnionOutputTypeDef,
     FieldValueUnionTypeDef,
     GetCaseEventConfigurationRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
-    GetDomainResponseTypeDef,
     GetLayoutRequestRequestTypeDef,
     GetTemplateRequestRequestTypeDef,
     LayoutConfigurationOutputTypeDef,
     RequiredFieldOutputTypeDef,
     LayoutSummaryTypeDef,
     ListCasesForContactRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFieldOptionsRequestRequestTypeDef,
     ListFieldsRequestRequestTypeDef,
     ListLayoutsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SortTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFieldRequestRequestTypeDef,
     BatchGetFieldRequestRequestTypeDef,
     CaseEventIncludedDataTypeDef,
     GetCaseRequestRequestTypeDef,
     BatchGetFieldResponseTypeDef,
+    CreateCaseResponseTypeDef,
+    CreateDomainResponseTypeDef,
+    CreateFieldResponseTypeDef,
+    CreateLayoutResponseTypeDef,
+    CreateRelatedItemResponseTypeDef,
+    CreateTemplateResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDomainResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     BatchPutFieldOptionsRequestRequestTypeDef,
     BatchPutFieldOptionsResponseTypeDef,
     CaseEventIncludedDataOutputTypeDef,
     ListCasesForContactResponseTypeDef,
     RelatedItemContentTypeDef,
     RelatedItemTypeFilterTypeDef,
     RelatedItemInputContentTypeDef,
```

### Comparing `mypy-boto3-connectcases-1.28.12/mypy_boto3_connectcases.egg-info/SOURCES.txt` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.12/setup.py` & `mypy-boto3-connectcases-1.28.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connectcases",
-    version="1.28.12",
+    version="1.28.8",
     packages=["mypy_boto3_connectcases"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConnectCases 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.ConnectCases 1.28.8 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

