# Comparing `tmp/mypy-boto3-lexv2-runtime-1.28.0.tar.gz` & `tmp/mypy-boto3-lexv2-runtime-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lexv2-runtime-1.28.0.tar", last modified: Thu Jul  6 20:59:58 2023, max compression
+gzip compressed data, was "mypy-boto3-lexv2-runtime-1.28.12.tar", last modified: Thu Jul 27 05:34:55 2023, max compression
```

## Comparing `mypy-boto3-lexv2-runtime-1.28.0.tar` & `mypy-boto3-lexv2-runtime-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:58.342351 mypy-boto3-lexv2-runtime-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:45:39.000000 mypy-boto3-lexv2-runtime-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13148 2023-07-06 20:59:58.342351 mypy-boto3-lexv2-runtime-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-07-06 20:45:39.000000 mypy-boto3-lexv2-runtime-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:58.334351 mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-06 20:45:39.000000 mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-06 20:45:39.000000 mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-06 20:45:39.000000 mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-06 20:45:39.000000 mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-07-06 20:45:39.000000 mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-07-06 20:45:39.000000 mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-07-06 20:45:39.000000 mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:45:39.000000 mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-07-06 20:45:40.000000 mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-07-06 20:45:40.000000 mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:45:39.000000 mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:58.342351 mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13148 2023-07-06 20:59:58.000000 mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-06 20:59:58.000000 mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:58.000000 mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:58.000000 mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:58.000000 mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 20:59:58.000000 mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:58.342351 mypy-boto3-lexv2-runtime-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-06 20:45:39.000000 mypy-boto3-lexv2-runtime-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.916460 mypy-boto3-lexv2-runtime-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-07-27 05:34:55.916460 mypy-boto3-lexv2-runtime-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.908460 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16324 2023-07-27 05:25:18.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16292 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.916460 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-07-27 05:34:55.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-27 05:34:55.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:55.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 05:34:55.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:55.916460 mypy-boto3-lexv2-runtime-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/setup.py
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.0/LICENSE` & `mypy-boto3-lexv2-runtime-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-runtime-1.28.0/PKG-INFO` & `mypy-boto3-lexv2-runtime-1.28.12/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lexv2-runtime
-Version: 1.28.0
-Summary: Type annotations for boto3.LexRuntimeV2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.LexRuntimeV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lexv2-runtime"></a>
 
 # mypy-boto3-lexv2-runtime
 
 [![PyPI - mypy-boto3-lexv2-runtime](https://img.shields.io/pypi/v/mypy-boto3-lexv2-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lexv2-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lexv2-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-lexv2-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lexv2-runtime)](https://pepy.tech/project/mypy-boto3-lexv2-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
+[boto3.LexRuntimeV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
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
 [mypy-boto3-lexv2-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,48 +303,62 @@
 ### Typed dictionaries
 
 `mypy_boto3_lexv2_runtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lexv2_runtime.type_defs import (
+    ActiveContextOutputTypeDef,
+    ActiveContextTimeToLiveOutputTypeDef,
     ActiveContextTimeToLiveTypeDef,
+    ActiveContextTypeDef,
+    ButtonOutputTypeDef,
     ButtonTypeDef,
     ConfidenceScoreTypeDef,
     DeleteSessionRequestRequestTypeDef,
     DeleteSessionResponseTypeDef,
+    DialogActionOutputTypeDef,
     DialogActionTypeDef,
+    ElicitSubSlotOutputTypeDef,
     ElicitSubSlotTypeDef,
     GetSessionRequestRequestTypeDef,
+    GetSessionResponseTypeDef,
+    ImageResponseCardOutputTypeDef,
+    ImageResponseCardTypeDef,
+    IntentOutputTypeDef,
     IntentTypeDef,
+    InterpretationTypeDef,
+    MessageOutputTypeDef,
+    MessageTypeDef,
+    PutSessionRequestRequestTypeDef,
     PutSessionResponseTypeDef,
-    RecognizedBotMemberTypeDef,
+    RecognizeTextRequestRequestTypeDef,
+    RecognizeTextResponseTypeDef,
     RecognizeUtteranceRequestRequestTypeDef,
     RecognizeUtteranceResponseTypeDef,
+    RecognizedBotMemberTypeDef,
     ResponseMetadataTypeDef,
+    RuntimeHintDetailsOutputTypeDef,
+    RuntimeHintDetailsTypeDef,
+    RuntimeHintValueOutputTypeDef,
     RuntimeHintValueTypeDef,
+    RuntimeHintsOutputTypeDef,
     RuntimeHintsTypeDef,
-    SentimentScoreTypeDef,
-    ValueTypeDef,
-    ActiveContextTypeDef,
-    ImageResponseCardTypeDef,
-    RuntimeHintDetailsTypeDef,
     SentimentResponseTypeDef,
-    SlotTypeDef,
+    SentimentScoreTypeDef,
+    SessionStateOutputTypeDef,
     SessionStateTypeDef,
-    MessageTypeDef,
-    InterpretationTypeDef,
-    RecognizeTextRequestRequestTypeDef,
-    PutSessionRequestRequestTypeDef,
-    GetSessionResponseTypeDef,
-    RecognizeTextResponseTypeDef,
+    SlotOutputTypeDef,
+    SlotTypeDef,
+    ValueOutputTypeDef,
+    ValueTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTimeToLiveTypeDef:
+def get_structure() -> ActiveContextOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.0/README.md` & `mypy-boto3-lexv2-runtime-1.28.12/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-lexv2-runtime"></a>
 
 # mypy-boto3-lexv2-runtime
 
 [![PyPI - mypy-boto3-lexv2-runtime](https://img.shields.io/pypi/v/mypy-boto3-lexv2-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lexv2-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lexv2-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-lexv2-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lexv2-runtime)](https://pepy.tech/project/mypy-boto3-lexv2-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
+[boto3.LexRuntimeV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
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
 [mypy-boto3-lexv2-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -271,48 +271,62 @@
 ### Typed dictionaries
 
 `mypy_boto3_lexv2_runtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lexv2_runtime.type_defs import (
+    ActiveContextOutputTypeDef,
+    ActiveContextTimeToLiveOutputTypeDef,
     ActiveContextTimeToLiveTypeDef,
+    ActiveContextTypeDef,
+    ButtonOutputTypeDef,
     ButtonTypeDef,
     ConfidenceScoreTypeDef,
     DeleteSessionRequestRequestTypeDef,
     DeleteSessionResponseTypeDef,
+    DialogActionOutputTypeDef,
     DialogActionTypeDef,
+    ElicitSubSlotOutputTypeDef,
     ElicitSubSlotTypeDef,
     GetSessionRequestRequestTypeDef,
+    GetSessionResponseTypeDef,
+    ImageResponseCardOutputTypeDef,
+    ImageResponseCardTypeDef,
+    IntentOutputTypeDef,
     IntentTypeDef,
+    InterpretationTypeDef,
+    MessageOutputTypeDef,
+    MessageTypeDef,
+    PutSessionRequestRequestTypeDef,
     PutSessionResponseTypeDef,
-    RecognizedBotMemberTypeDef,
+    RecognizeTextRequestRequestTypeDef,
+    RecognizeTextResponseTypeDef,
     RecognizeUtteranceRequestRequestTypeDef,
     RecognizeUtteranceResponseTypeDef,
+    RecognizedBotMemberTypeDef,
     ResponseMetadataTypeDef,
+    RuntimeHintDetailsOutputTypeDef,
+    RuntimeHintDetailsTypeDef,
+    RuntimeHintValueOutputTypeDef,
     RuntimeHintValueTypeDef,
+    RuntimeHintsOutputTypeDef,
     RuntimeHintsTypeDef,
-    SentimentScoreTypeDef,
-    ValueTypeDef,
-    ActiveContextTypeDef,
-    ImageResponseCardTypeDef,
-    RuntimeHintDetailsTypeDef,
     SentimentResponseTypeDef,
-    SlotTypeDef,
+    SentimentScoreTypeDef,
+    SessionStateOutputTypeDef,
     SessionStateTypeDef,
-    MessageTypeDef,
-    InterpretationTypeDef,
-    RecognizeTextRequestRequestTypeDef,
-    PutSessionRequestRequestTypeDef,
-    GetSessionResponseTypeDef,
-    RecognizeTextResponseTypeDef,
+    SlotOutputTypeDef,
+    SlotTypeDef,
+    ValueOutputTypeDef,
+    ValueTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTimeToLiveTypeDef:
+def get_structure() -> ActiveContextOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime/client.py` & `mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,16 +121,16 @@
     def put_session(
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
-        sessionState: SessionStateTypeDef,
-        messages: Sequence[MessageTypeDef] = ...,
+        sessionState: "SessionStateTypeDef",
+        messages: Sequence["MessageTypeDef"] = ...,
         requestAttributes: Mapping[str, str] = ...,
         responseContentType: str = ...
     ) -> PutSessionResponseTypeDef:
         """
         Creates a new session or modifies an existing session with an Amazon Lex V2 bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.put_session)
@@ -141,15 +141,15 @@
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
         text: str,
-        sessionState: SessionStateTypeDef = ...,
+        sessionState: "SessionStateTypeDef" = ...,
         requestAttributes: Mapping[str, str] = ...
     ) -> RecognizeTextResponseTypeDef:
         """
         Sends user input to Amazon Lex V2.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.recognize_text)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#recognize_text)
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime/client.pyi` & `mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -112,16 +112,16 @@
     def put_session(
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
-        sessionState: SessionStateTypeDef,
-        messages: Sequence[MessageTypeDef] = ...,
+        sessionState: "SessionStateTypeDef",
+        messages: Sequence["MessageTypeDef"] = ...,
         requestAttributes: Mapping[str, str] = ...,
         responseContentType: str = ...
     ) -> PutSessionResponseTypeDef:
         """
         Creates a new session or modifies an existing session with an Amazon Lex V2 bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.put_session)
@@ -131,15 +131,15 @@
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
         text: str,
-        sessionState: SessionStateTypeDef = ...,
+        sessionState: "SessionStateTypeDef" = ...,
         requestAttributes: Mapping[str, str] = ...
     ) -> RecognizeTextResponseTypeDef:
         """
         Sends user input to Amazon Lex V2.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.recognize_text)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#recognize_text)
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime/literals.py` & `mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,15 @@
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
@@ -247,26 +248,28 @@
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

### Comparing `mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime/literals.pyi` & `mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,15 @@
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
@@ -245,26 +246,28 @@
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

### Comparing `mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime.egg-info/PKG-INFO` & `mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lexv2-runtime
-Version: 1.28.0
-Summary: Type annotations for boto3.LexRuntimeV2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.LexRuntimeV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lexv2-runtime"></a>
 
 # mypy-boto3-lexv2-runtime
 
 [![PyPI - mypy-boto3-lexv2-runtime](https://img.shields.io/pypi/v/mypy-boto3-lexv2-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lexv2-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lexv2-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-lexv2-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lexv2-runtime)](https://pepy.tech/project/mypy-boto3-lexv2-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
+[boto3.LexRuntimeV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
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
 [mypy-boto3-lexv2-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,48 +303,62 @@
 ### Typed dictionaries
 
 `mypy_boto3_lexv2_runtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lexv2_runtime.type_defs import (
+    ActiveContextOutputTypeDef,
+    ActiveContextTimeToLiveOutputTypeDef,
     ActiveContextTimeToLiveTypeDef,
+    ActiveContextTypeDef,
+    ButtonOutputTypeDef,
     ButtonTypeDef,
     ConfidenceScoreTypeDef,
     DeleteSessionRequestRequestTypeDef,
     DeleteSessionResponseTypeDef,
+    DialogActionOutputTypeDef,
     DialogActionTypeDef,
+    ElicitSubSlotOutputTypeDef,
     ElicitSubSlotTypeDef,
     GetSessionRequestRequestTypeDef,
+    GetSessionResponseTypeDef,
+    ImageResponseCardOutputTypeDef,
+    ImageResponseCardTypeDef,
+    IntentOutputTypeDef,
     IntentTypeDef,
+    InterpretationTypeDef,
+    MessageOutputTypeDef,
+    MessageTypeDef,
+    PutSessionRequestRequestTypeDef,
     PutSessionResponseTypeDef,
-    RecognizedBotMemberTypeDef,
+    RecognizeTextRequestRequestTypeDef,
+    RecognizeTextResponseTypeDef,
     RecognizeUtteranceRequestRequestTypeDef,
     RecognizeUtteranceResponseTypeDef,
+    RecognizedBotMemberTypeDef,
     ResponseMetadataTypeDef,
+    RuntimeHintDetailsOutputTypeDef,
+    RuntimeHintDetailsTypeDef,
+    RuntimeHintValueOutputTypeDef,
     RuntimeHintValueTypeDef,
+    RuntimeHintsOutputTypeDef,
     RuntimeHintsTypeDef,
-    SentimentScoreTypeDef,
-    ValueTypeDef,
-    ActiveContextTypeDef,
-    ImageResponseCardTypeDef,
-    RuntimeHintDetailsTypeDef,
     SentimentResponseTypeDef,
-    SlotTypeDef,
+    SentimentScoreTypeDef,
+    SessionStateOutputTypeDef,
     SessionStateTypeDef,
-    MessageTypeDef,
-    InterpretationTypeDef,
-    RecognizeTextRequestRequestTypeDef,
-    PutSessionRequestRequestTypeDef,
-    GetSessionResponseTypeDef,
-    RecognizeTextResponseTypeDef,
+    SlotOutputTypeDef,
+    SlotTypeDef,
+    ValueOutputTypeDef,
+    ValueTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTimeToLiveTypeDef:
+def get_structure() -> ActiveContextOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.0/mypy_boto3_lexv2_runtime.egg-info/SOURCES.txt` & `mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-runtime-1.28.0/setup.py` & `mypy-boto3-lexv2-runtime-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lexv2-runtime",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_lexv2_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LexRuntimeV2 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.LexRuntimeV2 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

