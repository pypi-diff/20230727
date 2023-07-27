# Comparing `tmp/mypy-boto3-lex-models-1.28.0.tar.gz` & `tmp/mypy-boto3-lex-models-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lex-models-1.28.0.tar", last modified: Thu Jul  6 20:59:57 2023, max compression
+gzip compressed data, was "mypy-boto3-lex-models-1.28.12.tar", last modified: Thu Jul 27 05:34:55 2023, max compression
```

## Comparing `mypy-boto3-lex-models-1.28.0.tar` & `mypy-boto3-lex-models-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:57.814350 mypy-boto3-lex-models-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:45:14.000000 mypy-boto3-lex-models-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19255 2023-07-06 20:59:57.814350 mypy-boto3-lex-models-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17745 2023-07-06 20:45:14.000000 mypy-boto3-lex-models-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:57.802350 mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-06 20:45:14.000000 mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-06 20:45:14.000000 mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-06 20:45:14.000000 mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35106 2023-07-06 20:45:15.000000 mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35047 2023-07-06 20:45:14.000000 mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-07-06 20:45:15.000000 mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11145 2023-07-06 20:45:15.000000 mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-07-06 20:45:15.000000 mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-07-06 20:45:15.000000 mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:45:14.000000 mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46070 2023-07-06 20:45:16.000000 mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46017 2023-07-06 20:45:16.000000 mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:45:14.000000 mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:57.814350 mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19255 2023-07-06 20:59:57.000000 mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-06 20:59:57.000000 mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:57.000000 mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:57.000000 mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:57.000000 mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 20:59:57.000000 mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:57.814350 mypy-boto3-lex-models-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-06 20:45:14.000000 mypy-boto3-lex-models-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.716460 mypy-boto3-lex-models-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19784 2023-07-27 05:34:55.716460 mypy-boto3-lex-models-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18272 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.716460 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35106 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35047 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11225 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    51752 2023-07-27 05:25:00.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51686 2023-07-27 05:25:00.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.716460 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19784 2023-07-27 05:34:55.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:55.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:55.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:55.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:55.716460 mypy-boto3-lex-models-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/setup.py
```

### Comparing `mypy-boto3-lex-models-1.28.0/LICENSE` & `mypy-boto3-lex-models-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.0/PKG-INFO` & `mypy-boto3-lex-models-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lex-models
-Version: 1.28.0
-Summary: Type annotations for boto3.LexModelBuildingService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.LexModelBuildingService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lex-models"></a>
 
 # mypy-boto3-lex-models
 
 [![PyPI - mypy-boto3-lex-models](https://img.shields.io/pypi/v/mypy-boto3-lex-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-models)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-models)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lex-models?color=blue)](https://pypistats.org/packages/mypy-boto3-lex-models)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lex-models)](https://pepy.tech/project/mypy-boto3-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexModelBuildingService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
+[boto3.LexModelBuildingService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
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
 [mypy-boto3-lex-models docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/).
 
 See how it helps to find and fix potential bugs:
 
@@ -386,35 +386,37 @@
 ```python
 from mypy_boto3_lex_models.type_defs import (
     BotChannelAssociationTypeDef,
     BotMetadataTypeDef,
     BuiltinIntentMetadataTypeDef,
     BuiltinIntentSlotTypeDef,
     BuiltinSlotTypeMetadataTypeDef,
+    CodeHookOutputTypeDef,
     CodeHookTypeDef,
     LogSettingsRequestTypeDef,
     LogSettingsResponseTypeDef,
     CreateBotVersionRequestRequestTypeDef,
-    IntentTypeDef,
+    IntentOutputTypeDef,
     CreateIntentVersionRequestRequestTypeDef,
-    InputContextTypeDef,
-    KendraConfigurationTypeDef,
-    OutputContextTypeDef,
+    InputContextOutputTypeDef,
+    KendraConfigurationOutputTypeDef,
+    OutputContextOutputTypeDef,
     CreateSlotTypeVersionRequestRequestTypeDef,
-    EnumerationValueTypeDef,
+    EnumerationValueOutputTypeDef,
     DeleteBotAliasRequestRequestTypeDef,
     DeleteBotChannelAssociationRequestRequestTypeDef,
     DeleteBotRequestRequestTypeDef,
     DeleteBotVersionRequestRequestTypeDef,
     DeleteIntentRequestRequestTypeDef,
     DeleteIntentVersionRequestRequestTypeDef,
     DeleteSlotTypeRequestRequestTypeDef,
     DeleteSlotTypeVersionRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
+    EnumerationValueTypeDef,
     GetBotAliasRequestRequestTypeDef,
     GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
     GetBotAliasesRequestRequestTypeDef,
     GetBotChannelAssociationRequestRequestTypeDef,
     GetBotChannelAssociationResponseTypeDef,
     GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
     GetBotChannelAssociationsRequestRequestTypeDef,
@@ -445,69 +447,84 @@
     GetSlotTypeRequestRequestTypeDef,
     GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
     GetSlotTypeVersionsRequestRequestTypeDef,
     SlotTypeMetadataTypeDef,
     GetSlotTypesRequestGetSlotTypesPaginateTypeDef,
     GetSlotTypesRequestRequestTypeDef,
     GetUtterancesViewRequestRequestTypeDef,
+    InputContextTypeDef,
+    IntentTypeDef,
+    KendraConfigurationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
+    MessageOutputTypeDef,
     MessageTypeDef,
+    OutputContextTypeDef,
     PaginatorConfigTypeDef,
+    TagTypeDef,
     ResponseMetadataTypeDef,
+    SlotDefaultValueOutputTypeDef,
     SlotDefaultValueTypeDef,
+    SlotTypeRegexConfigurationOutputTypeDef,
     SlotTypeRegexConfigurationTypeDef,
     StartMigrationRequestRequestTypeDef,
     StartMigrationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UtteranceDataTypeDef,
     GetBotChannelAssociationsResponseTypeDef,
     GetBotVersionsResponseTypeDef,
     GetBotsResponseTypeDef,
     GetBuiltinIntentsResponseTypeDef,
     GetBuiltinIntentResponseTypeDef,
     GetBuiltinSlotTypesResponseTypeDef,
+    FulfillmentActivityOutputTypeDef,
     FulfillmentActivityTypeDef,
     ConversationLogsRequestTypeDef,
     ConversationLogsResponseTypeDef,
     GetIntentVersionsResponseTypeDef,
     GetIntentsResponseTypeDef,
     GetMigrationResponseTypeDef,
     GetMigrationsResponseTypeDef,
     GetSlotTypeVersionsResponseTypeDef,
     GetSlotTypesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
+    PromptOutputTypeDef,
+    StatementOutputTypeDef,
     PromptTypeDef,
     StatementTypeDef,
+    StartImportRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    SlotDefaultValueSpecOutputTypeDef,
     SlotDefaultValueSpecTypeDef,
+    SlotTypeConfigurationOutputTypeDef,
     SlotTypeConfigurationTypeDef,
     UtteranceListTypeDef,
     PutBotAliasRequestRequestTypeDef,
     BotAliasMetadataTypeDef,
     GetBotAliasResponseTypeDef,
     PutBotAliasResponseTypeDef,
     CreateBotVersionResponseTypeDef,
-    FollowUpPromptTypeDef,
+    FollowUpPromptOutputTypeDef,
     GetBotResponseTypeDef,
-    PutBotRequestRequestTypeDef,
     PutBotResponseTypeDef,
+    FollowUpPromptTypeDef,
+    PutBotRequestRequestTypeDef,
+    SlotOutputTypeDef,
     SlotTypeDef,
     CreateSlotTypeVersionResponseTypeDef,
     GetSlotTypeResponseTypeDef,
-    PutSlotTypeRequestRequestTypeDef,
     PutSlotTypeResponseTypeDef,
+    PutSlotTypeRequestRequestTypeDef,
     GetUtterancesViewResponseTypeDef,
     GetBotAliasesResponseTypeDef,
     CreateIntentVersionResponseTypeDef,
     GetIntentResponseTypeDef,
-    PutIntentRequestRequestTypeDef,
     PutIntentResponseTypeDef,
+    PutIntentRequestRequestTypeDef,
 )
 
 
 def get_structure() -> BotChannelAssociationTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-lex-models-1.28.0/README.md` & `mypy-boto3-lex-models-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-lex-models"></a>
 
 # mypy-boto3-lex-models
 
 [![PyPI - mypy-boto3-lex-models](https://img.shields.io/pypi/v/mypy-boto3-lex-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-models)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-models)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lex-models?color=blue)](https://pypistats.org/packages/mypy-boto3-lex-models)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lex-models)](https://pepy.tech/project/mypy-boto3-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexModelBuildingService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
+[boto3.LexModelBuildingService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
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
 [mypy-boto3-lex-models docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,35 +354,37 @@
 ```python
 from mypy_boto3_lex_models.type_defs import (
     BotChannelAssociationTypeDef,
     BotMetadataTypeDef,
     BuiltinIntentMetadataTypeDef,
     BuiltinIntentSlotTypeDef,
     BuiltinSlotTypeMetadataTypeDef,
+    CodeHookOutputTypeDef,
     CodeHookTypeDef,
     LogSettingsRequestTypeDef,
     LogSettingsResponseTypeDef,
     CreateBotVersionRequestRequestTypeDef,
-    IntentTypeDef,
+    IntentOutputTypeDef,
     CreateIntentVersionRequestRequestTypeDef,
-    InputContextTypeDef,
-    KendraConfigurationTypeDef,
-    OutputContextTypeDef,
+    InputContextOutputTypeDef,
+    KendraConfigurationOutputTypeDef,
+    OutputContextOutputTypeDef,
     CreateSlotTypeVersionRequestRequestTypeDef,
-    EnumerationValueTypeDef,
+    EnumerationValueOutputTypeDef,
     DeleteBotAliasRequestRequestTypeDef,
     DeleteBotChannelAssociationRequestRequestTypeDef,
     DeleteBotRequestRequestTypeDef,
     DeleteBotVersionRequestRequestTypeDef,
     DeleteIntentRequestRequestTypeDef,
     DeleteIntentVersionRequestRequestTypeDef,
     DeleteSlotTypeRequestRequestTypeDef,
     DeleteSlotTypeVersionRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
+    EnumerationValueTypeDef,
     GetBotAliasRequestRequestTypeDef,
     GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
     GetBotAliasesRequestRequestTypeDef,
     GetBotChannelAssociationRequestRequestTypeDef,
     GetBotChannelAssociationResponseTypeDef,
     GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
     GetBotChannelAssociationsRequestRequestTypeDef,
@@ -413,69 +415,84 @@
     GetSlotTypeRequestRequestTypeDef,
     GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
     GetSlotTypeVersionsRequestRequestTypeDef,
     SlotTypeMetadataTypeDef,
     GetSlotTypesRequestGetSlotTypesPaginateTypeDef,
     GetSlotTypesRequestRequestTypeDef,
     GetUtterancesViewRequestRequestTypeDef,
+    InputContextTypeDef,
+    IntentTypeDef,
+    KendraConfigurationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
+    MessageOutputTypeDef,
     MessageTypeDef,
+    OutputContextTypeDef,
     PaginatorConfigTypeDef,
+    TagTypeDef,
     ResponseMetadataTypeDef,
+    SlotDefaultValueOutputTypeDef,
     SlotDefaultValueTypeDef,
+    SlotTypeRegexConfigurationOutputTypeDef,
     SlotTypeRegexConfigurationTypeDef,
     StartMigrationRequestRequestTypeDef,
     StartMigrationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UtteranceDataTypeDef,
     GetBotChannelAssociationsResponseTypeDef,
     GetBotVersionsResponseTypeDef,
     GetBotsResponseTypeDef,
     GetBuiltinIntentsResponseTypeDef,
     GetBuiltinIntentResponseTypeDef,
     GetBuiltinSlotTypesResponseTypeDef,
+    FulfillmentActivityOutputTypeDef,
     FulfillmentActivityTypeDef,
     ConversationLogsRequestTypeDef,
     ConversationLogsResponseTypeDef,
     GetIntentVersionsResponseTypeDef,
     GetIntentsResponseTypeDef,
     GetMigrationResponseTypeDef,
     GetMigrationsResponseTypeDef,
     GetSlotTypeVersionsResponseTypeDef,
     GetSlotTypesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
+    PromptOutputTypeDef,
+    StatementOutputTypeDef,
     PromptTypeDef,
     StatementTypeDef,
+    StartImportRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    SlotDefaultValueSpecOutputTypeDef,
     SlotDefaultValueSpecTypeDef,
+    SlotTypeConfigurationOutputTypeDef,
     SlotTypeConfigurationTypeDef,
     UtteranceListTypeDef,
     PutBotAliasRequestRequestTypeDef,
     BotAliasMetadataTypeDef,
     GetBotAliasResponseTypeDef,
     PutBotAliasResponseTypeDef,
     CreateBotVersionResponseTypeDef,
-    FollowUpPromptTypeDef,
+    FollowUpPromptOutputTypeDef,
     GetBotResponseTypeDef,
-    PutBotRequestRequestTypeDef,
     PutBotResponseTypeDef,
+    FollowUpPromptTypeDef,
+    PutBotRequestRequestTypeDef,
+    SlotOutputTypeDef,
     SlotTypeDef,
     CreateSlotTypeVersionResponseTypeDef,
     GetSlotTypeResponseTypeDef,
-    PutSlotTypeRequestRequestTypeDef,
     PutSlotTypeResponseTypeDef,
+    PutSlotTypeRequestRequestTypeDef,
     GetUtterancesViewResponseTypeDef,
     GetBotAliasesResponseTypeDef,
     CreateIntentVersionResponseTypeDef,
     GetIntentResponseTypeDef,
-    PutIntentRequestRequestTypeDef,
     PutIntentResponseTypeDef,
+    PutIntentRequestRequestTypeDef,
 )
 
 
 def get_structure() -> BotChannelAssociationTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/__init__.py` & `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/__init__.pyi` & `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/__main__.py` & `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LexModelBuildingService 1.28.0\nVersion:        "
-        " 1.28.0\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.LexModelBuildingService 1.28.12\nVersion:        "
+        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService\nOther"
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

### Comparing `mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/client.py` & `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/client.pyi` & `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/literals.py` & `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ChannelStatusType",
     "ChannelTypeType",
     "ContentTypeType",
     "DestinationType",
     "ExportStatusType",
     "ExportTypeType",
@@ -56,15 +55,14 @@
     "LexModelBuildingServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ChannelStatusType = Literal["CREATED", "FAILED", "IN_PROGRESS"]
 ChannelTypeType = Literal["Facebook", "Kik", "Slack", "Twilio-Sms"]
 ContentTypeType = Literal["CustomPayload", "PlainText", "SSML"]
 DestinationType = Literal["CLOUDWATCH_LOGS", "S3"]
 ExportStatusType = Literal["FAILED", "IN_PROGRESS", "READY"]
 ExportTypeType = Literal["ALEXA_SKILLS_KIT", "LEX"]
 FulfillmentActivityTypeType = Literal["CodeHook", "ReturnIntent"]
@@ -224,14 +222,15 @@
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
@@ -310,26 +309,28 @@
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

### Comparing `mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/literals.pyi` & `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ChannelStatusType",
     "ChannelTypeType",
     "ContentTypeType",
     "DestinationType",
     "ExportStatusType",
     "ExportTypeType",
@@ -55,14 +56,15 @@
     "LexModelBuildingServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ChannelStatusType = Literal["CREATED", "FAILED", "IN_PROGRESS"]
 ChannelTypeType = Literal["Facebook", "Kik", "Slack", "Twilio-Sms"]
 ContentTypeType = Literal["CustomPayload", "PlainText", "SSML"]
 DestinationType = Literal["CLOUDWATCH_LOGS", "S3"]
 ExportStatusType = Literal["FAILED", "IN_PROGRESS", "READY"]
 ExportTypeType = Literal["ALEXA_SKILLS_KIT", "LEX"]
 FulfillmentActivityTypeType = Literal["CodeHook", "ReturnIntent"]
@@ -222,14 +224,15 @@
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
@@ -308,26 +311,28 @@
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

### Comparing `mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/paginator.py` & `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/paginator.pyi` & `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/type_defs.py` & `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -44,42 +44,43 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BotChannelAssociationTypeDef",
     "BotMetadataTypeDef",
     "BuiltinIntentMetadataTypeDef",
     "BuiltinIntentSlotTypeDef",
     "BuiltinSlotTypeMetadataTypeDef",
+    "CodeHookOutputTypeDef",
     "CodeHookTypeDef",
     "LogSettingsRequestTypeDef",
     "LogSettingsResponseTypeDef",
     "CreateBotVersionRequestRequestTypeDef",
-    "IntentTypeDef",
+    "IntentOutputTypeDef",
     "CreateIntentVersionRequestRequestTypeDef",
-    "InputContextTypeDef",
-    "KendraConfigurationTypeDef",
-    "OutputContextTypeDef",
+    "InputContextOutputTypeDef",
+    "KendraConfigurationOutputTypeDef",
+    "OutputContextOutputTypeDef",
     "CreateSlotTypeVersionRequestRequestTypeDef",
-    "EnumerationValueTypeDef",
+    "EnumerationValueOutputTypeDef",
     "DeleteBotAliasRequestRequestTypeDef",
     "DeleteBotChannelAssociationRequestRequestTypeDef",
     "DeleteBotRequestRequestTypeDef",
     "DeleteBotVersionRequestRequestTypeDef",
     "DeleteIntentRequestRequestTypeDef",
     "DeleteIntentVersionRequestRequestTypeDef",
     "DeleteSlotTypeRequestRequestTypeDef",
     "DeleteSlotTypeVersionRequestRequestTypeDef",
     "DeleteUtterancesRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EnumerationValueTypeDef",
     "GetBotAliasRequestRequestTypeDef",
     "GetBotAliasesRequestGetBotAliasesPaginateTypeDef",
     "GetBotAliasesRequestRequestTypeDef",
     "GetBotChannelAssociationRequestRequestTypeDef",
     "GetBotChannelAssociationResponseTypeDef",
     "GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
     "GetBotChannelAssociationsRequestRequestTypeDef",
@@ -110,69 +111,84 @@
     "GetSlotTypeRequestRequestTypeDef",
     "GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
     "GetSlotTypeVersionsRequestRequestTypeDef",
     "SlotTypeMetadataTypeDef",
     "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
     "GetSlotTypesRequestRequestTypeDef",
     "GetUtterancesViewRequestRequestTypeDef",
+    "InputContextTypeDef",
+    "IntentTypeDef",
+    "KendraConfigurationTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
+    "MessageOutputTypeDef",
     "MessageTypeDef",
+    "OutputContextTypeDef",
     "PaginatorConfigTypeDef",
+    "TagTypeDef",
     "ResponseMetadataTypeDef",
+    "SlotDefaultValueOutputTypeDef",
     "SlotDefaultValueTypeDef",
+    "SlotTypeRegexConfigurationOutputTypeDef",
     "SlotTypeRegexConfigurationTypeDef",
     "StartMigrationRequestRequestTypeDef",
     "StartMigrationResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UtteranceDataTypeDef",
     "GetBotChannelAssociationsResponseTypeDef",
     "GetBotVersionsResponseTypeDef",
     "GetBotsResponseTypeDef",
     "GetBuiltinIntentsResponseTypeDef",
     "GetBuiltinIntentResponseTypeDef",
     "GetBuiltinSlotTypesResponseTypeDef",
+    "FulfillmentActivityOutputTypeDef",
     "FulfillmentActivityTypeDef",
     "ConversationLogsRequestTypeDef",
     "ConversationLogsResponseTypeDef",
     "GetIntentVersionsResponseTypeDef",
     "GetIntentsResponseTypeDef",
     "GetMigrationResponseTypeDef",
     "GetMigrationsResponseTypeDef",
     "GetSlotTypeVersionsResponseTypeDef",
     "GetSlotTypesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
+    "PromptOutputTypeDef",
+    "StatementOutputTypeDef",
     "PromptTypeDef",
     "StatementTypeDef",
+    "StartImportRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "SlotDefaultValueSpecOutputTypeDef",
     "SlotDefaultValueSpecTypeDef",
+    "SlotTypeConfigurationOutputTypeDef",
     "SlotTypeConfigurationTypeDef",
     "UtteranceListTypeDef",
     "PutBotAliasRequestRequestTypeDef",
     "BotAliasMetadataTypeDef",
     "GetBotAliasResponseTypeDef",
     "PutBotAliasResponseTypeDef",
     "CreateBotVersionResponseTypeDef",
-    "FollowUpPromptTypeDef",
+    "FollowUpPromptOutputTypeDef",
     "GetBotResponseTypeDef",
-    "PutBotRequestRequestTypeDef",
     "PutBotResponseTypeDef",
+    "FollowUpPromptTypeDef",
+    "PutBotRequestRequestTypeDef",
+    "SlotOutputTypeDef",
     "SlotTypeDef",
     "CreateSlotTypeVersionResponseTypeDef",
     "GetSlotTypeResponseTypeDef",
-    "PutSlotTypeRequestRequestTypeDef",
     "PutSlotTypeResponseTypeDef",
+    "PutSlotTypeRequestRequestTypeDef",
     "GetUtterancesViewResponseTypeDef",
     "GetBotAliasesResponseTypeDef",
     "CreateIntentVersionResponseTypeDef",
     "GetIntentResponseTypeDef",
-    "PutIntentRequestRequestTypeDef",
     "PutIntentResponseTypeDef",
+    "PutIntentRequestRequestTypeDef",
 )
 
 BotChannelAssociationTypeDef = TypedDict(
     "BotChannelAssociationTypeDef",
     {
         "name": str,
         "description": str,
@@ -222,14 +238,22 @@
     {
         "signature": str,
         "supportedLocales": List[LocaleType],
     },
     total=False,
 )
 
+CodeHookOutputTypeDef = TypedDict(
+    "CodeHookOutputTypeDef",
+    {
+        "uri": str,
+        "messageVersion": str,
+    },
+)
+
 CodeHookTypeDef = TypedDict(
     "CodeHookTypeDef",
     {
         "uri": str,
         "messageVersion": str,
     },
 )
@@ -246,21 +270,19 @@
     "_OptionalLogSettingsRequestTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
 
-
 class LogSettingsRequestTypeDef(
     _RequiredLogSettingsRequestTypeDef, _OptionalLogSettingsRequestTypeDef
 ):
     pass
 
-
 LogSettingsResponseTypeDef = TypedDict(
     "LogSettingsResponseTypeDef",
     {
         "logType": LogTypeType,
         "destination": DestinationType,
         "kmsKeyArn": str,
         "resourceArn": str,
@@ -279,23 +301,21 @@
     "_OptionalCreateBotVersionRequestRequestTypeDef",
     {
         "checksum": str,
     },
     total=False,
 )
 
-
 class CreateBotVersionRequestRequestTypeDef(
     _RequiredCreateBotVersionRequestRequestTypeDef, _OptionalCreateBotVersionRequestRequestTypeDef
 ):
     pass
 
-
-IntentTypeDef = TypedDict(
-    "IntentTypeDef",
+IntentOutputTypeDef = TypedDict(
+    "IntentOutputTypeDef",
     {
         "intentName": str,
         "intentVersion": str,
     },
 )
 
 _RequiredCreateIntentVersionRequestRequestTypeDef = TypedDict(
@@ -308,53 +328,49 @@
     "_OptionalCreateIntentVersionRequestRequestTypeDef",
     {
         "checksum": str,
     },
     total=False,
 )
 
-
 class CreateIntentVersionRequestRequestTypeDef(
     _RequiredCreateIntentVersionRequestRequestTypeDef,
     _OptionalCreateIntentVersionRequestRequestTypeDef,
 ):
     pass
 
-
-InputContextTypeDef = TypedDict(
-    "InputContextTypeDef",
+InputContextOutputTypeDef = TypedDict(
+    "InputContextOutputTypeDef",
     {
         "name": str,
     },
 )
 
-_RequiredKendraConfigurationTypeDef = TypedDict(
-    "_RequiredKendraConfigurationTypeDef",
+_RequiredKendraConfigurationOutputTypeDef = TypedDict(
+    "_RequiredKendraConfigurationOutputTypeDef",
     {
         "kendraIndex": str,
         "role": str,
     },
 )
-_OptionalKendraConfigurationTypeDef = TypedDict(
-    "_OptionalKendraConfigurationTypeDef",
+_OptionalKendraConfigurationOutputTypeDef = TypedDict(
+    "_OptionalKendraConfigurationOutputTypeDef",
     {
         "queryFilterString": str,
     },
     total=False,
 )
 
-
-class KendraConfigurationTypeDef(
-    _RequiredKendraConfigurationTypeDef, _OptionalKendraConfigurationTypeDef
+class KendraConfigurationOutputTypeDef(
+    _RequiredKendraConfigurationOutputTypeDef, _OptionalKendraConfigurationOutputTypeDef
 ):
     pass
 
-
-OutputContextTypeDef = TypedDict(
-    "OutputContextTypeDef",
+OutputContextOutputTypeDef = TypedDict(
+    "OutputContextOutputTypeDef",
     {
         "name": str,
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
     },
 )
 
@@ -368,41 +384,39 @@
     "_OptionalCreateSlotTypeVersionRequestRequestTypeDef",
     {
         "checksum": str,
     },
     total=False,
 )
 
-
 class CreateSlotTypeVersionRequestRequestTypeDef(
     _RequiredCreateSlotTypeVersionRequestRequestTypeDef,
     _OptionalCreateSlotTypeVersionRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredEnumerationValueTypeDef = TypedDict(
-    "_RequiredEnumerationValueTypeDef",
+_RequiredEnumerationValueOutputTypeDef = TypedDict(
+    "_RequiredEnumerationValueOutputTypeDef",
     {
         "value": str,
     },
 )
-_OptionalEnumerationValueTypeDef = TypedDict(
-    "_OptionalEnumerationValueTypeDef",
+_OptionalEnumerationValueOutputTypeDef = TypedDict(
+    "_OptionalEnumerationValueOutputTypeDef",
     {
         "synonyms": List[str],
     },
     total=False,
 )
 
-
-class EnumerationValueTypeDef(_RequiredEnumerationValueTypeDef, _OptionalEnumerationValueTypeDef):
+class EnumerationValueOutputTypeDef(
+    _RequiredEnumerationValueOutputTypeDef, _OptionalEnumerationValueOutputTypeDef
+):
     pass
 
-
 DeleteBotAliasRequestRequestTypeDef = TypedDict(
     "DeleteBotAliasRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
     },
 )
@@ -472,14 +486,31 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredEnumerationValueTypeDef = TypedDict(
+    "_RequiredEnumerationValueTypeDef",
+    {
+        "value": str,
+    },
+)
+_OptionalEnumerationValueTypeDef = TypedDict(
+    "_OptionalEnumerationValueTypeDef",
+    {
+        "synonyms": Sequence[str],
+    },
+    total=False,
+)
+
+class EnumerationValueTypeDef(_RequiredEnumerationValueTypeDef, _OptionalEnumerationValueTypeDef):
+    pass
+
 GetBotAliasRequestRequestTypeDef = TypedDict(
     "GetBotAliasRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
     },
 )
@@ -495,22 +526,20 @@
     {
         "nameContains": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class GetBotAliasesRequestGetBotAliasesPaginateTypeDef(
     _RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
     _OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetBotAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotAliasesRequestRequestTypeDef",
     {
         "botName": str,
     },
 )
 _OptionalGetBotAliasesRequestRequestTypeDef = TypedDict(
@@ -519,21 +548,19 @@
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
     total=False,
 )
 
-
 class GetBotAliasesRequestRequestTypeDef(
     _RequiredGetBotAliasesRequestRequestTypeDef, _OptionalGetBotAliasesRequestRequestTypeDef
 ):
     pass
 
-
 GetBotChannelAssociationRequestRequestTypeDef = TypedDict(
     "GetBotChannelAssociationRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
         "botAlias": str,
     },
@@ -567,22 +594,20 @@
     {
         "nameContains": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef(
     _RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
     _OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetBotChannelAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotChannelAssociationsRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
     },
 )
@@ -592,22 +617,20 @@
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
     total=False,
 )
 
-
 class GetBotChannelAssociationsRequestRequestTypeDef(
     _RequiredGetBotChannelAssociationsRequestRequestTypeDef,
     _OptionalGetBotChannelAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
 GetBotRequestRequestTypeDef = TypedDict(
     "GetBotRequestRequestTypeDef",
     {
         "name": str,
         "versionOrAlias": str,
     },
 )
@@ -622,22 +645,20 @@
     "_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class GetBotVersionsRequestGetBotVersionsPaginateTypeDef(
     _RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
     _OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetBotVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetBotVersionsRequestRequestTypeDef = TypedDict(
@@ -645,21 +666,19 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetBotVersionsRequestRequestTypeDef(
     _RequiredGetBotVersionsRequestRequestTypeDef, _OptionalGetBotVersionsRequestRequestTypeDef
 ):
     pass
 
-
 GetBotsRequestGetBotsPaginateTypeDef = TypedDict(
     "GetBotsRequestGetBotsPaginateTypeDef",
     {
         "nameContains": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -787,22 +806,20 @@
     "_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef(
     _RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
     _OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetIntentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetIntentVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetIntentVersionsRequestRequestTypeDef = TypedDict(
@@ -810,21 +827,19 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetIntentVersionsRequestRequestTypeDef(
     _RequiredGetIntentVersionsRequestRequestTypeDef, _OptionalGetIntentVersionsRequestRequestTypeDef
 ):
     pass
 
-
 IntentMetadataTypeDef = TypedDict(
     "IntentMetadataTypeDef",
     {
         "name": str,
         "description": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
@@ -917,22 +932,20 @@
     "_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef(
     _RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
     _OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetSlotTypeVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSlotTypeVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetSlotTypeVersionsRequestRequestTypeDef = TypedDict(
@@ -940,22 +953,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetSlotTypeVersionsRequestRequestTypeDef(
     _RequiredGetSlotTypeVersionsRequestRequestTypeDef,
     _OptionalGetSlotTypeVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 SlotTypeMetadataTypeDef = TypedDict(
     "SlotTypeMetadataTypeDef",
     {
         "name": str,
         "description": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
@@ -988,29 +999,82 @@
     {
         "botName": str,
         "botVersions": Sequence[str],
         "statusType": StatusTypeType,
     },
 )
 
+InputContextTypeDef = TypedDict(
+    "InputContextTypeDef",
+    {
+        "name": str,
+    },
+)
+
+IntentTypeDef = TypedDict(
+    "IntentTypeDef",
+    {
+        "intentName": str,
+        "intentVersion": str,
+    },
+)
+
+_RequiredKendraConfigurationTypeDef = TypedDict(
+    "_RequiredKendraConfigurationTypeDef",
+    {
+        "kendraIndex": str,
+        "role": str,
+    },
+)
+_OptionalKendraConfigurationTypeDef = TypedDict(
+    "_OptionalKendraConfigurationTypeDef",
+    {
+        "queryFilterString": str,
+    },
+    total=False,
+)
+
+class KendraConfigurationTypeDef(
+    _RequiredKendraConfigurationTypeDef, _OptionalKendraConfigurationTypeDef
+):
+    pass
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
+_RequiredMessageOutputTypeDef = TypedDict(
+    "_RequiredMessageOutputTypeDef",
+    {
+        "contentType": ContentTypeType,
+        "content": str,
+    },
+)
+_OptionalMessageOutputTypeDef = TypedDict(
+    "_OptionalMessageOutputTypeDef",
+    {
+        "groupNumber": int,
+    },
+    total=False,
+)
+
+class MessageOutputTypeDef(_RequiredMessageOutputTypeDef, _OptionalMessageOutputTypeDef):
+    pass
+
 _RequiredMessageTypeDef = TypedDict(
     "_RequiredMessageTypeDef",
     {
         "contentType": ContentTypeType,
         "content": str,
     },
 )
@@ -1018,47 +1082,76 @@
     "_OptionalMessageTypeDef",
     {
         "groupNumber": int,
     },
     total=False,
 )
 
-
 class MessageTypeDef(_RequiredMessageTypeDef, _OptionalMessageTypeDef):
     pass
 
+OutputContextTypeDef = TypedDict(
+    "OutputContextTypeDef",
+    {
+        "name": str,
+        "timeToLiveInSeconds": int,
+        "turnsToLive": int,
+    },
+)
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+SlotDefaultValueOutputTypeDef = TypedDict(
+    "SlotDefaultValueOutputTypeDef",
+    {
+        "defaultValue": str,
+    },
+)
+
 SlotDefaultValueTypeDef = TypedDict(
     "SlotDefaultValueTypeDef",
     {
         "defaultValue": str,
     },
 )
 
+SlotTypeRegexConfigurationOutputTypeDef = TypedDict(
+    "SlotTypeRegexConfigurationOutputTypeDef",
+    {
+        "pattern": str,
+    },
+)
+
 SlotTypeRegexConfigurationTypeDef = TypedDict(
     "SlotTypeRegexConfigurationTypeDef",
     {
         "pattern": str,
     },
 )
 
@@ -1159,35 +1252,52 @@
     {
         "slotTypes": List[BuiltinSlotTypeMetadataTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredFulfillmentActivityOutputTypeDef = TypedDict(
+    "_RequiredFulfillmentActivityOutputTypeDef",
+    {
+        "type": FulfillmentActivityTypeType,
+    },
+)
+_OptionalFulfillmentActivityOutputTypeDef = TypedDict(
+    "_OptionalFulfillmentActivityOutputTypeDef",
+    {
+        "codeHook": CodeHookOutputTypeDef,
+    },
+    total=False,
+)
+
+class FulfillmentActivityOutputTypeDef(
+    _RequiredFulfillmentActivityOutputTypeDef, _OptionalFulfillmentActivityOutputTypeDef
+):
+    pass
+
 _RequiredFulfillmentActivityTypeDef = TypedDict(
     "_RequiredFulfillmentActivityTypeDef",
     {
         "type": FulfillmentActivityTypeType,
     },
 )
 _OptionalFulfillmentActivityTypeDef = TypedDict(
     "_OptionalFulfillmentActivityTypeDef",
     {
         "codeHook": CodeHookTypeDef,
     },
     total=False,
 )
 
-
 class FulfillmentActivityTypeDef(
     _RequiredFulfillmentActivityTypeDef, _OptionalFulfillmentActivityTypeDef
 ):
     pass
 
-
 ConversationLogsRequestTypeDef = TypedDict(
     "ConversationLogsRequestTypeDef",
     {
         "logSettings": Sequence[LogSettingsRequestTypeDef],
         "iamRoleArn": str,
     },
 )
@@ -1262,110 +1372,154 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStartImportRequestRequestTypeDef = TypedDict(
-    "_RequiredStartImportRequestRequestTypeDef",
+StartImportResponseTypeDef = TypedDict(
+    "StartImportResponseTypeDef",
     {
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "name": str,
         "resourceType": ResourceTypeType,
         "mergeStrategy": MergeStrategyType,
+        "importId": str,
+        "importStatus": ImportStatusType,
+        "tags": List[TagOutputTypeDef],
+        "createdDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalStartImportRequestRequestTypeDef = TypedDict(
-    "_OptionalStartImportRequestRequestTypeDef",
+
+_RequiredPromptOutputTypeDef = TypedDict(
+    "_RequiredPromptOutputTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
+        "messages": List[MessageOutputTypeDef],
+        "maxAttempts": int,
+    },
+)
+_OptionalPromptOutputTypeDef = TypedDict(
+    "_OptionalPromptOutputTypeDef",
+    {
+        "responseCard": str,
     },
     total=False,
 )
 
-
-class StartImportRequestRequestTypeDef(
-    _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
-):
+class PromptOutputTypeDef(_RequiredPromptOutputTypeDef, _OptionalPromptOutputTypeDef):
     pass
 
-
-StartImportResponseTypeDef = TypedDict(
-    "StartImportResponseTypeDef",
+_RequiredStatementOutputTypeDef = TypedDict(
+    "_RequiredStatementOutputTypeDef",
     {
-        "name": str,
-        "resourceType": ResourceTypeType,
-        "mergeStrategy": MergeStrategyType,
-        "importId": str,
-        "importStatus": ImportStatusType,
-        "tags": List[TagTypeDef],
-        "createdDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "messages": List[MessageOutputTypeDef],
     },
 )
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+_OptionalStatementOutputTypeDef = TypedDict(
+    "_OptionalStatementOutputTypeDef",
     {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
+        "responseCard": str,
     },
+    total=False,
 )
 
+class StatementOutputTypeDef(_RequiredStatementOutputTypeDef, _OptionalStatementOutputTypeDef):
+    pass
+
 _RequiredPromptTypeDef = TypedDict(
     "_RequiredPromptTypeDef",
     {
-        "messages": List[MessageTypeDef],
+        "messages": Sequence[MessageTypeDef],
         "maxAttempts": int,
     },
 )
 _OptionalPromptTypeDef = TypedDict(
     "_OptionalPromptTypeDef",
     {
         "responseCard": str,
     },
     total=False,
 )
 
-
 class PromptTypeDef(_RequiredPromptTypeDef, _OptionalPromptTypeDef):
     pass
 
-
 _RequiredStatementTypeDef = TypedDict(
     "_RequiredStatementTypeDef",
     {
-        "messages": List[MessageTypeDef],
+        "messages": Sequence[MessageTypeDef],
     },
 )
 _OptionalStatementTypeDef = TypedDict(
     "_OptionalStatementTypeDef",
     {
         "responseCard": str,
     },
     total=False,
 )
 
-
 class StatementTypeDef(_RequiredStatementTypeDef, _OptionalStatementTypeDef):
     pass
 
+_RequiredStartImportRequestRequestTypeDef = TypedDict(
+    "_RequiredStartImportRequestRequestTypeDef",
+    {
+        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "resourceType": ResourceTypeType,
+        "mergeStrategy": MergeStrategyType,
+    },
+)
+_OptionalStartImportRequestRequestTypeDef = TypedDict(
+    "_OptionalStartImportRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class StartImportRequestRequestTypeDef(
+    _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
+):
+    pass
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
+    },
+)
+
+SlotDefaultValueSpecOutputTypeDef = TypedDict(
+    "SlotDefaultValueSpecOutputTypeDef",
+    {
+        "defaultValueList": List[SlotDefaultValueOutputTypeDef],
+    },
+)
 
 SlotDefaultValueSpecTypeDef = TypedDict(
     "SlotDefaultValueSpecTypeDef",
     {
-        "defaultValueList": List[SlotDefaultValueTypeDef],
+        "defaultValueList": Sequence[SlotDefaultValueTypeDef],
     },
 )
 
+SlotTypeConfigurationOutputTypeDef = TypedDict(
+    "SlotTypeConfigurationOutputTypeDef",
+    {
+        "regexConfiguration": SlotTypeRegexConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 SlotTypeConfigurationTypeDef = TypedDict(
     "SlotTypeConfigurationTypeDef",
     {
         "regexConfiguration": SlotTypeRegexConfigurationTypeDef,
     },
     total=False,
 )
@@ -1394,21 +1548,19 @@
         "checksum": str,
         "conversationLogs": ConversationLogsRequestTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutBotAliasRequestRequestTypeDef(
     _RequiredPutBotAliasRequestRequestTypeDef, _OptionalPutBotAliasRequestRequestTypeDef
 ):
     pass
 
-
 BotAliasMetadataTypeDef = TypedDict(
     "BotAliasMetadataTypeDef",
     {
         "name": str,
         "description": str,
         "botVersion": str,
         "botName": str,
@@ -1442,27 +1594,27 @@
         "description": str,
         "botVersion": str,
         "botName": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "checksum": str,
         "conversationLogs": ConversationLogsResponseTypeDef,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateBotVersionResponseTypeDef = TypedDict(
     "CreateBotVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "intents": List[IntentTypeDef],
-        "clarificationPrompt": PromptTypeDef,
-        "abortStatement": StatementTypeDef,
+        "intents": List[IntentOutputTypeDef],
+        "clarificationPrompt": PromptOutputTypeDef,
+        "abortStatement": StatementOutputTypeDef,
         "status": StatusType,
         "failureReason": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "idleSessionTTLInSeconds": int,
         "voiceId": str,
         "checksum": str,
@@ -1471,32 +1623,32 @@
         "childDirected": bool,
         "enableModelImprovements": bool,
         "detectSentiment": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-FollowUpPromptTypeDef = TypedDict(
-    "FollowUpPromptTypeDef",
+FollowUpPromptOutputTypeDef = TypedDict(
+    "FollowUpPromptOutputTypeDef",
     {
-        "prompt": PromptTypeDef,
-        "rejectionStatement": StatementTypeDef,
+        "prompt": PromptOutputTypeDef,
+        "rejectionStatement": StatementOutputTypeDef,
     },
 )
 
 GetBotResponseTypeDef = TypedDict(
     "GetBotResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "intents": List[IntentTypeDef],
+        "intents": List[IntentOutputTypeDef],
         "enableModelImprovements": bool,
         "nluIntentConfidenceThreshold": float,
-        "clarificationPrompt": PromptTypeDef,
-        "abortStatement": StatementTypeDef,
+        "clarificationPrompt": PromptOutputTypeDef,
+        "abortStatement": StatementOutputTypeDef,
         "status": StatusType,
         "failureReason": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "idleSessionTTLInSeconds": int,
         "voiceId": str,
         "checksum": str,
@@ -1504,14 +1656,49 @@
         "locale": LocaleType,
         "childDirected": bool,
         "detectSentiment": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PutBotResponseTypeDef = TypedDict(
+    "PutBotResponseTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "intents": List[IntentOutputTypeDef],
+        "enableModelImprovements": bool,
+        "nluIntentConfidenceThreshold": float,
+        "clarificationPrompt": PromptOutputTypeDef,
+        "abortStatement": StatementOutputTypeDef,
+        "status": StatusType,
+        "failureReason": str,
+        "lastUpdatedDate": datetime,
+        "createdDate": datetime,
+        "idleSessionTTLInSeconds": int,
+        "voiceId": str,
+        "checksum": str,
+        "version": str,
+        "locale": LocaleType,
+        "childDirected": bool,
+        "createVersion": bool,
+        "detectSentiment": bool,
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+FollowUpPromptTypeDef = TypedDict(
+    "FollowUpPromptTypeDef",
+    {
+        "prompt": PromptTypeDef,
+        "rejectionStatement": StatementTypeDef,
+    },
+)
+
 _RequiredPutBotRequestRequestTypeDef = TypedDict(
     "_RequiredPutBotRequestRequestTypeDef",
     {
         "name": str,
         "locale": LocaleType,
         "childDirected": bool,
     },
@@ -1532,48 +1719,45 @@
         "detectSentiment": bool,
         "createVersion": bool,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutBotRequestRequestTypeDef(
     _RequiredPutBotRequestRequestTypeDef, _OptionalPutBotRequestRequestTypeDef
 ):
     pass
 
-
-PutBotResponseTypeDef = TypedDict(
-    "PutBotResponseTypeDef",
+_RequiredSlotOutputTypeDef = TypedDict(
+    "_RequiredSlotOutputTypeDef",
     {
         "name": str,
+        "slotConstraint": SlotConstraintType,
+    },
+)
+_OptionalSlotOutputTypeDef = TypedDict(
+    "_OptionalSlotOutputTypeDef",
+    {
         "description": str,
-        "intents": List[IntentTypeDef],
-        "enableModelImprovements": bool,
-        "nluIntentConfidenceThreshold": float,
-        "clarificationPrompt": PromptTypeDef,
-        "abortStatement": StatementTypeDef,
-        "status": StatusType,
-        "failureReason": str,
-        "lastUpdatedDate": datetime,
-        "createdDate": datetime,
-        "idleSessionTTLInSeconds": int,
-        "voiceId": str,
-        "checksum": str,
-        "version": str,
-        "locale": LocaleType,
-        "childDirected": bool,
-        "createVersion": bool,
-        "detectSentiment": bool,
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "slotType": str,
+        "slotTypeVersion": str,
+        "valueElicitationPrompt": PromptOutputTypeDef,
+        "priority": int,
+        "sampleUtterances": List[str],
+        "responseCard": str,
+        "obfuscationSetting": ObfuscationSettingType,
+        "defaultValueSpec": SlotDefaultValueSpecOutputTypeDef,
     },
+    total=False,
 )
 
+class SlotOutputTypeDef(_RequiredSlotOutputTypeDef, _OptionalSlotOutputTypeDef):
+    pass
+
 _RequiredSlotTypeDef = TypedDict(
     "_RequiredSlotTypeDef",
     {
         "name": str,
         "slotConstraint": SlotConstraintType,
     },
 )
@@ -1581,57 +1765,73 @@
     "_OptionalSlotTypeDef",
     {
         "description": str,
         "slotType": str,
         "slotTypeVersion": str,
         "valueElicitationPrompt": PromptTypeDef,
         "priority": int,
-        "sampleUtterances": List[str],
+        "sampleUtterances": Sequence[str],
         "responseCard": str,
         "obfuscationSetting": ObfuscationSettingType,
         "defaultValueSpec": SlotDefaultValueSpecTypeDef,
     },
     total=False,
 )
 
-
 class SlotTypeDef(_RequiredSlotTypeDef, _OptionalSlotTypeDef):
     pass
 
-
 CreateSlotTypeVersionResponseTypeDef = TypedDict(
     "CreateSlotTypeVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "enumerationValues": List[EnumerationValueTypeDef],
+        "enumerationValues": List[EnumerationValueOutputTypeDef],
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "parentSlotTypeSignature": str,
-        "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
+        "slotTypeConfigurations": List[SlotTypeConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSlotTypeResponseTypeDef = TypedDict(
     "GetSlotTypeResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "enumerationValues": List[EnumerationValueTypeDef],
+        "enumerationValues": List[EnumerationValueOutputTypeDef],
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "parentSlotTypeSignature": str,
-        "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
+        "slotTypeConfigurations": List[SlotTypeConfigurationOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutSlotTypeResponseTypeDef = TypedDict(
+    "PutSlotTypeResponseTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "enumerationValues": List[EnumerationValueOutputTypeDef],
+        "lastUpdatedDate": datetime,
+        "createdDate": datetime,
+        "version": str,
+        "checksum": str,
+        "valueSelectionStrategy": SlotValueSelectionStrategyType,
+        "createVersion": bool,
+        "parentSlotTypeSignature": str,
+        "slotTypeConfigurations": List[SlotTypeConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutSlotTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutSlotTypeRequestRequestTypeDef",
     {
@@ -1648,39 +1848,19 @@
         "createVersion": bool,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": Sequence[SlotTypeConfigurationTypeDef],
     },
     total=False,
 )
 
-
 class PutSlotTypeRequestRequestTypeDef(
     _RequiredPutSlotTypeRequestRequestTypeDef, _OptionalPutSlotTypeRequestRequestTypeDef
 ):
     pass
 
-
-PutSlotTypeResponseTypeDef = TypedDict(
-    "PutSlotTypeResponseTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "enumerationValues": List[EnumerationValueTypeDef],
-        "lastUpdatedDate": datetime,
-        "createdDate": datetime,
-        "version": str,
-        "checksum": str,
-        "valueSelectionStrategy": SlotValueSelectionStrategyType,
-        "createVersion": bool,
-        "parentSlotTypeSignature": str,
-        "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetUtterancesViewResponseTypeDef = TypedDict(
     "GetUtterancesViewResponseTypeDef",
     {
         "botName": str,
         "utterances": List[UtteranceListTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1696,55 +1876,81 @@
 )
 
 CreateIntentVersionResponseTypeDef = TypedDict(
     "CreateIntentVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "slots": List[SlotTypeDef],
+        "slots": List[SlotOutputTypeDef],
         "sampleUtterances": List[str],
-        "confirmationPrompt": PromptTypeDef,
-        "rejectionStatement": StatementTypeDef,
-        "followUpPrompt": FollowUpPromptTypeDef,
-        "conclusionStatement": StatementTypeDef,
-        "dialogCodeHook": CodeHookTypeDef,
-        "fulfillmentActivity": FulfillmentActivityTypeDef,
+        "confirmationPrompt": PromptOutputTypeDef,
+        "rejectionStatement": StatementOutputTypeDef,
+        "followUpPrompt": FollowUpPromptOutputTypeDef,
+        "conclusionStatement": StatementOutputTypeDef,
+        "dialogCodeHook": CodeHookOutputTypeDef,
+        "fulfillmentActivity": FulfillmentActivityOutputTypeDef,
         "parentIntentSignature": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
-        "kendraConfiguration": KendraConfigurationTypeDef,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
+        "kendraConfiguration": KendraConfigurationOutputTypeDef,
+        "inputContexts": List[InputContextOutputTypeDef],
+        "outputContexts": List[OutputContextOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIntentResponseTypeDef = TypedDict(
     "GetIntentResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "slots": List[SlotTypeDef],
+        "slots": List[SlotOutputTypeDef],
         "sampleUtterances": List[str],
-        "confirmationPrompt": PromptTypeDef,
-        "rejectionStatement": StatementTypeDef,
-        "followUpPrompt": FollowUpPromptTypeDef,
-        "conclusionStatement": StatementTypeDef,
-        "dialogCodeHook": CodeHookTypeDef,
-        "fulfillmentActivity": FulfillmentActivityTypeDef,
+        "confirmationPrompt": PromptOutputTypeDef,
+        "rejectionStatement": StatementOutputTypeDef,
+        "followUpPrompt": FollowUpPromptOutputTypeDef,
+        "conclusionStatement": StatementOutputTypeDef,
+        "dialogCodeHook": CodeHookOutputTypeDef,
+        "fulfillmentActivity": FulfillmentActivityOutputTypeDef,
         "parentIntentSignature": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
-        "kendraConfiguration": KendraConfigurationTypeDef,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
+        "kendraConfiguration": KendraConfigurationOutputTypeDef,
+        "inputContexts": List[InputContextOutputTypeDef],
+        "outputContexts": List[OutputContextOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutIntentResponseTypeDef = TypedDict(
+    "PutIntentResponseTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "slots": List[SlotOutputTypeDef],
+        "sampleUtterances": List[str],
+        "confirmationPrompt": PromptOutputTypeDef,
+        "rejectionStatement": StatementOutputTypeDef,
+        "followUpPrompt": FollowUpPromptOutputTypeDef,
+        "conclusionStatement": StatementOutputTypeDef,
+        "dialogCodeHook": CodeHookOutputTypeDef,
+        "fulfillmentActivity": FulfillmentActivityOutputTypeDef,
+        "parentIntentSignature": str,
+        "lastUpdatedDate": datetime,
+        "createdDate": datetime,
+        "version": str,
+        "checksum": str,
+        "createVersion": bool,
+        "kendraConfiguration": KendraConfigurationOutputTypeDef,
+        "inputContexts": List[InputContextOutputTypeDef],
+        "outputContexts": List[OutputContextOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutIntentRequestRequestTypeDef = TypedDict(
     "_RequiredPutIntentRequestRequestTypeDef",
     {
@@ -1769,39 +1975,11 @@
         "kendraConfiguration": KendraConfigurationTypeDef,
         "inputContexts": Sequence[InputContextTypeDef],
         "outputContexts": Sequence[OutputContextTypeDef],
     },
     total=False,
 )
 
-
 class PutIntentRequestRequestTypeDef(
     _RequiredPutIntentRequestRequestTypeDef, _OptionalPutIntentRequestRequestTypeDef
 ):
     pass
-
-
-PutIntentResponseTypeDef = TypedDict(
-    "PutIntentResponseTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "slots": List[SlotTypeDef],
-        "sampleUtterances": List[str],
-        "confirmationPrompt": PromptTypeDef,
-        "rejectionStatement": StatementTypeDef,
-        "followUpPrompt": FollowUpPromptTypeDef,
-        "conclusionStatement": StatementTypeDef,
-        "dialogCodeHook": CodeHookTypeDef,
-        "fulfillmentActivity": FulfillmentActivityTypeDef,
-        "parentIntentSignature": str,
-        "lastUpdatedDate": datetime,
-        "createdDate": datetime,
-        "version": str,
-        "checksum": str,
-        "createVersion": bool,
-        "kendraConfiguration": KendraConfigurationTypeDef,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models/type_defs.pyi` & `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,41 +44,44 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "BotChannelAssociationTypeDef",
     "BotMetadataTypeDef",
     "BuiltinIntentMetadataTypeDef",
     "BuiltinIntentSlotTypeDef",
     "BuiltinSlotTypeMetadataTypeDef",
+    "CodeHookOutputTypeDef",
     "CodeHookTypeDef",
     "LogSettingsRequestTypeDef",
     "LogSettingsResponseTypeDef",
     "CreateBotVersionRequestRequestTypeDef",
-    "IntentTypeDef",
+    "IntentOutputTypeDef",
     "CreateIntentVersionRequestRequestTypeDef",
-    "InputContextTypeDef",
-    "KendraConfigurationTypeDef",
-    "OutputContextTypeDef",
+    "InputContextOutputTypeDef",
+    "KendraConfigurationOutputTypeDef",
+    "OutputContextOutputTypeDef",
     "CreateSlotTypeVersionRequestRequestTypeDef",
-    "EnumerationValueTypeDef",
+    "EnumerationValueOutputTypeDef",
     "DeleteBotAliasRequestRequestTypeDef",
     "DeleteBotChannelAssociationRequestRequestTypeDef",
     "DeleteBotRequestRequestTypeDef",
     "DeleteBotVersionRequestRequestTypeDef",
     "DeleteIntentRequestRequestTypeDef",
     "DeleteIntentVersionRequestRequestTypeDef",
     "DeleteSlotTypeRequestRequestTypeDef",
     "DeleteSlotTypeVersionRequestRequestTypeDef",
     "DeleteUtterancesRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EnumerationValueTypeDef",
     "GetBotAliasRequestRequestTypeDef",
     "GetBotAliasesRequestGetBotAliasesPaginateTypeDef",
     "GetBotAliasesRequestRequestTypeDef",
     "GetBotChannelAssociationRequestRequestTypeDef",
     "GetBotChannelAssociationResponseTypeDef",
     "GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
     "GetBotChannelAssociationsRequestRequestTypeDef",
@@ -109,69 +112,84 @@
     "GetSlotTypeRequestRequestTypeDef",
     "GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
     "GetSlotTypeVersionsRequestRequestTypeDef",
     "SlotTypeMetadataTypeDef",
     "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
     "GetSlotTypesRequestRequestTypeDef",
     "GetUtterancesViewRequestRequestTypeDef",
+    "InputContextTypeDef",
+    "IntentTypeDef",
+    "KendraConfigurationTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
+    "MessageOutputTypeDef",
     "MessageTypeDef",
+    "OutputContextTypeDef",
     "PaginatorConfigTypeDef",
+    "TagTypeDef",
     "ResponseMetadataTypeDef",
+    "SlotDefaultValueOutputTypeDef",
     "SlotDefaultValueTypeDef",
+    "SlotTypeRegexConfigurationOutputTypeDef",
     "SlotTypeRegexConfigurationTypeDef",
     "StartMigrationRequestRequestTypeDef",
     "StartMigrationResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UtteranceDataTypeDef",
     "GetBotChannelAssociationsResponseTypeDef",
     "GetBotVersionsResponseTypeDef",
     "GetBotsResponseTypeDef",
     "GetBuiltinIntentsResponseTypeDef",
     "GetBuiltinIntentResponseTypeDef",
     "GetBuiltinSlotTypesResponseTypeDef",
+    "FulfillmentActivityOutputTypeDef",
     "FulfillmentActivityTypeDef",
     "ConversationLogsRequestTypeDef",
     "ConversationLogsResponseTypeDef",
     "GetIntentVersionsResponseTypeDef",
     "GetIntentsResponseTypeDef",
     "GetMigrationResponseTypeDef",
     "GetMigrationsResponseTypeDef",
     "GetSlotTypeVersionsResponseTypeDef",
     "GetSlotTypesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
+    "PromptOutputTypeDef",
+    "StatementOutputTypeDef",
     "PromptTypeDef",
     "StatementTypeDef",
+    "StartImportRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "SlotDefaultValueSpecOutputTypeDef",
     "SlotDefaultValueSpecTypeDef",
+    "SlotTypeConfigurationOutputTypeDef",
     "SlotTypeConfigurationTypeDef",
     "UtteranceListTypeDef",
     "PutBotAliasRequestRequestTypeDef",
     "BotAliasMetadataTypeDef",
     "GetBotAliasResponseTypeDef",
     "PutBotAliasResponseTypeDef",
     "CreateBotVersionResponseTypeDef",
-    "FollowUpPromptTypeDef",
+    "FollowUpPromptOutputTypeDef",
     "GetBotResponseTypeDef",
-    "PutBotRequestRequestTypeDef",
     "PutBotResponseTypeDef",
+    "FollowUpPromptTypeDef",
+    "PutBotRequestRequestTypeDef",
+    "SlotOutputTypeDef",
     "SlotTypeDef",
     "CreateSlotTypeVersionResponseTypeDef",
     "GetSlotTypeResponseTypeDef",
-    "PutSlotTypeRequestRequestTypeDef",
     "PutSlotTypeResponseTypeDef",
+    "PutSlotTypeRequestRequestTypeDef",
     "GetUtterancesViewResponseTypeDef",
     "GetBotAliasesResponseTypeDef",
     "CreateIntentVersionResponseTypeDef",
     "GetIntentResponseTypeDef",
-    "PutIntentRequestRequestTypeDef",
     "PutIntentResponseTypeDef",
+    "PutIntentRequestRequestTypeDef",
 )
 
 BotChannelAssociationTypeDef = TypedDict(
     "BotChannelAssociationTypeDef",
     {
         "name": str,
         "description": str,
@@ -221,14 +239,22 @@
     {
         "signature": str,
         "supportedLocales": List[LocaleType],
     },
     total=False,
 )
 
+CodeHookOutputTypeDef = TypedDict(
+    "CodeHookOutputTypeDef",
+    {
+        "uri": str,
+        "messageVersion": str,
+    },
+)
+
 CodeHookTypeDef = TypedDict(
     "CodeHookTypeDef",
     {
         "uri": str,
         "messageVersion": str,
     },
 )
@@ -245,19 +271,21 @@
     "_OptionalLogSettingsRequestTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
 
+
 class LogSettingsRequestTypeDef(
     _RequiredLogSettingsRequestTypeDef, _OptionalLogSettingsRequestTypeDef
 ):
     pass
 
+
 LogSettingsResponseTypeDef = TypedDict(
     "LogSettingsResponseTypeDef",
     {
         "logType": LogTypeType,
         "destination": DestinationType,
         "kmsKeyArn": str,
         "resourceArn": str,
@@ -276,21 +304,23 @@
     "_OptionalCreateBotVersionRequestRequestTypeDef",
     {
         "checksum": str,
     },
     total=False,
 )
 
+
 class CreateBotVersionRequestRequestTypeDef(
     _RequiredCreateBotVersionRequestRequestTypeDef, _OptionalCreateBotVersionRequestRequestTypeDef
 ):
     pass
 
-IntentTypeDef = TypedDict(
-    "IntentTypeDef",
+
+IntentOutputTypeDef = TypedDict(
+    "IntentOutputTypeDef",
     {
         "intentName": str,
         "intentVersion": str,
     },
 )
 
 _RequiredCreateIntentVersionRequestRequestTypeDef = TypedDict(
@@ -303,49 +333,53 @@
     "_OptionalCreateIntentVersionRequestRequestTypeDef",
     {
         "checksum": str,
     },
     total=False,
 )
 
+
 class CreateIntentVersionRequestRequestTypeDef(
     _RequiredCreateIntentVersionRequestRequestTypeDef,
     _OptionalCreateIntentVersionRequestRequestTypeDef,
 ):
     pass
 
-InputContextTypeDef = TypedDict(
-    "InputContextTypeDef",
+
+InputContextOutputTypeDef = TypedDict(
+    "InputContextOutputTypeDef",
     {
         "name": str,
     },
 )
 
-_RequiredKendraConfigurationTypeDef = TypedDict(
-    "_RequiredKendraConfigurationTypeDef",
+_RequiredKendraConfigurationOutputTypeDef = TypedDict(
+    "_RequiredKendraConfigurationOutputTypeDef",
     {
         "kendraIndex": str,
         "role": str,
     },
 )
-_OptionalKendraConfigurationTypeDef = TypedDict(
-    "_OptionalKendraConfigurationTypeDef",
+_OptionalKendraConfigurationOutputTypeDef = TypedDict(
+    "_OptionalKendraConfigurationOutputTypeDef",
     {
         "queryFilterString": str,
     },
     total=False,
 )
 
-class KendraConfigurationTypeDef(
-    _RequiredKendraConfigurationTypeDef, _OptionalKendraConfigurationTypeDef
+
+class KendraConfigurationOutputTypeDef(
+    _RequiredKendraConfigurationOutputTypeDef, _OptionalKendraConfigurationOutputTypeDef
 ):
     pass
 
-OutputContextTypeDef = TypedDict(
-    "OutputContextTypeDef",
+
+OutputContextOutputTypeDef = TypedDict(
+    "OutputContextOutputTypeDef",
     {
         "name": str,
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
     },
 )
 
@@ -359,37 +393,43 @@
     "_OptionalCreateSlotTypeVersionRequestRequestTypeDef",
     {
         "checksum": str,
     },
     total=False,
 )
 
+
 class CreateSlotTypeVersionRequestRequestTypeDef(
     _RequiredCreateSlotTypeVersionRequestRequestTypeDef,
     _OptionalCreateSlotTypeVersionRequestRequestTypeDef,
 ):
     pass
 
-_RequiredEnumerationValueTypeDef = TypedDict(
-    "_RequiredEnumerationValueTypeDef",
+
+_RequiredEnumerationValueOutputTypeDef = TypedDict(
+    "_RequiredEnumerationValueOutputTypeDef",
     {
         "value": str,
     },
 )
-_OptionalEnumerationValueTypeDef = TypedDict(
-    "_OptionalEnumerationValueTypeDef",
+_OptionalEnumerationValueOutputTypeDef = TypedDict(
+    "_OptionalEnumerationValueOutputTypeDef",
     {
         "synonyms": List[str],
     },
     total=False,
 )
 
-class EnumerationValueTypeDef(_RequiredEnumerationValueTypeDef, _OptionalEnumerationValueTypeDef):
+
+class EnumerationValueOutputTypeDef(
+    _RequiredEnumerationValueOutputTypeDef, _OptionalEnumerationValueOutputTypeDef
+):
     pass
 
+
 DeleteBotAliasRequestRequestTypeDef = TypedDict(
     "DeleteBotAliasRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
     },
 )
@@ -459,14 +499,33 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredEnumerationValueTypeDef = TypedDict(
+    "_RequiredEnumerationValueTypeDef",
+    {
+        "value": str,
+    },
+)
+_OptionalEnumerationValueTypeDef = TypedDict(
+    "_OptionalEnumerationValueTypeDef",
+    {
+        "synonyms": Sequence[str],
+    },
+    total=False,
+)
+
+
+class EnumerationValueTypeDef(_RequiredEnumerationValueTypeDef, _OptionalEnumerationValueTypeDef):
+    pass
+
+
 GetBotAliasRequestRequestTypeDef = TypedDict(
     "GetBotAliasRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
     },
 )
@@ -482,20 +541,22 @@
     {
         "nameContains": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class GetBotAliasesRequestGetBotAliasesPaginateTypeDef(
     _RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
     _OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetBotAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotAliasesRequestRequestTypeDef",
     {
         "botName": str,
     },
 )
 _OptionalGetBotAliasesRequestRequestTypeDef = TypedDict(
@@ -504,19 +565,21 @@
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
     total=False,
 )
 
+
 class GetBotAliasesRequestRequestTypeDef(
     _RequiredGetBotAliasesRequestRequestTypeDef, _OptionalGetBotAliasesRequestRequestTypeDef
 ):
     pass
 
+
 GetBotChannelAssociationRequestRequestTypeDef = TypedDict(
     "GetBotChannelAssociationRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
         "botAlias": str,
     },
@@ -550,20 +613,22 @@
     {
         "nameContains": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef(
     _RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
     _OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetBotChannelAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotChannelAssociationsRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
     },
 )
@@ -573,20 +638,22 @@
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
     total=False,
 )
 
+
 class GetBotChannelAssociationsRequestRequestTypeDef(
     _RequiredGetBotChannelAssociationsRequestRequestTypeDef,
     _OptionalGetBotChannelAssociationsRequestRequestTypeDef,
 ):
     pass
 
+
 GetBotRequestRequestTypeDef = TypedDict(
     "GetBotRequestRequestTypeDef",
     {
         "name": str,
         "versionOrAlias": str,
     },
 )
@@ -601,20 +668,22 @@
     "_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class GetBotVersionsRequestGetBotVersionsPaginateTypeDef(
     _RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
     _OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetBotVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetBotVersionsRequestRequestTypeDef = TypedDict(
@@ -622,19 +691,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetBotVersionsRequestRequestTypeDef(
     _RequiredGetBotVersionsRequestRequestTypeDef, _OptionalGetBotVersionsRequestRequestTypeDef
 ):
     pass
 
+
 GetBotsRequestGetBotsPaginateTypeDef = TypedDict(
     "GetBotsRequestGetBotsPaginateTypeDef",
     {
         "nameContains": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -762,20 +833,22 @@
     "_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef(
     _RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
     _OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetIntentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetIntentVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetIntentVersionsRequestRequestTypeDef = TypedDict(
@@ -783,19 +856,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetIntentVersionsRequestRequestTypeDef(
     _RequiredGetIntentVersionsRequestRequestTypeDef, _OptionalGetIntentVersionsRequestRequestTypeDef
 ):
     pass
 
+
 IntentMetadataTypeDef = TypedDict(
     "IntentMetadataTypeDef",
     {
         "name": str,
         "description": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
@@ -888,20 +963,22 @@
     "_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef(
     _RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
     _OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetSlotTypeVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSlotTypeVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetSlotTypeVersionsRequestRequestTypeDef = TypedDict(
@@ -909,20 +986,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetSlotTypeVersionsRequestRequestTypeDef(
     _RequiredGetSlotTypeVersionsRequestRequestTypeDef,
     _OptionalGetSlotTypeVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 SlotTypeMetadataTypeDef = TypedDict(
     "SlotTypeMetadataTypeDef",
     {
         "name": str,
         "description": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
@@ -955,29 +1034,86 @@
     {
         "botName": str,
         "botVersions": Sequence[str],
         "statusType": StatusTypeType,
     },
 )
 
+InputContextTypeDef = TypedDict(
+    "InputContextTypeDef",
+    {
+        "name": str,
+    },
+)
+
+IntentTypeDef = TypedDict(
+    "IntentTypeDef",
+    {
+        "intentName": str,
+        "intentVersion": str,
+    },
+)
+
+_RequiredKendraConfigurationTypeDef = TypedDict(
+    "_RequiredKendraConfigurationTypeDef",
+    {
+        "kendraIndex": str,
+        "role": str,
+    },
+)
+_OptionalKendraConfigurationTypeDef = TypedDict(
+    "_OptionalKendraConfigurationTypeDef",
+    {
+        "queryFilterString": str,
+    },
+    total=False,
+)
+
+
+class KendraConfigurationTypeDef(
+    _RequiredKendraConfigurationTypeDef, _OptionalKendraConfigurationTypeDef
+):
+    pass
+
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
+_RequiredMessageOutputTypeDef = TypedDict(
+    "_RequiredMessageOutputTypeDef",
+    {
+        "contentType": ContentTypeType,
+        "content": str,
+    },
+)
+_OptionalMessageOutputTypeDef = TypedDict(
+    "_OptionalMessageOutputTypeDef",
+    {
+        "groupNumber": int,
+    },
+    total=False,
+)
+
+
+class MessageOutputTypeDef(_RequiredMessageOutputTypeDef, _OptionalMessageOutputTypeDef):
+    pass
+
+
 _RequiredMessageTypeDef = TypedDict(
     "_RequiredMessageTypeDef",
     {
         "contentType": ContentTypeType,
         "content": str,
     },
 )
@@ -985,45 +1121,78 @@
     "_OptionalMessageTypeDef",
     {
         "groupNumber": int,
     },
     total=False,
 )
 
+
 class MessageTypeDef(_RequiredMessageTypeDef, _OptionalMessageTypeDef):
     pass
 
+
+OutputContextTypeDef = TypedDict(
+    "OutputContextTypeDef",
+    {
+        "name": str,
+        "timeToLiveInSeconds": int,
+        "turnsToLive": int,
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
     total=False,
 )
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+SlotDefaultValueOutputTypeDef = TypedDict(
+    "SlotDefaultValueOutputTypeDef",
+    {
+        "defaultValue": str,
+    },
+)
+
 SlotDefaultValueTypeDef = TypedDict(
     "SlotDefaultValueTypeDef",
     {
         "defaultValue": str,
     },
 )
 
+SlotTypeRegexConfigurationOutputTypeDef = TypedDict(
+    "SlotTypeRegexConfigurationOutputTypeDef",
+    {
+        "pattern": str,
+    },
+)
+
 SlotTypeRegexConfigurationTypeDef = TypedDict(
     "SlotTypeRegexConfigurationTypeDef",
     {
         "pattern": str,
     },
 )
 
@@ -1124,33 +1293,56 @@
     {
         "slotTypes": List[BuiltinSlotTypeMetadataTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredFulfillmentActivityOutputTypeDef = TypedDict(
+    "_RequiredFulfillmentActivityOutputTypeDef",
+    {
+        "type": FulfillmentActivityTypeType,
+    },
+)
+_OptionalFulfillmentActivityOutputTypeDef = TypedDict(
+    "_OptionalFulfillmentActivityOutputTypeDef",
+    {
+        "codeHook": CodeHookOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class FulfillmentActivityOutputTypeDef(
+    _RequiredFulfillmentActivityOutputTypeDef, _OptionalFulfillmentActivityOutputTypeDef
+):
+    pass
+
+
 _RequiredFulfillmentActivityTypeDef = TypedDict(
     "_RequiredFulfillmentActivityTypeDef",
     {
         "type": FulfillmentActivityTypeType,
     },
 )
 _OptionalFulfillmentActivityTypeDef = TypedDict(
     "_OptionalFulfillmentActivityTypeDef",
     {
         "codeHook": CodeHookTypeDef,
     },
     total=False,
 )
 
+
 class FulfillmentActivityTypeDef(
     _RequiredFulfillmentActivityTypeDef, _OptionalFulfillmentActivityTypeDef
 ):
     pass
 
+
 ConversationLogsRequestTypeDef = TypedDict(
     "ConversationLogsRequestTypeDef",
     {
         "logSettings": Sequence[LogSettingsRequestTypeDef],
         "iamRoleArn": str,
     },
 )
@@ -1225,104 +1417,164 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStartImportRequestRequestTypeDef = TypedDict(
-    "_RequiredStartImportRequestRequestTypeDef",
+StartImportResponseTypeDef = TypedDict(
+    "StartImportResponseTypeDef",
     {
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "name": str,
         "resourceType": ResourceTypeType,
         "mergeStrategy": MergeStrategyType,
+        "importId": str,
+        "importStatus": ImportStatusType,
+        "tags": List[TagOutputTypeDef],
+        "createdDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalStartImportRequestRequestTypeDef = TypedDict(
-    "_OptionalStartImportRequestRequestTypeDef",
+
+_RequiredPromptOutputTypeDef = TypedDict(
+    "_RequiredPromptOutputTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
+        "messages": List[MessageOutputTypeDef],
+        "maxAttempts": int,
+    },
+)
+_OptionalPromptOutputTypeDef = TypedDict(
+    "_OptionalPromptOutputTypeDef",
+    {
+        "responseCard": str,
     },
     total=False,
 )
 
-class StartImportRequestRequestTypeDef(
-    _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
-):
+
+class PromptOutputTypeDef(_RequiredPromptOutputTypeDef, _OptionalPromptOutputTypeDef):
     pass
 
-StartImportResponseTypeDef = TypedDict(
-    "StartImportResponseTypeDef",
+
+_RequiredStatementOutputTypeDef = TypedDict(
+    "_RequiredStatementOutputTypeDef",
     {
-        "name": str,
-        "resourceType": ResourceTypeType,
-        "mergeStrategy": MergeStrategyType,
-        "importId": str,
-        "importStatus": ImportStatusType,
-        "tags": List[TagTypeDef],
-        "createdDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "messages": List[MessageOutputTypeDef],
     },
 )
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+_OptionalStatementOutputTypeDef = TypedDict(
+    "_OptionalStatementOutputTypeDef",
     {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
+        "responseCard": str,
     },
+    total=False,
 )
 
+
+class StatementOutputTypeDef(_RequiredStatementOutputTypeDef, _OptionalStatementOutputTypeDef):
+    pass
+
+
 _RequiredPromptTypeDef = TypedDict(
     "_RequiredPromptTypeDef",
     {
-        "messages": List[MessageTypeDef],
+        "messages": Sequence[MessageTypeDef],
         "maxAttempts": int,
     },
 )
 _OptionalPromptTypeDef = TypedDict(
     "_OptionalPromptTypeDef",
     {
         "responseCard": str,
     },
     total=False,
 )
 
+
 class PromptTypeDef(_RequiredPromptTypeDef, _OptionalPromptTypeDef):
     pass
 
+
 _RequiredStatementTypeDef = TypedDict(
     "_RequiredStatementTypeDef",
     {
-        "messages": List[MessageTypeDef],
+        "messages": Sequence[MessageTypeDef],
     },
 )
 _OptionalStatementTypeDef = TypedDict(
     "_OptionalStatementTypeDef",
     {
         "responseCard": str,
     },
     total=False,
 )
 
+
 class StatementTypeDef(_RequiredStatementTypeDef, _OptionalStatementTypeDef):
     pass
 
+
+_RequiredStartImportRequestRequestTypeDef = TypedDict(
+    "_RequiredStartImportRequestRequestTypeDef",
+    {
+        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "resourceType": ResourceTypeType,
+        "mergeStrategy": MergeStrategyType,
+    },
+)
+_OptionalStartImportRequestRequestTypeDef = TypedDict(
+    "_OptionalStartImportRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class StartImportRequestRequestTypeDef(
+    _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
+):
+    pass
+
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
+    },
+)
+
+SlotDefaultValueSpecOutputTypeDef = TypedDict(
+    "SlotDefaultValueSpecOutputTypeDef",
+    {
+        "defaultValueList": List[SlotDefaultValueOutputTypeDef],
+    },
+)
+
 SlotDefaultValueSpecTypeDef = TypedDict(
     "SlotDefaultValueSpecTypeDef",
     {
-        "defaultValueList": List[SlotDefaultValueTypeDef],
+        "defaultValueList": Sequence[SlotDefaultValueTypeDef],
     },
 )
 
+SlotTypeConfigurationOutputTypeDef = TypedDict(
+    "SlotTypeConfigurationOutputTypeDef",
+    {
+        "regexConfiguration": SlotTypeRegexConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 SlotTypeConfigurationTypeDef = TypedDict(
     "SlotTypeConfigurationTypeDef",
     {
         "regexConfiguration": SlotTypeRegexConfigurationTypeDef,
     },
     total=False,
 )
@@ -1351,19 +1603,21 @@
         "checksum": str,
         "conversationLogs": ConversationLogsRequestTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutBotAliasRequestRequestTypeDef(
     _RequiredPutBotAliasRequestRequestTypeDef, _OptionalPutBotAliasRequestRequestTypeDef
 ):
     pass
 
+
 BotAliasMetadataTypeDef = TypedDict(
     "BotAliasMetadataTypeDef",
     {
         "name": str,
         "description": str,
         "botVersion": str,
         "botName": str,
@@ -1397,27 +1651,27 @@
         "description": str,
         "botVersion": str,
         "botName": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "checksum": str,
         "conversationLogs": ConversationLogsResponseTypeDef,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateBotVersionResponseTypeDef = TypedDict(
     "CreateBotVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "intents": List[IntentTypeDef],
-        "clarificationPrompt": PromptTypeDef,
-        "abortStatement": StatementTypeDef,
+        "intents": List[IntentOutputTypeDef],
+        "clarificationPrompt": PromptOutputTypeDef,
+        "abortStatement": StatementOutputTypeDef,
         "status": StatusType,
         "failureReason": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "idleSessionTTLInSeconds": int,
         "voiceId": str,
         "checksum": str,
@@ -1426,47 +1680,82 @@
         "childDirected": bool,
         "enableModelImprovements": bool,
         "detectSentiment": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-FollowUpPromptTypeDef = TypedDict(
-    "FollowUpPromptTypeDef",
+FollowUpPromptOutputTypeDef = TypedDict(
+    "FollowUpPromptOutputTypeDef",
     {
-        "prompt": PromptTypeDef,
-        "rejectionStatement": StatementTypeDef,
+        "prompt": PromptOutputTypeDef,
+        "rejectionStatement": StatementOutputTypeDef,
     },
 )
 
 GetBotResponseTypeDef = TypedDict(
     "GetBotResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "intents": List[IntentTypeDef],
+        "intents": List[IntentOutputTypeDef],
         "enableModelImprovements": bool,
         "nluIntentConfidenceThreshold": float,
-        "clarificationPrompt": PromptTypeDef,
-        "abortStatement": StatementTypeDef,
+        "clarificationPrompt": PromptOutputTypeDef,
+        "abortStatement": StatementOutputTypeDef,
+        "status": StatusType,
+        "failureReason": str,
+        "lastUpdatedDate": datetime,
+        "createdDate": datetime,
+        "idleSessionTTLInSeconds": int,
+        "voiceId": str,
+        "checksum": str,
+        "version": str,
+        "locale": LocaleType,
+        "childDirected": bool,
+        "detectSentiment": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutBotResponseTypeDef = TypedDict(
+    "PutBotResponseTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "intents": List[IntentOutputTypeDef],
+        "enableModelImprovements": bool,
+        "nluIntentConfidenceThreshold": float,
+        "clarificationPrompt": PromptOutputTypeDef,
+        "abortStatement": StatementOutputTypeDef,
         "status": StatusType,
         "failureReason": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "idleSessionTTLInSeconds": int,
         "voiceId": str,
         "checksum": str,
         "version": str,
         "locale": LocaleType,
         "childDirected": bool,
+        "createVersion": bool,
         "detectSentiment": bool,
+        "tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+FollowUpPromptTypeDef = TypedDict(
+    "FollowUpPromptTypeDef",
+    {
+        "prompt": PromptTypeDef,
+        "rejectionStatement": StatementTypeDef,
+    },
+)
+
 _RequiredPutBotRequestRequestTypeDef = TypedDict(
     "_RequiredPutBotRequestRequestTypeDef",
     {
         "name": str,
         "locale": LocaleType,
         "childDirected": bool,
     },
@@ -1487,46 +1776,49 @@
         "detectSentiment": bool,
         "createVersion": bool,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutBotRequestRequestTypeDef(
     _RequiredPutBotRequestRequestTypeDef, _OptionalPutBotRequestRequestTypeDef
 ):
     pass
 
-PutBotResponseTypeDef = TypedDict(
-    "PutBotResponseTypeDef",
+
+_RequiredSlotOutputTypeDef = TypedDict(
+    "_RequiredSlotOutputTypeDef",
     {
         "name": str,
+        "slotConstraint": SlotConstraintType,
+    },
+)
+_OptionalSlotOutputTypeDef = TypedDict(
+    "_OptionalSlotOutputTypeDef",
+    {
         "description": str,
-        "intents": List[IntentTypeDef],
-        "enableModelImprovements": bool,
-        "nluIntentConfidenceThreshold": float,
-        "clarificationPrompt": PromptTypeDef,
-        "abortStatement": StatementTypeDef,
-        "status": StatusType,
-        "failureReason": str,
-        "lastUpdatedDate": datetime,
-        "createdDate": datetime,
-        "idleSessionTTLInSeconds": int,
-        "voiceId": str,
-        "checksum": str,
-        "version": str,
-        "locale": LocaleType,
-        "childDirected": bool,
-        "createVersion": bool,
-        "detectSentiment": bool,
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "slotType": str,
+        "slotTypeVersion": str,
+        "valueElicitationPrompt": PromptOutputTypeDef,
+        "priority": int,
+        "sampleUtterances": List[str],
+        "responseCard": str,
+        "obfuscationSetting": ObfuscationSettingType,
+        "defaultValueSpec": SlotDefaultValueSpecOutputTypeDef,
     },
+    total=False,
 )
 
+
+class SlotOutputTypeDef(_RequiredSlotOutputTypeDef, _OptionalSlotOutputTypeDef):
+    pass
+
+
 _RequiredSlotTypeDef = TypedDict(
     "_RequiredSlotTypeDef",
     {
         "name": str,
         "slotConstraint": SlotConstraintType,
     },
 )
@@ -1534,55 +1826,75 @@
     "_OptionalSlotTypeDef",
     {
         "description": str,
         "slotType": str,
         "slotTypeVersion": str,
         "valueElicitationPrompt": PromptTypeDef,
         "priority": int,
-        "sampleUtterances": List[str],
+        "sampleUtterances": Sequence[str],
         "responseCard": str,
         "obfuscationSetting": ObfuscationSettingType,
         "defaultValueSpec": SlotDefaultValueSpecTypeDef,
     },
     total=False,
 )
 
+
 class SlotTypeDef(_RequiredSlotTypeDef, _OptionalSlotTypeDef):
     pass
 
+
 CreateSlotTypeVersionResponseTypeDef = TypedDict(
     "CreateSlotTypeVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "enumerationValues": List[EnumerationValueTypeDef],
+        "enumerationValues": List[EnumerationValueOutputTypeDef],
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "parentSlotTypeSignature": str,
-        "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
+        "slotTypeConfigurations": List[SlotTypeConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSlotTypeResponseTypeDef = TypedDict(
     "GetSlotTypeResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "enumerationValues": List[EnumerationValueTypeDef],
+        "enumerationValues": List[EnumerationValueOutputTypeDef],
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "parentSlotTypeSignature": str,
-        "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
+        "slotTypeConfigurations": List[SlotTypeConfigurationOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutSlotTypeResponseTypeDef = TypedDict(
+    "PutSlotTypeResponseTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "enumerationValues": List[EnumerationValueOutputTypeDef],
+        "lastUpdatedDate": datetime,
+        "createdDate": datetime,
+        "version": str,
+        "checksum": str,
+        "valueSelectionStrategy": SlotValueSelectionStrategyType,
+        "createVersion": bool,
+        "parentSlotTypeSignature": str,
+        "slotTypeConfigurations": List[SlotTypeConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutSlotTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutSlotTypeRequestRequestTypeDef",
     {
@@ -1599,36 +1911,20 @@
         "createVersion": bool,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": Sequence[SlotTypeConfigurationTypeDef],
     },
     total=False,
 )
 
+
 class PutSlotTypeRequestRequestTypeDef(
     _RequiredPutSlotTypeRequestRequestTypeDef, _OptionalPutSlotTypeRequestRequestTypeDef
 ):
     pass
 
-PutSlotTypeResponseTypeDef = TypedDict(
-    "PutSlotTypeResponseTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "enumerationValues": List[EnumerationValueTypeDef],
-        "lastUpdatedDate": datetime,
-        "createdDate": datetime,
-        "version": str,
-        "checksum": str,
-        "valueSelectionStrategy": SlotValueSelectionStrategyType,
-        "createVersion": bool,
-        "parentSlotTypeSignature": str,
-        "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetUtterancesViewResponseTypeDef = TypedDict(
     "GetUtterancesViewResponseTypeDef",
     {
         "botName": str,
         "utterances": List[UtteranceListTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1645,55 +1941,81 @@
 )
 
 CreateIntentVersionResponseTypeDef = TypedDict(
     "CreateIntentVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "slots": List[SlotTypeDef],
+        "slots": List[SlotOutputTypeDef],
         "sampleUtterances": List[str],
-        "confirmationPrompt": PromptTypeDef,
-        "rejectionStatement": StatementTypeDef,
-        "followUpPrompt": FollowUpPromptTypeDef,
-        "conclusionStatement": StatementTypeDef,
-        "dialogCodeHook": CodeHookTypeDef,
-        "fulfillmentActivity": FulfillmentActivityTypeDef,
+        "confirmationPrompt": PromptOutputTypeDef,
+        "rejectionStatement": StatementOutputTypeDef,
+        "followUpPrompt": FollowUpPromptOutputTypeDef,
+        "conclusionStatement": StatementOutputTypeDef,
+        "dialogCodeHook": CodeHookOutputTypeDef,
+        "fulfillmentActivity": FulfillmentActivityOutputTypeDef,
         "parentIntentSignature": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
-        "kendraConfiguration": KendraConfigurationTypeDef,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
+        "kendraConfiguration": KendraConfigurationOutputTypeDef,
+        "inputContexts": List[InputContextOutputTypeDef],
+        "outputContexts": List[OutputContextOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIntentResponseTypeDef = TypedDict(
     "GetIntentResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "slots": List[SlotTypeDef],
+        "slots": List[SlotOutputTypeDef],
         "sampleUtterances": List[str],
-        "confirmationPrompt": PromptTypeDef,
-        "rejectionStatement": StatementTypeDef,
-        "followUpPrompt": FollowUpPromptTypeDef,
-        "conclusionStatement": StatementTypeDef,
-        "dialogCodeHook": CodeHookTypeDef,
-        "fulfillmentActivity": FulfillmentActivityTypeDef,
+        "confirmationPrompt": PromptOutputTypeDef,
+        "rejectionStatement": StatementOutputTypeDef,
+        "followUpPrompt": FollowUpPromptOutputTypeDef,
+        "conclusionStatement": StatementOutputTypeDef,
+        "dialogCodeHook": CodeHookOutputTypeDef,
+        "fulfillmentActivity": FulfillmentActivityOutputTypeDef,
         "parentIntentSignature": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
-        "kendraConfiguration": KendraConfigurationTypeDef,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
+        "kendraConfiguration": KendraConfigurationOutputTypeDef,
+        "inputContexts": List[InputContextOutputTypeDef],
+        "outputContexts": List[OutputContextOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutIntentResponseTypeDef = TypedDict(
+    "PutIntentResponseTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "slots": List[SlotOutputTypeDef],
+        "sampleUtterances": List[str],
+        "confirmationPrompt": PromptOutputTypeDef,
+        "rejectionStatement": StatementOutputTypeDef,
+        "followUpPrompt": FollowUpPromptOutputTypeDef,
+        "conclusionStatement": StatementOutputTypeDef,
+        "dialogCodeHook": CodeHookOutputTypeDef,
+        "fulfillmentActivity": FulfillmentActivityOutputTypeDef,
+        "parentIntentSignature": str,
+        "lastUpdatedDate": datetime,
+        "createdDate": datetime,
+        "version": str,
+        "checksum": str,
+        "createVersion": bool,
+        "kendraConfiguration": KendraConfigurationOutputTypeDef,
+        "inputContexts": List[InputContextOutputTypeDef],
+        "outputContexts": List[OutputContextOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutIntentRequestRequestTypeDef = TypedDict(
     "_RequiredPutIntentRequestRequestTypeDef",
     {
@@ -1718,37 +2040,12 @@
         "kendraConfiguration": KendraConfigurationTypeDef,
         "inputContexts": Sequence[InputContextTypeDef],
         "outputContexts": Sequence[OutputContextTypeDef],
     },
     total=False,
 )
 
+
 class PutIntentRequestRequestTypeDef(
     _RequiredPutIntentRequestRequestTypeDef, _OptionalPutIntentRequestRequestTypeDef
 ):
     pass
-
-PutIntentResponseTypeDef = TypedDict(
-    "PutIntentResponseTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "slots": List[SlotTypeDef],
-        "sampleUtterances": List[str],
-        "confirmationPrompt": PromptTypeDef,
-        "rejectionStatement": StatementTypeDef,
-        "followUpPrompt": FollowUpPromptTypeDef,
-        "conclusionStatement": StatementTypeDef,
-        "dialogCodeHook": CodeHookTypeDef,
-        "fulfillmentActivity": FulfillmentActivityTypeDef,
-        "parentIntentSignature": str,
-        "lastUpdatedDate": datetime,
-        "createdDate": datetime,
-        "version": str,
-        "checksum": str,
-        "createVersion": bool,
-        "kendraConfiguration": KendraConfigurationTypeDef,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models.egg-info/PKG-INFO` & `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lex-models
-Version: 1.28.0
-Summary: Type annotations for boto3.LexModelBuildingService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.LexModelBuildingService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lex-models"></a>
 
 # mypy-boto3-lex-models
 
 [![PyPI - mypy-boto3-lex-models](https://img.shields.io/pypi/v/mypy-boto3-lex-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-models)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-models)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lex-models?color=blue)](https://pypistats.org/packages/mypy-boto3-lex-models)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lex-models)](https://pepy.tech/project/mypy-boto3-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexModelBuildingService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
+[boto3.LexModelBuildingService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
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
 [mypy-boto3-lex-models docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/).
 
 See how it helps to find and fix potential bugs:
 
@@ -386,35 +386,37 @@
 ```python
 from mypy_boto3_lex_models.type_defs import (
     BotChannelAssociationTypeDef,
     BotMetadataTypeDef,
     BuiltinIntentMetadataTypeDef,
     BuiltinIntentSlotTypeDef,
     BuiltinSlotTypeMetadataTypeDef,
+    CodeHookOutputTypeDef,
     CodeHookTypeDef,
     LogSettingsRequestTypeDef,
     LogSettingsResponseTypeDef,
     CreateBotVersionRequestRequestTypeDef,
-    IntentTypeDef,
+    IntentOutputTypeDef,
     CreateIntentVersionRequestRequestTypeDef,
-    InputContextTypeDef,
-    KendraConfigurationTypeDef,
-    OutputContextTypeDef,
+    InputContextOutputTypeDef,
+    KendraConfigurationOutputTypeDef,
+    OutputContextOutputTypeDef,
     CreateSlotTypeVersionRequestRequestTypeDef,
-    EnumerationValueTypeDef,
+    EnumerationValueOutputTypeDef,
     DeleteBotAliasRequestRequestTypeDef,
     DeleteBotChannelAssociationRequestRequestTypeDef,
     DeleteBotRequestRequestTypeDef,
     DeleteBotVersionRequestRequestTypeDef,
     DeleteIntentRequestRequestTypeDef,
     DeleteIntentVersionRequestRequestTypeDef,
     DeleteSlotTypeRequestRequestTypeDef,
     DeleteSlotTypeVersionRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
+    EnumerationValueTypeDef,
     GetBotAliasRequestRequestTypeDef,
     GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
     GetBotAliasesRequestRequestTypeDef,
     GetBotChannelAssociationRequestRequestTypeDef,
     GetBotChannelAssociationResponseTypeDef,
     GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
     GetBotChannelAssociationsRequestRequestTypeDef,
@@ -445,69 +447,84 @@
     GetSlotTypeRequestRequestTypeDef,
     GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
     GetSlotTypeVersionsRequestRequestTypeDef,
     SlotTypeMetadataTypeDef,
     GetSlotTypesRequestGetSlotTypesPaginateTypeDef,
     GetSlotTypesRequestRequestTypeDef,
     GetUtterancesViewRequestRequestTypeDef,
+    InputContextTypeDef,
+    IntentTypeDef,
+    KendraConfigurationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
+    MessageOutputTypeDef,
     MessageTypeDef,
+    OutputContextTypeDef,
     PaginatorConfigTypeDef,
+    TagTypeDef,
     ResponseMetadataTypeDef,
+    SlotDefaultValueOutputTypeDef,
     SlotDefaultValueTypeDef,
+    SlotTypeRegexConfigurationOutputTypeDef,
     SlotTypeRegexConfigurationTypeDef,
     StartMigrationRequestRequestTypeDef,
     StartMigrationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UtteranceDataTypeDef,
     GetBotChannelAssociationsResponseTypeDef,
     GetBotVersionsResponseTypeDef,
     GetBotsResponseTypeDef,
     GetBuiltinIntentsResponseTypeDef,
     GetBuiltinIntentResponseTypeDef,
     GetBuiltinSlotTypesResponseTypeDef,
+    FulfillmentActivityOutputTypeDef,
     FulfillmentActivityTypeDef,
     ConversationLogsRequestTypeDef,
     ConversationLogsResponseTypeDef,
     GetIntentVersionsResponseTypeDef,
     GetIntentsResponseTypeDef,
     GetMigrationResponseTypeDef,
     GetMigrationsResponseTypeDef,
     GetSlotTypeVersionsResponseTypeDef,
     GetSlotTypesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
+    PromptOutputTypeDef,
+    StatementOutputTypeDef,
     PromptTypeDef,
     StatementTypeDef,
+    StartImportRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    SlotDefaultValueSpecOutputTypeDef,
     SlotDefaultValueSpecTypeDef,
+    SlotTypeConfigurationOutputTypeDef,
     SlotTypeConfigurationTypeDef,
     UtteranceListTypeDef,
     PutBotAliasRequestRequestTypeDef,
     BotAliasMetadataTypeDef,
     GetBotAliasResponseTypeDef,
     PutBotAliasResponseTypeDef,
     CreateBotVersionResponseTypeDef,
-    FollowUpPromptTypeDef,
+    FollowUpPromptOutputTypeDef,
     GetBotResponseTypeDef,
-    PutBotRequestRequestTypeDef,
     PutBotResponseTypeDef,
+    FollowUpPromptTypeDef,
+    PutBotRequestRequestTypeDef,
+    SlotOutputTypeDef,
     SlotTypeDef,
     CreateSlotTypeVersionResponseTypeDef,
     GetSlotTypeResponseTypeDef,
-    PutSlotTypeRequestRequestTypeDef,
     PutSlotTypeResponseTypeDef,
+    PutSlotTypeRequestRequestTypeDef,
     GetUtterancesViewResponseTypeDef,
     GetBotAliasesResponseTypeDef,
     CreateIntentVersionResponseTypeDef,
     GetIntentResponseTypeDef,
-    PutIntentRequestRequestTypeDef,
     PutIntentResponseTypeDef,
+    PutIntentRequestRequestTypeDef,
 )
 
 
 def get_structure() -> BotChannelAssociationTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-lex-models-1.28.0/mypy_boto3_lex_models.egg-info/SOURCES.txt` & `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.0/setup.py` & `mypy-boto3-lex-models-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lex-models",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_lex_models"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LexModelBuildingService 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.LexModelBuildingService 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

