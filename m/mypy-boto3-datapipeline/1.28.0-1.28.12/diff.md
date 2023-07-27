# Comparing `tmp/mypy-boto3-datapipeline-1.28.0.tar.gz` & `tmp/mypy-boto3-datapipeline-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-datapipeline-1.28.0.tar", last modified: Thu Jul  6 20:59:22 2023, max compression
+gzip compressed data, was "mypy-boto3-datapipeline-1.28.12.tar", last modified: Thu Jul 27 05:34:33 2023, max compression
```

## Comparing `mypy-boto3-datapipeline-1.28.0.tar` & `mypy-boto3-datapipeline-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:22.698274 mypy-boto3-datapipeline-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:37:28.000000 mypy-boto3-datapipeline-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-07-06 20:59:22.698274 mypy-boto3-datapipeline-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13438 2023-07-06 20:37:28.000000 mypy-boto3-datapipeline-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:22.686274 mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-06 20:37:28.000000 mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-06 20:37:28.000000 mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:37:28.000000 mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-07-06 20:37:28.000000 mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-07-06 20:37:28.000000 mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-07-06 20:37:28.000000 mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-06 20:37:28.000000 mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-06 20:37:28.000000 mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-07-06 20:37:28.000000 mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:37:28.000000 mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17905 2023-07-06 20:37:29.000000 mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17873 2023-07-06 20:37:29.000000 mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:37:28.000000 mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:22.698274 mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-07-06 20:59:22.000000 mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 20:59:22.000000 mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:22.000000 mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:22.000000 mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:22.000000 mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 20:59:22.000000 mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:22.698274 mypy-boto3-datapipeline-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:37:28.000000 mypy-boto3-datapipeline-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.608536 mypy-boto3-datapipeline-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-07-27 05:34:33.608536 mypy-boto3-datapipeline-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13606 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.604536 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19268 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19234 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.608536 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-07-27 05:34:33.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:34:33.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:33.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:33.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:33.608536 mypy-boto3-datapipeline-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:19:59.000000 mypy-boto3-datapipeline-1.28.12/setup.py
```

### Comparing `mypy-boto3-datapipeline-1.28.0/LICENSE` & `mypy-boto3-datapipeline-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.0/PKG-INFO` & `mypy-boto3-datapipeline-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datapipeline
-Version: 1.28.0
-Summary: Type annotations for boto3.DataPipeline 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.DataPipeline 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-datapipeline"></a>
 
 # mypy-boto3-datapipeline
 
 [![PyPI - mypy-boto3-datapipeline](https://img.shields.io/pypi/v/mypy-boto3-datapipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-datapipeline)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datapipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-datapipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-datapipeline?color=blue)](https://pypistats.org/packages/mypy-boto3-datapipeline)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-datapipeline)](https://pepy.tech/project/mypy-boto3-datapipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataPipeline 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
+[boto3.DataPipeline 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
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
 [mypy-boto3-datapipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,52 +340,58 @@
     DeletePipelineInputRequestTypeDef,
     DescribeObjectsInputDescribeObjectsPaginateTypeDef,
     DescribeObjectsInputRequestTypeDef,
     DescribePipelinesInputRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluateExpressionInputRequestTypeDef,
     EvaluateExpressionOutputTypeDef,
+    FieldOutputTypeDef,
     FieldTypeDef,
     GetPipelineDefinitionInputRequestTypeDef,
+    ParameterValueOutputTypeDef,
     InstanceIdentityTypeDef,
     ListPipelinesInputListPipelinesPaginateTypeDef,
     ListPipelinesInputRequestTypeDef,
     PipelineIdNameTypeDef,
     OperatorTypeDef,
     PaginatorConfigTypeDef,
+    ParameterAttributeOutputTypeDef,
     ParameterAttributeTypeDef,
+    TagOutputTypeDef,
     ValidationErrorTypeDef,
     ValidationWarningTypeDef,
     QueryObjectsOutputTypeDef,
     RemoveTagsInputRequestTypeDef,
     ReportTaskProgressOutputTypeDef,
     ReportTaskRunnerHeartbeatInputRequestTypeDef,
     ReportTaskRunnerHeartbeatOutputTypeDef,
     ResponseMetadataTypeDef,
     SetStatusInputRequestTypeDef,
     SetTaskStatusInputRequestTypeDef,
     ActivatePipelineInputRequestTypeDef,
     AddTagsInputRequestTypeDef,
     CreatePipelineInputRequestTypeDef,
-    PipelineDescriptionTypeDef,
+    PipelineObjectOutputTypeDef,
     PipelineObjectTypeDef,
     ReportTaskProgressInputRequestTypeDef,
     PollForTaskInputRequestTypeDef,
     ListPipelinesOutputTypeDef,
     SelectorTypeDef,
+    ParameterObjectOutputTypeDef,
     ParameterObjectTypeDef,
+    PipelineDescriptionTypeDef,
     PutPipelineDefinitionOutputTypeDef,
     ValidatePipelineDefinitionOutputTypeDef,
-    DescribePipelinesOutputTypeDef,
     DescribeObjectsOutputTypeDef,
     TaskObjectTypeDef,
     QueryTypeDef,
     GetPipelineDefinitionOutputTypeDef,
     PutPipelineDefinitionInputRequestTypeDef,
     ValidatePipelineDefinitionInputRequestTypeDef,
+    DescribePipelinesOutputTypeDef,
     PollForTaskOutputTypeDef,
     QueryObjectsInputQueryObjectsPaginateTypeDef,
     QueryObjectsInputRequestTypeDef,
 )
 
 
 def get_structure() -> ParameterValueTypeDef:
```

### Comparing `mypy-boto3-datapipeline-1.28.0/README.md` & `mypy-boto3-datapipeline-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-datapipeline"></a>
 
 # mypy-boto3-datapipeline
 
 [![PyPI - mypy-boto3-datapipeline](https://img.shields.io/pypi/v/mypy-boto3-datapipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-datapipeline)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datapipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-datapipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-datapipeline?color=blue)](https://pypistats.org/packages/mypy-boto3-datapipeline)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-datapipeline)](https://pepy.tech/project/mypy-boto3-datapipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataPipeline 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
+[boto3.DataPipeline 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
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
 [mypy-boto3-datapipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/).
 
 See how it helps to find and fix potential bugs:
 
@@ -308,52 +308,58 @@
     DeletePipelineInputRequestTypeDef,
     DescribeObjectsInputDescribeObjectsPaginateTypeDef,
     DescribeObjectsInputRequestTypeDef,
     DescribePipelinesInputRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluateExpressionInputRequestTypeDef,
     EvaluateExpressionOutputTypeDef,
+    FieldOutputTypeDef,
     FieldTypeDef,
     GetPipelineDefinitionInputRequestTypeDef,
+    ParameterValueOutputTypeDef,
     InstanceIdentityTypeDef,
     ListPipelinesInputListPipelinesPaginateTypeDef,
     ListPipelinesInputRequestTypeDef,
     PipelineIdNameTypeDef,
     OperatorTypeDef,
     PaginatorConfigTypeDef,
+    ParameterAttributeOutputTypeDef,
     ParameterAttributeTypeDef,
+    TagOutputTypeDef,
     ValidationErrorTypeDef,
     ValidationWarningTypeDef,
     QueryObjectsOutputTypeDef,
     RemoveTagsInputRequestTypeDef,
     ReportTaskProgressOutputTypeDef,
     ReportTaskRunnerHeartbeatInputRequestTypeDef,
     ReportTaskRunnerHeartbeatOutputTypeDef,
     ResponseMetadataTypeDef,
     SetStatusInputRequestTypeDef,
     SetTaskStatusInputRequestTypeDef,
     ActivatePipelineInputRequestTypeDef,
     AddTagsInputRequestTypeDef,
     CreatePipelineInputRequestTypeDef,
-    PipelineDescriptionTypeDef,
+    PipelineObjectOutputTypeDef,
     PipelineObjectTypeDef,
     ReportTaskProgressInputRequestTypeDef,
     PollForTaskInputRequestTypeDef,
     ListPipelinesOutputTypeDef,
     SelectorTypeDef,
+    ParameterObjectOutputTypeDef,
     ParameterObjectTypeDef,
+    PipelineDescriptionTypeDef,
     PutPipelineDefinitionOutputTypeDef,
     ValidatePipelineDefinitionOutputTypeDef,
-    DescribePipelinesOutputTypeDef,
     DescribeObjectsOutputTypeDef,
     TaskObjectTypeDef,
     QueryTypeDef,
     GetPipelineDefinitionOutputTypeDef,
     PutPipelineDefinitionInputRequestTypeDef,
     ValidatePipelineDefinitionInputRequestTypeDef,
+    DescribePipelinesOutputTypeDef,
     PollForTaskOutputTypeDef,
     QueryObjectsInputQueryObjectsPaginateTypeDef,
     QueryObjectsInputRequestTypeDef,
 )
 
 
 def get_structure() -> ParameterValueTypeDef:
```

### Comparing `mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/__init__.py` & `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/__init__.pyi` & `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/__main__.py` & `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DataPipeline 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.DataPipeline 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline\nOther"
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

### Comparing `mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/client.py` & `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/client.pyi` & `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/literals.py` & `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,15 @@
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
@@ -240,26 +241,28 @@
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

### Comparing `mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/literals.pyi` & `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,15 @@
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
@@ -238,26 +239,28 @@
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

### Comparing `mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/paginator.py` & `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/paginator.pyi` & `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/type_defs.py` & `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,52 +31,58 @@
     "DeletePipelineInputRequestTypeDef",
     "DescribeObjectsInputDescribeObjectsPaginateTypeDef",
     "DescribeObjectsInputRequestTypeDef",
     "DescribePipelinesInputRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EvaluateExpressionInputRequestTypeDef",
     "EvaluateExpressionOutputTypeDef",
+    "FieldOutputTypeDef",
     "FieldTypeDef",
     "GetPipelineDefinitionInputRequestTypeDef",
+    "ParameterValueOutputTypeDef",
     "InstanceIdentityTypeDef",
     "ListPipelinesInputListPipelinesPaginateTypeDef",
     "ListPipelinesInputRequestTypeDef",
     "PipelineIdNameTypeDef",
     "OperatorTypeDef",
     "PaginatorConfigTypeDef",
+    "ParameterAttributeOutputTypeDef",
     "ParameterAttributeTypeDef",
+    "TagOutputTypeDef",
     "ValidationErrorTypeDef",
     "ValidationWarningTypeDef",
     "QueryObjectsOutputTypeDef",
     "RemoveTagsInputRequestTypeDef",
     "ReportTaskProgressOutputTypeDef",
     "ReportTaskRunnerHeartbeatInputRequestTypeDef",
     "ReportTaskRunnerHeartbeatOutputTypeDef",
     "ResponseMetadataTypeDef",
     "SetStatusInputRequestTypeDef",
     "SetTaskStatusInputRequestTypeDef",
     "ActivatePipelineInputRequestTypeDef",
     "AddTagsInputRequestTypeDef",
     "CreatePipelineInputRequestTypeDef",
-    "PipelineDescriptionTypeDef",
+    "PipelineObjectOutputTypeDef",
     "PipelineObjectTypeDef",
     "ReportTaskProgressInputRequestTypeDef",
     "PollForTaskInputRequestTypeDef",
     "ListPipelinesOutputTypeDef",
     "SelectorTypeDef",
+    "ParameterObjectOutputTypeDef",
     "ParameterObjectTypeDef",
+    "PipelineDescriptionTypeDef",
     "PutPipelineDefinitionOutputTypeDef",
     "ValidatePipelineDefinitionOutputTypeDef",
-    "DescribePipelinesOutputTypeDef",
     "DescribeObjectsOutputTypeDef",
     "TaskObjectTypeDef",
     "QueryTypeDef",
     "GetPipelineDefinitionOutputTypeDef",
     "PutPipelineDefinitionInputRequestTypeDef",
     "ValidatePipelineDefinitionInputRequestTypeDef",
+    "DescribePipelinesOutputTypeDef",
     "PollForTaskOutputTypeDef",
     "QueryObjectsInputQueryObjectsPaginateTypeDef",
     "QueryObjectsInputRequestTypeDef",
 )
 
 ParameterValueTypeDef = TypedDict(
     "ParameterValueTypeDef",
@@ -204,14 +210,34 @@
     "EvaluateExpressionOutputTypeDef",
     {
         "evaluatedExpression": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredFieldOutputTypeDef = TypedDict(
+    "_RequiredFieldOutputTypeDef",
+    {
+        "key": str,
+    },
+)
+_OptionalFieldOutputTypeDef = TypedDict(
+    "_OptionalFieldOutputTypeDef",
+    {
+        "stringValue": str,
+        "refValue": str,
+    },
+    total=False,
+)
+
+
+class FieldOutputTypeDef(_RequiredFieldOutputTypeDef, _OptionalFieldOutputTypeDef):
+    pass
+
+
 _RequiredFieldTypeDef = TypedDict(
     "_RequiredFieldTypeDef",
     {
         "key": str,
     },
 )
 _OptionalFieldTypeDef = TypedDict(
@@ -246,14 +272,22 @@
 class GetPipelineDefinitionInputRequestTypeDef(
     _RequiredGetPipelineDefinitionInputRequestTypeDef,
     _OptionalGetPipelineDefinitionInputRequestTypeDef,
 ):
     pass
 
 
+ParameterValueOutputTypeDef = TypedDict(
+    "ParameterValueOutputTypeDef",
+    {
+        "id": str,
+        "stringValue": str,
+    },
+)
+
 InstanceIdentityTypeDef = TypedDict(
     "InstanceIdentityTypeDef",
     {
         "document": str,
         "signature": str,
     },
     total=False,
@@ -299,22 +333,38 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+ParameterAttributeOutputTypeDef = TypedDict(
+    "ParameterAttributeOutputTypeDef",
+    {
+        "key": str,
+        "stringValue": str,
+    },
+)
+
 ParameterAttributeTypeDef = TypedDict(
     "ParameterAttributeTypeDef",
     {
         "key": str,
         "stringValue": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 ValidationErrorTypeDef = TypedDict(
     "ValidationErrorTypeDef",
     {
         "id": str,
         "errors": List[str],
     },
     total=False,
@@ -479,44 +529,29 @@
 
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
 
-_RequiredPipelineDescriptionTypeDef = TypedDict(
-    "_RequiredPipelineDescriptionTypeDef",
+PipelineObjectOutputTypeDef = TypedDict(
+    "PipelineObjectOutputTypeDef",
     {
-        "pipelineId": str,
+        "id": str,
         "name": str,
-        "fields": List[FieldTypeDef],
-    },
-)
-_OptionalPipelineDescriptionTypeDef = TypedDict(
-    "_OptionalPipelineDescriptionTypeDef",
-    {
-        "description": str,
-        "tags": List[TagTypeDef],
+        "fields": List[FieldOutputTypeDef],
     },
-    total=False,
 )
 
-
-class PipelineDescriptionTypeDef(
-    _RequiredPipelineDescriptionTypeDef, _OptionalPipelineDescriptionTypeDef
-):
-    pass
-
-
 PipelineObjectTypeDef = TypedDict(
     "PipelineObjectTypeDef",
     {
         "id": str,
         "name": str,
-        "fields": List[FieldTypeDef],
+        "fields": Sequence[FieldTypeDef],
     },
 )
 
 _RequiredReportTaskProgressInputRequestTypeDef = TypedDict(
     "_RequiredReportTaskProgressInputRequestTypeDef",
     {
         "taskId": str,
@@ -574,22 +609,54 @@
     {
         "fieldName": str,
         "operator": OperatorTypeDef,
     },
     total=False,
 )
 
+ParameterObjectOutputTypeDef = TypedDict(
+    "ParameterObjectOutputTypeDef",
+    {
+        "id": str,
+        "attributes": List[ParameterAttributeOutputTypeDef],
+    },
+)
+
 ParameterObjectTypeDef = TypedDict(
     "ParameterObjectTypeDef",
     {
         "id": str,
-        "attributes": List[ParameterAttributeTypeDef],
+        "attributes": Sequence[ParameterAttributeTypeDef],
     },
 )
 
+_RequiredPipelineDescriptionTypeDef = TypedDict(
+    "_RequiredPipelineDescriptionTypeDef",
+    {
+        "pipelineId": str,
+        "name": str,
+        "fields": List[FieldOutputTypeDef],
+    },
+)
+_OptionalPipelineDescriptionTypeDef = TypedDict(
+    "_OptionalPipelineDescriptionTypeDef",
+    {
+        "description": str,
+        "tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class PipelineDescriptionTypeDef(
+    _RequiredPipelineDescriptionTypeDef, _OptionalPipelineDescriptionTypeDef
+):
+    pass
+
+
 PutPipelineDefinitionOutputTypeDef = TypedDict(
     "PutPipelineDefinitionOutputTypeDef",
     {
         "validationErrors": List[ValidationErrorTypeDef],
         "validationWarnings": List[ValidationWarningTypeDef],
         "errored": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -602,39 +669,31 @@
         "validationErrors": List[ValidationErrorTypeDef],
         "validationWarnings": List[ValidationWarningTypeDef],
         "errored": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribePipelinesOutputTypeDef = TypedDict(
-    "DescribePipelinesOutputTypeDef",
-    {
-        "pipelineDescriptionList": List[PipelineDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeObjectsOutputTypeDef = TypedDict(
     "DescribeObjectsOutputTypeDef",
     {
-        "pipelineObjects": List[PipelineObjectTypeDef],
+        "pipelineObjects": List[PipelineObjectOutputTypeDef],
         "marker": str,
         "hasMoreResults": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TaskObjectTypeDef = TypedDict(
     "TaskObjectTypeDef",
     {
         "taskId": str,
         "pipelineId": str,
         "attemptId": str,
-        "objects": Dict[str, PipelineObjectTypeDef],
+        "objects": Dict[str, PipelineObjectOutputTypeDef],
     },
     total=False,
 )
 
 QueryTypeDef = TypedDict(
     "QueryTypeDef",
     {
@@ -642,17 +701,17 @@
     },
     total=False,
 )
 
 GetPipelineDefinitionOutputTypeDef = TypedDict(
     "GetPipelineDefinitionOutputTypeDef",
     {
-        "pipelineObjects": List[PipelineObjectTypeDef],
-        "parameterObjects": List[ParameterObjectTypeDef],
-        "parameterValues": List[ParameterValueTypeDef],
+        "pipelineObjects": List[PipelineObjectOutputTypeDef],
+        "parameterObjects": List[ParameterObjectOutputTypeDef],
+        "parameterValues": List[ParameterValueOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_RequiredPutPipelineDefinitionInputRequestTypeDef",
     {
@@ -697,14 +756,22 @@
 class ValidatePipelineDefinitionInputRequestTypeDef(
     _RequiredValidatePipelineDefinitionInputRequestTypeDef,
     _OptionalValidatePipelineDefinitionInputRequestTypeDef,
 ):
     pass
 
 
+DescribePipelinesOutputTypeDef = TypedDict(
+    "DescribePipelinesOutputTypeDef",
+    {
+        "pipelineDescriptionList": List[PipelineDescriptionTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PollForTaskOutputTypeDef = TypedDict(
     "PollForTaskOutputTypeDef",
     {
         "taskObject": TaskObjectTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline/type_defs.pyi` & `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -30,52 +30,58 @@
     "DeletePipelineInputRequestTypeDef",
     "DescribeObjectsInputDescribeObjectsPaginateTypeDef",
     "DescribeObjectsInputRequestTypeDef",
     "DescribePipelinesInputRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EvaluateExpressionInputRequestTypeDef",
     "EvaluateExpressionOutputTypeDef",
+    "FieldOutputTypeDef",
     "FieldTypeDef",
     "GetPipelineDefinitionInputRequestTypeDef",
+    "ParameterValueOutputTypeDef",
     "InstanceIdentityTypeDef",
     "ListPipelinesInputListPipelinesPaginateTypeDef",
     "ListPipelinesInputRequestTypeDef",
     "PipelineIdNameTypeDef",
     "OperatorTypeDef",
     "PaginatorConfigTypeDef",
+    "ParameterAttributeOutputTypeDef",
     "ParameterAttributeTypeDef",
+    "TagOutputTypeDef",
     "ValidationErrorTypeDef",
     "ValidationWarningTypeDef",
     "QueryObjectsOutputTypeDef",
     "RemoveTagsInputRequestTypeDef",
     "ReportTaskProgressOutputTypeDef",
     "ReportTaskRunnerHeartbeatInputRequestTypeDef",
     "ReportTaskRunnerHeartbeatOutputTypeDef",
     "ResponseMetadataTypeDef",
     "SetStatusInputRequestTypeDef",
     "SetTaskStatusInputRequestTypeDef",
     "ActivatePipelineInputRequestTypeDef",
     "AddTagsInputRequestTypeDef",
     "CreatePipelineInputRequestTypeDef",
-    "PipelineDescriptionTypeDef",
+    "PipelineObjectOutputTypeDef",
     "PipelineObjectTypeDef",
     "ReportTaskProgressInputRequestTypeDef",
     "PollForTaskInputRequestTypeDef",
     "ListPipelinesOutputTypeDef",
     "SelectorTypeDef",
+    "ParameterObjectOutputTypeDef",
     "ParameterObjectTypeDef",
+    "PipelineDescriptionTypeDef",
     "PutPipelineDefinitionOutputTypeDef",
     "ValidatePipelineDefinitionOutputTypeDef",
-    "DescribePipelinesOutputTypeDef",
     "DescribeObjectsOutputTypeDef",
     "TaskObjectTypeDef",
     "QueryTypeDef",
     "GetPipelineDefinitionOutputTypeDef",
     "PutPipelineDefinitionInputRequestTypeDef",
     "ValidatePipelineDefinitionInputRequestTypeDef",
+    "DescribePipelinesOutputTypeDef",
     "PollForTaskOutputTypeDef",
     "QueryObjectsInputQueryObjectsPaginateTypeDef",
     "QueryObjectsInputRequestTypeDef",
 )
 
 ParameterValueTypeDef = TypedDict(
     "ParameterValueTypeDef",
@@ -197,14 +203,32 @@
     "EvaluateExpressionOutputTypeDef",
     {
         "evaluatedExpression": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredFieldOutputTypeDef = TypedDict(
+    "_RequiredFieldOutputTypeDef",
+    {
+        "key": str,
+    },
+)
+_OptionalFieldOutputTypeDef = TypedDict(
+    "_OptionalFieldOutputTypeDef",
+    {
+        "stringValue": str,
+        "refValue": str,
+    },
+    total=False,
+)
+
+class FieldOutputTypeDef(_RequiredFieldOutputTypeDef, _OptionalFieldOutputTypeDef):
+    pass
+
 _RequiredFieldTypeDef = TypedDict(
     "_RequiredFieldTypeDef",
     {
         "key": str,
     },
 )
 _OptionalFieldTypeDef = TypedDict(
@@ -235,14 +259,22 @@
 
 class GetPipelineDefinitionInputRequestTypeDef(
     _RequiredGetPipelineDefinitionInputRequestTypeDef,
     _OptionalGetPipelineDefinitionInputRequestTypeDef,
 ):
     pass
 
+ParameterValueOutputTypeDef = TypedDict(
+    "ParameterValueOutputTypeDef",
+    {
+        "id": str,
+        "stringValue": str,
+    },
+)
+
 InstanceIdentityTypeDef = TypedDict(
     "InstanceIdentityTypeDef",
     {
         "document": str,
         "signature": str,
     },
     total=False,
@@ -288,22 +320,38 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+ParameterAttributeOutputTypeDef = TypedDict(
+    "ParameterAttributeOutputTypeDef",
+    {
+        "key": str,
+        "stringValue": str,
+    },
+)
+
 ParameterAttributeTypeDef = TypedDict(
     "ParameterAttributeTypeDef",
     {
         "key": str,
         "stringValue": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 ValidationErrorTypeDef = TypedDict(
     "ValidationErrorTypeDef",
     {
         "id": str,
         "errors": List[str],
     },
     total=False,
@@ -460,42 +508,29 @@
 )
 
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
-_RequiredPipelineDescriptionTypeDef = TypedDict(
-    "_RequiredPipelineDescriptionTypeDef",
+PipelineObjectOutputTypeDef = TypedDict(
+    "PipelineObjectOutputTypeDef",
     {
-        "pipelineId": str,
+        "id": str,
         "name": str,
-        "fields": List[FieldTypeDef],
+        "fields": List[FieldOutputTypeDef],
     },
 )
-_OptionalPipelineDescriptionTypeDef = TypedDict(
-    "_OptionalPipelineDescriptionTypeDef",
-    {
-        "description": str,
-        "tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-class PipelineDescriptionTypeDef(
-    _RequiredPipelineDescriptionTypeDef, _OptionalPipelineDescriptionTypeDef
-):
-    pass
 
 PipelineObjectTypeDef = TypedDict(
     "PipelineObjectTypeDef",
     {
         "id": str,
         "name": str,
-        "fields": List[FieldTypeDef],
+        "fields": Sequence[FieldTypeDef],
     },
 )
 
 _RequiredReportTaskProgressInputRequestTypeDef = TypedDict(
     "_RequiredReportTaskProgressInputRequestTypeDef",
     {
         "taskId": str,
@@ -549,22 +584,52 @@
     {
         "fieldName": str,
         "operator": OperatorTypeDef,
     },
     total=False,
 )
 
+ParameterObjectOutputTypeDef = TypedDict(
+    "ParameterObjectOutputTypeDef",
+    {
+        "id": str,
+        "attributes": List[ParameterAttributeOutputTypeDef],
+    },
+)
+
 ParameterObjectTypeDef = TypedDict(
     "ParameterObjectTypeDef",
     {
         "id": str,
-        "attributes": List[ParameterAttributeTypeDef],
+        "attributes": Sequence[ParameterAttributeTypeDef],
+    },
+)
+
+_RequiredPipelineDescriptionTypeDef = TypedDict(
+    "_RequiredPipelineDescriptionTypeDef",
+    {
+        "pipelineId": str,
+        "name": str,
+        "fields": List[FieldOutputTypeDef],
+    },
+)
+_OptionalPipelineDescriptionTypeDef = TypedDict(
+    "_OptionalPipelineDescriptionTypeDef",
+    {
+        "description": str,
+        "tags": List[TagOutputTypeDef],
     },
+    total=False,
 )
 
+class PipelineDescriptionTypeDef(
+    _RequiredPipelineDescriptionTypeDef, _OptionalPipelineDescriptionTypeDef
+):
+    pass
+
 PutPipelineDefinitionOutputTypeDef = TypedDict(
     "PutPipelineDefinitionOutputTypeDef",
     {
         "validationErrors": List[ValidationErrorTypeDef],
         "validationWarnings": List[ValidationWarningTypeDef],
         "errored": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -577,39 +642,31 @@
         "validationErrors": List[ValidationErrorTypeDef],
         "validationWarnings": List[ValidationWarningTypeDef],
         "errored": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribePipelinesOutputTypeDef = TypedDict(
-    "DescribePipelinesOutputTypeDef",
-    {
-        "pipelineDescriptionList": List[PipelineDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeObjectsOutputTypeDef = TypedDict(
     "DescribeObjectsOutputTypeDef",
     {
-        "pipelineObjects": List[PipelineObjectTypeDef],
+        "pipelineObjects": List[PipelineObjectOutputTypeDef],
         "marker": str,
         "hasMoreResults": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TaskObjectTypeDef = TypedDict(
     "TaskObjectTypeDef",
     {
         "taskId": str,
         "pipelineId": str,
         "attemptId": str,
-        "objects": Dict[str, PipelineObjectTypeDef],
+        "objects": Dict[str, PipelineObjectOutputTypeDef],
     },
     total=False,
 )
 
 QueryTypeDef = TypedDict(
     "QueryTypeDef",
     {
@@ -617,17 +674,17 @@
     },
     total=False,
 )
 
 GetPipelineDefinitionOutputTypeDef = TypedDict(
     "GetPipelineDefinitionOutputTypeDef",
     {
-        "pipelineObjects": List[PipelineObjectTypeDef],
-        "parameterObjects": List[ParameterObjectTypeDef],
-        "parameterValues": List[ParameterValueTypeDef],
+        "pipelineObjects": List[PipelineObjectOutputTypeDef],
+        "parameterObjects": List[ParameterObjectOutputTypeDef],
+        "parameterValues": List[ParameterValueOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_RequiredPutPipelineDefinitionInputRequestTypeDef",
     {
@@ -668,14 +725,22 @@
 
 class ValidatePipelineDefinitionInputRequestTypeDef(
     _RequiredValidatePipelineDefinitionInputRequestTypeDef,
     _OptionalValidatePipelineDefinitionInputRequestTypeDef,
 ):
     pass
 
+DescribePipelinesOutputTypeDef = TypedDict(
+    "DescribePipelinesOutputTypeDef",
+    {
+        "pipelineDescriptionList": List[PipelineDescriptionTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PollForTaskOutputTypeDef = TypedDict(
     "PollForTaskOutputTypeDef",
     {
         "taskObject": TaskObjectTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline.egg-info/PKG-INFO` & `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datapipeline
-Version: 1.28.0
-Summary: Type annotations for boto3.DataPipeline 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.DataPipeline 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-datapipeline"></a>
 
 # mypy-boto3-datapipeline
 
 [![PyPI - mypy-boto3-datapipeline](https://img.shields.io/pypi/v/mypy-boto3-datapipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-datapipeline)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datapipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-datapipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-datapipeline?color=blue)](https://pypistats.org/packages/mypy-boto3-datapipeline)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-datapipeline)](https://pepy.tech/project/mypy-boto3-datapipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataPipeline 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
+[boto3.DataPipeline 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
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
 [mypy-boto3-datapipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,52 +340,58 @@
     DeletePipelineInputRequestTypeDef,
     DescribeObjectsInputDescribeObjectsPaginateTypeDef,
     DescribeObjectsInputRequestTypeDef,
     DescribePipelinesInputRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluateExpressionInputRequestTypeDef,
     EvaluateExpressionOutputTypeDef,
+    FieldOutputTypeDef,
     FieldTypeDef,
     GetPipelineDefinitionInputRequestTypeDef,
+    ParameterValueOutputTypeDef,
     InstanceIdentityTypeDef,
     ListPipelinesInputListPipelinesPaginateTypeDef,
     ListPipelinesInputRequestTypeDef,
     PipelineIdNameTypeDef,
     OperatorTypeDef,
     PaginatorConfigTypeDef,
+    ParameterAttributeOutputTypeDef,
     ParameterAttributeTypeDef,
+    TagOutputTypeDef,
     ValidationErrorTypeDef,
     ValidationWarningTypeDef,
     QueryObjectsOutputTypeDef,
     RemoveTagsInputRequestTypeDef,
     ReportTaskProgressOutputTypeDef,
     ReportTaskRunnerHeartbeatInputRequestTypeDef,
     ReportTaskRunnerHeartbeatOutputTypeDef,
     ResponseMetadataTypeDef,
     SetStatusInputRequestTypeDef,
     SetTaskStatusInputRequestTypeDef,
     ActivatePipelineInputRequestTypeDef,
     AddTagsInputRequestTypeDef,
     CreatePipelineInputRequestTypeDef,
-    PipelineDescriptionTypeDef,
+    PipelineObjectOutputTypeDef,
     PipelineObjectTypeDef,
     ReportTaskProgressInputRequestTypeDef,
     PollForTaskInputRequestTypeDef,
     ListPipelinesOutputTypeDef,
     SelectorTypeDef,
+    ParameterObjectOutputTypeDef,
     ParameterObjectTypeDef,
+    PipelineDescriptionTypeDef,
     PutPipelineDefinitionOutputTypeDef,
     ValidatePipelineDefinitionOutputTypeDef,
-    DescribePipelinesOutputTypeDef,
     DescribeObjectsOutputTypeDef,
     TaskObjectTypeDef,
     QueryTypeDef,
     GetPipelineDefinitionOutputTypeDef,
     PutPipelineDefinitionInputRequestTypeDef,
     ValidatePipelineDefinitionInputRequestTypeDef,
+    DescribePipelinesOutputTypeDef,
     PollForTaskOutputTypeDef,
     QueryObjectsInputQueryObjectsPaginateTypeDef,
     QueryObjectsInputRequestTypeDef,
 )
 
 
 def get_structure() -> ParameterValueTypeDef:
```

### Comparing `mypy-boto3-datapipeline-1.28.0/mypy_boto3_datapipeline.egg-info/SOURCES.txt` & `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.0/setup.py` & `mypy-boto3-datapipeline-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-datapipeline",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_datapipeline"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DataPipeline 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.DataPipeline 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

