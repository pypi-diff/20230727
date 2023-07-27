# Comparing `tmp/mypy-boto3-polly-1.28.0.tar.gz` & `tmp/mypy-boto3-polly-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-polly-1.28.0.tar", last modified: Thu Jul  6 21:00:21 2023, max compression
+gzip compressed data, was "mypy-boto3-polly-1.28.12.tar", last modified: Thu Jul 27 05:44:17 2023, max compression
```

## Comparing `mypy-boto3-polly-1.28.0.tar` & `mypy-boto3-polly-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:21.486398 mypy-boto3-polly-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:49:42.000000 mypy-boto3-polly-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13873 2023-07-06 21:00:21.486398 mypy-boto3-polly-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12396 2023-07-06 20:49:42.000000 mypy-boto3-polly-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:21.482398 mypy-boto3-polly-1.28.0/mypy_boto3_polly/
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-06 20:49:42.000000 mypy-boto3-polly-1.28.0/mypy_boto3_polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-06 20:49:42.000000 mypy-boto3-polly-1.28.0/mypy_boto3_polly/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-06 20:49:42.000000 mypy-boto3-polly-1.28.0/mypy_boto3_polly/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-07-06 20:49:42.000000 mypy-boto3-polly-1.28.0/mypy_boto3_polly/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-07-06 20:49:42.000000 mypy-boto3-polly-1.28.0/mypy_boto3_polly/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10606 2023-07-06 20:49:43.000000 mypy-boto3-polly-1.28.0/mypy_boto3_polly/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-07-06 20:49:43.000000 mypy-boto3-polly-1.28.0/mypy_boto3_polly/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-06 20:49:43.000000 mypy-boto3-polly-1.28.0/mypy_boto3_polly/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-06 20:49:42.000000 mypy-boto3-polly-1.28.0/mypy_boto3_polly/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:49:42.000000 mypy-boto3-polly-1.28.0/mypy_boto3_polly/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-07-06 20:49:43.000000 mypy-boto3-polly-1.28.0/mypy_boto3_polly/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-07-06 20:49:43.000000 mypy-boto3-polly-1.28.0/mypy_boto3_polly/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:49:42.000000 mypy-boto3-polly-1.28.0/mypy_boto3_polly/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:21.486398 mypy-boto3-polly-1.28.0/mypy_boto3_polly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13873 2023-07-06 21:00:21.000000 mypy-boto3-polly-1.28.0/mypy_boto3_polly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-06 21:00:21.000000 mypy-boto3-polly-1.28.0/mypy_boto3_polly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:21.000000 mypy-boto3-polly-1.28.0/mypy_boto3_polly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:21.000000 mypy-boto3-polly-1.28.0/mypy_boto3_polly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:21.000000 mypy-boto3-polly-1.28.0/mypy_boto3_polly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 21:00:21.000000 mypy-boto3-polly-1.28.0/mypy_boto3_polly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:21.486398 mypy-boto3-polly-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-06 20:49:42.000000 mypy-boto3-polly-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:17.363381 mypy-boto3-polly-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:44:04.000000 mypy-boto3-polly-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13860 2023-07-27 05:44:17.363381 mypy-boto3-polly-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-07-27 05:44:04.000000 mypy-boto3-polly-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:17.363381 mypy-boto3-polly-1.28.12/mypy_boto3_polly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-27 05:44:04.000000 mypy-boto3-polly-1.28.12/mypy_boto3_polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-27 05:44:04.000000 mypy-boto3-polly-1.28.12/mypy_boto3_polly/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 05:44:04.000000 mypy-boto3-polly-1.28.12/mypy_boto3_polly/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-07-27 05:44:04.000000 mypy-boto3-polly-1.28.12/mypy_boto3_polly/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-07-27 05:44:04.000000 mypy-boto3-polly-1.28.12/mypy_boto3_polly/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-07-27 05:44:04.000000 mypy-boto3-polly-1.28.12/mypy_boto3_polly/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-07-27 05:44:04.000000 mypy-boto3-polly-1.28.12/mypy_boto3_polly/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-27 05:44:04.000000 mypy-boto3-polly-1.28.12/mypy_boto3_polly/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-27 05:44:04.000000 mypy-boto3-polly-1.28.12/mypy_boto3_polly/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:04.000000 mypy-boto3-polly-1.28.12/mypy_boto3_polly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-07-27 05:44:04.000000 mypy-boto3-polly-1.28.12/mypy_boto3_polly/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-07-27 05:44:04.000000 mypy-boto3-polly-1.28.12/mypy_boto3_polly/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:44:04.000000 mypy-boto3-polly-1.28.12/mypy_boto3_polly/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:17.363381 mypy-boto3-polly-1.28.12/mypy_boto3_polly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13860 2023-07-27 05:44:17.000000 mypy-boto3-polly-1.28.12/mypy_boto3_polly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-27 05:44:17.000000 mypy-boto3-polly-1.28.12/mypy_boto3_polly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:44:17.000000 mypy-boto3-polly-1.28.12/mypy_boto3_polly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:44:17.000000 mypy-boto3-polly-1.28.12/mypy_boto3_polly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:44:17.000000 mypy-boto3-polly-1.28.12/mypy_boto3_polly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 05:44:17.000000 mypy-boto3-polly-1.28.12/mypy_boto3_polly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:44:17.363381 mypy-boto3-polly-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 05:44:04.000000 mypy-boto3-polly-1.28.12/setup.py
```

### Comparing `mypy-boto3-polly-1.28.0/LICENSE` & `mypy-boto3-polly-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.0/PKG-INFO` & `mypy-boto3-polly-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-polly
-Version: 1.28.0
-Summary: Type annotations for boto3.Polly 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Polly 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-polly"></a>
 
 # mypy-boto3-polly
 
 [![PyPI - mypy-boto3-polly](https://img.shields.io/pypi/v/mypy-boto3-polly.svg?color=blue)](https://pypi.org/project/mypy-boto3-polly)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-polly.svg?color=blue)](https://pypi.org/project/mypy-boto3-polly)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-polly?color=blue)](https://pypistats.org/packages/mypy-boto3-polly)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-polly)](https://pepy.tech/project/mypy-boto3-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Polly 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[boto3.Polly 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
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
 [mypy-boto3-polly docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/).
 
 See how it helps to find and fix potential bugs:
 
@@ -337,31 +337,31 @@
 
 `mypy_boto3_polly.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_polly.type_defs import (
     DeleteLexiconInputRequestTypeDef,
-    DescribeVoicesInputDescribeVoicesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeVoicesInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     VoiceTypeDef,
     GetLexiconInputRequestTypeDef,
     LexiconAttributesTypeDef,
     LexiconTypeDef,
     GetSpeechSynthesisTaskInputRequestTypeDef,
     SynthesisTaskTypeDef,
-    ListLexiconsInputListLexiconsPaginateTypeDef,
     ListLexiconsInputRequestTypeDef,
-    ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef,
     ListSpeechSynthesisTasksInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutLexiconInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartSpeechSynthesisTaskInputRequestTypeDef,
     SynthesizeSpeechInputRequestTypeDef,
+    DescribeVoicesInputDescribeVoicesPaginateTypeDef,
+    ListLexiconsInputListLexiconsPaginateTypeDef,
+    ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef,
     SynthesizeSpeechOutputTypeDef,
     DescribeVoicesOutputTypeDef,
     LexiconDescriptionTypeDef,
     GetLexiconOutputTypeDef,
     GetSpeechSynthesisTaskOutputTypeDef,
     ListSpeechSynthesisTasksOutputTypeDef,
     StartSpeechSynthesisTaskOutputTypeDef,
```

### Comparing `mypy-boto3-polly-1.28.0/README.md` & `mypy-boto3-polly-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-polly"></a>
 
 # mypy-boto3-polly
 
 [![PyPI - mypy-boto3-polly](https://img.shields.io/pypi/v/mypy-boto3-polly.svg?color=blue)](https://pypi.org/project/mypy-boto3-polly)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-polly.svg?color=blue)](https://pypi.org/project/mypy-boto3-polly)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-polly?color=blue)](https://pypistats.org/packages/mypy-boto3-polly)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-polly)](https://pepy.tech/project/mypy-boto3-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Polly 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[boto3.Polly 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
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
 [mypy-boto3-polly docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,31 +305,31 @@
 
 `mypy_boto3_polly.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_polly.type_defs import (
     DeleteLexiconInputRequestTypeDef,
-    DescribeVoicesInputDescribeVoicesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeVoicesInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     VoiceTypeDef,
     GetLexiconInputRequestTypeDef,
     LexiconAttributesTypeDef,
     LexiconTypeDef,
     GetSpeechSynthesisTaskInputRequestTypeDef,
     SynthesisTaskTypeDef,
-    ListLexiconsInputListLexiconsPaginateTypeDef,
     ListLexiconsInputRequestTypeDef,
-    ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef,
     ListSpeechSynthesisTasksInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutLexiconInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartSpeechSynthesisTaskInputRequestTypeDef,
     SynthesizeSpeechInputRequestTypeDef,
+    DescribeVoicesInputDescribeVoicesPaginateTypeDef,
+    ListLexiconsInputListLexiconsPaginateTypeDef,
+    ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef,
     SynthesizeSpeechOutputTypeDef,
     DescribeVoicesOutputTypeDef,
     LexiconDescriptionTypeDef,
     GetLexiconOutputTypeDef,
     GetSpeechSynthesisTaskOutputTypeDef,
     ListSpeechSynthesisTasksOutputTypeDef,
     StartSpeechSynthesisTaskOutputTypeDef,
```

### Comparing `mypy-boto3-polly-1.28.0/mypy_boto3_polly/__init__.py` & `mypy-boto3-polly-1.28.12/mypy_boto3_polly/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.0/mypy_boto3_polly/__init__.pyi` & `mypy-boto3-polly-1.28.12/mypy_boto3_polly/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.0/mypy_boto3_polly/client.py` & `mypy-boto3-polly-1.28.12/mypy_boto3_polly/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.0/mypy_boto3_polly/client.pyi` & `mypy-boto3-polly-1.28.12/mypy_boto3_polly/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.0/mypy_boto3_polly/literals.py` & `mypy-boto3-polly-1.28.12/mypy_boto3_polly/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     "fr-FR",
     "hi-IN",
     "is-IS",
     "it-IT",
     "ja-JP",
     "ko-KR",
     "nb-NO",
+    "nl-BE",
     "nl-NL",
     "pl-PL",
     "pt-BR",
     "pt-PT",
     "ro-RO",
     "ru-RU",
     "sv-SE",
@@ -134,14 +135,15 @@
     "Kazuha",
     "Kendra",
     "Kevin",
     "Kimberly",
     "Laura",
     "Lea",
     "Liam",
+    "Lisa",
     "Liv",
     "Lotte",
     "Lucia",
     "Lupe",
     "Mads",
     "Maja",
     "Marlene",
@@ -295,14 +297,15 @@
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
@@ -381,26 +384,28 @@
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

### Comparing `mypy-boto3-polly-1.28.0/mypy_boto3_polly/literals.pyi` & `mypy-boto3-polly-1.28.12/mypy_boto3_polly/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     "fr-FR",
     "hi-IN",
     "is-IS",
     "it-IT",
     "ja-JP",
     "ko-KR",
     "nb-NO",
+    "nl-BE",
     "nl-NL",
     "pl-PL",
     "pt-BR",
     "pt-PT",
     "ro-RO",
     "ru-RU",
     "sv-SE",
@@ -132,14 +133,15 @@
     "Kazuha",
     "Kendra",
     "Kevin",
     "Kimberly",
     "Laura",
     "Lea",
     "Liam",
+    "Lisa",
     "Liv",
     "Lotte",
     "Lucia",
     "Lupe",
     "Mads",
     "Maja",
     "Marlene",
@@ -293,14 +295,15 @@
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
@@ -379,26 +382,28 @@
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

### Comparing `mypy-boto3-polly-1.28.0/mypy_boto3_polly/paginator.py` & `mypy-boto3-polly-1.28.12/mypy_boto3_polly/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,43 +56,43 @@
 
     def paginate(
         self,
         *,
         Engine: EngineType = ...,
         LanguageCode: LanguageCodeType = ...,
         IncludeAdditionalLanguageCodes: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeVoicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.DescribeVoices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/paginators/#describevoicespaginator)
         """
 
 
 class ListLexiconsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListLexicons)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/paginators/#listlexiconspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLexiconsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListLexicons.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/paginators/#listlexiconspaginator)
         """
 
 
 class ListSpeechSynthesisTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListSpeechSynthesisTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/paginators/#listspeechsynthesistaskspaginator)
     """
 
     def paginate(
-        self, *, Status: TaskStatusType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Status: TaskStatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSpeechSynthesisTasksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListSpeechSynthesisTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/paginators/#listspeechsynthesistaskspaginator)
         """
```

### Comparing `mypy-boto3-polly-1.28.0/mypy_boto3_polly/paginator.pyi` & `mypy-boto3-polly-1.28.12/mypy_boto3_polly/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -53,41 +53,41 @@
 
     def paginate(
         self,
         *,
         Engine: EngineType = ...,
         LanguageCode: LanguageCodeType = ...,
         IncludeAdditionalLanguageCodes: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeVoicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.DescribeVoices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/paginators/#describevoicespaginator)
         """
 
 class ListLexiconsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListLexicons)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/paginators/#listlexiconspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLexiconsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListLexicons.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/paginators/#listlexiconspaginator)
         """
 
 class ListSpeechSynthesisTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListSpeechSynthesisTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/paginators/#listspeechsynthesistaskspaginator)
     """
 
     def paginate(
-        self, *, Status: TaskStatusType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Status: TaskStatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSpeechSynthesisTasksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListSpeechSynthesisTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/paginators/#listspeechsynthesistaskspaginator)
         """
```

### Comparing `mypy-boto3-polly-1.28.0/mypy_boto3_polly/type_defs.py` & `mypy-boto3-polly-1.28.12/mypy_boto3_polly/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,31 +32,31 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "DeleteLexiconInputRequestTypeDef",
-    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeVoicesInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "VoiceTypeDef",
     "GetLexiconInputRequestTypeDef",
     "LexiconAttributesTypeDef",
     "LexiconTypeDef",
     "GetSpeechSynthesisTaskInputRequestTypeDef",
     "SynthesisTaskTypeDef",
-    "ListLexiconsInputListLexiconsPaginateTypeDef",
     "ListLexiconsInputRequestTypeDef",
-    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
     "ListSpeechSynthesisTasksInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutLexiconInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StartSpeechSynthesisTaskInputRequestTypeDef",
     "SynthesizeSpeechInputRequestTypeDef",
+    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
+    "ListLexiconsInputListLexiconsPaginateTypeDef",
+    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
     "SynthesizeSpeechOutputTypeDef",
     "DescribeVoicesOutputTypeDef",
     "LexiconDescriptionTypeDef",
     "GetLexiconOutputTypeDef",
     "GetSpeechSynthesisTaskOutputTypeDef",
     "ListSpeechSynthesisTasksOutputTypeDef",
     "StartSpeechSynthesisTaskOutputTypeDef",
@@ -66,21 +66,20 @@
 DeleteLexiconInputRequestTypeDef = TypedDict(
     "DeleteLexiconInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribeVoicesInputDescribeVoicesPaginateTypeDef = TypedDict(
-    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Engine": EngineType,
-        "LanguageCode": LanguageCodeType,
-        "IncludeAdditionalLanguageCodes": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeVoicesInputRequestTypeDef = TypedDict(
     "DescribeVoicesInputRequestTypeDef",
     {
@@ -88,14 +87,25 @@
         "LanguageCode": LanguageCodeType,
         "IncludeAdditionalLanguageCodes": bool,
         "NextToken": str,
     },
     total=False,
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
 VoiceTypeDef = TypedDict(
     "VoiceTypeDef",
     {
         "Gender": GenderType,
         "Id": VoiceIdType,
         "LanguageCode": LanguageCodeType,
         "LanguageName": str,
@@ -160,78 +170,40 @@
         "TextType": TextTypeType,
         "VoiceId": VoiceIdType,
         "LanguageCode": LanguageCodeType,
     },
     total=False,
 )
 
-ListLexiconsInputListLexiconsPaginateTypeDef = TypedDict(
-    "ListLexiconsInputListLexiconsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLexiconsInputRequestTypeDef = TypedDict(
     "ListLexiconsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef = TypedDict(
-    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
-    {
-        "Status": TaskStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSpeechSynthesisTasksInputRequestTypeDef = TypedDict(
     "ListSpeechSynthesisTasksInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Status": TaskStatusType,
     },
     total=False,
 )
 
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
 PutLexiconInputRequestTypeDef = TypedDict(
     "PutLexiconInputRequestTypeDef",
     {
         "Name": str,
         "Content": str,
     },
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
 _RequiredStartSpeechSynthesisTaskInputRequestTypeDef = TypedDict(
     "_RequiredStartSpeechSynthesisTaskInputRequestTypeDef",
     {
         "OutputFormat": OutputFormatType,
         "OutputS3BucketName": str,
         "Text": str,
         "VoiceId": VoiceIdType,
@@ -284,30 +256,58 @@
 
 class SynthesizeSpeechInputRequestTypeDef(
     _RequiredSynthesizeSpeechInputRequestTypeDef, _OptionalSynthesizeSpeechInputRequestTypeDef
 ):
     pass
 
 
+DescribeVoicesInputDescribeVoicesPaginateTypeDef = TypedDict(
+    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
+    {
+        "Engine": EngineType,
+        "LanguageCode": LanguageCodeType,
+        "IncludeAdditionalLanguageCodes": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListLexiconsInputListLexiconsPaginateTypeDef = TypedDict(
+    "ListLexiconsInputListLexiconsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef = TypedDict(
+    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
+    {
+        "Status": TaskStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 SynthesizeSpeechOutputTypeDef = TypedDict(
     "SynthesizeSpeechOutputTypeDef",
     {
         "AudioStream": StreamingBody,
         "ContentType": str,
         "RequestCharacters": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVoicesOutputTypeDef = TypedDict(
     "DescribeVoicesOutputTypeDef",
     {
         "Voices": List[VoiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LexiconDescriptionTypeDef = TypedDict(
     "LexiconDescriptionTypeDef",
     {
         "Name": str,
@@ -317,44 +317,44 @@
 )
 
 GetLexiconOutputTypeDef = TypedDict(
     "GetLexiconOutputTypeDef",
     {
         "Lexicon": LexiconTypeDef,
         "LexiconAttributes": LexiconAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSpeechSynthesisTaskOutputTypeDef = TypedDict(
     "GetSpeechSynthesisTaskOutputTypeDef",
     {
         "SynthesisTask": SynthesisTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSpeechSynthesisTasksOutputTypeDef = TypedDict(
     "ListSpeechSynthesisTasksOutputTypeDef",
     {
         "NextToken": str,
         "SynthesisTasks": List[SynthesisTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSpeechSynthesisTaskOutputTypeDef = TypedDict(
     "StartSpeechSynthesisTaskOutputTypeDef",
     {
         "SynthesisTask": SynthesisTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLexiconsOutputTypeDef = TypedDict(
     "ListLexiconsOutputTypeDef",
     {
         "Lexicons": List[LexiconDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-polly-1.28.0/mypy_boto3_polly/type_defs.pyi` & `mypy-boto3-polly-1.28.12/mypy_boto3_polly/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -31,31 +31,31 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "DeleteLexiconInputRequestTypeDef",
-    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeVoicesInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "VoiceTypeDef",
     "GetLexiconInputRequestTypeDef",
     "LexiconAttributesTypeDef",
     "LexiconTypeDef",
     "GetSpeechSynthesisTaskInputRequestTypeDef",
     "SynthesisTaskTypeDef",
-    "ListLexiconsInputListLexiconsPaginateTypeDef",
     "ListLexiconsInputRequestTypeDef",
-    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
     "ListSpeechSynthesisTasksInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutLexiconInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StartSpeechSynthesisTaskInputRequestTypeDef",
     "SynthesizeSpeechInputRequestTypeDef",
+    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
+    "ListLexiconsInputListLexiconsPaginateTypeDef",
+    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
     "SynthesizeSpeechOutputTypeDef",
     "DescribeVoicesOutputTypeDef",
     "LexiconDescriptionTypeDef",
     "GetLexiconOutputTypeDef",
     "GetSpeechSynthesisTaskOutputTypeDef",
     "ListSpeechSynthesisTasksOutputTypeDef",
     "StartSpeechSynthesisTaskOutputTypeDef",
@@ -65,21 +65,20 @@
 DeleteLexiconInputRequestTypeDef = TypedDict(
     "DeleteLexiconInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribeVoicesInputDescribeVoicesPaginateTypeDef = TypedDict(
-    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Engine": EngineType,
-        "LanguageCode": LanguageCodeType,
-        "IncludeAdditionalLanguageCodes": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeVoicesInputRequestTypeDef = TypedDict(
     "DescribeVoicesInputRequestTypeDef",
     {
@@ -87,14 +86,25 @@
         "LanguageCode": LanguageCodeType,
         "IncludeAdditionalLanguageCodes": bool,
         "NextToken": str,
     },
     total=False,
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
 VoiceTypeDef = TypedDict(
     "VoiceTypeDef",
     {
         "Gender": GenderType,
         "Id": VoiceIdType,
         "LanguageCode": LanguageCodeType,
         "LanguageName": str,
@@ -159,78 +169,40 @@
         "TextType": TextTypeType,
         "VoiceId": VoiceIdType,
         "LanguageCode": LanguageCodeType,
     },
     total=False,
 )
 
-ListLexiconsInputListLexiconsPaginateTypeDef = TypedDict(
-    "ListLexiconsInputListLexiconsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLexiconsInputRequestTypeDef = TypedDict(
     "ListLexiconsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef = TypedDict(
-    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
-    {
-        "Status": TaskStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSpeechSynthesisTasksInputRequestTypeDef = TypedDict(
     "ListSpeechSynthesisTasksInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Status": TaskStatusType,
     },
     total=False,
 )
 
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
 PutLexiconInputRequestTypeDef = TypedDict(
     "PutLexiconInputRequestTypeDef",
     {
         "Name": str,
         "Content": str,
     },
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
 _RequiredStartSpeechSynthesisTaskInputRequestTypeDef = TypedDict(
     "_RequiredStartSpeechSynthesisTaskInputRequestTypeDef",
     {
         "OutputFormat": OutputFormatType,
         "OutputS3BucketName": str,
         "Text": str,
         "VoiceId": VoiceIdType,
@@ -279,30 +251,58 @@
 )
 
 class SynthesizeSpeechInputRequestTypeDef(
     _RequiredSynthesizeSpeechInputRequestTypeDef, _OptionalSynthesizeSpeechInputRequestTypeDef
 ):
     pass
 
+DescribeVoicesInputDescribeVoicesPaginateTypeDef = TypedDict(
+    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
+    {
+        "Engine": EngineType,
+        "LanguageCode": LanguageCodeType,
+        "IncludeAdditionalLanguageCodes": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListLexiconsInputListLexiconsPaginateTypeDef = TypedDict(
+    "ListLexiconsInputListLexiconsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef = TypedDict(
+    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
+    {
+        "Status": TaskStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 SynthesizeSpeechOutputTypeDef = TypedDict(
     "SynthesizeSpeechOutputTypeDef",
     {
         "AudioStream": StreamingBody,
         "ContentType": str,
         "RequestCharacters": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVoicesOutputTypeDef = TypedDict(
     "DescribeVoicesOutputTypeDef",
     {
         "Voices": List[VoiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LexiconDescriptionTypeDef = TypedDict(
     "LexiconDescriptionTypeDef",
     {
         "Name": str,
@@ -312,44 +312,44 @@
 )
 
 GetLexiconOutputTypeDef = TypedDict(
     "GetLexiconOutputTypeDef",
     {
         "Lexicon": LexiconTypeDef,
         "LexiconAttributes": LexiconAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSpeechSynthesisTaskOutputTypeDef = TypedDict(
     "GetSpeechSynthesisTaskOutputTypeDef",
     {
         "SynthesisTask": SynthesisTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSpeechSynthesisTasksOutputTypeDef = TypedDict(
     "ListSpeechSynthesisTasksOutputTypeDef",
     {
         "NextToken": str,
         "SynthesisTasks": List[SynthesisTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSpeechSynthesisTaskOutputTypeDef = TypedDict(
     "StartSpeechSynthesisTaskOutputTypeDef",
     {
         "SynthesisTask": SynthesisTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLexiconsOutputTypeDef = TypedDict(
     "ListLexiconsOutputTypeDef",
     {
         "Lexicons": List[LexiconDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-polly-1.28.0/mypy_boto3_polly.egg-info/PKG-INFO` & `mypy-boto3-polly-1.28.12/mypy_boto3_polly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-polly
-Version: 1.28.0
-Summary: Type annotations for boto3.Polly 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Polly 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-polly"></a>
 
 # mypy-boto3-polly
 
 [![PyPI - mypy-boto3-polly](https://img.shields.io/pypi/v/mypy-boto3-polly.svg?color=blue)](https://pypi.org/project/mypy-boto3-polly)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-polly.svg?color=blue)](https://pypi.org/project/mypy-boto3-polly)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-polly?color=blue)](https://pypistats.org/packages/mypy-boto3-polly)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-polly)](https://pepy.tech/project/mypy-boto3-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Polly 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[boto3.Polly 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
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
 [mypy-boto3-polly docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/).
 
 See how it helps to find and fix potential bugs:
 
@@ -337,31 +337,31 @@
 
 `mypy_boto3_polly.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_polly.type_defs import (
     DeleteLexiconInputRequestTypeDef,
-    DescribeVoicesInputDescribeVoicesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeVoicesInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     VoiceTypeDef,
     GetLexiconInputRequestTypeDef,
     LexiconAttributesTypeDef,
     LexiconTypeDef,
     GetSpeechSynthesisTaskInputRequestTypeDef,
     SynthesisTaskTypeDef,
-    ListLexiconsInputListLexiconsPaginateTypeDef,
     ListLexiconsInputRequestTypeDef,
-    ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef,
     ListSpeechSynthesisTasksInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutLexiconInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartSpeechSynthesisTaskInputRequestTypeDef,
     SynthesizeSpeechInputRequestTypeDef,
+    DescribeVoicesInputDescribeVoicesPaginateTypeDef,
+    ListLexiconsInputListLexiconsPaginateTypeDef,
+    ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef,
     SynthesizeSpeechOutputTypeDef,
     DescribeVoicesOutputTypeDef,
     LexiconDescriptionTypeDef,
     GetLexiconOutputTypeDef,
     GetSpeechSynthesisTaskOutputTypeDef,
     ListSpeechSynthesisTasksOutputTypeDef,
     StartSpeechSynthesisTaskOutputTypeDef,
```

### Comparing `mypy-boto3-polly-1.28.0/mypy_boto3_polly.egg-info/SOURCES.txt` & `mypy-boto3-polly-1.28.12/mypy_boto3_polly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.0/setup.py` & `mypy-boto3-polly-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-polly",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_polly"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Polly 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Polly 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

