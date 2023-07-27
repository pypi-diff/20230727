# Comparing `tmp/mypy-boto3-databrew-1.28.0.tar.gz` & `tmp/mypy-boto3-databrew-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-databrew-1.28.0.tar", last modified: Thu Jul  6 20:59:22 2023, max compression
+gzip compressed data, was "mypy-boto3-databrew-1.28.12.tar", last modified: Thu Jul 27 05:34:33 2023, max compression
```

## Comparing `mypy-boto3-databrew-1.28.0.tar` & `mypy-boto3-databrew-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:22.570274 mypy-boto3-databrew-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:37:21.000000 mypy-boto3-databrew-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18990 2023-07-06 20:59:22.570274 mypy-boto3-databrew-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17497 2023-07-06 20:37:21.000000 mypy-boto3-databrew-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:22.570274 mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-06 20:37:21.000000 mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-06 20:37:21.000000 mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 20:37:21.000000 mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33785 2023-07-06 20:37:21.000000 mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33726 2023-07-06 20:37:21.000000 mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-07-06 20:37:22.000000 mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-07-06 20:37:21.000000 mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-07-06 20:37:21.000000 mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-07-06 20:37:21.000000 mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:37:21.000000 mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    54172 2023-07-06 20:37:23.000000 mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    54074 2023-07-06 20:37:22.000000 mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:37:21.000000 mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:22.570274 mypy-boto3-databrew-1.28.0/mypy_boto3_databrew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18990 2023-07-06 20:59:22.000000 mypy-boto3-databrew-1.28.0/mypy_boto3_databrew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 20:59:22.000000 mypy-boto3-databrew-1.28.0/mypy_boto3_databrew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:22.000000 mypy-boto3-databrew-1.28.0/mypy_boto3_databrew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:22.000000 mypy-boto3-databrew-1.28.0/mypy_boto3_databrew.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:22.000000 mypy-boto3-databrew-1.28.0/mypy_boto3_databrew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 20:59:22.000000 mypy-boto3-databrew-1.28.0/mypy_boto3_databrew.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:22.570274 mypy-boto3-databrew-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-06 20:37:21.000000 mypy-boto3-databrew-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.292537 mypy-boto3-databrew-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20150 2023-07-27 05:34:33.292537 mypy-boto3-databrew-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18655 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.288537 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33785 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33726 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    67166 2023-07-27 05:19:58.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67034 2023-07-27 05:19:56.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.292537 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20150 2023-07-27 05:34:33.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 05:34:33.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:33.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 05:34:33.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:33.292537 mypy-boto3-databrew-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/setup.py
```

### Comparing `mypy-boto3-databrew-1.28.0/LICENSE` & `mypy-boto3-databrew-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.0/PKG-INFO` & `mypy-boto3-databrew-1.28.12/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-databrew
-Version: 1.28.0
-Summary: Type annotations for boto3.GlueDataBrew 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.GlueDataBrew 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-databrew"></a>
 
 # mypy-boto3-databrew
 
 [![PyPI - mypy-boto3-databrew](https://img.shields.io/pypi/v/mypy-boto3-databrew.svg?color=blue)](https://pypi.org/project/mypy-boto3-databrew)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-databrew.svg?color=blue)](https://pypi.org/project/mypy-boto3-databrew)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-databrew?color=blue)](https://pypistats.org/packages/mypy-boto3-databrew)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-databrew)](https://pepy.tech/project/mypy-boto3-databrew)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GlueDataBrew 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
+[boto3.GlueDataBrew 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
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
 [mypy-boto3-databrew docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/).
 
 See how it helps to find and fix potential bugs:
 
@@ -362,34 +362,42 @@
 ### Typed dictionaries
 
 `mypy_boto3_databrew.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_databrew.type_defs import (
+    AllowedStatisticsOutputTypeDef,
     AllowedStatisticsTypeDef,
     BatchDeleteRecipeVersionRequestRequestTypeDef,
     RecipeVersionErrorDetailTypeDef,
+    ColumnSelectorOutputTypeDef,
     ColumnSelectorTypeDef,
+    ConditionExpressionOutputTypeDef,
     ConditionExpressionTypeDef,
     CreateDatasetResponseTypeDef,
     JobSampleTypeDef,
     S3LocationTypeDef,
     ValidationConfigurationTypeDef,
     CreateProfileJobResponseTypeDef,
     SampleTypeDef,
     CreateProjectResponseTypeDef,
     RecipeReferenceTypeDef,
     CreateRecipeJobResponseTypeDef,
     CreateRecipeResponseTypeDef,
     CreateRulesetResponseTypeDef,
     CreateScheduleRequestRequestTypeDef,
     CreateScheduleResponseTypeDef,
+    CsvOptionsOutputTypeDef,
     CsvOptionsTypeDef,
+    CsvOutputOptionsOutputTypeDef,
     CsvOutputOptionsTypeDef,
+    S3LocationOutputTypeDef,
+    DatetimeOptionsOutputTypeDef,
+    FilterExpressionOutputTypeDef,
     DatetimeOptionsTypeDef,
     FilterExpressionTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteDatasetResponseTypeDef,
     DeleteJobRequestRequestTypeDef,
     DeleteJobResponseTypeDef,
     DeleteProjectRequestRequestTypeDef,
@@ -398,23 +406,31 @@
     DeleteRecipeVersionResponseTypeDef,
     DeleteRulesetRequestRequestTypeDef,
     DeleteRulesetResponseTypeDef,
     DeleteScheduleRequestRequestTypeDef,
     DeleteScheduleResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
+    JobSampleOutputTypeDef,
+    RecipeReferenceOutputTypeDef,
+    ValidationConfigurationOutputTypeDef,
     DescribeJobRunRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
+    SampleOutputTypeDef,
     DescribeRecipeRequestRequestTypeDef,
     DescribeRulesetRequestRequestTypeDef,
     DescribeScheduleRequestRequestTypeDef,
     DescribeScheduleResponseTypeDef,
+    ExcelOptionsOutputTypeDef,
     ExcelOptionsTypeDef,
+    FilesLimitOutputTypeDef,
     FilesLimitTypeDef,
+    JsonOptionsOutputTypeDef,
     JsonOptionsTypeDef,
+    MetadataOutputTypeDef,
     MetadataTypeDef,
     ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
@@ -431,91 +447,109 @@
     ListSchedulesRequestRequestTypeDef,
     ScheduleTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     PublishRecipeRequestRequestTypeDef,
     PublishRecipeResponseTypeDef,
+    RecipeActionOutputTypeDef,
     RecipeActionTypeDef,
     ResponseMetadataTypeDef,
+    ThresholdOutputTypeDef,
     ThresholdTypeDef,
     ViewFrameTypeDef,
     SendProjectSessionActionResponseTypeDef,
     StartJobRunRequestRequestTypeDef,
     StartJobRunResponseTypeDef,
     StartProjectSessionRequestRequestTypeDef,
     StartProjectSessionResponseTypeDef,
+    StatisticOverrideOutputTypeDef,
     StatisticOverrideTypeDef,
     StopJobRunRequestRequestTypeDef,
     StopJobRunResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetResponseTypeDef,
     UpdateProfileJobResponseTypeDef,
     UpdateProjectResponseTypeDef,
     UpdateRecipeJobResponseTypeDef,
     UpdateRecipeResponseTypeDef,
     UpdateRulesetResponseTypeDef,
     UpdateScheduleRequestRequestTypeDef,
     UpdateScheduleResponseTypeDef,
+    EntityDetectorConfigurationOutputTypeDef,
     EntityDetectorConfigurationTypeDef,
     BatchDeleteRecipeVersionResponseTypeDef,
     DataCatalogInputDefinitionTypeDef,
     DatabaseInputDefinitionTypeDef,
     DatabaseTableOutputOptionsTypeDef,
     S3TableOutputOptionsTypeDef,
     CreateProjectRequestRequestTypeDef,
-    DescribeProjectResponseTypeDef,
-    ProjectTypeDef,
     UpdateProjectRequestRequestTypeDef,
+    OutputFormatOptionsOutputTypeDef,
     OutputFormatOptionsTypeDef,
+    DataCatalogInputDefinitionOutputTypeDef,
+    DatabaseInputDefinitionOutputTypeDef,
+    DatabaseTableOutputOptionsOutputTypeDef,
+    S3TableOutputOptionsOutputTypeDef,
+    DatasetParameterOutputTypeDef,
     DatasetParameterTypeDef,
+    DescribeProjectResponseTypeDef,
+    ProjectTypeDef,
+    FormatOptionsOutputTypeDef,
     FormatOptionsTypeDef,
     ListRulesetsResponseTypeDef,
     ListSchedulesResponseTypeDef,
+    RecipeStepOutputTypeDef,
     RecipeStepTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
+    StatisticsConfigurationOutputTypeDef,
     StatisticsConfigurationTypeDef,
     InputTypeDef,
     DatabaseOutputTypeDef,
     DataCatalogOutputTypeDef,
-    ListProjectsResponseTypeDef,
     OutputTypeDef,
+    InputOutputTypeDef,
+    PathOptionsOutputTypeDef,
     PathOptionsTypeDef,
-    CreateRecipeRequestRequestTypeDef,
+    ListProjectsResponseTypeDef,
     DescribeRecipeResponseTypeDef,
     RecipeTypeDef,
+    CreateRecipeRequestRequestTypeDef,
     SendProjectSessionActionRequestRequestTypeDef,
     UpdateRecipeRequestRequestTypeDef,
-    CreateRulesetRequestRequestTypeDef,
     DescribeRulesetResponseTypeDef,
+    CreateRulesetRequestRequestTypeDef,
     UpdateRulesetRequestRequestTypeDef,
+    ColumnStatisticsConfigurationOutputTypeDef,
     ColumnStatisticsConfigurationTypeDef,
     CreateRecipeJobRequestRequestTypeDef,
     JobRunTypeDef,
     JobTypeDef,
     UpdateRecipeJobRequestRequestTypeDef,
-    CreateDatasetRequestRequestTypeDef,
     DatasetTypeDef,
     DescribeDatasetResponseTypeDef,
+    CreateDatasetRequestRequestTypeDef,
     UpdateDatasetRequestRequestTypeDef,
     ListRecipeVersionsResponseTypeDef,
     ListRecipesResponseTypeDef,
+    ProfileConfigurationOutputTypeDef,
     ProfileConfigurationTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobsResponseTypeDef,
     ListDatasetsResponseTypeDef,
-    CreateProfileJobRequestRequestTypeDef,
     DescribeJobResponseTypeDef,
     DescribeJobRunResponseTypeDef,
+    CreateProfileJobRequestRequestTypeDef,
     UpdateProfileJobRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AllowedStatisticsTypeDef:
+def get_structure() -> AllowedStatisticsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-databrew-1.28.0/README.md` & `mypy-boto3-databrew-1.28.12/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-databrew"></a>
 
 # mypy-boto3-databrew
 
 [![PyPI - mypy-boto3-databrew](https://img.shields.io/pypi/v/mypy-boto3-databrew.svg?color=blue)](https://pypi.org/project/mypy-boto3-databrew)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-databrew.svg?color=blue)](https://pypi.org/project/mypy-boto3-databrew)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-databrew?color=blue)](https://pypistats.org/packages/mypy-boto3-databrew)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-databrew)](https://pepy.tech/project/mypy-boto3-databrew)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GlueDataBrew 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
+[boto3.GlueDataBrew 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
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
 [mypy-boto3-databrew docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,34 +330,42 @@
 ### Typed dictionaries
 
 `mypy_boto3_databrew.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_databrew.type_defs import (
+    AllowedStatisticsOutputTypeDef,
     AllowedStatisticsTypeDef,
     BatchDeleteRecipeVersionRequestRequestTypeDef,
     RecipeVersionErrorDetailTypeDef,
+    ColumnSelectorOutputTypeDef,
     ColumnSelectorTypeDef,
+    ConditionExpressionOutputTypeDef,
     ConditionExpressionTypeDef,
     CreateDatasetResponseTypeDef,
     JobSampleTypeDef,
     S3LocationTypeDef,
     ValidationConfigurationTypeDef,
     CreateProfileJobResponseTypeDef,
     SampleTypeDef,
     CreateProjectResponseTypeDef,
     RecipeReferenceTypeDef,
     CreateRecipeJobResponseTypeDef,
     CreateRecipeResponseTypeDef,
     CreateRulesetResponseTypeDef,
     CreateScheduleRequestRequestTypeDef,
     CreateScheduleResponseTypeDef,
+    CsvOptionsOutputTypeDef,
     CsvOptionsTypeDef,
+    CsvOutputOptionsOutputTypeDef,
     CsvOutputOptionsTypeDef,
+    S3LocationOutputTypeDef,
+    DatetimeOptionsOutputTypeDef,
+    FilterExpressionOutputTypeDef,
     DatetimeOptionsTypeDef,
     FilterExpressionTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteDatasetResponseTypeDef,
     DeleteJobRequestRequestTypeDef,
     DeleteJobResponseTypeDef,
     DeleteProjectRequestRequestTypeDef,
@@ -366,23 +374,31 @@
     DeleteRecipeVersionResponseTypeDef,
     DeleteRulesetRequestRequestTypeDef,
     DeleteRulesetResponseTypeDef,
     DeleteScheduleRequestRequestTypeDef,
     DeleteScheduleResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
+    JobSampleOutputTypeDef,
+    RecipeReferenceOutputTypeDef,
+    ValidationConfigurationOutputTypeDef,
     DescribeJobRunRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
+    SampleOutputTypeDef,
     DescribeRecipeRequestRequestTypeDef,
     DescribeRulesetRequestRequestTypeDef,
     DescribeScheduleRequestRequestTypeDef,
     DescribeScheduleResponseTypeDef,
+    ExcelOptionsOutputTypeDef,
     ExcelOptionsTypeDef,
+    FilesLimitOutputTypeDef,
     FilesLimitTypeDef,
+    JsonOptionsOutputTypeDef,
     JsonOptionsTypeDef,
+    MetadataOutputTypeDef,
     MetadataTypeDef,
     ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
@@ -399,91 +415,109 @@
     ListSchedulesRequestRequestTypeDef,
     ScheduleTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     PublishRecipeRequestRequestTypeDef,
     PublishRecipeResponseTypeDef,
+    RecipeActionOutputTypeDef,
     RecipeActionTypeDef,
     ResponseMetadataTypeDef,
+    ThresholdOutputTypeDef,
     ThresholdTypeDef,
     ViewFrameTypeDef,
     SendProjectSessionActionResponseTypeDef,
     StartJobRunRequestRequestTypeDef,
     StartJobRunResponseTypeDef,
     StartProjectSessionRequestRequestTypeDef,
     StartProjectSessionResponseTypeDef,
+    StatisticOverrideOutputTypeDef,
     StatisticOverrideTypeDef,
     StopJobRunRequestRequestTypeDef,
     StopJobRunResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetResponseTypeDef,
     UpdateProfileJobResponseTypeDef,
     UpdateProjectResponseTypeDef,
     UpdateRecipeJobResponseTypeDef,
     UpdateRecipeResponseTypeDef,
     UpdateRulesetResponseTypeDef,
     UpdateScheduleRequestRequestTypeDef,
     UpdateScheduleResponseTypeDef,
+    EntityDetectorConfigurationOutputTypeDef,
     EntityDetectorConfigurationTypeDef,
     BatchDeleteRecipeVersionResponseTypeDef,
     DataCatalogInputDefinitionTypeDef,
     DatabaseInputDefinitionTypeDef,
     DatabaseTableOutputOptionsTypeDef,
     S3TableOutputOptionsTypeDef,
     CreateProjectRequestRequestTypeDef,
-    DescribeProjectResponseTypeDef,
-    ProjectTypeDef,
     UpdateProjectRequestRequestTypeDef,
+    OutputFormatOptionsOutputTypeDef,
     OutputFormatOptionsTypeDef,
+    DataCatalogInputDefinitionOutputTypeDef,
+    DatabaseInputDefinitionOutputTypeDef,
+    DatabaseTableOutputOptionsOutputTypeDef,
+    S3TableOutputOptionsOutputTypeDef,
+    DatasetParameterOutputTypeDef,
     DatasetParameterTypeDef,
+    DescribeProjectResponseTypeDef,
+    ProjectTypeDef,
+    FormatOptionsOutputTypeDef,
     FormatOptionsTypeDef,
     ListRulesetsResponseTypeDef,
     ListSchedulesResponseTypeDef,
+    RecipeStepOutputTypeDef,
     RecipeStepTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
+    StatisticsConfigurationOutputTypeDef,
     StatisticsConfigurationTypeDef,
     InputTypeDef,
     DatabaseOutputTypeDef,
     DataCatalogOutputTypeDef,
-    ListProjectsResponseTypeDef,
     OutputTypeDef,
+    InputOutputTypeDef,
+    PathOptionsOutputTypeDef,
     PathOptionsTypeDef,
-    CreateRecipeRequestRequestTypeDef,
+    ListProjectsResponseTypeDef,
     DescribeRecipeResponseTypeDef,
     RecipeTypeDef,
+    CreateRecipeRequestRequestTypeDef,
     SendProjectSessionActionRequestRequestTypeDef,
     UpdateRecipeRequestRequestTypeDef,
-    CreateRulesetRequestRequestTypeDef,
     DescribeRulesetResponseTypeDef,
+    CreateRulesetRequestRequestTypeDef,
     UpdateRulesetRequestRequestTypeDef,
+    ColumnStatisticsConfigurationOutputTypeDef,
     ColumnStatisticsConfigurationTypeDef,
     CreateRecipeJobRequestRequestTypeDef,
     JobRunTypeDef,
     JobTypeDef,
     UpdateRecipeJobRequestRequestTypeDef,
-    CreateDatasetRequestRequestTypeDef,
     DatasetTypeDef,
     DescribeDatasetResponseTypeDef,
+    CreateDatasetRequestRequestTypeDef,
     UpdateDatasetRequestRequestTypeDef,
     ListRecipeVersionsResponseTypeDef,
     ListRecipesResponseTypeDef,
+    ProfileConfigurationOutputTypeDef,
     ProfileConfigurationTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobsResponseTypeDef,
     ListDatasetsResponseTypeDef,
-    CreateProfileJobRequestRequestTypeDef,
     DescribeJobResponseTypeDef,
     DescribeJobRunResponseTypeDef,
+    CreateProfileJobRequestRequestTypeDef,
     UpdateProfileJobRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AllowedStatisticsTypeDef:
+def get_structure() -> AllowedStatisticsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/__init__.py` & `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/__init__.pyi` & `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/__main__.py` & `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GlueDataBrew 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.GlueDataBrew 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew\nOther"
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

### Comparing `mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/client.py` & `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/client.pyi` & `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/literals.py` & `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/literals.pyi`

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
     "AnalyticsModeType",
     "CompressionFormatType",
     "DatabaseOutputModeType",
     "EncryptionModeType",
     "InputFormatType",
     "JobRunStateType",
@@ -50,15 +49,14 @@
     "GlueDataBrewServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AnalyticsModeType = Literal["DISABLE", "ENABLE"]
 CompressionFormatType = Literal[
     "BROTLI", "BZIP2", "DEFLATE", "GZIP", "LZ4", "LZO", "SNAPPY", "ZLIB", "ZSTD"
 ]
 DatabaseOutputModeType = Literal["NEW_TABLE"]
 EncryptionModeType = Literal["SSE-KMS", "SSE-S3"]
 InputFormatType = Literal["CSV", "EXCEL", "JSON", "ORC", "PARQUET"]
@@ -217,14 +215,15 @@
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
@@ -303,26 +302,28 @@
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

### Comparing `mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/literals.pyi` & `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/literals.py`

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
     "AnalyticsModeType",
     "CompressionFormatType",
     "DatabaseOutputModeType",
     "EncryptionModeType",
     "InputFormatType",
     "JobRunStateType",
@@ -49,14 +50,15 @@
     "GlueDataBrewServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AnalyticsModeType = Literal["DISABLE", "ENABLE"]
 CompressionFormatType = Literal[
     "BROTLI", "BZIP2", "DEFLATE", "GZIP", "LZ4", "LZO", "SNAPPY", "ZLIB", "ZSTD"
 ]
 DatabaseOutputModeType = Literal["NEW_TABLE"]
 EncryptionModeType = Literal["SSE-KMS", "SSE-S3"]
 InputFormatType = Literal["CSV", "EXCEL", "JSON", "ORC", "PARQUET"]
@@ -215,14 +217,15 @@
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
@@ -301,26 +304,28 @@
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

### Comparing `mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/paginator.py` & `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/paginator.pyi` & `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/type_defs.py` & `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/type_defs.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for databrew service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_databrew.type_defs import AllowedStatisticsTypeDef
+    from mypy_boto3_databrew.type_defs import AllowedStatisticsOutputTypeDef
 
-    data: AllowedStatisticsTypeDef = {...}
+    data: AllowedStatisticsOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -39,36 +39,43 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "AllowedStatisticsOutputTypeDef",
     "AllowedStatisticsTypeDef",
     "BatchDeleteRecipeVersionRequestRequestTypeDef",
     "RecipeVersionErrorDetailTypeDef",
+    "ColumnSelectorOutputTypeDef",
     "ColumnSelectorTypeDef",
+    "ConditionExpressionOutputTypeDef",
     "ConditionExpressionTypeDef",
     "CreateDatasetResponseTypeDef",
     "JobSampleTypeDef",
     "S3LocationTypeDef",
     "ValidationConfigurationTypeDef",
     "CreateProfileJobResponseTypeDef",
     "SampleTypeDef",
     "CreateProjectResponseTypeDef",
     "RecipeReferenceTypeDef",
     "CreateRecipeJobResponseTypeDef",
     "CreateRecipeResponseTypeDef",
     "CreateRulesetResponseTypeDef",
     "CreateScheduleRequestRequestTypeDef",
     "CreateScheduleResponseTypeDef",
+    "CsvOptionsOutputTypeDef",
     "CsvOptionsTypeDef",
+    "CsvOutputOptionsOutputTypeDef",
     "CsvOutputOptionsTypeDef",
+    "S3LocationOutputTypeDef",
+    "DatetimeOptionsOutputTypeDef",
+    "FilterExpressionOutputTypeDef",
     "DatetimeOptionsTypeDef",
     "FilterExpressionTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteDatasetResponseTypeDef",
     "DeleteJobRequestRequestTypeDef",
     "DeleteJobResponseTypeDef",
     "DeleteProjectRequestRequestTypeDef",
@@ -77,23 +84,31 @@
     "DeleteRecipeVersionResponseTypeDef",
     "DeleteRulesetRequestRequestTypeDef",
     "DeleteRulesetResponseTypeDef",
     "DeleteScheduleRequestRequestTypeDef",
     "DeleteScheduleResponseTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
+    "JobSampleOutputTypeDef",
+    "RecipeReferenceOutputTypeDef",
+    "ValidationConfigurationOutputTypeDef",
     "DescribeJobRunRequestRequestTypeDef",
     "DescribeProjectRequestRequestTypeDef",
+    "SampleOutputTypeDef",
     "DescribeRecipeRequestRequestTypeDef",
     "DescribeRulesetRequestRequestTypeDef",
     "DescribeScheduleRequestRequestTypeDef",
     "DescribeScheduleResponseTypeDef",
+    "ExcelOptionsOutputTypeDef",
     "ExcelOptionsTypeDef",
+    "FilesLimitOutputTypeDef",
     "FilesLimitTypeDef",
+    "JsonOptionsOutputTypeDef",
     "JsonOptionsTypeDef",
+    "MetadataOutputTypeDef",
     "MetadataTypeDef",
     "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
@@ -110,89 +125,114 @@
     "ListSchedulesRequestRequestTypeDef",
     "ScheduleTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
     "PublishRecipeRequestRequestTypeDef",
     "PublishRecipeResponseTypeDef",
+    "RecipeActionOutputTypeDef",
     "RecipeActionTypeDef",
     "ResponseMetadataTypeDef",
+    "ThresholdOutputTypeDef",
     "ThresholdTypeDef",
     "ViewFrameTypeDef",
     "SendProjectSessionActionResponseTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "StartJobRunResponseTypeDef",
     "StartProjectSessionRequestRequestTypeDef",
     "StartProjectSessionResponseTypeDef",
+    "StatisticOverrideOutputTypeDef",
     "StatisticOverrideTypeDef",
     "StopJobRunRequestRequestTypeDef",
     "StopJobRunResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasetResponseTypeDef",
     "UpdateProfileJobResponseTypeDef",
     "UpdateProjectResponseTypeDef",
     "UpdateRecipeJobResponseTypeDef",
     "UpdateRecipeResponseTypeDef",
     "UpdateRulesetResponseTypeDef",
     "UpdateScheduleRequestRequestTypeDef",
     "UpdateScheduleResponseTypeDef",
+    "EntityDetectorConfigurationOutputTypeDef",
     "EntityDetectorConfigurationTypeDef",
     "BatchDeleteRecipeVersionResponseTypeDef",
     "DataCatalogInputDefinitionTypeDef",
     "DatabaseInputDefinitionTypeDef",
     "DatabaseTableOutputOptionsTypeDef",
     "S3TableOutputOptionsTypeDef",
     "CreateProjectRequestRequestTypeDef",
-    "DescribeProjectResponseTypeDef",
-    "ProjectTypeDef",
     "UpdateProjectRequestRequestTypeDef",
+    "OutputFormatOptionsOutputTypeDef",
     "OutputFormatOptionsTypeDef",
+    "DataCatalogInputDefinitionOutputTypeDef",
+    "DatabaseInputDefinitionOutputTypeDef",
+    "DatabaseTableOutputOptionsOutputTypeDef",
+    "S3TableOutputOptionsOutputTypeDef",
+    "DatasetParameterOutputTypeDef",
     "DatasetParameterTypeDef",
+    "DescribeProjectResponseTypeDef",
+    "ProjectTypeDef",
+    "FormatOptionsOutputTypeDef",
     "FormatOptionsTypeDef",
     "ListRulesetsResponseTypeDef",
     "ListSchedulesResponseTypeDef",
+    "RecipeStepOutputTypeDef",
     "RecipeStepTypeDef",
+    "RuleOutputTypeDef",
     "RuleTypeDef",
+    "StatisticsConfigurationOutputTypeDef",
     "StatisticsConfigurationTypeDef",
     "InputTypeDef",
     "DatabaseOutputTypeDef",
     "DataCatalogOutputTypeDef",
-    "ListProjectsResponseTypeDef",
     "OutputTypeDef",
+    "InputOutputTypeDef",
+    "PathOptionsOutputTypeDef",
     "PathOptionsTypeDef",
-    "CreateRecipeRequestRequestTypeDef",
+    "ListProjectsResponseTypeDef",
     "DescribeRecipeResponseTypeDef",
     "RecipeTypeDef",
+    "CreateRecipeRequestRequestTypeDef",
     "SendProjectSessionActionRequestRequestTypeDef",
     "UpdateRecipeRequestRequestTypeDef",
-    "CreateRulesetRequestRequestTypeDef",
     "DescribeRulesetResponseTypeDef",
+    "CreateRulesetRequestRequestTypeDef",
     "UpdateRulesetRequestRequestTypeDef",
+    "ColumnStatisticsConfigurationOutputTypeDef",
     "ColumnStatisticsConfigurationTypeDef",
     "CreateRecipeJobRequestRequestTypeDef",
     "JobRunTypeDef",
     "JobTypeDef",
     "UpdateRecipeJobRequestRequestTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
     "DatasetTypeDef",
     "DescribeDatasetResponseTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
     "UpdateDatasetRequestRequestTypeDef",
     "ListRecipeVersionsResponseTypeDef",
     "ListRecipesResponseTypeDef",
+    "ProfileConfigurationOutputTypeDef",
     "ProfileConfigurationTypeDef",
     "ListJobRunsResponseTypeDef",
     "ListJobsResponseTypeDef",
     "ListDatasetsResponseTypeDef",
-    "CreateProfileJobRequestRequestTypeDef",
     "DescribeJobResponseTypeDef",
     "DescribeJobRunResponseTypeDef",
+    "CreateProfileJobRequestRequestTypeDef",
     "UpdateProfileJobRequestRequestTypeDef",
 )
 
+AllowedStatisticsOutputTypeDef = TypedDict(
+    "AllowedStatisticsOutputTypeDef",
+    {
+        "Statistics": List[str],
+    },
+)
+
 AllowedStatisticsTypeDef = TypedDict(
     "AllowedStatisticsTypeDef",
     {
         "Statistics": Sequence[str],
     },
 )
 
@@ -210,23 +250,52 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "RecipeVersion": str,
     },
     total=False,
 )
 
+ColumnSelectorOutputTypeDef = TypedDict(
+    "ColumnSelectorOutputTypeDef",
+    {
+        "Regex": str,
+        "Name": str,
+    },
+    total=False,
+)
+
 ColumnSelectorTypeDef = TypedDict(
     "ColumnSelectorTypeDef",
     {
         "Regex": str,
         "Name": str,
     },
     total=False,
 )
 
+_RequiredConditionExpressionOutputTypeDef = TypedDict(
+    "_RequiredConditionExpressionOutputTypeDef",
+    {
+        "Condition": str,
+        "TargetColumn": str,
+    },
+)
+_OptionalConditionExpressionOutputTypeDef = TypedDict(
+    "_OptionalConditionExpressionOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+class ConditionExpressionOutputTypeDef(
+    _RequiredConditionExpressionOutputTypeDef, _OptionalConditionExpressionOutputTypeDef
+):
+    pass
+
 _RequiredConditionExpressionTypeDef = TypedDict(
     "_RequiredConditionExpressionTypeDef",
     {
         "Condition": str,
         "TargetColumn": str,
     },
 )
@@ -234,21 +303,19 @@
     "_OptionalConditionExpressionTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class ConditionExpressionTypeDef(
     _RequiredConditionExpressionTypeDef, _OptionalConditionExpressionTypeDef
 ):
     pass
 
-
 CreateDatasetResponseTypeDef = TypedDict(
     "CreateDatasetResponseTypeDef",
     {
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -273,40 +340,36 @@
     {
         "Key": str,
         "BucketOwner": str,
     },
     total=False,
 )
 
-
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
-
 _RequiredValidationConfigurationTypeDef = TypedDict(
     "_RequiredValidationConfigurationTypeDef",
     {
         "RulesetArn": str,
     },
 )
 _OptionalValidationConfigurationTypeDef = TypedDict(
     "_OptionalValidationConfigurationTypeDef",
     {
         "ValidationMode": Literal["CHECK_ALL"],
     },
     total=False,
 )
 
-
 class ValidationConfigurationTypeDef(
     _RequiredValidationConfigurationTypeDef, _OptionalValidationConfigurationTypeDef
 ):
     pass
 
-
 CreateProfileJobResponseTypeDef = TypedDict(
     "CreateProfileJobResponseTypeDef",
     {
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -321,19 +384,17 @@
     "_OptionalSampleTypeDef",
     {
         "Size": int,
     },
     total=False,
 )
 
-
 class SampleTypeDef(_RequiredSampleTypeDef, _OptionalSampleTypeDef):
     pass
 
-
 CreateProjectResponseTypeDef = TypedDict(
     "CreateProjectResponseTypeDef",
     {
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -348,19 +409,17 @@
     "_OptionalRecipeReferenceTypeDef",
     {
         "RecipeVersion": str,
     },
     total=False,
 )
 
-
 class RecipeReferenceTypeDef(_RequiredRecipeReferenceTypeDef, _OptionalRecipeReferenceTypeDef):
     pass
 
-
 CreateRecipeJobResponseTypeDef = TypedDict(
     "CreateRecipeJobResponseTypeDef",
     {
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -393,46 +452,107 @@
     {
         "JobNames": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateScheduleRequestRequestTypeDef(
     _RequiredCreateScheduleRequestRequestTypeDef, _OptionalCreateScheduleRequestRequestTypeDef
 ):
     pass
 
-
 CreateScheduleResponseTypeDef = TypedDict(
     "CreateScheduleResponseTypeDef",
     {
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CsvOptionsOutputTypeDef = TypedDict(
+    "CsvOptionsOutputTypeDef",
+    {
+        "Delimiter": str,
+        "HeaderRow": bool,
+    },
+    total=False,
+)
+
 CsvOptionsTypeDef = TypedDict(
     "CsvOptionsTypeDef",
     {
         "Delimiter": str,
         "HeaderRow": bool,
     },
     total=False,
 )
 
+CsvOutputOptionsOutputTypeDef = TypedDict(
+    "CsvOutputOptionsOutputTypeDef",
+    {
+        "Delimiter": str,
+    },
+    total=False,
+)
+
 CsvOutputOptionsTypeDef = TypedDict(
     "CsvOutputOptionsTypeDef",
     {
         "Delimiter": str,
     },
     total=False,
 )
 
+_RequiredS3LocationOutputTypeDef = TypedDict(
+    "_RequiredS3LocationOutputTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalS3LocationOutputTypeDef = TypedDict(
+    "_OptionalS3LocationOutputTypeDef",
+    {
+        "Key": str,
+        "BucketOwner": str,
+    },
+    total=False,
+)
+
+class S3LocationOutputTypeDef(_RequiredS3LocationOutputTypeDef, _OptionalS3LocationOutputTypeDef):
+    pass
+
+_RequiredDatetimeOptionsOutputTypeDef = TypedDict(
+    "_RequiredDatetimeOptionsOutputTypeDef",
+    {
+        "Format": str,
+    },
+)
+_OptionalDatetimeOptionsOutputTypeDef = TypedDict(
+    "_OptionalDatetimeOptionsOutputTypeDef",
+    {
+        "TimezoneOffset": str,
+        "LocaleCode": str,
+    },
+    total=False,
+)
+
+class DatetimeOptionsOutputTypeDef(
+    _RequiredDatetimeOptionsOutputTypeDef, _OptionalDatetimeOptionsOutputTypeDef
+):
+    pass
+
+FilterExpressionOutputTypeDef = TypedDict(
+    "FilterExpressionOutputTypeDef",
+    {
+        "Expression": str,
+        "ValuesMap": Dict[str, str],
+    },
+)
+
 _RequiredDatetimeOptionsTypeDef = TypedDict(
     "_RequiredDatetimeOptionsTypeDef",
     {
         "Format": str,
     },
 )
 _OptionalDatetimeOptionsTypeDef = TypedDict(
@@ -440,19 +560,17 @@
     {
         "TimezoneOffset": str,
         "LocaleCode": str,
     },
     total=False,
 )
 
-
 class DatetimeOptionsTypeDef(_RequiredDatetimeOptionsTypeDef, _OptionalDatetimeOptionsTypeDef):
     pass
 
-
 FilterExpressionTypeDef = TypedDict(
     "FilterExpressionTypeDef",
     {
         "Expression": str,
         "ValuesMap": Mapping[str, str],
     },
 )
@@ -559,14 +677,61 @@
 DescribeJobRequestRequestTypeDef = TypedDict(
     "DescribeJobRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+JobSampleOutputTypeDef = TypedDict(
+    "JobSampleOutputTypeDef",
+    {
+        "Mode": SampleModeType,
+        "Size": int,
+    },
+    total=False,
+)
+
+_RequiredRecipeReferenceOutputTypeDef = TypedDict(
+    "_RequiredRecipeReferenceOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalRecipeReferenceOutputTypeDef = TypedDict(
+    "_OptionalRecipeReferenceOutputTypeDef",
+    {
+        "RecipeVersion": str,
+    },
+    total=False,
+)
+
+class RecipeReferenceOutputTypeDef(
+    _RequiredRecipeReferenceOutputTypeDef, _OptionalRecipeReferenceOutputTypeDef
+):
+    pass
+
+_RequiredValidationConfigurationOutputTypeDef = TypedDict(
+    "_RequiredValidationConfigurationOutputTypeDef",
+    {
+        "RulesetArn": str,
+    },
+)
+_OptionalValidationConfigurationOutputTypeDef = TypedDict(
+    "_OptionalValidationConfigurationOutputTypeDef",
+    {
+        "ValidationMode": Literal["CHECK_ALL"],
+    },
+    total=False,
+)
+
+class ValidationConfigurationOutputTypeDef(
+    _RequiredValidationConfigurationOutputTypeDef, _OptionalValidationConfigurationOutputTypeDef
+):
+    pass
+
 DescribeJobRunRequestRequestTypeDef = TypedDict(
     "DescribeJobRunRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
@@ -574,35 +739,50 @@
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+_RequiredSampleOutputTypeDef = TypedDict(
+    "_RequiredSampleOutputTypeDef",
+    {
+        "Type": SampleTypeType,
+    },
+)
+_OptionalSampleOutputTypeDef = TypedDict(
+    "_OptionalSampleOutputTypeDef",
+    {
+        "Size": int,
+    },
+    total=False,
+)
+
+class SampleOutputTypeDef(_RequiredSampleOutputTypeDef, _OptionalSampleOutputTypeDef):
+    pass
+
 _RequiredDescribeRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRecipeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDescribeRecipeRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeRecipeRequestRequestTypeDef",
     {
         "RecipeVersion": str,
     },
     total=False,
 )
 
-
 class DescribeRecipeRequestRequestTypeDef(
     _RequiredDescribeRecipeRequestRequestTypeDef, _OptionalDescribeRecipeRequestRequestTypeDef
 ):
     pass
 
-
 DescribeRulesetRequestRequestTypeDef = TypedDict(
     "DescribeRulesetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -625,24 +805,52 @@
         "CronExpression": str,
         "Tags": Dict[str, str],
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ExcelOptionsOutputTypeDef = TypedDict(
+    "ExcelOptionsOutputTypeDef",
+    {
+        "SheetNames": List[str],
+        "SheetIndexes": List[int],
+        "HeaderRow": bool,
+    },
+    total=False,
+)
+
 ExcelOptionsTypeDef = TypedDict(
     "ExcelOptionsTypeDef",
     {
         "SheetNames": Sequence[str],
         "SheetIndexes": Sequence[int],
         "HeaderRow": bool,
     },
     total=False,
 )
 
+_RequiredFilesLimitOutputTypeDef = TypedDict(
+    "_RequiredFilesLimitOutputTypeDef",
+    {
+        "MaxFiles": int,
+    },
+)
+_OptionalFilesLimitOutputTypeDef = TypedDict(
+    "_OptionalFilesLimitOutputTypeDef",
+    {
+        "OrderedBy": Literal["LAST_MODIFIED_DATE"],
+        "Order": OrderType,
+    },
+    total=False,
+)
+
+class FilesLimitOutputTypeDef(_RequiredFilesLimitOutputTypeDef, _OptionalFilesLimitOutputTypeDef):
+    pass
+
 _RequiredFilesLimitTypeDef = TypedDict(
     "_RequiredFilesLimitTypeDef",
     {
         "MaxFiles": int,
     },
 )
 _OptionalFilesLimitTypeDef = TypedDict(
@@ -650,27 +858,41 @@
     {
         "OrderedBy": Literal["LAST_MODIFIED_DATE"],
         "Order": OrderType,
     },
     total=False,
 )
 
-
 class FilesLimitTypeDef(_RequiredFilesLimitTypeDef, _OptionalFilesLimitTypeDef):
     pass
 
+JsonOptionsOutputTypeDef = TypedDict(
+    "JsonOptionsOutputTypeDef",
+    {
+        "MultiLine": bool,
+    },
+    total=False,
+)
 
 JsonOptionsTypeDef = TypedDict(
     "JsonOptionsTypeDef",
     {
         "MultiLine": bool,
     },
     total=False,
 )
 
+MetadataOutputTypeDef = TypedDict(
+    "MetadataOutputTypeDef",
+    {
+        "SourceArn": str,
+    },
+    total=False,
+)
+
 MetadataTypeDef = TypedDict(
     "MetadataTypeDef",
     {
         "SourceArn": str,
     },
     total=False,
 )
@@ -702,22 +924,20 @@
     "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListJobRunsRequestListJobRunsPaginateTypeDef(
     _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
     _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobRunsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -725,21 +945,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
-
 ListJobsRequestListJobsPaginateTypeDef = TypedDict(
     "ListJobsRequestListJobsPaginateTypeDef",
     {
         "DatasetName": str,
         "ProjectName": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -784,22 +1002,20 @@
     "_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef(
     _RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
     _OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListRecipeVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListRecipeVersionsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListRecipeVersionsRequestRequestTypeDef = TypedDict(
@@ -807,22 +1023,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListRecipeVersionsRequestRequestTypeDef(
     _RequiredListRecipeVersionsRequestRequestTypeDef,
     _OptionalListRecipeVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListRecipesRequestListRecipesPaginateTypeDef = TypedDict(
     "ListRecipesRequestListRecipesPaginateTypeDef",
     {
         "RecipeVersion": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -876,19 +1090,17 @@
         "ResourceArn": str,
         "RuleCount": int,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class RulesetItemTypeDef(_RequiredRulesetItemTypeDef, _OptionalRulesetItemTypeDef):
     pass
 
-
 ListSchedulesRequestListSchedulesPaginateTypeDef = TypedDict(
     "ListSchedulesRequestListSchedulesPaginateTypeDef",
     {
         "JobName": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -922,19 +1134,17 @@
         "ResourceArn": str,
         "CronExpression": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class ScheduleTypeDef(_RequiredScheduleTypeDef, _OptionalScheduleTypeDef):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -966,59 +1176,92 @@
     "_OptionalPublishRecipeRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class PublishRecipeRequestRequestTypeDef(
     _RequiredPublishRecipeRequestRequestTypeDef, _OptionalPublishRecipeRequestRequestTypeDef
 ):
     pass
 
-
 PublishRecipeResponseTypeDef = TypedDict(
     "PublishRecipeResponseTypeDef",
     {
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredRecipeActionOutputTypeDef = TypedDict(
+    "_RequiredRecipeActionOutputTypeDef",
+    {
+        "Operation": str,
+    },
+)
+_OptionalRecipeActionOutputTypeDef = TypedDict(
+    "_OptionalRecipeActionOutputTypeDef",
+    {
+        "Parameters": Dict[str, str],
+    },
+    total=False,
+)
+
+class RecipeActionOutputTypeDef(
+    _RequiredRecipeActionOutputTypeDef, _OptionalRecipeActionOutputTypeDef
+):
+    pass
+
 _RequiredRecipeActionTypeDef = TypedDict(
     "_RequiredRecipeActionTypeDef",
     {
         "Operation": str,
     },
 )
 _OptionalRecipeActionTypeDef = TypedDict(
     "_OptionalRecipeActionTypeDef",
     {
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
-
 class RecipeActionTypeDef(_RequiredRecipeActionTypeDef, _OptionalRecipeActionTypeDef):
     pass
 
-
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
 
+_RequiredThresholdOutputTypeDef = TypedDict(
+    "_RequiredThresholdOutputTypeDef",
+    {
+        "Value": float,
+    },
+)
+_OptionalThresholdOutputTypeDef = TypedDict(
+    "_OptionalThresholdOutputTypeDef",
+    {
+        "Type": ThresholdTypeType,
+        "Unit": ThresholdUnitType,
+    },
+    total=False,
+)
+
+class ThresholdOutputTypeDef(_RequiredThresholdOutputTypeDef, _OptionalThresholdOutputTypeDef):
+    pass
+
 _RequiredThresholdTypeDef = TypedDict(
     "_RequiredThresholdTypeDef",
     {
         "Value": float,
     },
 )
 _OptionalThresholdTypeDef = TypedDict(
@@ -1026,19 +1269,17 @@
     {
         "Type": ThresholdTypeType,
         "Unit": ThresholdUnitType,
     },
     total=False,
 )
 
-
 class ThresholdTypeDef(_RequiredThresholdTypeDef, _OptionalThresholdTypeDef):
     pass
 
-
 _RequiredViewFrameTypeDef = TypedDict(
     "_RequiredViewFrameTypeDef",
     {
         "StartColumnIndex": int,
     },
 )
 _OptionalViewFrameTypeDef = TypedDict(
@@ -1049,19 +1290,17 @@
         "StartRowIndex": int,
         "RowRange": int,
         "Analytics": AnalyticsModeType,
     },
     total=False,
 )
 
-
 class ViewFrameTypeDef(_RequiredViewFrameTypeDef, _OptionalViewFrameTypeDef):
     pass
 
-
 SendProjectSessionActionResponseTypeDef = TypedDict(
     "SendProjectSessionActionResponseTypeDef",
     {
         "Result": str,
         "Name": str,
         "ActionId": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1093,31 +1332,37 @@
     "_OptionalStartProjectSessionRequestRequestTypeDef",
     {
         "AssumeControl": bool,
     },
     total=False,
 )
 
-
 class StartProjectSessionRequestRequestTypeDef(
     _RequiredStartProjectSessionRequestRequestTypeDef,
     _OptionalStartProjectSessionRequestRequestTypeDef,
 ):
     pass
 
-
 StartProjectSessionResponseTypeDef = TypedDict(
     "StartProjectSessionResponseTypeDef",
     {
         "Name": str,
         "ClientSessionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+StatisticOverrideOutputTypeDef = TypedDict(
+    "StatisticOverrideOutputTypeDef",
+    {
+        "Statistic": str,
+        "Parameters": Dict[str, str],
+    },
+)
+
 StatisticOverrideTypeDef = TypedDict(
     "StatisticOverrideTypeDef",
     {
         "Statistic": str,
         "Parameters": Mapping[str, str],
     },
 )
@@ -1214,50 +1459,66 @@
     "_OptionalUpdateScheduleRequestRequestTypeDef",
     {
         "JobNames": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateScheduleRequestRequestTypeDef(
     _RequiredUpdateScheduleRequestRequestTypeDef, _OptionalUpdateScheduleRequestRequestTypeDef
 ):
     pass
 
-
 UpdateScheduleResponseTypeDef = TypedDict(
     "UpdateScheduleResponseTypeDef",
     {
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredEntityDetectorConfigurationOutputTypeDef = TypedDict(
+    "_RequiredEntityDetectorConfigurationOutputTypeDef",
+    {
+        "EntityTypes": List[str],
+    },
+)
+_OptionalEntityDetectorConfigurationOutputTypeDef = TypedDict(
+    "_OptionalEntityDetectorConfigurationOutputTypeDef",
+    {
+        "AllowedStatistics": List[AllowedStatisticsOutputTypeDef],
+    },
+    total=False,
+)
+
+class EntityDetectorConfigurationOutputTypeDef(
+    _RequiredEntityDetectorConfigurationOutputTypeDef,
+    _OptionalEntityDetectorConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredEntityDetectorConfigurationTypeDef = TypedDict(
     "_RequiredEntityDetectorConfigurationTypeDef",
     {
         "EntityTypes": Sequence[str],
     },
 )
 _OptionalEntityDetectorConfigurationTypeDef = TypedDict(
     "_OptionalEntityDetectorConfigurationTypeDef",
     {
         "AllowedStatistics": Sequence[AllowedStatisticsTypeDef],
     },
     total=False,
 )
 
-
 class EntityDetectorConfigurationTypeDef(
     _RequiredEntityDetectorConfigurationTypeDef, _OptionalEntityDetectorConfigurationTypeDef
 ):
     pass
 
-
 BatchDeleteRecipeVersionResponseTypeDef = TypedDict(
     "BatchDeleteRecipeVersionResponseTypeDef",
     {
         "Name": str,
         "Errors": List[RecipeVersionErrorDetailTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1275,21 +1536,19 @@
     {
         "CatalogId": str,
         "TempDirectory": S3LocationTypeDef,
     },
     total=False,
 )
 
-
 class DataCatalogInputDefinitionTypeDef(
     _RequiredDataCatalogInputDefinitionTypeDef, _OptionalDataCatalogInputDefinitionTypeDef
 ):
     pass
 
-
 _RequiredDatabaseInputDefinitionTypeDef = TypedDict(
     "_RequiredDatabaseInputDefinitionTypeDef",
     {
         "GlueConnectionName": str,
     },
 )
 _OptionalDatabaseInputDefinitionTypeDef = TypedDict(
@@ -1298,42 +1557,38 @@
         "DatabaseTableName": str,
         "TempDirectory": S3LocationTypeDef,
         "QueryString": str,
     },
     total=False,
 )
 
-
 class DatabaseInputDefinitionTypeDef(
     _RequiredDatabaseInputDefinitionTypeDef, _OptionalDatabaseInputDefinitionTypeDef
 ):
     pass
 
-
 _RequiredDatabaseTableOutputOptionsTypeDef = TypedDict(
     "_RequiredDatabaseTableOutputOptionsTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalDatabaseTableOutputOptionsTypeDef = TypedDict(
     "_OptionalDatabaseTableOutputOptionsTypeDef",
     {
         "TempDirectory": S3LocationTypeDef,
     },
     total=False,
 )
 
-
 class DatabaseTableOutputOptionsTypeDef(
     _RequiredDatabaseTableOutputOptionsTypeDef, _OptionalDatabaseTableOutputOptionsTypeDef
 ):
     pass
 
-
 S3TableOutputOptionsTypeDef = TypedDict(
     "S3TableOutputOptionsTypeDef",
     {
         "Location": S3LocationTypeDef,
     },
 )
 
@@ -1351,103 +1606,147 @@
     {
         "Sample": SampleTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
-
-DescribeProjectResponseTypeDef = TypedDict(
-    "DescribeProjectResponseTypeDef",
+_RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateProjectRequestRequestTypeDef",
     {
-        "CreateDate": datetime,
-        "CreatedBy": str,
-        "DatasetName": str,
-        "LastModifiedDate": datetime,
-        "LastModifiedBy": str,
+        "RoleArn": str,
         "Name": str,
-        "RecipeName": str,
-        "ResourceArn": str,
+    },
+)
+_OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateProjectRequestRequestTypeDef",
+    {
         "Sample": SampleTypeDef,
-        "RoleArn": str,
-        "Tags": Dict[str, str],
-        "SessionStatus": SessionStatusType,
-        "OpenedBy": str,
-        "OpenDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-_RequiredProjectTypeDef = TypedDict(
-    "_RequiredProjectTypeDef",
+class UpdateProjectRequestRequestTypeDef(
+    _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
+):
+    pass
+
+OutputFormatOptionsOutputTypeDef = TypedDict(
+    "OutputFormatOptionsOutputTypeDef",
     {
-        "Name": str,
-        "RecipeName": str,
+        "Csv": CsvOutputOptionsOutputTypeDef,
     },
+    total=False,
 )
-_OptionalProjectTypeDef = TypedDict(
-    "_OptionalProjectTypeDef",
+
+OutputFormatOptionsTypeDef = TypedDict(
+    "OutputFormatOptionsTypeDef",
     {
-        "AccountId": str,
-        "CreateDate": datetime,
-        "CreatedBy": str,
-        "DatasetName": str,
-        "LastModifiedDate": datetime,
-        "LastModifiedBy": str,
-        "ResourceArn": str,
-        "Sample": SampleTypeDef,
-        "Tags": Dict[str, str],
-        "RoleArn": str,
-        "OpenedBy": str,
-        "OpenDate": datetime,
+        "Csv": CsvOutputOptionsTypeDef,
     },
     total=False,
 )
 
+_RequiredDataCatalogInputDefinitionOutputTypeDef = TypedDict(
+    "_RequiredDataCatalogInputDefinitionOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+    },
+)
+_OptionalDataCatalogInputDefinitionOutputTypeDef = TypedDict(
+    "_OptionalDataCatalogInputDefinitionOutputTypeDef",
+    {
+        "CatalogId": str,
+        "TempDirectory": S3LocationOutputTypeDef,
+    },
+    total=False,
+)
 
-class ProjectTypeDef(_RequiredProjectTypeDef, _OptionalProjectTypeDef):
+class DataCatalogInputDefinitionOutputTypeDef(
+    _RequiredDataCatalogInputDefinitionOutputTypeDef,
+    _OptionalDataCatalogInputDefinitionOutputTypeDef,
+):
     pass
 
-
-_RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateProjectRequestRequestTypeDef",
+_RequiredDatabaseInputDefinitionOutputTypeDef = TypedDict(
+    "_RequiredDatabaseInputDefinitionOutputTypeDef",
     {
-        "RoleArn": str,
-        "Name": str,
+        "GlueConnectionName": str,
     },
 )
-_OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateProjectRequestRequestTypeDef",
+_OptionalDatabaseInputDefinitionOutputTypeDef = TypedDict(
+    "_OptionalDatabaseInputDefinitionOutputTypeDef",
     {
-        "Sample": SampleTypeDef,
+        "DatabaseTableName": str,
+        "TempDirectory": S3LocationOutputTypeDef,
+        "QueryString": str,
     },
     total=False,
 )
 
+class DatabaseInputDefinitionOutputTypeDef(
+    _RequiredDatabaseInputDefinitionOutputTypeDef, _OptionalDatabaseInputDefinitionOutputTypeDef
+):
+    pass
 
-class UpdateProjectRequestRequestTypeDef(
-    _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
+_RequiredDatabaseTableOutputOptionsOutputTypeDef = TypedDict(
+    "_RequiredDatabaseTableOutputOptionsOutputTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalDatabaseTableOutputOptionsOutputTypeDef = TypedDict(
+    "_OptionalDatabaseTableOutputOptionsOutputTypeDef",
+    {
+        "TempDirectory": S3LocationOutputTypeDef,
+    },
+    total=False,
+)
+
+class DatabaseTableOutputOptionsOutputTypeDef(
+    _RequiredDatabaseTableOutputOptionsOutputTypeDef,
+    _OptionalDatabaseTableOutputOptionsOutputTypeDef,
 ):
     pass
 
+S3TableOutputOptionsOutputTypeDef = TypedDict(
+    "S3TableOutputOptionsOutputTypeDef",
+    {
+        "Location": S3LocationOutputTypeDef,
+    },
+)
 
-OutputFormatOptionsTypeDef = TypedDict(
-    "OutputFormatOptionsTypeDef",
+_RequiredDatasetParameterOutputTypeDef = TypedDict(
+    "_RequiredDatasetParameterOutputTypeDef",
     {
-        "Csv": CsvOutputOptionsTypeDef,
+        "Name": str,
+        "Type": ParameterTypeType,
+    },
+)
+_OptionalDatasetParameterOutputTypeDef = TypedDict(
+    "_OptionalDatasetParameterOutputTypeDef",
+    {
+        "DatetimeOptions": DatetimeOptionsOutputTypeDef,
+        "CreateColumn": bool,
+        "Filter": FilterExpressionOutputTypeDef,
     },
     total=False,
 )
 
+class DatasetParameterOutputTypeDef(
+    _RequiredDatasetParameterOutputTypeDef, _OptionalDatasetParameterOutputTypeDef
+):
+    pass
+
 _RequiredDatasetParameterTypeDef = TypedDict(
     "_RequiredDatasetParameterTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
     },
 )
@@ -1457,18 +1756,76 @@
         "DatetimeOptions": DatetimeOptionsTypeDef,
         "CreateColumn": bool,
         "Filter": FilterExpressionTypeDef,
     },
     total=False,
 )
 
-
 class DatasetParameterTypeDef(_RequiredDatasetParameterTypeDef, _OptionalDatasetParameterTypeDef):
     pass
 
+DescribeProjectResponseTypeDef = TypedDict(
+    "DescribeProjectResponseTypeDef",
+    {
+        "CreateDate": datetime,
+        "CreatedBy": str,
+        "DatasetName": str,
+        "LastModifiedDate": datetime,
+        "LastModifiedBy": str,
+        "Name": str,
+        "RecipeName": str,
+        "ResourceArn": str,
+        "Sample": SampleOutputTypeDef,
+        "RoleArn": str,
+        "Tags": Dict[str, str],
+        "SessionStatus": SessionStatusType,
+        "OpenedBy": str,
+        "OpenDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredProjectTypeDef = TypedDict(
+    "_RequiredProjectTypeDef",
+    {
+        "Name": str,
+        "RecipeName": str,
+    },
+)
+_OptionalProjectTypeDef = TypedDict(
+    "_OptionalProjectTypeDef",
+    {
+        "AccountId": str,
+        "CreateDate": datetime,
+        "CreatedBy": str,
+        "DatasetName": str,
+        "LastModifiedDate": datetime,
+        "LastModifiedBy": str,
+        "ResourceArn": str,
+        "Sample": SampleOutputTypeDef,
+        "Tags": Dict[str, str],
+        "RoleArn": str,
+        "OpenedBy": str,
+        "OpenDate": datetime,
+    },
+    total=False,
+)
+
+class ProjectTypeDef(_RequiredProjectTypeDef, _OptionalProjectTypeDef):
+    pass
+
+FormatOptionsOutputTypeDef = TypedDict(
+    "FormatOptionsOutputTypeDef",
+    {
+        "Json": JsonOptionsOutputTypeDef,
+        "Excel": ExcelOptionsOutputTypeDef,
+        "Csv": CsvOptionsOutputTypeDef,
+    },
+    total=False,
+)
 
 FormatOptionsTypeDef = TypedDict(
     "FormatOptionsTypeDef",
     {
         "Json": JsonOptionsTypeDef,
         "Excel": ExcelOptionsTypeDef,
         "Csv": CsvOptionsTypeDef,
@@ -1490,32 +1847,68 @@
     {
         "Schedules": List[ScheduleTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredRecipeStepOutputTypeDef = TypedDict(
+    "_RequiredRecipeStepOutputTypeDef",
+    {
+        "Action": RecipeActionOutputTypeDef,
+    },
+)
+_OptionalRecipeStepOutputTypeDef = TypedDict(
+    "_OptionalRecipeStepOutputTypeDef",
+    {
+        "ConditionExpressions": List[ConditionExpressionOutputTypeDef],
+    },
+    total=False,
+)
+
+class RecipeStepOutputTypeDef(_RequiredRecipeStepOutputTypeDef, _OptionalRecipeStepOutputTypeDef):
+    pass
+
 _RequiredRecipeStepTypeDef = TypedDict(
     "_RequiredRecipeStepTypeDef",
     {
         "Action": RecipeActionTypeDef,
     },
 )
 _OptionalRecipeStepTypeDef = TypedDict(
     "_OptionalRecipeStepTypeDef",
     {
         "ConditionExpressions": Sequence[ConditionExpressionTypeDef],
     },
     total=False,
 )
 
-
 class RecipeStepTypeDef(_RequiredRecipeStepTypeDef, _OptionalRecipeStepTypeDef):
     pass
 
+_RequiredRuleOutputTypeDef = TypedDict(
+    "_RequiredRuleOutputTypeDef",
+    {
+        "Name": str,
+        "CheckExpression": str,
+    },
+)
+_OptionalRuleOutputTypeDef = TypedDict(
+    "_OptionalRuleOutputTypeDef",
+    {
+        "Disabled": bool,
+        "SubstitutionMap": Dict[str, str],
+        "Threshold": ThresholdOutputTypeDef,
+        "ColumnSelectors": List[ColumnSelectorOutputTypeDef],
+    },
+    total=False,
+)
+
+class RuleOutputTypeDef(_RequiredRuleOutputTypeDef, _OptionalRuleOutputTypeDef):
+    pass
 
 _RequiredRuleTypeDef = TypedDict(
     "_RequiredRuleTypeDef",
     {
         "Name": str,
         "CheckExpression": str,
     },
@@ -1527,18 +1920,25 @@
         "SubstitutionMap": Mapping[str, str],
         "Threshold": ThresholdTypeDef,
         "ColumnSelectors": Sequence[ColumnSelectorTypeDef],
     },
     total=False,
 )
 
-
 class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
+StatisticsConfigurationOutputTypeDef = TypedDict(
+    "StatisticsConfigurationOutputTypeDef",
+    {
+        "IncludedStatistics": List[str],
+        "Overrides": List[StatisticOverrideOutputTypeDef],
+    },
+    total=False,
+)
 
 StatisticsConfigurationTypeDef = TypedDict(
     "StatisticsConfigurationTypeDef",
     {
         "IncludedStatistics": Sequence[str],
         "Overrides": Sequence[StatisticOverrideTypeDef],
     },
@@ -1567,19 +1967,17 @@
     "_OptionalDatabaseOutputTypeDef",
     {
         "DatabaseOutputMode": Literal["NEW_TABLE"],
     },
     total=False,
 )
 
-
 class DatabaseOutputTypeDef(_RequiredDatabaseOutputTypeDef, _OptionalDatabaseOutputTypeDef):
     pass
 
-
 _RequiredDataCatalogOutputTypeDef = TypedDict(
     "_RequiredDataCatalogOutputTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -1590,30 +1988,19 @@
         "S3Options": S3TableOutputOptionsTypeDef,
         "DatabaseOptions": DatabaseTableOutputOptionsTypeDef,
         "Overwrite": bool,
     },
     total=False,
 )
 
-
 class DataCatalogOutputTypeDef(
     _RequiredDataCatalogOutputTypeDef, _OptionalDataCatalogOutputTypeDef
 ):
     pass
 
-
-ListProjectsResponseTypeDef = TypedDict(
-    "ListProjectsResponseTypeDef",
-    {
-        "Projects": List[ProjectTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredOutputTypeDef = TypedDict(
     "_RequiredOutputTypeDef",
     {
         "Location": S3LocationTypeDef,
     },
 )
 _OptionalOutputTypeDef = TypedDict(
@@ -1625,65 +2012,70 @@
         "Overwrite": bool,
         "FormatOptions": OutputFormatOptionsTypeDef,
         "MaxOutputFiles": int,
     },
     total=False,
 )
 
-
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
 
+InputOutputTypeDef = TypedDict(
+    "InputOutputTypeDef",
+    {
+        "S3InputDefinition": S3LocationOutputTypeDef,
+        "DataCatalogInputDefinition": DataCatalogInputDefinitionOutputTypeDef,
+        "DatabaseInputDefinition": DatabaseInputDefinitionOutputTypeDef,
+        "Metadata": MetadataOutputTypeDef,
+    },
+    total=False,
+)
+
+PathOptionsOutputTypeDef = TypedDict(
+    "PathOptionsOutputTypeDef",
+    {
+        "LastModifiedDateCondition": FilterExpressionOutputTypeDef,
+        "FilesLimit": FilesLimitOutputTypeDef,
+        "Parameters": Dict[str, DatasetParameterOutputTypeDef],
+    },
+    total=False,
+)
 
 PathOptionsTypeDef = TypedDict(
     "PathOptionsTypeDef",
     {
         "LastModifiedDateCondition": FilterExpressionTypeDef,
         "FilesLimit": FilesLimitTypeDef,
         "Parameters": Mapping[str, DatasetParameterTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateRecipeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRecipeRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Steps": Sequence[RecipeStepTypeDef],
-    },
-)
-_OptionalCreateRecipeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRecipeRequestRequestTypeDef",
+ListProjectsResponseTypeDef = TypedDict(
+    "ListProjectsResponseTypeDef",
     {
-        "Description": str,
-        "Tags": Mapping[str, str],
+        "Projects": List[ProjectTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class CreateRecipeRequestRequestTypeDef(
-    _RequiredCreateRecipeRequestRequestTypeDef, _OptionalCreateRecipeRequestRequestTypeDef
-):
-    pass
-
-
 DescribeRecipeResponseTypeDef = TypedDict(
     "DescribeRecipeResponseTypeDef",
     {
         "CreatedBy": str,
         "CreateDate": datetime,
         "LastModifiedBy": str,
         "LastModifiedDate": datetime,
         "ProjectName": str,
         "PublishedBy": str,
         "PublishedDate": datetime,
         "Description": str,
         "Name": str,
-        "Steps": List[RecipeStepTypeDef],
+        "Steps": List[RecipeStepOutputTypeDef],
         "Tags": Dict[str, str],
         "ResourceArn": str,
         "RecipeVersion": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1701,25 +2093,44 @@
         "LastModifiedBy": str,
         "LastModifiedDate": datetime,
         "ProjectName": str,
         "PublishedBy": str,
         "PublishedDate": datetime,
         "Description": str,
         "ResourceArn": str,
-        "Steps": List[RecipeStepTypeDef],
+        "Steps": List[RecipeStepOutputTypeDef],
         "Tags": Dict[str, str],
         "RecipeVersion": str,
     },
     total=False,
 )
 
-
 class RecipeTypeDef(_RequiredRecipeTypeDef, _OptionalRecipeTypeDef):
     pass
 
+_RequiredCreateRecipeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRecipeRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Steps": Sequence[RecipeStepTypeDef],
+    },
+)
+_OptionalCreateRecipeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRecipeRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateRecipeRequestRequestTypeDef(
+    _RequiredCreateRecipeRequestRequestTypeDef, _OptionalCreateRecipeRequestRequestTypeDef
+):
+    pass
 
 _RequiredSendProjectSessionActionRequestRequestTypeDef = TypedDict(
     "_RequiredSendProjectSessionActionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
@@ -1731,22 +2142,20 @@
         "StepIndex": int,
         "ClientSessionId": str,
         "ViewFrame": ViewFrameTypeDef,
     },
     total=False,
 )
 
-
 class SendProjectSessionActionRequestRequestTypeDef(
     _RequiredSendProjectSessionActionRequestRequestTypeDef,
     _OptionalSendProjectSessionActionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRecipeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateRecipeRequestRequestTypeDef = TypedDict(
@@ -1754,20 +2163,35 @@
     {
         "Description": str,
         "Steps": Sequence[RecipeStepTypeDef],
     },
     total=False,
 )
 
-
 class UpdateRecipeRequestRequestTypeDef(
     _RequiredUpdateRecipeRequestRequestTypeDef, _OptionalUpdateRecipeRequestRequestTypeDef
 ):
     pass
 
+DescribeRulesetResponseTypeDef = TypedDict(
+    "DescribeRulesetResponseTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "TargetArn": str,
+        "Rules": List[RuleOutputTypeDef],
+        "CreateDate": datetime,
+        "CreatedBy": str,
+        "LastModifiedBy": str,
+        "LastModifiedDate": datetime,
+        "ResourceArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredCreateRulesetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRulesetRequestRequestTypeDef",
     {
         "Name": str,
         "TargetArn": str,
         "Rules": Sequence[RuleTypeDef],
@@ -1778,38 +2202,19 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateRulesetRequestRequestTypeDef(
     _RequiredCreateRulesetRequestRequestTypeDef, _OptionalCreateRulesetRequestRequestTypeDef
 ):
     pass
 
-
-DescribeRulesetResponseTypeDef = TypedDict(
-    "DescribeRulesetResponseTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "TargetArn": str,
-        "Rules": List[RuleTypeDef],
-        "CreateDate": datetime,
-        "CreatedBy": str,
-        "LastModifiedBy": str,
-        "LastModifiedDate": datetime,
-        "ResourceArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateRulesetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRulesetRequestRequestTypeDef",
     {
         "Name": str,
         "Rules": Sequence[RuleTypeDef],
     },
 )
@@ -1817,20 +2222,38 @@
     "_OptionalUpdateRulesetRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateRulesetRequestRequestTypeDef(
     _RequiredUpdateRulesetRequestRequestTypeDef, _OptionalUpdateRulesetRequestRequestTypeDef
 ):
     pass
 
+_RequiredColumnStatisticsConfigurationOutputTypeDef = TypedDict(
+    "_RequiredColumnStatisticsConfigurationOutputTypeDef",
+    {
+        "Statistics": StatisticsConfigurationOutputTypeDef,
+    },
+)
+_OptionalColumnStatisticsConfigurationOutputTypeDef = TypedDict(
+    "_OptionalColumnStatisticsConfigurationOutputTypeDef",
+    {
+        "Selectors": List[ColumnSelectorOutputTypeDef],
+    },
+    total=False,
+)
+
+class ColumnStatisticsConfigurationOutputTypeDef(
+    _RequiredColumnStatisticsConfigurationOutputTypeDef,
+    _OptionalColumnStatisticsConfigurationOutputTypeDef,
+):
+    pass
 
 _RequiredColumnStatisticsConfigurationTypeDef = TypedDict(
     "_RequiredColumnStatisticsConfigurationTypeDef",
     {
         "Statistics": StatisticsConfigurationTypeDef,
     },
 )
@@ -1838,21 +2261,19 @@
     "_OptionalColumnStatisticsConfigurationTypeDef",
     {
         "Selectors": Sequence[ColumnSelectorTypeDef],
     },
     total=False,
 )
 
-
 class ColumnStatisticsConfigurationTypeDef(
     _RequiredColumnStatisticsConfigurationTypeDef, _OptionalColumnStatisticsConfigurationTypeDef
 ):
     pass
 
-
 _RequiredCreateRecipeJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRecipeJobRequestRequestTypeDef",
     {
         "Name": str,
         "RoleArn": str,
     },
 )
@@ -1872,21 +2293,19 @@
         "RecipeReference": RecipeReferenceTypeDef,
         "Tags": Mapping[str, str],
         "Timeout": int,
     },
     total=False,
 )
 
-
 class CreateRecipeJobRequestRequestTypeDef(
     _RequiredCreateRecipeJobRequestRequestTypeDef, _OptionalCreateRecipeJobRequestRequestTypeDef
 ):
     pass
 
-
 JobRunTypeDef = TypedDict(
     "JobRunTypeDef",
     {
         "Attempt": int,
         "CompletedOn": datetime,
         "DatasetName": str,
         "ErrorMessage": str,
@@ -1895,19 +2314,19 @@
         "RunId": str,
         "State": JobRunStateType,
         "LogSubscription": LogSubscriptionType,
         "LogGroupName": str,
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
         "DatabaseOutputs": List[DatabaseOutputTypeDef],
-        "RecipeReference": RecipeReferenceTypeDef,
+        "RecipeReference": RecipeReferenceOutputTypeDef,
         "StartedBy": str,
         "StartedOn": datetime,
-        "JobSample": JobSampleTypeDef,
-        "ValidationConfigurations": List[ValidationConfigurationTypeDef],
+        "JobSample": JobSampleOutputTypeDef,
+        "ValidationConfigurations": List[ValidationConfigurationOutputTypeDef],
     },
     total=False,
 )
 
 _RequiredJobTypeDef = TypedDict(
     "_RequiredJobTypeDef",
     {
@@ -1929,30 +2348,28 @@
         "LogSubscription": LogSubscriptionType,
         "MaxCapacity": int,
         "MaxRetries": int,
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
         "DatabaseOutputs": List[DatabaseOutputTypeDef],
         "ProjectName": str,
-        "RecipeReference": RecipeReferenceTypeDef,
+        "RecipeReference": RecipeReferenceOutputTypeDef,
         "ResourceArn": str,
         "RoleArn": str,
         "Timeout": int,
         "Tags": Dict[str, str],
-        "JobSample": JobSampleTypeDef,
-        "ValidationConfigurations": List[ValidationConfigurationTypeDef],
+        "JobSample": JobSampleOutputTypeDef,
+        "ValidationConfigurations": List[ValidationConfigurationOutputTypeDef],
     },
     total=False,
 )
 
-
 class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
     pass
 
-
 _RequiredUpdateRecipeJobRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRecipeJobRequestRequestTypeDef",
     {
         "Name": str,
         "RoleArn": str,
     },
 )
@@ -1968,95 +2385,89 @@
         "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
         "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
         "Timeout": int,
     },
     total=False,
 )
 
-
 class UpdateRecipeJobRequestRequestTypeDef(
     _RequiredUpdateRecipeJobRequestRequestTypeDef, _OptionalUpdateRecipeJobRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Input": InputTypeDef,
-    },
-)
-_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetRequestRequestTypeDef",
-    {
-        "Format": InputFormatType,
-        "FormatOptions": FormatOptionsTypeDef,
-        "PathOptions": PathOptionsTypeDef,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateDatasetRequestRequestTypeDef(
-    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredDatasetTypeDef = TypedDict(
     "_RequiredDatasetTypeDef",
     {
         "Name": str,
-        "Input": InputTypeDef,
+        "Input": InputOutputTypeDef,
     },
 )
 _OptionalDatasetTypeDef = TypedDict(
     "_OptionalDatasetTypeDef",
     {
         "AccountId": str,
         "CreatedBy": str,
         "CreateDate": datetime,
         "Format": InputFormatType,
-        "FormatOptions": FormatOptionsTypeDef,
+        "FormatOptions": FormatOptionsOutputTypeDef,
         "LastModifiedDate": datetime,
         "LastModifiedBy": str,
         "Source": SourceType,
-        "PathOptions": PathOptionsTypeDef,
+        "PathOptions": PathOptionsOutputTypeDef,
         "Tags": Dict[str, str],
         "ResourceArn": str,
     },
     total=False,
 )
 
-
 class DatasetTypeDef(_RequiredDatasetTypeDef, _OptionalDatasetTypeDef):
     pass
 
-
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "CreatedBy": str,
         "CreateDate": datetime,
         "Name": str,
         "Format": InputFormatType,
-        "FormatOptions": FormatOptionsTypeDef,
-        "Input": InputTypeDef,
+        "FormatOptions": FormatOptionsOutputTypeDef,
+        "Input": InputOutputTypeDef,
         "LastModifiedDate": datetime,
         "LastModifiedBy": str,
         "Source": SourceType,
-        "PathOptions": PathOptionsTypeDef,
+        "PathOptions": PathOptionsOutputTypeDef,
         "Tags": Dict[str, str],
         "ResourceArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Input": InputTypeDef,
+    },
+)
+_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetRequestRequestTypeDef",
+    {
+        "Format": InputFormatType,
+        "FormatOptions": FormatOptionsTypeDef,
+        "PathOptions": PathOptionsTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateDatasetRequestRequestTypeDef(
+    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
+):
+    pass
+
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "Name": str,
         "Input": InputTypeDef,
     },
 )
@@ -2066,21 +2477,19 @@
         "Format": InputFormatType,
         "FormatOptions": FormatOptionsTypeDef,
         "PathOptions": PathOptionsTypeDef,
     },
     total=False,
 )
 
-
 class UpdateDatasetRequestRequestTypeDef(
     _RequiredUpdateDatasetRequestRequestTypeDef, _OptionalUpdateDatasetRequestRequestTypeDef
 ):
     pass
 
-
 ListRecipeVersionsResponseTypeDef = TypedDict(
     "ListRecipeVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Recipes": List[RecipeTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2091,14 +2500,25 @@
     {
         "Recipes": List[RecipeTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ProfileConfigurationOutputTypeDef = TypedDict(
+    "ProfileConfigurationOutputTypeDef",
+    {
+        "DatasetStatisticsConfiguration": StatisticsConfigurationOutputTypeDef,
+        "ProfileColumns": List[ColumnSelectorOutputTypeDef],
+        "ColumnStatisticsConfigurations": List[ColumnStatisticsConfigurationOutputTypeDef],
+        "EntityDetectorConfiguration": EntityDetectorConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ProfileConfigurationTypeDef = TypedDict(
     "ProfileConfigurationTypeDef",
     {
         "DatasetStatisticsConfiguration": StatisticsConfigurationTypeDef,
         "ProfileColumns": Sequence[ColumnSelectorTypeDef],
         "ColumnStatisticsConfigurations": Sequence[ColumnStatisticsConfigurationTypeDef],
         "EntityDetectorConfiguration": EntityDetectorConfigurationTypeDef,
@@ -2129,47 +2549,14 @@
     {
         "Datasets": List[DatasetTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateProfileJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProfileJobRequestRequestTypeDef",
-    {
-        "DatasetName": str,
-        "Name": str,
-        "OutputLocation": S3LocationTypeDef,
-        "RoleArn": str,
-    },
-)
-_OptionalCreateProfileJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProfileJobRequestRequestTypeDef",
-    {
-        "EncryptionKeyArn": str,
-        "EncryptionMode": EncryptionModeType,
-        "LogSubscription": LogSubscriptionType,
-        "MaxCapacity": int,
-        "MaxRetries": int,
-        "Configuration": ProfileConfigurationTypeDef,
-        "ValidationConfigurations": Sequence[ValidationConfigurationTypeDef],
-        "Tags": Mapping[str, str],
-        "Timeout": int,
-        "JobSample": JobSampleTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateProfileJobRequestRequestTypeDef(
-    _RequiredCreateProfileJobRequestRequestTypeDef, _OptionalCreateProfileJobRequestRequestTypeDef
-):
-    pass
-
-
 DescribeJobResponseTypeDef = TypedDict(
     "DescribeJobResponseTypeDef",
     {
         "CreateDate": datetime,
         "CreatedBy": str,
         "DatasetName": str,
         "EncryptionKeyArn": str,
@@ -2181,52 +2568,83 @@
         "LogSubscription": LogSubscriptionType,
         "MaxCapacity": int,
         "MaxRetries": int,
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
         "DatabaseOutputs": List[DatabaseOutputTypeDef],
         "ProjectName": str,
-        "ProfileConfiguration": ProfileConfigurationTypeDef,
-        "ValidationConfigurations": List[ValidationConfigurationTypeDef],
-        "RecipeReference": RecipeReferenceTypeDef,
+        "ProfileConfiguration": ProfileConfigurationOutputTypeDef,
+        "ValidationConfigurations": List[ValidationConfigurationOutputTypeDef],
+        "RecipeReference": RecipeReferenceOutputTypeDef,
         "ResourceArn": str,
         "RoleArn": str,
         "Tags": Dict[str, str],
         "Timeout": int,
-        "JobSample": JobSampleTypeDef,
+        "JobSample": JobSampleOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeJobRunResponseTypeDef = TypedDict(
     "DescribeJobRunResponseTypeDef",
     {
         "Attempt": int,
         "CompletedOn": datetime,
         "DatasetName": str,
         "ErrorMessage": str,
         "ExecutionTime": int,
         "JobName": str,
-        "ProfileConfiguration": ProfileConfigurationTypeDef,
-        "ValidationConfigurations": List[ValidationConfigurationTypeDef],
+        "ProfileConfiguration": ProfileConfigurationOutputTypeDef,
+        "ValidationConfigurations": List[ValidationConfigurationOutputTypeDef],
         "RunId": str,
         "State": JobRunStateType,
         "LogSubscription": LogSubscriptionType,
         "LogGroupName": str,
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
         "DatabaseOutputs": List[DatabaseOutputTypeDef],
-        "RecipeReference": RecipeReferenceTypeDef,
+        "RecipeReference": RecipeReferenceOutputTypeDef,
         "StartedBy": str,
         "StartedOn": datetime,
-        "JobSample": JobSampleTypeDef,
+        "JobSample": JobSampleOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCreateProfileJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProfileJobRequestRequestTypeDef",
+    {
+        "DatasetName": str,
+        "Name": str,
+        "OutputLocation": S3LocationTypeDef,
+        "RoleArn": str,
+    },
+)
+_OptionalCreateProfileJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProfileJobRequestRequestTypeDef",
+    {
+        "EncryptionKeyArn": str,
+        "EncryptionMode": EncryptionModeType,
+        "LogSubscription": LogSubscriptionType,
+        "MaxCapacity": int,
+        "MaxRetries": int,
+        "Configuration": ProfileConfigurationTypeDef,
+        "ValidationConfigurations": Sequence[ValidationConfigurationTypeDef],
+        "Tags": Mapping[str, str],
+        "Timeout": int,
+        "JobSample": JobSampleTypeDef,
+    },
+    total=False,
+)
+
+class CreateProfileJobRequestRequestTypeDef(
+    _RequiredCreateProfileJobRequestRequestTypeDef, _OptionalCreateProfileJobRequestRequestTypeDef
+):
+    pass
+
 _RequiredUpdateProfileJobRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProfileJobRequestRequestTypeDef",
     {
         "Name": str,
         "OutputLocation": S3LocationTypeDef,
         "RoleArn": str,
     },
@@ -2243,12 +2661,11 @@
         "ValidationConfigurations": Sequence[ValidationConfigurationTypeDef],
         "Timeout": int,
         "JobSample": JobSampleTypeDef,
     },
     total=False,
 )
 
-
 class UpdateProfileJobRequestRequestTypeDef(
     _RequiredUpdateProfileJobRequestRequestTypeDef, _OptionalUpdateProfileJobRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-databrew-1.28.0/mypy_boto3_databrew/type_defs.pyi` & `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/type_defs.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for databrew service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_databrew.type_defs import AllowedStatisticsTypeDef
+    from mypy_boto3_databrew.type_defs import AllowedStatisticsOutputTypeDef
 
-    data: AllowedStatisticsTypeDef = {...}
+    data: AllowedStatisticsOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -39,35 +39,44 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "AllowedStatisticsOutputTypeDef",
     "AllowedStatisticsTypeDef",
     "BatchDeleteRecipeVersionRequestRequestTypeDef",
     "RecipeVersionErrorDetailTypeDef",
+    "ColumnSelectorOutputTypeDef",
     "ColumnSelectorTypeDef",
+    "ConditionExpressionOutputTypeDef",
     "ConditionExpressionTypeDef",
     "CreateDatasetResponseTypeDef",
     "JobSampleTypeDef",
     "S3LocationTypeDef",
     "ValidationConfigurationTypeDef",
     "CreateProfileJobResponseTypeDef",
     "SampleTypeDef",
     "CreateProjectResponseTypeDef",
     "RecipeReferenceTypeDef",
     "CreateRecipeJobResponseTypeDef",
     "CreateRecipeResponseTypeDef",
     "CreateRulesetResponseTypeDef",
     "CreateScheduleRequestRequestTypeDef",
     "CreateScheduleResponseTypeDef",
+    "CsvOptionsOutputTypeDef",
     "CsvOptionsTypeDef",
+    "CsvOutputOptionsOutputTypeDef",
     "CsvOutputOptionsTypeDef",
+    "S3LocationOutputTypeDef",
+    "DatetimeOptionsOutputTypeDef",
+    "FilterExpressionOutputTypeDef",
     "DatetimeOptionsTypeDef",
     "FilterExpressionTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteDatasetResponseTypeDef",
     "DeleteJobRequestRequestTypeDef",
     "DeleteJobResponseTypeDef",
     "DeleteProjectRequestRequestTypeDef",
@@ -76,23 +85,31 @@
     "DeleteRecipeVersionResponseTypeDef",
     "DeleteRulesetRequestRequestTypeDef",
     "DeleteRulesetResponseTypeDef",
     "DeleteScheduleRequestRequestTypeDef",
     "DeleteScheduleResponseTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
+    "JobSampleOutputTypeDef",
+    "RecipeReferenceOutputTypeDef",
+    "ValidationConfigurationOutputTypeDef",
     "DescribeJobRunRequestRequestTypeDef",
     "DescribeProjectRequestRequestTypeDef",
+    "SampleOutputTypeDef",
     "DescribeRecipeRequestRequestTypeDef",
     "DescribeRulesetRequestRequestTypeDef",
     "DescribeScheduleRequestRequestTypeDef",
     "DescribeScheduleResponseTypeDef",
+    "ExcelOptionsOutputTypeDef",
     "ExcelOptionsTypeDef",
+    "FilesLimitOutputTypeDef",
     "FilesLimitTypeDef",
+    "JsonOptionsOutputTypeDef",
     "JsonOptionsTypeDef",
+    "MetadataOutputTypeDef",
     "MetadataTypeDef",
     "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
@@ -109,89 +126,114 @@
     "ListSchedulesRequestRequestTypeDef",
     "ScheduleTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
     "PublishRecipeRequestRequestTypeDef",
     "PublishRecipeResponseTypeDef",
+    "RecipeActionOutputTypeDef",
     "RecipeActionTypeDef",
     "ResponseMetadataTypeDef",
+    "ThresholdOutputTypeDef",
     "ThresholdTypeDef",
     "ViewFrameTypeDef",
     "SendProjectSessionActionResponseTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "StartJobRunResponseTypeDef",
     "StartProjectSessionRequestRequestTypeDef",
     "StartProjectSessionResponseTypeDef",
+    "StatisticOverrideOutputTypeDef",
     "StatisticOverrideTypeDef",
     "StopJobRunRequestRequestTypeDef",
     "StopJobRunResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasetResponseTypeDef",
     "UpdateProfileJobResponseTypeDef",
     "UpdateProjectResponseTypeDef",
     "UpdateRecipeJobResponseTypeDef",
     "UpdateRecipeResponseTypeDef",
     "UpdateRulesetResponseTypeDef",
     "UpdateScheduleRequestRequestTypeDef",
     "UpdateScheduleResponseTypeDef",
+    "EntityDetectorConfigurationOutputTypeDef",
     "EntityDetectorConfigurationTypeDef",
     "BatchDeleteRecipeVersionResponseTypeDef",
     "DataCatalogInputDefinitionTypeDef",
     "DatabaseInputDefinitionTypeDef",
     "DatabaseTableOutputOptionsTypeDef",
     "S3TableOutputOptionsTypeDef",
     "CreateProjectRequestRequestTypeDef",
-    "DescribeProjectResponseTypeDef",
-    "ProjectTypeDef",
     "UpdateProjectRequestRequestTypeDef",
+    "OutputFormatOptionsOutputTypeDef",
     "OutputFormatOptionsTypeDef",
+    "DataCatalogInputDefinitionOutputTypeDef",
+    "DatabaseInputDefinitionOutputTypeDef",
+    "DatabaseTableOutputOptionsOutputTypeDef",
+    "S3TableOutputOptionsOutputTypeDef",
+    "DatasetParameterOutputTypeDef",
     "DatasetParameterTypeDef",
+    "DescribeProjectResponseTypeDef",
+    "ProjectTypeDef",
+    "FormatOptionsOutputTypeDef",
     "FormatOptionsTypeDef",
     "ListRulesetsResponseTypeDef",
     "ListSchedulesResponseTypeDef",
+    "RecipeStepOutputTypeDef",
     "RecipeStepTypeDef",
+    "RuleOutputTypeDef",
     "RuleTypeDef",
+    "StatisticsConfigurationOutputTypeDef",
     "StatisticsConfigurationTypeDef",
     "InputTypeDef",
     "DatabaseOutputTypeDef",
     "DataCatalogOutputTypeDef",
-    "ListProjectsResponseTypeDef",
     "OutputTypeDef",
+    "InputOutputTypeDef",
+    "PathOptionsOutputTypeDef",
     "PathOptionsTypeDef",
-    "CreateRecipeRequestRequestTypeDef",
+    "ListProjectsResponseTypeDef",
     "DescribeRecipeResponseTypeDef",
     "RecipeTypeDef",
+    "CreateRecipeRequestRequestTypeDef",
     "SendProjectSessionActionRequestRequestTypeDef",
     "UpdateRecipeRequestRequestTypeDef",
-    "CreateRulesetRequestRequestTypeDef",
     "DescribeRulesetResponseTypeDef",
+    "CreateRulesetRequestRequestTypeDef",
     "UpdateRulesetRequestRequestTypeDef",
+    "ColumnStatisticsConfigurationOutputTypeDef",
     "ColumnStatisticsConfigurationTypeDef",
     "CreateRecipeJobRequestRequestTypeDef",
     "JobRunTypeDef",
     "JobTypeDef",
     "UpdateRecipeJobRequestRequestTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
     "DatasetTypeDef",
     "DescribeDatasetResponseTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
     "UpdateDatasetRequestRequestTypeDef",
     "ListRecipeVersionsResponseTypeDef",
     "ListRecipesResponseTypeDef",
+    "ProfileConfigurationOutputTypeDef",
     "ProfileConfigurationTypeDef",
     "ListJobRunsResponseTypeDef",
     "ListJobsResponseTypeDef",
     "ListDatasetsResponseTypeDef",
-    "CreateProfileJobRequestRequestTypeDef",
     "DescribeJobResponseTypeDef",
     "DescribeJobRunResponseTypeDef",
+    "CreateProfileJobRequestRequestTypeDef",
     "UpdateProfileJobRequestRequestTypeDef",
 )
 
+AllowedStatisticsOutputTypeDef = TypedDict(
+    "AllowedStatisticsOutputTypeDef",
+    {
+        "Statistics": List[str],
+    },
+)
+
 AllowedStatisticsTypeDef = TypedDict(
     "AllowedStatisticsTypeDef",
     {
         "Statistics": Sequence[str],
     },
 )
 
@@ -209,23 +251,54 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "RecipeVersion": str,
     },
     total=False,
 )
 
+ColumnSelectorOutputTypeDef = TypedDict(
+    "ColumnSelectorOutputTypeDef",
+    {
+        "Regex": str,
+        "Name": str,
+    },
+    total=False,
+)
+
 ColumnSelectorTypeDef = TypedDict(
     "ColumnSelectorTypeDef",
     {
         "Regex": str,
         "Name": str,
     },
     total=False,
 )
 
+_RequiredConditionExpressionOutputTypeDef = TypedDict(
+    "_RequiredConditionExpressionOutputTypeDef",
+    {
+        "Condition": str,
+        "TargetColumn": str,
+    },
+)
+_OptionalConditionExpressionOutputTypeDef = TypedDict(
+    "_OptionalConditionExpressionOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+
+class ConditionExpressionOutputTypeDef(
+    _RequiredConditionExpressionOutputTypeDef, _OptionalConditionExpressionOutputTypeDef
+):
+    pass
+
+
 _RequiredConditionExpressionTypeDef = TypedDict(
     "_RequiredConditionExpressionTypeDef",
     {
         "Condition": str,
         "TargetColumn": str,
     },
 )
@@ -233,19 +306,21 @@
     "_OptionalConditionExpressionTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class ConditionExpressionTypeDef(
     _RequiredConditionExpressionTypeDef, _OptionalConditionExpressionTypeDef
 ):
     pass
 
+
 CreateDatasetResponseTypeDef = TypedDict(
     "CreateDatasetResponseTypeDef",
     {
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -270,36 +345,40 @@
     {
         "Key": str,
         "BucketOwner": str,
     },
     total=False,
 )
 
+
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
+
 _RequiredValidationConfigurationTypeDef = TypedDict(
     "_RequiredValidationConfigurationTypeDef",
     {
         "RulesetArn": str,
     },
 )
 _OptionalValidationConfigurationTypeDef = TypedDict(
     "_OptionalValidationConfigurationTypeDef",
     {
         "ValidationMode": Literal["CHECK_ALL"],
     },
     total=False,
 )
 
+
 class ValidationConfigurationTypeDef(
     _RequiredValidationConfigurationTypeDef, _OptionalValidationConfigurationTypeDef
 ):
     pass
 
+
 CreateProfileJobResponseTypeDef = TypedDict(
     "CreateProfileJobResponseTypeDef",
     {
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -314,17 +393,19 @@
     "_OptionalSampleTypeDef",
     {
         "Size": int,
     },
     total=False,
 )
 
+
 class SampleTypeDef(_RequiredSampleTypeDef, _OptionalSampleTypeDef):
     pass
 
+
 CreateProjectResponseTypeDef = TypedDict(
     "CreateProjectResponseTypeDef",
     {
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -339,17 +420,19 @@
     "_OptionalRecipeReferenceTypeDef",
     {
         "RecipeVersion": str,
     },
     total=False,
 )
 
+
 class RecipeReferenceTypeDef(_RequiredRecipeReferenceTypeDef, _OptionalRecipeReferenceTypeDef):
     pass
 
+
 CreateRecipeJobResponseTypeDef = TypedDict(
     "CreateRecipeJobResponseTypeDef",
     {
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -382,44 +465,113 @@
     {
         "JobNames": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateScheduleRequestRequestTypeDef(
     _RequiredCreateScheduleRequestRequestTypeDef, _OptionalCreateScheduleRequestRequestTypeDef
 ):
     pass
 
+
 CreateScheduleResponseTypeDef = TypedDict(
     "CreateScheduleResponseTypeDef",
     {
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CsvOptionsOutputTypeDef = TypedDict(
+    "CsvOptionsOutputTypeDef",
+    {
+        "Delimiter": str,
+        "HeaderRow": bool,
+    },
+    total=False,
+)
+
 CsvOptionsTypeDef = TypedDict(
     "CsvOptionsTypeDef",
     {
         "Delimiter": str,
         "HeaderRow": bool,
     },
     total=False,
 )
 
+CsvOutputOptionsOutputTypeDef = TypedDict(
+    "CsvOutputOptionsOutputTypeDef",
+    {
+        "Delimiter": str,
+    },
+    total=False,
+)
+
 CsvOutputOptionsTypeDef = TypedDict(
     "CsvOutputOptionsTypeDef",
     {
         "Delimiter": str,
     },
     total=False,
 )
 
+_RequiredS3LocationOutputTypeDef = TypedDict(
+    "_RequiredS3LocationOutputTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalS3LocationOutputTypeDef = TypedDict(
+    "_OptionalS3LocationOutputTypeDef",
+    {
+        "Key": str,
+        "BucketOwner": str,
+    },
+    total=False,
+)
+
+
+class S3LocationOutputTypeDef(_RequiredS3LocationOutputTypeDef, _OptionalS3LocationOutputTypeDef):
+    pass
+
+
+_RequiredDatetimeOptionsOutputTypeDef = TypedDict(
+    "_RequiredDatetimeOptionsOutputTypeDef",
+    {
+        "Format": str,
+    },
+)
+_OptionalDatetimeOptionsOutputTypeDef = TypedDict(
+    "_OptionalDatetimeOptionsOutputTypeDef",
+    {
+        "TimezoneOffset": str,
+        "LocaleCode": str,
+    },
+    total=False,
+)
+
+
+class DatetimeOptionsOutputTypeDef(
+    _RequiredDatetimeOptionsOutputTypeDef, _OptionalDatetimeOptionsOutputTypeDef
+):
+    pass
+
+
+FilterExpressionOutputTypeDef = TypedDict(
+    "FilterExpressionOutputTypeDef",
+    {
+        "Expression": str,
+        "ValuesMap": Dict[str, str],
+    },
+)
+
 _RequiredDatetimeOptionsTypeDef = TypedDict(
     "_RequiredDatetimeOptionsTypeDef",
     {
         "Format": str,
     },
 )
 _OptionalDatetimeOptionsTypeDef = TypedDict(
@@ -427,17 +579,19 @@
     {
         "TimezoneOffset": str,
         "LocaleCode": str,
     },
     total=False,
 )
 
+
 class DatetimeOptionsTypeDef(_RequiredDatetimeOptionsTypeDef, _OptionalDatetimeOptionsTypeDef):
     pass
 
+
 FilterExpressionTypeDef = TypedDict(
     "FilterExpressionTypeDef",
     {
         "Expression": str,
         "ValuesMap": Mapping[str, str],
     },
 )
@@ -544,14 +698,65 @@
 DescribeJobRequestRequestTypeDef = TypedDict(
     "DescribeJobRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+JobSampleOutputTypeDef = TypedDict(
+    "JobSampleOutputTypeDef",
+    {
+        "Mode": SampleModeType,
+        "Size": int,
+    },
+    total=False,
+)
+
+_RequiredRecipeReferenceOutputTypeDef = TypedDict(
+    "_RequiredRecipeReferenceOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalRecipeReferenceOutputTypeDef = TypedDict(
+    "_OptionalRecipeReferenceOutputTypeDef",
+    {
+        "RecipeVersion": str,
+    },
+    total=False,
+)
+
+
+class RecipeReferenceOutputTypeDef(
+    _RequiredRecipeReferenceOutputTypeDef, _OptionalRecipeReferenceOutputTypeDef
+):
+    pass
+
+
+_RequiredValidationConfigurationOutputTypeDef = TypedDict(
+    "_RequiredValidationConfigurationOutputTypeDef",
+    {
+        "RulesetArn": str,
+    },
+)
+_OptionalValidationConfigurationOutputTypeDef = TypedDict(
+    "_OptionalValidationConfigurationOutputTypeDef",
+    {
+        "ValidationMode": Literal["CHECK_ALL"],
+    },
+    total=False,
+)
+
+
+class ValidationConfigurationOutputTypeDef(
+    _RequiredValidationConfigurationOutputTypeDef, _OptionalValidationConfigurationOutputTypeDef
+):
+    pass
+
+
 DescribeJobRunRequestRequestTypeDef = TypedDict(
     "DescribeJobRunRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
@@ -559,33 +764,54 @@
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+_RequiredSampleOutputTypeDef = TypedDict(
+    "_RequiredSampleOutputTypeDef",
+    {
+        "Type": SampleTypeType,
+    },
+)
+_OptionalSampleOutputTypeDef = TypedDict(
+    "_OptionalSampleOutputTypeDef",
+    {
+        "Size": int,
+    },
+    total=False,
+)
+
+
+class SampleOutputTypeDef(_RequiredSampleOutputTypeDef, _OptionalSampleOutputTypeDef):
+    pass
+
+
 _RequiredDescribeRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRecipeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDescribeRecipeRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeRecipeRequestRequestTypeDef",
     {
         "RecipeVersion": str,
     },
     total=False,
 )
 
+
 class DescribeRecipeRequestRequestTypeDef(
     _RequiredDescribeRecipeRequestRequestTypeDef, _OptionalDescribeRecipeRequestRequestTypeDef
 ):
     pass
 
+
 DescribeRulesetRequestRequestTypeDef = TypedDict(
     "DescribeRulesetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -608,24 +834,54 @@
         "CronExpression": str,
         "Tags": Dict[str, str],
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ExcelOptionsOutputTypeDef = TypedDict(
+    "ExcelOptionsOutputTypeDef",
+    {
+        "SheetNames": List[str],
+        "SheetIndexes": List[int],
+        "HeaderRow": bool,
+    },
+    total=False,
+)
+
 ExcelOptionsTypeDef = TypedDict(
     "ExcelOptionsTypeDef",
     {
         "SheetNames": Sequence[str],
         "SheetIndexes": Sequence[int],
         "HeaderRow": bool,
     },
     total=False,
 )
 
+_RequiredFilesLimitOutputTypeDef = TypedDict(
+    "_RequiredFilesLimitOutputTypeDef",
+    {
+        "MaxFiles": int,
+    },
+)
+_OptionalFilesLimitOutputTypeDef = TypedDict(
+    "_OptionalFilesLimitOutputTypeDef",
+    {
+        "OrderedBy": Literal["LAST_MODIFIED_DATE"],
+        "Order": OrderType,
+    },
+    total=False,
+)
+
+
+class FilesLimitOutputTypeDef(_RequiredFilesLimitOutputTypeDef, _OptionalFilesLimitOutputTypeDef):
+    pass
+
+
 _RequiredFilesLimitTypeDef = TypedDict(
     "_RequiredFilesLimitTypeDef",
     {
         "MaxFiles": int,
     },
 )
 _OptionalFilesLimitTypeDef = TypedDict(
@@ -633,25 +889,43 @@
     {
         "OrderedBy": Literal["LAST_MODIFIED_DATE"],
         "Order": OrderType,
     },
     total=False,
 )
 
+
 class FilesLimitTypeDef(_RequiredFilesLimitTypeDef, _OptionalFilesLimitTypeDef):
     pass
 
+
+JsonOptionsOutputTypeDef = TypedDict(
+    "JsonOptionsOutputTypeDef",
+    {
+        "MultiLine": bool,
+    },
+    total=False,
+)
+
 JsonOptionsTypeDef = TypedDict(
     "JsonOptionsTypeDef",
     {
         "MultiLine": bool,
     },
     total=False,
 )
 
+MetadataOutputTypeDef = TypedDict(
+    "MetadataOutputTypeDef",
+    {
+        "SourceArn": str,
+    },
+    total=False,
+)
+
 MetadataTypeDef = TypedDict(
     "MetadataTypeDef",
     {
         "SourceArn": str,
     },
     total=False,
 )
@@ -683,20 +957,22 @@
     "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListJobRunsRequestListJobRunsPaginateTypeDef(
     _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
     _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobRunsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -704,19 +980,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
+
 ListJobsRequestListJobsPaginateTypeDef = TypedDict(
     "ListJobsRequestListJobsPaginateTypeDef",
     {
         "DatasetName": str,
         "ProjectName": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -761,20 +1039,22 @@
     "_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef(
     _RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
     _OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListRecipeVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListRecipeVersionsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListRecipeVersionsRequestRequestTypeDef = TypedDict(
@@ -782,20 +1062,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListRecipeVersionsRequestRequestTypeDef(
     _RequiredListRecipeVersionsRequestRequestTypeDef,
     _OptionalListRecipeVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListRecipesRequestListRecipesPaginateTypeDef = TypedDict(
     "ListRecipesRequestListRecipesPaginateTypeDef",
     {
         "RecipeVersion": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -849,17 +1131,19 @@
         "ResourceArn": str,
         "RuleCount": int,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class RulesetItemTypeDef(_RequiredRulesetItemTypeDef, _OptionalRulesetItemTypeDef):
     pass
 
+
 ListSchedulesRequestListSchedulesPaginateTypeDef = TypedDict(
     "ListSchedulesRequestListSchedulesPaginateTypeDef",
     {
         "JobName": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -893,17 +1177,19 @@
         "ResourceArn": str,
         "CronExpression": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class ScheduleTypeDef(_RequiredScheduleTypeDef, _OptionalScheduleTypeDef):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -935,55 +1221,100 @@
     "_OptionalPublishRecipeRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class PublishRecipeRequestRequestTypeDef(
     _RequiredPublishRecipeRequestRequestTypeDef, _OptionalPublishRecipeRequestRequestTypeDef
 ):
     pass
 
+
 PublishRecipeResponseTypeDef = TypedDict(
     "PublishRecipeResponseTypeDef",
     {
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredRecipeActionOutputTypeDef = TypedDict(
+    "_RequiredRecipeActionOutputTypeDef",
+    {
+        "Operation": str,
+    },
+)
+_OptionalRecipeActionOutputTypeDef = TypedDict(
+    "_OptionalRecipeActionOutputTypeDef",
+    {
+        "Parameters": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class RecipeActionOutputTypeDef(
+    _RequiredRecipeActionOutputTypeDef, _OptionalRecipeActionOutputTypeDef
+):
+    pass
+
+
 _RequiredRecipeActionTypeDef = TypedDict(
     "_RequiredRecipeActionTypeDef",
     {
         "Operation": str,
     },
 )
 _OptionalRecipeActionTypeDef = TypedDict(
     "_OptionalRecipeActionTypeDef",
     {
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
+
 class RecipeActionTypeDef(_RequiredRecipeActionTypeDef, _OptionalRecipeActionTypeDef):
     pass
 
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
 
+_RequiredThresholdOutputTypeDef = TypedDict(
+    "_RequiredThresholdOutputTypeDef",
+    {
+        "Value": float,
+    },
+)
+_OptionalThresholdOutputTypeDef = TypedDict(
+    "_OptionalThresholdOutputTypeDef",
+    {
+        "Type": ThresholdTypeType,
+        "Unit": ThresholdUnitType,
+    },
+    total=False,
+)
+
+
+class ThresholdOutputTypeDef(_RequiredThresholdOutputTypeDef, _OptionalThresholdOutputTypeDef):
+    pass
+
+
 _RequiredThresholdTypeDef = TypedDict(
     "_RequiredThresholdTypeDef",
     {
         "Value": float,
     },
 )
 _OptionalThresholdTypeDef = TypedDict(
@@ -991,17 +1322,19 @@
     {
         "Type": ThresholdTypeType,
         "Unit": ThresholdUnitType,
     },
     total=False,
 )
 
+
 class ThresholdTypeDef(_RequiredThresholdTypeDef, _OptionalThresholdTypeDef):
     pass
 
+
 _RequiredViewFrameTypeDef = TypedDict(
     "_RequiredViewFrameTypeDef",
     {
         "StartColumnIndex": int,
     },
 )
 _OptionalViewFrameTypeDef = TypedDict(
@@ -1012,17 +1345,19 @@
         "StartRowIndex": int,
         "RowRange": int,
         "Analytics": AnalyticsModeType,
     },
     total=False,
 )
 
+
 class ViewFrameTypeDef(_RequiredViewFrameTypeDef, _OptionalViewFrameTypeDef):
     pass
 
+
 SendProjectSessionActionResponseTypeDef = TypedDict(
     "SendProjectSessionActionResponseTypeDef",
     {
         "Result": str,
         "Name": str,
         "ActionId": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1054,29 +1389,39 @@
     "_OptionalStartProjectSessionRequestRequestTypeDef",
     {
         "AssumeControl": bool,
     },
     total=False,
 )
 
+
 class StartProjectSessionRequestRequestTypeDef(
     _RequiredStartProjectSessionRequestRequestTypeDef,
     _OptionalStartProjectSessionRequestRequestTypeDef,
 ):
     pass
 
+
 StartProjectSessionResponseTypeDef = TypedDict(
     "StartProjectSessionResponseTypeDef",
     {
         "Name": str,
         "ClientSessionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+StatisticOverrideOutputTypeDef = TypedDict(
+    "StatisticOverrideOutputTypeDef",
+    {
+        "Statistic": str,
+        "Parameters": Dict[str, str],
+    },
+)
+
 StatisticOverrideTypeDef = TypedDict(
     "StatisticOverrideTypeDef",
     {
         "Statistic": str,
         "Parameters": Mapping[str, str],
     },
 )
@@ -1173,46 +1518,72 @@
     "_OptionalUpdateScheduleRequestRequestTypeDef",
     {
         "JobNames": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateScheduleRequestRequestTypeDef(
     _RequiredUpdateScheduleRequestRequestTypeDef, _OptionalUpdateScheduleRequestRequestTypeDef
 ):
     pass
 
+
 UpdateScheduleResponseTypeDef = TypedDict(
     "UpdateScheduleResponseTypeDef",
     {
         "Name": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredEntityDetectorConfigurationOutputTypeDef = TypedDict(
+    "_RequiredEntityDetectorConfigurationOutputTypeDef",
+    {
+        "EntityTypes": List[str],
+    },
+)
+_OptionalEntityDetectorConfigurationOutputTypeDef = TypedDict(
+    "_OptionalEntityDetectorConfigurationOutputTypeDef",
+    {
+        "AllowedStatistics": List[AllowedStatisticsOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class EntityDetectorConfigurationOutputTypeDef(
+    _RequiredEntityDetectorConfigurationOutputTypeDef,
+    _OptionalEntityDetectorConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredEntityDetectorConfigurationTypeDef = TypedDict(
     "_RequiredEntityDetectorConfigurationTypeDef",
     {
         "EntityTypes": Sequence[str],
     },
 )
 _OptionalEntityDetectorConfigurationTypeDef = TypedDict(
     "_OptionalEntityDetectorConfigurationTypeDef",
     {
         "AllowedStatistics": Sequence[AllowedStatisticsTypeDef],
     },
     total=False,
 )
 
+
 class EntityDetectorConfigurationTypeDef(
     _RequiredEntityDetectorConfigurationTypeDef, _OptionalEntityDetectorConfigurationTypeDef
 ):
     pass
 
+
 BatchDeleteRecipeVersionResponseTypeDef = TypedDict(
     "BatchDeleteRecipeVersionResponseTypeDef",
     {
         "Name": str,
         "Errors": List[RecipeVersionErrorDetailTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1230,19 +1601,21 @@
     {
         "CatalogId": str,
         "TempDirectory": S3LocationTypeDef,
     },
     total=False,
 )
 
+
 class DataCatalogInputDefinitionTypeDef(
     _RequiredDataCatalogInputDefinitionTypeDef, _OptionalDataCatalogInputDefinitionTypeDef
 ):
     pass
 
+
 _RequiredDatabaseInputDefinitionTypeDef = TypedDict(
     "_RequiredDatabaseInputDefinitionTypeDef",
     {
         "GlueConnectionName": str,
     },
 )
 _OptionalDatabaseInputDefinitionTypeDef = TypedDict(
@@ -1251,38 +1624,42 @@
         "DatabaseTableName": str,
         "TempDirectory": S3LocationTypeDef,
         "QueryString": str,
     },
     total=False,
 )
 
+
 class DatabaseInputDefinitionTypeDef(
     _RequiredDatabaseInputDefinitionTypeDef, _OptionalDatabaseInputDefinitionTypeDef
 ):
     pass
 
+
 _RequiredDatabaseTableOutputOptionsTypeDef = TypedDict(
     "_RequiredDatabaseTableOutputOptionsTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalDatabaseTableOutputOptionsTypeDef = TypedDict(
     "_OptionalDatabaseTableOutputOptionsTypeDef",
     {
         "TempDirectory": S3LocationTypeDef,
     },
     total=False,
 )
 
+
 class DatabaseTableOutputOptionsTypeDef(
     _RequiredDatabaseTableOutputOptionsTypeDef, _OptionalDatabaseTableOutputOptionsTypeDef
 ):
     pass
 
+
 S3TableOutputOptionsTypeDef = TypedDict(
     "S3TableOutputOptionsTypeDef",
     {
         "Location": S3LocationTypeDef,
     },
 )
 
@@ -1300,31 +1677,193 @@
     {
         "Sample": SampleTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateProjectRequestRequestTypeDef",
+    {
+        "RoleArn": str,
+        "Name": str,
+    },
+)
+_OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateProjectRequestRequestTypeDef",
+    {
+        "Sample": SampleTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateProjectRequestRequestTypeDef(
+    _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
+):
+    pass
+
+
+OutputFormatOptionsOutputTypeDef = TypedDict(
+    "OutputFormatOptionsOutputTypeDef",
+    {
+        "Csv": CsvOutputOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
+OutputFormatOptionsTypeDef = TypedDict(
+    "OutputFormatOptionsTypeDef",
+    {
+        "Csv": CsvOutputOptionsTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDataCatalogInputDefinitionOutputTypeDef = TypedDict(
+    "_RequiredDataCatalogInputDefinitionOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+    },
+)
+_OptionalDataCatalogInputDefinitionOutputTypeDef = TypedDict(
+    "_OptionalDataCatalogInputDefinitionOutputTypeDef",
+    {
+        "CatalogId": str,
+        "TempDirectory": S3LocationOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class DataCatalogInputDefinitionOutputTypeDef(
+    _RequiredDataCatalogInputDefinitionOutputTypeDef,
+    _OptionalDataCatalogInputDefinitionOutputTypeDef,
+):
+    pass
+
+
+_RequiredDatabaseInputDefinitionOutputTypeDef = TypedDict(
+    "_RequiredDatabaseInputDefinitionOutputTypeDef",
+    {
+        "GlueConnectionName": str,
+    },
+)
+_OptionalDatabaseInputDefinitionOutputTypeDef = TypedDict(
+    "_OptionalDatabaseInputDefinitionOutputTypeDef",
+    {
+        "DatabaseTableName": str,
+        "TempDirectory": S3LocationOutputTypeDef,
+        "QueryString": str,
+    },
+    total=False,
+)
+
+
+class DatabaseInputDefinitionOutputTypeDef(
+    _RequiredDatabaseInputDefinitionOutputTypeDef, _OptionalDatabaseInputDefinitionOutputTypeDef
+):
+    pass
+
+
+_RequiredDatabaseTableOutputOptionsOutputTypeDef = TypedDict(
+    "_RequiredDatabaseTableOutputOptionsOutputTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalDatabaseTableOutputOptionsOutputTypeDef = TypedDict(
+    "_OptionalDatabaseTableOutputOptionsOutputTypeDef",
+    {
+        "TempDirectory": S3LocationOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class DatabaseTableOutputOptionsOutputTypeDef(
+    _RequiredDatabaseTableOutputOptionsOutputTypeDef,
+    _OptionalDatabaseTableOutputOptionsOutputTypeDef,
+):
+    pass
+
+
+S3TableOutputOptionsOutputTypeDef = TypedDict(
+    "S3TableOutputOptionsOutputTypeDef",
+    {
+        "Location": S3LocationOutputTypeDef,
+    },
+)
+
+_RequiredDatasetParameterOutputTypeDef = TypedDict(
+    "_RequiredDatasetParameterOutputTypeDef",
+    {
+        "Name": str,
+        "Type": ParameterTypeType,
+    },
+)
+_OptionalDatasetParameterOutputTypeDef = TypedDict(
+    "_OptionalDatasetParameterOutputTypeDef",
+    {
+        "DatetimeOptions": DatetimeOptionsOutputTypeDef,
+        "CreateColumn": bool,
+        "Filter": FilterExpressionOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class DatasetParameterOutputTypeDef(
+    _RequiredDatasetParameterOutputTypeDef, _OptionalDatasetParameterOutputTypeDef
+):
+    pass
+
+
+_RequiredDatasetParameterTypeDef = TypedDict(
+    "_RequiredDatasetParameterTypeDef",
+    {
+        "Name": str,
+        "Type": ParameterTypeType,
+    },
+)
+_OptionalDatasetParameterTypeDef = TypedDict(
+    "_OptionalDatasetParameterTypeDef",
+    {
+        "DatetimeOptions": DatetimeOptionsTypeDef,
+        "CreateColumn": bool,
+        "Filter": FilterExpressionTypeDef,
+    },
+    total=False,
+)
+
+
+class DatasetParameterTypeDef(_RequiredDatasetParameterTypeDef, _OptionalDatasetParameterTypeDef):
+    pass
+
+
 DescribeProjectResponseTypeDef = TypedDict(
     "DescribeProjectResponseTypeDef",
     {
         "CreateDate": datetime,
         "CreatedBy": str,
         "DatasetName": str,
         "LastModifiedDate": datetime,
         "LastModifiedBy": str,
         "Name": str,
         "RecipeName": str,
         "ResourceArn": str,
-        "Sample": SampleTypeDef,
+        "Sample": SampleOutputTypeDef,
         "RoleArn": str,
         "Tags": Dict[str, str],
         "SessionStatus": SessionStatusType,
         "OpenedBy": str,
         "OpenDate": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1343,74 +1882,38 @@
         "AccountId": str,
         "CreateDate": datetime,
         "CreatedBy": str,
         "DatasetName": str,
         "LastModifiedDate": datetime,
         "LastModifiedBy": str,
         "ResourceArn": str,
-        "Sample": SampleTypeDef,
+        "Sample": SampleOutputTypeDef,
         "Tags": Dict[str, str],
         "RoleArn": str,
         "OpenedBy": str,
         "OpenDate": datetime,
     },
     total=False,
 )
 
-class ProjectTypeDef(_RequiredProjectTypeDef, _OptionalProjectTypeDef):
-    pass
 
-_RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateProjectRequestRequestTypeDef",
-    {
-        "RoleArn": str,
-        "Name": str,
-    },
-)
-_OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateProjectRequestRequestTypeDef",
-    {
-        "Sample": SampleTypeDef,
-    },
-    total=False,
-)
-
-class UpdateProjectRequestRequestTypeDef(
-    _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
-):
+class ProjectTypeDef(_RequiredProjectTypeDef, _OptionalProjectTypeDef):
     pass
 
-OutputFormatOptionsTypeDef = TypedDict(
-    "OutputFormatOptionsTypeDef",
-    {
-        "Csv": CsvOutputOptionsTypeDef,
-    },
-    total=False,
-)
 
-_RequiredDatasetParameterTypeDef = TypedDict(
-    "_RequiredDatasetParameterTypeDef",
+FormatOptionsOutputTypeDef = TypedDict(
+    "FormatOptionsOutputTypeDef",
     {
-        "Name": str,
-        "Type": ParameterTypeType,
-    },
-)
-_OptionalDatasetParameterTypeDef = TypedDict(
-    "_OptionalDatasetParameterTypeDef",
-    {
-        "DatetimeOptions": DatetimeOptionsTypeDef,
-        "CreateColumn": bool,
-        "Filter": FilterExpressionTypeDef,
+        "Json": JsonOptionsOutputTypeDef,
+        "Excel": ExcelOptionsOutputTypeDef,
+        "Csv": CsvOptionsOutputTypeDef,
     },
     total=False,
 )
 
-class DatasetParameterTypeDef(_RequiredDatasetParameterTypeDef, _OptionalDatasetParameterTypeDef):
-    pass
-
 FormatOptionsTypeDef = TypedDict(
     "FormatOptionsTypeDef",
     {
         "Json": JsonOptionsTypeDef,
         "Excel": ExcelOptionsTypeDef,
         "Csv": CsvOptionsTypeDef,
     },
@@ -1431,31 +1934,75 @@
     {
         "Schedules": List[ScheduleTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredRecipeStepOutputTypeDef = TypedDict(
+    "_RequiredRecipeStepOutputTypeDef",
+    {
+        "Action": RecipeActionOutputTypeDef,
+    },
+)
+_OptionalRecipeStepOutputTypeDef = TypedDict(
+    "_OptionalRecipeStepOutputTypeDef",
+    {
+        "ConditionExpressions": List[ConditionExpressionOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class RecipeStepOutputTypeDef(_RequiredRecipeStepOutputTypeDef, _OptionalRecipeStepOutputTypeDef):
+    pass
+
+
 _RequiredRecipeStepTypeDef = TypedDict(
     "_RequiredRecipeStepTypeDef",
     {
         "Action": RecipeActionTypeDef,
     },
 )
 _OptionalRecipeStepTypeDef = TypedDict(
     "_OptionalRecipeStepTypeDef",
     {
         "ConditionExpressions": Sequence[ConditionExpressionTypeDef],
     },
     total=False,
 )
 
+
 class RecipeStepTypeDef(_RequiredRecipeStepTypeDef, _OptionalRecipeStepTypeDef):
     pass
 
+
+_RequiredRuleOutputTypeDef = TypedDict(
+    "_RequiredRuleOutputTypeDef",
+    {
+        "Name": str,
+        "CheckExpression": str,
+    },
+)
+_OptionalRuleOutputTypeDef = TypedDict(
+    "_OptionalRuleOutputTypeDef",
+    {
+        "Disabled": bool,
+        "SubstitutionMap": Dict[str, str],
+        "Threshold": ThresholdOutputTypeDef,
+        "ColumnSelectors": List[ColumnSelectorOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class RuleOutputTypeDef(_RequiredRuleOutputTypeDef, _OptionalRuleOutputTypeDef):
+    pass
+
+
 _RequiredRuleTypeDef = TypedDict(
     "_RequiredRuleTypeDef",
     {
         "Name": str,
         "CheckExpression": str,
     },
 )
@@ -1466,17 +2013,28 @@
         "SubstitutionMap": Mapping[str, str],
         "Threshold": ThresholdTypeDef,
         "ColumnSelectors": Sequence[ColumnSelectorTypeDef],
     },
     total=False,
 )
 
+
 class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
+
+StatisticsConfigurationOutputTypeDef = TypedDict(
+    "StatisticsConfigurationOutputTypeDef",
+    {
+        "IncludedStatistics": List[str],
+        "Overrides": List[StatisticOverrideOutputTypeDef],
+    },
+    total=False,
+)
+
 StatisticsConfigurationTypeDef = TypedDict(
     "StatisticsConfigurationTypeDef",
     {
         "IncludedStatistics": Sequence[str],
         "Overrides": Sequence[StatisticOverrideTypeDef],
     },
     total=False,
@@ -1504,17 +2062,19 @@
     "_OptionalDatabaseOutputTypeDef",
     {
         "DatabaseOutputMode": Literal["NEW_TABLE"],
     },
     total=False,
 )
 
+
 class DatabaseOutputTypeDef(_RequiredDatabaseOutputTypeDef, _OptionalDatabaseOutputTypeDef):
     pass
 
+
 _RequiredDataCatalogOutputTypeDef = TypedDict(
     "_RequiredDataCatalogOutputTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -1525,27 +2085,20 @@
         "S3Options": S3TableOutputOptionsTypeDef,
         "DatabaseOptions": DatabaseTableOutputOptionsTypeDef,
         "Overwrite": bool,
     },
     total=False,
 )
 
+
 class DataCatalogOutputTypeDef(
     _RequiredDataCatalogOutputTypeDef, _OptionalDataCatalogOutputTypeDef
 ):
     pass
 
-ListProjectsResponseTypeDef = TypedDict(
-    "ListProjectsResponseTypeDef",
-    {
-        "Projects": List[ProjectTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredOutputTypeDef = TypedDict(
     "_RequiredOutputTypeDef",
     {
         "Location": S3LocationTypeDef,
     },
 )
@@ -1558,61 +2111,72 @@
         "Overwrite": bool,
         "FormatOptions": OutputFormatOptionsTypeDef,
         "MaxOutputFiles": int,
     },
     total=False,
 )
 
+
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
 
-PathOptionsTypeDef = TypedDict(
-    "PathOptionsTypeDef",
+
+InputOutputTypeDef = TypedDict(
+    "InputOutputTypeDef",
     {
-        "LastModifiedDateCondition": FilterExpressionTypeDef,
-        "FilesLimit": FilesLimitTypeDef,
-        "Parameters": Mapping[str, DatasetParameterTypeDef],
+        "S3InputDefinition": S3LocationOutputTypeDef,
+        "DataCatalogInputDefinition": DataCatalogInputDefinitionOutputTypeDef,
+        "DatabaseInputDefinition": DatabaseInputDefinitionOutputTypeDef,
+        "Metadata": MetadataOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateRecipeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRecipeRequestRequestTypeDef",
+PathOptionsOutputTypeDef = TypedDict(
+    "PathOptionsOutputTypeDef",
     {
-        "Name": str,
-        "Steps": Sequence[RecipeStepTypeDef],
+        "LastModifiedDateCondition": FilterExpressionOutputTypeDef,
+        "FilesLimit": FilesLimitOutputTypeDef,
+        "Parameters": Dict[str, DatasetParameterOutputTypeDef],
     },
+    total=False,
 )
-_OptionalCreateRecipeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRecipeRequestRequestTypeDef",
+
+PathOptionsTypeDef = TypedDict(
+    "PathOptionsTypeDef",
     {
-        "Description": str,
-        "Tags": Mapping[str, str],
+        "LastModifiedDateCondition": FilterExpressionTypeDef,
+        "FilesLimit": FilesLimitTypeDef,
+        "Parameters": Mapping[str, DatasetParameterTypeDef],
     },
     total=False,
 )
 
-class CreateRecipeRequestRequestTypeDef(
-    _RequiredCreateRecipeRequestRequestTypeDef, _OptionalCreateRecipeRequestRequestTypeDef
-):
-    pass
+ListProjectsResponseTypeDef = TypedDict(
+    "ListProjectsResponseTypeDef",
+    {
+        "Projects": List[ProjectTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 DescribeRecipeResponseTypeDef = TypedDict(
     "DescribeRecipeResponseTypeDef",
     {
         "CreatedBy": str,
         "CreateDate": datetime,
         "LastModifiedBy": str,
         "LastModifiedDate": datetime,
         "ProjectName": str,
         "PublishedBy": str,
         "PublishedDate": datetime,
         "Description": str,
         "Name": str,
-        "Steps": List[RecipeStepTypeDef],
+        "Steps": List[RecipeStepOutputTypeDef],
         "Tags": Dict[str, str],
         "ResourceArn": str,
         "RecipeVersion": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1630,24 +2194,49 @@
         "LastModifiedBy": str,
         "LastModifiedDate": datetime,
         "ProjectName": str,
         "PublishedBy": str,
         "PublishedDate": datetime,
         "Description": str,
         "ResourceArn": str,
-        "Steps": List[RecipeStepTypeDef],
+        "Steps": List[RecipeStepOutputTypeDef],
         "Tags": Dict[str, str],
         "RecipeVersion": str,
     },
     total=False,
 )
 
+
 class RecipeTypeDef(_RequiredRecipeTypeDef, _OptionalRecipeTypeDef):
     pass
 
+
+_RequiredCreateRecipeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRecipeRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Steps": Sequence[RecipeStepTypeDef],
+    },
+)
+_OptionalCreateRecipeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRecipeRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateRecipeRequestRequestTypeDef(
+    _RequiredCreateRecipeRequestRequestTypeDef, _OptionalCreateRecipeRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredSendProjectSessionActionRequestRequestTypeDef = TypedDict(
     "_RequiredSendProjectSessionActionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalSendProjectSessionActionRequestRequestTypeDef = TypedDict(
@@ -1658,20 +2247,22 @@
         "StepIndex": int,
         "ClientSessionId": str,
         "ViewFrame": ViewFrameTypeDef,
     },
     total=False,
 )
 
+
 class SendProjectSessionActionRequestRequestTypeDef(
     _RequiredSendProjectSessionActionRequestRequestTypeDef,
     _OptionalSendProjectSessionActionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRecipeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateRecipeRequestRequestTypeDef = TypedDict(
@@ -1679,19 +2270,38 @@
     {
         "Description": str,
         "Steps": Sequence[RecipeStepTypeDef],
     },
     total=False,
 )
 
+
 class UpdateRecipeRequestRequestTypeDef(
     _RequiredUpdateRecipeRequestRequestTypeDef, _OptionalUpdateRecipeRequestRequestTypeDef
 ):
     pass
 
+
+DescribeRulesetResponseTypeDef = TypedDict(
+    "DescribeRulesetResponseTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "TargetArn": str,
+        "Rules": List[RuleOutputTypeDef],
+        "CreateDate": datetime,
+        "CreatedBy": str,
+        "LastModifiedBy": str,
+        "LastModifiedDate": datetime,
+        "ResourceArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateRulesetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRulesetRequestRequestTypeDef",
     {
         "Name": str,
         "TargetArn": str,
         "Rules": Sequence[RuleTypeDef],
     },
@@ -1701,35 +2311,20 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateRulesetRequestRequestTypeDef(
     _RequiredCreateRulesetRequestRequestTypeDef, _OptionalCreateRulesetRequestRequestTypeDef
 ):
     pass
 
-DescribeRulesetResponseTypeDef = TypedDict(
-    "DescribeRulesetResponseTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "TargetArn": str,
-        "Rules": List[RuleTypeDef],
-        "CreateDate": datetime,
-        "CreatedBy": str,
-        "LastModifiedBy": str,
-        "LastModifiedDate": datetime,
-        "ResourceArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateRulesetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRulesetRequestRequestTypeDef",
     {
         "Name": str,
         "Rules": Sequence[RuleTypeDef],
     },
@@ -1738,38 +2333,64 @@
     "_OptionalUpdateRulesetRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateRulesetRequestRequestTypeDef(
     _RequiredUpdateRulesetRequestRequestTypeDef, _OptionalUpdateRulesetRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredColumnStatisticsConfigurationOutputTypeDef = TypedDict(
+    "_RequiredColumnStatisticsConfigurationOutputTypeDef",
+    {
+        "Statistics": StatisticsConfigurationOutputTypeDef,
+    },
+)
+_OptionalColumnStatisticsConfigurationOutputTypeDef = TypedDict(
+    "_OptionalColumnStatisticsConfigurationOutputTypeDef",
+    {
+        "Selectors": List[ColumnSelectorOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class ColumnStatisticsConfigurationOutputTypeDef(
+    _RequiredColumnStatisticsConfigurationOutputTypeDef,
+    _OptionalColumnStatisticsConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredColumnStatisticsConfigurationTypeDef = TypedDict(
     "_RequiredColumnStatisticsConfigurationTypeDef",
     {
         "Statistics": StatisticsConfigurationTypeDef,
     },
 )
 _OptionalColumnStatisticsConfigurationTypeDef = TypedDict(
     "_OptionalColumnStatisticsConfigurationTypeDef",
     {
         "Selectors": Sequence[ColumnSelectorTypeDef],
     },
     total=False,
 )
 
+
 class ColumnStatisticsConfigurationTypeDef(
     _RequiredColumnStatisticsConfigurationTypeDef, _OptionalColumnStatisticsConfigurationTypeDef
 ):
     pass
 
+
 _RequiredCreateRecipeJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRecipeJobRequestRequestTypeDef",
     {
         "Name": str,
         "RoleArn": str,
     },
 )
@@ -1789,19 +2410,21 @@
         "RecipeReference": RecipeReferenceTypeDef,
         "Tags": Mapping[str, str],
         "Timeout": int,
     },
     total=False,
 )
 
+
 class CreateRecipeJobRequestRequestTypeDef(
     _RequiredCreateRecipeJobRequestRequestTypeDef, _OptionalCreateRecipeJobRequestRequestTypeDef
 ):
     pass
 
+
 JobRunTypeDef = TypedDict(
     "JobRunTypeDef",
     {
         "Attempt": int,
         "CompletedOn": datetime,
         "DatasetName": str,
         "ErrorMessage": str,
@@ -1810,19 +2433,19 @@
         "RunId": str,
         "State": JobRunStateType,
         "LogSubscription": LogSubscriptionType,
         "LogGroupName": str,
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
         "DatabaseOutputs": List[DatabaseOutputTypeDef],
-        "RecipeReference": RecipeReferenceTypeDef,
+        "RecipeReference": RecipeReferenceOutputTypeDef,
         "StartedBy": str,
         "StartedOn": datetime,
-        "JobSample": JobSampleTypeDef,
-        "ValidationConfigurations": List[ValidationConfigurationTypeDef],
+        "JobSample": JobSampleOutputTypeDef,
+        "ValidationConfigurations": List[ValidationConfigurationOutputTypeDef],
     },
     total=False,
 )
 
 _RequiredJobTypeDef = TypedDict(
     "_RequiredJobTypeDef",
     {
@@ -1844,28 +2467,30 @@
         "LogSubscription": LogSubscriptionType,
         "MaxCapacity": int,
         "MaxRetries": int,
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
         "DatabaseOutputs": List[DatabaseOutputTypeDef],
         "ProjectName": str,
-        "RecipeReference": RecipeReferenceTypeDef,
+        "RecipeReference": RecipeReferenceOutputTypeDef,
         "ResourceArn": str,
         "RoleArn": str,
         "Timeout": int,
         "Tags": Dict[str, str],
-        "JobSample": JobSampleTypeDef,
-        "ValidationConfigurations": List[ValidationConfigurationTypeDef],
+        "JobSample": JobSampleOutputTypeDef,
+        "ValidationConfigurations": List[ValidationConfigurationOutputTypeDef],
     },
     total=False,
 )
 
+
 class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
     pass
 
+
 _RequiredUpdateRecipeJobRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRecipeJobRequestRequestTypeDef",
     {
         "Name": str,
         "RoleArn": str,
     },
 )
@@ -1881,89 +2506,95 @@
         "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
         "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
         "Timeout": int,
     },
     total=False,
 )
 
+
 class UpdateRecipeJobRequestRequestTypeDef(
     _RequiredUpdateRecipeJobRequestRequestTypeDef, _OptionalUpdateRecipeJobRequestRequestTypeDef
 ):
     pass
 
-_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Input": InputTypeDef,
-    },
-)
-_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetRequestRequestTypeDef",
-    {
-        "Format": InputFormatType,
-        "FormatOptions": FormatOptionsTypeDef,
-        "PathOptions": PathOptionsTypeDef,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateDatasetRequestRequestTypeDef(
-    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
-):
-    pass
 
 _RequiredDatasetTypeDef = TypedDict(
     "_RequiredDatasetTypeDef",
     {
         "Name": str,
-        "Input": InputTypeDef,
+        "Input": InputOutputTypeDef,
     },
 )
 _OptionalDatasetTypeDef = TypedDict(
     "_OptionalDatasetTypeDef",
     {
         "AccountId": str,
         "CreatedBy": str,
         "CreateDate": datetime,
         "Format": InputFormatType,
-        "FormatOptions": FormatOptionsTypeDef,
+        "FormatOptions": FormatOptionsOutputTypeDef,
         "LastModifiedDate": datetime,
         "LastModifiedBy": str,
         "Source": SourceType,
-        "PathOptions": PathOptionsTypeDef,
+        "PathOptions": PathOptionsOutputTypeDef,
         "Tags": Dict[str, str],
         "ResourceArn": str,
     },
     total=False,
 )
 
+
 class DatasetTypeDef(_RequiredDatasetTypeDef, _OptionalDatasetTypeDef):
     pass
 
+
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "CreatedBy": str,
         "CreateDate": datetime,
         "Name": str,
         "Format": InputFormatType,
-        "FormatOptions": FormatOptionsTypeDef,
-        "Input": InputTypeDef,
+        "FormatOptions": FormatOptionsOutputTypeDef,
+        "Input": InputOutputTypeDef,
         "LastModifiedDate": datetime,
         "LastModifiedBy": str,
         "Source": SourceType,
-        "PathOptions": PathOptionsTypeDef,
+        "PathOptions": PathOptionsOutputTypeDef,
         "Tags": Dict[str, str],
         "ResourceArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Input": InputTypeDef,
+    },
+)
+_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetRequestRequestTypeDef",
+    {
+        "Format": InputFormatType,
+        "FormatOptions": FormatOptionsTypeDef,
+        "PathOptions": PathOptionsTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateDatasetRequestRequestTypeDef(
+    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "Name": str,
         "Input": InputTypeDef,
     },
 )
@@ -1973,19 +2604,21 @@
         "Format": InputFormatType,
         "FormatOptions": FormatOptionsTypeDef,
         "PathOptions": PathOptionsTypeDef,
     },
     total=False,
 )
 
+
 class UpdateDatasetRequestRequestTypeDef(
     _RequiredUpdateDatasetRequestRequestTypeDef, _OptionalUpdateDatasetRequestRequestTypeDef
 ):
     pass
 
+
 ListRecipeVersionsResponseTypeDef = TypedDict(
     "ListRecipeVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Recipes": List[RecipeTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1996,14 +2629,25 @@
     {
         "Recipes": List[RecipeTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ProfileConfigurationOutputTypeDef = TypedDict(
+    "ProfileConfigurationOutputTypeDef",
+    {
+        "DatasetStatisticsConfiguration": StatisticsConfigurationOutputTypeDef,
+        "ProfileColumns": List[ColumnSelectorOutputTypeDef],
+        "ColumnStatisticsConfigurations": List[ColumnStatisticsConfigurationOutputTypeDef],
+        "EntityDetectorConfiguration": EntityDetectorConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ProfileConfigurationTypeDef = TypedDict(
     "ProfileConfigurationTypeDef",
     {
         "DatasetStatisticsConfiguration": StatisticsConfigurationTypeDef,
         "ProfileColumns": Sequence[ColumnSelectorTypeDef],
         "ColumnStatisticsConfigurations": Sequence[ColumnStatisticsConfigurationTypeDef],
         "EntityDetectorConfiguration": EntityDetectorConfigurationTypeDef,
@@ -2034,45 +2678,14 @@
     {
         "Datasets": List[DatasetTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateProfileJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProfileJobRequestRequestTypeDef",
-    {
-        "DatasetName": str,
-        "Name": str,
-        "OutputLocation": S3LocationTypeDef,
-        "RoleArn": str,
-    },
-)
-_OptionalCreateProfileJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProfileJobRequestRequestTypeDef",
-    {
-        "EncryptionKeyArn": str,
-        "EncryptionMode": EncryptionModeType,
-        "LogSubscription": LogSubscriptionType,
-        "MaxCapacity": int,
-        "MaxRetries": int,
-        "Configuration": ProfileConfigurationTypeDef,
-        "ValidationConfigurations": Sequence[ValidationConfigurationTypeDef],
-        "Tags": Mapping[str, str],
-        "Timeout": int,
-        "JobSample": JobSampleTypeDef,
-    },
-    total=False,
-)
-
-class CreateProfileJobRequestRequestTypeDef(
-    _RequiredCreateProfileJobRequestRequestTypeDef, _OptionalCreateProfileJobRequestRequestTypeDef
-):
-    pass
-
 DescribeJobResponseTypeDef = TypedDict(
     "DescribeJobResponseTypeDef",
     {
         "CreateDate": datetime,
         "CreatedBy": str,
         "DatasetName": str,
         "EncryptionKeyArn": str,
@@ -2084,52 +2697,85 @@
         "LogSubscription": LogSubscriptionType,
         "MaxCapacity": int,
         "MaxRetries": int,
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
         "DatabaseOutputs": List[DatabaseOutputTypeDef],
         "ProjectName": str,
-        "ProfileConfiguration": ProfileConfigurationTypeDef,
-        "ValidationConfigurations": List[ValidationConfigurationTypeDef],
-        "RecipeReference": RecipeReferenceTypeDef,
+        "ProfileConfiguration": ProfileConfigurationOutputTypeDef,
+        "ValidationConfigurations": List[ValidationConfigurationOutputTypeDef],
+        "RecipeReference": RecipeReferenceOutputTypeDef,
         "ResourceArn": str,
         "RoleArn": str,
         "Tags": Dict[str, str],
         "Timeout": int,
-        "JobSample": JobSampleTypeDef,
+        "JobSample": JobSampleOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeJobRunResponseTypeDef = TypedDict(
     "DescribeJobRunResponseTypeDef",
     {
         "Attempt": int,
         "CompletedOn": datetime,
         "DatasetName": str,
         "ErrorMessage": str,
         "ExecutionTime": int,
         "JobName": str,
-        "ProfileConfiguration": ProfileConfigurationTypeDef,
-        "ValidationConfigurations": List[ValidationConfigurationTypeDef],
+        "ProfileConfiguration": ProfileConfigurationOutputTypeDef,
+        "ValidationConfigurations": List[ValidationConfigurationOutputTypeDef],
         "RunId": str,
         "State": JobRunStateType,
         "LogSubscription": LogSubscriptionType,
         "LogGroupName": str,
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
         "DatabaseOutputs": List[DatabaseOutputTypeDef],
-        "RecipeReference": RecipeReferenceTypeDef,
+        "RecipeReference": RecipeReferenceOutputTypeDef,
         "StartedBy": str,
         "StartedOn": datetime,
-        "JobSample": JobSampleTypeDef,
+        "JobSample": JobSampleOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCreateProfileJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProfileJobRequestRequestTypeDef",
+    {
+        "DatasetName": str,
+        "Name": str,
+        "OutputLocation": S3LocationTypeDef,
+        "RoleArn": str,
+    },
+)
+_OptionalCreateProfileJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProfileJobRequestRequestTypeDef",
+    {
+        "EncryptionKeyArn": str,
+        "EncryptionMode": EncryptionModeType,
+        "LogSubscription": LogSubscriptionType,
+        "MaxCapacity": int,
+        "MaxRetries": int,
+        "Configuration": ProfileConfigurationTypeDef,
+        "ValidationConfigurations": Sequence[ValidationConfigurationTypeDef],
+        "Tags": Mapping[str, str],
+        "Timeout": int,
+        "JobSample": JobSampleTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateProfileJobRequestRequestTypeDef(
+    _RequiredCreateProfileJobRequestRequestTypeDef, _OptionalCreateProfileJobRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredUpdateProfileJobRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProfileJobRequestRequestTypeDef",
     {
         "Name": str,
         "OutputLocation": S3LocationTypeDef,
         "RoleArn": str,
     },
@@ -2146,11 +2792,12 @@
         "ValidationConfigurations": Sequence[ValidationConfigurationTypeDef],
         "Timeout": int,
         "JobSample": JobSampleTypeDef,
     },
     total=False,
 )
 
+
 class UpdateProfileJobRequestRequestTypeDef(
     _RequiredUpdateProfileJobRequestRequestTypeDef, _OptionalUpdateProfileJobRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-databrew-1.28.0/mypy_boto3_databrew.egg-info/PKG-INFO` & `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-databrew
-Version: 1.28.0
-Summary: Type annotations for boto3.GlueDataBrew 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.GlueDataBrew 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-databrew"></a>
 
 # mypy-boto3-databrew
 
 [![PyPI - mypy-boto3-databrew](https://img.shields.io/pypi/v/mypy-boto3-databrew.svg?color=blue)](https://pypi.org/project/mypy-boto3-databrew)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-databrew.svg?color=blue)](https://pypi.org/project/mypy-boto3-databrew)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-databrew?color=blue)](https://pypistats.org/packages/mypy-boto3-databrew)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-databrew)](https://pepy.tech/project/mypy-boto3-databrew)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GlueDataBrew 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
+[boto3.GlueDataBrew 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
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
 [mypy-boto3-databrew docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/).
 
 See how it helps to find and fix potential bugs:
 
@@ -362,34 +362,42 @@
 ### Typed dictionaries
 
 `mypy_boto3_databrew.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_databrew.type_defs import (
+    AllowedStatisticsOutputTypeDef,
     AllowedStatisticsTypeDef,
     BatchDeleteRecipeVersionRequestRequestTypeDef,
     RecipeVersionErrorDetailTypeDef,
+    ColumnSelectorOutputTypeDef,
     ColumnSelectorTypeDef,
+    ConditionExpressionOutputTypeDef,
     ConditionExpressionTypeDef,
     CreateDatasetResponseTypeDef,
     JobSampleTypeDef,
     S3LocationTypeDef,
     ValidationConfigurationTypeDef,
     CreateProfileJobResponseTypeDef,
     SampleTypeDef,
     CreateProjectResponseTypeDef,
     RecipeReferenceTypeDef,
     CreateRecipeJobResponseTypeDef,
     CreateRecipeResponseTypeDef,
     CreateRulesetResponseTypeDef,
     CreateScheduleRequestRequestTypeDef,
     CreateScheduleResponseTypeDef,
+    CsvOptionsOutputTypeDef,
     CsvOptionsTypeDef,
+    CsvOutputOptionsOutputTypeDef,
     CsvOutputOptionsTypeDef,
+    S3LocationOutputTypeDef,
+    DatetimeOptionsOutputTypeDef,
+    FilterExpressionOutputTypeDef,
     DatetimeOptionsTypeDef,
     FilterExpressionTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteDatasetResponseTypeDef,
     DeleteJobRequestRequestTypeDef,
     DeleteJobResponseTypeDef,
     DeleteProjectRequestRequestTypeDef,
@@ -398,23 +406,31 @@
     DeleteRecipeVersionResponseTypeDef,
     DeleteRulesetRequestRequestTypeDef,
     DeleteRulesetResponseTypeDef,
     DeleteScheduleRequestRequestTypeDef,
     DeleteScheduleResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
+    JobSampleOutputTypeDef,
+    RecipeReferenceOutputTypeDef,
+    ValidationConfigurationOutputTypeDef,
     DescribeJobRunRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
+    SampleOutputTypeDef,
     DescribeRecipeRequestRequestTypeDef,
     DescribeRulesetRequestRequestTypeDef,
     DescribeScheduleRequestRequestTypeDef,
     DescribeScheduleResponseTypeDef,
+    ExcelOptionsOutputTypeDef,
     ExcelOptionsTypeDef,
+    FilesLimitOutputTypeDef,
     FilesLimitTypeDef,
+    JsonOptionsOutputTypeDef,
     JsonOptionsTypeDef,
+    MetadataOutputTypeDef,
     MetadataTypeDef,
     ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
@@ -431,91 +447,109 @@
     ListSchedulesRequestRequestTypeDef,
     ScheduleTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     PublishRecipeRequestRequestTypeDef,
     PublishRecipeResponseTypeDef,
+    RecipeActionOutputTypeDef,
     RecipeActionTypeDef,
     ResponseMetadataTypeDef,
+    ThresholdOutputTypeDef,
     ThresholdTypeDef,
     ViewFrameTypeDef,
     SendProjectSessionActionResponseTypeDef,
     StartJobRunRequestRequestTypeDef,
     StartJobRunResponseTypeDef,
     StartProjectSessionRequestRequestTypeDef,
     StartProjectSessionResponseTypeDef,
+    StatisticOverrideOutputTypeDef,
     StatisticOverrideTypeDef,
     StopJobRunRequestRequestTypeDef,
     StopJobRunResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetResponseTypeDef,
     UpdateProfileJobResponseTypeDef,
     UpdateProjectResponseTypeDef,
     UpdateRecipeJobResponseTypeDef,
     UpdateRecipeResponseTypeDef,
     UpdateRulesetResponseTypeDef,
     UpdateScheduleRequestRequestTypeDef,
     UpdateScheduleResponseTypeDef,
+    EntityDetectorConfigurationOutputTypeDef,
     EntityDetectorConfigurationTypeDef,
     BatchDeleteRecipeVersionResponseTypeDef,
     DataCatalogInputDefinitionTypeDef,
     DatabaseInputDefinitionTypeDef,
     DatabaseTableOutputOptionsTypeDef,
     S3TableOutputOptionsTypeDef,
     CreateProjectRequestRequestTypeDef,
-    DescribeProjectResponseTypeDef,
-    ProjectTypeDef,
     UpdateProjectRequestRequestTypeDef,
+    OutputFormatOptionsOutputTypeDef,
     OutputFormatOptionsTypeDef,
+    DataCatalogInputDefinitionOutputTypeDef,
+    DatabaseInputDefinitionOutputTypeDef,
+    DatabaseTableOutputOptionsOutputTypeDef,
+    S3TableOutputOptionsOutputTypeDef,
+    DatasetParameterOutputTypeDef,
     DatasetParameterTypeDef,
+    DescribeProjectResponseTypeDef,
+    ProjectTypeDef,
+    FormatOptionsOutputTypeDef,
     FormatOptionsTypeDef,
     ListRulesetsResponseTypeDef,
     ListSchedulesResponseTypeDef,
+    RecipeStepOutputTypeDef,
     RecipeStepTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
+    StatisticsConfigurationOutputTypeDef,
     StatisticsConfigurationTypeDef,
     InputTypeDef,
     DatabaseOutputTypeDef,
     DataCatalogOutputTypeDef,
-    ListProjectsResponseTypeDef,
     OutputTypeDef,
+    InputOutputTypeDef,
+    PathOptionsOutputTypeDef,
     PathOptionsTypeDef,
-    CreateRecipeRequestRequestTypeDef,
+    ListProjectsResponseTypeDef,
     DescribeRecipeResponseTypeDef,
     RecipeTypeDef,
+    CreateRecipeRequestRequestTypeDef,
     SendProjectSessionActionRequestRequestTypeDef,
     UpdateRecipeRequestRequestTypeDef,
-    CreateRulesetRequestRequestTypeDef,
     DescribeRulesetResponseTypeDef,
+    CreateRulesetRequestRequestTypeDef,
     UpdateRulesetRequestRequestTypeDef,
+    ColumnStatisticsConfigurationOutputTypeDef,
     ColumnStatisticsConfigurationTypeDef,
     CreateRecipeJobRequestRequestTypeDef,
     JobRunTypeDef,
     JobTypeDef,
     UpdateRecipeJobRequestRequestTypeDef,
-    CreateDatasetRequestRequestTypeDef,
     DatasetTypeDef,
     DescribeDatasetResponseTypeDef,
+    CreateDatasetRequestRequestTypeDef,
     UpdateDatasetRequestRequestTypeDef,
     ListRecipeVersionsResponseTypeDef,
     ListRecipesResponseTypeDef,
+    ProfileConfigurationOutputTypeDef,
     ProfileConfigurationTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobsResponseTypeDef,
     ListDatasetsResponseTypeDef,
-    CreateProfileJobRequestRequestTypeDef,
     DescribeJobResponseTypeDef,
     DescribeJobRunResponseTypeDef,
+    CreateProfileJobRequestRequestTypeDef,
     UpdateProfileJobRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AllowedStatisticsTypeDef:
+def get_structure() -> AllowedStatisticsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-databrew-1.28.0/mypy_boto3_databrew.egg-info/SOURCES.txt` & `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.0/setup.py` & `mypy-boto3-databrew-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-databrew",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_databrew"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GlueDataBrew 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.GlueDataBrew 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

