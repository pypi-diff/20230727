# Comparing `tmp/mypy-boto3-migrationhuborchestrator-1.28.0.tar.gz` & `tmp/mypy-boto3-migrationhuborchestrator-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-migrationhuborchestrator-1.28.0.tar", last modified: Thu Jul  6 21:00:09 2023, max compression
+gzip compressed data, was "mypy-boto3-migrationhuborchestrator-1.28.12.tar", last modified: Thu Jul 27 05:35:03 2023, max compression
```

## Comparing `mypy-boto3-migrationhuborchestrator-1.28.0.tar` & `mypy-boto3-migrationhuborchestrator-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:09.518374 mypy-boto3-migrationhuborchestrator-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:47:48.000000 mypy-boto3-migrationhuborchestrator-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-07-06 21:00:09.518374 mypy-boto3-migrationhuborchestrator-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-07-06 20:47:48.000000 mypy-boto3-migrationhuborchestrator-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:09.518374 mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-06 20:47:48.000000 mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-06 20:47:48.000000 mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-06 20:47:48.000000 mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25168 2023-07-06 20:47:48.000000 mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-07-06 20:47:48.000000 mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-07-06 20:47:48.000000 mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-07-06 20:47:48.000000 mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9380 2023-07-06 20:47:48.000000 mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-07-06 20:47:48.000000 mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:47:48.000000 mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31882 2023-07-06 20:47:49.000000 mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31854 2023-07-06 20:47:49.000000 mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:47:48.000000 mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:09.518374 mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-07-06 21:00:09.000000 mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-06 21:00:09.000000 mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:09.000000 mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:09.000000 mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:09.000000 mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 21:00:09.000000 mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:09.518374 mypy-boto3-migrationhuborchestrator-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-06 20:47:47.000000 mypy-boto3-migrationhuborchestrator-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:03.860431 mypy-boto3-migrationhuborchestrator-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18188 2023-07-27 05:35:03.860431 mypy-boto3-migrationhuborchestrator-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16633 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:03.852431 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25168 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9380 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33023 2023-07-27 05:26:42.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32995 2023-07-27 05:26:42.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:03.860431 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18188 2023-07-27 05:35:03.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-27 05:35:03.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:03.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:03.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:03.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-27 05:35:03.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:03.860431 mypy-boto3-migrationhuborchestrator-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/setup.py
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.0/LICENSE` & `mypy-boto3-migrationhuborchestrator-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.0/PKG-INFO` & `mypy-boto3-migrationhuborchestrator-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhuborchestrator
-Version: 1.28.0
-Summary: Type annotations for boto3.MigrationHubOrchestrator 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MigrationHubOrchestrator 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-migrationhuborchestrator"></a>
 
 # mypy-boto3-migrationhuborchestrator
 
 [![PyPI - mypy-boto3-migrationhuborchestrator](https://img.shields.io/pypi/v/mypy-boto3-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhuborchestrator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhuborchestrator)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migrationhuborchestrator?color=blue)](https://pypistats.org/packages/mypy-boto3-migrationhuborchestrator)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhuborchestrator)](https://pepy.tech/project/mypy-boto3-migrationhuborchestrator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubOrchestrator 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
+[boto3.MigrationHubOrchestrator 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
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
 [mypy-boto3-migrationhuborchestrator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/).
 
 See how it helps to find and fix potential bugs:
 
@@ -359,14 +359,15 @@
 
 `mypy_boto3_migrationhuborchestrator.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migrationhuborchestrator.type_defs import (
     StepInputTypeDef,
+    StepInputOutputTypeDef,
     CreateWorkflowStepGroupRequestRequestTypeDef,
     ToolTypeDef,
     CreateWorkflowStepResponseTypeDef,
     DeleteMigrationWorkflowRequestRequestTypeDef,
     DeleteMigrationWorkflowResponseTypeDef,
     DeleteWorkflowStepGroupRequestRequestTypeDef,
     DeleteWorkflowStepRequestRequestTypeDef,
@@ -398,31 +399,33 @@
     ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
     ListWorkflowStepGroupsRequestRequestTypeDef,
     WorkflowStepGroupSummaryTypeDef,
     ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
     ListWorkflowStepsRequestRequestTypeDef,
     WorkflowStepSummaryTypeDef,
     PaginatorConfigTypeDef,
+    PlatformCommandOutputTypeDef,
     PlatformCommandTypeDef,
+    PlatformScriptKeyOutputTypeDef,
     PlatformScriptKeyTypeDef,
     ResponseMetadataTypeDef,
     RetryWorkflowStepRequestRequestTypeDef,
     RetryWorkflowStepResponseTypeDef,
     StartMigrationWorkflowRequestRequestTypeDef,
     StartMigrationWorkflowResponseTypeDef,
     StopMigrationWorkflowRequestRequestTypeDef,
     StopMigrationWorkflowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWorkflowStepGroupRequestRequestTypeDef,
     UpdateWorkflowStepResponseTypeDef,
     WorkflowStepOutputUnionTypeDef,
     CreateMigrationWorkflowRequestRequestTypeDef,
-    CreateMigrationWorkflowResponseTypeDef,
     UpdateMigrationWorkflowRequestRequestTypeDef,
+    CreateMigrationWorkflowResponseTypeDef,
     UpdateMigrationWorkflowResponseTypeDef,
     CreateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowResponseTypeDef,
     GetTemplateStepGroupResponseTypeDef,
     GetWorkflowStepGroupResponseTypeDef,
     UpdateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowTemplateResponseTypeDef,
@@ -430,14 +433,15 @@
     ListMigrationWorkflowsResponseTypeDef,
     ListPluginsResponseTypeDef,
     ListTemplateStepGroupsResponseTypeDef,
     ListTemplateStepsResponseTypeDef,
     ListWorkflowStepGroupsResponseTypeDef,
     ListWorkflowStepsResponseTypeDef,
     StepAutomationConfigurationTypeDef,
+    WorkflowStepAutomationConfigurationOutputTypeDef,
     WorkflowStepAutomationConfigurationTypeDef,
     WorkflowStepOutputTypeDef,
     GetTemplateStepResponseTypeDef,
     CreateWorkflowStepRequestRequestTypeDef,
     GetWorkflowStepResponseTypeDef,
     UpdateWorkflowStepRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.0/README.md` & `mypy-boto3-migrationhuborchestrator-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-migrationhuborchestrator"></a>
 
 # mypy-boto3-migrationhuborchestrator
 
 [![PyPI - mypy-boto3-migrationhuborchestrator](https://img.shields.io/pypi/v/mypy-boto3-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhuborchestrator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhuborchestrator)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migrationhuborchestrator?color=blue)](https://pypistats.org/packages/mypy-boto3-migrationhuborchestrator)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhuborchestrator)](https://pepy.tech/project/mypy-boto3-migrationhuborchestrator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubOrchestrator 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
+[boto3.MigrationHubOrchestrator 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
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
 [mypy-boto3-migrationhuborchestrator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,14 +327,15 @@
 
 `mypy_boto3_migrationhuborchestrator.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migrationhuborchestrator.type_defs import (
     StepInputTypeDef,
+    StepInputOutputTypeDef,
     CreateWorkflowStepGroupRequestRequestTypeDef,
     ToolTypeDef,
     CreateWorkflowStepResponseTypeDef,
     DeleteMigrationWorkflowRequestRequestTypeDef,
     DeleteMigrationWorkflowResponseTypeDef,
     DeleteWorkflowStepGroupRequestRequestTypeDef,
     DeleteWorkflowStepRequestRequestTypeDef,
@@ -366,31 +367,33 @@
     ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
     ListWorkflowStepGroupsRequestRequestTypeDef,
     WorkflowStepGroupSummaryTypeDef,
     ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
     ListWorkflowStepsRequestRequestTypeDef,
     WorkflowStepSummaryTypeDef,
     PaginatorConfigTypeDef,
+    PlatformCommandOutputTypeDef,
     PlatformCommandTypeDef,
+    PlatformScriptKeyOutputTypeDef,
     PlatformScriptKeyTypeDef,
     ResponseMetadataTypeDef,
     RetryWorkflowStepRequestRequestTypeDef,
     RetryWorkflowStepResponseTypeDef,
     StartMigrationWorkflowRequestRequestTypeDef,
     StartMigrationWorkflowResponseTypeDef,
     StopMigrationWorkflowRequestRequestTypeDef,
     StopMigrationWorkflowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWorkflowStepGroupRequestRequestTypeDef,
     UpdateWorkflowStepResponseTypeDef,
     WorkflowStepOutputUnionTypeDef,
     CreateMigrationWorkflowRequestRequestTypeDef,
-    CreateMigrationWorkflowResponseTypeDef,
     UpdateMigrationWorkflowRequestRequestTypeDef,
+    CreateMigrationWorkflowResponseTypeDef,
     UpdateMigrationWorkflowResponseTypeDef,
     CreateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowResponseTypeDef,
     GetTemplateStepGroupResponseTypeDef,
     GetWorkflowStepGroupResponseTypeDef,
     UpdateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowTemplateResponseTypeDef,
@@ -398,14 +401,15 @@
     ListMigrationWorkflowsResponseTypeDef,
     ListPluginsResponseTypeDef,
     ListTemplateStepGroupsResponseTypeDef,
     ListTemplateStepsResponseTypeDef,
     ListWorkflowStepGroupsResponseTypeDef,
     ListWorkflowStepsResponseTypeDef,
     StepAutomationConfigurationTypeDef,
+    WorkflowStepAutomationConfigurationOutputTypeDef,
     WorkflowStepAutomationConfigurationTypeDef,
     WorkflowStepOutputTypeDef,
     GetTemplateStepResponseTypeDef,
     CreateWorkflowStepRequestRequestTypeDef,
     GetWorkflowStepResponseTypeDef,
     UpdateWorkflowStepRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/__init__.py` & `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/__init__.pyi` & `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/__main__.py` & `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MigrationHubOrchestrator 1.28.0\nVersion:        "
-        " 1.28.0\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.MigrationHubOrchestrator 1.28.12\nVersion:        "
+        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator\nOther"
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

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/client.py` & `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/client.pyi` & `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/literals.py` & `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,15 @@
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
@@ -296,26 +297,28 @@
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

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/literals.pyi` & `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -208,14 +208,15 @@
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
@@ -294,26 +295,28 @@
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

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/paginator.py` & `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/paginator.pyi` & `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/type_defs.py` & `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "StepInputTypeDef",
+    "StepInputOutputTypeDef",
     "CreateWorkflowStepGroupRequestRequestTypeDef",
     "ToolTypeDef",
     "CreateWorkflowStepResponseTypeDef",
     "DeleteMigrationWorkflowRequestRequestTypeDef",
     "DeleteMigrationWorkflowResponseTypeDef",
     "DeleteWorkflowStepGroupRequestRequestTypeDef",
     "DeleteWorkflowStepRequestRequestTypeDef",
@@ -74,31 +75,33 @@
     "ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
     "ListWorkflowStepGroupsRequestRequestTypeDef",
     "WorkflowStepGroupSummaryTypeDef",
     "ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
     "ListWorkflowStepsRequestRequestTypeDef",
     "WorkflowStepSummaryTypeDef",
     "PaginatorConfigTypeDef",
+    "PlatformCommandOutputTypeDef",
     "PlatformCommandTypeDef",
+    "PlatformScriptKeyOutputTypeDef",
     "PlatformScriptKeyTypeDef",
     "ResponseMetadataTypeDef",
     "RetryWorkflowStepRequestRequestTypeDef",
     "RetryWorkflowStepResponseTypeDef",
     "StartMigrationWorkflowRequestRequestTypeDef",
     "StartMigrationWorkflowResponseTypeDef",
     "StopMigrationWorkflowRequestRequestTypeDef",
     "StopMigrationWorkflowResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWorkflowStepGroupRequestRequestTypeDef",
     "UpdateWorkflowStepResponseTypeDef",
     "WorkflowStepOutputUnionTypeDef",
     "CreateMigrationWorkflowRequestRequestTypeDef",
-    "CreateMigrationWorkflowResponseTypeDef",
     "UpdateMigrationWorkflowRequestRequestTypeDef",
+    "CreateMigrationWorkflowResponseTypeDef",
     "UpdateMigrationWorkflowResponseTypeDef",
     "CreateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowResponseTypeDef",
     "GetTemplateStepGroupResponseTypeDef",
     "GetWorkflowStepGroupResponseTypeDef",
     "UpdateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowTemplateResponseTypeDef",
@@ -106,14 +109,15 @@
     "ListMigrationWorkflowsResponseTypeDef",
     "ListPluginsResponseTypeDef",
     "ListTemplateStepGroupsResponseTypeDef",
     "ListTemplateStepsResponseTypeDef",
     "ListWorkflowStepGroupsResponseTypeDef",
     "ListWorkflowStepsResponseTypeDef",
     "StepAutomationConfigurationTypeDef",
+    "WorkflowStepAutomationConfigurationOutputTypeDef",
     "WorkflowStepAutomationConfigurationTypeDef",
     "WorkflowStepOutputTypeDef",
     "GetTemplateStepResponseTypeDef",
     "CreateWorkflowStepRequestRequestTypeDef",
     "GetWorkflowStepResponseTypeDef",
     "UpdateWorkflowStepRequestRequestTypeDef",
 )
@@ -125,14 +129,25 @@
         "stringValue": str,
         "listOfStringsValue": Sequence[str],
         "mapOfStringValue": Mapping[str, str],
     },
     total=False,
 )
 
+StepInputOutputTypeDef = TypedDict(
+    "StepInputOutputTypeDef",
+    {
+        "integerValue": int,
+        "stringValue": str,
+        "listOfStringsValue": List[str],
+        "mapOfStringValue": Dict[str, str],
+    },
+    total=False,
+)
+
 _RequiredCreateWorkflowStepGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowStepGroupRequestRequestTypeDef",
     {
         "workflowId": str,
         "name": str,
     },
 )
@@ -641,23 +656,41 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+PlatformCommandOutputTypeDef = TypedDict(
+    "PlatformCommandOutputTypeDef",
+    {
+        "linux": str,
+        "windows": str,
+    },
+    total=False,
+)
+
 PlatformCommandTypeDef = TypedDict(
     "PlatformCommandTypeDef",
     {
         "linux": str,
         "windows": str,
     },
     total=False,
 )
 
+PlatformScriptKeyOutputTypeDef = TypedDict(
+    "PlatformScriptKeyOutputTypeDef",
+    {
+        "linux": str,
+        "windows": str,
+    },
+    total=False,
+)
+
 PlatformScriptKeyTypeDef = TypedDict(
     "PlatformScriptKeyTypeDef",
     {
         "linux": str,
         "windows": str,
     },
     total=False,
@@ -818,32 +851,14 @@
 class CreateMigrationWorkflowRequestRequestTypeDef(
     _RequiredCreateMigrationWorkflowRequestRequestTypeDef,
     _OptionalCreateMigrationWorkflowRequestRequestTypeDef,
 ):
     pass
 
 
-CreateMigrationWorkflowResponseTypeDef = TypedDict(
-    "CreateMigrationWorkflowResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "name": str,
-        "description": str,
-        "templateId": str,
-        "adsApplicationConfigurationId": str,
-        "workflowInputs": Dict[str, StepInputTypeDef],
-        "stepTargets": List[str],
-        "status": MigrationWorkflowStatusEnumType,
-        "creationTime": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
@@ -861,24 +876,42 @@
 class UpdateMigrationWorkflowRequestRequestTypeDef(
     _RequiredUpdateMigrationWorkflowRequestRequestTypeDef,
     _OptionalUpdateMigrationWorkflowRequestRequestTypeDef,
 ):
     pass
 
 
+CreateMigrationWorkflowResponseTypeDef = TypedDict(
+    "CreateMigrationWorkflowResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "description": str,
+        "templateId": str,
+        "adsApplicationConfigurationId": str,
+        "workflowInputs": Dict[str, StepInputOutputTypeDef],
+        "stepTargets": List[str],
+        "status": MigrationWorkflowStatusEnumType,
+        "creationTime": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateMigrationWorkflowResponseTypeDef = TypedDict(
     "UpdateMigrationWorkflowResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
         "templateId": str,
         "adsApplicationConfigurationId": str,
-        "workflowInputs": Dict[str, StepInputTypeDef],
+        "workflowInputs": Dict[str, StepInputOutputTypeDef],
         "stepTargets": List[str],
         "status": MigrationWorkflowStatusEnumType,
         "creationTime": datetime,
         "lastModifiedTime": datetime,
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -915,15 +948,15 @@
         "lastStartTime": datetime,
         "lastStopTime": datetime,
         "lastModifiedTime": datetime,
         "endTime": datetime,
         "tools": List[ToolTypeDef],
         "totalSteps": int,
         "completedSteps": int,
-        "workflowInputs": Dict[str, StepInputTypeDef],
+        "workflowInputs": Dict[str, StepInputOutputTypeDef],
         "tags": Dict[str, str],
         "workflowBucket": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTemplateStepGroupResponseTypeDef = TypedDict(
@@ -1054,16 +1087,28 @@
     },
 )
 
 StepAutomationConfigurationTypeDef = TypedDict(
     "StepAutomationConfigurationTypeDef",
     {
         "scriptLocationS3Bucket": str,
-        "scriptLocationS3Key": PlatformScriptKeyTypeDef,
-        "command": PlatformCommandTypeDef,
+        "scriptLocationS3Key": PlatformScriptKeyOutputTypeDef,
+        "command": PlatformCommandOutputTypeDef,
+        "runEnvironment": RunEnvironmentType,
+        "targetType": TargetTypeType,
+    },
+    total=False,
+)
+
+WorkflowStepAutomationConfigurationOutputTypeDef = TypedDict(
+    "WorkflowStepAutomationConfigurationOutputTypeDef",
+    {
+        "scriptLocationS3Bucket": str,
+        "scriptLocationS3Key": PlatformScriptKeyOutputTypeDef,
+        "command": PlatformCommandOutputTypeDef,
         "runEnvironment": RunEnvironmentType,
         "targetType": TargetTypeType,
     },
     total=False,
 )
 
 WorkflowStepAutomationConfigurationTypeDef = TypedDict(
@@ -1143,15 +1188,15 @@
         "name": str,
         "stepGroupId": str,
         "workflowId": str,
         "stepId": str,
         "description": str,
         "stepActionType": StepActionTypeType,
         "owner": OwnerType,
-        "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationTypeDef,
+        "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationOutputTypeDef,
         "stepTarget": List[str],
         "outputs": List[WorkflowStepOutputTypeDef],
         "previous": List[str],
         "next": List[str],
         "status": StepStatusType,
         "statusMessage": str,
         "scriptOutputLocation": str,
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator/type_defs.pyi` & `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "StepInputTypeDef",
+    "StepInputOutputTypeDef",
     "CreateWorkflowStepGroupRequestRequestTypeDef",
     "ToolTypeDef",
     "CreateWorkflowStepResponseTypeDef",
     "DeleteMigrationWorkflowRequestRequestTypeDef",
     "DeleteMigrationWorkflowResponseTypeDef",
     "DeleteWorkflowStepGroupRequestRequestTypeDef",
     "DeleteWorkflowStepRequestRequestTypeDef",
@@ -73,31 +74,33 @@
     "ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
     "ListWorkflowStepGroupsRequestRequestTypeDef",
     "WorkflowStepGroupSummaryTypeDef",
     "ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
     "ListWorkflowStepsRequestRequestTypeDef",
     "WorkflowStepSummaryTypeDef",
     "PaginatorConfigTypeDef",
+    "PlatformCommandOutputTypeDef",
     "PlatformCommandTypeDef",
+    "PlatformScriptKeyOutputTypeDef",
     "PlatformScriptKeyTypeDef",
     "ResponseMetadataTypeDef",
     "RetryWorkflowStepRequestRequestTypeDef",
     "RetryWorkflowStepResponseTypeDef",
     "StartMigrationWorkflowRequestRequestTypeDef",
     "StartMigrationWorkflowResponseTypeDef",
     "StopMigrationWorkflowRequestRequestTypeDef",
     "StopMigrationWorkflowResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWorkflowStepGroupRequestRequestTypeDef",
     "UpdateWorkflowStepResponseTypeDef",
     "WorkflowStepOutputUnionTypeDef",
     "CreateMigrationWorkflowRequestRequestTypeDef",
-    "CreateMigrationWorkflowResponseTypeDef",
     "UpdateMigrationWorkflowRequestRequestTypeDef",
+    "CreateMigrationWorkflowResponseTypeDef",
     "UpdateMigrationWorkflowResponseTypeDef",
     "CreateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowResponseTypeDef",
     "GetTemplateStepGroupResponseTypeDef",
     "GetWorkflowStepGroupResponseTypeDef",
     "UpdateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowTemplateResponseTypeDef",
@@ -105,14 +108,15 @@
     "ListMigrationWorkflowsResponseTypeDef",
     "ListPluginsResponseTypeDef",
     "ListTemplateStepGroupsResponseTypeDef",
     "ListTemplateStepsResponseTypeDef",
     "ListWorkflowStepGroupsResponseTypeDef",
     "ListWorkflowStepsResponseTypeDef",
     "StepAutomationConfigurationTypeDef",
+    "WorkflowStepAutomationConfigurationOutputTypeDef",
     "WorkflowStepAutomationConfigurationTypeDef",
     "WorkflowStepOutputTypeDef",
     "GetTemplateStepResponseTypeDef",
     "CreateWorkflowStepRequestRequestTypeDef",
     "GetWorkflowStepResponseTypeDef",
     "UpdateWorkflowStepRequestRequestTypeDef",
 )
@@ -124,14 +128,25 @@
         "stringValue": str,
         "listOfStringsValue": Sequence[str],
         "mapOfStringValue": Mapping[str, str],
     },
     total=False,
 )
 
+StepInputOutputTypeDef = TypedDict(
+    "StepInputOutputTypeDef",
+    {
+        "integerValue": int,
+        "stringValue": str,
+        "listOfStringsValue": List[str],
+        "mapOfStringValue": Dict[str, str],
+    },
+    total=False,
+)
+
 _RequiredCreateWorkflowStepGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowStepGroupRequestRequestTypeDef",
     {
         "workflowId": str,
         "name": str,
     },
 )
@@ -622,23 +637,41 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+PlatformCommandOutputTypeDef = TypedDict(
+    "PlatformCommandOutputTypeDef",
+    {
+        "linux": str,
+        "windows": str,
+    },
+    total=False,
+)
+
 PlatformCommandTypeDef = TypedDict(
     "PlatformCommandTypeDef",
     {
         "linux": str,
         "windows": str,
     },
     total=False,
 )
 
+PlatformScriptKeyOutputTypeDef = TypedDict(
+    "PlatformScriptKeyOutputTypeDef",
+    {
+        "linux": str,
+        "windows": str,
+    },
+    total=False,
+)
+
 PlatformScriptKeyTypeDef = TypedDict(
     "PlatformScriptKeyTypeDef",
     {
         "linux": str,
         "windows": str,
     },
     total=False,
@@ -795,32 +828,14 @@
 
 class CreateMigrationWorkflowRequestRequestTypeDef(
     _RequiredCreateMigrationWorkflowRequestRequestTypeDef,
     _OptionalCreateMigrationWorkflowRequestRequestTypeDef,
 ):
     pass
 
-CreateMigrationWorkflowResponseTypeDef = TypedDict(
-    "CreateMigrationWorkflowResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "name": str,
-        "description": str,
-        "templateId": str,
-        "adsApplicationConfigurationId": str,
-        "workflowInputs": Dict[str, StepInputTypeDef],
-        "stepTargets": List[str],
-        "status": MigrationWorkflowStatusEnumType,
-        "creationTime": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
@@ -836,24 +851,42 @@
 
 class UpdateMigrationWorkflowRequestRequestTypeDef(
     _RequiredUpdateMigrationWorkflowRequestRequestTypeDef,
     _OptionalUpdateMigrationWorkflowRequestRequestTypeDef,
 ):
     pass
 
+CreateMigrationWorkflowResponseTypeDef = TypedDict(
+    "CreateMigrationWorkflowResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "description": str,
+        "templateId": str,
+        "adsApplicationConfigurationId": str,
+        "workflowInputs": Dict[str, StepInputOutputTypeDef],
+        "stepTargets": List[str],
+        "status": MigrationWorkflowStatusEnumType,
+        "creationTime": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateMigrationWorkflowResponseTypeDef = TypedDict(
     "UpdateMigrationWorkflowResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
         "templateId": str,
         "adsApplicationConfigurationId": str,
-        "workflowInputs": Dict[str, StepInputTypeDef],
+        "workflowInputs": Dict[str, StepInputOutputTypeDef],
         "stepTargets": List[str],
         "status": MigrationWorkflowStatusEnumType,
         "creationTime": datetime,
         "lastModifiedTime": datetime,
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -890,15 +923,15 @@
         "lastStartTime": datetime,
         "lastStopTime": datetime,
         "lastModifiedTime": datetime,
         "endTime": datetime,
         "tools": List[ToolTypeDef],
         "totalSteps": int,
         "completedSteps": int,
-        "workflowInputs": Dict[str, StepInputTypeDef],
+        "workflowInputs": Dict[str, StepInputOutputTypeDef],
         "tags": Dict[str, str],
         "workflowBucket": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTemplateStepGroupResponseTypeDef = TypedDict(
@@ -1029,16 +1062,28 @@
     },
 )
 
 StepAutomationConfigurationTypeDef = TypedDict(
     "StepAutomationConfigurationTypeDef",
     {
         "scriptLocationS3Bucket": str,
-        "scriptLocationS3Key": PlatformScriptKeyTypeDef,
-        "command": PlatformCommandTypeDef,
+        "scriptLocationS3Key": PlatformScriptKeyOutputTypeDef,
+        "command": PlatformCommandOutputTypeDef,
+        "runEnvironment": RunEnvironmentType,
+        "targetType": TargetTypeType,
+    },
+    total=False,
+)
+
+WorkflowStepAutomationConfigurationOutputTypeDef = TypedDict(
+    "WorkflowStepAutomationConfigurationOutputTypeDef",
+    {
+        "scriptLocationS3Bucket": str,
+        "scriptLocationS3Key": PlatformScriptKeyOutputTypeDef,
+        "command": PlatformCommandOutputTypeDef,
         "runEnvironment": RunEnvironmentType,
         "targetType": TargetTypeType,
     },
     total=False,
 )
 
 WorkflowStepAutomationConfigurationTypeDef = TypedDict(
@@ -1116,15 +1161,15 @@
         "name": str,
         "stepGroupId": str,
         "workflowId": str,
         "stepId": str,
         "description": str,
         "stepActionType": StepActionTypeType,
         "owner": OwnerType,
-        "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationTypeDef,
+        "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationOutputTypeDef,
         "stepTarget": List[str],
         "outputs": List[WorkflowStepOutputTypeDef],
         "previous": List[str],
         "next": List[str],
         "status": StepStatusType,
         "statusMessage": str,
         "scriptOutputLocation": str,
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator.egg-info/PKG-INFO` & `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhuborchestrator
-Version: 1.28.0
-Summary: Type annotations for boto3.MigrationHubOrchestrator 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MigrationHubOrchestrator 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-migrationhuborchestrator"></a>
 
 # mypy-boto3-migrationhuborchestrator
 
 [![PyPI - mypy-boto3-migrationhuborchestrator](https://img.shields.io/pypi/v/mypy-boto3-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhuborchestrator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhuborchestrator)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migrationhuborchestrator?color=blue)](https://pypistats.org/packages/mypy-boto3-migrationhuborchestrator)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhuborchestrator)](https://pepy.tech/project/mypy-boto3-migrationhuborchestrator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubOrchestrator 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
+[boto3.MigrationHubOrchestrator 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
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
 [mypy-boto3-migrationhuborchestrator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/).
 
 See how it helps to find and fix potential bugs:
 
@@ -359,14 +359,15 @@
 
 `mypy_boto3_migrationhuborchestrator.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migrationhuborchestrator.type_defs import (
     StepInputTypeDef,
+    StepInputOutputTypeDef,
     CreateWorkflowStepGroupRequestRequestTypeDef,
     ToolTypeDef,
     CreateWorkflowStepResponseTypeDef,
     DeleteMigrationWorkflowRequestRequestTypeDef,
     DeleteMigrationWorkflowResponseTypeDef,
     DeleteWorkflowStepGroupRequestRequestTypeDef,
     DeleteWorkflowStepRequestRequestTypeDef,
@@ -398,31 +399,33 @@
     ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
     ListWorkflowStepGroupsRequestRequestTypeDef,
     WorkflowStepGroupSummaryTypeDef,
     ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
     ListWorkflowStepsRequestRequestTypeDef,
     WorkflowStepSummaryTypeDef,
     PaginatorConfigTypeDef,
+    PlatformCommandOutputTypeDef,
     PlatformCommandTypeDef,
+    PlatformScriptKeyOutputTypeDef,
     PlatformScriptKeyTypeDef,
     ResponseMetadataTypeDef,
     RetryWorkflowStepRequestRequestTypeDef,
     RetryWorkflowStepResponseTypeDef,
     StartMigrationWorkflowRequestRequestTypeDef,
     StartMigrationWorkflowResponseTypeDef,
     StopMigrationWorkflowRequestRequestTypeDef,
     StopMigrationWorkflowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWorkflowStepGroupRequestRequestTypeDef,
     UpdateWorkflowStepResponseTypeDef,
     WorkflowStepOutputUnionTypeDef,
     CreateMigrationWorkflowRequestRequestTypeDef,
-    CreateMigrationWorkflowResponseTypeDef,
     UpdateMigrationWorkflowRequestRequestTypeDef,
+    CreateMigrationWorkflowResponseTypeDef,
     UpdateMigrationWorkflowResponseTypeDef,
     CreateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowResponseTypeDef,
     GetTemplateStepGroupResponseTypeDef,
     GetWorkflowStepGroupResponseTypeDef,
     UpdateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowTemplateResponseTypeDef,
@@ -430,14 +433,15 @@
     ListMigrationWorkflowsResponseTypeDef,
     ListPluginsResponseTypeDef,
     ListTemplateStepGroupsResponseTypeDef,
     ListTemplateStepsResponseTypeDef,
     ListWorkflowStepGroupsResponseTypeDef,
     ListWorkflowStepsResponseTypeDef,
     StepAutomationConfigurationTypeDef,
+    WorkflowStepAutomationConfigurationOutputTypeDef,
     WorkflowStepAutomationConfigurationTypeDef,
     WorkflowStepOutputTypeDef,
     GetTemplateStepResponseTypeDef,
     CreateWorkflowStepRequestRequestTypeDef,
     GetWorkflowStepResponseTypeDef,
     UpdateWorkflowStepRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.0/mypy_boto3_migrationhuborchestrator.egg-info/SOURCES.txt` & `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.0/setup.py` & `mypy-boto3-migrationhuborchestrator-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-migrationhuborchestrator",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_migrationhuborchestrator"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MigrationHubOrchestrator 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.MigrationHubOrchestrator 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

