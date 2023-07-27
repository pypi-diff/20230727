# Comparing `tmp/mypy-boto3-iottwinmaker-1.28.0.tar.gz` & `tmp/mypy-boto3-iottwinmaker-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iottwinmaker-1.28.0.tar", last modified: Thu Jul  6 20:59:50 2023, max compression
+gzip compressed data, was "mypy-boto3-iottwinmaker-1.28.12.tar", last modified: Thu Jul 27 05:34:51 2023, max compression
```

## Comparing `mypy-boto3-iottwinmaker-1.28.0.tar` & `mypy-boto3-iottwinmaker-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:50.846336 mypy-boto3-iottwinmaker-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:44:07.000000 mypy-boto3-iottwinmaker-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16412 2023-07-06 20:59:50.846336 mypy-boto3-iottwinmaker-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-06 20:44:07.000000 mypy-boto3-iottwinmaker-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:50.834336 mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-06 20:44:07.000000 mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-06 20:44:07.000000 mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:44:07.000000 mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24767 2023-07-06 20:44:07.000000 mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24727 2023-07-06 20:44:07.000000 mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-06 20:44:08.000000 mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-06 20:44:08.000000 mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:44:07.000000 mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    43539 2023-07-06 20:44:11.000000 mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43466 2023-07-06 20:44:08.000000 mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:44:07.000000 mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:50.846336 mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16412 2023-07-06 20:59:50.000000 mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-06 20:59:50.000000 mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:50.000000 mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:50.000000 mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:50.000000 mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 20:59:50.000000 mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:50.846336 mypy-boto3-iottwinmaker-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:44:07.000000 mypy-boto3-iottwinmaker-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.288476 mypy-boto3-iottwinmaker-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16697 2023-07-27 05:34:51.288476 mypy-boto3-iottwinmaker-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15190 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.288476 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24767 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24727 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9642 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    47041 2023-07-27 05:24:18.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46960 2023-07-27 05:24:18.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.288476 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16697 2023-07-27 05:34:51.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-27 05:34:51.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:51.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:51.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:51.288476 mypy-boto3-iottwinmaker-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/setup.py
```

### Comparing `mypy-boto3-iottwinmaker-1.28.0/LICENSE` & `mypy-boto3-iottwinmaker-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.28.0/PKG-INFO` & `mypy-boto3-iottwinmaker-1.28.12/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iottwinmaker
-Version: 1.28.0
-Summary: Type annotations for boto3.IoTTwinMaker 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTTwinMaker 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iottwinmaker"></a>
 
 # mypy-boto3-iottwinmaker
 
 [![PyPI - mypy-boto3-iottwinmaker](https://img.shields.io/pypi/v/mypy-boto3-iottwinmaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-iottwinmaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iottwinmaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-iottwinmaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iottwinmaker?color=blue)](https://pypistats.org/packages/mypy-boto3-iottwinmaker)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iottwinmaker)](https://pepy.tech/project/mypy-boto3-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTTwinMaker 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
+[boto3.IoTTwinMaker 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
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
 [mypy-boto3-iottwinmaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,25 +330,29 @@
     CreateEntityResponseTypeDef,
     CreateSceneRequestRequestTypeDef,
     CreateSceneResponseTypeDef,
     CreateSyncJobRequestRequestTypeDef,
     CreateSyncJobResponseTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
     CreateWorkspaceResponseTypeDef,
+    LambdaFunctionOutputTypeDef,
     LambdaFunctionTypeDef,
+    RelationshipOutputTypeDef,
     RelationshipTypeDef,
+    RelationshipValueOutputTypeDef,
     RelationshipValueTypeDef,
     DeleteComponentTypeRequestRequestTypeDef,
     DeleteComponentTypeResponseTypeDef,
     DeleteEntityRequestRequestTypeDef,
     DeleteEntityResponseTypeDef,
     DeleteSceneRequestRequestTypeDef,
     DeleteSyncJobRequestRequestTypeDef,
     DeleteSyncJobResponseTypeDef,
     DeleteWorkspaceRequestRequestTypeDef,
+    EntityPropertyReferenceOutputTypeDef,
     EntityPropertyReferenceTypeDef,
     ErrorDetailsTypeDef,
     ExecuteQueryRequestRequestTypeDef,
     RowTypeDef,
     GetComponentTypeRequestRequestTypeDef,
     PropertyDefinitionResponseTypeDef,
     PropertyGroupResponseTypeDef,
@@ -368,29 +372,33 @@
     SyncResourceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkspacesRequestRequestTypeDef,
     WorkspaceSummaryTypeDef,
     OrderByTypeDef,
     ParentEntityUpdateRequestTypeDef,
+    PropertyValueOutputTypeDef,
     PropertyValueTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateComponentTypeResponseTypeDef,
     UpdateEntityResponseTypeDef,
     UpdatePricingPlanRequestRequestTypeDef,
     UpdateSceneRequestRequestTypeDef,
     UpdateSceneResponseTypeDef,
     UpdateWorkspaceRequestRequestTypeDef,
     UpdateWorkspaceResponseTypeDef,
     PricingPlanTypeDef,
     PropertyRequestTypeDef,
+    DataConnectorOutputTypeDef,
     DataConnectorTypeDef,
+    DataTypeOutputTypeDef,
     DataTypeTypeDef,
+    DataValueOutputTypeDef,
     DataValueTypeDef,
     PropertyLatestValueTypeDef,
     StatusTypeDef,
     SyncJobStatusTypeDef,
     SyncResourceStatusTypeDef,
     ExecuteQueryResponseTypeDef,
     PropertyResponseTypeDef,
@@ -398,38 +406,39 @@
     GetSceneResponseTypeDef,
     ListComponentTypesRequestRequestTypeDef,
     ListEntitiesRequestRequestTypeDef,
     ListScenesResponseTypeDef,
     ListSyncResourcesRequestRequestTypeDef,
     ListWorkspacesResponseTypeDef,
     TabularConditionsTypeDef,
-    PropertyValueEntryTypeDef,
+    PropertyValueEntryOutputTypeDef,
     PropertyValueHistoryTypeDef,
+    PropertyValueEntryTypeDef,
     GetPricingPlanResponseTypeDef,
     UpdatePricingPlanResponseTypeDef,
     ComponentRequestTypeDef,
     ComponentUpdateRequestTypeDef,
-    FunctionRequestTypeDef,
     FunctionResponseTypeDef,
+    FunctionRequestTypeDef,
     GetPropertyValueResponseTypeDef,
     ComponentTypeSummaryTypeDef,
     EntitySummaryTypeDef,
     GetSyncJobResponseTypeDef,
     SyncJobSummaryTypeDef,
     SyncResourceSummaryTypeDef,
     ComponentResponseTypeDef,
     GetPropertyValueRequestRequestTypeDef,
     BatchPutPropertyErrorTypeDef,
-    BatchPutPropertyValuesRequestRequestTypeDef,
     GetPropertyValueHistoryResponseTypeDef,
+    BatchPutPropertyValuesRequestRequestTypeDef,
     CreateEntityRequestRequestTypeDef,
     UpdateEntityRequestRequestTypeDef,
+    GetComponentTypeResponseTypeDef,
     CreateComponentTypeRequestRequestTypeDef,
     UpdateComponentTypeRequestRequestTypeDef,
-    GetComponentTypeResponseTypeDef,
     ListComponentTypesResponseTypeDef,
     ListEntitiesResponseTypeDef,
     ListSyncJobsResponseTypeDef,
     ListSyncResourcesResponseTypeDef,
     GetEntityResponseTypeDef,
     BatchPutPropertyErrorEntryTypeDef,
     BatchPutPropertyValuesResponseTypeDef,
```

### Comparing `mypy-boto3-iottwinmaker-1.28.0/README.md` & `mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-iottwinmaker
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTTwinMaker 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 iottwinmaker type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-iottwinmaker"></a>
 
 # mypy-boto3-iottwinmaker
 
 [![PyPI - mypy-boto3-iottwinmaker](https://img.shields.io/pypi/v/mypy-boto3-iottwinmaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-iottwinmaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iottwinmaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-iottwinmaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iottwinmaker?color=blue)](https://pypistats.org/packages/mypy-boto3-iottwinmaker)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iottwinmaker)](https://pepy.tech/project/mypy-boto3-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTTwinMaker 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
+[boto3.IoTTwinMaker 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
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
 [mypy-boto3-iottwinmaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,25 +330,29 @@
     CreateEntityResponseTypeDef,
     CreateSceneRequestRequestTypeDef,
     CreateSceneResponseTypeDef,
     CreateSyncJobRequestRequestTypeDef,
     CreateSyncJobResponseTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
     CreateWorkspaceResponseTypeDef,
+    LambdaFunctionOutputTypeDef,
     LambdaFunctionTypeDef,
+    RelationshipOutputTypeDef,
     RelationshipTypeDef,
+    RelationshipValueOutputTypeDef,
     RelationshipValueTypeDef,
     DeleteComponentTypeRequestRequestTypeDef,
     DeleteComponentTypeResponseTypeDef,
     DeleteEntityRequestRequestTypeDef,
     DeleteEntityResponseTypeDef,
     DeleteSceneRequestRequestTypeDef,
     DeleteSyncJobRequestRequestTypeDef,
     DeleteSyncJobResponseTypeDef,
     DeleteWorkspaceRequestRequestTypeDef,
+    EntityPropertyReferenceOutputTypeDef,
     EntityPropertyReferenceTypeDef,
     ErrorDetailsTypeDef,
     ExecuteQueryRequestRequestTypeDef,
     RowTypeDef,
     GetComponentTypeRequestRequestTypeDef,
     PropertyDefinitionResponseTypeDef,
     PropertyGroupResponseTypeDef,
@@ -336,29 +372,33 @@
     SyncResourceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkspacesRequestRequestTypeDef,
     WorkspaceSummaryTypeDef,
     OrderByTypeDef,
     ParentEntityUpdateRequestTypeDef,
+    PropertyValueOutputTypeDef,
     PropertyValueTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateComponentTypeResponseTypeDef,
     UpdateEntityResponseTypeDef,
     UpdatePricingPlanRequestRequestTypeDef,
     UpdateSceneRequestRequestTypeDef,
     UpdateSceneResponseTypeDef,
     UpdateWorkspaceRequestRequestTypeDef,
     UpdateWorkspaceResponseTypeDef,
     PricingPlanTypeDef,
     PropertyRequestTypeDef,
+    DataConnectorOutputTypeDef,
     DataConnectorTypeDef,
+    DataTypeOutputTypeDef,
     DataTypeTypeDef,
+    DataValueOutputTypeDef,
     DataValueTypeDef,
     PropertyLatestValueTypeDef,
     StatusTypeDef,
     SyncJobStatusTypeDef,
     SyncResourceStatusTypeDef,
     ExecuteQueryResponseTypeDef,
     PropertyResponseTypeDef,
@@ -366,38 +406,39 @@
     GetSceneResponseTypeDef,
     ListComponentTypesRequestRequestTypeDef,
     ListEntitiesRequestRequestTypeDef,
     ListScenesResponseTypeDef,
     ListSyncResourcesRequestRequestTypeDef,
     ListWorkspacesResponseTypeDef,
     TabularConditionsTypeDef,
-    PropertyValueEntryTypeDef,
+    PropertyValueEntryOutputTypeDef,
     PropertyValueHistoryTypeDef,
+    PropertyValueEntryTypeDef,
     GetPricingPlanResponseTypeDef,
     UpdatePricingPlanResponseTypeDef,
     ComponentRequestTypeDef,
     ComponentUpdateRequestTypeDef,
-    FunctionRequestTypeDef,
     FunctionResponseTypeDef,
+    FunctionRequestTypeDef,
     GetPropertyValueResponseTypeDef,
     ComponentTypeSummaryTypeDef,
     EntitySummaryTypeDef,
     GetSyncJobResponseTypeDef,
     SyncJobSummaryTypeDef,
     SyncResourceSummaryTypeDef,
     ComponentResponseTypeDef,
     GetPropertyValueRequestRequestTypeDef,
     BatchPutPropertyErrorTypeDef,
-    BatchPutPropertyValuesRequestRequestTypeDef,
     GetPropertyValueHistoryResponseTypeDef,
+    BatchPutPropertyValuesRequestRequestTypeDef,
     CreateEntityRequestRequestTypeDef,
     UpdateEntityRequestRequestTypeDef,
+    GetComponentTypeResponseTypeDef,
     CreateComponentTypeRequestRequestTypeDef,
     UpdateComponentTypeRequestRequestTypeDef,
-    GetComponentTypeResponseTypeDef,
     ListComponentTypesResponseTypeDef,
     ListEntitiesResponseTypeDef,
     ListSyncJobsResponseTypeDef,
     ListSyncResourcesResponseTypeDef,
     GetEntityResponseTypeDef,
     BatchPutPropertyErrorEntryTypeDef,
     BatchPutPropertyValuesResponseTypeDef,
```

### Comparing `mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker/__main__.py` & `mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTTwinMaker 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.IoTTwinMaker 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker\nOther"
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

### Comparing `mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker/client.py` & `mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker/client.pyi` & `mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker/literals.py` & `mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,15 @@
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
@@ -277,26 +278,28 @@
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

### Comparing `mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker/literals.pyi` & `mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,15 @@
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
@@ -275,26 +276,28 @@
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

### Comparing `mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker/type_defs.py` & `mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,25 +56,29 @@
     "CreateEntityResponseTypeDef",
     "CreateSceneRequestRequestTypeDef",
     "CreateSceneResponseTypeDef",
     "CreateSyncJobRequestRequestTypeDef",
     "CreateSyncJobResponseTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
     "CreateWorkspaceResponseTypeDef",
+    "LambdaFunctionOutputTypeDef",
     "LambdaFunctionTypeDef",
+    "RelationshipOutputTypeDef",
     "RelationshipTypeDef",
+    "RelationshipValueOutputTypeDef",
     "RelationshipValueTypeDef",
     "DeleteComponentTypeRequestRequestTypeDef",
     "DeleteComponentTypeResponseTypeDef",
     "DeleteEntityRequestRequestTypeDef",
     "DeleteEntityResponseTypeDef",
     "DeleteSceneRequestRequestTypeDef",
     "DeleteSyncJobRequestRequestTypeDef",
     "DeleteSyncJobResponseTypeDef",
     "DeleteWorkspaceRequestRequestTypeDef",
+    "EntityPropertyReferenceOutputTypeDef",
     "EntityPropertyReferenceTypeDef",
     "ErrorDetailsTypeDef",
     "ExecuteQueryRequestRequestTypeDef",
     "RowTypeDef",
     "GetComponentTypeRequestRequestTypeDef",
     "PropertyDefinitionResponseTypeDef",
     "PropertyGroupResponseTypeDef",
@@ -94,29 +98,33 @@
     "SyncResourceFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
     "WorkspaceSummaryTypeDef",
     "OrderByTypeDef",
     "ParentEntityUpdateRequestTypeDef",
+    "PropertyValueOutputTypeDef",
     "PropertyValueTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateComponentTypeResponseTypeDef",
     "UpdateEntityResponseTypeDef",
     "UpdatePricingPlanRequestRequestTypeDef",
     "UpdateSceneRequestRequestTypeDef",
     "UpdateSceneResponseTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
     "UpdateWorkspaceResponseTypeDef",
     "PricingPlanTypeDef",
     "PropertyRequestTypeDef",
+    "DataConnectorOutputTypeDef",
     "DataConnectorTypeDef",
+    "DataTypeOutputTypeDef",
     "DataTypeTypeDef",
+    "DataValueOutputTypeDef",
     "DataValueTypeDef",
     "PropertyLatestValueTypeDef",
     "StatusTypeDef",
     "SyncJobStatusTypeDef",
     "SyncResourceStatusTypeDef",
     "ExecuteQueryResponseTypeDef",
     "PropertyResponseTypeDef",
@@ -124,38 +132,39 @@
     "GetSceneResponseTypeDef",
     "ListComponentTypesRequestRequestTypeDef",
     "ListEntitiesRequestRequestTypeDef",
     "ListScenesResponseTypeDef",
     "ListSyncResourcesRequestRequestTypeDef",
     "ListWorkspacesResponseTypeDef",
     "TabularConditionsTypeDef",
-    "PropertyValueEntryTypeDef",
+    "PropertyValueEntryOutputTypeDef",
     "PropertyValueHistoryTypeDef",
+    "PropertyValueEntryTypeDef",
     "GetPricingPlanResponseTypeDef",
     "UpdatePricingPlanResponseTypeDef",
     "ComponentRequestTypeDef",
     "ComponentUpdateRequestTypeDef",
-    "FunctionRequestTypeDef",
     "FunctionResponseTypeDef",
+    "FunctionRequestTypeDef",
     "GetPropertyValueResponseTypeDef",
     "ComponentTypeSummaryTypeDef",
     "EntitySummaryTypeDef",
     "GetSyncJobResponseTypeDef",
     "SyncJobSummaryTypeDef",
     "SyncResourceSummaryTypeDef",
     "ComponentResponseTypeDef",
     "GetPropertyValueRequestRequestTypeDef",
     "BatchPutPropertyErrorTypeDef",
-    "BatchPutPropertyValuesRequestRequestTypeDef",
     "GetPropertyValueHistoryResponseTypeDef",
+    "BatchPutPropertyValuesRequestRequestTypeDef",
     "CreateEntityRequestRequestTypeDef",
     "UpdateEntityRequestRequestTypeDef",
+    "GetComponentTypeResponseTypeDef",
     "CreateComponentTypeRequestRequestTypeDef",
     "UpdateComponentTypeRequestRequestTypeDef",
-    "GetComponentTypeResponseTypeDef",
     "ListComponentTypesResponseTypeDef",
     "ListEntitiesResponseTypeDef",
     "ListSyncJobsResponseTypeDef",
     "ListSyncResourcesResponseTypeDef",
     "GetEntityResponseTypeDef",
     "BatchPutPropertyErrorEntryTypeDef",
     "BatchPutPropertyValuesResponseTypeDef",
@@ -352,30 +361,55 @@
     {
         "arn": str,
         "creationDateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LambdaFunctionOutputTypeDef = TypedDict(
+    "LambdaFunctionOutputTypeDef",
+    {
+        "arn": str,
+    },
+)
+
 LambdaFunctionTypeDef = TypedDict(
     "LambdaFunctionTypeDef",
     {
         "arn": str,
     },
 )
 
+RelationshipOutputTypeDef = TypedDict(
+    "RelationshipOutputTypeDef",
+    {
+        "targetComponentTypeId": str,
+        "relationshipType": str,
+    },
+    total=False,
+)
+
 RelationshipTypeDef = TypedDict(
     "RelationshipTypeDef",
     {
         "targetComponentTypeId": str,
         "relationshipType": str,
     },
     total=False,
 )
 
+RelationshipValueOutputTypeDef = TypedDict(
+    "RelationshipValueOutputTypeDef",
+    {
+        "targetEntityId": str,
+        "targetComponentName": str,
+    },
+    total=False,
+)
+
 RelationshipValueTypeDef = TypedDict(
     "RelationshipValueTypeDef",
     {
         "targetEntityId": str,
         "targetComponentName": str,
     },
     total=False,
@@ -454,14 +488,37 @@
 DeleteWorkspaceRequestRequestTypeDef = TypedDict(
     "DeleteWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 
+_RequiredEntityPropertyReferenceOutputTypeDef = TypedDict(
+    "_RequiredEntityPropertyReferenceOutputTypeDef",
+    {
+        "propertyName": str,
+    },
+)
+_OptionalEntityPropertyReferenceOutputTypeDef = TypedDict(
+    "_OptionalEntityPropertyReferenceOutputTypeDef",
+    {
+        "componentName": str,
+        "externalIdProperty": Dict[str, str],
+        "entityId": str,
+    },
+    total=False,
+)
+
+
+class EntityPropertyReferenceOutputTypeDef(
+    _RequiredEntityPropertyReferenceOutputTypeDef, _OptionalEntityPropertyReferenceOutputTypeDef
+):
+    pass
+
+
 _RequiredEntityPropertyReferenceTypeDef = TypedDict(
     "_RequiredEntityPropertyReferenceTypeDef",
     {
         "propertyName": str,
     },
 )
 _OptionalEntityPropertyReferenceTypeDef = TypedDict(
@@ -528,28 +585,28 @@
         "componentTypeId": str,
     },
 )
 
 _RequiredPropertyDefinitionResponseTypeDef = TypedDict(
     "_RequiredPropertyDefinitionResponseTypeDef",
     {
-        "dataType": "DataTypeTypeDef",
+        "dataType": "DataTypeOutputTypeDef",
         "isTimeSeries": bool,
         "isRequiredInEntity": bool,
         "isExternalId": bool,
         "isStoredExternally": bool,
         "isImported": bool,
         "isFinal": bool,
         "isInherited": bool,
     },
 )
 _OptionalPropertyDefinitionResponseTypeDef = TypedDict(
     "_OptionalPropertyDefinitionResponseTypeDef",
     {
-        "defaultValue": "DataValueTypeDef",
+        "defaultValue": "DataValueOutputTypeDef",
         "configuration": Dict[str, str],
         "displayName": str,
     },
     total=False,
 )
 
 
@@ -851,14 +908,36 @@
 
 class ParentEntityUpdateRequestTypeDef(
     _RequiredParentEntityUpdateRequestTypeDef, _OptionalParentEntityUpdateRequestTypeDef
 ):
     pass
 
 
+_RequiredPropertyValueOutputTypeDef = TypedDict(
+    "_RequiredPropertyValueOutputTypeDef",
+    {
+        "value": "DataValueOutputTypeDef",
+    },
+)
+_OptionalPropertyValueOutputTypeDef = TypedDict(
+    "_OptionalPropertyValueOutputTypeDef",
+    {
+        "timestamp": datetime,
+        "time": str,
+    },
+    total=False,
+)
+
+
+class PropertyValueOutputTypeDef(
+    _RequiredPropertyValueOutputTypeDef, _OptionalPropertyValueOutputTypeDef
+):
+    pass
+
+
 _RequiredPropertyValueTypeDef = TypedDict(
     "_RequiredPropertyValueTypeDef",
     {
         "value": "DataValueTypeDef",
     },
 )
 _OptionalPropertyValueTypeDef = TypedDict(
@@ -1035,23 +1114,54 @@
         "definition": PropertyDefinitionRequestTypeDef,
         "value": "DataValueTypeDef",
         "updateType": PropertyUpdateTypeType,
     },
     total=False,
 )
 
+DataConnectorOutputTypeDef = TypedDict(
+    "DataConnectorOutputTypeDef",
+    {
+        "lambda": LambdaFunctionOutputTypeDef,
+        "isNative": bool,
+    },
+    total=False,
+)
+
 DataConnectorTypeDef = TypedDict(
     "DataConnectorTypeDef",
     {
         "lambda": LambdaFunctionTypeDef,
         "isNative": bool,
     },
     total=False,
 )
 
+_RequiredDataTypeOutputTypeDef = TypedDict(
+    "_RequiredDataTypeOutputTypeDef",
+    {
+        "type": TypeType,
+    },
+)
+_OptionalDataTypeOutputTypeDef = TypedDict(
+    "_OptionalDataTypeOutputTypeDef",
+    {
+        "nestedType": Dict[str, Any],
+        "allowedValues": List["DataValueOutputTypeDef"],
+        "unitOfMeasure": str,
+        "relationship": RelationshipOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class DataTypeOutputTypeDef(_RequiredDataTypeOutputTypeDef, _OptionalDataTypeOutputTypeDef):
+    pass
+
+
 _RequiredDataTypeTypeDef = TypedDict(
     "_RequiredDataTypeTypeDef",
     {
         "type": TypeType,
     },
 )
 _OptionalDataTypeTypeDef = TypedDict(
@@ -1066,14 +1176,30 @@
 )
 
 
 class DataTypeTypeDef(_RequiredDataTypeTypeDef, _OptionalDataTypeTypeDef):
     pass
 
 
+DataValueOutputTypeDef = TypedDict(
+    "DataValueOutputTypeDef",
+    {
+        "booleanValue": bool,
+        "doubleValue": float,
+        "integerValue": int,
+        "longValue": int,
+        "stringValue": str,
+        "listValue": List[Dict[str, Any]],
+        "mapValue": Dict[str, Dict[str, Any]],
+        "relationshipValue": RelationshipValueOutputTypeDef,
+        "expression": str,
+    },
+    total=False,
+)
+
 DataValueTypeDef = TypedDict(
     "DataValueTypeDef",
     {
         "booleanValue": bool,
         "doubleValue": float,
         "integerValue": int,
         "longValue": int,
@@ -1085,21 +1211,21 @@
     },
     total=False,
 )
 
 _RequiredPropertyLatestValueTypeDef = TypedDict(
     "_RequiredPropertyLatestValueTypeDef",
     {
-        "propertyReference": EntityPropertyReferenceTypeDef,
+        "propertyReference": EntityPropertyReferenceOutputTypeDef,
     },
 )
 _OptionalPropertyLatestValueTypeDef = TypedDict(
     "_OptionalPropertyLatestValueTypeDef",
     {
-        "propertyValue": "DataValueTypeDef",
+        "propertyValue": "DataValueOutputTypeDef",
     },
     total=False,
 )
 
 
 class PropertyLatestValueTypeDef(
     _RequiredPropertyLatestValueTypeDef, _OptionalPropertyLatestValueTypeDef
@@ -1144,15 +1270,15 @@
     },
 )
 
 PropertyResponseTypeDef = TypedDict(
     "PropertyResponseTypeDef",
     {
         "definition": PropertyDefinitionResponseTypeDef,
-        "value": "DataValueTypeDef",
+        "value": "DataValueOutputTypeDef",
     },
     total=False,
 )
 
 _RequiredGetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetPropertyValueHistoryRequestRequestTypeDef",
     {
@@ -1299,56 +1425,77 @@
     {
         "orderBy": Sequence[OrderByTypeDef],
         "propertyFilters": Sequence[PropertyFilterTypeDef],
     },
     total=False,
 )
 
-_RequiredPropertyValueEntryTypeDef = TypedDict(
-    "_RequiredPropertyValueEntryTypeDef",
+_RequiredPropertyValueEntryOutputTypeDef = TypedDict(
+    "_RequiredPropertyValueEntryOutputTypeDef",
     {
-        "entityPropertyReference": EntityPropertyReferenceTypeDef,
+        "entityPropertyReference": EntityPropertyReferenceOutputTypeDef,
     },
 )
-_OptionalPropertyValueEntryTypeDef = TypedDict(
-    "_OptionalPropertyValueEntryTypeDef",
+_OptionalPropertyValueEntryOutputTypeDef = TypedDict(
+    "_OptionalPropertyValueEntryOutputTypeDef",
     {
-        "propertyValues": Sequence[PropertyValueTypeDef],
+        "propertyValues": List[PropertyValueOutputTypeDef],
     },
     total=False,
 )
 
 
-class PropertyValueEntryTypeDef(
-    _RequiredPropertyValueEntryTypeDef, _OptionalPropertyValueEntryTypeDef
+class PropertyValueEntryOutputTypeDef(
+    _RequiredPropertyValueEntryOutputTypeDef, _OptionalPropertyValueEntryOutputTypeDef
 ):
     pass
 
 
 _RequiredPropertyValueHistoryTypeDef = TypedDict(
     "_RequiredPropertyValueHistoryTypeDef",
     {
-        "entityPropertyReference": EntityPropertyReferenceTypeDef,
+        "entityPropertyReference": EntityPropertyReferenceOutputTypeDef,
     },
 )
 _OptionalPropertyValueHistoryTypeDef = TypedDict(
     "_OptionalPropertyValueHistoryTypeDef",
     {
-        "values": List[PropertyValueTypeDef],
+        "values": List[PropertyValueOutputTypeDef],
     },
     total=False,
 )
 
 
 class PropertyValueHistoryTypeDef(
     _RequiredPropertyValueHistoryTypeDef, _OptionalPropertyValueHistoryTypeDef
 ):
     pass
 
 
+_RequiredPropertyValueEntryTypeDef = TypedDict(
+    "_RequiredPropertyValueEntryTypeDef",
+    {
+        "entityPropertyReference": EntityPropertyReferenceTypeDef,
+    },
+)
+_OptionalPropertyValueEntryTypeDef = TypedDict(
+    "_OptionalPropertyValueEntryTypeDef",
+    {
+        "propertyValues": Sequence[PropertyValueTypeDef],
+    },
+    total=False,
+)
+
+
+class PropertyValueEntryTypeDef(
+    _RequiredPropertyValueEntryTypeDef, _OptionalPropertyValueEntryTypeDef
+):
+    pass
+
+
 GetPricingPlanResponseTypeDef = TypedDict(
     "GetPricingPlanResponseTypeDef",
     {
         "currentPricingPlan": PricingPlanTypeDef,
         "pendingPricingPlan": PricingPlanTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1382,41 +1529,41 @@
         "componentTypeId": str,
         "propertyUpdates": Mapping[str, PropertyRequestTypeDef],
         "propertyGroupUpdates": Mapping[str, ComponentPropertyGroupRequestTypeDef],
     },
     total=False,
 )
 
-FunctionRequestTypeDef = TypedDict(
-    "FunctionRequestTypeDef",
+FunctionResponseTypeDef = TypedDict(
+    "FunctionResponseTypeDef",
     {
-        "requiredProperties": Sequence[str],
+        "requiredProperties": List[str],
         "scope": ScopeType,
-        "implementedBy": DataConnectorTypeDef,
+        "implementedBy": DataConnectorOutputTypeDef,
+        "isInherited": bool,
     },
     total=False,
 )
 
-FunctionResponseTypeDef = TypedDict(
-    "FunctionResponseTypeDef",
+FunctionRequestTypeDef = TypedDict(
+    "FunctionRequestTypeDef",
     {
-        "requiredProperties": List[str],
+        "requiredProperties": Sequence[str],
         "scope": ScopeType,
         "implementedBy": DataConnectorTypeDef,
-        "isInherited": bool,
     },
     total=False,
 )
 
 GetPropertyValueResponseTypeDef = TypedDict(
     "GetPropertyValueResponseTypeDef",
     {
         "propertyValues": Dict[str, PropertyLatestValueTypeDef],
         "nextToken": str,
-        "tabularPropertyValues": List[List[Dict[str, "DataValueTypeDef"]]],
+        "tabularPropertyValues": List[List[Dict[str, "DataValueOutputTypeDef"]]],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredComponentTypeSummaryTypeDef = TypedDict(
     "_RequiredComponentTypeSummaryTypeDef",
     {
@@ -1552,35 +1699,35 @@
 
 
 BatchPutPropertyErrorTypeDef = TypedDict(
     "BatchPutPropertyErrorTypeDef",
     {
         "errorCode": str,
         "errorMessage": str,
-        "entry": PropertyValueEntryTypeDef,
-    },
-)
-
-BatchPutPropertyValuesRequestRequestTypeDef = TypedDict(
-    "BatchPutPropertyValuesRequestRequestTypeDef",
-    {
-        "workspaceId": str,
-        "entries": Sequence[PropertyValueEntryTypeDef],
+        "entry": PropertyValueEntryOutputTypeDef,
     },
 )
 
 GetPropertyValueHistoryResponseTypeDef = TypedDict(
     "GetPropertyValueHistoryResponseTypeDef",
     {
         "propertyValues": List[PropertyValueHistoryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+BatchPutPropertyValuesRequestRequestTypeDef = TypedDict(
+    "BatchPutPropertyValuesRequestRequestTypeDef",
+    {
+        "workspaceId": str,
+        "entries": Sequence[PropertyValueEntryTypeDef],
+    },
+)
+
 _RequiredCreateEntityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEntityRequestRequestTypeDef",
     {
         "workspaceId": str,
         "entityName": str,
     },
 )
@@ -1624,14 +1771,37 @@
 
 class UpdateEntityRequestRequestTypeDef(
     _RequiredUpdateEntityRequestRequestTypeDef, _OptionalUpdateEntityRequestRequestTypeDef
 ):
     pass
 
 
+GetComponentTypeResponseTypeDef = TypedDict(
+    "GetComponentTypeResponseTypeDef",
+    {
+        "workspaceId": str,
+        "isSingleton": bool,
+        "componentTypeId": str,
+        "description": str,
+        "propertyDefinitions": Dict[str, PropertyDefinitionResponseTypeDef],
+        "extendsFrom": List[str],
+        "functions": Dict[str, FunctionResponseTypeDef],
+        "creationDateTime": datetime,
+        "updateDateTime": datetime,
+        "arn": str,
+        "isAbstract": bool,
+        "isSchemaInitialized": bool,
+        "status": StatusTypeDef,
+        "propertyGroups": Dict[str, PropertyGroupResponseTypeDef],
+        "syncSource": str,
+        "componentTypeName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateComponentTypeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateComponentTypeRequestRequestTypeDef",
     {
         "workspaceId": str,
         "componentTypeId": str,
     },
 )
@@ -1683,37 +1853,14 @@
 class UpdateComponentTypeRequestRequestTypeDef(
     _RequiredUpdateComponentTypeRequestRequestTypeDef,
     _OptionalUpdateComponentTypeRequestRequestTypeDef,
 ):
     pass
 
 
-GetComponentTypeResponseTypeDef = TypedDict(
-    "GetComponentTypeResponseTypeDef",
-    {
-        "workspaceId": str,
-        "isSingleton": bool,
-        "componentTypeId": str,
-        "description": str,
-        "propertyDefinitions": Dict[str, PropertyDefinitionResponseTypeDef],
-        "extendsFrom": List[str],
-        "functions": Dict[str, FunctionResponseTypeDef],
-        "creationDateTime": datetime,
-        "updateDateTime": datetime,
-        "arn": str,
-        "isAbstract": bool,
-        "isSchemaInitialized": bool,
-        "status": StatusTypeDef,
-        "propertyGroups": Dict[str, PropertyGroupResponseTypeDef],
-        "syncSource": str,
-        "componentTypeName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListComponentTypesResponseTypeDef = TypedDict(
     "ListComponentTypesResponseTypeDef",
     {
         "workspaceId": str,
         "componentTypeSummaries": List[ComponentTypeSummaryTypeDef],
         "nextToken": str,
         "maxResults": int,
```

### Comparing `mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker/type_defs.pyi` & `mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -55,25 +55,29 @@
     "CreateEntityResponseTypeDef",
     "CreateSceneRequestRequestTypeDef",
     "CreateSceneResponseTypeDef",
     "CreateSyncJobRequestRequestTypeDef",
     "CreateSyncJobResponseTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
     "CreateWorkspaceResponseTypeDef",
+    "LambdaFunctionOutputTypeDef",
     "LambdaFunctionTypeDef",
+    "RelationshipOutputTypeDef",
     "RelationshipTypeDef",
+    "RelationshipValueOutputTypeDef",
     "RelationshipValueTypeDef",
     "DeleteComponentTypeRequestRequestTypeDef",
     "DeleteComponentTypeResponseTypeDef",
     "DeleteEntityRequestRequestTypeDef",
     "DeleteEntityResponseTypeDef",
     "DeleteSceneRequestRequestTypeDef",
     "DeleteSyncJobRequestRequestTypeDef",
     "DeleteSyncJobResponseTypeDef",
     "DeleteWorkspaceRequestRequestTypeDef",
+    "EntityPropertyReferenceOutputTypeDef",
     "EntityPropertyReferenceTypeDef",
     "ErrorDetailsTypeDef",
     "ExecuteQueryRequestRequestTypeDef",
     "RowTypeDef",
     "GetComponentTypeRequestRequestTypeDef",
     "PropertyDefinitionResponseTypeDef",
     "PropertyGroupResponseTypeDef",
@@ -93,29 +97,33 @@
     "SyncResourceFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
     "WorkspaceSummaryTypeDef",
     "OrderByTypeDef",
     "ParentEntityUpdateRequestTypeDef",
+    "PropertyValueOutputTypeDef",
     "PropertyValueTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateComponentTypeResponseTypeDef",
     "UpdateEntityResponseTypeDef",
     "UpdatePricingPlanRequestRequestTypeDef",
     "UpdateSceneRequestRequestTypeDef",
     "UpdateSceneResponseTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
     "UpdateWorkspaceResponseTypeDef",
     "PricingPlanTypeDef",
     "PropertyRequestTypeDef",
+    "DataConnectorOutputTypeDef",
     "DataConnectorTypeDef",
+    "DataTypeOutputTypeDef",
     "DataTypeTypeDef",
+    "DataValueOutputTypeDef",
     "DataValueTypeDef",
     "PropertyLatestValueTypeDef",
     "StatusTypeDef",
     "SyncJobStatusTypeDef",
     "SyncResourceStatusTypeDef",
     "ExecuteQueryResponseTypeDef",
     "PropertyResponseTypeDef",
@@ -123,38 +131,39 @@
     "GetSceneResponseTypeDef",
     "ListComponentTypesRequestRequestTypeDef",
     "ListEntitiesRequestRequestTypeDef",
     "ListScenesResponseTypeDef",
     "ListSyncResourcesRequestRequestTypeDef",
     "ListWorkspacesResponseTypeDef",
     "TabularConditionsTypeDef",
-    "PropertyValueEntryTypeDef",
+    "PropertyValueEntryOutputTypeDef",
     "PropertyValueHistoryTypeDef",
+    "PropertyValueEntryTypeDef",
     "GetPricingPlanResponseTypeDef",
     "UpdatePricingPlanResponseTypeDef",
     "ComponentRequestTypeDef",
     "ComponentUpdateRequestTypeDef",
-    "FunctionRequestTypeDef",
     "FunctionResponseTypeDef",
+    "FunctionRequestTypeDef",
     "GetPropertyValueResponseTypeDef",
     "ComponentTypeSummaryTypeDef",
     "EntitySummaryTypeDef",
     "GetSyncJobResponseTypeDef",
     "SyncJobSummaryTypeDef",
     "SyncResourceSummaryTypeDef",
     "ComponentResponseTypeDef",
     "GetPropertyValueRequestRequestTypeDef",
     "BatchPutPropertyErrorTypeDef",
-    "BatchPutPropertyValuesRequestRequestTypeDef",
     "GetPropertyValueHistoryResponseTypeDef",
+    "BatchPutPropertyValuesRequestRequestTypeDef",
     "CreateEntityRequestRequestTypeDef",
     "UpdateEntityRequestRequestTypeDef",
+    "GetComponentTypeResponseTypeDef",
     "CreateComponentTypeRequestRequestTypeDef",
     "UpdateComponentTypeRequestRequestTypeDef",
-    "GetComponentTypeResponseTypeDef",
     "ListComponentTypesResponseTypeDef",
     "ListEntitiesResponseTypeDef",
     "ListSyncJobsResponseTypeDef",
     "ListSyncResourcesResponseTypeDef",
     "GetEntityResponseTypeDef",
     "BatchPutPropertyErrorEntryTypeDef",
     "BatchPutPropertyValuesResponseTypeDef",
@@ -343,30 +352,55 @@
     {
         "arn": str,
         "creationDateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LambdaFunctionOutputTypeDef = TypedDict(
+    "LambdaFunctionOutputTypeDef",
+    {
+        "arn": str,
+    },
+)
+
 LambdaFunctionTypeDef = TypedDict(
     "LambdaFunctionTypeDef",
     {
         "arn": str,
     },
 )
 
+RelationshipOutputTypeDef = TypedDict(
+    "RelationshipOutputTypeDef",
+    {
+        "targetComponentTypeId": str,
+        "relationshipType": str,
+    },
+    total=False,
+)
+
 RelationshipTypeDef = TypedDict(
     "RelationshipTypeDef",
     {
         "targetComponentTypeId": str,
         "relationshipType": str,
     },
     total=False,
 )
 
+RelationshipValueOutputTypeDef = TypedDict(
+    "RelationshipValueOutputTypeDef",
+    {
+        "targetEntityId": str,
+        "targetComponentName": str,
+    },
+    total=False,
+)
+
 RelationshipValueTypeDef = TypedDict(
     "RelationshipValueTypeDef",
     {
         "targetEntityId": str,
         "targetComponentName": str,
     },
     total=False,
@@ -443,14 +477,35 @@
 DeleteWorkspaceRequestRequestTypeDef = TypedDict(
     "DeleteWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 
+_RequiredEntityPropertyReferenceOutputTypeDef = TypedDict(
+    "_RequiredEntityPropertyReferenceOutputTypeDef",
+    {
+        "propertyName": str,
+    },
+)
+_OptionalEntityPropertyReferenceOutputTypeDef = TypedDict(
+    "_OptionalEntityPropertyReferenceOutputTypeDef",
+    {
+        "componentName": str,
+        "externalIdProperty": Dict[str, str],
+        "entityId": str,
+    },
+    total=False,
+)
+
+class EntityPropertyReferenceOutputTypeDef(
+    _RequiredEntityPropertyReferenceOutputTypeDef, _OptionalEntityPropertyReferenceOutputTypeDef
+):
+    pass
+
 _RequiredEntityPropertyReferenceTypeDef = TypedDict(
     "_RequiredEntityPropertyReferenceTypeDef",
     {
         "propertyName": str,
     },
 )
 _OptionalEntityPropertyReferenceTypeDef = TypedDict(
@@ -513,28 +568,28 @@
         "componentTypeId": str,
     },
 )
 
 _RequiredPropertyDefinitionResponseTypeDef = TypedDict(
     "_RequiredPropertyDefinitionResponseTypeDef",
     {
-        "dataType": "DataTypeTypeDef",
+        "dataType": "DataTypeOutputTypeDef",
         "isTimeSeries": bool,
         "isRequiredInEntity": bool,
         "isExternalId": bool,
         "isStoredExternally": bool,
         "isImported": bool,
         "isFinal": bool,
         "isInherited": bool,
     },
 )
 _OptionalPropertyDefinitionResponseTypeDef = TypedDict(
     "_OptionalPropertyDefinitionResponseTypeDef",
     {
-        "defaultValue": "DataValueTypeDef",
+        "defaultValue": "DataValueOutputTypeDef",
         "configuration": Dict[str, str],
         "displayName": str,
     },
     total=False,
 )
 
 class PropertyDefinitionResponseTypeDef(
@@ -818,14 +873,34 @@
 )
 
 class ParentEntityUpdateRequestTypeDef(
     _RequiredParentEntityUpdateRequestTypeDef, _OptionalParentEntityUpdateRequestTypeDef
 ):
     pass
 
+_RequiredPropertyValueOutputTypeDef = TypedDict(
+    "_RequiredPropertyValueOutputTypeDef",
+    {
+        "value": "DataValueOutputTypeDef",
+    },
+)
+_OptionalPropertyValueOutputTypeDef = TypedDict(
+    "_OptionalPropertyValueOutputTypeDef",
+    {
+        "timestamp": datetime,
+        "time": str,
+    },
+    total=False,
+)
+
+class PropertyValueOutputTypeDef(
+    _RequiredPropertyValueOutputTypeDef, _OptionalPropertyValueOutputTypeDef
+):
+    pass
+
 _RequiredPropertyValueTypeDef = TypedDict(
     "_RequiredPropertyValueTypeDef",
     {
         "value": "DataValueTypeDef",
     },
 )
 _OptionalPropertyValueTypeDef = TypedDict(
@@ -992,23 +1067,52 @@
         "definition": PropertyDefinitionRequestTypeDef,
         "value": "DataValueTypeDef",
         "updateType": PropertyUpdateTypeType,
     },
     total=False,
 )
 
+DataConnectorOutputTypeDef = TypedDict(
+    "DataConnectorOutputTypeDef",
+    {
+        "lambda": LambdaFunctionOutputTypeDef,
+        "isNative": bool,
+    },
+    total=False,
+)
+
 DataConnectorTypeDef = TypedDict(
     "DataConnectorTypeDef",
     {
         "lambda": LambdaFunctionTypeDef,
         "isNative": bool,
     },
     total=False,
 )
 
+_RequiredDataTypeOutputTypeDef = TypedDict(
+    "_RequiredDataTypeOutputTypeDef",
+    {
+        "type": TypeType,
+    },
+)
+_OptionalDataTypeOutputTypeDef = TypedDict(
+    "_OptionalDataTypeOutputTypeDef",
+    {
+        "nestedType": Dict[str, Any],
+        "allowedValues": List["DataValueOutputTypeDef"],
+        "unitOfMeasure": str,
+        "relationship": RelationshipOutputTypeDef,
+    },
+    total=False,
+)
+
+class DataTypeOutputTypeDef(_RequiredDataTypeOutputTypeDef, _OptionalDataTypeOutputTypeDef):
+    pass
+
 _RequiredDataTypeTypeDef = TypedDict(
     "_RequiredDataTypeTypeDef",
     {
         "type": TypeType,
     },
 )
 _OptionalDataTypeTypeDef = TypedDict(
@@ -1021,14 +1125,30 @@
     },
     total=False,
 )
 
 class DataTypeTypeDef(_RequiredDataTypeTypeDef, _OptionalDataTypeTypeDef):
     pass
 
+DataValueOutputTypeDef = TypedDict(
+    "DataValueOutputTypeDef",
+    {
+        "booleanValue": bool,
+        "doubleValue": float,
+        "integerValue": int,
+        "longValue": int,
+        "stringValue": str,
+        "listValue": List[Dict[str, Any]],
+        "mapValue": Dict[str, Dict[str, Any]],
+        "relationshipValue": RelationshipValueOutputTypeDef,
+        "expression": str,
+    },
+    total=False,
+)
+
 DataValueTypeDef = TypedDict(
     "DataValueTypeDef",
     {
         "booleanValue": bool,
         "doubleValue": float,
         "integerValue": int,
         "longValue": int,
@@ -1040,21 +1160,21 @@
     },
     total=False,
 )
 
 _RequiredPropertyLatestValueTypeDef = TypedDict(
     "_RequiredPropertyLatestValueTypeDef",
     {
-        "propertyReference": EntityPropertyReferenceTypeDef,
+        "propertyReference": EntityPropertyReferenceOutputTypeDef,
     },
 )
 _OptionalPropertyLatestValueTypeDef = TypedDict(
     "_OptionalPropertyLatestValueTypeDef",
     {
-        "propertyValue": "DataValueTypeDef",
+        "propertyValue": "DataValueOutputTypeDef",
     },
     total=False,
 )
 
 class PropertyLatestValueTypeDef(
     _RequiredPropertyLatestValueTypeDef, _OptionalPropertyLatestValueTypeDef
 ):
@@ -1097,15 +1217,15 @@
     },
 )
 
 PropertyResponseTypeDef = TypedDict(
     "PropertyResponseTypeDef",
     {
         "definition": PropertyDefinitionResponseTypeDef,
-        "value": "DataValueTypeDef",
+        "value": "DataValueOutputTypeDef",
     },
     total=False,
 )
 
 _RequiredGetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetPropertyValueHistoryRequestRequestTypeDef",
     {
@@ -1244,52 +1364,71 @@
     {
         "orderBy": Sequence[OrderByTypeDef],
         "propertyFilters": Sequence[PropertyFilterTypeDef],
     },
     total=False,
 )
 
-_RequiredPropertyValueEntryTypeDef = TypedDict(
-    "_RequiredPropertyValueEntryTypeDef",
+_RequiredPropertyValueEntryOutputTypeDef = TypedDict(
+    "_RequiredPropertyValueEntryOutputTypeDef",
     {
-        "entityPropertyReference": EntityPropertyReferenceTypeDef,
+        "entityPropertyReference": EntityPropertyReferenceOutputTypeDef,
     },
 )
-_OptionalPropertyValueEntryTypeDef = TypedDict(
-    "_OptionalPropertyValueEntryTypeDef",
+_OptionalPropertyValueEntryOutputTypeDef = TypedDict(
+    "_OptionalPropertyValueEntryOutputTypeDef",
     {
-        "propertyValues": Sequence[PropertyValueTypeDef],
+        "propertyValues": List[PropertyValueOutputTypeDef],
     },
     total=False,
 )
 
-class PropertyValueEntryTypeDef(
-    _RequiredPropertyValueEntryTypeDef, _OptionalPropertyValueEntryTypeDef
+class PropertyValueEntryOutputTypeDef(
+    _RequiredPropertyValueEntryOutputTypeDef, _OptionalPropertyValueEntryOutputTypeDef
 ):
     pass
 
 _RequiredPropertyValueHistoryTypeDef = TypedDict(
     "_RequiredPropertyValueHistoryTypeDef",
     {
-        "entityPropertyReference": EntityPropertyReferenceTypeDef,
+        "entityPropertyReference": EntityPropertyReferenceOutputTypeDef,
     },
 )
 _OptionalPropertyValueHistoryTypeDef = TypedDict(
     "_OptionalPropertyValueHistoryTypeDef",
     {
-        "values": List[PropertyValueTypeDef],
+        "values": List[PropertyValueOutputTypeDef],
     },
     total=False,
 )
 
 class PropertyValueHistoryTypeDef(
     _RequiredPropertyValueHistoryTypeDef, _OptionalPropertyValueHistoryTypeDef
 ):
     pass
 
+_RequiredPropertyValueEntryTypeDef = TypedDict(
+    "_RequiredPropertyValueEntryTypeDef",
+    {
+        "entityPropertyReference": EntityPropertyReferenceTypeDef,
+    },
+)
+_OptionalPropertyValueEntryTypeDef = TypedDict(
+    "_OptionalPropertyValueEntryTypeDef",
+    {
+        "propertyValues": Sequence[PropertyValueTypeDef],
+    },
+    total=False,
+)
+
+class PropertyValueEntryTypeDef(
+    _RequiredPropertyValueEntryTypeDef, _OptionalPropertyValueEntryTypeDef
+):
+    pass
+
 GetPricingPlanResponseTypeDef = TypedDict(
     "GetPricingPlanResponseTypeDef",
     {
         "currentPricingPlan": PricingPlanTypeDef,
         "pendingPricingPlan": PricingPlanTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1323,41 +1462,41 @@
         "componentTypeId": str,
         "propertyUpdates": Mapping[str, PropertyRequestTypeDef],
         "propertyGroupUpdates": Mapping[str, ComponentPropertyGroupRequestTypeDef],
     },
     total=False,
 )
 
-FunctionRequestTypeDef = TypedDict(
-    "FunctionRequestTypeDef",
+FunctionResponseTypeDef = TypedDict(
+    "FunctionResponseTypeDef",
     {
-        "requiredProperties": Sequence[str],
+        "requiredProperties": List[str],
         "scope": ScopeType,
-        "implementedBy": DataConnectorTypeDef,
+        "implementedBy": DataConnectorOutputTypeDef,
+        "isInherited": bool,
     },
     total=False,
 )
 
-FunctionResponseTypeDef = TypedDict(
-    "FunctionResponseTypeDef",
+FunctionRequestTypeDef = TypedDict(
+    "FunctionRequestTypeDef",
     {
-        "requiredProperties": List[str],
+        "requiredProperties": Sequence[str],
         "scope": ScopeType,
         "implementedBy": DataConnectorTypeDef,
-        "isInherited": bool,
     },
     total=False,
 )
 
 GetPropertyValueResponseTypeDef = TypedDict(
     "GetPropertyValueResponseTypeDef",
     {
         "propertyValues": Dict[str, PropertyLatestValueTypeDef],
         "nextToken": str,
-        "tabularPropertyValues": List[List[Dict[str, "DataValueTypeDef"]]],
+        "tabularPropertyValues": List[List[Dict[str, "DataValueOutputTypeDef"]]],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredComponentTypeSummaryTypeDef = TypedDict(
     "_RequiredComponentTypeSummaryTypeDef",
     {
@@ -1487,35 +1626,35 @@
     pass
 
 BatchPutPropertyErrorTypeDef = TypedDict(
     "BatchPutPropertyErrorTypeDef",
     {
         "errorCode": str,
         "errorMessage": str,
-        "entry": PropertyValueEntryTypeDef,
-    },
-)
-
-BatchPutPropertyValuesRequestRequestTypeDef = TypedDict(
-    "BatchPutPropertyValuesRequestRequestTypeDef",
-    {
-        "workspaceId": str,
-        "entries": Sequence[PropertyValueEntryTypeDef],
+        "entry": PropertyValueEntryOutputTypeDef,
     },
 )
 
 GetPropertyValueHistoryResponseTypeDef = TypedDict(
     "GetPropertyValueHistoryResponseTypeDef",
     {
         "propertyValues": List[PropertyValueHistoryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+BatchPutPropertyValuesRequestRequestTypeDef = TypedDict(
+    "BatchPutPropertyValuesRequestRequestTypeDef",
+    {
+        "workspaceId": str,
+        "entries": Sequence[PropertyValueEntryTypeDef],
+    },
+)
+
 _RequiredCreateEntityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEntityRequestRequestTypeDef",
     {
         "workspaceId": str,
         "entityName": str,
     },
 )
@@ -1555,14 +1694,37 @@
 )
 
 class UpdateEntityRequestRequestTypeDef(
     _RequiredUpdateEntityRequestRequestTypeDef, _OptionalUpdateEntityRequestRequestTypeDef
 ):
     pass
 
+GetComponentTypeResponseTypeDef = TypedDict(
+    "GetComponentTypeResponseTypeDef",
+    {
+        "workspaceId": str,
+        "isSingleton": bool,
+        "componentTypeId": str,
+        "description": str,
+        "propertyDefinitions": Dict[str, PropertyDefinitionResponseTypeDef],
+        "extendsFrom": List[str],
+        "functions": Dict[str, FunctionResponseTypeDef],
+        "creationDateTime": datetime,
+        "updateDateTime": datetime,
+        "arn": str,
+        "isAbstract": bool,
+        "isSchemaInitialized": bool,
+        "status": StatusTypeDef,
+        "propertyGroups": Dict[str, PropertyGroupResponseTypeDef],
+        "syncSource": str,
+        "componentTypeName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateComponentTypeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateComponentTypeRequestRequestTypeDef",
     {
         "workspaceId": str,
         "componentTypeId": str,
     },
 )
@@ -1610,37 +1772,14 @@
 
 class UpdateComponentTypeRequestRequestTypeDef(
     _RequiredUpdateComponentTypeRequestRequestTypeDef,
     _OptionalUpdateComponentTypeRequestRequestTypeDef,
 ):
     pass
 
-GetComponentTypeResponseTypeDef = TypedDict(
-    "GetComponentTypeResponseTypeDef",
-    {
-        "workspaceId": str,
-        "isSingleton": bool,
-        "componentTypeId": str,
-        "description": str,
-        "propertyDefinitions": Dict[str, PropertyDefinitionResponseTypeDef],
-        "extendsFrom": List[str],
-        "functions": Dict[str, FunctionResponseTypeDef],
-        "creationDateTime": datetime,
-        "updateDateTime": datetime,
-        "arn": str,
-        "isAbstract": bool,
-        "isSchemaInitialized": bool,
-        "status": StatusTypeDef,
-        "propertyGroups": Dict[str, PropertyGroupResponseTypeDef],
-        "syncSource": str,
-        "componentTypeName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListComponentTypesResponseTypeDef = TypedDict(
     "ListComponentTypesResponseTypeDef",
     {
         "workspaceId": str,
         "componentTypeSummaries": List[ComponentTypeSummaryTypeDef],
         "nextToken": str,
         "maxResults": int,
```

### Comparing `mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker.egg-info/PKG-INFO` & `mypy-boto3-iottwinmaker-1.28.12/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-iottwinmaker
-Version: 1.28.0
-Summary: Type annotations for boto3.IoTTwinMaker 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iottwinmaker type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-iottwinmaker"></a>
 
 # mypy-boto3-iottwinmaker
 
 [![PyPI - mypy-boto3-iottwinmaker](https://img.shields.io/pypi/v/mypy-boto3-iottwinmaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-iottwinmaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iottwinmaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-iottwinmaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iottwinmaker?color=blue)](https://pypistats.org/packages/mypy-boto3-iottwinmaker)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iottwinmaker)](https://pepy.tech/project/mypy-boto3-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTTwinMaker 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
+[boto3.IoTTwinMaker 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
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
 [mypy-boto3-iottwinmaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,25 +298,29 @@
     CreateEntityResponseTypeDef,
     CreateSceneRequestRequestTypeDef,
     CreateSceneResponseTypeDef,
     CreateSyncJobRequestRequestTypeDef,
     CreateSyncJobResponseTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
     CreateWorkspaceResponseTypeDef,
+    LambdaFunctionOutputTypeDef,
     LambdaFunctionTypeDef,
+    RelationshipOutputTypeDef,
     RelationshipTypeDef,
+    RelationshipValueOutputTypeDef,
     RelationshipValueTypeDef,
     DeleteComponentTypeRequestRequestTypeDef,
     DeleteComponentTypeResponseTypeDef,
     DeleteEntityRequestRequestTypeDef,
     DeleteEntityResponseTypeDef,
     DeleteSceneRequestRequestTypeDef,
     DeleteSyncJobRequestRequestTypeDef,
     DeleteSyncJobResponseTypeDef,
     DeleteWorkspaceRequestRequestTypeDef,
+    EntityPropertyReferenceOutputTypeDef,
     EntityPropertyReferenceTypeDef,
     ErrorDetailsTypeDef,
     ExecuteQueryRequestRequestTypeDef,
     RowTypeDef,
     GetComponentTypeRequestRequestTypeDef,
     PropertyDefinitionResponseTypeDef,
     PropertyGroupResponseTypeDef,
@@ -368,29 +340,33 @@
     SyncResourceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkspacesRequestRequestTypeDef,
     WorkspaceSummaryTypeDef,
     OrderByTypeDef,
     ParentEntityUpdateRequestTypeDef,
+    PropertyValueOutputTypeDef,
     PropertyValueTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateComponentTypeResponseTypeDef,
     UpdateEntityResponseTypeDef,
     UpdatePricingPlanRequestRequestTypeDef,
     UpdateSceneRequestRequestTypeDef,
     UpdateSceneResponseTypeDef,
     UpdateWorkspaceRequestRequestTypeDef,
     UpdateWorkspaceResponseTypeDef,
     PricingPlanTypeDef,
     PropertyRequestTypeDef,
+    DataConnectorOutputTypeDef,
     DataConnectorTypeDef,
+    DataTypeOutputTypeDef,
     DataTypeTypeDef,
+    DataValueOutputTypeDef,
     DataValueTypeDef,
     PropertyLatestValueTypeDef,
     StatusTypeDef,
     SyncJobStatusTypeDef,
     SyncResourceStatusTypeDef,
     ExecuteQueryResponseTypeDef,
     PropertyResponseTypeDef,
@@ -398,38 +374,39 @@
     GetSceneResponseTypeDef,
     ListComponentTypesRequestRequestTypeDef,
     ListEntitiesRequestRequestTypeDef,
     ListScenesResponseTypeDef,
     ListSyncResourcesRequestRequestTypeDef,
     ListWorkspacesResponseTypeDef,
     TabularConditionsTypeDef,
-    PropertyValueEntryTypeDef,
+    PropertyValueEntryOutputTypeDef,
     PropertyValueHistoryTypeDef,
+    PropertyValueEntryTypeDef,
     GetPricingPlanResponseTypeDef,
     UpdatePricingPlanResponseTypeDef,
     ComponentRequestTypeDef,
     ComponentUpdateRequestTypeDef,
-    FunctionRequestTypeDef,
     FunctionResponseTypeDef,
+    FunctionRequestTypeDef,
     GetPropertyValueResponseTypeDef,
     ComponentTypeSummaryTypeDef,
     EntitySummaryTypeDef,
     GetSyncJobResponseTypeDef,
     SyncJobSummaryTypeDef,
     SyncResourceSummaryTypeDef,
     ComponentResponseTypeDef,
     GetPropertyValueRequestRequestTypeDef,
     BatchPutPropertyErrorTypeDef,
-    BatchPutPropertyValuesRequestRequestTypeDef,
     GetPropertyValueHistoryResponseTypeDef,
+    BatchPutPropertyValuesRequestRequestTypeDef,
     CreateEntityRequestRequestTypeDef,
     UpdateEntityRequestRequestTypeDef,
+    GetComponentTypeResponseTypeDef,
     CreateComponentTypeRequestRequestTypeDef,
     UpdateComponentTypeRequestRequestTypeDef,
-    GetComponentTypeResponseTypeDef,
     ListComponentTypesResponseTypeDef,
     ListEntitiesResponseTypeDef,
     ListSyncJobsResponseTypeDef,
     ListSyncResourcesResponseTypeDef,
     GetEntityResponseTypeDef,
     BatchPutPropertyErrorEntryTypeDef,
     BatchPutPropertyValuesResponseTypeDef,
```

### Comparing `mypy-boto3-iottwinmaker-1.28.0/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt` & `mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.28.0/setup.py` & `mypy-boto3-iottwinmaker-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iottwinmaker",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_iottwinmaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTTwinMaker 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.IoTTwinMaker 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

