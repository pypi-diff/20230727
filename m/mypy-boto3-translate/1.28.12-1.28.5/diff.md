# Comparing `tmp/mypy-boto3-translate-1.28.12.tar.gz` & `tmp/mypy-boto3-translate-1.28.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-translate-1.28.12.tar", last modified: Thu Jul 27 11:49:47 2023, max compression
+gzip compressed data, was "mypy-boto3-translate-1.28.5.tar", last modified: Tue Jul 18 19:32:41 2023, max compression
```

## Comparing `mypy-boto3-translate-1.28.12.tar` & `mypy-boto3-translate-1.28.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:47.153460 mypy-boto3-translate-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:12.000000 mypy-boto3-translate-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15190 2023-07-27 11:49:47.145460 mypy-boto3-translate-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-07-27 11:48:12.000000 mypy-boto3-translate-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:47.145460 mypy-boto3-translate-1.28.12/mypy_boto3_translate/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-27 11:48:12.000000 mypy-boto3-translate-1.28.12/mypy_boto3_translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-27 11:48:12.000000 mypy-boto3-translate-1.28.12/mypy_boto3_translate/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 11:48:12.000000 mypy-boto3-translate-1.28.12/mypy_boto3_translate/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-07-27 11:48:12.000000 mypy-boto3-translate-1.28.12/mypy_boto3_translate/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-07-27 11:48:12.000000 mypy-boto3-translate-1.28.12/mypy_boto3_translate/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-07-27 11:48:12.000000 mypy-boto3-translate-1.28.12/mypy_boto3_translate/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-07-27 11:48:12.000000 mypy-boto3-translate-1.28.12/mypy_boto3_translate/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-27 11:48:12.000000 mypy-boto3-translate-1.28.12/mypy_boto3_translate/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-27 11:48:12.000000 mypy-boto3-translate-1.28.12/mypy_boto3_translate/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:12.000000 mypy-boto3-translate-1.28.12/mypy_boto3_translate/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21592 2023-07-27 11:48:13.000000 mypy-boto3-translate-1.28.12/mypy_boto3_translate/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21571 2023-07-27 11:48:13.000000 mypy-boto3-translate-1.28.12/mypy_boto3_translate/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:12.000000 mypy-boto3-translate-1.28.12/mypy_boto3_translate/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:47.145460 mypy-boto3-translate-1.28.12/mypy_boto3_translate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15190 2023-07-27 11:49:46.000000 mypy-boto3-translate-1.28.12/mypy_boto3_translate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 11:49:46.000000 mypy-boto3-translate-1.28.12/mypy_boto3_translate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-translate-1.28.12/mypy_boto3_translate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-translate-1.28.12/mypy_boto3_translate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:46.000000 mypy-boto3-translate-1.28.12/mypy_boto3_translate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 11:49:46.000000 mypy-boto3-translate-1.28.12/mypy_boto3_translate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:47.153460 mypy-boto3-translate-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 11:48:12.000000 mypy-boto3-translate-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.774719 mypy-boto3-translate-1.28.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-07-18 19:32:41.774719 mypy-boto3-translate-1.28.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13710 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.766719 mypy-boto3-translate-1.28.5/mypy_boto3_translate/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21226 2023-07-18 19:32:30.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21207 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.774719 mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-07-18 19:32:41.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-18 19:32:41.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 19:32:41.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 19:32:41.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:32:41.774719 mypy-boto3-translate-1.28.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/setup.py
```

### Comparing `mypy-boto3-translate-1.28.12/LICENSE` & `mypy-boto3-translate-1.28.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.12/PKG-INFO` & `mypy-boto3-translate-1.28.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-translate
-Version: 1.28.12
-Summary: Type annotations for boto3.Translate 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.5
+Summary: Type annotations for boto3.Translate 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-translate"></a>
 
 # mypy-boto3-translate
 
 [![PyPI - mypy-boto3-translate](https://img.shields.io/pypi/v/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-translate)](https://pepy.tech/project/mypy-boto3-translate)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-translate?color=blue)](https://pypistats.org/packages/mypy-boto3-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Translate 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
+[boto3.Translate 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
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
 [mypy-boto3-translate docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,59 +334,59 @@
 
 ```python
 from mypy_boto3_translate.type_defs import (
     TermTypeDef,
     EncryptionKeyTypeDef,
     ParallelDataConfigTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateParallelDataResponseTypeDef,
     DeleteParallelDataRequestRequestTypeDef,
+    DeleteParallelDataResponseTypeDef,
     DeleteTerminologyRequestRequestTypeDef,
     DescribeTextTranslationJobRequestRequestTypeDef,
     DocumentTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionKeyOutputTypeDef,
     GetParallelDataRequestRequestTypeDef,
     ParallelDataDataLocationTypeDef,
     GetTerminologyRequestRequestTypeDef,
     TerminologyDataLocationTypeDef,
     TerminologyDataTypeDef,
     InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
     JobDetailsTypeDef,
     LanguageTypeDef,
     ListLanguagesRequestRequestTypeDef,
     ListParallelDataRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagOutputTypeDef,
-    PaginatorConfigTypeDef,
+    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     ListTerminologiesRequestRequestTypeDef,
     TextTranslationJobFilterTypeDef,
+    PaginatorConfigTypeDef,
     ParallelDataConfigOutputTypeDef,
+    ResponseMetadataTypeDef,
     TranslationSettingsTypeDef,
+    StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobRequestRequestTypeDef,
+    StopTextTranslationJobResponseTypeDef,
     TranslationSettingsOutputTypeDef,
     TranslatedDocumentTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateParallelDataResponseTypeDef,
     AppliedTerminologyTypeDef,
     OutputDataConfigTypeDef,
     UpdateParallelDataRequestRequestTypeDef,
     CreateParallelDataRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateParallelDataResponseTypeDef,
-    DeleteParallelDataResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    StartTextTranslationJobResponseTypeDef,
-    StopTextTranslationJobResponseTypeDef,
-    UpdateParallelDataResponseTypeDef,
     OutputDataConfigOutputTypeDef,
     TerminologyPropertiesTypeDef,
     ImportTerminologyRequestRequestTypeDef,
     ListLanguagesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     ListTextTranslationJobsRequestRequestTypeDef,
     ParallelDataPropertiesTypeDef,
     TranslateDocumentRequestRequestTypeDef,
     TranslateTextRequestRequestTypeDef,
     TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
     StartTextTranslationJobRequestRequestTypeDef,
```

### Comparing `mypy-boto3-translate-1.28.12/README.md` & `mypy-boto3-translate-1.28.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-translate"></a>
 
 # mypy-boto3-translate
 
 [![PyPI - mypy-boto3-translate](https://img.shields.io/pypi/v/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-translate)](https://pepy.tech/project/mypy-boto3-translate)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-translate?color=blue)](https://pypistats.org/packages/mypy-boto3-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Translate 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
+[boto3.Translate 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
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
 [mypy-boto3-translate docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,59 +302,59 @@
 
 ```python
 from mypy_boto3_translate.type_defs import (
     TermTypeDef,
     EncryptionKeyTypeDef,
     ParallelDataConfigTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateParallelDataResponseTypeDef,
     DeleteParallelDataRequestRequestTypeDef,
+    DeleteParallelDataResponseTypeDef,
     DeleteTerminologyRequestRequestTypeDef,
     DescribeTextTranslationJobRequestRequestTypeDef,
     DocumentTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionKeyOutputTypeDef,
     GetParallelDataRequestRequestTypeDef,
     ParallelDataDataLocationTypeDef,
     GetTerminologyRequestRequestTypeDef,
     TerminologyDataLocationTypeDef,
     TerminologyDataTypeDef,
     InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
     JobDetailsTypeDef,
     LanguageTypeDef,
     ListLanguagesRequestRequestTypeDef,
     ListParallelDataRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagOutputTypeDef,
-    PaginatorConfigTypeDef,
+    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     ListTerminologiesRequestRequestTypeDef,
     TextTranslationJobFilterTypeDef,
+    PaginatorConfigTypeDef,
     ParallelDataConfigOutputTypeDef,
+    ResponseMetadataTypeDef,
     TranslationSettingsTypeDef,
+    StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobRequestRequestTypeDef,
+    StopTextTranslationJobResponseTypeDef,
     TranslationSettingsOutputTypeDef,
     TranslatedDocumentTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateParallelDataResponseTypeDef,
     AppliedTerminologyTypeDef,
     OutputDataConfigTypeDef,
     UpdateParallelDataRequestRequestTypeDef,
     CreateParallelDataRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateParallelDataResponseTypeDef,
-    DeleteParallelDataResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    StartTextTranslationJobResponseTypeDef,
-    StopTextTranslationJobResponseTypeDef,
-    UpdateParallelDataResponseTypeDef,
     OutputDataConfigOutputTypeDef,
     TerminologyPropertiesTypeDef,
     ImportTerminologyRequestRequestTypeDef,
     ListLanguagesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     ListTextTranslationJobsRequestRequestTypeDef,
     ParallelDataPropertiesTypeDef,
     TranslateDocumentRequestRequestTypeDef,
     TranslateTextRequestRequestTypeDef,
     TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
     StartTextTranslationJobRequestRequestTypeDef,
```

### Comparing `mypy-boto3-translate-1.28.12/mypy_boto3_translate/__init__.py` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.12/mypy_boto3_translate/__init__.pyi` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.12/mypy_boto3_translate/__main__.py` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Translate 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Translate 1.28.5\nVersion:         1.28.5\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.5")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-translate-1.28.12/mypy_boto3_translate/client.py` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.12/mypy_boto3_translate/client.pyi` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.12/mypy_boto3_translate/literals.py` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,15 +174,14 @@
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
@@ -261,28 +260,26 @@
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
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-translate-1.28.12/mypy_boto3_translate/literals.pyi` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,14 @@
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
@@ -259,28 +258,26 @@
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
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-translate-1.28.12/mypy_boto3_translate/paginator.py` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListTerminologiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Paginator.ListTerminologies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/paginators/#listterminologiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTerminologiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Paginator.ListTerminologies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/paginators/#listterminologiespaginator)
         """
```

### Comparing `mypy-boto3-translate-1.28.12/mypy_boto3_translate/paginator.pyi` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListTerminologiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Paginator.ListTerminologies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/paginators/#listterminologiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTerminologiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Paginator.ListTerminologies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/paginators/#listterminologiespaginator)
         """
```

### Comparing `mypy-boto3-translate-1.28.12/mypy_boto3_translate/type_defs.py` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -32,65 +32,64 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TermTypeDef",
     "EncryptionKeyTypeDef",
     "ParallelDataConfigTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateParallelDataResponseTypeDef",
     "DeleteParallelDataRequestRequestTypeDef",
+    "DeleteParallelDataResponseTypeDef",
     "DeleteTerminologyRequestRequestTypeDef",
     "DescribeTextTranslationJobRequestRequestTypeDef",
     "DocumentTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EncryptionKeyOutputTypeDef",
     "GetParallelDataRequestRequestTypeDef",
     "ParallelDataDataLocationTypeDef",
     "GetTerminologyRequestRequestTypeDef",
     "TerminologyDataLocationTypeDef",
     "TerminologyDataTypeDef",
     "InputDataConfigOutputTypeDef",
     "InputDataConfigTypeDef",
     "JobDetailsTypeDef",
     "LanguageTypeDef",
     "ListLanguagesRequestRequestTypeDef",
     "ListParallelDataRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagOutputTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     "ListTerminologiesRequestRequestTypeDef",
     "TextTranslationJobFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "ParallelDataConfigOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "TranslationSettingsTypeDef",
+    "StartTextTranslationJobResponseTypeDef",
     "StopTextTranslationJobRequestRequestTypeDef",
+    "StopTextTranslationJobResponseTypeDef",
     "TranslationSettingsOutputTypeDef",
     "TranslatedDocumentTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateParallelDataResponseTypeDef",
     "AppliedTerminologyTypeDef",
     "OutputDataConfigTypeDef",
     "UpdateParallelDataRequestRequestTypeDef",
     "CreateParallelDataRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "CreateParallelDataResponseTypeDef",
-    "DeleteParallelDataResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "StartTextTranslationJobResponseTypeDef",
-    "StopTextTranslationJobResponseTypeDef",
-    "UpdateParallelDataResponseTypeDef",
     "OutputDataConfigOutputTypeDef",
     "TerminologyPropertiesTypeDef",
     "ImportTerminologyRequestRequestTypeDef",
     "ListLanguagesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     "ListTextTranslationJobsRequestRequestTypeDef",
     "ParallelDataPropertiesTypeDef",
     "TranslateDocumentRequestRequestTypeDef",
     "TranslateTextRequestRequestTypeDef",
     "TranslateDocumentResponseTypeDef",
     "TranslateTextResponseTypeDef",
     "StartTextTranslationJobRequestRequestTypeDef",
@@ -106,15 +105,14 @@
 
 TermTypeDef = TypedDict(
     "TermTypeDef",
     {
         "SourceText": str,
         "TargetText": str,
     },
-    total=False,
 )
 
 EncryptionKeyTypeDef = TypedDict(
     "EncryptionKeyTypeDef",
     {
         "Type": Literal["KMS"],
         "Id": str,
@@ -133,32 +131,39 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateParallelDataResponseTypeDef = TypedDict(
+    "CreateParallelDataResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteParallelDataRequestRequestTypeDef = TypedDict(
     "DeleteParallelDataRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteParallelDataResponseTypeDef = TypedDict(
+    "DeleteParallelDataResponseTypeDef",
+    {
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteTerminologyRequestRequestTypeDef = TypedDict(
     "DeleteTerminologyRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -173,14 +178,21 @@
     "DocumentTypeDef",
     {
         "Content": Union[str, bytes, IO[Any], StreamingBody],
         "ContentType": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EncryptionKeyOutputTypeDef = TypedDict(
     "EncryptionKeyOutputTypeDef",
     {
         "Type": Literal["KMS"],
         "Id": str,
     },
 )
@@ -210,21 +222,19 @@
     "_OptionalGetTerminologyRequestRequestTypeDef",
     {
         "TerminologyDataFormat": TerminologyDataFormatType,
     },
     total=False,
 )
 
-
 class GetTerminologyRequestRequestTypeDef(
     _RequiredGetTerminologyRequestRequestTypeDef, _OptionalGetTerminologyRequestRequestTypeDef
 ):
     pass
 
-
 TerminologyDataLocationTypeDef = TypedDict(
     "TerminologyDataLocationTypeDef",
     {
         "RepositoryType": str,
         "Location": str,
     },
 )
@@ -240,19 +250,17 @@
     "_OptionalTerminologyDataTypeDef",
     {
         "Directionality": DirectionalityType,
     },
     total=False,
 )
 
-
 class TerminologyDataTypeDef(_RequiredTerminologyDataTypeDef, _OptionalTerminologyDataTypeDef):
     pass
 
-
 InputDataConfigOutputTypeDef = TypedDict(
     "InputDataConfigOutputTypeDef",
     {
         "S3Uri": str,
         "ContentType": str,
     },
 )
@@ -268,15 +276,14 @@
 JobDetailsTypeDef = TypedDict(
     "JobDetailsTypeDef",
     {
         "TranslatedDocumentsCount": int,
         "DocumentsWithErrorsCount": int,
         "InputDocumentsCount": int,
     },
-    total=False,
 )
 
 LanguageTypeDef = TypedDict(
     "LanguageTypeDef",
     {
         "LanguageName": str,
         "LanguageCode": str,
@@ -313,20 +320,18 @@
     "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListTerminologiesRequestListTerminologiesPaginateTypeDef = TypedDict(
+    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListTerminologiesRequestRequestTypeDef = TypedDict(
     "ListTerminologiesRequestRequestTypeDef",
     {
@@ -343,45 +348,83 @@
         "JobStatus": JobStatusType,
         "SubmittedBeforeTime": Union[datetime, str],
         "SubmittedAfterTime": Union[datetime, str],
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 ParallelDataConfigOutputTypeDef = TypedDict(
     "ParallelDataConfigOutputTypeDef",
     {
         "S3Uri": str,
         "Format": ParallelDataFormatType,
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
 TranslationSettingsTypeDef = TypedDict(
     "TranslationSettingsTypeDef",
     {
         "Formality": FormalityType,
         "Profanity": Literal["MASK"],
     },
     total=False,
 )
 
+StartTextTranslationJobResponseTypeDef = TypedDict(
+    "StartTextTranslationJobResponseTypeDef",
+    {
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopTextTranslationJobRequestRequestTypeDef = TypedDict(
     "StopTextTranslationJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+StopTextTranslationJobResponseTypeDef = TypedDict(
+    "StopTextTranslationJobResponseTypeDef",
+    {
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TranslationSettingsOutputTypeDef = TypedDict(
     "TranslationSettingsOutputTypeDef",
     {
         "Formality": FormalityType,
         "Profanity": Literal["MASK"],
     },
-    total=False,
 )
 
 TranslatedDocumentTypeDef = TypedDict(
     "TranslatedDocumentTypeDef",
     {
         "Content": bytes,
     },
@@ -391,21 +434,31 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateParallelDataResponseTypeDef = TypedDict(
+    "UpdateParallelDataResponseTypeDef",
+    {
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "LatestUpdateAttemptStatus": ParallelDataStatusType,
+        "LatestUpdateAttemptAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AppliedTerminologyTypeDef = TypedDict(
     "AppliedTerminologyTypeDef",
     {
         "Name": str,
         "Terms": List[TermTypeDef],
     },
-    total=False,
 )
 
 _RequiredOutputDataConfigTypeDef = TypedDict(
     "_RequiredOutputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
@@ -414,19 +467,17 @@
     "_OptionalOutputDataConfigTypeDef",
     {
         "EncryptionKey": EncryptionKeyTypeDef,
     },
     total=False,
 )
 
-
 class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
-
 _RequiredUpdateParallelDataRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateParallelDataRequestRequestTypeDef",
     {
         "Name": str,
         "ParallelDataConfig": ParallelDataConfigTypeDef,
         "ClientToken": str,
     },
@@ -435,22 +486,20 @@
     "_OptionalUpdateParallelDataRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateParallelDataRequestRequestTypeDef(
     _RequiredUpdateParallelDataRequestRequestTypeDef,
     _OptionalUpdateParallelDataRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateParallelDataRequestRequestTypeDef = TypedDict(
     "_RequiredCreateParallelDataRequestRequestTypeDef",
     {
         "Name": str,
         "ParallelDataConfig": ParallelDataConfigTypeDef,
         "ClientToken": str,
     },
@@ -461,105 +510,36 @@
         "Description": str,
         "EncryptionKey": EncryptionKeyTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateParallelDataRequestRequestTypeDef(
     _RequiredCreateParallelDataRequestRequestTypeDef,
     _OptionalCreateParallelDataRequestRequestTypeDef,
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-CreateParallelDataResponseTypeDef = TypedDict(
-    "CreateParallelDataResponseTypeDef",
-    {
-        "Name": str,
-        "Status": ParallelDataStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteParallelDataResponseTypeDef = TypedDict(
-    "DeleteParallelDataResponseTypeDef",
-    {
-        "Name": str,
-        "Status": ParallelDataStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartTextTranslationJobResponseTypeDef = TypedDict(
-    "StartTextTranslationJobResponseTypeDef",
-    {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopTextTranslationJobResponseTypeDef = TypedDict(
-    "StopTextTranslationJobResponseTypeDef",
-    {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateParallelDataResponseTypeDef = TypedDict(
-    "UpdateParallelDataResponseTypeDef",
-    {
-        "Name": str,
-        "Status": ParallelDataStatusType,
-        "LatestUpdateAttemptStatus": ParallelDataStatusType,
-        "LatestUpdateAttemptAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredOutputDataConfigOutputTypeDef = TypedDict(
-    "_RequiredOutputDataConfigOutputTypeDef",
+OutputDataConfigOutputTypeDef = TypedDict(
+    "OutputDataConfigOutputTypeDef",
     {
         "S3Uri": str,
-    },
-)
-_OptionalOutputDataConfigOutputTypeDef = TypedDict(
-    "_OptionalOutputDataConfigOutputTypeDef",
-    {
         "EncryptionKey": EncryptionKeyOutputTypeDef,
     },
-    total=False,
 )
 
-
-class OutputDataConfigOutputTypeDef(
-    _RequiredOutputDataConfigOutputTypeDef, _OptionalOutputDataConfigOutputTypeDef
-):
-    pass
-
-
 TerminologyPropertiesTypeDef = TypedDict(
     "TerminologyPropertiesTypeDef",
     {
         "Name": str,
         "Description": str,
         "Arn": str,
         "SourceLanguageCode": str,
@@ -570,15 +550,14 @@
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Directionality": DirectionalityType,
         "Message": str,
         "SkippedTermCount": int,
         "Format": TerminologyDataFormatType,
     },
-    total=False,
 )
 
 _RequiredImportTerminologyRequestRequestTypeDef = TypedDict(
     "_RequiredImportTerminologyRequestRequestTypeDef",
     {
         "Name": str,
         "MergeStrategy": Literal["OVERWRITE"],
@@ -591,47 +570,37 @@
         "Description": str,
         "EncryptionKey": EncryptionKeyTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class ImportTerminologyRequestRequestTypeDef(
     _RequiredImportTerminologyRequestRequestTypeDef, _OptionalImportTerminologyRequestRequestTypeDef
 ):
     pass
 
-
 ListLanguagesResponseTypeDef = TypedDict(
     "ListLanguagesResponseTypeDef",
     {
         "Languages": List[LanguageTypeDef],
         "DisplayLanguageCode": DisplayLanguageCodeType,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTerminologiesRequestListTerminologiesPaginateTypeDef = TypedDict(
-    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListTextTranslationJobsRequestRequestTypeDef = TypedDict(
     "ListTextTranslationJobsRequestRequestTypeDef",
     {
         "Filter": TextTranslationJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -655,15 +624,14 @@
         "SkippedRecordCount": int,
         "EncryptionKey": EncryptionKeyOutputTypeDef,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "LatestUpdateAttemptStatus": ParallelDataStatusType,
         "LatestUpdateAttemptAt": datetime,
     },
-    total=False,
 )
 
 _RequiredTranslateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredTranslateDocumentRequestRequestTypeDef",
     {
         "Document": DocumentTypeDef,
         "SourceLanguageCode": str,
@@ -675,21 +643,19 @@
     {
         "TerminologyNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
-
 class TranslateDocumentRequestRequestTypeDef(
     _RequiredTranslateDocumentRequestRequestTypeDef, _OptionalTranslateDocumentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredTranslateTextRequestRequestTypeDef = TypedDict(
     "_RequiredTranslateTextRequestRequestTypeDef",
     {
         "Text": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
     },
@@ -699,42 +665,40 @@
     {
         "TerminologyNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
-
 class TranslateTextRequestRequestTypeDef(
     _RequiredTranslateTextRequestRequestTypeDef, _OptionalTranslateTextRequestRequestTypeDef
 ):
     pass
 
-
 TranslateDocumentResponseTypeDef = TypedDict(
     "TranslateDocumentResponseTypeDef",
     {
         "TranslatedDocument": TranslatedDocumentTypeDef,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
         "AppliedTerminologies": List[AppliedTerminologyTypeDef],
         "AppliedSettings": TranslationSettingsOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TranslateTextResponseTypeDef = TypedDict(
     "TranslateTextResponseTypeDef",
     {
         "TranslatedText": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
         "AppliedTerminologies": List[AppliedTerminologyTypeDef],
         "AppliedSettings": TranslationSettingsOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartTextTranslationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTextTranslationJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
@@ -752,22 +716,20 @@
         "TerminologyNames": Sequence[str],
         "ParallelDataNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
-
 class StartTextTranslationJobRequestRequestTypeDef(
     _RequiredStartTextTranslationJobRequestRequestTypeDef,
     _OptionalStartTextTranslationJobRequestRequestTypeDef,
 ):
     pass
 
-
 TextTranslationJobPropertiesTypeDef = TypedDict(
     "TextTranslationJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "JobDetails": JobDetailsTypeDef,
@@ -779,74 +741,73 @@
         "SubmittedTime": datetime,
         "EndTime": datetime,
         "InputDataConfig": InputDataConfigOutputTypeDef,
         "OutputDataConfig": OutputDataConfigOutputTypeDef,
         "DataAccessRoleArn": str,
         "Settings": TranslationSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 GetTerminologyResponseTypeDef = TypedDict(
     "GetTerminologyResponseTypeDef",
     {
         "TerminologyProperties": TerminologyPropertiesTypeDef,
         "TerminologyDataLocation": TerminologyDataLocationTypeDef,
         "AuxiliaryDataLocation": TerminologyDataLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportTerminologyResponseTypeDef = TypedDict(
     "ImportTerminologyResponseTypeDef",
     {
         "TerminologyProperties": TerminologyPropertiesTypeDef,
         "AuxiliaryDataLocation": TerminologyDataLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTerminologiesResponseTypeDef = TypedDict(
     "ListTerminologiesResponseTypeDef",
     {
         "TerminologyPropertiesList": List[TerminologyPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetParallelDataResponseTypeDef = TypedDict(
     "GetParallelDataResponseTypeDef",
     {
         "ParallelDataProperties": ParallelDataPropertiesTypeDef,
         "DataLocation": ParallelDataDataLocationTypeDef,
         "AuxiliaryDataLocation": ParallelDataDataLocationTypeDef,
         "LatestUpdateAttemptAuxiliaryDataLocation": ParallelDataDataLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListParallelDataResponseTypeDef = TypedDict(
     "ListParallelDataResponseTypeDef",
     {
         "ParallelDataPropertiesList": List[ParallelDataPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTextTranslationJobResponseTypeDef = TypedDict(
     "DescribeTextTranslationJobResponseTypeDef",
     {
         "TextTranslationJobProperties": TextTranslationJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTextTranslationJobsResponseTypeDef = TypedDict(
     "ListTextTranslationJobsResponseTypeDef",
     {
         "TextTranslationJobPropertiesList": List[TextTranslationJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-translate-1.28.12/mypy_boto3_translate/type_defs.pyi` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,64 +32,65 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TermTypeDef",
     "EncryptionKeyTypeDef",
     "ParallelDataConfigTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateParallelDataResponseTypeDef",
     "DeleteParallelDataRequestRequestTypeDef",
+    "DeleteParallelDataResponseTypeDef",
     "DeleteTerminologyRequestRequestTypeDef",
     "DescribeTextTranslationJobRequestRequestTypeDef",
     "DocumentTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EncryptionKeyOutputTypeDef",
     "GetParallelDataRequestRequestTypeDef",
     "ParallelDataDataLocationTypeDef",
     "GetTerminologyRequestRequestTypeDef",
     "TerminologyDataLocationTypeDef",
     "TerminologyDataTypeDef",
     "InputDataConfigOutputTypeDef",
     "InputDataConfigTypeDef",
     "JobDetailsTypeDef",
     "LanguageTypeDef",
     "ListLanguagesRequestRequestTypeDef",
     "ListParallelDataRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagOutputTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     "ListTerminologiesRequestRequestTypeDef",
     "TextTranslationJobFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "ParallelDataConfigOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "TranslationSettingsTypeDef",
+    "StartTextTranslationJobResponseTypeDef",
     "StopTextTranslationJobRequestRequestTypeDef",
+    "StopTextTranslationJobResponseTypeDef",
     "TranslationSettingsOutputTypeDef",
     "TranslatedDocumentTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateParallelDataResponseTypeDef",
     "AppliedTerminologyTypeDef",
     "OutputDataConfigTypeDef",
     "UpdateParallelDataRequestRequestTypeDef",
     "CreateParallelDataRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "CreateParallelDataResponseTypeDef",
-    "DeleteParallelDataResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "StartTextTranslationJobResponseTypeDef",
-    "StopTextTranslationJobResponseTypeDef",
-    "UpdateParallelDataResponseTypeDef",
     "OutputDataConfigOutputTypeDef",
     "TerminologyPropertiesTypeDef",
     "ImportTerminologyRequestRequestTypeDef",
     "ListLanguagesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     "ListTextTranslationJobsRequestRequestTypeDef",
     "ParallelDataPropertiesTypeDef",
     "TranslateDocumentRequestRequestTypeDef",
     "TranslateTextRequestRequestTypeDef",
     "TranslateDocumentResponseTypeDef",
     "TranslateTextResponseTypeDef",
     "StartTextTranslationJobRequestRequestTypeDef",
@@ -105,15 +106,14 @@
 
 TermTypeDef = TypedDict(
     "TermTypeDef",
     {
         "SourceText": str,
         "TargetText": str,
     },
-    total=False,
 )
 
 EncryptionKeyTypeDef = TypedDict(
     "EncryptionKeyTypeDef",
     {
         "Type": Literal["KMS"],
         "Id": str,
@@ -132,32 +132,39 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateParallelDataResponseTypeDef = TypedDict(
+    "CreateParallelDataResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteParallelDataRequestRequestTypeDef = TypedDict(
     "DeleteParallelDataRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteParallelDataResponseTypeDef = TypedDict(
+    "DeleteParallelDataResponseTypeDef",
+    {
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteTerminologyRequestRequestTypeDef = TypedDict(
     "DeleteTerminologyRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -172,14 +179,21 @@
     "DocumentTypeDef",
     {
         "Content": Union[str, bytes, IO[Any], StreamingBody],
         "ContentType": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EncryptionKeyOutputTypeDef = TypedDict(
     "EncryptionKeyOutputTypeDef",
     {
         "Type": Literal["KMS"],
         "Id": str,
     },
 )
@@ -209,19 +223,21 @@
     "_OptionalGetTerminologyRequestRequestTypeDef",
     {
         "TerminologyDataFormat": TerminologyDataFormatType,
     },
     total=False,
 )
 
+
 class GetTerminologyRequestRequestTypeDef(
     _RequiredGetTerminologyRequestRequestTypeDef, _OptionalGetTerminologyRequestRequestTypeDef
 ):
     pass
 
+
 TerminologyDataLocationTypeDef = TypedDict(
     "TerminologyDataLocationTypeDef",
     {
         "RepositoryType": str,
         "Location": str,
     },
 )
@@ -237,17 +253,19 @@
     "_OptionalTerminologyDataTypeDef",
     {
         "Directionality": DirectionalityType,
     },
     total=False,
 )
 
+
 class TerminologyDataTypeDef(_RequiredTerminologyDataTypeDef, _OptionalTerminologyDataTypeDef):
     pass
 
+
 InputDataConfigOutputTypeDef = TypedDict(
     "InputDataConfigOutputTypeDef",
     {
         "S3Uri": str,
         "ContentType": str,
     },
 )
@@ -263,15 +281,14 @@
 JobDetailsTypeDef = TypedDict(
     "JobDetailsTypeDef",
     {
         "TranslatedDocumentsCount": int,
         "DocumentsWithErrorsCount": int,
         "InputDocumentsCount": int,
     },
-    total=False,
 )
 
 LanguageTypeDef = TypedDict(
     "LanguageTypeDef",
     {
         "LanguageName": str,
         "LanguageCode": str,
@@ -308,20 +325,18 @@
     "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListTerminologiesRequestListTerminologiesPaginateTypeDef = TypedDict(
+    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListTerminologiesRequestRequestTypeDef = TypedDict(
     "ListTerminologiesRequestRequestTypeDef",
     {
@@ -338,45 +353,83 @@
         "JobStatus": JobStatusType,
         "SubmittedBeforeTime": Union[datetime, str],
         "SubmittedAfterTime": Union[datetime, str],
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 ParallelDataConfigOutputTypeDef = TypedDict(
     "ParallelDataConfigOutputTypeDef",
     {
         "S3Uri": str,
         "Format": ParallelDataFormatType,
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
 TranslationSettingsTypeDef = TypedDict(
     "TranslationSettingsTypeDef",
     {
         "Formality": FormalityType,
         "Profanity": Literal["MASK"],
     },
     total=False,
 )
 
+StartTextTranslationJobResponseTypeDef = TypedDict(
+    "StartTextTranslationJobResponseTypeDef",
+    {
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopTextTranslationJobRequestRequestTypeDef = TypedDict(
     "StopTextTranslationJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+StopTextTranslationJobResponseTypeDef = TypedDict(
+    "StopTextTranslationJobResponseTypeDef",
+    {
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TranslationSettingsOutputTypeDef = TypedDict(
     "TranslationSettingsOutputTypeDef",
     {
         "Formality": FormalityType,
         "Profanity": Literal["MASK"],
     },
-    total=False,
 )
 
 TranslatedDocumentTypeDef = TypedDict(
     "TranslatedDocumentTypeDef",
     {
         "Content": bytes,
     },
@@ -386,21 +439,31 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateParallelDataResponseTypeDef = TypedDict(
+    "UpdateParallelDataResponseTypeDef",
+    {
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "LatestUpdateAttemptStatus": ParallelDataStatusType,
+        "LatestUpdateAttemptAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AppliedTerminologyTypeDef = TypedDict(
     "AppliedTerminologyTypeDef",
     {
         "Name": str,
         "Terms": List[TermTypeDef],
     },
-    total=False,
 )
 
 _RequiredOutputDataConfigTypeDef = TypedDict(
     "_RequiredOutputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
@@ -409,17 +472,19 @@
     "_OptionalOutputDataConfigTypeDef",
     {
         "EncryptionKey": EncryptionKeyTypeDef,
     },
     total=False,
 )
 
+
 class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
+
 _RequiredUpdateParallelDataRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateParallelDataRequestRequestTypeDef",
     {
         "Name": str,
         "ParallelDataConfig": ParallelDataConfigTypeDef,
         "ClientToken": str,
     },
@@ -428,20 +493,22 @@
     "_OptionalUpdateParallelDataRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateParallelDataRequestRequestTypeDef(
     _RequiredUpdateParallelDataRequestRequestTypeDef,
     _OptionalUpdateParallelDataRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateParallelDataRequestRequestTypeDef = TypedDict(
     "_RequiredCreateParallelDataRequestRequestTypeDef",
     {
         "Name": str,
         "ParallelDataConfig": ParallelDataConfigTypeDef,
         "ClientToken": str,
     },
@@ -452,101 +519,38 @@
         "Description": str,
         "EncryptionKey": EncryptionKeyTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateParallelDataRequestRequestTypeDef(
     _RequiredCreateParallelDataRequestRequestTypeDef,
     _OptionalCreateParallelDataRequestRequestTypeDef,
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-CreateParallelDataResponseTypeDef = TypedDict(
-    "CreateParallelDataResponseTypeDef",
-    {
-        "Name": str,
-        "Status": ParallelDataStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteParallelDataResponseTypeDef = TypedDict(
-    "DeleteParallelDataResponseTypeDef",
-    {
-        "Name": str,
-        "Status": ParallelDataStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartTextTranslationJobResponseTypeDef = TypedDict(
-    "StartTextTranslationJobResponseTypeDef",
-    {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopTextTranslationJobResponseTypeDef = TypedDict(
-    "StopTextTranslationJobResponseTypeDef",
-    {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateParallelDataResponseTypeDef = TypedDict(
-    "UpdateParallelDataResponseTypeDef",
-    {
-        "Name": str,
-        "Status": ParallelDataStatusType,
-        "LatestUpdateAttemptStatus": ParallelDataStatusType,
-        "LatestUpdateAttemptAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredOutputDataConfigOutputTypeDef = TypedDict(
-    "_RequiredOutputDataConfigOutputTypeDef",
+OutputDataConfigOutputTypeDef = TypedDict(
+    "OutputDataConfigOutputTypeDef",
     {
         "S3Uri": str,
-    },
-)
-_OptionalOutputDataConfigOutputTypeDef = TypedDict(
-    "_OptionalOutputDataConfigOutputTypeDef",
-    {
         "EncryptionKey": EncryptionKeyOutputTypeDef,
     },
-    total=False,
 )
 
-class OutputDataConfigOutputTypeDef(
-    _RequiredOutputDataConfigOutputTypeDef, _OptionalOutputDataConfigOutputTypeDef
-):
-    pass
-
 TerminologyPropertiesTypeDef = TypedDict(
     "TerminologyPropertiesTypeDef",
     {
         "Name": str,
         "Description": str,
         "Arn": str,
         "SourceLanguageCode": str,
@@ -557,15 +561,14 @@
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Directionality": DirectionalityType,
         "Message": str,
         "SkippedTermCount": int,
         "Format": TerminologyDataFormatType,
     },
-    total=False,
 )
 
 _RequiredImportTerminologyRequestRequestTypeDef = TypedDict(
     "_RequiredImportTerminologyRequestRequestTypeDef",
     {
         "Name": str,
         "MergeStrategy": Literal["OVERWRITE"],
@@ -578,45 +581,39 @@
         "Description": str,
         "EncryptionKey": EncryptionKeyTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class ImportTerminologyRequestRequestTypeDef(
     _RequiredImportTerminologyRequestRequestTypeDef, _OptionalImportTerminologyRequestRequestTypeDef
 ):
     pass
 
+
 ListLanguagesResponseTypeDef = TypedDict(
     "ListLanguagesResponseTypeDef",
     {
         "Languages": List[LanguageTypeDef],
         "DisplayLanguageCode": DisplayLanguageCodeType,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTerminologiesRequestListTerminologiesPaginateTypeDef = TypedDict(
-    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListTextTranslationJobsRequestRequestTypeDef = TypedDict(
     "ListTextTranslationJobsRequestRequestTypeDef",
     {
         "Filter": TextTranslationJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -640,15 +637,14 @@
         "SkippedRecordCount": int,
         "EncryptionKey": EncryptionKeyOutputTypeDef,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "LatestUpdateAttemptStatus": ParallelDataStatusType,
         "LatestUpdateAttemptAt": datetime,
     },
-    total=False,
 )
 
 _RequiredTranslateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredTranslateDocumentRequestRequestTypeDef",
     {
         "Document": DocumentTypeDef,
         "SourceLanguageCode": str,
@@ -660,19 +656,21 @@
     {
         "TerminologyNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
+
 class TranslateDocumentRequestRequestTypeDef(
     _RequiredTranslateDocumentRequestRequestTypeDef, _OptionalTranslateDocumentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredTranslateTextRequestRequestTypeDef = TypedDict(
     "_RequiredTranslateTextRequestRequestTypeDef",
     {
         "Text": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
     },
@@ -682,40 +680,42 @@
     {
         "TerminologyNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
+
 class TranslateTextRequestRequestTypeDef(
     _RequiredTranslateTextRequestRequestTypeDef, _OptionalTranslateTextRequestRequestTypeDef
 ):
     pass
 
+
 TranslateDocumentResponseTypeDef = TypedDict(
     "TranslateDocumentResponseTypeDef",
     {
         "TranslatedDocument": TranslatedDocumentTypeDef,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
         "AppliedTerminologies": List[AppliedTerminologyTypeDef],
         "AppliedSettings": TranslationSettingsOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TranslateTextResponseTypeDef = TypedDict(
     "TranslateTextResponseTypeDef",
     {
         "TranslatedText": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
         "AppliedTerminologies": List[AppliedTerminologyTypeDef],
         "AppliedSettings": TranslationSettingsOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartTextTranslationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTextTranslationJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
@@ -733,20 +733,22 @@
         "TerminologyNames": Sequence[str],
         "ParallelDataNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
+
 class StartTextTranslationJobRequestRequestTypeDef(
     _RequiredStartTextTranslationJobRequestRequestTypeDef,
     _OptionalStartTextTranslationJobRequestRequestTypeDef,
 ):
     pass
 
+
 TextTranslationJobPropertiesTypeDef = TypedDict(
     "TextTranslationJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "JobDetails": JobDetailsTypeDef,
@@ -758,74 +760,73 @@
         "SubmittedTime": datetime,
         "EndTime": datetime,
         "InputDataConfig": InputDataConfigOutputTypeDef,
         "OutputDataConfig": OutputDataConfigOutputTypeDef,
         "DataAccessRoleArn": str,
         "Settings": TranslationSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 GetTerminologyResponseTypeDef = TypedDict(
     "GetTerminologyResponseTypeDef",
     {
         "TerminologyProperties": TerminologyPropertiesTypeDef,
         "TerminologyDataLocation": TerminologyDataLocationTypeDef,
         "AuxiliaryDataLocation": TerminologyDataLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportTerminologyResponseTypeDef = TypedDict(
     "ImportTerminologyResponseTypeDef",
     {
         "TerminologyProperties": TerminologyPropertiesTypeDef,
         "AuxiliaryDataLocation": TerminologyDataLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTerminologiesResponseTypeDef = TypedDict(
     "ListTerminologiesResponseTypeDef",
     {
         "TerminologyPropertiesList": List[TerminologyPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetParallelDataResponseTypeDef = TypedDict(
     "GetParallelDataResponseTypeDef",
     {
         "ParallelDataProperties": ParallelDataPropertiesTypeDef,
         "DataLocation": ParallelDataDataLocationTypeDef,
         "AuxiliaryDataLocation": ParallelDataDataLocationTypeDef,
         "LatestUpdateAttemptAuxiliaryDataLocation": ParallelDataDataLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListParallelDataResponseTypeDef = TypedDict(
     "ListParallelDataResponseTypeDef",
     {
         "ParallelDataPropertiesList": List[ParallelDataPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTextTranslationJobResponseTypeDef = TypedDict(
     "DescribeTextTranslationJobResponseTypeDef",
     {
         "TextTranslationJobProperties": TextTranslationJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTextTranslationJobsResponseTypeDef = TypedDict(
     "ListTextTranslationJobsResponseTypeDef",
     {
         "TextTranslationJobPropertiesList": List[TextTranslationJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-translate-1.28.12/mypy_boto3_translate.egg-info/PKG-INFO` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-translate
-Version: 1.28.12
-Summary: Type annotations for boto3.Translate 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.5
+Summary: Type annotations for boto3.Translate 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-translate"></a>
 
 # mypy-boto3-translate
 
 [![PyPI - mypy-boto3-translate](https://img.shields.io/pypi/v/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-translate)](https://pepy.tech/project/mypy-boto3-translate)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-translate?color=blue)](https://pypistats.org/packages/mypy-boto3-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Translate 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
+[boto3.Translate 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
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
 [mypy-boto3-translate docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,59 +334,59 @@
 
 ```python
 from mypy_boto3_translate.type_defs import (
     TermTypeDef,
     EncryptionKeyTypeDef,
     ParallelDataConfigTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateParallelDataResponseTypeDef,
     DeleteParallelDataRequestRequestTypeDef,
+    DeleteParallelDataResponseTypeDef,
     DeleteTerminologyRequestRequestTypeDef,
     DescribeTextTranslationJobRequestRequestTypeDef,
     DocumentTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionKeyOutputTypeDef,
     GetParallelDataRequestRequestTypeDef,
     ParallelDataDataLocationTypeDef,
     GetTerminologyRequestRequestTypeDef,
     TerminologyDataLocationTypeDef,
     TerminologyDataTypeDef,
     InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
     JobDetailsTypeDef,
     LanguageTypeDef,
     ListLanguagesRequestRequestTypeDef,
     ListParallelDataRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagOutputTypeDef,
-    PaginatorConfigTypeDef,
+    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     ListTerminologiesRequestRequestTypeDef,
     TextTranslationJobFilterTypeDef,
+    PaginatorConfigTypeDef,
     ParallelDataConfigOutputTypeDef,
+    ResponseMetadataTypeDef,
     TranslationSettingsTypeDef,
+    StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobRequestRequestTypeDef,
+    StopTextTranslationJobResponseTypeDef,
     TranslationSettingsOutputTypeDef,
     TranslatedDocumentTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateParallelDataResponseTypeDef,
     AppliedTerminologyTypeDef,
     OutputDataConfigTypeDef,
     UpdateParallelDataRequestRequestTypeDef,
     CreateParallelDataRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateParallelDataResponseTypeDef,
-    DeleteParallelDataResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    StartTextTranslationJobResponseTypeDef,
-    StopTextTranslationJobResponseTypeDef,
-    UpdateParallelDataResponseTypeDef,
     OutputDataConfigOutputTypeDef,
     TerminologyPropertiesTypeDef,
     ImportTerminologyRequestRequestTypeDef,
     ListLanguagesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     ListTextTranslationJobsRequestRequestTypeDef,
     ParallelDataPropertiesTypeDef,
     TranslateDocumentRequestRequestTypeDef,
     TranslateTextRequestRequestTypeDef,
     TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
     StartTextTranslationJobRequestRequestTypeDef,
```

### Comparing `mypy-boto3-translate-1.28.12/mypy_boto3_translate.egg-info/SOURCES.txt` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.12/setup.py` & `mypy-boto3-translate-1.28.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-translate",
-    version="1.28.12",
+    version="1.28.5",
     packages=["mypy_boto3_translate"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Translate 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Translate 1.28.5 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

