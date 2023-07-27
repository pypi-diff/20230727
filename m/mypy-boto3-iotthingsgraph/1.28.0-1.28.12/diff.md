# Comparing `tmp/mypy-boto3-iotthingsgraph-1.28.0.tar.gz` & `tmp/mypy-boto3-iotthingsgraph-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotthingsgraph-1.28.0.tar", last modified: Thu Jul  6 20:59:50 2023, max compression
+gzip compressed data, was "mypy-boto3-iotthingsgraph-1.28.12.tar", last modified: Thu Jul 27 05:34:51 2023, max compression
```

## Comparing `mypy-boto3-iotthingsgraph-1.28.0.tar` & `mypy-boto3-iotthingsgraph-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:50.858336 mypy-boto3-iotthingsgraph-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:44:05.000000 mypy-boto3-iotthingsgraph-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18922 2023-07-06 20:59:50.850336 mypy-boto3-iotthingsgraph-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17409 2023-07-06 20:44:05.000000 mypy-boto3-iotthingsgraph-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:50.846336 mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-06 20:44:05.000000 mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-06 20:44:05.000000 mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 20:44:05.000000 mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29250 2023-07-06 20:44:05.000000 mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29198 2023-07-06 20:44:05.000000 mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-07-06 20:44:05.000000 mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-07-06 20:44:05.000000 mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-07-06 20:44:05.000000 mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13084 2023-07-06 20:44:05.000000 mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:44:05.000000 mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33757 2023-07-06 20:44:06.000000 mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33710 2023-07-06 20:44:06.000000 mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:44:05.000000 mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:50.850336 mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18922 2023-07-06 20:59:50.000000 mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 20:59:50.000000 mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:50.000000 mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:50.000000 mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:50.000000 mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 20:59:50.000000 mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:50.858336 mypy-boto3-iotthingsgraph-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-06 20:44:04.000000 mypy-boto3-iotthingsgraph-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.068477 mypy-boto3-iotthingsgraph-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19007 2023-07-27 05:34:51.068477 mypy-boto3-iotthingsgraph-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17492 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.056477 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29250 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29198 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11270 2023-07-27 05:24:15.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-07-27 05:24:15.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-07-27 05:24:15.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13084 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34361 2023-07-27 05:24:15.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34314 2023-07-27 05:24:15.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.068477 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19007 2023-07-27 05:34:50.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 05:34:50.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:50.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:50.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:50.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:34:50.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:51.068477 mypy-boto3-iotthingsgraph-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/setup.py
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.0/LICENSE` & `mypy-boto3-iotthingsgraph-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.0/PKG-INFO` & `mypy-boto3-iotthingsgraph-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotthingsgraph
-Version: 1.28.0
-Summary: Type annotations for boto3.IoTThingsGraph 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTThingsGraph 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iotthingsgraph"></a>
 
 # mypy-boto3-iotthingsgraph
 
 [![PyPI - mypy-boto3-iotthingsgraph](https://img.shields.io/pypi/v/mypy-boto3-iotthingsgraph.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotthingsgraph)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotthingsgraph.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotthingsgraph)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotthingsgraph?color=blue)](https://pypistats.org/packages/mypy-boto3-iotthingsgraph)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotthingsgraph)](https://pepy.tech/project/mypy-boto3-iotthingsgraph)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTThingsGraph 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
+[boto3.IoTThingsGraph 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
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
 [mypy-boto3-iotthingsgraph docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/).
 
 See how it helps to find and fix potential bugs:
 
@@ -385,14 +385,15 @@
     AssociateEntityToThingRequestRequestTypeDef,
     DefinitionDocumentTypeDef,
     FlowTemplateSummaryTypeDef,
     MetricsConfigurationTypeDef,
     TagTypeDef,
     SystemInstanceSummaryTypeDef,
     SystemTemplateSummaryTypeDef,
+    DefinitionDocumentOutputTypeDef,
     DeleteFlowTemplateRequestRequestTypeDef,
     DeleteNamespaceResponseTypeDef,
     DeleteSystemInstanceRequestRequestTypeDef,
     DeleteSystemTemplateRequestRequestTypeDef,
     DependencyRevisionTypeDef,
     DeploySystemInstanceRequestRequestTypeDef,
     DeprecateFlowTemplateRequestRequestTypeDef,
@@ -415,56 +416,58 @@
     GetSystemTemplateRevisionsRequestRequestTypeDef,
     GetUploadStatusRequestRequestTypeDef,
     GetUploadStatusResponseTypeDef,
     ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
     ListFlowExecutionMessagesRequestRequestTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    MetricsConfigurationOutputTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     SearchFlowExecutionsRequestRequestTypeDef,
     SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
     SearchThingsRequestRequestTypeDef,
     SearchThingsRequestSearchThingsPaginateTypeDef,
     ThingTypeDef,
     UndeploySystemInstanceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UploadEntityDefinitionsResponseTypeDef,
     CreateFlowTemplateRequestRequestTypeDef,
     CreateSystemTemplateRequestRequestTypeDef,
-    EntityDescriptionTypeDef,
     UpdateFlowTemplateRequestRequestTypeDef,
     UpdateSystemTemplateRequestRequestTypeDef,
     UploadEntityDefinitionsRequestRequestTypeDef,
     CreateFlowTemplateResponseTypeDef,
-    FlowTemplateDescriptionTypeDef,
     GetFlowTemplateRevisionsResponseTypeDef,
     SearchFlowTemplatesResponseTypeDef,
     UpdateFlowTemplateResponseTypeDef,
     CreateSystemInstanceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSystemInstanceResponseTypeDef,
     DeploySystemInstanceResponseTypeDef,
     SearchSystemInstancesResponseTypeDef,
     UndeploySystemInstanceResponseTypeDef,
     CreateSystemTemplateResponseTypeDef,
     GetSystemTemplateRevisionsResponseTypeDef,
     SearchSystemTemplatesResponseTypeDef,
-    SystemTemplateDescriptionTypeDef,
     UpdateSystemTemplateResponseTypeDef,
-    SystemInstanceDescriptionTypeDef,
+    EntityDescriptionTypeDef,
+    FlowTemplateDescriptionTypeDef,
+    SystemTemplateDescriptionTypeDef,
     SearchEntitiesRequestRequestTypeDef,
     SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     ListFlowExecutionMessagesResponseTypeDef,
     SearchFlowExecutionsResponseTypeDef,
     SearchFlowTemplatesRequestRequestTypeDef,
     SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SystemInstanceDescriptionTypeDef,
     SearchSystemInstancesRequestRequestTypeDef,
     SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef,
     SearchSystemTemplatesRequestRequestTypeDef,
     SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef,
     SearchThingsResponseTypeDef,
     GetEntitiesResponseTypeDef,
     SearchEntitiesResponseTypeDef,
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.0/README.md` & `mypy-boto3-iotthingsgraph-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iotthingsgraph"></a>
 
 # mypy-boto3-iotthingsgraph
 
 [![PyPI - mypy-boto3-iotthingsgraph](https://img.shields.io/pypi/v/mypy-boto3-iotthingsgraph.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotthingsgraph)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotthingsgraph.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotthingsgraph)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotthingsgraph?color=blue)](https://pypistats.org/packages/mypy-boto3-iotthingsgraph)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotthingsgraph)](https://pepy.tech/project/mypy-boto3-iotthingsgraph)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTThingsGraph 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
+[boto3.IoTThingsGraph 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
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
 [mypy-boto3-iotthingsgraph docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,14 +353,15 @@
     AssociateEntityToThingRequestRequestTypeDef,
     DefinitionDocumentTypeDef,
     FlowTemplateSummaryTypeDef,
     MetricsConfigurationTypeDef,
     TagTypeDef,
     SystemInstanceSummaryTypeDef,
     SystemTemplateSummaryTypeDef,
+    DefinitionDocumentOutputTypeDef,
     DeleteFlowTemplateRequestRequestTypeDef,
     DeleteNamespaceResponseTypeDef,
     DeleteSystemInstanceRequestRequestTypeDef,
     DeleteSystemTemplateRequestRequestTypeDef,
     DependencyRevisionTypeDef,
     DeploySystemInstanceRequestRequestTypeDef,
     DeprecateFlowTemplateRequestRequestTypeDef,
@@ -383,56 +384,58 @@
     GetSystemTemplateRevisionsRequestRequestTypeDef,
     GetUploadStatusRequestRequestTypeDef,
     GetUploadStatusResponseTypeDef,
     ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
     ListFlowExecutionMessagesRequestRequestTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    MetricsConfigurationOutputTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     SearchFlowExecutionsRequestRequestTypeDef,
     SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
     SearchThingsRequestRequestTypeDef,
     SearchThingsRequestSearchThingsPaginateTypeDef,
     ThingTypeDef,
     UndeploySystemInstanceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UploadEntityDefinitionsResponseTypeDef,
     CreateFlowTemplateRequestRequestTypeDef,
     CreateSystemTemplateRequestRequestTypeDef,
-    EntityDescriptionTypeDef,
     UpdateFlowTemplateRequestRequestTypeDef,
     UpdateSystemTemplateRequestRequestTypeDef,
     UploadEntityDefinitionsRequestRequestTypeDef,
     CreateFlowTemplateResponseTypeDef,
-    FlowTemplateDescriptionTypeDef,
     GetFlowTemplateRevisionsResponseTypeDef,
     SearchFlowTemplatesResponseTypeDef,
     UpdateFlowTemplateResponseTypeDef,
     CreateSystemInstanceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSystemInstanceResponseTypeDef,
     DeploySystemInstanceResponseTypeDef,
     SearchSystemInstancesResponseTypeDef,
     UndeploySystemInstanceResponseTypeDef,
     CreateSystemTemplateResponseTypeDef,
     GetSystemTemplateRevisionsResponseTypeDef,
     SearchSystemTemplatesResponseTypeDef,
-    SystemTemplateDescriptionTypeDef,
     UpdateSystemTemplateResponseTypeDef,
-    SystemInstanceDescriptionTypeDef,
+    EntityDescriptionTypeDef,
+    FlowTemplateDescriptionTypeDef,
+    SystemTemplateDescriptionTypeDef,
     SearchEntitiesRequestRequestTypeDef,
     SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     ListFlowExecutionMessagesResponseTypeDef,
     SearchFlowExecutionsResponseTypeDef,
     SearchFlowTemplatesRequestRequestTypeDef,
     SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SystemInstanceDescriptionTypeDef,
     SearchSystemInstancesRequestRequestTypeDef,
     SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef,
     SearchSystemTemplatesRequestRequestTypeDef,
     SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef,
     SearchThingsResponseTypeDef,
     GetEntitiesResponseTypeDef,
     SearchEntitiesResponseTypeDef,
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/__init__.py` & `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/__init__.pyi` & `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/__main__.py` & `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTThingsGraph 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.IoTThingsGraph 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph\nOther"
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

### Comparing `mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/client.py` & `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/client.pyi` & `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/literals.py` & `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DefinitionLanguageType",
     "DeploymentTargetType",
     "EntityFilterNameType",
     "EntityTypeType",
     "FlowExecutionEventTypeType",
     "FlowExecutionStatusType",
@@ -46,15 +45,14 @@
     "IoTThingsGraphServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DefinitionLanguageType = Literal["GRAPHQL"]
 DeploymentTargetType = Literal["CLOUD", "GREENGRASS"]
 EntityFilterNameType = Literal["NAME", "NAMESPACE", "REFERENCED_ENTITY_ID", "SEMANTIC_TYPE_PATH"]
 EntityTypeType = Literal[
     "ACTION",
     "CAPABILITY",
     "DEVICE",
@@ -228,14 +226,15 @@
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
@@ -314,26 +313,28 @@
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

### Comparing `mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/literals.pyi` & `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/literals.py`

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
     "DefinitionLanguageType",
     "DeploymentTargetType",
     "EntityFilterNameType",
     "EntityTypeType",
     "FlowExecutionEventTypeType",
     "FlowExecutionStatusType",
@@ -45,14 +46,15 @@
     "IoTThingsGraphServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 DefinitionLanguageType = Literal["GRAPHQL"]
 DeploymentTargetType = Literal["CLOUD", "GREENGRASS"]
 EntityFilterNameType = Literal["NAME", "NAMESPACE", "REFERENCED_ENTITY_ID", "SEMANTIC_TYPE_PATH"]
 EntityTypeType = Literal[
     "ACTION",
     "CAPABILITY",
     "DEVICE",
@@ -226,14 +228,15 @@
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
@@ -312,26 +315,28 @@
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

### Comparing `mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/paginator.py` & `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/paginator.pyi` & `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/type_defs.py` & `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -32,23 +32,23 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateEntityToThingRequestRequestTypeDef",
     "DefinitionDocumentTypeDef",
     "FlowTemplateSummaryTypeDef",
     "MetricsConfigurationTypeDef",
     "TagTypeDef",
     "SystemInstanceSummaryTypeDef",
     "SystemTemplateSummaryTypeDef",
+    "DefinitionDocumentOutputTypeDef",
     "DeleteFlowTemplateRequestRequestTypeDef",
     "DeleteNamespaceResponseTypeDef",
     "DeleteSystemInstanceRequestRequestTypeDef",
     "DeleteSystemTemplateRequestRequestTypeDef",
     "DependencyRevisionTypeDef",
     "DeploySystemInstanceRequestRequestTypeDef",
     "DeprecateFlowTemplateRequestRequestTypeDef",
@@ -71,56 +71,58 @@
     "GetSystemTemplateRevisionsRequestRequestTypeDef",
     "GetUploadStatusRequestRequestTypeDef",
     "GetUploadStatusResponseTypeDef",
     "ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
     "ListFlowExecutionMessagesRequestRequestTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "MetricsConfigurationOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "SearchFlowExecutionsRequestRequestTypeDef",
     "SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     "SystemInstanceFilterTypeDef",
     "SystemTemplateFilterTypeDef",
     "SearchThingsRequestRequestTypeDef",
     "SearchThingsRequestSearchThingsPaginateTypeDef",
     "ThingTypeDef",
     "UndeploySystemInstanceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UploadEntityDefinitionsResponseTypeDef",
     "CreateFlowTemplateRequestRequestTypeDef",
     "CreateSystemTemplateRequestRequestTypeDef",
-    "EntityDescriptionTypeDef",
     "UpdateFlowTemplateRequestRequestTypeDef",
     "UpdateSystemTemplateRequestRequestTypeDef",
     "UploadEntityDefinitionsRequestRequestTypeDef",
     "CreateFlowTemplateResponseTypeDef",
-    "FlowTemplateDescriptionTypeDef",
     "GetFlowTemplateRevisionsResponseTypeDef",
     "SearchFlowTemplatesResponseTypeDef",
     "UpdateFlowTemplateResponseTypeDef",
     "CreateSystemInstanceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSystemInstanceResponseTypeDef",
     "DeploySystemInstanceResponseTypeDef",
     "SearchSystemInstancesResponseTypeDef",
     "UndeploySystemInstanceResponseTypeDef",
     "CreateSystemTemplateResponseTypeDef",
     "GetSystemTemplateRevisionsResponseTypeDef",
     "SearchSystemTemplatesResponseTypeDef",
-    "SystemTemplateDescriptionTypeDef",
     "UpdateSystemTemplateResponseTypeDef",
-    "SystemInstanceDescriptionTypeDef",
+    "EntityDescriptionTypeDef",
+    "FlowTemplateDescriptionTypeDef",
+    "SystemTemplateDescriptionTypeDef",
     "SearchEntitiesRequestRequestTypeDef",
     "SearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     "ListFlowExecutionMessagesResponseTypeDef",
     "SearchFlowExecutionsResponseTypeDef",
     "SearchFlowTemplatesRequestRequestTypeDef",
     "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "SystemInstanceDescriptionTypeDef",
     "SearchSystemInstancesRequestRequestTypeDef",
     "SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef",
     "SearchSystemTemplatesRequestRequestTypeDef",
     "SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef",
     "SearchThingsResponseTypeDef",
     "GetEntitiesResponseTypeDef",
     "SearchEntitiesResponseTypeDef",
@@ -140,22 +142,20 @@
     "_OptionalAssociateEntityToThingRequestRequestTypeDef",
     {
         "namespaceVersion": int,
     },
     total=False,
 )
 
-
 class AssociateEntityToThingRequestRequestTypeDef(
     _RequiredAssociateEntityToThingRequestRequestTypeDef,
     _OptionalAssociateEntityToThingRequestRequestTypeDef,
 ):
     pass
 
-
 DefinitionDocumentTypeDef = TypedDict(
     "DefinitionDocumentTypeDef",
     {
         "language": Literal["GRAPHQL"],
         "text": str,
     },
 )
@@ -211,14 +211,22 @@
         "arn": str,
         "revisionNumber": int,
         "createdAt": datetime,
     },
     total=False,
 )
 
+DefinitionDocumentOutputTypeDef = TypedDict(
+    "DefinitionDocumentOutputTypeDef",
+    {
+        "language": Literal["GRAPHQL"],
+        "text": str,
+    },
+)
+
 DeleteFlowTemplateRequestRequestTypeDef = TypedDict(
     "DeleteFlowTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -356,64 +364,58 @@
     "_OptionalGetEntitiesRequestRequestTypeDef",
     {
         "namespaceVersion": int,
     },
     total=False,
 )
 
-
 class GetEntitiesRequestRequestTypeDef(
     _RequiredGetEntitiesRequestRequestTypeDef, _OptionalGetEntitiesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetFlowTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredGetFlowTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetFlowTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalGetFlowTemplateRequestRequestTypeDef",
     {
         "revisionNumber": int,
     },
     total=False,
 )
 
-
 class GetFlowTemplateRequestRequestTypeDef(
     _RequiredGetFlowTemplateRequestRequestTypeDef, _OptionalGetFlowTemplateRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
     "_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
     "_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef(
     _RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
     _OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetFlowTemplateRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFlowTemplateRevisionsRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetFlowTemplateRevisionsRequestRequestTypeDef = TypedDict(
@@ -421,22 +423,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetFlowTemplateRevisionsRequestRequestTypeDef(
     _RequiredGetFlowTemplateRevisionsRequestRequestTypeDef,
     _OptionalGetFlowTemplateRevisionsRequestRequestTypeDef,
 ):
     pass
 
-
 GetNamespaceDeletionStatusResponseTypeDef = TypedDict(
     "GetNamespaceDeletionStatusResponseTypeDef",
     {
         "namespaceArn": str,
         "namespaceName": str,
         "status": NamespaceDeletionStatusType,
         "errorCode": Literal["VALIDATION_FAILED"],
@@ -462,43 +462,39 @@
     "_OptionalGetSystemTemplateRequestRequestTypeDef",
     {
         "revisionNumber": int,
     },
     total=False,
 )
 
-
 class GetSystemTemplateRequestRequestTypeDef(
     _RequiredGetSystemTemplateRequestRequestTypeDef, _OptionalGetSystemTemplateRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
     "_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
     "_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef(
     _RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
     _OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetSystemTemplateRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSystemTemplateRevisionsRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetSystemTemplateRevisionsRequestRequestTypeDef = TypedDict(
@@ -506,22 +502,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetSystemTemplateRevisionsRequestRequestTypeDef(
     _RequiredGetSystemTemplateRevisionsRequestRequestTypeDef,
     _OptionalGetSystemTemplateRevisionsRequestRequestTypeDef,
 ):
     pass
 
-
 GetUploadStatusRequestRequestTypeDef = TypedDict(
     "GetUploadStatusRequestRequestTypeDef",
     {
         "uploadId": str,
     },
 )
 
@@ -549,22 +543,20 @@
     "_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef(
     _RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
     _OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListFlowExecutionMessagesRequestRequestTypeDef = TypedDict(
     "_RequiredListFlowExecutionMessagesRequestRequestTypeDef",
     {
         "flowExecutionId": str,
     },
 )
 _OptionalListFlowExecutionMessagesRequestRequestTypeDef = TypedDict(
@@ -572,44 +564,40 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListFlowExecutionMessagesRequestRequestTypeDef(
     _RequiredListFlowExecutionMessagesRequestRequestTypeDef,
     _OptionalListFlowExecutionMessagesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
     "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -617,21 +605,36 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
+MetricsConfigurationOutputTypeDef = TypedDict(
+    "MetricsConfigurationOutputTypeDef",
+    {
+        "cloudMetricEnabled": bool,
+        "metricRuleRoleArn": str,
+    },
+    total=False,
+)
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
@@ -664,22 +667,20 @@
         "endTime": Union[datetime, str],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class SearchFlowExecutionsRequestRequestTypeDef(
     _RequiredSearchFlowExecutionsRequestRequestTypeDef,
     _OptionalSearchFlowExecutionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
     "_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     {
         "systemInstanceId": str,
     },
 )
 _OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
@@ -689,22 +690,20 @@
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef(
     _RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     _OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
 ):
     pass
 
-
 SystemInstanceFilterTypeDef = TypedDict(
     "SystemInstanceFilterTypeDef",
     {
         "name": SystemInstanceFilterNameType,
         "value": Sequence[str],
     },
     total=False,
@@ -730,21 +729,19 @@
         "nextToken": str,
         "maxResults": int,
         "namespaceVersion": int,
     },
     total=False,
 )
 
-
 class SearchThingsRequestRequestTypeDef(
     _RequiredSearchThingsRequestRequestTypeDef, _OptionalSearchThingsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
     "_RequiredSearchThingsRequestSearchThingsPaginateTypeDef",
     {
         "entityId": str,
     },
 )
 _OptionalSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
@@ -752,22 +749,20 @@
     {
         "namespaceVersion": int,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchThingsRequestSearchThingsPaginateTypeDef(
     _RequiredSearchThingsRequestSearchThingsPaginateTypeDef,
     _OptionalSearchThingsRequestSearchThingsPaginateTypeDef,
 ):
     pass
 
-
 ThingTypeDef = TypedDict(
     "ThingTypeDef",
     {
         "thingArn": str,
         "thingName": str,
     },
     total=False,
@@ -807,56 +802,40 @@
     "_OptionalCreateFlowTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
-
 class CreateFlowTemplateRequestRequestTypeDef(
     _RequiredCreateFlowTemplateRequestRequestTypeDef,
     _OptionalCreateFlowTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateSystemTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSystemTemplateRequestRequestTypeDef",
     {
         "definition": DefinitionDocumentTypeDef,
     },
 )
 _OptionalCreateSystemTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSystemTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
-
 class CreateSystemTemplateRequestRequestTypeDef(
     _RequiredCreateSystemTemplateRequestRequestTypeDef,
     _OptionalCreateSystemTemplateRequestRequestTypeDef,
 ):
     pass
 
-
-EntityDescriptionTypeDef = TypedDict(
-    "EntityDescriptionTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "type": EntityTypeType,
-        "createdAt": datetime,
-        "definition": DefinitionDocumentTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateFlowTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowTemplateRequestRequestTypeDef",
     {
         "id": str,
         "definition": DefinitionDocumentTypeDef,
     },
 )
@@ -864,22 +843,20 @@
     "_OptionalUpdateFlowTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
-
 class UpdateFlowTemplateRequestRequestTypeDef(
     _RequiredUpdateFlowTemplateRequestRequestTypeDef,
     _OptionalUpdateFlowTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateSystemTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSystemTemplateRequestRequestTypeDef",
     {
         "id": str,
         "definition": DefinitionDocumentTypeDef,
     },
 )
@@ -887,22 +864,20 @@
     "_OptionalUpdateSystemTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
-
 class UpdateSystemTemplateRequestRequestTypeDef(
     _RequiredUpdateSystemTemplateRequestRequestTypeDef,
     _OptionalUpdateSystemTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 UploadEntityDefinitionsRequestRequestTypeDef = TypedDict(
     "UploadEntityDefinitionsRequestRequestTypeDef",
     {
         "document": DefinitionDocumentTypeDef,
         "syncWithPublicNamespace": bool,
         "deprecateExistingEntities": bool,
     },
@@ -913,24 +888,14 @@
     "CreateFlowTemplateResponseTypeDef",
     {
         "summary": FlowTemplateSummaryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-FlowTemplateDescriptionTypeDef = TypedDict(
-    "FlowTemplateDescriptionTypeDef",
-    {
-        "summary": FlowTemplateSummaryTypeDef,
-        "definition": DefinitionDocumentTypeDef,
-        "validatedNamespaceVersion": int,
-    },
-    total=False,
-)
-
 GetFlowTemplateRevisionsResponseTypeDef = TypedDict(
     "GetFlowTemplateRevisionsResponseTypeDef",
     {
         "summaries": List[FlowTemplateSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -968,31 +933,20 @@
         "s3BucketName": str,
         "metricsConfiguration": MetricsConfigurationTypeDef,
         "flowActionsRoleArn": str,
     },
     total=False,
 )
 
-
 class CreateSystemInstanceRequestRequestTypeDef(
     _RequiredCreateSystemInstanceRequestRequestTypeDef,
     _OptionalCreateSystemInstanceRequestRequestTypeDef,
 ):
     pass
 
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "nextToken": str,
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
@@ -1053,42 +1007,50 @@
     {
         "summaries": List[SystemTemplateSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SystemTemplateDescriptionTypeDef = TypedDict(
-    "SystemTemplateDescriptionTypeDef",
+UpdateSystemTemplateResponseTypeDef = TypedDict(
+    "UpdateSystemTemplateResponseTypeDef",
     {
         "summary": SystemTemplateSummaryTypeDef,
-        "definition": DefinitionDocumentTypeDef,
-        "validatedNamespaceVersion": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EntityDescriptionTypeDef = TypedDict(
+    "EntityDescriptionTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "type": EntityTypeType,
+        "createdAt": datetime,
+        "definition": DefinitionDocumentOutputTypeDef,
     },
     total=False,
 )
 
-UpdateSystemTemplateResponseTypeDef = TypedDict(
-    "UpdateSystemTemplateResponseTypeDef",
+FlowTemplateDescriptionTypeDef = TypedDict(
+    "FlowTemplateDescriptionTypeDef",
     {
-        "summary": SystemTemplateSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "summary": FlowTemplateSummaryTypeDef,
+        "definition": DefinitionDocumentOutputTypeDef,
+        "validatedNamespaceVersion": int,
     },
+    total=False,
 )
 
-SystemInstanceDescriptionTypeDef = TypedDict(
-    "SystemInstanceDescriptionTypeDef",
+SystemTemplateDescriptionTypeDef = TypedDict(
+    "SystemTemplateDescriptionTypeDef",
     {
-        "summary": SystemInstanceSummaryTypeDef,
-        "definition": DefinitionDocumentTypeDef,
-        "s3BucketName": str,
-        "metricsConfiguration": MetricsConfigurationTypeDef,
+        "summary": SystemTemplateSummaryTypeDef,
+        "definition": DefinitionDocumentOutputTypeDef,
         "validatedNamespaceVersion": int,
-        "validatedDependencyRevisions": List[DependencyRevisionTypeDef],
-        "flowActionsRoleArn": str,
     },
     total=False,
 )
 
 _RequiredSearchEntitiesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchEntitiesRequestRequestTypeDef",
     {
@@ -1102,21 +1064,19 @@
         "nextToken": str,
         "maxResults": int,
         "namespaceVersion": int,
     },
     total=False,
 )
 
-
 class SearchEntitiesRequestRequestTypeDef(
     _RequiredSearchEntitiesRequestRequestTypeDef, _OptionalSearchEntitiesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef = TypedDict(
     "_RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     {
         "entityTypes": Sequence[EntityTypeType],
     },
 )
 _OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef = TypedDict(
@@ -1125,22 +1085,20 @@
         "filters": Sequence[EntityFilterTypeDef],
         "namespaceVersion": int,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchEntitiesRequestSearchEntitiesPaginateTypeDef(
     _RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     _OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef,
 ):
     pass
 
-
 ListFlowExecutionMessagesResponseTypeDef = TypedDict(
     "ListFlowExecutionMessagesResponseTypeDef",
     {
         "messages": List[FlowExecutionMessageTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1170,14 +1128,37 @@
     {
         "filters": Sequence[FlowTemplateFilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+SystemInstanceDescriptionTypeDef = TypedDict(
+    "SystemInstanceDescriptionTypeDef",
+    {
+        "summary": SystemInstanceSummaryTypeDef,
+        "definition": DefinitionDocumentOutputTypeDef,
+        "s3BucketName": str,
+        "metricsConfiguration": MetricsConfigurationOutputTypeDef,
+        "validatedNamespaceVersion": int,
+        "validatedDependencyRevisions": List[DependencyRevisionTypeDef],
+        "flowActionsRoleArn": str,
+    },
+    total=False,
+)
+
 SearchSystemInstancesRequestRequestTypeDef = TypedDict(
     "SearchSystemInstancesRequestRequestTypeDef",
     {
         "filters": Sequence[SystemInstanceFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph/type_defs.pyi` & `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,22 +32,24 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssociateEntityToThingRequestRequestTypeDef",
     "DefinitionDocumentTypeDef",
     "FlowTemplateSummaryTypeDef",
     "MetricsConfigurationTypeDef",
     "TagTypeDef",
     "SystemInstanceSummaryTypeDef",
     "SystemTemplateSummaryTypeDef",
+    "DefinitionDocumentOutputTypeDef",
     "DeleteFlowTemplateRequestRequestTypeDef",
     "DeleteNamespaceResponseTypeDef",
     "DeleteSystemInstanceRequestRequestTypeDef",
     "DeleteSystemTemplateRequestRequestTypeDef",
     "DependencyRevisionTypeDef",
     "DeploySystemInstanceRequestRequestTypeDef",
     "DeprecateFlowTemplateRequestRequestTypeDef",
@@ -70,56 +72,58 @@
     "GetSystemTemplateRevisionsRequestRequestTypeDef",
     "GetUploadStatusRequestRequestTypeDef",
     "GetUploadStatusResponseTypeDef",
     "ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
     "ListFlowExecutionMessagesRequestRequestTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "MetricsConfigurationOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "SearchFlowExecutionsRequestRequestTypeDef",
     "SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     "SystemInstanceFilterTypeDef",
     "SystemTemplateFilterTypeDef",
     "SearchThingsRequestRequestTypeDef",
     "SearchThingsRequestSearchThingsPaginateTypeDef",
     "ThingTypeDef",
     "UndeploySystemInstanceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UploadEntityDefinitionsResponseTypeDef",
     "CreateFlowTemplateRequestRequestTypeDef",
     "CreateSystemTemplateRequestRequestTypeDef",
-    "EntityDescriptionTypeDef",
     "UpdateFlowTemplateRequestRequestTypeDef",
     "UpdateSystemTemplateRequestRequestTypeDef",
     "UploadEntityDefinitionsRequestRequestTypeDef",
     "CreateFlowTemplateResponseTypeDef",
-    "FlowTemplateDescriptionTypeDef",
     "GetFlowTemplateRevisionsResponseTypeDef",
     "SearchFlowTemplatesResponseTypeDef",
     "UpdateFlowTemplateResponseTypeDef",
     "CreateSystemInstanceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSystemInstanceResponseTypeDef",
     "DeploySystemInstanceResponseTypeDef",
     "SearchSystemInstancesResponseTypeDef",
     "UndeploySystemInstanceResponseTypeDef",
     "CreateSystemTemplateResponseTypeDef",
     "GetSystemTemplateRevisionsResponseTypeDef",
     "SearchSystemTemplatesResponseTypeDef",
-    "SystemTemplateDescriptionTypeDef",
     "UpdateSystemTemplateResponseTypeDef",
-    "SystemInstanceDescriptionTypeDef",
+    "EntityDescriptionTypeDef",
+    "FlowTemplateDescriptionTypeDef",
+    "SystemTemplateDescriptionTypeDef",
     "SearchEntitiesRequestRequestTypeDef",
     "SearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     "ListFlowExecutionMessagesResponseTypeDef",
     "SearchFlowExecutionsResponseTypeDef",
     "SearchFlowTemplatesRequestRequestTypeDef",
     "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "SystemInstanceDescriptionTypeDef",
     "SearchSystemInstancesRequestRequestTypeDef",
     "SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef",
     "SearchSystemTemplatesRequestRequestTypeDef",
     "SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef",
     "SearchThingsResponseTypeDef",
     "GetEntitiesResponseTypeDef",
     "SearchEntitiesResponseTypeDef",
@@ -139,20 +143,22 @@
     "_OptionalAssociateEntityToThingRequestRequestTypeDef",
     {
         "namespaceVersion": int,
     },
     total=False,
 )
 
+
 class AssociateEntityToThingRequestRequestTypeDef(
     _RequiredAssociateEntityToThingRequestRequestTypeDef,
     _OptionalAssociateEntityToThingRequestRequestTypeDef,
 ):
     pass
 
+
 DefinitionDocumentTypeDef = TypedDict(
     "DefinitionDocumentTypeDef",
     {
         "language": Literal["GRAPHQL"],
         "text": str,
     },
 )
@@ -208,14 +214,22 @@
         "arn": str,
         "revisionNumber": int,
         "createdAt": datetime,
     },
     total=False,
 )
 
+DefinitionDocumentOutputTypeDef = TypedDict(
+    "DefinitionDocumentOutputTypeDef",
+    {
+        "language": Literal["GRAPHQL"],
+        "text": str,
+    },
+)
+
 DeleteFlowTemplateRequestRequestTypeDef = TypedDict(
     "DeleteFlowTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -353,58 +367,64 @@
     "_OptionalGetEntitiesRequestRequestTypeDef",
     {
         "namespaceVersion": int,
     },
     total=False,
 )
 
+
 class GetEntitiesRequestRequestTypeDef(
     _RequiredGetEntitiesRequestRequestTypeDef, _OptionalGetEntitiesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetFlowTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredGetFlowTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetFlowTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalGetFlowTemplateRequestRequestTypeDef",
     {
         "revisionNumber": int,
     },
     total=False,
 )
 
+
 class GetFlowTemplateRequestRequestTypeDef(
     _RequiredGetFlowTemplateRequestRequestTypeDef, _OptionalGetFlowTemplateRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
     "_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
     "_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef(
     _RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
     _OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetFlowTemplateRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFlowTemplateRevisionsRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetFlowTemplateRevisionsRequestRequestTypeDef = TypedDict(
@@ -412,20 +432,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetFlowTemplateRevisionsRequestRequestTypeDef(
     _RequiredGetFlowTemplateRevisionsRequestRequestTypeDef,
     _OptionalGetFlowTemplateRevisionsRequestRequestTypeDef,
 ):
     pass
 
+
 GetNamespaceDeletionStatusResponseTypeDef = TypedDict(
     "GetNamespaceDeletionStatusResponseTypeDef",
     {
         "namespaceArn": str,
         "namespaceName": str,
         "status": NamespaceDeletionStatusType,
         "errorCode": Literal["VALIDATION_FAILED"],
@@ -451,39 +473,43 @@
     "_OptionalGetSystemTemplateRequestRequestTypeDef",
     {
         "revisionNumber": int,
     },
     total=False,
 )
 
+
 class GetSystemTemplateRequestRequestTypeDef(
     _RequiredGetSystemTemplateRequestRequestTypeDef, _OptionalGetSystemTemplateRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
     "_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
     "_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef(
     _RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
     _OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetSystemTemplateRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSystemTemplateRevisionsRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetSystemTemplateRevisionsRequestRequestTypeDef = TypedDict(
@@ -491,20 +517,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetSystemTemplateRevisionsRequestRequestTypeDef(
     _RequiredGetSystemTemplateRevisionsRequestRequestTypeDef,
     _OptionalGetSystemTemplateRevisionsRequestRequestTypeDef,
 ):
     pass
 
+
 GetUploadStatusRequestRequestTypeDef = TypedDict(
     "GetUploadStatusRequestRequestTypeDef",
     {
         "uploadId": str,
     },
 )
 
@@ -532,20 +560,22 @@
     "_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef(
     _RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
     _OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListFlowExecutionMessagesRequestRequestTypeDef = TypedDict(
     "_RequiredListFlowExecutionMessagesRequestRequestTypeDef",
     {
         "flowExecutionId": str,
     },
 )
 _OptionalListFlowExecutionMessagesRequestRequestTypeDef = TypedDict(
@@ -553,40 +583,44 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListFlowExecutionMessagesRequestRequestTypeDef(
     _RequiredListFlowExecutionMessagesRequestRequestTypeDef,
     _OptionalListFlowExecutionMessagesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
     "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -594,20 +628,39 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
+MetricsConfigurationOutputTypeDef = TypedDict(
+    "MetricsConfigurationOutputTypeDef",
+    {
+        "cloudMetricEnabled": bool,
+        "metricRuleRoleArn": str,
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
@@ -639,20 +692,22 @@
         "endTime": Union[datetime, str],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class SearchFlowExecutionsRequestRequestTypeDef(
     _RequiredSearchFlowExecutionsRequestRequestTypeDef,
     _OptionalSearchFlowExecutionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
     "_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     {
         "systemInstanceId": str,
     },
 )
 _OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
@@ -662,20 +717,22 @@
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef(
     _RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     _OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
 ):
     pass
 
+
 SystemInstanceFilterTypeDef = TypedDict(
     "SystemInstanceFilterTypeDef",
     {
         "name": SystemInstanceFilterNameType,
         "value": Sequence[str],
     },
     total=False,
@@ -701,19 +758,21 @@
         "nextToken": str,
         "maxResults": int,
         "namespaceVersion": int,
     },
     total=False,
 )
 
+
 class SearchThingsRequestRequestTypeDef(
     _RequiredSearchThingsRequestRequestTypeDef, _OptionalSearchThingsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
     "_RequiredSearchThingsRequestSearchThingsPaginateTypeDef",
     {
         "entityId": str,
     },
 )
 _OptionalSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
@@ -721,20 +780,22 @@
     {
         "namespaceVersion": int,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchThingsRequestSearchThingsPaginateTypeDef(
     _RequiredSearchThingsRequestSearchThingsPaginateTypeDef,
     _OptionalSearchThingsRequestSearchThingsPaginateTypeDef,
 ):
     pass
 
+
 ThingTypeDef = TypedDict(
     "ThingTypeDef",
     {
         "thingArn": str,
         "thingName": str,
     },
     total=False,
@@ -774,51 +835,43 @@
     "_OptionalCreateFlowTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
+
 class CreateFlowTemplateRequestRequestTypeDef(
     _RequiredCreateFlowTemplateRequestRequestTypeDef,
     _OptionalCreateFlowTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateSystemTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSystemTemplateRequestRequestTypeDef",
     {
         "definition": DefinitionDocumentTypeDef,
     },
 )
 _OptionalCreateSystemTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSystemTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
+
 class CreateSystemTemplateRequestRequestTypeDef(
     _RequiredCreateSystemTemplateRequestRequestTypeDef,
     _OptionalCreateSystemTemplateRequestRequestTypeDef,
 ):
     pass
 
-EntityDescriptionTypeDef = TypedDict(
-    "EntityDescriptionTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "type": EntityTypeType,
-        "createdAt": datetime,
-        "definition": DefinitionDocumentTypeDef,
-    },
-    total=False,
-)
 
 _RequiredUpdateFlowTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowTemplateRequestRequestTypeDef",
     {
         "id": str,
         "definition": DefinitionDocumentTypeDef,
     },
@@ -827,20 +880,22 @@
     "_OptionalUpdateFlowTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
+
 class UpdateFlowTemplateRequestRequestTypeDef(
     _RequiredUpdateFlowTemplateRequestRequestTypeDef,
     _OptionalUpdateFlowTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateSystemTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSystemTemplateRequestRequestTypeDef",
     {
         "id": str,
         "definition": DefinitionDocumentTypeDef,
     },
 )
@@ -848,20 +903,22 @@
     "_OptionalUpdateSystemTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
+
 class UpdateSystemTemplateRequestRequestTypeDef(
     _RequiredUpdateSystemTemplateRequestRequestTypeDef,
     _OptionalUpdateSystemTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 UploadEntityDefinitionsRequestRequestTypeDef = TypedDict(
     "UploadEntityDefinitionsRequestRequestTypeDef",
     {
         "document": DefinitionDocumentTypeDef,
         "syncWithPublicNamespace": bool,
         "deprecateExistingEntities": bool,
     },
@@ -872,24 +929,14 @@
     "CreateFlowTemplateResponseTypeDef",
     {
         "summary": FlowTemplateSummaryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-FlowTemplateDescriptionTypeDef = TypedDict(
-    "FlowTemplateDescriptionTypeDef",
-    {
-        "summary": FlowTemplateSummaryTypeDef,
-        "definition": DefinitionDocumentTypeDef,
-        "validatedNamespaceVersion": int,
-    },
-    total=False,
-)
-
 GetFlowTemplateRevisionsResponseTypeDef = TypedDict(
     "GetFlowTemplateRevisionsResponseTypeDef",
     {
         "summaries": List[FlowTemplateSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -927,28 +974,21 @@
         "s3BucketName": str,
         "metricsConfiguration": MetricsConfigurationTypeDef,
         "flowActionsRoleArn": str,
     },
     total=False,
 )
 
+
 class CreateSystemInstanceRequestRequestTypeDef(
     _RequiredCreateSystemInstanceRequestRequestTypeDef,
     _OptionalCreateSystemInstanceRequestRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
@@ -1010,42 +1050,50 @@
     {
         "summaries": List[SystemTemplateSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SystemTemplateDescriptionTypeDef = TypedDict(
-    "SystemTemplateDescriptionTypeDef",
+UpdateSystemTemplateResponseTypeDef = TypedDict(
+    "UpdateSystemTemplateResponseTypeDef",
     {
         "summary": SystemTemplateSummaryTypeDef,
-        "definition": DefinitionDocumentTypeDef,
-        "validatedNamespaceVersion": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EntityDescriptionTypeDef = TypedDict(
+    "EntityDescriptionTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "type": EntityTypeType,
+        "createdAt": datetime,
+        "definition": DefinitionDocumentOutputTypeDef,
     },
     total=False,
 )
 
-UpdateSystemTemplateResponseTypeDef = TypedDict(
-    "UpdateSystemTemplateResponseTypeDef",
+FlowTemplateDescriptionTypeDef = TypedDict(
+    "FlowTemplateDescriptionTypeDef",
     {
-        "summary": SystemTemplateSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "summary": FlowTemplateSummaryTypeDef,
+        "definition": DefinitionDocumentOutputTypeDef,
+        "validatedNamespaceVersion": int,
     },
+    total=False,
 )
 
-SystemInstanceDescriptionTypeDef = TypedDict(
-    "SystemInstanceDescriptionTypeDef",
+SystemTemplateDescriptionTypeDef = TypedDict(
+    "SystemTemplateDescriptionTypeDef",
     {
-        "summary": SystemInstanceSummaryTypeDef,
-        "definition": DefinitionDocumentTypeDef,
-        "s3BucketName": str,
-        "metricsConfiguration": MetricsConfigurationTypeDef,
+        "summary": SystemTemplateSummaryTypeDef,
+        "definition": DefinitionDocumentOutputTypeDef,
         "validatedNamespaceVersion": int,
-        "validatedDependencyRevisions": List[DependencyRevisionTypeDef],
-        "flowActionsRoleArn": str,
     },
     total=False,
 )
 
 _RequiredSearchEntitiesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchEntitiesRequestRequestTypeDef",
     {
@@ -1059,19 +1107,21 @@
         "nextToken": str,
         "maxResults": int,
         "namespaceVersion": int,
     },
     total=False,
 )
 
+
 class SearchEntitiesRequestRequestTypeDef(
     _RequiredSearchEntitiesRequestRequestTypeDef, _OptionalSearchEntitiesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef = TypedDict(
     "_RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     {
         "entityTypes": Sequence[EntityTypeType],
     },
 )
 _OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef = TypedDict(
@@ -1080,20 +1130,22 @@
         "filters": Sequence[EntityFilterTypeDef],
         "namespaceVersion": int,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchEntitiesRequestSearchEntitiesPaginateTypeDef(
     _RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     _OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef,
 ):
     pass
 
+
 ListFlowExecutionMessagesResponseTypeDef = TypedDict(
     "ListFlowExecutionMessagesResponseTypeDef",
     {
         "messages": List[FlowExecutionMessageTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1123,14 +1175,37 @@
     {
         "filters": Sequence[FlowTemplateFilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+SystemInstanceDescriptionTypeDef = TypedDict(
+    "SystemInstanceDescriptionTypeDef",
+    {
+        "summary": SystemInstanceSummaryTypeDef,
+        "definition": DefinitionDocumentOutputTypeDef,
+        "s3BucketName": str,
+        "metricsConfiguration": MetricsConfigurationOutputTypeDef,
+        "validatedNamespaceVersion": int,
+        "validatedDependencyRevisions": List[DependencyRevisionTypeDef],
+        "flowActionsRoleArn": str,
+    },
+    total=False,
+)
+
 SearchSystemInstancesRequestRequestTypeDef = TypedDict(
     "SearchSystemInstancesRequestRequestTypeDef",
     {
         "filters": Sequence[SystemInstanceFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph.egg-info/PKG-INFO` & `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotthingsgraph
-Version: 1.28.0
-Summary: Type annotations for boto3.IoTThingsGraph 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTThingsGraph 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iotthingsgraph"></a>
 
 # mypy-boto3-iotthingsgraph
 
 [![PyPI - mypy-boto3-iotthingsgraph](https://img.shields.io/pypi/v/mypy-boto3-iotthingsgraph.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotthingsgraph)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotthingsgraph.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotthingsgraph)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotthingsgraph?color=blue)](https://pypistats.org/packages/mypy-boto3-iotthingsgraph)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotthingsgraph)](https://pepy.tech/project/mypy-boto3-iotthingsgraph)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTThingsGraph 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
+[boto3.IoTThingsGraph 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
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
 [mypy-boto3-iotthingsgraph docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/).
 
 See how it helps to find and fix potential bugs:
 
@@ -385,14 +385,15 @@
     AssociateEntityToThingRequestRequestTypeDef,
     DefinitionDocumentTypeDef,
     FlowTemplateSummaryTypeDef,
     MetricsConfigurationTypeDef,
     TagTypeDef,
     SystemInstanceSummaryTypeDef,
     SystemTemplateSummaryTypeDef,
+    DefinitionDocumentOutputTypeDef,
     DeleteFlowTemplateRequestRequestTypeDef,
     DeleteNamespaceResponseTypeDef,
     DeleteSystemInstanceRequestRequestTypeDef,
     DeleteSystemTemplateRequestRequestTypeDef,
     DependencyRevisionTypeDef,
     DeploySystemInstanceRequestRequestTypeDef,
     DeprecateFlowTemplateRequestRequestTypeDef,
@@ -415,56 +416,58 @@
     GetSystemTemplateRevisionsRequestRequestTypeDef,
     GetUploadStatusRequestRequestTypeDef,
     GetUploadStatusResponseTypeDef,
     ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
     ListFlowExecutionMessagesRequestRequestTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    MetricsConfigurationOutputTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     SearchFlowExecutionsRequestRequestTypeDef,
     SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
     SearchThingsRequestRequestTypeDef,
     SearchThingsRequestSearchThingsPaginateTypeDef,
     ThingTypeDef,
     UndeploySystemInstanceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UploadEntityDefinitionsResponseTypeDef,
     CreateFlowTemplateRequestRequestTypeDef,
     CreateSystemTemplateRequestRequestTypeDef,
-    EntityDescriptionTypeDef,
     UpdateFlowTemplateRequestRequestTypeDef,
     UpdateSystemTemplateRequestRequestTypeDef,
     UploadEntityDefinitionsRequestRequestTypeDef,
     CreateFlowTemplateResponseTypeDef,
-    FlowTemplateDescriptionTypeDef,
     GetFlowTemplateRevisionsResponseTypeDef,
     SearchFlowTemplatesResponseTypeDef,
     UpdateFlowTemplateResponseTypeDef,
     CreateSystemInstanceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSystemInstanceResponseTypeDef,
     DeploySystemInstanceResponseTypeDef,
     SearchSystemInstancesResponseTypeDef,
     UndeploySystemInstanceResponseTypeDef,
     CreateSystemTemplateResponseTypeDef,
     GetSystemTemplateRevisionsResponseTypeDef,
     SearchSystemTemplatesResponseTypeDef,
-    SystemTemplateDescriptionTypeDef,
     UpdateSystemTemplateResponseTypeDef,
-    SystemInstanceDescriptionTypeDef,
+    EntityDescriptionTypeDef,
+    FlowTemplateDescriptionTypeDef,
+    SystemTemplateDescriptionTypeDef,
     SearchEntitiesRequestRequestTypeDef,
     SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     ListFlowExecutionMessagesResponseTypeDef,
     SearchFlowExecutionsResponseTypeDef,
     SearchFlowTemplatesRequestRequestTypeDef,
     SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SystemInstanceDescriptionTypeDef,
     SearchSystemInstancesRequestRequestTypeDef,
     SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef,
     SearchSystemTemplatesRequestRequestTypeDef,
     SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef,
     SearchThingsResponseTypeDef,
     GetEntitiesResponseTypeDef,
     SearchEntitiesResponseTypeDef,
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.0/mypy_boto3_iotthingsgraph.egg-info/SOURCES.txt` & `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.0/setup.py` & `mypy-boto3-iotthingsgraph-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotthingsgraph",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_iotthingsgraph"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTThingsGraph 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.IoTThingsGraph 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

